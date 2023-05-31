# Comparing `tmp/Simba-UW-tf-dev-1.61.8.tar.gz` & `tmp/Simba-UW-tf-dev-1.61.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.61.8.tar", last modified: Wed May 31 14:35:37 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.61.9.tar", last modified: Wed May 31 20:52:43 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.61.8.tar` & `Simba-UW-tf-dev-1.61.9.tar`

### file list

```diff
@@ -1,509 +1,511 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-30 12:37:26.000000 Simba-UW-tf-dev-1.61.8/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.61.8/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.61.8/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.8/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.61.8/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.8/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.8/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.61.8/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.61.8/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.61.8/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.61.8/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.61.8/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.8/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-29 21:05:41.000000 Simba-UW-tf-dev-1.61.8/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8741 2023-05-31 13:49:15.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8464 2023-05-31 14:17:45.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.61.8/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42902 2023-05-25 18:14:02.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    33507 2023-05-25 18:37:00.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1118 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9144 2023-05-28 17:30:45.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    67334 2023-05-31 14:17:45.000000 Simba-UW-tf-dev-1.61.8/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18514 2023-05-29 20:20:16.000000 Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.61.8/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20973 2023-05-25 13:55:35.000000 Simba-UW-tf-dev-1.61.8/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.8/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.8/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.61.8/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.61.8/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.61.8/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.61.8/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.61.8/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.61.8/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.61.8/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.8/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.8/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.8/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.61.8/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    13770 2023-05-23 16:26:11.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9274 2023-05-23 16:26:19.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.8/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.61.8/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19101 2023-05-30 20:48:53.000000 Simba-UW-tf-dev-1.61.8/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.61.8/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.8/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18879 2023-05-31 13:33:07.000000 Simba-UW-tf-dev-1.61.8/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.61.8/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.61.8/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.61.8/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.8/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.8/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.61.8/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.61.8/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.8/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.61.8/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.61.8/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.61.8/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8176 2023-05-25 14:24:49.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    65549 2023-05-25 18:24:18.000000 Simba-UW-tf-dev-1.61.8/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.61.8/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.61.8/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.61.8/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.61.8/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.61.8/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.61.8/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.61.8/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.8/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-31 14:35:36.000000 Simba-UW-tf-dev-1.61.8/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    18746 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-31 14:35:36.000000 Simba-UW-tf-dev-1.61.8/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-31 14:35:36.000000 Simba-UW-tf-dev-1.61.8/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-05-31 14:35:36.000000 Simba-UW-tf-dev-1.61.8/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-31 14:35:36.000000 Simba-UW-tf-dev-1.61.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.61.8/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.61.8/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.61.8/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.8/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.61.8/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.61.8/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.61.8/tests/test_featurizers.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.8/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/tests/data/test_projects/two_c57/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.8/tests/data/test_projects/two_c57/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.8/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.8/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.8/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.61.8/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.61.8/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.61.8/tests/test_thirdparty_appenders.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.61.8/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.61.8/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-31 14:35:35.000000 Simba-UW-tf-dev-1.61.8/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-31 14:35:37.000000 Simba-UW-tf-dev-1.61.8/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-30 12:37:26.000000 Simba-UW-tf-dev-1.61.9/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.61.9/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.61.9/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.9/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.61.9/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.9/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.9/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.61.9/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.61.9/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.61.9/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.61.9/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.61.9/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.9/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-31 16:51:24.000000 Simba-UW-tf-dev-1.61.9/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8509 2023-05-31 20:41:12.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.61.9/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42902 2023-05-25 18:14:02.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    33507 2023-05-25 18:37:00.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1118 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9144 2023-05-28 17:30:45.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    67184 2023-05-31 20:48:26.000000 Simba-UW-tf-dev-1.61.9/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18514 2023-05-29 20:20:16.000000 Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.61.9/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20973 2023-05-25 13:55:35.000000 Simba-UW-tf-dev-1.61.9/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.9/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.9/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.61.9/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.61.9/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.61.9/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.61.9/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.61.9/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.61.9/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.61.9/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.9/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.9/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.9/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.61.9/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    13770 2023-05-23 16:26:11.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9274 2023-05-23 16:26:19.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.9/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.61.9/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19101 2023-05-30 20:48:53.000000 Simba-UW-tf-dev-1.61.9/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.61.9/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.9/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18879 2023-05-31 13:33:07.000000 Simba-UW-tf-dev-1.61.9/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.61.9/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.61.9/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.61.9/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.9/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.9/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.61.9/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.61.9/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.9/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.61.9/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.61.9/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.61.9/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8176 2023-05-25 14:24:49.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    65549 2023-05-25 18:24:18.000000 Simba-UW-tf-dev-1.61.9/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.61.9/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.61.9/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.61.9/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.61.9/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.61.9/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.61.9/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.61.9/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.9/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    18808 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-31 20:52:42.000000 Simba-UW-tf-dev-1.61.9/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.61.9/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.61.9/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.61.9/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.61.9/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.9/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.61.9/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.61.9/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.61.9/tests/test_featurizers.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.9/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/tests/data/test_projects/two_c57/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.9/tests/data/test_projects/two_c57/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.9/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.9/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.9/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.61.9/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.61.9/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.61.9/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.61.9/tests/test_validation_clips.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.61.9/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.61.9/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-31 20:52:35.000000 Simba-UW-tf-dev-1.61.9/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-31 20:52:43.000000 Simba-UW-tf-dev-1.61.9/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.61.8/PKG-INFO` & `Simba-UW-tf-dev-1.61.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.61.8
+Version: 1.61.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,10 +161,10 @@
                                                         video_setting=self.distance_videos_var.get(),
                                                         final_img=self.distance_final_img_var.get(),
                                                         style_attr=style_attr,
                                                         files_found=data_paths,
                                                         line_attr=line_attr,
                                                         core_cnt=int(self.multiprocess_dropdown.getChoices()))
 
-        distance_plotter.create_distance_plot()
+        distance_plotter.run()
 
 #_ = DistancePlotterPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.61.9/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.61.9/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.61.9/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.61.9/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.61.9/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.61.9/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.61.9/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -1489,15 +1489,15 @@
 00005d00: 000f 0000 0000 0000 0000 0000 0000 0000  ................
 00005d10: 009a 0000 0012 0066 0065 0061 0074 0075  .......f.e.a.t.u
 00005d20: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d30: 0063 0074 006f 0072 0073 6473 636c 626f  .c.t.o.r.sdsclbo
 00005d40: 6f6c 0000 0000 1200 6600 6500 6100 7400  ol......f.e.a.t.
 00005d50: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
 00005d60: 6100 6300 7400 6f00 7200 736c 6731 5363  a.c.t.o.r.slg1Sc
-00005d70: 6f6d 7000 0000 0000 08ae 3a09 5863 6f6d  omp.......:.Xcom
+00005d70: 6f6d 7000 0000 0000 08f1 6f09 5863 6f6d  omp.......o.Xcom
 00005d80: 6d65 6e74 73d4 0d0e 0f10 163e 1640 0810  ments......>.@..
 00005d90: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
 00005da0: 64d4 0d0e 0f10 161c 1644 0808 5964 6174  d........D..Ydat
 00005db0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
 00005dc0: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
 00005dd0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
 00005de0: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
@@ -1582,19 +1582,19 @@
 000062d0: 0000 0000 0000 0000 0000 0001 e500 0000  ................
 000062e0: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000062f0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 00006300: 6f00 7200 736d 6f44 4462 6c6f 6200 0000  o.r.smoDDblob...
 00006310: 0869 3ef0 203f 0dc5 4100 0000 1200 6600  .i>. ?..A.....f.
 00006320: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
 00006330: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
-00006340: 736d 6f64 4462 6c6f 6200 0000 08cc d9f8  smodDblob.......
-00006350: 15cc 0cc5 4100 0000 1200 6600 6500 6100  ....A.....f.e.a.
+00006340: 736d 6f64 4462 6c6f 6200 0000 0869 3ef0  smodDblob....i>.
+00006350: 203f 0dc5 4100 0000 1200 6600 6500 6100   ?..A.....f.e.a.
 00006360: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00006370: 7200 6100 6300 7400 6f00 7200 7370 6831  r.a.c.t.o.r.sph1
-00006380: 5363 6f6d 7000 0000 0000 0a90 0000 0000  Scomp...........
+00006380: 5363 6f6d 7000 0000 0000 0af0 0000 0000  Scomp...........
 00006390: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000063a0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 000063b0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
 000063c0: 0100 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
 000063d0: 6c00 6900 6e00 6762 7773 7062 6c6f 6200  l.i.n.gbwspblob.
 000063e0: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 000063f0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
@@ -1714,15 +1714,15 @@
 00006b10: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
 00006b20: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
 00006b30: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
 00006b40: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
 00006b50: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 00006b60: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
 00006b70: 0000 0600 6d00 6900 7800 6900 6e00 736c  ....m.i.x.i.n.sl
-00006b80: 6731 5363 6f6d 7000 0000 0000 0826 1f00  g1Scomp......&..
+00006b80: 6731 5363 6f6d 7000 0000 0000 0850 5a00  g1Scomp......PZ.
 00006b90: 0000 0600 6d00 6900 7800 6900 6e00 736c  ....m.i.x.i.n.sl
 00006ba0: 7376 4362 6c6f 6200 0002 8162 706c 6973  svCblob....bplis
 00006bb0: 7430 30d8 0102 0304 0506 0708 090a 0b16  t00.............
 00006bc0: 4647 480a 5f10 1276 6965 774f 7074 696f  FGH._..viewOptio
 00006bd0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
 00006be0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
 00006bf0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
@@ -1788,20 +1788,20 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 2594 dda2 e311 c541  blob....%......A
+00007020: 626c 6f62 0000 0008 7fa4 e944 c713 c541  blob.......D...A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 f794 ee44  modDblob.......D
-00007050: dd11 c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 7fa4 e944  modDblob.......D
+00007050: c713 c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 0008 e000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
+00007070: 0009 1000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
@@ -1810,16 +1810,16 @@
 00007110: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 00007120: 6261 7208 0809 0809 5f10 187b 7b33 3335  bar....._..{{335
 00007130: 2c20 3139 387d 2c20 7b39 3237 2c20 3536  , 198}, {927, 56
 00007140: 387d 7d09 0817 2531 3d49 606d 797a 7b7c  8}}...%1=I`myz{|
 00007150: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
 00007160: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
 00007170: 0000 9a00 0000 0500 6d00 6f00 6400 6500  ........m.o.d.e.
-00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 012c  llg1Scomp......,
-00007190: b200 0000 0500 6d00 6f00 6400 6500 6c6c  ......m.o.d.e.ll
+00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 012d  llg1Scomp......-
+00007190: 0600 0000 0500 6d00 6f00 6400 6500 6c6c  ......m.o.d.e.ll
 000071a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
 000071b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
 000071c0: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
 000071d0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 000071e0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
 000071f0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
 00007200: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
@@ -1893,15 +1893,15 @@
 00007640: 014e 0150 0159 015a 015b 015d 015f 0168  .N.P.Y.Z.[.]._.h
 00007650: 0169 016a 016c 016e 0177 0178 0179 017b  .i.j.l.n.w.x.y.{
 00007660: 017d 0186 0187 0188 018a 018c 0195 0196  .}..............
 00007670: 0197 019a 019c 019d 01a6 01ab 0000 0000  ................
 00007680: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
 00007690: 0000 0000 0000 0000 0000 01ac 0000 0005  ................
 000076a0: 006d 006f 0064 0065 006c 6d6f 4444 626c  .m.o.d.e.lmoDDbl
-000076b0: 6f62 0000 0008 32f5 d3ed cc0c c541 0000  ob....2......A..
+000076b0: 6f62 0000 0008 0eab fd09 c213 c541 0000  ob...........A..
 000076c0: 0005 006d 006f 0064 0065 006c 6d6f 6444  ...m.o.d.e.lmodD
 000076d0: 626c 6f62 0000 0008 32f5 d3ed cc0c c541  blob....2......A
 000076e0: 0000 0005 006d 006f 0064 0065 006c 7068  .....m.o.d.e.lph
 000076f0: 3153 636f 6d70 0000 0000 0001 6000 0000  1Scomp......`...
 00007700: 0005 006d 006f 0064 0065 006c 7653 726e  ...m.o.d.e.lvSrn
 00007710: 6c6f 6e67 0000 0001 0000 000d 006f 0075  long.........o.u
 00007720: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
@@ -2029,21 +2029,21 @@
 00007ec0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00007ed0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
 00007ee0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
 00007ef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
 00007f00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
 00007f10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
 00007f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-00007f30: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
+00007f30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 00007f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 00007f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 00007f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 00007f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 00007f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-00007f90: 5363 6f6d 7000 0000 0000 08bf 7d00 0000  Scomp.......}...
+00007f90: 5363 6f6d 7000 0000 0000 08c2 1e00 0000  Scomp...........
 00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
@@ -2088,15 +2088,15 @@
 00008270: 7a01 7c01 7d01 7e01 8701 8901 8b01 8c01  z.|.}.~.........
 00008280: 8d01 9601 9801 9a01 9b01 9c01 a501 a701  ................
 00008290: a901 aa01 ab01 b401 b601 b901 ba01 bb01  ................
 000082a0: bc01 c501 ce01 db01 e400 0000 0000 0002  ................
 000082b0: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
 000082c0: 0000 0000 0000 0001 e500 0000 0800 7000  ..............p.
 000082d0: 6c00 6f00 7400 7400 6900 6e00 676d 6f44  l.o.t.t.i.n.gmoD
-000082e0: 4462 6c6f 6200 0000 08e6 e1c8 639f 12c5  Dblob.......c...
+000082e0: 4462 6c6f 6200 0000 08c4 1ccf bcd8 13c5  Dblob...........
 000082f0: 4100 0000 0800 7000 6c00 6f00 7400 7400  A.....p.l.o.t.t.
 00008300: 6900 6e00 676d 6f64 4462 6c6f 6200 0000  i.n.gmodDblob...
 00008310: 08e6 e1c8 639f 12c5 4100 0000 0800 7000  ....c...A.....p.
 00008320: 6c00 6f00 7400 7400 6900 6e00 6770 6831  l.o.t.t.i.n.gph1
 00008330: 5363 6f6d 7000 0000 0000 0ae0 0000 0000  Scomp...........
 00008340: 0800 7000 6c00 6f00 7400 7400 6900 6e00  ..p.l.o.t.t.i.n.
 00008350: 6776 5372 6e6c 6f6e 6700 0000 0100 0000  gvSrnlong.......
@@ -2285,21 +2285,21 @@
 00008ec0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00008ed0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
 00008ee0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
 00008ef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
 00008f00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
 00008f10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
 00008f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-00008f30: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
+00008f30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 00008f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 00008f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 00008f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 00008f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 00008f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-00008f90: 5363 6f6d 7000 0000 0000 08bf 7d00 0000  Scomp.......}...
+00008f90: 5363 6f6d 7000 0000 0000 08c2 1e00 0000  Scomp...........
 00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009000: 0000 0000 0000 0000 0000 0010 0000 000e  ................
@@ -2541,21 +2541,21 @@
 00009ec0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00009ed0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
 00009ee0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
 00009ef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
 00009f00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
 00009f10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
 00009f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-00009f30: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
+00009f30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 00009f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 00009f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 00009f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 00009f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 00009f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-00009f90: 5363 6f6d 7000 0000 0000 08bf 7d00 0000  Scomp.......}...
+00009f90: 5363 6f6d 7000 0000 0000 08c2 1e00 0000  Scomp...........
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000a000: 0000 0000 0000 0000 0000 0014 0000 0009  ................
@@ -2707,15 +2707,15 @@
 0000a920: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
 0000a930: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
 0000a940: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
 0000a950: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 0000a960: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
 0000a970: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
 0000a980: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000a990: 0000 0000 0009 72ef 0000 0002 0075 0069  ......r......u.i
+0000a990: 0000 0000 0009 737c 0000 0002 0075 0069  ......s|.....u.i
 0000a9a0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
 0000a9b0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 0000a9c0: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
 0000a9d0: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
 0000a9e0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
 0000a9f0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
 0000aa00: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
@@ -2797,21 +2797,21 @@
 0000aec0: 6c6f 6200 0000 0841 e3d5 bf76 0ec5 4100  lob....A...v..A.
 0000aed0: 0000 0200 7500 6970 6831 5363 6f6d 7000  ....u.iph1Scomp.
 0000aee0: 0000 0000 0c90 006f 6c62 6172 5b53 686f  .......olbar[Sho
 0000aef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
 0000af00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
 0000af10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
 0000af20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-0000af30: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
+0000af30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 0000af40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 0000af50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 0000af60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 0000af70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 0000af80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-0000af90: 5363 6f6d 7000 0000 0000 08bf 7d00 0000  Scomp.......}...
+0000af90: 5363 6f6d 7000 0000 0000 08c2 1e00 0000  Scomp...........
 0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000b000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
@@ -2963,15 +2963,15 @@
 0000b920: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
 0000b930: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
 0000b940: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
 0000b950: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 0000b960: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
 0000b970: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
 0000b980: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000b990: 0000 0000 0009 72ef 0000 0002 0075 0069  ......r......u.i
+0000b990: 0000 0000 0009 737c 0000 0002 0075 0069  ......s|.....u.i
 0000b9a0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
 0000b9b0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 0000b9c0: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
 0000b9d0: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
 0000b9e0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
 0000b9f0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
 0000ba00: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
@@ -3053,21 +3053,21 @@
 0000bec0: 6c6f 6200 0000 0841 e3d5 bf76 0ec5 4100  lob....A...v..A.
 0000bed0: 0000 0200 7500 6970 6831 5363 6f6d 7000  ....u.iph1Scomp.
 0000bee0: 0000 0000 0c90 006f 6c62 6172 5b53 686f  .......olbar[Sho
 0000bef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
 0000bf00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
 0000bf10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
 0000bf20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-0000bf30: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
+0000bf30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 0000bf40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 0000bf50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 0000bf60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 0000bf70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 0000bf80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-0000bf90: 5363 6f6d 7000 0000 0000 08bf 7d00 0000  Scomp.......}...
+0000bf90: 5363 6f6d 7000 0000 0000 08c2 1e00 0000  Scomp...........
 0000bfa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000c000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from itertools import repeat
 import os
 import shap
 import numpy as np
 from concurrent.futures import ProcessPoolExecutor
 from simba.utils.warnings import NotEnoughDataWarning
 from simba.plotting.shap_agg_stats_visualizer import ShapAggregateStatisticsVisualizer
-from joblib import Parallel, delayed
 
 
 
 
 def _create_shap_mp_helper(data: pd.DataFrame,
                     clf_name: str,
                     explainer: shap.TreeExplainer,
@@ -85,75 +84,71 @@
         cnt_absent = len(nontarget_df)
     non_target_for_shap = nontarget_df.sample(cnt_absent, replace=False)
     targets_for_shap = target_df.sample(cnt_present, replace=False)
     explainer = shap.TreeExplainer(rf_clf, data=None, model_output='raw', feature_perturbation='tree_path_dependent')
     expected_value = explainer.expected_value[1]
     cores, _ = find_core_cnt()
     shap_data_df = pd.concat([targets_for_shap, non_target_for_shap], axis=0)
-    if (len(shap_data_df) / batch_size) < 1: batch_size = 1
+    if (len(shap_data_df) / batch_size) < 1:
+        batch_size = 1
+    elif (len(shap_data_df) > 100) & (save_it >= 100):
+        batch_size = 100
     shap_data = np.array_split(shap_data_df, len(shap_data_df) / batch_size)
-    shap_results, shap_raw = [], []
-    shap_data, shap_raw = Parallel(n_jobs=cores, verbose=2, backend="multiprocessing")(delayed(_create_shap_mp_helper)(x, clf_name, explainer, rf_clf, expected_value) for x in shap_data)
-
-    #
-    #
-    #
-    #
-    #
-    # with ProcessPoolExecutor(int(np.ceil(cores / 2))) as pool:
-    #     for it_cnt, res in enumerate(pool.map(_create_shap_mp_helper, shap_data, repeat(clf_name), repeat(explainer), repeat(rf_clf), repeat(expected_value))):
-    #         shap_frm_timer = SimbaTimer(start=True)
-    #         shap_values, raw_values = res
-    #         shap_results.append(shap_values); shap_raw.append(raw_values)
-    #         data_size = int(len(shap_results)*batch_size)
-    #         if (data_size != 0) and (data_size % save_it == 0) or (data_size == len(shap_data_df)):
-    #             print(f'Saving SHAP data after {data_size} iterations...')
-    #             shap_save_df = pd.DataFrame(data=np.row_stack(shap_results), columns=list(x_names) + ['Expected_value', 'Sum', 'Prediction_probability', clf_name])
-    #             raw_save_df = pd.DataFrame(data=np.row_stack(shap_raw), columns=list(x_names))
-    #             shap_save_df.to_csv(out_df_shap_path)
-    #             raw_save_df.to_csv(out_df_raw_path)
-    #         shap_frm_timer.stop_timer()
-    #         print(f'SHAP frame: {data_size} / {len(shap_data_df)}, elapsed time: {shap_frm_timer.elapsed_time_str}...')
+    shap_results, shap_raw, processed_counter = [], [], 0
+    with ProcessPoolExecutor(int(np.ceil(cores / 2))) as pool:
+        for it_cnt, res in enumerate(pool.map(_create_shap_mp_helper, shap_data, repeat(clf_name), repeat(explainer), repeat(rf_clf), repeat(expected_value))):
+            shap_values, raw_values = res
+            shap_results.append(shap_values); shap_raw.append(raw_values)
+            processed_counter += shap_values.shape[0]
+            if (processed_counter != 0) and (processed_counter % save_it == 0) or (processed_counter == len(shap_data_df)):
+                print(f'Saving SHAP data after {processed_counter} iterations...')
+                shap_save_df = pd.DataFrame(data=np.row_stack(shap_results), columns=list(x_names) + ['Expected_value', 'Sum', 'Prediction_probability', clf_name])
+                raw_save_df = pd.DataFrame(data=np.row_stack(shap_raw), columns=list(x_names))
+                shap_save_df.to_csv(out_df_shap_path)
+                raw_save_df.to_csv(out_df_raw_path)
+            print(f'SHAP frame: {processed_counter} / {len(shap_data_df)}...')
 
     shap_timer.stop_timer()
     stdout_success(msg='SHAP calculations complete', elapsed_time=shap_timer.elapsed_time_str)
     _ = ShapAggregateStatisticsVisualizer(config_path=ini_file_path,
                                           classifier_name=clf_name,
                                           shap_df=shap_save_df,
                                           shap_baseline_value=int(expected_value * 100),
                                           save_path=save_path)
 
-data_path = '/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/csv/targets_inserted/122_SA_Day_03_20200705T1429.csv'
-data_df = pd.read_csv(data_path, index_col=0)
-clf_names = ['Attack', 'Escape', 'Defensive']
-# data_cols = [x for x in data_df.columns if not 'Probability_' in x]
-# data_cols = [x for x in data_cols if not x is 'Escape']
-# data_cols = [x for x in data_cols if not x is 'Defensive']
-data_df = data_df[list(data_df.columns)[:-2]]
-
-config = ConfigReader(config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini')
-
-x_df = data_df.drop(config.bp_col_names, axis=1)
-y_df = x_df.pop('Attack')
-
-ini_file_path = '/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini'
-rf_clf = read_df(file_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/models/generated_models/Attack.sav', file_type='pickle')
+
+if __name__ == '__main__':
+    data_path = '/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/csv/targets_inserted/122_SA_Day_03_20200705T1429.csv'
+    data_df = pd.read_csv(data_path, index_col=0)
+    clf_names = ['Attack', 'Escape', 'Defensive']
+    # data_cols = [x for x in data_df.columns if not 'Probability_' in x]
+    # data_cols = [x for x in data_cols if not x is 'Escape']
+    # data_cols = [x for x in data_cols if not x is 'Defensive']
+    data_df = data_df[list(data_df.columns)[:-2]]
+
+    config = ConfigReader(config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini')
+
+    x_df = data_df.drop(config.bp_col_names, axis=1)
+    y_df = x_df.pop('Attack')
+
+    ini_file_path = '/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini'
+    rf_clf = read_df(file_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/models/generated_models/Attack.sav', file_type='pickle')
 
 
 
-create_shap_log_mp(ini_file_path=ini_file_path,
-                rf_clf=rf_clf,
-                x_df=x_df,
-                y_df=y_df,
-                x_names=x_df.columns,
-                clf_name='Attack',
-                cnt_present=100,
-                cnt_absent=100,
-                save_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models',
-                save_it=200)
+    create_shap_log_mp(ini_file_path=ini_file_path,
+                    rf_clf=rf_clf,
+                    x_df=x_df,
+                    y_df=y_df,
+                    x_names=x_df.columns,
+                    clf_name='Attack',
+                    cnt_present=100,
+                    cnt_absent=100,
+                    save_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models',
+                    save_it=1000)
 
 
 # def create_shap_log(self,
 #                     ini_file_path: str,
 #                     rf_clf: RandomForestClassifier,
 #                     x_df: pd.DataFrame,
 #                     y_df: pd.DataFrame,
```

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import pandas as pd
 from sklearn.ensemble import RandomForestClassifier
 from simba.utils.read_write import read_df
 from typing import List, Optional
 from simba.utils.read_write import find_core_cnt
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import SimbaTimer, stdout_success
-from itertools import repeat
 import os
 import shap
 import numpy as np
 from concurrent.futures import ProcessPoolExecutor
 from simba.utils.warnings import NotEnoughDataWarning
 from simba.plotting.shap_agg_stats_visualizer import ShapAggregateStatisticsVisualizer
+from joblib import Parallel, delayed
+import multiprocessing
+import functools
+import concurrent
 
 
 
 
 def _create_shap_mp_helper(data: pd.DataFrame,
-                    clf_name: str,
-                    explainer: shap.TreeExplainer,
-                    clf: RandomForestClassifier,
-                    expected_value: float):
+                           explainer: shap.TreeExplainer,
+                           clf_name: str,
+                           rf_clf: RandomForestClassifier,
+                           expected_value: float):
 
     target = data.pop(clf_name).values.reshape(-1, 1)
     frame_batch_shap = explainer.shap_values(data.values, check_additivity=False)[1]
     shap_sum = np.sum(frame_batch_shap, axis=1).reshape(-1, 1)
