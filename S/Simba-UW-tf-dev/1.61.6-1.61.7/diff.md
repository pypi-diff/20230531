# Comparing `tmp/Simba-UW-tf-dev-1.61.6.tar.gz` & `tmp/Simba-UW-tf-dev-1.61.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.61.6.tar", last modified: Mon May 29 21:41:15 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.61.7.tar", last modified: Wed May 31 13:33:14 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.61.6.tar` & `Simba-UW-tf-dev-1.61.7.tar`

### file list

```diff
@@ -1,507 +1,508 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-23 17:02:30.000000 Simba-UW-tf-dev-1.61.6/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.61.6/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.61.6/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.6/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.61.6/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.6/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.6/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.61.6/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.61.6/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.61.6/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.61.6/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.61.6/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.6/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-29 21:05:41.000000 Simba-UW-tf-dev-1.61.6/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.61.6/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42902 2023-05-25 18:14:02.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    33507 2023-05-25 18:37:00.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1118 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9144 2023-05-28 17:30:45.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-25 14:55:02.000000 Simba-UW-tf-dev-1.61.6/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18514 2023-05-29 20:20:16.000000 Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.61.6/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20973 2023-05-25 13:55:35.000000 Simba-UW-tf-dev-1.61.6/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.6/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.6/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.61.6/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.61.6/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.61.6/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.61.6/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.61.6/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.61.6/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.61.6/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.6/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.6/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.6/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.61.6/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    13770 2023-05-23 16:26:11.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9274 2023-05-23 16:26:19.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.6/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.61.6/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.61.6/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.61.6/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.6/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.6/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.61.6/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.61.6/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.61.6/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.6/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.6/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.61.6/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.61.6/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.6/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.61.6/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.61.6/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.61.6/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8176 2023-05-25 14:24:49.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    65549 2023-05-25 18:24:18.000000 Simba-UW-tf-dev-1.61.6/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.61.6/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.61.6/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.61.6/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.61.6/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.61.6/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.61.6/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.61.6/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.6/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-29 21:41:14.000000 Simba-UW-tf-dev-1.61.6/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    18654 2023-05-29 21:41:14.000000 Simba-UW-tf-dev-1.61.6/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-29 21:41:14.000000 Simba-UW-tf-dev-1.61.6/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-29 21:41:14.000000 Simba-UW-tf-dev-1.61.6/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-05-29 21:41:14.000000 Simba-UW-tf-dev-1.61.6/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-29 21:41:14.000000 Simba-UW-tf-dev-1.61.6/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.61.6/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.61.6/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.61.6/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.6/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.61.6/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.61.6/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.61.6/tests/test_featurizers.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.6/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/tests/data/test_projects/two_c57/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.6/tests/data/test_projects/two_c57/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.6/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.6/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.6/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.61.6/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.61.6/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.61.6/tests/test_thirdparty_appenders.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.61.6/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.61.6/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-29 21:41:14.000000 Simba-UW-tf-dev-1.61.6/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-29 21:41:15.000000 Simba-UW-tf-dev-1.61.6/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-30 12:37:26.000000 Simba-UW-tf-dev-1.61.7/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.61.7/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.61.7/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.7/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.61.7/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.7/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.7/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.61.7/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.61.7/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.61.7/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.61.7/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.61.7/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.7/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-29 21:05:41.000000 Simba-UW-tf-dev-1.61.7/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8457 2023-05-30 20:48:53.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.61.7/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42902 2023-05-25 18:14:02.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    33507 2023-05-25 18:37:00.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1118 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9144 2023-05-28 17:30:45.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    67192 2023-05-31 13:29:28.000000 Simba-UW-tf-dev-1.61.7/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18514 2023-05-29 20:20:16.000000 Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.61.7/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20973 2023-05-25 13:55:35.000000 Simba-UW-tf-dev-1.61.7/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.7/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.7/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.61.7/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.61.7/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.61.7/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.61.7/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.61.7/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.61.7/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.61.7/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.7/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.7/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.7/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.61.7/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    13770 2023-05-23 16:26:11.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9274 2023-05-23 16:26:19.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.7/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.61.7/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19101 2023-05-30 20:48:53.000000 Simba-UW-tf-dev-1.61.7/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.61.7/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.7/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18879 2023-05-31 13:33:07.000000 Simba-UW-tf-dev-1.61.7/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.61.7/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.61.7/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.61.7/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.7/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.7/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.61.7/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.61.7/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.7/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.61.7/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.61.7/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.61.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8176 2023-05-25 14:24:49.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    65549 2023-05-25 18:24:18.000000 Simba-UW-tf-dev-1.61.7/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.61.7/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.61.7/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.61.7/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.61.7/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.61.7/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.61.7/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.61.7/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.7/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-31 13:33:13.000000 Simba-UW-tf-dev-1.61.7/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    18699 2023-05-31 13:33:13.000000 Simba-UW-tf-dev-1.61.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-31 13:33:13.000000 Simba-UW-tf-dev-1.61.7/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-31 13:33:13.000000 Simba-UW-tf-dev-1.61.7/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-05-31 13:33:13.000000 Simba-UW-tf-dev-1.61.7/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-31 13:33:13.000000 Simba-UW-tf-dev-1.61.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.61.7/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.61.7/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.61.7/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.7/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.61.7/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.61.7/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.61.7/tests/test_featurizers.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.7/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/tests/data/test_projects/two_c57/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.7/tests/data/test_projects/two_c57/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.7/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.7/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.7/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.61.7/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.61.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.61.7/tests/test_thirdparty_appenders.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.61.7/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.61.7/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-31 13:33:07.000000 Simba-UW-tf-dev-1.61.7/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-31 13:33:14.000000 Simba-UW-tf-dev-1.61.7/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.61.6/PKG-INFO` & `Simba-UW-tf-dev-1.61.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.61.6
+Version: 1.61.7
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/video_processors/.DS_Store`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 000c  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
 00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
 00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,141 +250,141 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 000c 0000 000b  ................
