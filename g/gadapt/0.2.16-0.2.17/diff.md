# Comparing `tmp/gadapt-0.2.16.tar.gz` & `tmp/gadapt-0.2.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gadapt-0.2.16.tar", last modified: Mon May 29 20:08:10 2023, max compression
+gzip compressed data, was "dist\gadapt-0.2.17.tar", last modified: Wed May 31 14:56:47 2023, max compression
```

## Comparing `gadapt-0.2.16.tar` & `gadapt-0.2.17.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.496283 gadapt-0.2.16/
--rw-rw-rw-   0        0        0    21690 2023-05-29 20:08:10.496783 gadapt-0.2.16/PKG-INFO
--rw-rw-rw-   0        0        0    19352 2023-05-29 09:13:58.000000 gadapt-0.2.16/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:09.962781 gadapt-0.2.16/gadapt/
--rw-rw-rw-   0        0        0        2 2023-05-24 06:11:19.000000 gadapt-0.2.16/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.018279 gadapt-0.2.16/gadapt/cost_finding/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:46.000000 gadapt-0.2.16/gadapt/cost_finding/__init__.py
--rw-rw-rw-   0        0        0      728 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     2112 2023-05-24 06:54:25.000000 gadapt-0.2.16/gadapt/cost_finding/common_cost_finder.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.037782 gadapt-0.2.16/gadapt/crossover/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:39.000000 gadapt-0.2.16/gadapt/crossover/__init__.py
--rw-rw-rw-   0        0        0     7034 2023-05-28 13:24:31.000000 gadapt-0.2.16/gadapt/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1257 2023-05-23 23:45:14.000000 gadapt-0.2.16/gadapt/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.047281 gadapt-0.2.16/gadapt/execution/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:34.000000 gadapt-0.2.16/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3233 2023-05-27 11:13:47.000000 gadapt-0.2.16/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.082782 gadapt-0.2.16/gadapt/exit_check/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:29.000000 gadapt-0.2.16/gadapt/exit_check/__init__.py
--rw-rw-rw-   0        0        0      315 2023-05-23 23:28:45.000000 gadapt-0.2.16/gadapt/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1060 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      305 2023-05-23 23:28:54.000000 gadapt-0.2.16/gadapt/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      387 2023-05-23 23:29:00.000000 gadapt-0.2.16/gadapt/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.093782 gadapt-0.2.16/gadapt/factory/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:24.000000 gadapt-0.2.16/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0     9949 2023-05-28 13:25:45.000000 gadapt-0.2.16/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0     8920 2023-05-28 13:38:36.000000 gadapt-0.2.16/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.104282 gadapt-0.2.16/gadapt/ga_logging/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:17.000000 gadapt-0.2.16/gadapt/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-05-24 07:42:21.000000 gadapt-0.2.16/gadapt/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.184281 gadapt-0.2.16/gadapt/ga_model/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:07.000000 gadapt-0.2.16/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     6671 2023-05-28 13:24:31.000000 gadapt-0.2.16/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0      680 2023-05-28 13:25:45.000000 gadapt-0.2.16/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     5248 2023-05-25 16:08:26.000000 gadapt-0.2.16/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     1398 2023-05-24 16:01:11.000000 gadapt-0.2.16/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     1339 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0     2546 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/ga_model/genetic_variable.py
--rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.16/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    10169 2023-05-24 16:00:25.000000 gadapt-0.2.16/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0      785 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.201282 gadapt-0.2.16/gadapt/gene_combination/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:01.000000 gadapt-0.2.16/gadapt/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      308 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0      837 2023-05-23 23:22:44.000000 gadapt-0.2.16/gadapt/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.203282 gadapt-0.2.16/gadapt/immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 00:04:24.000000 gadapt-0.2.16/gadapt/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.232282 gadapt-0.2.16/gadapt/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:55.000000 gadapt-0.2.16/gadapt/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      611 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      336 2023-05-23 23:22:33.000000 gadapt-0.2.16/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.249784 gadapt-0.2.16/gadapt/immigration/population_immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:43.000000 gadapt-0.2.16/gadapt/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0      174 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0      831 2023-05-23 23:22:20.000000 gadapt-0.2.16/gadapt/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.251282 gadapt-0.2.16/gadapt/mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 00:04:04.000000 gadapt-0.2.16/gadapt/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.279784 gadapt-0.2.16/gadapt/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:32.000000 gadapt-0.2.16/gadapt/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0      841 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
--rw-rw-rw-   0        0        0     2938 2023-05-24 06:54:25.000000 gadapt-0.2.16/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
--rw-rw-rw-   0        0        0      936 2023-05-23 23:45:26.000000 gadapt-0.2.16/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.328783 gadapt-0.2.16/gadapt/mutation/population_mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:12.000000 gadapt-0.2.16/gadapt/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0     1402 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/mutation/population_mutation/base_population_mutator.py
--rw-rw-rw-   0        0        0     1269 2023-05-23 23:43:50.000000 gadapt-0.2.16/gadapt/mutation/population_mutation/composed_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.338784 gadapt-0.2.16/gadapt/mutation/population_mutation/cost_diversity/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:26.000000 gadapt-0.2.16/gadapt/mutation/population_mutation/cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     2899 2023-05-24 06:54:25.000000 gadapt-0.2.16/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     1976 2023-05-28 15:09:04.000000 gadapt-0.2.16/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.360283 gadapt-0.2.16/gadapt/mutation/population_mutation/previous_cost_diversity/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:19.000000 gadapt-0.2.16/gadapt/mutation/population_mutation/previous_cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     3769 2023-05-24 06:54:24.000000 gadapt-0.2.16/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0      469 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_property_taker.py
--rw-rw-rw-   0        0        0     1069 2023-05-23 23:46:12.000000 gadapt-0.2.16/gadapt/mutation/population_mutation/random_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.379783 gadapt-0.2.16/gadapt/parent_selection/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:56.000000 gadapt-0.2.16/gadapt/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      299 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0      883 2023-05-23 23:20:13.000000 gadapt-0.2.16/gadapt/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.423285 gadapt-0.2.16/gadapt/sampling/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:48.000000 gadapt-0.2.16/gadapt/sampling/__init__.py
--rw-rw-rw-   0        0        0      707 2023-05-24 06:38:53.000000 gadapt-0.2.16/gadapt/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      433 2023-05-23 23:19:58.000000 gadapt-0.2.16/gadapt/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      425 2023-05-23 23:46:22.000000 gadapt-0.2.16/gadapt/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1812 2023-05-23 23:46:32.000000 gadapt-0.2.16/gadapt/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2622 2023-05-23 23:46:42.000000 gadapt-0.2.16/gadapt/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.433784 gadapt-0.2.16/gadapt/string_operation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:11:28.000000 gadapt-0.2.16/gadapt/string_operation/__init__.py
--rw-rw-rw-   0        0        0     3219 2023-05-24 06:41:20.000000 gadapt-0.2.16/gadapt/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.455283 gadapt-0.2.16/gadapt/utils/
--rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.16/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:32.000000 gadapt-0.2.16/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     1272 2023-05-25 15:37:31.000000 gadapt-0.2.16/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.477283 gadapt-0.2.16/gadapt/validation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:26.000000 gadapt-0.2.16/gadapt/validation/__init__.py
--rw-rw-rw-   0        0        0      787 2023-05-24 06:45:03.000000 gadapt-0.2.16/gadapt/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    17413 2023-05-28 13:25:45.000000 gadapt-0.2.16/gadapt/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:10.494783 gadapt-0.2.16/gadapt/variable_update/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:11.000000 gadapt-0.2.16/gadapt/variable_update/__init__.py
--rw-rw-rw-   0        0        0      176 2023-05-24 06:38:52.000000 gadapt-0.2.16/gadapt/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     2001 2023-05-24 06:54:25.000000 gadapt-0.2.16/gadapt/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:08:09.999280 gadapt-0.2.16/gadapt.egg-info/
--rw-rw-rw-   0        0        0    21690 2023-05-29 20:08:09.000000 gadapt-0.2.16/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3460 2023-05-29 20:08:09.000000 gadapt-0.2.16/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 20:08:09.000000 gadapt-0.2.16/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 20:08:09.000000 gadapt-0.2.16/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-05-29 20:08:10.498785 gadapt-0.2.16/setup.cfg
--rw-rw-rw-   0        0        0      465 2023-05-29 20:07:06.000000 gadapt-0.2.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.302404 gadapt-0.2.17/
+-rw-rw-rw-   0        0        0    21692 2023-05-31 14:56:47.302904 gadapt-0.2.17/PKG-INFO
+-rw-rw-rw-   0        0        0    19354 2023-05-31 09:31:35.000000 gadapt-0.2.17/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.015403 gadapt-0.2.17/gadapt/
+-rw-rw-rw-   0        0        0        2 2023-05-24 06:11:19.000000 gadapt-0.2.17/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.129404 gadapt-0.2.17/gadapt/cost_finding/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:46.000000 gadapt-0.2.17/gadapt/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0      728 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     2112 2023-05-24 06:54:25.000000 gadapt-0.2.17/gadapt/cost_finding/common_cost_finder.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.166903 gadapt-0.2.17/gadapt/crossover/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:39.000000 gadapt-0.2.17/gadapt/crossover/__init__.py
+-rw-rw-rw-   0        0        0     7034 2023-05-28 13:24:31.000000 gadapt-0.2.17/gadapt/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1257 2023-05-23 23:45:14.000000 gadapt-0.2.17/gadapt/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.169404 gadapt-0.2.17/gadapt/execution/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:34.000000 gadapt-0.2.17/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3233 2023-05-27 11:13:47.000000 gadapt-0.2.17/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.177905 gadapt-0.2.17/gadapt/exit_check/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:29.000000 gadapt-0.2.17/gadapt/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      315 2023-05-23 23:28:45.000000 gadapt-0.2.17/gadapt/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1060 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      305 2023-05-23 23:28:54.000000 gadapt-0.2.17/gadapt/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      387 2023-05-23 23:29:00.000000 gadapt-0.2.17/gadapt/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.180904 gadapt-0.2.17/gadapt/factory/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:24.000000 gadapt-0.2.17/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0     9949 2023-05-28 13:25:45.000000 gadapt-0.2.17/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0     8920 2023-05-28 13:38:36.000000 gadapt-0.2.17/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.184903 gadapt-0.2.17/gadapt/ga_logging/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:17.000000 gadapt-0.2.17/gadapt/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-05-24 07:42:21.000000 gadapt-0.2.17/gadapt/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.202404 gadapt-0.2.17/gadapt/ga_model/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:07.000000 gadapt-0.2.17/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     6671 2023-05-28 13:24:31.000000 gadapt-0.2.17/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0      680 2023-05-28 13:25:45.000000 gadapt-0.2.17/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     5248 2023-05-25 16:08:26.000000 gadapt-0.2.17/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     1398 2023-05-24 16:01:11.000000 gadapt-0.2.17/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     1339 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0     2546 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/ga_model/genetic_variable.py
+-rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.17/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    10169 2023-05-24 16:00:25.000000 gadapt-0.2.17/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0      785 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.205903 gadapt-0.2.17/gadapt/gene_combination/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:01.000000 gadapt-0.2.17/gadapt/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      308 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0      837 2023-05-23 23:22:44.000000 gadapt-0.2.17/gadapt/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.208404 gadapt-0.2.17/gadapt/immigration/
+-rw-rw-rw-   0        0        0        0 2023-05-24 00:04:24.000000 gadapt-0.2.17/gadapt/immigration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.216904 gadapt-0.2.17/gadapt/immigration/chromosome_immigration/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:55.000000 gadapt-0.2.17/gadapt/immigration/chromosome_immigration/__init__.py
+-rw-rw-rw-   0        0        0      611 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
+-rw-rw-rw-   0        0        0      336 2023-05-23 23:22:33.000000 gadapt-0.2.17/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.223403 gadapt-0.2.17/gadapt/immigration/population_immigration/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:43.000000 gadapt-0.2.17/gadapt/immigration/population_immigration/__init__.py
+-rw-rw-rw-   0        0        0      174 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/immigration/population_immigration/base_population_immigrator.py
+-rw-rw-rw-   0        0        0      831 2023-05-23 23:22:20.000000 gadapt-0.2.17/gadapt/immigration/population_immigration/common_population_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.224904 gadapt-0.2.17/gadapt/mutation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 00:04:04.000000 gadapt-0.2.17/gadapt/mutation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.229904 gadapt-0.2.17/gadapt/mutation/chromosome_mutation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:32.000000 gadapt-0.2.17/gadapt/mutation/chromosome_mutation/__init__.py
+-rw-rw-rw-   0        0        0      841 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
+-rw-rw-rw-   0        0        0     2938 2023-05-24 06:54:25.000000 gadapt-0.2.17/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
+-rw-rw-rw-   0        0        0      936 2023-05-23 23:45:26.000000 gadapt-0.2.17/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.237405 gadapt-0.2.17/gadapt/mutation/population_mutation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:12.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/__init__.py
+-rw-rw-rw-   0        0        0     1402 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/base_population_mutator.py
+-rw-rw-rw-   0        0        0     1269 2023-05-23 23:43:50.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/composed_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.239405 gadapt-0.2.17/gadapt/mutation/population_mutation/cost_diversity/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:26.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/cost_diversity/__init__.py
+-rw-rw-rw-   0        0        0     2899 2023-05-24 06:54:25.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     1976 2023-05-28 15:09:04.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.259404 gadapt-0.2.17/gadapt/mutation/population_mutation/previous_cost_diversity/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:19.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/previous_cost_diversity/__init__.py
+-rw-rw-rw-   0        0        0     3769 2023-05-24 06:54:24.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0      469 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_property_taker.py
+-rw-rw-rw-   0        0        0     1069 2023-05-23 23:46:12.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/random_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.268404 gadapt-0.2.17/gadapt/parent_selection/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:56.000000 gadapt-0.2.17/gadapt/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      299 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0      883 2023-05-23 23:20:13.000000 gadapt-0.2.17/gadapt/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.285905 gadapt-0.2.17/gadapt/sampling/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:48.000000 gadapt-0.2.17/gadapt/sampling/__init__.py
+-rw-rw-rw-   0        0        0      707 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      433 2023-05-23 23:19:58.000000 gadapt-0.2.17/gadapt/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      425 2023-05-23 23:46:22.000000 gadapt-0.2.17/gadapt/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1812 2023-05-23 23:46:32.000000 gadapt-0.2.17/gadapt/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2622 2023-05-23 23:46:42.000000 gadapt-0.2.17/gadapt/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.288404 gadapt-0.2.17/gadapt/string_operation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:11:28.000000 gadapt-0.2.17/gadapt/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     3219 2023-05-24 06:41:20.000000 gadapt-0.2.17/gadapt/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.292405 gadapt-0.2.17/gadapt/utils/
+-rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.17/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:32.000000 gadapt-0.2.17/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1272 2023-05-25 15:37:31.000000 gadapt-0.2.17/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.296905 gadapt-0.2.17/gadapt/validation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:26.000000 gadapt-0.2.17/gadapt/validation/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-05-24 06:45:03.000000 gadapt-0.2.17/gadapt/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    17413 2023-05-28 13:25:45.000000 gadapt-0.2.17/gadapt/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.301406 gadapt-0.2.17/gadapt/variable_update/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:11.000000 gadapt-0.2.17/gadapt/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      176 2023-05-24 06:38:52.000000 gadapt-0.2.17/gadapt/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2001 2023-05-24 06:54:25.000000 gadapt-0.2.17/gadapt/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.123925 gadapt-0.2.17/gadapt.egg-info/
+-rw-rw-rw-   0        0        0    21692 2023-05-31 14:56:46.000000 gadapt-0.2.17/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3460 2023-05-31 14:56:46.000000 gadapt-0.2.17/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 14:56:46.000000 gadapt-0.2.17/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 14:56:46.000000 gadapt-0.2.17/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-31 14:56:47.304905 gadapt-0.2.17/setup.cfg
+-rw-rw-rw-   0        0        0      465 2023-05-31 09:29:04.000000 gadapt-0.2.17/setup.py
```

### Comparing `gadapt-0.2.16/PKG-INFO` & `gadapt-0.2.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.2.16
+Version: 0.2.17
 Summary: GAdapt: A Python Library for Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 License: UNKNOWN
 Description: # GAdapt: Self-Adaptive Genetic Algorithm
         **GAdapt** (https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
@@ -62,15 +62,15 @@
         2: 86.4
         3: 0.0
         4: 1.0
         5: 3.14
         6: -1.0
         ```
         
-        In this example, the genetic algorithm searches for the combination of six parameters, bringing the lowest value for the passed function. The only mandatory attribute to the genetic algorithm is *cost_function*, and other attributes in this example took default values. Parameters to be optimized are added by the "add" method. There are seven parameters to be optimized in this example.
+        In this example, the genetic algorithm searches for the combination of seven parameters, bringing the lowest value for the passed function. The only mandatory attribute to the genetic algorithm is *cost_function*, and other attributes in this example took default values. Parameters to be optimized are added by the "add" method. There are seven parameters to be optimized in this example.
         # Parameter Settings
         GAdapt genetic algorithm can receive parameters using constructor, properties, or combined.
         
         Passing parameters through the class constructor:
         ```python
         ga = GA(cost_function=trig_func,
             population_size=32,
@@ -103,15 +103,15 @@
         ga.number_of_mutation_genes=2
         ga.exit_check="min_cost"
         ga.max_attempt_no=20
         ga.logging=True
         ga.timeout=3600
         ```
         # Parameters description
-        **cost_function**=*None* - Custom function for the fitness calculation (cost). The optimisation goal is minimising the output of the cost function. *cost_function* must be the function with one argument - a dictionary of values, where the key is an index (the ordinal of adding parameters) and the key is the parameter's value to be optimised. When adding parameters, there should be as many parameters as the function uses. The *cost_function* is the only mandatory parameter.
+        **cost_function**=*None* - Custom function for the cost calculation (fitness). The optimisation goal is minimising the output of the cost function. *cost_function* must be the function with one argument - a dictionary of values, where the key is an index (the ordinal of adding parameters) and the key is the parameter's value to be optimised. When adding parameters, there should be as many parameters as the function uses. The *cost_function* is the only mandatory parameter.
         
         **population_size**=*64* - Number of chromosomes in the population.
         
         **exit_check**=*"avg_cost"* - A criteria for the exit for the genetic algorithm.  
         Supported values:
         - *"avg_cost"* - The optimisation exit is triggered when the average cost of the upper half of the population is not improved in the specified number of generations  
         - *"min_cost"* - The optimisation exit is triggered when the minimal cost in the population is not improved in the specified number of generations
```

### Comparing `gadapt-0.2.16/README.md` & `gadapt-0.2.17/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 2: 86.4
 3: 0.0
 4: 1.0
 5: 3.14
 6: -1.0
 ```
 
-In this example, the genetic algorithm searches for the combination of six parameters, bringing the lowest value for the passed function. The only mandatory attribute to the genetic algorithm is *cost_function*, and other attributes in this example took default values. Parameters to be optimized are added by the "add" method. There are seven parameters to be optimized in this example.
+In this example, the genetic algorithm searches for the combination of seven parameters, bringing the lowest value for the passed function. The only mandatory attribute to the genetic algorithm is *cost_function*, and other attributes in this example took default values. Parameters to be optimized are added by the "add" method. There are seven parameters to be optimized in this example.
 # Parameter Settings
 GAdapt genetic algorithm can receive parameters using constructor, properties, or combined.
 
 Passing parameters through the class constructor:
 ```python
 ga = GA(cost_function=trig_func,
     population_size=32,
@@ -95,15 +95,15 @@
 ga.number_of_mutation_genes=2
 ga.exit_check="min_cost"
 ga.max_attempt_no=20
 ga.logging=True
 ga.timeout=3600
 ```
 # Parameters description
-**cost_function**=*None* - Custom function for the fitness calculation (cost). The optimisation goal is minimising the output of the cost function. *cost_function* must be the function with one argument - a dictionary of values, where the key is an index (the ordinal of adding parameters) and the key is the parameter's value to be optimised. When adding parameters, there should be as many parameters as the function uses. The *cost_function* is the only mandatory parameter.
+**cost_function**=*None* - Custom function for the cost calculation (fitness). The optimisation goal is minimising the output of the cost function. *cost_function* must be the function with one argument - a dictionary of values, where the key is an index (the ordinal of adding parameters) and the key is the parameter's value to be optimised. When adding parameters, there should be as many parameters as the function uses. The *cost_function* is the only mandatory parameter.
 
 **population_size**=*64* - Number of chromosomes in the population.
 
 **exit_check**=*"avg_cost"* - A criteria for the exit for the genetic algorithm.  
 Supported values:
 - *"avg_cost"* - The optimisation exit is triggered when the average cost of the upper half of the population is not improved in the specified number of generations  
 - *"min_cost"* - The optimisation exit is triggered when the minimal cost in the population is not improved in the specified number of generations
```

### Comparing `gadapt-0.2.16/gadapt/cost_finding/base_cost_finder.py` & `gadapt-0.2.17/gadapt/cost_finding/base_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/cost_finding/common_cost_finder.py` & `gadapt-0.2.17/gadapt/cost_finding/common_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/crossover/base_crossover.py` & `gadapt-0.2.17/gadapt/crossover/base_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/crossover/uniform_crossover.py` & `gadapt-0.2.17/gadapt/crossover/uniform_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/execution/ga_executor.py` & `gadapt-0.2.17/gadapt/execution/ga_executor.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/exit_check/base_exit_checker.py` & `gadapt-0.2.17/gadapt/exit_check/base_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/factory/ga_factory.py` & `gadapt-0.2.17/gadapt/factory/ga_factory.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/ga.py` & `gadapt-0.2.17/gadapt/ga.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/ga_logging/logging_settings.py` & `gadapt-0.2.17/gadapt/ga_logging/logging_settings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/ga_model/chromosome.py` & `gadapt-0.2.17/gadapt/ga_model/chromosome.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/ga_model/definitions.py` & `gadapt-0.2.17/gadapt/ga_model/definitions.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/ga_model/ga_options.py` & `gadapt-0.2.17/gadapt/ga_model/ga_options.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/ga_model/ga_results.py` & `gadapt-0.2.17/gadapt/ga_model/ga_results.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/ga_model/gene.py` & `gadapt-0.2.17/gadapt/ga_model/gene.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/ga_model/genetic_variable.py` & `gadapt-0.2.17/gadapt/ga_model/genetic_variable.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/ga_model/population.py` & `gadapt-0.2.17/gadapt/ga_model/population.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/ga_model/ranking_model.py` & `gadapt-0.2.17/gadapt/ga_model/ranking_model.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/gene_combination/blending_gene_combination.py` & `gadapt-0.2.17/gadapt/gene_combination/blending_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py` & `gadapt-0.2.17/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/immigration/population_immigration/common_population_immigrator.py` & `gadapt-0.2.17/gadapt/immigration/population_immigration/common_population_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py` & `gadapt-0.2.17/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py` & `gadapt-0.2.17/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py` & `gadapt-0.2.17/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/mutation/population_mutation/base_population_mutator.py` & `gadapt-0.2.17/gadapt/mutation/population_mutation/base_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/mutation/population_mutation/composed_population_mutator.py` & `gadapt-0.2.17/gadapt/mutation/population_mutation/composed_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py` & `gadapt-0.2.17/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py` & `gadapt-0.2.17/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py` & `gadapt-0.2.17/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/mutation/population_mutation/random_population_mutator.py` & `gadapt-0.2.17/gadapt/mutation/population_mutation/random_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/parent_selection/sampling_parent_selector.py` & `gadapt-0.2.17/gadapt/parent_selection/sampling_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/sampling/base_sampling.py` & `gadapt-0.2.17/gadapt/sampling/base_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/sampling/roulette_wheel_sampling.py` & `gadapt-0.2.17/gadapt/sampling/roulette_wheel_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/sampling/tournament_sampling.py` & `gadapt-0.2.17/gadapt/sampling/tournament_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/string_operation/ga_strings.py` & `gadapt-0.2.17/gadapt/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/utils/ga_utils.py` & `gadapt-0.2.17/gadapt/utils/ga_utils.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/validation/base_options_validator.py` & `gadapt-0.2.17/gadapt/validation/base_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/validation/common_options_validator.py` & `gadapt-0.2.17/gadapt/validation/common_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt/variable_update/common_variable_updater.py` & `gadapt-0.2.17/gadapt/variable_update/common_variable_updater.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.16/gadapt.egg-info/PKG-INFO` & `gadapt-0.2.17/gadapt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.2.16
+Version: 0.2.17
 Summary: GAdapt: A Python Library for Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 License: UNKNOWN
 Description: # GAdapt: Self-Adaptive Genetic Algorithm
         **GAdapt** (https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
@@ -62,15 +62,15 @@
         2: 86.4
         3: 0.0
         4: 1.0
         5: 3.14
         6: -1.0
         ```
         
-        In this example, the genetic algorithm searches for the combination of six parameters, bringing the lowest value for the passed function. The only mandatory attribute to the genetic algorithm is *cost_function*, and other attributes in this example took default values. Parameters to be optimized are added by the "add" method. There are seven parameters to be optimized in this example.
+        In this example, the genetic algorithm searches for the combination of seven parameters, bringing the lowest value for the passed function. The only mandatory attribute to the genetic algorithm is *cost_function*, and other attributes in this example took default values. Parameters to be optimized are added by the "add" method. There are seven parameters to be optimized in this example.
         # Parameter Settings
         GAdapt genetic algorithm can receive parameters using constructor, properties, or combined.
         
         Passing parameters through the class constructor:
         ```python
         ga = GA(cost_function=trig_func,
             population_size=32,
@@ -103,15 +103,15 @@
         ga.number_of_mutation_genes=2
         ga.exit_check="min_cost"
         ga.max_attempt_no=20
         ga.logging=True
         ga.timeout=3600
         ```
         # Parameters description
-        **cost_function**=*None* - Custom function for the fitness calculation (cost). The optimisation goal is minimising the output of the cost function. *cost_function* must be the function with one argument - a dictionary of values, where the key is an index (the ordinal of adding parameters) and the key is the parameter's value to be optimised. When adding parameters, there should be as many parameters as the function uses. The *cost_function* is the only mandatory parameter.
+        **cost_function**=*None* - Custom function for the cost calculation (fitness). The optimisation goal is minimising the output of the cost function. *cost_function* must be the function with one argument - a dictionary of values, where the key is an index (the ordinal of adding parameters) and the key is the parameter's value to be optimised. When adding parameters, there should be as many parameters as the function uses. The *cost_function* is the only mandatory parameter.
         
         **population_size**=*64* - Number of chromosomes in the population.
         
         **exit_check**=*"avg_cost"* - A criteria for the exit for the genetic algorithm.  
         Supported values:
         - *"avg_cost"* - The optimisation exit is triggered when the average cost of the upper half of the population is not improved in the specified number of generations  
         - *"min_cost"* - The optimisation exit is triggered when the minimal cost in the population is not improved in the specified number of generations
```

### Comparing `gadapt-0.2.16/gadapt.egg-info/SOURCES.txt` & `gadapt-0.2.17/gadapt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