-    proba = clf.predict_proba(data)[:, 1].reshape(-1, 1)
+    proba = rf_clf.predict_proba(data)[:, 1].reshape(-1, 1)
     frame_batch_shap = np.hstack((frame_batch_shap, np.full((frame_batch_shap.shape[0]), expected_value).reshape(-1, 1), shap_sum, proba, target))
     return frame_batch_shap, data.values[0]
 
 def create_shap_log_mp(ini_file_path: str,
                        rf_clf: RandomForestClassifier,
                        x_df: pd.DataFrame,
                        y_df: pd.DataFrame,
@@ -84,25 +87,22 @@
         cnt_absent = len(nontarget_df)
     non_target_for_shap = nontarget_df.sample(cnt_absent, replace=False)
     targets_for_shap = target_df.sample(cnt_present, replace=False)
     explainer = shap.TreeExplainer(rf_clf, data=None, model_output='raw', feature_perturbation='tree_path_dependent')
     expected_value = explainer.expected_value[1]
     cores, _ = find_core_cnt()
     shap_data_df = pd.concat([targets_for_shap, non_target_for_shap], axis=0)
-    if (len(shap_data_df) / batch_size) < 1:
-        batch_size = 1
-    elif (len(shap_data_df) > 100) & (save_it >= 100):
-        batch_size = 100
+    if (len(shap_data_df) / batch_size) < 1: batch_size = 1
     shap_data = np.array_split(shap_data_df, len(shap_data_df) / batch_size)
     shap_results, shap_raw, processed_counter = [], [], 0
-    with ProcessPoolExecutor(int(np.ceil(cores / 2))) as pool:
-        for it_cnt, res in enumerate(pool.map(_create_shap_mp_helper, shap_data, repeat(clf_name), repeat(explainer), repeat(rf_clf), repeat(expected_value))):
-            shap_values, raw_values = res
-            shap_results.append(shap_values); shap_raw.append(raw_values)
-            processed_counter += shap_values.shape[0]
+    with concurrent.futures.ProcessPoolExecutor(max_workers=cores) as executor:
+        futures = [executor.submit(_create_shap_mp_helper, data, explainer, clf_name, rf_clf, expected_value) for data in shap_data]
+        for future in concurrent.futures.as_completed(futures):
+            shap_results.append(future.result()[0]); shap_raw.append(future.result()[1])
+            processed_counter += future.result()[0].shape[0]
             if (processed_counter != 0) and (processed_counter % save_it == 0) or (processed_counter == len(shap_data_df)):
                 print(f'Saving SHAP data after {processed_counter} iterations...')
                 shap_save_df = pd.DataFrame(data=np.row_stack(shap_results), columns=list(x_names) + ['Expected_value', 'Sum', 'Prediction_probability', clf_name])
                 raw_save_df = pd.DataFrame(data=np.row_stack(shap_raw), columns=list(x_names))
                 shap_save_df.to_csv(out_df_shap_path)
                 raw_save_df.to_csv(out_df_raw_path)
             print(f'SHAP frame: {processed_counter} / {len(shap_data_df)}...')
@@ -138,15 +138,15 @@
                 x_df=x_df,
                 y_df=y_df,
                 x_names=x_df.columns,
                 clf_name='Attack',
                 cnt_present=100,
                 cnt_absent=100,
                 save_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models',
-                save_it=1000)
+                save_it=100)
 
 
 # def create_shap_log(self,
 #                     ini_file_path: str,
 #                     rf_clf: RandomForestClassifier,
 #                     x_df: pd.DataFrame,
 #                     y_df: pd.DataFrame,