+00001000: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0000 de4d 0000 000b 005f 005f 0070  .....M....._._.p
-00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 c442 b1c2  moDDblob.....B..
-00001060: 760e c541 0000 000b 005f 005f 0070 0079  v..A....._._.p.y
-00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 ed9b b6f1 cc0c  dDblob..........
-00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
-000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0001 1000 0000 0007  comp............
-000010c0: 0070 006f 0070 005f 0075 0070 0073 6277  .p.o.p._.u.p.sbw
-000010d0: 7370 626c 6f62 0000 00ca 6270 6c69 7374  spblob....bplist
-000010e0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
-000010f0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-00001100: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
-00001110: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-00001120: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-00001130: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-00001140: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00001150: 6261 7208 0809 0809 5f10 197b 7b33 3333  bar....._..{{333
-00001160: 2c20 3132 387d 2c20 7b31 3037 362c 2036  , 128}, {1076, 6
-00001170: 3231 7d7d 0908 1725 313d 4960 6d79 7a7b  21}}...%1=I`myz{
-00001180: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
-00001190: 0000 000f 0000 0000 0000 0000 0000 0000  ................
-000011a0: 0000 009b 0000 0007 0070 006f 0070 005f  .........p.o.p._
-000011b0: 0075 0070 0073 6c67 3153 636f 6d70 0000  .u.p.slg1Scomp..
-000011c0: 0000 0007 3ca2 0000 0007 0070 006f 0070  ....<......p.o.p
-000011d0: 005f 0075 0070 0073 6c73 7643 626c 6f62  ._.u.p.slsvCblob
-000011e0: 0000 02bb 6270 6c69 7374 3030 da01 0203  ....bplist00....
-000011f0: 0405 0607 0809 0a0b 0c0d 1848 494a 4b0c  ...........HIJK.
-00001200: 4d58 6963 6f6e 5369 7a65 5f10 0f73 686f  MXiconSize_..sho
-00001210: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-00001220: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-00001230: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
-00001240: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
-00001250: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
-00001260: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
-00001270: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-00001280: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-00001290: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-000012a0: 0009 ab0e 171c 2125 2a2f 3439 3e43 d40f  ......!%*/49>C..
-000012b0: 1011 1213 140c 0c5a 6964 656e 7469 6669  .......Zidentifi
-000012c0: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
-000012d0: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
-000012e0: 01c7 0909 d412 1011 0f18 1918 1b08 1023  ...............#
-000012f0: 0858 7562 6971 7569 7479 d40f 1011 121d  .Xubiquity......
-00001300: 1e18 0c5c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
-00001310: 10b5 0809 d40f 1011 1222 1e18 185b 6461  ........."...[da
-00001320: 7465 4372 6561 7465 6408 08d4 0f10 1112  teCreated.......
-00001330: 2627 180c 5473 697a 6510 6108 09d4 0f10  &'..Tsize.a.....
-00001340: 1112 2b2c 0c0c 546b 696e 6410 7309 09d4  ..+,..Tkind.s...
-00001350: 0f10 1112 3031 0c18 556c 6162 656c 1064  ....01..Ulabel.d
-00001360: 0908 d40f 1011 1235 360c 1857 7665 7273  .......56..Wvers
-00001370: 696f 6e10 4b09 08d4 0f10 1112 3a3b 0c18  ion.K.......:;..
-00001380: 5863 6f6d 6d65 6e74 7311 012c 0908 d40f  Xcomments..,....
-00001390: 1011 123f 4018 185e 6461 7465 4c61 7374  ...?@..^dateLast
-000013a0: 4f70 656e 6564 10c8 0808 d412 1011 0f18  Opened..........
-000013b0: 1e18 4608 0859 6461 7465 4164 6465 6408  ..F..YdateAdded.
-000013c0: 2340 73a0 0000 0000 0023 4028 0000 0000  #@s......#@(....
-000013d0: 0000 2300 0000 0000 0000 0054 6e61 6d65  ..#........Tname
-000013e0: 0910 0100 0800 1d00 2600 3800 4000 5400  ........&.8.@.T.
-000013f0: 6600 6f00 8100 8c00 9f00 b400 bd00 be00  f.o.............
-00001400: ca00 d300 de00 e400 ee00 f600 fb00 fe00  ................
-00001410: ff01 0001 0901 0a01 0c01 0d01 1601 1f01  ................
-00001420: 2c01 2e01 2f01 3001 3901 4501 4601 4701  ,.../.0.9.E.F.G.
-00001430: 5001 5501 5701 5801 5901 6201 6701 6901  P.U.W.X.Y.b.g.i.
-00001440: 6a01 6b01 7401 7a01 7c01 7d01 7e01 8701  j.k.t.z.|.}.~...
-00001450: 8f01 9101 9201 9301 9c01 a501 a801 a901  ................
-00001460: aa01 b301 c201 c401 c501 c601 cf01 d001  ................
-00001470: d101 db01 dc01 e501 ee01 f701 fc01 fd00  ................
-00001480: 0000 0000 0002 0100 0000 0000 0000 4e00  ..............N.
-00001490: 0000 0000 0000 0000 0000 0000 0001 ff00  ................
-000014a0: 0000 0700 7000 6f00 7000 5f00 7500 7000  ....p.o.p._.u.p.
-000014b0: 736c 7376 7062 6c6f 6200 0002 a062 706c  slsvpblob....bpl
-000014c0: 6973 7430 30da 0102 0304 0506 0708 090a  ist00...........
-000014d0: 0b0c 0d1c 4849 4a4b 0c29 5869 636f 6e53  ....HIJK.)XiconS
-000014e0: 697a 655f 100f 7368 6f77 4963 6f6e 5072  ize_..showIconPr
-000014f0: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00001500: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00001510: 735f 100f 7363 726f 6c6c 506f 7369 7469  s_..scrollPositi
-00001520: 6f6e 5958 7465 7874 5369 7a65 5f10 0f73  onYXtextSize_..s
-00001530: 6372 6f6c 6c50 6f73 6974 696f 6e58 5a73  crollPositionXZs
-00001540: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
-00001550: 656c 6174 6976 6544 6174 6573 5f10 1276  elativeDates_..v
-00001560: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-00001570: 6e23 4030 0000 0000 0000 09d9 0e0f 1011  n#@0............
-00001580: 1213 1415 1617 2025 2a2e 3338 3d42 5863  ...... %*.38=BXc
-00001590: 6f6d 6d65 6e74 735e 6461 7465 4c61 7374  omments^dateLast
-000015a0: 4f70 656e 6564 5c64 6174 654d 6f64 6966  Opened\dateModif
-000015b0: 6965 645b 6461 7465 4372 6561 7465 6454  ied[dateCreatedT
-000015c0: 7369 7a65 556c 6162 656c 546b 696e 6457  sizeUlabelTkindW
-000015d0: 7665 7273 696f 6e54 6e61 6d65 d418 191a  versionTname....
-000015e0: 1b1c 1d0c 1f57 7669 7369 626c 6555 7769  .....WvisibleUwi
-000015f0: 6474 6859 6173 6365 6e64 696e 6755 696e  dthYascendingUin
-00001600: 6465 7808 1101 2c09 1007 d418 191a 1b1c  dex...,.........
-00001610: 221c 2408 10c8 0810 08d4 1819 1a1b 0c27  ".$............'
-00001620: 1c29 0910 b508 1001 d418 191a 1b1c 271c  .)............'.
-00001630: 2d08 0810 02d4 1819 1a1b 0c30 1c32 0910  -..........0.2..
-00001640: 6108 1003 d418 191a 1b1c 350c 3708 1064  a.........5.7..d
-00001650: 0910 05d4 1819 1a1b 0c3a 0c3c 0910 7309  .........:.<..s.
-00001660: 1004 d418 191a 1b1c 3f0c 4108 104b 0910  ........?.A..K..
-00001670: 06d4 1819 1a1b 0c44 0c46 0911 01c7 0910  .......D.F......
-00001680: 0008 2340 73a0 0000 0000 0023 4028 0000  ..#@s......#@(..
-00001690: 0000 0000 2300 0000 0000 0000 0054 6e61  ....#........Tna
-000016a0: 6d65 0900 0800 1d00 2600 3800 4000 5400  me......&.8.@.T.
-000016b0: 6600 6f00 8100 8c00 9f00 b400 bd00 be00  f.o.............
-000016c0: d100 da00 e900 f601 0201 0701 0d01 1201  ................
-000016d0: 1a01 1f01 2801 3001 3601 4001 4601 4701  ....(.0.6.@.F.G.
-000016e0: 4a01 4b01 4d01 5601 5701 5901 5a01 5c01  J.K.M.V.W.Y.Z.\.
-000016f0: 6501 6601 6801 6901 6b01 7401 7501 7601  e.f.h.i.k.t.u.v.
-00001700: 7801 8101 8201 8401 8501 8701 9001 9101  x...............
-00001710: 9301 9401 9601 9f01 a001 a201 a301 a501  ................
-00001720: ae01 af01 b101 b201 b401 bd01 be01 c101  ................
-00001730: c201 c401 c501 ce01 d701 e001 e500 0000  ................
-00001740: 0000 0002 0100 0000 0000 0000 4d00 0000  ............M...
-00001750: 0000 0000 0000 0000 0000 0001 e600 0000  ................
-00001760: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
-00001770: 6f44 4462 6c6f 6200 0000 080e 96d0 4582  oDDblob.......E.
-00001780: 0ec5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
-00001790: 7500 7000 736d 6f64 4462 6c6f 6200 0000  u.p.smodDblob...
-000017a0: 080e 96d0 4582 0ec5 4100 0000 0700 7000  ....E...A.....p.
-000017b0: 6f00 7000 5f00 7500 7000 7370 6831 5363  o.p._.u.p.sph1Sc
-000017c0: 6f6d 7000 0000 0000 09d0 0000 0000 0700  omp.............
-000017d0: 7000 6f00 7000 5f00 7500 7000 7376 5372  p.o.p._.u.p.svSr
-000017e0: 6e6c 6f6e 6700 0000 0100 0000 0000 0000  nlong...........
+00001020: 0065 005f 005f 6277 7370 626c 6f62 0000  .e._._bwspblob..
+00001030: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
+00001040: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
+00001050: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
+00001060: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
+00001070: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+00001080: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+00001090: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+000010a0: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
+000010b0: 5f10 197b 7b31 3036 322c 2033 3733 7d2c  _..{{1062, 373},
+000010c0: 207b 3737 302c 2034 3336 7d7d 0908 1725   {770, 436}}...%
+000010d0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
+000010e0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
+000010f0: 0000 0000 0000 0000 0000 009b 0000 000b  ................
+00001100: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
+00001110: 0065 005f 005f 6c73 7643 626c 6f62 0000  .e._._lsvCblob..
+00001120: 02d4 6270 6c69 7374 3030 da01 0203 0405  ..bplist00......
+00001130: 0607 0809 0a0b 0c0d 1d4a 4b4c 4d0c 4f5f  .........JKLM.O_
+00001140: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+00001150: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
+00001160: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+00001170: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+00001180: 6573 5f10 0f73 6372 6f6c 6c50 6f73 6974  es_..scrollPosit
+00001190: 696f 6e59 5874 6578 7453 697a 655f 100f  ionYXtextSize_..
+000011a0: 7363 726f 6c6c 506f 7369 7469 6f6e 585a  scrollPositionXZ
+000011b0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
+000011c0: 5265 6c61 7469 7665 4461 7465 7358 6963  RelativeDatesXic
+000011d0: 6f6e 5369 7a65 1001 09ab 0e17 1f24 282d  onSize.......$(-
+000011e0: 3237 3c40 45d4 0f10 1112 130c 150c 5a69  27<@E.........Zi
+000011f0: 6465 6e74 6966 6965 7259 6173 6365 6e64  dentifierYascend
+00001200: 696e 6755 7769 6474 6857 7669 7369 626c  ingUwidthWvisibl
+00001210: 6554 6e61 6d65 0911 012c 09d4 0f18 191a  eTname...,......
+00001220: 1b1c 1d1d 5577 6964 7468 5961 7363 656e  ....UwidthYascen
+00001230: 6469 6e67 5776 6973 6962 6c65 5875 6269  dingWvisibleXubi
+00001240: 7175 6974 7910 2308 08d4 0f10 1112 201d  quity.#....... .
+00001250: 220c 5c64 6174 654d 6f64 6966 6965 6408  ".\dateModified.
+00001260: 10b5 09d4 0f10 1112 251d 221d 5b64 6174  ........%.".[dat
+00001270: 6543 7265 6174 6564 0808 d40f 1011 1229  eCreated.......)
+00001280: 1d2b 0c54 7369 7a65 0810 6109 d40f 1011  .+.Tsize..a.....
+00001290: 122e 0c30 0c54 6b69 6e64 0910 7309 d40f  ...0.Tkind..s...
+000012a0: 1011 1233 0c35 1d55 6c61 6265 6c09 1064  ...3.5.Ulabel..d
+000012b0: 08d4 0f10 1112 380c 3a1d 5776 6572 7369  ......8.:.Wversi
+000012c0: 6f6e 0910 4b08 d40f 1011 123d 0c15 1d58  on..K......=...X
+000012d0: 636f 6d6d 656e 7473 0908 d40f 1011 1241  comments.......A
+000012e0: 1d43 1d5e 6461 7465 4c61 7374 4f70 656e  .C.^dateLastOpen
+000012f0: 6564 0810 c808 d40f 1819 1a46 221d 1d59  ed.........F"..Y
+00001300: 6461 7465 4164 6465 6408 0808 2300 0000  dateAdded...#...
+00001310: 0000 0000 0023 4028 0000 0000 0000 2340  .....#@(......#@
+00001320: 1400 0000 0000 0054 6e61 6d65 0923 4030  .......Tname.#@0
+00001330: 0000 0000 0000 0008 001d 0032 0044 004c  ...........2.D.L
+00001340: 0060 0072 007b 008d 0098 00ab 00b4 00b6  .`.r.{..........
+00001350: 00b7 00c3 00cc 00d7 00e1 00e7 00ef 00f4  ................
+00001360: 00f5 00f8 00f9 0102 0108 0112 011a 0123  ...............#
+00001370: 0125 0126 0127 0130 013d 013e 0140 0141  .%.&.'.0.=.>.@.A
+00001380: 014a 0156 0157 0158 0161 0166 0167 0169  .J.V.W.X.a.f.g.i
+00001390: 016a 0173 0178 0179 017b 017c 0185 018b  .j.s.x.y.{.|....
+000013a0: 018c 018e 018f 0198 01a0 01a1 01a3 01a4  ................
+000013b0: 01ad 01b6 01b7 01b8 01c1 01d0 01d1 01d3  ................
+000013c0: 01d4 01dd 01e7 01e8 01e9 01ea 01f3 01fc  ................
+000013d0: 0205 020a 020b 0000 0000 0000 0201 0000  ................
+000013e0: 0000 0000 0050 0000 0000 0000 0000 0000  .....P..........
+000013f0: 0000 0000 0214 0000 000b 005f 005f 0070  ..........._._.p
+00001400: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+00001410: 6c73 7670 626c 6f62 0000 029b 6270 6c69  lsvpblob....bpli
+00001420: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
+00001430: 0c0d 1c46 4748 490c 4b5f 1012 7669 6577  ...FGHI.K_..view
+00001440: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+00001450: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00001460: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00001470: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
+00001480: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
+00001490: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
+000014a0: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
+000014b0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+000014c0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
+000014d0: 1001 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
+000014e0: 2a2f 3439 3e42 5863 6f6d 6d65 6e74 735e  */49>BXcomments^
+000014f0: 6461 7465 4c61 7374 4f70 656e 6564 5b64  dateLastOpened[d
+00001500: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
+00001510: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+00001520: 6f6e 546e 616d 655c 6461 7465 4d6f 6469  onTname\dateModi
+00001530: 6669 6564 d418 191a 1b1c 0c1e 1f57 7669  fied.........Wvi
+00001540: 7369 626c 6559 6173 6365 6e64 696e 6755  sibleYascendingU
+00001550: 7769 6474 6855 696e 6465 7808 0911 012c  widthUindex....,
+00001560: 1007 d418 191a 1b1c 1c23 2408 0810 c810  .........#$.....
+00001570: 08d4 1819 1a1b 1c1c 2829 0808 10b5 1002  ........()......
+00001580: d418 191a 1b0c 1c2d 2e09 0810 6110 03d4  .......-....a...
+00001590: 1819 1a1b 1c0c 3233 0809 1064 1005 d418  ......23...d....
+000015a0: 191a 1b0c 0c37 3809 0910 7310 04d4 1819  .....78...s.....
+000015b0: 1a1b 1c0c 3c3d 0809 104b 1006 d418 191a  ....<=...K......
+000015c0: 1b0c 0c1e 4109 0910 00d4 1819 1a1b 0c1c  ....A...........
+000015d0: 280b 0908 0823 0000 0000 0000 0000 2340  (....#........#@
+000015e0: 2800 0000 0000 0023 4014 0000 0000 0000  (......#@.......
+000015f0: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
+00001600: 0800 1d00 3200 4400 4c00 6000 7200 7b00  ....2.D.L.`.r.{.
+00001610: 8d00 9800 ab00 b400 b600 b700 ca00 d300  ................
+00001620: e200 ee00 f300 f900 fe01 0601 0b01 1801  ................
+00001630: 2101 2901 3301 3901 3f01 4001 4101 4401  !.).3.9.?.@.A.D.
+00001640: 4601 4f01 5001 5101 5301 5501 5e01 5f01  F.O.P.Q.S.U.^._.
+00001650: 6001 6201 6401 6d01 6e01 6f01 7101 7301  `.b.d.m.n.o.q.s.
+00001660: 7c01 7d01 7e01 8001 8201 8b01 8c01 8d01  |.}.~...........
+00001670: 8f01 9101 9a01 9b01 9c01 9e01 a001 a901  ................
+00001680: aa01 ab01 ad01 b601 b701 b801 b901 c201  ................
+00001690: cb01 d401 d901 da00 0000 0000 0002 0100  ................
+000016a0: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
+000016b0: 0000 0000 0001 e300 0000 0b00 5f00 5f00  ............_._.
+000016c0: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
+000016d0: 5f76 5372 6e6c 6f6e 6700 0000 0100 0000  _vSrnlong.......
+000016e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000016f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001800: 0000 0000 0000 0003 0000 0000 0000 180b  ................
 00001810: 0000 0045 0000 100b 0000 0000 0000 0000  ...E............
 00001820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,57 +457,57 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 005f 1011  .....@......._..
-00001d00: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00001d10: 735f 100f 7363 726f 6c6c 506f 7369 7469  s_..scrollPositi
-00001d20: 6f6e 5958 7465 7874 5369 7a65 5f10 0f73  onYXtextSize_..s
-00001d30: 6372 6f6c 6c50 6f73 6974 696f 6e58 5a73  crollPositionXZs
-00001d40: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
-00001d50: 656c 6174 6976 6544 6174 6573 5f10 1276  elativeDates_..v
-00001d60: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-00001d70: 6e23 4030 0000 0000 0000 09d9 0e0f 1011  n#@0............
-00001d80: 1213 1415 1617 2025 2a2e 3338 3d42 5863  ...... %*.38=BXc
-00001d90: 6f6d 6d65 6e74 735e 6461 7465 4c61 7374  omments^dateLast
-00001da0: 4f70 656e 6564 5c64 6174 654d 6f64 6966  Opened\dateModif
-00001db0: 6965 645b 6461 7465 4372 6561 7465 6454  ied[dateCreatedT
-00001dc0: 7369 7a65 556c 6162 656c 546b 696e 6457  sizeUlabelTkindW
-00001dd0: 7665 7273 696f 6e54 6e61 6d65 d418 191a  versionTname....
-00001de0: 1b1c 1d0c 1f57 7669 7369 626c 6555 7769  .....WvisibleUwi
-00001df0: 6474 6859 6173 6365 6e64 696e 6755 696e  dthYascendingUin
-00001e00: 6465 7808 1101 2c09 1007 d418 191a 1b1c  dex...,.........
-00001e10: 221c 2408 10c8 0810 08d4 1819 1a1b 0c27  ".$............'
-00001e20: 1c29 0910 b508 1001 d418 191a 1b1c 271c  .)............'.
-00001e30: 2d08 0810 02d4 1819 1a1b 0c30 1c32 0910  -..........0.2..
-00001e40: 6108 1003 d418 191a 1b1c 350c 3708 1064  a.........5.7..d
-00001e50: 0910 05d4 1819 1a1b 0c3a 0c3c 0910 7309  .........:.<..s.
-00001e60: 1004 d418 191a 1b1c 3f0c 4108 104b 0910  ........?.A..K..
-00001e70: 06d4 1819 1a1b 0c44 0c46 0911 01c7 0910  .......D.F......
-00001e80: 0008 2340 73a0 0000 0000 0023 4028 0000  ..#@s......#@(..
-00001e90: 0000 0000 2300 0000 0000 0000 0054 6e61  ....#........Tna
-00001ea0: 6d65 0900 0800 1d00 2600 3800 4000 5400  me......&.8.@.T.
-00001eb0: 6600 6f00 8100 8c00 9f00 b400 bd00 be00  f.o.............
-00001ec0: d100 da00 e900 f601 0201 0701 0d01 1201  ................
-00001ed0: 1a01 1f01 2801 3001 3601 4001 4601 4701  ....(.0.6.@.F.G.
-00001ee0: 4a01 4b01 4d01 5601 5701 5901 5a01 5c01  J.K.M.V.W.Y.Z.\.
-00001ef0: 6501 6601 6801 6901 6b01 7401 7501 7601  e.f.h.i.k.t.u.v.
-00001f00: 7801 8101 8201 8401 8501 8701 9001 9101  x...............
-00001f10: 9301 9401 9601 9f01 a001 a201 a301 a501  ................
-00001f20: ae01 af01 b101 b201 b401 bd01 be01 c101  ................
-00001f30: c201 c401 c501 ce01 d701 e001 e500 0000  ................
-00001f40: 0000 0002 0100 0000 0000 0000 4d00 0000  ............M...
-00001f50: 0000 0000 0000 0000 0000 0001 e600 0000  ................
-00001f60: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
-00001f70: 6f44 4462 6c6f 6200 0000 080e 96d0 4582  oDDblob.......E.
-00001f80: 0ec5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
-00001f90: 7500 7000 736d 6f64 4462 6c6f 6200 0000  u.p.smodDblob...
-00001fa0: 080e 96d0 4582 0ec5 4100 0000 0700 7000  ....E...A.....p.
-00001fb0: 6f00 7000 5f00 7500 7000 7370 6831 5363  o.p._.u.p.sph1Sc
-00001fc0: 6f6d 7000 0000 0000 09d0 0000 0000 0700  omp.............
-00001fd0: 7000 6f00 7000 5f00 7500 7000 7376 5372  p.o.p._.u.p.svSr
-00001fe0: 6e6c 6f6e 6700 0000 0100 0000 0000 0000  nlong...........
+00001cf0: 0000 0000 0140 0000 0000 0000 0064 5b64  .....@.......d[d
+00001d00: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
+00001d10: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+00001d20: 6f6e 546e 616d 655c 6461 7465 4d6f 6469  onTname\dateModi
+00001d30: 6669 6564 d418 191a 1b1c 0c1e 1f57 7669  fied.........Wvi
+00001d40: 7369 626c 6559 6173 6365 6e64 696e 6755  sibleYascendingU
+00001d50: 7769 6474 6855 696e 6465 7808 0911 012c  widthUindex....,
+00001d60: 1007 d418 191a 1b1c 1c23 2408 0810 c810  .........#$.....
+00001d70: 08d4 1819 1a1b 1c1c 2829 0808 10b5 1002  ........()......
+00001d80: d418 191a 1b0c 1c2d 2e09 0810 6110 03d4  .......-....a...
+00001d90: 1819 1a1b 1c0c 3233 0809 1064 1005 d418  ......23...d....
+00001da0: 191a 1b0c 0c37 3809 0910 7310 04d4 1819  .....78...s.....
+00001db0: 1a1b 1c0c 3c3d 0809 104b 1006 d418 191a  ....<=...K......
+00001dc0: 1b0c 0c1e 4109 0910 00d4 1819 1a1b 0c1c  ....A...........
+00001dd0: 280b 0908 0823 0000 0000 0000 0000 2340  (....#........#@
+00001de0: 2800 0000 0000 0023 4014 0000 0000 0000  (......#@.......
+00001df0: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
+00001e00: 0800 1d00 3200 4400 4c00 6000 7200 7b00  ....2.D.L.`.r.{.
+00001e10: 8d00 9800 ab00 b400 b600 b700 ca00 d300  ................
+00001e20: e200 ee00 f300 f900 fe01 0601 0b01 1801  ................
+00001e30: 2101 2901 3301 3901 3f01 4001 4101 4401  !.).3.9.?.@.A.D.
+00001e40: 4601 4f01 5001 5101 5301 5501 5e01 5f01  F.O.P.Q.S.U.^._.
+00001e50: 6001 6201 6401 6d01 6e01 6f01 7101 7301  `.b.d.m.n.o.q.s.
+00001e60: 7c01 7d01 7e01 8001 8201 8b01 8c01 8d01  |.}.~...........
+00001e70: 8f01 9101 9a01 9b01 9c01 9e01 a001 a901  ................
+00001e80: aa01 ab01 ad01 b601 b701 b801 b901 c201  ................
+00001e90: cb01 d401 d901 da00 0000 0000 0002 0100  ................
+00001ea0: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
+00001eb0: 0000 0000 0001 e300 0000 0b00 5f00 5f00  ............_._.
+00001ec0: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
+00001ed0: 5f76 5372 6e6c 6f6e 6700 0000 0100 0000  _vSrnlong.......
+00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
         run_btn = Button(self.main_frm, text='CONFIRM', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='red', command=lambda: self.run())
         run_btn.grid(row=3, column=0, sticky=NW)
 
     def run(self):
         check_float(name='LOCATION CRITERION', value=self.location_criterion.entry_get, min_value=0.0)
         check_float(name='MOVEMENT CRITERION', value=self.movement_criterion.entry_get, min_value=0.0)
+        if not self.config.has_section('Outlier settings'): self.config.add_section('Outlier settings')
         self.config.set('Outlier settings', 'movement_criterion', str(self.movement_criterion.entry_get))
         self.config.set('Outlier settings', 'location_criterion', str(self.location_criterion.entry_get))
         self.config.set('Outlier settings', 'mean_or_median', str(self.agg_type_dropdown.getChoices()))
         for animal_cnt, animal_name in enumerate(self.animal_bp_dict.keys()):
             self.config.set('Outlier settings', 'movement_bodyPart1_{}'.format(animal_name), self.criterion_dropdowns[animal_name]['movement_bp_1'].getChoices())
             self.config.set('Outlier settings', 'movement_bodyPart2_{}'.format(animal_name), self.criterion_dropdowns[animal_name]['movement_bp_2'].getChoices())
             self.config.set('Outlier settings', 'location_bodyPart1_{}'.format(animal_name), self.criterion_dropdowns[animal_name]['location_bp_1'].getChoices())
```

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.61.7/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.61.7/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.61.7/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.61.7/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.61.7/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.61.7/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.61.7/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.61.7/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/requirements.txt` & `Simba-UW-tf-dev-1.61.7/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.61.7/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.61.7/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.61.7/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.61.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.61.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.61.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.61.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.61.7/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.61.7/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.61.7/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.61.7/simba/mixins/train_model_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -564,14 +564,17 @@
         .. seealso::
            `Documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#train-predictive-classifiers-settings>`_
 
            .. image:: _static/img/shap.png
               :width: 400
               :align: center
 
+        .. note::
+           For improved run-times, use multiprocessing through :meth:`simba.mixins.train_model_mixins.TrainModelMixin.create_shap_log_mp`
+
         :param str ini_file_path: Path to the SimBA project_config.ini
         :param RandomForestClassifier rf_clf: sklearn random forest classifier
         :param pd.DataFrame x_df: Test features.
         :param pd.DataFrame y_df: Test target.
         :param List[str] x_names: Feature names.
         :param str clf_name: Classifier name.
         :param int cnt_present: Number of behavior-present frames to calculate SHAP values for.
@@ -590,27 +593,24 @@
             out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{clf_name}.csv')
         else:
             out_df_shap_path = os.path.join(save_path, f'SHAP_values_{str(save_file_no)}_{clf_name}.csv')
             out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{str(save_file_no)}_{clf_name}.csv')
 
         target_df, nontarget_df = data_df[data_df[y_df.name] == 1], data_df[data_df[y_df.name] == 0]
         if len(target_df) < cnt_present:
-            NotEnoughDataWarning(
-                msg=f'Train data contains {str(len(target_df))} behavior-present annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_present)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-present frames available')
+            NotEnoughDataWarning(msg=f'Train data contains {str(len(target_df))} behavior-present annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_present)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-present frames available')
             cnt_present = len(target_df)
         if len(nontarget_df) < cnt_absent:
-            NotEnoughDataWarning(
-                msg=f'Train data contains {str(len(nontarget_df))} behavior-absent annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_absent)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-absent frames available')
+            NotEnoughDataWarning(msg=f'Train data contains {str(len(nontarget_df))} behavior-absent annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_absent)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-absent frames available')
             cnt_absent = len(nontarget_df)
         non_target_for_shap = nontarget_df.sample(cnt_absent, replace=False)
         targets_for_shap = target_df.sample(cnt_present, replace=False)
         shap_df = pd.concat([targets_for_shap, non_target_for_shap], axis=0)
         y_df = shap_df.pop(clf_name).values
-        explainer = shap.TreeExplainer(rf_clf, data=None, model_output='raw',
-                                       feature_perturbation='tree_path_dependent')
+        explainer = shap.TreeExplainer(rf_clf, data=None, model_output='raw', feature_perturbation='tree_path_dependent')
         expected_value = explainer.expected_value[1]
         out_df_raw = pd.DataFrame(columns=x_names)
         shap_headers = list(x_names)
         shap_headers.extend(('Expected_value', 'Sum', 'Prediction_probability', clf_name))
         out_df_shap = pd.DataFrame(columns=shap_headers)
         for cnt, frame in enumerate(range(len(shap_df))):
             shap_frm_timer = SimbaTimer(start=True)
@@ -1079,22 +1079,122 @@
             results = pd.DataFrame.from_dict(data=results, orient='index')
             results.to_csv(save_log_path)
             raise FaultyTrainingSetError(
                 msg=f'{len(nan_cols)} feature columns exist in some files, but missing in others. The feature files are found in the project_folder/csv/targets_inserted directory. ' \
                     f'SimBA expects all files within the project_folder/csv/targets_inserted directory to have the same number of features: the first 10 ' \
                     f'column names with mismatches are: {nan_cols[0:9]}. For a log of the files that contain, and not contain, the mis-matched columns, see {save_log_path}')
 
+    def _create_shap_mp_helper(self,
+                               data: pd.DataFrame,
+                               clf_name: str,
+                               explainer: shap.TreeExplainer,
+                               clf: RandomForestClassifier,
+                               expected_value: float):
+
+        target = data.pop(clf_name).values.reshape(-1, 1)
+        frame_batch_shap = explainer.shap_values(data.values, check_additivity=False)[1]
+        shap_sum = np.sum(frame_batch_shap, axis=1).reshape(-1, 1)
+        proba = clf.predict_proba(data)[:, 1].reshape(-1, 1)
+        frame_batch_shap = np.hstack((frame_batch_shap,
+                                      np.full((frame_batch_shap.shape[0]), expected_value).reshape(-1, 1), shap_sum,
+                                      proba, target))
+        return frame_batch_shap, data.values[0]
+
+    def create_shap_log_mp(self,
+                           ini_file_path: str,
+                           rf_clf: RandomForestClassifier,
+                           x_df: pd.DataFrame,
+                           y_df: pd.DataFrame,
+                           x_names: List[str],
+                           clf_name: str,
+                           cnt_present: int,
+                           cnt_absent: int,
+                           save_path: str,
+                           batch_size: int = 10,
+                           save_it: int = 100,
+                           save_file_no: Optional[int] = None) -> None:
+        """
+        Helper to compute SHAP values using multiprocessing.
+        For single-core alternative, see  meth:`simba.mixins.train_model_mixins.TrainModelMixin.create_shap_log_mp`.
+
+        .. seealso::
+           `Documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#train-predictive-classifiers-settings>`_
+
+           .. image:: _static/img/shap.png
+              :width: 400
+              :align: center
+
+        :param str ini_file_path: Path to the SimBA project_config.ini
+        :param RandomForestClassifier rf_clf: sklearn random forest classifier
+        :param pd.DataFrame x_df: Test features.
+        :param pd.DataFrame y_df: Test target.
+        :param List[str] x_names: Feature names.
+        :param str clf_name: Classifier name.
+        :param int cnt_present: Number of behavior-present frames to calculate SHAP values for.
+        :param int cnt_absent: Number of behavior-absent frames to calculate SHAP values for.
+        :param str save_dir: Directory where to save output in csv file format.
+        :param Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
+            part of a grid search.
+
+        """
+
+        print('Calculating SHAP values...')
+        shap_timer = SimbaTimer(start=True)
+        data_df = pd.concat([x_df, y_df], axis=1)
+        if save_file_no == None:
+            out_df_shap_path = os.path.join(save_path, f'SHAP_values_{clf_name}.csv')
+            out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{clf_name}.csv')
+        else:
+            out_df_shap_path = os.path.join(save_path, f'SHAP_values_{str(save_file_no)}_{clf_name}.csv')
+            out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{str(save_file_no)}_{clf_name}.csv')
+        target_df, nontarget_df = data_df[data_df[y_df.name] == 1], data_df[data_df[y_df.name] == 0]
+        if len(target_df) < cnt_present:
+            NotEnoughDataWarning(
+                msg=f'Train data contains {str(len(target_df))} behavior-present annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_present)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-present frames available')
+            cnt_present = len(target_df)
+        if len(nontarget_df) < cnt_absent:
+            NotEnoughDataWarning(
+                msg=f'Train data contains {str(len(nontarget_df))} behavior-absent annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_absent)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-absent frames available')
+            cnt_absent = len(nontarget_df)
+        non_target_for_shap = nontarget_df.sample(cnt_absent, replace=False)
+        targets_for_shap = target_df.sample(cnt_present, replace=False)
+        explainer = shap.TreeExplainer(rf_clf, data=None, model_output='raw',
+                                       feature_perturbation='tree_path_dependent')
+        expected_value = explainer.expected_value[1]
+        cores, _ = find_core_cnt()
+        shap_data_df = pd.concat([targets_for_shap, non_target_for_shap], axis=0)
+        if (len(shap_data_df) / batch_size) < 1: batch_size = 1
+        shap_data = np.array_split(shap_data_df, len(shap_data_df) / batch_size)
+        shap_results, shap_raw = [], []
+        with ProcessPoolExecutor(cores) as pool:
+            for it_cnt, res in enumerate(pool.map(self._create_shap_mp_helper, shap_data, repeat(clf_name), repeat(explainer), repeat(rf_clf), repeat(expected_value))):
+                shap_values, raw_values = res
+                shap_results.append(shap_values);
+                shap_raw.append(raw_values)
+                data_size = int(len(shap_results) * batch_size)
+                if (data_size != 0) and (data_size % save_it == 0) or (data_size == len(shap_data_df)):
+                    print(f'Saving SHAP data after {data_size} iterations...')
+                    shap_save_df = pd.DataFrame(data=np.row_stack(shap_results),
+                                                columns=list(x_names) + ['Expected_value', 'Sum',
+                                                                         'Prediction_probability', clf_name])
+                    raw_save_df = pd.DataFrame(data=np.row_stack(shap_raw), columns=list(x_names))
+                    shap_save_df.to_csv(out_df_shap_path)
+                    raw_save_df.to_csv(out_df_raw_path)
+                print(f'SHAP frame: {data_size} / {len(shap_data_df)} complete...')
+
+        shap_timer.stop_timer()
+        stdout_success(msg='SHAP calculations complete', elapsed_time=shap_timer.elapsed_time_str)
+        _ = ShapAggregateStatisticsVisualizer(config_path=ini_file_path,
+                                              classifier_name=clf_name,
+                                              shap_df=shap_save_df,
+                                              shap_baseline_value=int(expected_value * 100),
+                                              save_path=save_path)
 
 # test = TrainModelMixin()
 # test.read_all_files_in_folder(file_paths=['/Users/simon/Desktop/envs/troubleshooting/jake/project_folder/csv/targets_inserted/22-437C_c3_2022-11-01_13-16-23_color.csv', '/Users/simon/Desktop/envs/troubleshooting/jake/project_folder/csv/targets_inserted/22-437D_c4_2022-11-01_13-16-39_color.csv'],
 #                               file_type='csv', classifier_names=['attack', 'non-agresive parallel swimming'])
 
 
 # test = TrainModelMixin()
 # test.read_all_files_in_folder_mp(file_paths=['/Users/simon/Desktop/envs/troubleshooting/jake/project_folder/csv/targets_inserted/22-437C_c3_2022-11-01_13-16-23_color.csv', '/Users/simon/Desktop/envs/troubleshooting/jake/project_folder/csv/targets_inserted/22-437D_c4_2022-11-01_13-16-39_color.csv'],
 #                               file_type='csv', classifier_names=['attack', 'non-agresive parallel swimming'])
 #
-#     #
-    # def read_all_files_in_folder(self,
-    #                              file_paths: List[str],
-    #                              file_type: str,
-    #                              classifier_names: Optional[List[str]] = None) -> pd.DataFrame:
```

### Comparing `Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.61.7/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.61.7/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.61.7/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/utils/enums.py` & `Simba-UW-tf-dev-1.61.7/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.61.7/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/utils/checks.py` & `Simba-UW-tf-dev-1.61.7/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.61.7/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.61.7/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.61.7/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/utils/errors.py` & `Simba-UW-tf-dev-1.61.7/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/utils/data.py` & `Simba-UW-tf-dev-1.61.7/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/utils/printing.py` & `Simba-UW-tf-dev-1.61.7/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.61.7/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.61.7/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.61.7/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.61.7/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.61.7/simba/model/train_rf.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,24 +185,24 @@
             if generate_features_importance_log in Options.PERFORM_FLAGS.value:
                 self.create_x_importance_log(self.rf_clf, self.feature_names, self.clf_name, self.eval_out_path)
             if generate_features_importance_bar_graph in Options.PERFORM_FLAGS.value:
                 self.create_x_importance_bar_chart(self.rf_clf, self.feature_names, self.clf_name, self.eval_out_path, feature_importance_bars)
             if generate_example_decision_tree_fancy in Options.PERFORM_FLAGS.value:
                 self.dviz_classification_visualization(self.x_train, self.y_train, self.clf_name, self.class_names, self.eval_out_path)
             if generate_shap_scores in Options.PERFORM_FLAGS.value:
-                self.create_shap_log(ini_file_path=self.config_path,
-                                rf_clf=self.rf_clf,
-                                x_df=self.x_train,
-                                y_df=self.y_train,
-                                x_names=self.feature_names,
-                                clf_name=self.clf_name,
-                                cnt_present=shap_target_present_cnt,
-                                cnt_absent=shap_target_absent_cnt,
-                                save_it=shap_save_n,
-                                save_path=self.eval_out_path)
+                self.create_shap_log_mp(ini_file_path=self.config_path,
+                                        rf_clf=self.rf_clf,
+                                        x_df=self.x_train,
+                                        y_df=self.y_train,
+                                        x_names=self.feature_names,
+                                        clf_name=self.clf_name,
+                                        cnt_present=shap_target_present_cnt,
+                                        cnt_absent=shap_target_absent_cnt,
+                                        save_it=shap_save_n,
+                                        save_path=self.eval_out_path)
 
             if compute_partial_dependency in Options.PERFORM_FLAGS.value:
                 self.partial_dependence_calculator(clf=self.rf_clf, x_df=self.x_train, clf_name=self.clf_name, save_dir=self.eval_out_path)
 
             if save_meta_data in Options.PERFORM_FLAGS.value:
                 meta_data_lst = [self.clf_name, criterion, max_features, min_sample_leaf,
                                  n_estimators, compute_permutation_importance, generate_classification_report,
```

### Comparing `Simba-UW-tf-dev-1.61.6/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.61.7/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.61.7/simba/model/grid_search_rf.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
                 save_n = meta_dict[MetaKeys.SHAP_PRESENT.value] + meta_dict[MetaKeys.SHAP_ABSENT.value]
                 if MetaKeys.SHAP_SAVE_ITERATION.value in meta_dict.keys():
                     try:
                         save_n = int(meta_dict[MetaKeys.SHAP_SAVE_ITERATION.value])
                     except ValueError:
                         save_n = meta_dict[MetaKeys.SHAP_PRESENT.value] + meta_dict[MetaKeys.SHAP_ABSENT.value]
                 if meta_dict[MetaKeys.SHAP_SCORES.value] in Options.PERFORM_FLAGS.value:
-                    self.create_shap_log(self.config_path, self.rf_clf, self.x_train, self.y_train, self.feature_names, self.clf_name, meta_dict[MetaKeys.SHAP_PRESENT.value], meta_dict[MetaKeys.SHAP_ABSENT.value], self.model_dir_out, save_it=save_n, save_file_no=config_cnt)
+                    self.create_shap_log_mp(self.config_path, self.rf_clf, self.x_train, self.y_train, self.feature_names, self.clf_name, meta_dict[MetaKeys.SHAP_PRESENT.value], meta_dict[MetaKeys.SHAP_ABSENT.value], self.model_dir_out, save_it=save_n, save_file_no=config_cnt)
             if MetaKeys.PARTIAL_DEPENDENCY.value in meta_dict.keys():
                 if meta_dict[MetaKeys.PARTIAL_DEPENDENCY.value] in Options.PERFORM_FLAGS.value:
                     self.partial_dependence_calculator(clf=self.rf_clf, x_df=self.x_train, clf_name=self.clf_name, save_dir=self.model_dir_out)
             self.create_meta_data_csv_training_multiple_models(meta_dict, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
             self.save_rf_model(self.rf_clf, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
             print('Classifier {} saved in models/validations/model_files directory ...'.format(str(self.clf_name + '_' + str(config_cnt))))
         stdout_success(msg='All models and evaluations complete. The models/evaluation files are in models/validations folders')
```

### Comparing `Simba-UW-tf-dev-1.61.6/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.61.7/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.61.7/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.61.7/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.61.7/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.61.7/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/ui/.DS_Store`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 000c  ................
 00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
 00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,141 +250,141 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0004 0000 000b  ................
+00001000: 0000 0000 0000 0000 0000 000c 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00001020: 0065 005f 005f 6277 7370 626c 6f62 0000  .e._._bwspblob..
-00001030: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-00001040: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
-00001050: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-00001060: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-00001070: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00001080: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00001090: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-000010a0: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
-000010b0: 5f10 197b 7b31 3036 322c 2033 3733 7d2c  _..{{1062, 373},
-000010c0: 207b 3737 302c 2034 3336 7d7d 0908 1725   {770, 436}}...%
-000010d0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
-000010e0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-000010f0: 0000 0000 0000 0000 0000 009b 0000 000b  ................
-00001100: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00001110: 0065 005f 005f 6c73 7643 626c 6f62 0000  .e._._lsvCblob..
-00001120: 02d4 6270 6c69 7374 3030 da01 0203 0405  ..bplist00......
-00001130: 0607 0809 0a0b 0c0d 1d4a 4b4c 4d0c 4f5f  .........JKLM.O_
-00001140: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-00001150: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
-00001160: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-00001170: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-00001180: 6573 5f10 0f73 6372 6f6c 6c50 6f73 6974  es_..scrollPosit
-00001190: 696f 6e59 5874 6578 7453 697a 655f 100f  ionYXtextSize_..
-000011a0: 7363 726f 6c6c 506f 7369 7469 6f6e 585a  scrollPositionXZ
-000011b0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
-000011c0: 5265 6c61 7469 7665 4461 7465 7358 6963  RelativeDatesXic
-000011d0: 6f6e 5369 7a65 1001 09ab 0e17 1f24 282d  onSize.......$(-
-000011e0: 3237 3c40 45d4 0f10 1112 130c 150c 5a69  27<@E.........Zi
-000011f0: 6465 6e74 6966 6965 7259 6173 6365 6e64  dentifierYascend
-00001200: 696e 6755 7769 6474 6857 7669 7369 626c  ingUwidthWvisibl
-00001210: 6554 6e61 6d65 0911 012c 09d4 0f18 191a  eTname...,......
-00001220: 1b1c 1d1d 5577 6964 7468 5961 7363 656e  ....UwidthYascen
-00001230: 6469 6e67 5776 6973 6962 6c65 5875 6269  dingWvisibleXubi
-00001240: 7175 6974 7910 2308 08d4 0f10 1112 201d  quity.#....... .
-00001250: 220c 5c64 6174 654d 6f64 6966 6965 6408  ".\dateModified.
-00001260: 10b5 09d4 0f10 1112 251d 221d 5b64 6174  ........%.".[dat
-00001270: 6543 7265 6174 6564 0808 d40f 1011 1229  eCreated.......)
-00001280: 1d2b 0c54 7369 7a65 0810 6109 d40f 1011  .+.Tsize..a.....
-00001290: 122e 0c30 0c54 6b69 6e64 0910 7309 d40f  ...0.Tkind..s...
-000012a0: 1011 1233 0c35 1d55 6c61 6265 6c09 1064  ...3.5.Ulabel..d
-000012b0: 08d4 0f10 1112 380c 3a1d 5776 6572 7369  ......8.:.Wversi
-000012c0: 6f6e 0910 4b08 d40f 1011 123d 0c15 1d58  on..K......=...X
-000012d0: 636f 6d6d 656e 7473 0908 d40f 1011 1241  comments.......A
-000012e0: 1d43 1d5e 6461 7465 4c61 7374 4f70 656e  .C.^dateLastOpen
-000012f0: 6564 0810 c808 d40f 1819 1a46 221d 1d59  ed.........F"..Y
-00001300: 6461 7465 4164 6465 6408 0808 2300 0000  dateAdded...#...
-00001310: 0000 0000 0023 4028 0000 0000 0000 2340  .....#@(......#@
-00001320: 1400 0000 0000 0054 6e61 6d65 0923 4030  .......Tname.#@0
-00001330: 0000 0000 0000 0008 001d 0032 0044 004c  ...........2.D.L
-00001340: 0060 0072 007b 008d 0098 00ab 00b4 00b6  .`.r.{..........
-00001350: 00b7 00c3 00cc 00d7 00e1 00e7 00ef 00f4  ................
-00001360: 00f5 00f8 00f9 0102 0108 0112 011a 0123  ...............#
-00001370: 0125 0126 0127 0130 013d 013e 0140 0141  .%.&.'.0.=.>.@.A
-00001380: 014a 0156 0157 0158 0161 0166 0167 0169  .J.V.W.X.a.f.g.i
-00001390: 016a 0173 0178 0179 017b 017c 0185 018b  .j.s.x.y.{.|....
-000013a0: 018c 018e 018f 0198 01a0 01a1 01a3 01a4  ................
-000013b0: 01ad 01b6 01b7 01b8 01c1 01d0 01d1 01d3  ................
-000013c0: 01d4 01dd 01e7 01e8 01e9 01ea 01f3 01fc  ................
-000013d0: 0205 020a 020b 0000 0000 0000 0201 0000  ................
-000013e0: 0000 0000 0050 0000 0000 0000 0000 0000  .....P..........
-000013f0: 0000 0000 0214 0000 000b 005f 005f 0070  ..........._._.p
-00001400: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001410: 6c73 7670 626c 6f62 0000 029b 6270 6c69  lsvpblob....bpli
-00001420: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-00001430: 0c0d 1c46 4748 490c 4b5f 1012 7669 6577  ...FGHI.K_..view
-00001440: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
-00001450: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00001460: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00001470: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
-00001480: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
-00001490: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
-000014a0: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
-000014b0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-000014c0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
-000014d0: 1001 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
-000014e0: 2a2f 3439 3e42 5863 6f6d 6d65 6e74 735e  */49>BXcomments^
-000014f0: 6461 7465 4c61 7374 4f70 656e 6564 5b64  dateLastOpened[d
-00001500: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
-00001510: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-00001520: 6f6e 546e 616d 655c 6461 7465 4d6f 6469  onTname\dateModi
-00001530: 6669 6564 d418 191a 1b1c 0c1e 1f57 7669  fied.........Wvi
-00001540: 7369 626c 6559 6173 6365 6e64 696e 6755  sibleYascendingU
-00001550: 7769 6474 6855 696e 6465 7808 0911 012c  widthUindex....,
-00001560: 1007 d418 191a 1b1c 1c23 2408 0810 c810  .........#$.....
-00001570: 08d4 1819 1a1b 1c1c 2829 0808 10b5 1002  ........()......
-00001580: d418 191a 1b0c 1c2d 2e09 0810 6110 03d4  .......-....a...
-00001590: 1819 1a1b 1c0c 3233 0809 1064 1005 d418  ......23...d....
-000015a0: 191a 1b0c 0c37 3809 0910 7310 04d4 1819  .....78...s.....
-000015b0: 1a1b 1c0c 3c3d 0809 104b 1006 d418 191a  ....<=...K......
-000015c0: 1b0c 0c1e 4109 0910 00d4 1819 1a1b 0c1c  ....A...........
-000015d0: 280b 0908 0823 0000 0000 0000 0000 2340  (....#........#@
-000015e0: 2800 0000 0000 0023 4014 0000 0000 0000  (......#@.......
-000015f0: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
-00001600: 0800 1d00 3200 4400 4c00 6000 7200 7b00  ....2.D.L.`.r.{.
-00001610: 8d00 9800 ab00 b400 b600 b700 ca00 d300  ................
-00001620: e200 ee00 f300 f900 fe01 0601 0b01 1801  ................
-00001630: 2101 2901 3301 3901 3f01 4001 4101 4401  !.).3.9.?.@.A.D.
-00001640: 4601 4f01 5001 5101 5301 5501 5e01 5f01  F.O.P.Q.S.U.^._.
-00001650: 6001 6201 6401 6d01 6e01 6f01 7101 7301  `.b.d.m.n.o.q.s.
-00001660: 7c01 7d01 7e01 8001 8201 8b01 8c01 8d01  |.}.~...........
-00001670: 8f01 9101 9a01 9b01 9c01 9e01 a001 a901  ................
-00001680: aa01 ab01 ad01 b601 b701 b801 b901 c201  ................
-00001690: cb01 d401 d901 da00 0000 0000 0002 0100  ................
-000016a0: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
-000016b0: 0000 0000 0001 e300 0000 0b00 5f00 5f00  ............_._.
-000016c0: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
-000016d0: 5f76 5372 6e6c 6f6e 6700 0000 0100 0000  _vSrnlong.......
-000016e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000016f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
+00001030: 0000 0000 de4d 0000 000b 005f 005f 0070  .....M....._._.p
+00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+00001050: 6d6f 4444 626c 6f62 0000 0008 c442 b1c2  moDDblob.....B..
+00001060: 760e c541 0000 000b 005f 005f 0070 0079  v..A....._._.p.y
+00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
+00001080: 6444 626c 6f62 0000 0008 ed9b b6f1 cc0c  dDblob..........
+00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
+000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
+000010b0: 636f 6d70 0000 0000 0001 1000 0000 0007  comp............
+000010c0: 0070 006f 0070 005f 0075 0070 0073 6277  .p.o.p._.u.p.sbw
+000010d0: 7370 626c 6f62 0000 00ca 6270 6c69 7374  spblob....bplist
+000010e0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
+000010f0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00001100: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
+00001110: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00001120: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00001130: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00001140: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00001150: 6261 7208 0809 0809 5f10 197b 7b33 3534  bar....._..{{354
+00001160: 2c20 3132 347d 2c20 7b31 3037 362c 2036  , 124}, {1076, 6
+00001170: 3231 7d7d 0908 1725 313d 4960 6d79 7a7b  21}}...%1=I`myz{
+00001180: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
+00001190: 0000 000f 0000 0000 0000 0000 0000 0000  ................
+000011a0: 0000 009b 0000 0007 0070 006f 0070 005f  .........p.o.p._
+000011b0: 0075 0070 0073 6c67 3153 636f 6d70 0000  .u.p.slg1Scomp..
+000011c0: 0000 0007 49d7 0000 0007 0070 006f 0070  ....I......p.o.p
+000011d0: 005f 0075 0070 0073 6c73 7643 626c 6f62  ._.u.p.slsvCblob
+000011e0: 0000 02b8 6270 6c69 7374 3030 da01 0203  ....bplist00....
+000011f0: 0405 0607 0809 0a0b 0c0d 1848 4948 4a0c  ...........HIHJ.
+00001200: 4c5f 1012 7669 6577 4f70 7469 6f6e 7356  L_..viewOptionsV
+00001210: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
+00001220: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00001230: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00001240: 697a 6573 5f10 0f73 6372 6f6c 6c50 6f73  izes_..scrollPos
+00001250: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
+00001260: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
+00001270: 585a 736f 7274 436f 6c75 6d6e 5f10 1075  XZsortColumn_..u
+00001280: 7365 5265 6c61 7469 7665 4461 7465 7358  seRelativeDatesX
+00001290: 6963 6f6e 5369 7a65 1001 09ab 0e17 1c21  iconSize.......!
+000012a0: 252a 2f34 393e 43d4 0f10 1112 1314 0c0c  %*/49>C.........
+000012b0: 5a69 6465 6e74 6966 6965 7255 7769 6474  ZidentifierUwidt
+000012c0: 6859 6173 6365 6e64 696e 6757 7669 7369  hYascendingWvisi
+000012d0: 626c 6554 6e61 6d65 1101 c709 09d4 1210  bleTname........
+000012e0: 110f 1819 181b 0810 2308 5875 6269 7175  ........#.Xubiqu
+000012f0: 6974 79d4 0f10 1112 1d1e 180c 5c64 6174  ity.........\dat
+00001300: 654d 6f64 6966 6965 6410 b508 09d4 0f10  eModified.......
+00001310: 1112 221e 1818 5b64 6174 6543 7265 6174  .."...[dateCreat
+00001320: 6564 0808 d40f 1011 1226 2718 0c54 7369  ed.......&'..Tsi
+00001330: 7a65 1061 0809 d40f 1011 122b 2c0c 0c54  ze.a.......+,..T
+00001340: 6b69 6e64 1073 0909 d40f 1011 1230 310c  kind.s.......01.
+00001350: 1855 6c61 6265 6c10 6409 08d4 0f10 1112  .Ulabel.d.......
+00001360: 3536 0c18 5776 6572 7369 6f6e 104b 0908  56..Wversion.K..
+00001370: d40f 1011 123a 3b0c 1858 636f 6d6d 656e  .....:;..Xcommen
+00001380: 7473 1101 2c09 08d4 0f10 1112 3f40 1818  ts..,.......?@..
+00001390: 5e64 6174 654c 6173 744f 7065 6e65 6410  ^dateLastOpened.
+000013a0: c808 08d4 1210 110f 181e 1846 0808 5964  ...........F..Yd
+000013b0: 6174 6541 6464 6564 0823 0000 0000 0000  ateAdded.#......
+000013c0: 0000 2340 2800 0000 0000 005c 6461 7465  ..#@(......\date
+000013d0: 4d6f 6469 6669 6564 0923 4030 0000 0000  Modified.#@0....
+000013e0: 0000 0008 001d 0032 0044 004c 0060 0072  .......2.D.L.`.r
+000013f0: 007b 008d 0098 00ab 00b4 00b6 00b7 00c3  .{..............
+00001400: 00cc 00d7 00dd 00e7 00ef 00f4 00f7 00f8  ................
+00001410: 00f9 0102 0103 0105 0106 010f 0118 0125  ...............%
+00001420: 0127 0128 0129 0132 013e 013f 0140 0149  .'.(.).2.>.?.@.I
+00001430: 014e 0150 0151 0152 015b 0160 0162 0163  .N.P.Q.R.[.`.b.c
+00001440: 0164 016d 0173 0175 0176 0177 0180 0188  .d.m.s.u.v.w....
+00001450: 018a 018b 018c 0195 019e 01a1 01a2 01a3  ................
+00001460: 01ac 01bb 01bd 01be 01bf 01c8 01c9 01ca  ................
+00001470: 01d4 01d5 01de 01e7 01f4 01f5 0000 0000  ................
+00001480: 0000 0201 0000 0000 0000 004d 0000 0000  ...........M....
+00001490: 0000 0000 0000 0000 0000 01fe 0000 0007  ................
+000014a0: 0070 006f 0070 005f 0075 0070 0073 6c73  .p.o.p._.u.p.sls
+000014b0: 7670 626c 6f62 0000 029d 6270 6c69 7374  vpblob....bplist
+000014c0: 3030 da01 0203 0405 0607 0809 0a0b 0c0d  00..............
+000014d0: 1c47 4847 490c 4b5f 1012 7669 6577 4f70  .GHGI.K_..viewOp
+000014e0: 7469 6f6e 7356 6572 7369 6f6e 5f10 0f73  tionsVersion_..s
+000014f0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+00001500: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00001510: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
+00001520: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
+00001530: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
+00001540: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
+00001550: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
+00001560: 4461 7465 7358 6963 6f6e 5369 7a65 1001  DatesXiconSize..
+00001570: 09d9 0e0f 1011 1213 1415 1617 2025 292d  ............ %)-
+00001580: 3237 3c41 5863 6f6d 6d65 6e74 735e 6461  27<AXcomments^da
+00001590: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
+000015a0: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
+000015b0: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+000015c0: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+000015d0: 6d65 d418 191a 1b1c 1d0c 1f57 7669 7369  me.........Wvisi
+000015e0: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
+000015f0: 696e 6755 696e 6465 7808 1101 2c09 1007  ingUindex...,...
+00001600: d418 191a 1b1c 221c 2408 10c8 0810 08d4  ......".$.......
+00001610: 1819 1a1b 0c27 1c0b 0910 b508 d418 191a  .....'..........
+00001620: 1b1c 271c 2c08 0810 02d4 1819 1a1b 0c2f  ..'.,........../
+00001630: 1c31 0910 6108 1003 d418 191a 1b1c 340c  .1..a.........4.
+00001640: 3608 1064 0910 05d4 1819 1a1b 0c39 0c3b  6..d.........9.;
+00001650: 0910 7309 1004 d418 191a 1b1c 3e0c 4008  ..s.........>.@.
+00001660: 104b 0910 06d4 1819 1a1b 0c43 0c45 0911  .K.........C.E..
+00001670: 01c7 0910 0008 2300 0000 0000 0000 0023  ......#........#
+00001680: 4028 0000 0000 0000 5c64 6174 654d 6f64  @(......\dateMod
+00001690: 6966 6965 6409 2340 3000 0000 0000 0000  ified.#@0.......
+000016a0: 0800 1d00 3200 4400 4c00 6000 7200 7b00  ....2.D.L.`.r.{.
+000016b0: 8d00 9800 ab00 b400 b600 b700 ca00 d300  ................
+000016c0: e200 ef00 fb01 0001 0601 0b01 1301 1801  ................
+000016d0: 2101 2901 2f01 3901 3f01 4001 4301 4401  !.)./.9.?.@.C.D.
+000016e0: 4601 4f01 5001 5201 5301 5501 5e01 5f01  F.O.P.R.S.U.^._.
+000016f0: 6101 6201 6b01 6c01 6d01 6f01 7801 7901  a.b.k.l.m.o.x.y.
+00001700: 7b01 7c01 7e01 8701 8801 8a01 8b01 8d01  {.|.~...........
+00001710: 9601 9701 9901 9a01 9c01 a501 a601 a801  ................
+00001720: a901 ab01 b401 b501 b801 b901 bb01 bc01  ................
+00001730: c501 ce01 db01 dc00 0000 0000 0002 0100  ................
+00001740: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
+00001750: 0000 0000 0001 e500 0000 0700 7000 6f00  ............p.o.
+00001760: 7000 5f00 7500 7000 736d 6f44 4462 6c6f  p._.u.p.smoDDblo
+00001770: 6200 0000 0804 1204 40f3 0fc5 4100 0000  b.......@...A...
+00001780: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
+00001790: 6f64 4462 6c6f 6200 0000 0804 1204 40f3  odDblob.......@.
+000017a0: 0fc5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
+000017b0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
+000017c0: 0000 09f0 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
+000017d0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
+000017e0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001800: 0000 0000 0000 0003 0000 0000 0000 180b  ................
 00001810: 0000 0045 0000 100b 0000 0000 0000 0000  ...E............
 00001820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,57 +457,57 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 0064 5b64  .....@.......d[d
-00001d00: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
-00001d10: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-00001d20: 6f6e 546e 616d 655c 6461 7465 4d6f 6469  onTname\dateModi
-00001d30: 6669 6564 d418 191a 1b1c 0c1e 1f57 7669  fied.........Wvi
-00001d40: 7369 626c 6559 6173 6365 6e64 696e 6755  sibleYascendingU
-00001d50: 7769 6474 6855 696e 6465 7808 0911 012c  widthUindex....,
-00001d60: 1007 d418 191a 1b1c 1c23 2408 0810 c810  .........#$.....
-00001d70: 08d4 1819 1a1b 1c1c 2829 0808 10b5 1002  ........()......
-00001d80: d418 191a 1b0c 1c2d 2e09 0810 6110 03d4  .......-....a...
-00001d90: 1819 1a1b 1c0c 3233 0809 1064 1005 d418  ......23...d....
-00001da0: 191a 1b0c 0c37 3809 0910 7310 04d4 1819  .....78...s.....
-00001db0: 1a1b 1c0c 3c3d 0809 104b 1006 d418 191a  ....<=...K......
-00001dc0: 1b0c 0c1e 4109 0910 00d4 1819 1a1b 0c1c  ....A...........
-00001dd0: 280b 0908 0823 0000 0000 0000 0000 2340  (....#........#@
-00001de0: 2800 0000 0000 0023 4014 0000 0000 0000  (......#@.......
-00001df0: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
-00001e00: 0800 1d00 3200 4400 4c00 6000 7200 7b00  ....2.D.L.`.r.{.
-00001e10: 8d00 9800 ab00 b400 b600 b700 ca00 d300  ................
-00001e20: e200 ee00 f300 f900 fe01 0601 0b01 1801  ................
-00001e30: 2101 2901 3301 3901 3f01 4001 4101 4401  !.).3.9.?.@.A.D.
-00001e40: 4601 4f01 5001 5101 5301 5501 5e01 5f01  F.O.P.Q.S.U.^._.
-00001e50: 6001 6201 6401 6d01 6e01 6f01 7101 7301  `.b.d.m.n.o.q.s.
-00001e60: 7c01 7d01 7e01 8001 8201 8b01 8c01 8d01  |.}.~...........
-00001e70: 8f01 9101 9a01 9b01 9c01 9e01 a001 a901  ................
-00001e80: aa01 ab01 ad01 b601 b701 b801 b901 c201  ................
-00001e90: cb01 d401 d901 da00 0000 0000 0002 0100  ................
-00001ea0: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
-00001eb0: 0000 0000 0001 e300 0000 0b00 5f00 5f00  ............_._.
-00001ec0: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
-00001ed0: 5f76 5372 6e6c 6f6e 6700 0000 0100 0000  _vSrnlong.......
-00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cf0: 0000 0000 0140 0000 0000 0000 0077 5763  .....@.......wWc
+00001d00: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00001d10: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
+00001d20: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
+00001d30: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
+00001d40: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
+00001d50: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
+00001d60: 4461 7465 7358 6963 6f6e 5369 7a65 1001  DatesXiconSize..
+00001d70: 09d9 0e0f 1011 1213 1415 1617 2025 292d  ............ %)-
+00001d80: 3237 3c41 5863 6f6d 6d65 6e74 735e 6461  27<AXcomments^da
+00001d90: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
+00001da0: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
+00001db0: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+00001dc0: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+00001dd0: 6d65 d418 191a 1b1c 1d0c 1f57 7669 7369  me.........Wvisi
+00001de0: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
+00001df0: 696e 6755 696e 6465 7808 1101 2c09 1007  ingUindex...,...
+00001e00: d418 191a 1b1c 221c 2408 10c8 0810 08d4  ......".$.......
+00001e10: 1819 1a1b 0c27 1c0b 0910 b508 d418 191a  .....'..........
+00001e20: 1b1c 271c 2c08 0810 02d4 1819 1a1b 0c2f  ..'.,........../
+00001e30: 1c31 0910 6108 1003 d418 191a 1b1c 340c  .1..a.........4.
+00001e40: 3608 1064 0910 05d4 1819 1a1b 0c39 0c3b  6..d.........9.;
+00001e50: 0910 7309 1004 d418 191a 1b1c 3e0c 4008  ..s.........>.@.
+00001e60: 104b 0910 06d4 1819 1a1b 0c43 0c45 0911  .K.........C.E..
+00001e70: 01c7 0910 0008 2300 0000 0000 0000 0023  ......#........#
+00001e80: 4028 0000 0000 0000 5c64 6174 654d 6f64  @(......\dateMod
+00001e90: 6966 6965 6409 2340 3000 0000 0000 0000  ified.#@0.......
+00001ea0: 0800 1d00 3200 4400 4c00 6000 7200 7b00  ....2.D.L.`.r.{.
+00001eb0: 8d00 9800 ab00 b400 b600 b700 ca00 d300  ................
+00001ec0: e200 ef00 fb01 0001 0601 0b01 1301 1801  ................
+00001ed0: 2101 2901 2f01 3901 3f01 4001 4301 4401  !.)./.9.?.@.C.D.
+00001ee0: 4601 4f01 5001 5201 5301 5501 5e01 5f01  F.O.P.R.S.U.^._.
+00001ef0: 6101 6201 6b01 6c01 6d01 6f01 7801 7901  a.b.k.l.m.o.x.y.
+00001f00: 7b01 7c01 7e01 8701 8801 8a01 8b01 8d01  {.|.~...........
+00001f10: 9601 9701 9901 9a01 9c01 a501 a601 a801  ................
+00001f20: a901 ab01 b401 b501 b801 b901 bb01 bc01  ................
+00001f30: c501 ce01 db01 dc00 0000 0000 0002 0100  ................
+00001f40: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
+00001f50: 0000 0000 0001 e500 0000 0700 7000 6f00  ............p.o.
+00001f60: 7000 5f00 7500 7000 736d 6f44 4462 6c6f  p._.u.p.smoDDblo
+00001f70: 6200 0000 0804 1204 40f3 0fc5 4100 0000  b.......@...A...
+00001f80: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
+00001f90: 6f64 4462 6c6f 6200 0000 0804 1204 40f3  odDblob.......@.
+00001fa0: 0fc5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
+00001fb0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
+00001fc0: 0000 09f0 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
+00001fd0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
+00001fe0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.61.6/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.61.7/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.61.7/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.61.7/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.61.7/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.61.7/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.61.7/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.61.7/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.61.7/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.61.7/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.61.7/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.61.7/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/SimBA.py` & `Simba-UW-tf-dev-1.61.7/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.61.7/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.61.7/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.61.7/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.61.7/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.61.7/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.61.7/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.61.7/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.61.7/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.61.7/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.61.7/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.61.7/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.61.7/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.61.7/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.61.7/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.61.7/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.61.7/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.61.7/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.61.7/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.61.6
+Version: 1.61.7
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.61.6/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.61.7/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -178,14 +178,15 @@
 simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
 simba/feature_extractors/misc/graph_3d_plotter.py
 simba/feature_extractors/misc/graph_creator.py
 simba/feature_extractors/misc/make_splash.py
 simba/feature_extractors/misc/mutual_exclusive.py
 simba/feature_extractors/misc/peaks.py
 simba/feature_extractors/misc/read_in_mp.py
+simba/feature_extractors/misc/shap_log_mp.py
 simba/feature_extractors/misc/termite_rois.csv
 simba/feature_extractors/misc/time_stamp_calculator.py
 simba/feature_extractors/misc/video_color.py
 simba/feature_extractors/misc/video_rotator.py
 simba/feature_extractors/misc/video_rotator_mp.py
 simba/labelling/.DS_Store
 simba/labelling/__init__.py
```

### Comparing `Simba-UW-tf-dev-1.61.6/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.61.7/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/LICENSE.md` & `Simba-UW-tf-dev-1.61.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.61.7/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.61.7/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.61.7/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.61.7/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.61.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.61.7/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/README.md` & `Simba-UW-tf-dev-1.61.7/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.6/setup.py` & `Simba-UW-tf-dev-1.61.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.61.6",
+    version="1.61.7",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