```

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.61.9/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/requirements.txt` & `Simba-UW-tf-dev-1.61.9/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.61.9/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.61.9/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.61.9/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.61.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.61.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.61.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.61.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.61.9/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.61.9/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.61.9/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.61.9/simba/mixins/train_model_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from concurrent.futures import ProcessPoolExecutor
 from concurrent.futures.process import BrokenProcessPool
 from itertools import repeat
 import configparser
 import platform
 from sklearn.utils import parallel_backend
 import pickle
+import concurrent
 from dtreeviz.trees import tree, dtreeviz
 import matplotlib.pyplot as plt
 import multiprocessing
 from typing import List, Optional, Union, Dict, Any
 try:
     from typing import Literal
 except:
@@ -1079,28 +1080,26 @@
             results = pd.DataFrame.from_dict(data=results, orient='index')
             results.to_csv(save_log_path)
             raise FaultyTrainingSetError(
                 msg=f'{len(nan_cols)} feature columns exist in some files, but missing in others. The feature files are found in the project_folder/csv/targets_inserted directory. ' \
                     f'SimBA expects all files within the project_folder/csv/targets_inserted directory to have the same number of features: the first 10 ' \
                     f'column names with mismatches are: {nan_cols[0:9]}. For a log of the files that contain, and not contain, the mis-matched columns, see {save_log_path}')
 
-    def _create_shap_mp_helper(self,
-                               data: pd.DataFrame,
-                               clf_name: str,
+    @staticmethod
+    def _create_shap_mp_helper(data: pd.DataFrame,
                                explainer: shap.TreeExplainer,
-                               clf: RandomForestClassifier,
+                               clf_name: str,
+                               rf_clf: RandomForestClassifier,
                                expected_value: float):
 
         target = data.pop(clf_name).values.reshape(-1, 1)
         frame_batch_shap = explainer.shap_values(data.values, check_additivity=False)[1]
         shap_sum = np.sum(frame_batch_shap, axis=1).reshape(-1, 1)
-        proba = clf.predict_proba(data)[:, 1].reshape(-1, 1)
-        frame_batch_shap = np.hstack((frame_batch_shap,
-                                      np.full((frame_batch_shap.shape[0]), expected_value).reshape(-1, 1), shap_sum,
-                                      proba, target))
+        proba = rf_clf.predict_proba(data)[:, 1].reshape(-1, 1)
+        frame_batch_shap = np.hstack((frame_batch_shap, np.full((frame_batch_shap.shape[0]), expected_value).reshape(-1, 1), shap_sum, proba, target))
         return frame_batch_shap, data.values[0]
 
     def create_shap_log_mp(self,
                            ini_file_path: str,
                            rf_clf: RandomForestClassifier,
                            x_df: pd.DataFrame,
                            y_df: pd.DataFrame,
@@ -1163,31 +1162,28 @@
         cores, _ = find_core_cnt()
         shap_data_df = pd.concat([targets_for_shap, non_target_for_shap], axis=0)
         if (len(shap_data_df) / batch_size) < 1:
             batch_size = 1
         elif (len(shap_data_df) > 100) & (save_it >= 100):
             batch_size = 100
 
-
         shap_data = np.array_split(shap_data_df, len(shap_data_df) / batch_size)
         shap_results, shap_raw, processed_counter = [], [], 0
-        with ProcessPoolExecutor(cores) as pool:
-            for it_cnt, res in enumerate(pool.map(self._create_shap_mp_helper, shap_data, repeat(clf_name), repeat(explainer), repeat(rf_clf), repeat(expected_value))):
-                shap_values, raw_values = res
-                shap_results.append(shap_values); shap_raw.append(raw_values)
-                processed_counter += shap_values.shape[0]
+        with concurrent.futures.ProcessPoolExecutor(max_workers=cores) as executor:
+            futures = [executor.submit(self._create_shap_mp_helper, data, explainer, clf_name, rf_clf, expected_value) for data in shap_data]
+            for future in concurrent.futures.as_completed(futures):
+                shap_results.append(future.result()[0]); shap_raw.append(future.result()[1])
+                processed_counter += future.result()[0].shape[0]
                 if (processed_counter != 0) and (processed_counter % save_it == 0) or (processed_counter == len(shap_data_df)):
                     print(f'Saving SHAP data after {processed_counter} iterations...')
-                    shap_save_df = pd.DataFrame(data=np.row_stack(shap_results),
-                                                columns=list(x_names) + ['Expected_value', 'Sum',
-                                                                         'Prediction_probability', clf_name])
+                    shap_save_df = pd.DataFrame(data=np.row_stack(shap_results), columns=list(x_names) + ['Expected_value', 'Sum', 'Prediction_probability', clf_name])
                     raw_save_df = pd.DataFrame(data=np.row_stack(shap_raw), columns=list(x_names))
                     shap_save_df.to_csv(out_df_shap_path)
                     raw_save_df.to_csv(out_df_raw_path)
-                print(f'SHAP frame: {processed_counter} / {len(shap_data_df)} complete...')
+                print(f'SHAP frame: {processed_counter} / {len(shap_data_df)}...')
 
         shap_timer.stop_timer()
         stdout_success(msg='SHAP calculations complete', elapsed_time=shap_timer.elapsed_time_str)
         _ = ShapAggregateStatisticsVisualizer(config_path=ini_file_path,
                                               classifier_name=clf_name,
                                               shap_df=shap_save_df,
                                               shap_baseline_value=int(expected_value * 100),
```

### Comparing `Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.61.9/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.61.9/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.61.9/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/utils/enums.py` & `Simba-UW-tf-dev-1.61.9/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.61.9/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/utils/checks.py` & `Simba-UW-tf-dev-1.61.9/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.61.9/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.61.9/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.61.9/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/utils/errors.py` & `Simba-UW-tf-dev-1.61.9/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/utils/data.py` & `Simba-UW-tf-dev-1.61.9/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/utils/printing.py` & `Simba-UW-tf-dev-1.61.9/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/distance_plotter_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     .. note::
        `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
     Examples
     -----
     >>> style_attr = {'width': 640, 'height': 480, 'line width': 6, 'font size': 8, 'opacity': 0.5}
     >>> line_attr = {0: ['Center_1', 'Center_2', 'Green'], 1: ['Ear_left_2', 'Ear_left_1', 'Red']}
-    >>> _ = DistancePlotterMultiCore(config_path=r'/tests_/project_folder/project_config.ini', frame_setting=False, video_setting=True, final_img=True, style_attr=style_attr, line_attr=line_attr,  files_found=['/test_/project_folder/csv/machine_results/Together_1.csv'], core_cnt=5)
-
+    >>> distance_plotter = DistancePlotterMultiCore(config_path=r'/tests_/project_folder/project_config.ini', frame_setting=False, video_setting=True, final_img=True, style_attr=style_attr, line_attr=line_attr,  files_found=['/test_/project_folder/csv/machine_results/Together_1.csv'], core_cnt=5)
+    >>> distance_plotter.run()
     """
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
                  final_img: bool,
@@ -69,15 +69,15 @@
     @jit(nopython=True)
     def __insert_group_idx_column(data: np.array,
                                   group: int):
         group_col = np.full((data.shape[0], 1), group)
         return np.hstack((group_col, data))
 
 
-    def create_distance_plot(self):
+    def run(self):
         '''
         Creates line charts. Results are stored in the `project_folder/frames/line_plot` directory
 
         Returns
         ----------
         None
         '''
```

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/distance_plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,18 +27,20 @@
 
        `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
     :parameter str config_path: path to SimBA project config file in Configparser format.
     :parameter bool frame_setting: If True, creates individual frames.
     :parameter bool video_setting: If True, creates videos
 
-    Examples
-    -----
-    >>> distance_plotter = DistancePlotterSingleCore(config_path=r'MyProjectConfig', frame_setting=False, video_setting=True)
-    >>> distance_plotter.create_distance_plot()
+    :examples:
+
+    >>> style_attr = {'width': 640, 'height': 480, 'line width': 6, 'font size': 8, 'opacity': 0.5}
+    >>> line_attr = {0: ['Center_1', 'Center_2', 'Green'], 1: ['Ear_left_2', 'Ear_left_1', 'Red']}
+    >>> distance_plotter = DistancePlotterSingleCore(config_path=r'MyProjectConfig', files_found=['test/two_c57s/project_folder/csv/outlier_corrected_movement_location/Video_1.csv'], frame_setting=False, video_setting=True, final_img=True)
+    >>> distance_plotter.run()
     """
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
                  final_img: bool,
@@ -53,15 +55,15 @@
             raise NoSpecifiedOutputError('Please choice to create frames and/or video distance plots')
         self.colors_dict = get_color_dict()
         if not os.path.exists(self.line_plot_dir): os.makedirs(self.line_plot_dir)
         check_if_filepath_list_is_empty(filepaths=self.outlier_corrected_paths,
                                         error_msg='SIMBA ERROR: Zero files found in the project_folder/csv/machine_results directory. Create classification results before visualizing distances.')
         print(f'Processing {str(len(self.files_found))} videos...')
 
-    def create_distance_plot(self):
+    def run(self):
         '''
         Creates line charts. Results are stored in the `project_folder/frames/line_plot` directory
 
         Returns
         ----------
         None
         '''
```

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.61.9/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.61.9/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.61.9/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.61.9/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.61.9/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.61.9/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.61.9/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.61.9/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.61.9/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.61.9/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.61.9/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.61.9/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.61.9/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.61.9/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.61.9/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.61.9/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.61.9/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.61.9/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.61.9/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.61.9/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.61.9/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.61.9/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.61.9/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/SimBA.py` & `Simba-UW-tf-dev-1.61.9/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.61.9/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.61.9/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.61.9/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.61.9/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.61.9/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.61.9/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.61.9/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.61.9/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.61.9/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.61.9/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.61.9/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.61.9/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.61.9/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.61.9/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.61.9/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.61.9/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.61.9/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.61.9/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.61.8
+Version: 1.61.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.61.8/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.61.9/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -431,17 +431,19 @@
 simba/video_processors/extract_frames.py
 simba/video_processors/extract_seqframes.py
 simba/video_processors/multi_cropper.py
 simba/video_processors/px_to_mm.py
 simba/video_processors/video_processing.py
 tests/__init__.py
 tests/test_data_processors.py
+tests/test_distance_plotter.py
 tests/test_featurizers.py
 tests/test_outlier_correctors.py
 tests/test_thirdparty_appenders.py
+tests/test_validation_clips.py
 tests/test_visualize_directing_animals.py
 tests/data/__init__.py
 tests/data/test_projects/__init__.py
 tests/data/test_projects/mouse_open_field/__init__.py
 tests/data/test_projects/two_c57/__init__.py
 tests/data/test_projects/zebrafish/__init__.py
 tests/data/test_projects/zebrafish/feature_file/__init__.py
```

### Comparing `Simba-UW-tf-dev-1.61.8/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.61.9/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/LICENSE.md` & `Simba-UW-tf-dev-1.61.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.61.9/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.61.9/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.61.9/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.61.9/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.61.9/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.61.9/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/README.md` & `Simba-UW-tf-dev-1.61.9/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.8/setup.py` & `Simba-UW-tf-dev-1.61.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.61.8",
+    version="1.61.9",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

