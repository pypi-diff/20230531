# Comparing `tmp/dp4plus_app-0.1.3.tar.gz` & `tmp/dp4plus_app-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp4plus_app-0.1.3.tar", last modified: Wed May 24 19:44:42 2023, max compression
+gzip compressed data, was "dp4plus_app-0.1.4.tar", last modified: Wed May 31 15:03:51 2023, max compression
```

## Comparing `dp4plus_app-0.1.3.tar` & `dp4plus_app-0.1.4.tar`

### file list

```diff
@@ -1,134 +1,146 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 19:44:42.183916 dp4plus_app-0.1.3/
--rw-rw-rw-   0        0        0     1092 2023-03-10 18:45:01.000000 dp4plus_app-0.1.3/LICENCE
--rw-rw-rw-   0        0        0     4710 2023-05-24 19:44:42.182938 dp4plus_app-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4136 2023-05-24 19:44:27.000000 dp4plus_app-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 19:44:42.184891 dp4plus_app-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2000 2023-05-24 19:43:44.000000 dp4plus_app-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:44:40.897740 dp4plus_app-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 19:44:41.109661 dp4plus_app-0.1.3/src/dp4plus_app/
-drwxrwxrwx   0        0        0        0 2023-05-24 19:44:41.217087 dp4plus_app-0.1.3/src/dp4plus_app/UserGuide/
--rw-rw-rw-   0        0        0  2019530 2023-05-24 16:22:12.000000 dp4plus_app-0.1.3/src/dp4plus_app/UserGuide/UserGuide.docx
--rw-rw-rw-   0        0        0  1000915 2023-05-24 16:22:39.000000 dp4plus_app-0.1.3/src/dp4plus_app/UserGuide/UserGuide.pdf
--rw-rw-rw-   0        0        0   684479 2023-05-24 18:42:29.000000 dp4plus_app-0.1.3/src/dp4plus_app/UserGuide/UserGuideFigures.pptx
--rw-rw-rw-   0        0        0        0 2023-03-23 20:21:29.000000 dp4plus_app-0.1.3/src/dp4plus_app/__init__.py
--rw-rw-rw-   0        0        0     9392 2023-05-23 19:18:37.000000 dp4plus_app-0.1.3/src/dp4plus_app/bugs_a_warning_module.py
--rw-rw-rw-   0        0        0     9506 2023-05-24 18:48:39.000000 dp4plus_app-0.1.3/src/dp4plus_app/correlation_module.py
--rw-rw-rw-   0        0        0    18484 2023-05-24 18:36:04.000000 dp4plus_app-0.1.3/src/dp4plus_app/custom_gui_module.py
--rw-rw-rw-   0        0        0     8513 2023-05-24 18:48:30.000000 dp4plus_app-0.1.3/src/dp4plus_app/custom_module.py
--rw-rw-rw-   0        0        0    13610 2023-05-24 18:19:35.000000 dp4plus_app-0.1.3/src/dp4plus_app/data_base_Custom.xlsx
--rw-rw-rw-   0        0        0    61121 2023-05-16 14:51:37.000000 dp4plus_app-0.1.3/src/dp4plus_app/data_base_MM.xlsx
--rw-rw-rw-   0        0        0    42509 2023-02-28 18:07:42.000000 dp4plus_app-0.1.3/src/dp4plus_app/data_base_QM.xlsx
--rw-rw-rw-   0        0        0     7267 2023-05-24 18:48:21.000000 dp4plus_app-0.1.3/src/dp4plus_app/dp4_module.py
--rw-rw-rw-   0        0        0    73188 2023-03-07 17:33:34.000000 dp4plus_app-0.1.3/src/dp4plus_app/logo_CONICET.png
--rw-rw-rw-   0        0        0    21045 2023-03-07 17:09:01.000000 dp4plus_app-0.1.3/src/dp4plus_app/logo_INGEBIO.png
--rw-rw-rw-   0        0        0     3589 2023-05-24 18:48:00.000000 dp4plus_app-0.1.3/src/dp4plus_app/main.py
--rw-rw-rw-   0        0        0    18960 2023-05-24 18:37:34.000000 dp4plus_app-0.1.3/src/dp4plus_app/main_gui_module.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:44:41.242480 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/
--rw-rw-rw-   0        0        0    36731 2023-03-15 19:25:14.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx
--rw-rw-rw-   0        0        0    67105 2023-03-14 13:31:40.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/custom_molecules_set.docx
-drwxrwxrwx   0        0        0        0 2023-05-24 19:44:41.309864 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/
--rw-rw-rw-   0        0        0      588 2023-03-09 17:59:12.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_TMS_optB.gjc
--rw-rw-rw-   0        0        0      529 2023-03-09 17:59:12.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_optB.gjc
--rw-rw-rw-   0        0        0     1057 2023-03-09 17:59:12.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_optB.gjc
--rw-rw-rw-   0        0        0     1539 2023-03-09 17:59:12.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_optB.gjc
--rw-rw-rw-   0        0        0     1531 2023-03-09 17:59:12.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_optB.gjc
--rw-rw-rw-   0        0        0      750 2023-03-09 17:59:12.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_optB.gjc
--rw-rw-rw-   0        0        0     1032 2023-03-09 17:59:12.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_optB.gjc
--rw-rw-rw-   0        0        0     1368 2023-03-09 17:59:12.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_optB.gjc
--rw-rw-rw-   0        0        0     1716 2023-03-09 17:59:12.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_optB.gjc
-drwxrwxrwx   0        0        0        0 2023-05-24 19:44:41.433891 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/
--rw-rw-rw-   0        0        0      588 2022-10-04 14:19:04.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/0_TMS_Custom_MMFF.gjc
--rw-rw-rw-   0        0        0      529 2022-10-04 14:19:04.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_MMFF.gjc
--rw-rw-rw-   0        0        0     1057 2022-10-04 14:19:04.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_MMFF.gjc
--rw-rw-rw-   0        0        0     1539 2022-10-04 14:19:04.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_MMFF.gjc
--rw-rw-rw-   0        0        0     1534 2022-10-04 14:19:06.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_MMFF.gjc
--rw-rw-rw-   0        0        0      749 2022-10-04 14:19:04.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_MMFF.gjc
--rw-rw-rw-   0        0        0     1030 2022-10-04 14:19:16.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_MMFF.gjc
--rw-rw-rw-   0        0        0     1369 2022-10-04 14:19:08.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_MMFF.gjc
--rw-rw-rw-   0        0        0     1712 2022-10-04 14:19:10.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_MMFF.gjc
-drwxrwxrwx   0        0        0        0 2023-05-24 19:44:42.172195 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/
--rw-rw-rw-   0        0        0    16107 2023-03-13 19:26:08.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a - copia.xlsx
--rw-rw-rw-   0        0        0    62190 2022-05-17 17:47:26.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62202 2022-05-17 17:59:17.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62133 2022-05-17 18:10:35.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62150 2022-05-17 18:21:10.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62411 2022-05-17 18:31:50.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62149 2022-05-17 18:42:51.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62608 2022-05-17 18:54:27.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62119 2022-05-17 19:06:23.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62121 2022-05-17 19:17:42.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62114 2022-05-17 19:29:29.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62393 2022-05-17 19:40:13.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62174 2022-05-17 19:51:50.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62373 2022-05-17 20:02:41.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62105 2022-05-17 20:14:06.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62116 2022-05-17 20:24:59.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62115 2022-05-17 20:35:55.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62446 2022-05-17 20:46:44.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62187 2022-05-17 20:57:46.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62154 2022-05-17 21:08:39.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62493 2022-05-17 18:10:10.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62148 2022-05-17 18:40:52.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62142 2022-05-17 19:11:10.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62196 2022-05-17 19:40:30.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62042 2022-05-17 20:09:33.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62182 2022-05-17 20:38:31.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62183 2022-05-17 21:08:56.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62120 2022-05-17 21:39:48.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62186 2022-05-17 22:10:41.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62172 2022-05-17 22:41:37.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62078 2022-05-17 23:14:34.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62352 2022-05-17 23:49:30.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62156 2022-05-18 00:18:50.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62159 2022-05-18 00:52:59.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62114 2022-05-18 01:23:09.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62635 2022-05-18 01:55:00.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62125 2022-05-18 02:27:45.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62530 2022-05-18 02:58:42.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62375 2022-05-18 03:34:04.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62140 2022-05-17 18:21:07.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62059 2022-05-17 18:56:41.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    61990 2022-05-17 19:26:23.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62108 2022-05-17 19:53:58.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62035 2022-05-17 20:19:33.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62125 2022-05-17 20:47:31.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62189 2022-05-17 21:16:05.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62289 2022-05-17 21:40:37.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62204 2022-05-17 22:05:51.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62168 2022-05-17 22:33:21.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62204 2022-05-17 23:01:32.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62373 2022-05-17 23:36:01.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62132 2022-05-18 00:05:25.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62094 2022-05-18 00:41:01.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62003 2022-05-18 01:14:58.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62114 2022-05-18 01:51:51.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62174 2022-05-18 02:25:20.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62111 2022-05-18 03:04:33.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62153 2022-05-18 03:34:21.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62159 2022-05-17 18:26:26.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62110 2022-05-17 18:32:41.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62223 2022-05-17 18:39:11.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62314 2022-05-17 18:46:00.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62290 2022-05-17 18:52:29.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62120 2022-05-17 18:59:07.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62387 2022-05-17 19:05:40.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62437 2022-05-17 19:12:26.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62096 2022-05-17 19:18:31.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    66884 2022-05-17 19:25:09.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62111 2022-05-17 19:31:38.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62040 2022-05-17 19:37:41.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62317 2022-05-17 19:44:23.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62120 2022-05-17 19:51:02.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62010 2022-05-17 19:57:03.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62101 2022-05-17 20:03:32.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62045 2022-05-17 20:10:05.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    63152 2022-05-17 20:16:50.000000 dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    10839 2023-05-24 18:47:37.000000 dp4plus_app-0.1.3/src/dp4plus_app/output_module.py
--rw-rw-rw-   0        0        0     5113 2023-05-24 18:48:16.000000 dp4plus_app-0.1.3/src/dp4plus_app/validation_module.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:44:41.173140 dp4plus_app-0.1.3/src/dp4plus_app.egg-info/
--rw-rw-rw-   0        0        0     4710 2023-05-24 19:44:40.000000 dp4plus_app-0.1.3/src/dp4plus_app.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6225 2023-05-24 19:44:40.000000 dp4plus_app-0.1.3/src/dp4plus_app.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 19:44:40.000000 dp4plus_app-0.1.3/src/dp4plus_app.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-05-24 19:44:40.000000 dp4plus_app-0.1.3/src/dp4plus_app.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2023-05-24 19:44:40.000000 dp4plus_app-0.1.3/src/dp4plus_app.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-24 19:44:40.000000 dp4plus_app-0.1.3/src/dp4plus_app.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 15:03:51.830796 dp4plus_app-0.1.4/
+-rw-rw-rw-   0        0        0     1092 2023-03-10 18:45:01.000000 dp4plus_app-0.1.4/LICENCE
+-rw-rw-rw-   0        0        0     4710 2023-05-31 15:03:51.830796 dp4plus_app-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4136 2023-05-24 19:44:27.000000 dp4plus_app-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 15:03:51.830796 dp4plus_app-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1990 2023-05-31 14:46:02.000000 dp4plus_app-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:03:48.352635 dp4plus_app-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 15:03:48.502543 dp4plus_app-0.1.4/src/dp4plus_app/
+drwxrwxrwx   0        0        0        0 2023-05-31 15:03:49.410782 dp4plus_app-0.1.4/src/dp4plus_app/UserGuide/
+-rw-rw-rw-   0        0        0  2019530 2023-05-24 16:22:12.000000 dp4plus_app-0.1.4/src/dp4plus_app/UserGuide/UserGuide.docx
+-rw-rw-rw-   0        0        0  1000915 2023-05-24 16:22:39.000000 dp4plus_app-0.1.4/src/dp4plus_app/UserGuide/UserGuide.pdf
+-rw-rw-rw-   0        0        0   684479 2023-05-24 18:42:29.000000 dp4plus_app-0.1.4/src/dp4plus_app/UserGuide/UserGuideFigures.pptx
+-rw-rw-rw-   0        0        0        0 2023-03-23 20:21:29.000000 dp4plus_app-0.1.4/src/dp4plus_app/__init__.py
+-rw-rw-rw-   0        0        0     9392 2023-05-23 19:18:37.000000 dp4plus_app-0.1.4/src/dp4plus_app/bugs_a_warning_module.py
+-rw-rw-rw-   0        0        0     9506 2023-05-24 18:48:39.000000 dp4plus_app-0.1.4/src/dp4plus_app/correlation_module.py
+-rw-rw-rw-   0        0        0    18484 2023-05-24 18:36:04.000000 dp4plus_app-0.1.4/src/dp4plus_app/custom_gui_module.py
+-rw-rw-rw-   0        0        0     8540 2023-05-31 14:53:49.000000 dp4plus_app-0.1.4/src/dp4plus_app/custom_module.py
+-rw-rw-rw-   0        0        0    13662 2023-05-31 15:03:06.000000 dp4plus_app-0.1.4/src/dp4plus_app/data_base_Custom.xlsx
+-rw-rw-rw-   0        0        0    61121 2023-05-16 14:51:37.000000 dp4plus_app-0.1.4/src/dp4plus_app/data_base_MM.xlsx
+-rw-rw-rw-   0        0        0    42509 2023-02-28 18:07:42.000000 dp4plus_app-0.1.4/src/dp4plus_app/data_base_QM.xlsx
+-rw-rw-rw-   0        0        0     7269 2023-05-30 17:36:59.000000 dp4plus_app-0.1.4/src/dp4plus_app/dp4_module.py
+-rw-rw-rw-   0        0        0    73188 2023-03-07 17:33:34.000000 dp4plus_app-0.1.4/src/dp4plus_app/logo_CONICET.png
+-rw-rw-rw-   0        0        0    21045 2023-03-07 17:09:01.000000 dp4plus_app-0.1.4/src/dp4plus_app/logo_INGEBIO.png
+-rw-rw-rw-   0        0        0     3589 2023-05-24 18:48:00.000000 dp4plus_app-0.1.4/src/dp4plus_app/main.py
+-rw-rw-rw-   0        0        0    18960 2023-05-24 18:37:34.000000 dp4plus_app-0.1.4/src/dp4plus_app/main_gui_module.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:03:49.416130 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/
+-rw-rw-rw-   0        0        0    36815 2023-05-31 14:49:36.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx
+-rw-rw-rw-   0        0        0    67105 2023-03-14 13:31:40.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/custom_molecules_set.docx
+drwxrwxrwx   0        0        0        0 2023-05-31 15:03:49.816046 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/
+-rw-rw-rw-   0        0        0      588 2023-03-09 17:59:12.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc
+-rw-rw-rw-   0        0        0      529 2023-03-09 17:59:12.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1057 2023-03-09 17:59:12.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1539 2023-03-09 17:59:12.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1537 2023-03-15 13:03:00.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc
+-rw-rw-rw-   0        0        0     1531 2023-03-09 17:59:12.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1530 2023-03-15 13:03:00.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc
+-rw-rw-rw-   0        0        0      750 2023-03-09 17:59:12.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1032 2023-03-09 17:59:12.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1368 2023-03-09 17:59:12.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1372 2023-03-15 13:03:00.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc
+-rw-rw-rw-   0        0        0     1374 2023-03-15 13:03:00.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc
+-rw-rw-rw-   0        0        0     1384 2023-03-15 13:03:00.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc
+-rw-rw-rw-   0        0        0     1716 2023-03-09 17:59:12.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1725 2023-03-15 13:03:00.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc
+drwxrwxrwx   0        0        0        0 2023-05-31 15:03:49.856086 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/
+-rw-rw-rw-   0        0        0      588 2022-10-04 14:19:04.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc
+-rw-rw-rw-   0        0        0      529 2022-10-04 14:19:04.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1057 2022-10-04 14:19:04.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1539 2022-10-04 14:19:04.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1536 2022-10-04 14:19:04.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc
+-rw-rw-rw-   0        0        0     1534 2022-10-04 14:19:06.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1529 2022-10-04 14:19:06.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc
+-rw-rw-rw-   0        0        0      749 2022-10-04 14:19:04.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1030 2022-10-04 14:19:16.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1369 2022-10-04 14:19:08.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1372 2022-10-04 14:19:08.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc
+-rw-rw-rw-   0        0        0     1376 2022-10-04 14:19:08.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc
+-rw-rw-rw-   0        0        0     1382 2022-10-04 14:19:08.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc
+-rw-rw-rw-   0        0        0     1712 2022-10-04 14:19:10.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1724 2022-10-04 14:19:10.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc
+drwxrwxrwx   0        0        0        0 2023-05-31 15:03:51.825885 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/
+-rw-rw-rw-   0        0        0    16107 2023-03-13 19:26:08.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a - copia.xlsx
+-rw-rw-rw-   0        0        0    62190 2022-05-17 17:47:26.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62202 2022-05-17 17:59:17.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62133 2022-05-17 18:10:35.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62150 2022-05-17 18:21:10.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62411 2022-05-17 18:31:50.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62149 2022-05-17 18:42:51.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62608 2022-05-17 18:54:27.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62119 2022-05-17 19:06:23.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62121 2022-05-17 19:17:42.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62114 2022-05-17 19:29:29.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62393 2022-05-17 19:40:13.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62174 2022-05-17 19:51:50.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62373 2022-05-17 20:02:41.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62105 2022-05-17 20:14:06.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62116 2022-05-17 20:24:59.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62115 2022-05-17 20:35:55.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62446 2022-05-17 20:46:44.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62187 2022-05-17 20:57:46.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62154 2022-05-17 21:08:39.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62493 2022-05-17 18:10:10.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62148 2022-05-17 18:40:52.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62142 2022-05-17 19:11:10.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62196 2022-05-17 19:40:30.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62042 2022-05-17 20:09:33.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62182 2022-05-17 20:38:31.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62183 2022-05-17 21:08:56.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62120 2022-05-17 21:39:48.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62186 2022-05-17 22:10:41.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62172 2022-05-17 22:41:37.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62078 2022-05-17 23:14:34.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62352 2022-05-17 23:49:30.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62156 2022-05-18 00:18:50.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62159 2022-05-18 00:52:59.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62114 2022-05-18 01:23:09.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62635 2022-05-18 01:55:00.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62125 2022-05-18 02:27:45.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62530 2022-05-18 02:58:42.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62375 2022-05-18 03:34:04.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62140 2022-05-17 18:21:07.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62059 2022-05-17 18:56:41.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    61990 2022-05-17 19:26:23.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62108 2022-05-17 19:53:58.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62035 2022-05-17 20:19:33.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62125 2022-05-17 20:47:31.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62189 2022-05-17 21:16:05.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62289 2022-05-17 21:40:37.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62204 2022-05-17 22:05:51.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62168 2022-05-17 22:33:21.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62204 2022-05-17 23:01:32.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62373 2022-05-17 23:36:01.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62132 2022-05-18 00:05:25.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62094 2022-05-18 00:41:01.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62003 2022-05-18 01:14:58.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62114 2022-05-18 01:51:51.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62174 2022-05-18 02:25:20.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62111 2022-05-18 03:04:33.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62153 2022-05-18 03:34:21.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62159 2022-05-17 18:26:26.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62110 2022-05-17 18:32:41.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62223 2022-05-17 18:39:11.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62314 2022-05-17 18:46:00.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62290 2022-05-17 18:52:29.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62120 2022-05-17 18:59:07.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62387 2022-05-17 19:05:40.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62437 2022-05-17 19:12:26.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62096 2022-05-17 19:18:31.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    66884 2022-05-17 19:25:09.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62111 2022-05-17 19:31:38.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62040 2022-05-17 19:37:41.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62317 2022-05-17 19:44:23.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62120 2022-05-17 19:51:02.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62010 2022-05-17 19:57:03.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62101 2022-05-17 20:03:32.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62045 2022-05-17 20:10:05.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    63152 2022-05-17 20:16:50.000000 dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    10835 2023-05-29 19:47:47.000000 dp4plus_app-0.1.4/src/dp4plus_app/output_module.py
+-rw-rw-rw-   0        0        0     5113 2023-05-24 18:48:16.000000 dp4plus_app-0.1.4/src/dp4plus_app/validation_module.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:03:48.570906 dp4plus_app-0.1.4/src/dp4plus_app.egg-info/
+-rw-rw-rw-   0        0        0     4710 2023-05-31 15:03:47.000000 dp4plus_app-0.1.4/src/dp4plus_app.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7047 2023-05-31 15:03:47.000000 dp4plus_app-0.1.4/src/dp4plus_app.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 15:03:47.000000 dp4plus_app-0.1.4/src/dp4plus_app.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-05-31 15:03:47.000000 dp4plus_app-0.1.4/src/dp4plus_app.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      125 2023-05-31 15:03:47.000000 dp4plus_app-0.1.4/src/dp4plus_app.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-31 15:03:47.000000 dp4plus_app-0.1.4/src/dp4plus_app.egg-info/top_level.txt
```

### Comparing `dp4plus_app-0.1.3/LICENCE` & `dp4plus_app-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/PKG-INFO` & `dp4plus_app-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp4plus_app
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool to simplify your DP4+ calculations
 Home-page: https://github.com/RosarioCCLab/DP4plus-App
 Author: Bruno A. Franco
 Author-email: bruno.agustin.franco@gmail.com
 License: MIT
 Keywords: nmr
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dp4plus_app-0.1.3/README.md` & `dp4plus_app-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/setup.py` & `dp4plus_app-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,33 +2,28 @@
 """
 Created on Mon Mar 27 12:15:45 2023
 
 @author: Franco, Bruno Agustín 
 
 """
 
-
-
-
 ### AGREGAR RELATIVE IMPORTS
 
 ### OCULTAR TRAZABILIDAD DEL TRAINING
 
-
-
 from setuptools import setup, find_namespace_packages
 
 with open('README.md') as file:         #sirve para incluir el REEDME
     long_description = file.read()
 
 short_description = 'A tool to simplify your DP4+ calculations'
 
 setup(
     name='dp4plus_app',
-    version='0.1.3',
+    version='0.1.4',
     
     author='Bruno A. Franco',
     author_email='bruno.agustin.franco@gmail.com',
     url='https://github.com/RosarioCCLab/DP4plus-App',
     description =short_description	,
     long_description = long_description,
     long_description_content_type ="text/markdown",
```

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/UserGuide/UserGuide.docx` & `dp4plus_app-0.1.4/src/dp4plus_app/UserGuide/UserGuide.docx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/UserGuide/UserGuide.pdf` & `dp4plus_app-0.1.4/src/dp4plus_app/UserGuide/UserGuide.pdf`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/UserGuide/UserGuideFigures.pptx` & `dp4plus_app-0.1.4/src/dp4plus_app/UserGuide/UserGuideFigures.pptx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/bugs_a_warning_module.py` & `dp4plus_app-0.1.4/src/dp4plus_app/bugs_a_warning_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/correlation_module.py` & `dp4plus_app-0.1.4/src/dp4plus_app/correlation_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/custom_gui_module.py` & `dp4plus_app-0.1.4/src/dp4plus_app/custom_gui_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/custom_module.py` & `dp4plus_app-0.1.4/src/dp4plus_app/custom_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,24 +67,25 @@
     return param
 
 def get_command():
     '''saves the command line of 10% of the files used in the 
     parameterization
     '''
     files= glob.glob('*nmr*.log') + glob.glob('*nmr*.out')
-    choose = sample(files, len(files)//10)
+    choose = sample(files, (len(files)//10)+1 )
     g09command =[]
     
     for file in choose: 
         with open(file,'r') as to_read: 
                 for row in to_read.readlines(): 
                     if '#' in row:   
                         g09command.append(row)
                         break
                     
+                    
     g09command = Counter(g09command).most_common()[0][0]
     return g09command
 
 def n_warning (param): 
     '''Generates a popup window that allows you to change the degrees of 
     freedom obtained by other averages.
     This function is usually called when the sampling points are very few
```

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/data_base_Custom.xlsx` & `dp4plus_app-0.1.4/src/dp4plus_app/data_base_Custom.xlsx`

 * *Files 14% similar despite different names*

```diff
@@ -351,501 +351,504 @@
 000015e0: 7c1f ccf3 bf98 e6dd b707 180f 47b3 86c3  |...........G...
 000015f0: ccd7 7db2 7d8a 3747 5b8a 071b 177e 370d  ..}.}.7G[....~7.
 00001600: 20ec 61ec d368 1c9c c761 e0e5 a741 e88d   .a..h...a...A..
 00001610: c664 e24d c6a7 b197 c761 b41c 8fe6 1771  .d.M.....a.....q
 00001620: 1e0f 628f dff8 fd08 fc30 dc7f 3fda 309e  ..b......0..?.0.
 00001630: 1926 2867 72cf d59e a1a1 1548 82ed 2f92  .&(gr......H../.
 00001640: f0f7 4cf8 c70f 7bf6 0300 00ff ff03 0050  ..L...{........P
-00001650: 4b03 0414 0006 0008 0000 0021 00fb ed03  K..........!....
-00001660: d299 0200 00ad 0500 0018 0000 0078 6c2f  .............xl/
+00001650: 4b03 0414 0006 0008 0000 0021 00fe ec43  K..........!...C
+00001660: 95cc 0200 0091 0600 0018 0000 0078 6c2f  .............xl/
 00001670: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00001680: 312e 786d 6c8c 945b 4fdb 3014 c7df 27ed  1.xml..[O.0...'.
-00001690: 3b58 7e27 374a a155 5324 e8ba 218d 695a  ;X~'7J.US$..!.iZ
-000016a0: 7779 769c 93c6 22c9 c96c b7a5 7cfa 1d3b  wyv..."..l..|..;
-000016b0: 490b 2a43 bcc4 767c fc3b ff73 b167 d78f  I.*C..v|.;.s.g..
-000016c0: 75c5 b6a0 8dc2 26e5 7110 7106 8dc4 5c35  u.....&.q.q...\5
-000016d0: eb94 fffa b93c bbe2 cc58 d1e4 a2c2 0652  .....<...X.....R
-000016e0: be07 c3af e71f 3fcc 76a8 1f4c 0960 1911  ......?.v..L.`..
-000016f0: 1a93 f2d2 da76 1a86 4696 500b 1360 0b0d  .....v..F.P..`..
-00001700: ed14 a86b 6169 a9d7 a169 3588 dc1f aaab  ...kai...i5.....
-00001710: 3089 a271 580b d5f0 8e30 d5ef 6160 5128  0..qX....0..a`Q(
-00001720: 090b 949b 1a1a db41 3454 c292 7e53 aad6  .......A4T..~S..
-00001730: 0cb4 5abe 0757 0bfd b069 cf24 d62d 2132  ..Z..W...i.$.-!2
-00001740: 5529 bbf7 50ce 6a39 bd5b 37a8 4556 51dc  U)..P.j9.[7.EVQ.
-00001750: 8ff1 48c8 81ed 1727 f85a 498d 060b 1b10  ..H....'.ZI.....
-00001760: 2eec 849e c63c 0927 2191 e6b3 5c51 042e  .....<.'!...\Q..
-00001770: ed4c 4391 f29b 78fa 29e6 e17c e6f3 f35b  .LC...x.)..|...[
-00001780: c1ce 3c9b 3353 e2ee b356 f957 d500 259b  ..<.3S...V.W..%.
-00001790: ca64 45b6 820a a485 9c0a c7d9 1362 bd92  .dE..........b..
-000017a0: c289 8de3 8b67 eb6f ae04 55ff d795 2d43  .....g.o..U...-C
-000017b0: 7c70 0eee e860 444a 8cc7 3825 425a b585  |p...`DJ..8%BZ..
-000017c0: 5ba8 c87c 1913 d4fc f5e2 dc9c a485 076d  [..|...........m
-000017d0: cfe7 83ce a52f f577 cd32 61e0 16ab 3f2a  ...../.w.2a...?*
-000017e0: b725 b925 ad39 1462 53d9 e3cf 4910 8fa2  .%.%.9.bS...I...
-000017f0: 7142 32fb ad1f b8fb 026a 5d5a 3a90 0497  qB2......j]Z:...
-00001800: b4e1 933c cdf7 0b30 924a 4d52 83c4 8990  ...<...0.JMR....
-00001810: 5891 47fa b25a b996 a54a 8947 3fee 7a87  X.G..Z...J.G?.z.
-00001820: e303 dcd8 bdcf 0767 7263 2cd6 83a4 9ed3  .......grc,.....
-00001830: 1192 9e70 ced9 4088 8251 7271 7915 3b81  ...p..@..Qrqy.;.
-00001840: 3d83 76df 608c 7a06 8d03 830e f447 c9c1  =.v.`.z......G..
-00001850: 1b47 c985 0f80 c6e1 e8c5 2b01 6460 ec52  .G........+.d`.R
-00001860: b9f4 bc49 1b0f 428e d11c 73fd ae74 8c86  ...I..B...s..t..
-00001870: 58e2 f1f9 d531 9e57 28ae 23ba 6af8 be58  X....1.W(.#.j..X
-00001880: 082b e633 8d3b 4637 d9f5 4e2b dcbb 904c  .+.3.;F7..N+...L
-00001890: ff57 4caa a233 bd71 b664 472d 9d72 43fd  .WL..3.q.dG-.rC.
-000018a0: b89d 47b3 70eb e0bd c5ed a945 fcd2 6271  ..G.p......E..bq
-000018b0: 6a91 bcb4 a0cb e5bc d0f7 e0e5 fc60 1192  j............`..
-000018c0: eaa1 a5bb 305a b186 7ba1 d7aa 31ac 82c2  ....0Z..{...1...
-000018d0: b7df 2567 ba6b d128 a0b9 c5d6 35a5 ebd5  ..%g.k.(....5...
-000018e0: 0c2d 75d7 b02a e995 030a 2c0a a808 05a2  .-u..*....,.....
-000018f0: 1d16 9430 c75d 81dd b4ac 152d e895 7aa2  ...0.].....-..z.
-00001900: fb3a e10c b5a2 26f7 cf58 ca5b d456 0b65  .:....&..X.[.V.e
-00001910: fd9d 3b3c b4f3 7f00 0000 ffff 0300 504b  ..;<..........PK
-00001920: 0304 1400 0600 0800 0000 2100 d734 7830  ..........!..4x0
-00001930: bb01 0000 7d04 0000 1800 2800 6375 7374  ....}.....(.cust
-00001940: 6f6d 586d 6c2f 6974 656d 5072 6f70 7332  omXml/itemProps2
-00001950: 2e78 6d6c 20a2 2400 28a0 2000 0000 0000  .xml .$.(. .....
-00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001970: 0000 0000 0000 0000 0000 0000 b494 dd6a  ...............j
-00001980: dc30 1085 ef0b 7d07 a37b 59f2 bf37 c41b  .0....}..{Y..7..
-00001990: d636 8540 0325 4d21 b763 59da 35b5 2423  .6.@.%M!.cY.5.$#
-000019a0: c9dd 96d2 77af eca4 9434 1bb6 a5ed 953d  ....w....4.....=
-000019b0: 3673 cecc f127 5f5e 7d96 63f0 891b 3b68  6s...'_^}.c...;h
-000019c0: 55a1 28a4 28e0 8ae9 7e50 fb0a 7db8 7b83  U.(.(...~P..}.{.
-000019d0: 4b14 5807 aa87 512b 5e21 a5d1 d5f6 f5ab  K.X...Q+^!......
-000019e0: cbde 5ef4 e0c0 3a6d f8b5 e332 f00f 067f  ..^...:m...2....
-000019f0: bd6e 2bf4 b56e cb26 a937 25ce e33a c369  .n+..n.&.7%..:.i
-00001a00: d136 78d7 b431 6ecb 84b6 75da eca2 bcfe  .6x..1n...u.....
-00001a10: 8602 6fad bc8c add0 c1b9 e982 10cb 0e5c  ..o............\
-00001a20: 820d f5c4 957f 29b4 91e0 7c69 f644 0b31  ......)...|i.D.1
-00001a30: 30de 6a36 4bae 1c89 29cd 099b bdbd bc97  0.j6K...).......
-00001a40: 23da 2ef3 3c74 df72 619f 96cb 68b3 199e  #...<t.ra...h...
-00001a50: b9c8 8119 6db5 7021 d3f2 d1e0 4158 7207  ....m.p!....AXr.
-00001a60: cb76 8469 e5bc dddd 9789 23f2 cf54 27e3  .v.i......#..T'.
-00001a70: 1734 6ee0 962c 4e3b e7cc d0cd 8edb 731e  .4n..,N;......s.
-00001a80: c7e3 313c 266b 1e3e 8088 dcdf bc7d bf46  ..1<&k.>.....}.F
-00001a90: f65f 867b 51b4 2b68 0eb9 4830 2d44 87d3  ._.{Q.+h..H0-D..
-00001aa0: 2e29 7199 d10c 4351 6439 2ba3 4d97 c28b  .)q...CQd9+.M...
-00001ab0: cd34 2a23 e8b3 0267 9b2c c629 f577 2040  .4*#...g.,.).w @
-00001ac0: e082 26d0 c734 d900 2bff 7e9d fe11 941b  ..&..4..+.~.....
-00001ad0: 50b0 e72b 32ce 7fc4 b309 ff20 f024 1b83  P..+2...... .$..
-00001ae0: 127a 0277 5820 29c8 3b30 4e71 d378 448c  .z.wX ).;0Nq.xD.
-00001af0: 1e7f 5bf9 04db 13b0 8f7e ca67 ec19 8e7f  ..[......~.g....
-00001b00: a272 2e93 6936 e34a 46cf 081f d795 2d89  .r..i6.JF.....-.
-00001b10: c288 fc49 a3e3 46da b31d a743 1afc 5131  ...I..F....C..Q1
-00001b20: 0a46 a2bb 7ef1 24bf 1cc9 a57e f2cb d87e  .F..~.$....~...~
-00001b30: 0700 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00001b40: 0000 0021 005c 9627 22c3 0000 0028 0100  ...!.\.'"....(..
-00001b50: 001e 0008 0163 7573 746f 6d58 6d6c 2f5f  .....customXml/_
-00001b60: 7265 6c73 2f69 7465 6d32 2e78 6d6c 2e72  rels/item2.xml.r
-00001b70: 656c 7320 a204 0128 a000 0100 0000 0000  els ...(........
-00001b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001680: 312e 786d 6c8c 55c9 6edb 3010 bd17 e83f  1.xml.U.n.0....?
+00001690: 10bc 479b 97c4 86e5 20b5 9334 405b 1475  ..G..... ..4@[.u
+000016a0: 9733 458d 2c22 92a8 92b4 1de7 eb3b a424  .3E.,".......;.$
+000016b0: cb81 1bc3 1769 28ce bc79 b36a 76fb 5216  .....i(..y.jv.R.
+000016c0: 640b 4a0b 59c5 34f4 024a a0e2 3215 d53a  d.J.Y.4..J..2..:
+000016d0: a6bf 7e3e 5cdd 50a2 0dab 5256 c80a 62ba  ..~>\.P...RV..b.
+000016e0: 074d 6fe7 1f3f cc76 523d eb1c c010 44a8  .Mo..?.vR=....D.
+000016f0: 744c 7363 eaa9 ef6b 9e43 c9b4 276b a8f0  tLsc...k.C..'k..
+00001700: 2693 aa64 068f 6aed eb5a 014b 9d51 59f8  &..d..j..Z.K.QY.
+00001710: 5110 8cfd 9289 8a36 0853 7509 86cc 32c1  Q......6.Su...2.
+00001720: 6129 f9a6 84ca 3420 0a0a 6690 bfce 45ad  a)....4 ..f...E.
+00001730: 3bb4 925f 0257 32f5 bca9 afb8 2c6b 8448  ;.._.W2.....,k.H
+00001740: 4421 ccde 8152 52f2 e9d3 ba92 8a25 05c6  D!...RR......%..
+00001750: fd12 0e19 efb0 dde1 04be 145c 492d 33e3  ...........\I-3.
+00001760: 219c df10 3d8d 79e2 4f7c 449a cf52 8111  !...=.y.O|D..R..
+00001770: d8b4 1305 594c efc2 e9fd 80fa f399 cbcf  ....YL..........
+00001780: 6f01 3b7d 2413 9dcb dda3 12e9 1751 0126  o.;}$........Q.&
+00001790: 1bcb 6458 b282 02b8 8114 0b47 c9ab 94e5  ..dX.......G....
+000017a0: 8a33 4b36 0c47 47e7 6fb6 0445 fbd5 962d  .3K6.GG.o..E...-
+000017b0: 91f2 d93a 7842 c300 9968 0763 9930 6ec4  ...:xB...h.c.0n.
+000017c0: 1616 50a0 fae3 3556 feaf e386 2212 f30f  ..P...5V...."...
+000017d0: cc8e e58e e583 2bf4 7745 12a6 6121 8b3f  ......+.wE..a!.?
+000017e0: 2235 393a 45a6 2964 6c53 98fe e3c4 0b87  "59:E.)dlS......
+000017f0: c138 4292 edd5 0fb9 fb0c 629d 1b34 88bc  .8B.......b..4..
+00001800: 6bbc 7029 9ea6 fb25 688e 8546 a25e 6449  k.p)...%h..F.^dI
+00001810: 7059 a047 7c92 52d8 86c5 3ab1 17f7 deb5  pY.G|.R...:.....
+00001820: 0ec7 0770 6df6 2e1b 94f0 8d36 b2ec 28b5  ...pm......6..(.
+00001830: 380d 42d4 220c 28e9 1002 6f18 8dae 6f42  8.B.".(...o...oB
+00001840: 4bb0 c5c0 db33 18c3 1603 df1d 061a b4a6  K....3..........
+00001850: e8e0 8c29 ba70 01e0 bb33 1dfd 2780 04b4  ...).p...3..'...
+00001860: 7910 363d 67d1 c61d 919e 499f eb8b d231  y.6=g.....I....1
+00001870: ec08 85e3 c1cd 5914 db11 4d35 5c5f 2c99  ......Y...M5\_,.
+00001880: 61f3 9992 3b82 738c 2c75 cdec 5608 a7ef  a...;.s.,u..V...
+00001890: 1513 ab68 553f 59dd 9862 9630 3a8d ddb8  ...hU?Y..b.0:...
+000018a0: 9d07 337f 6bc1 5b8d c5a9 46f8 5663 79aa  ..3.k.[...F.Vcy.
+000018b0: 11bd d5b8 6f34 f079 f032 3868 f8c8 fa40  ....o4.y.28h...@
+000018c0: 1d89 1c53 772d f94e 0823 64eb 62b8 6b5a  ...Sw-.N.#d.b.kZ
+000018d0: d385 d38b 8b5e 5cf6 e2bd 13df b8b4 bd72  .....^\........r
+000018e0: 94ad cb5c ba5d d164 b017 17bd b8ec c566  ...\.].d.......f
+000018f0: af34 2e9b 216e 8a55 b335 7c65 6a2d 2a4d  .4..!n.U.5|ej-*M
+00001900: 0ac8 dc90 e1d0 ab66 1003 0f65 236b 3b7a  .......f...e#k;z
+00001910: 7622 1369 7086 ba53 8e9b 1cb0 7c81 87ec  v".ip..S....|...
+00001920: 3329 4d77 c0b6 b0b8 2b30 9b9a d4ac 06b5  3)Mw....+0......
+00001930: 12af b893 2694 4825 7094 ddaa 8e69 2d95  ....&.H%p....i-.
+00001940: 514c 18b7 590e 3f93 f93f 0000 00ff ff03  QL..Y.?..?......
+00001950: 0050 4b03 0414 0006 0008 0000 0021 0039  .PK..........!.9
+00001960: 34ab 99bd 0100 007d 0400 0018 0028 0063  4......}.....(.c
+00001970: 7573 746f 6d58 6d6c 2f69 7465 6d50 726f  ustomXml/itemPro
+00001980: 7073 322e 786d 6c20 a224 0028 a020 0000  ps2.xml .$.(. ..
+00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019a0: 0000 0000 0000 0000 0000 0000 0000 00b4  ................
+000019b0: 945f 6bdb 3014 c5df 07fb 0e46 efb2 e47f  ._k.0......F....
+000019c0: b15d ea94 26a9 a1b0 c2d8 3ae8 ebb5 2c25  .]..&.....:...,%
+000019d0: 6296 6424 65d9 18fb ee93 dd8e d135 251b  b.d$e........5%.
+000019e0: 6b9f ec6b 73cf b9f7 f827 9f5f 7c55 43f4  k..ks....'._|UC.
+000019f0: 855b 278d 6e50 1253 1471 cd4c 2ff5 b641  .['.nP.S.q.L/..A
+00001a00: 9f6e 5b5c a1c8 79d0 3d0c 46f3 0669 832e  .n[\..y.=.F..i..
+00001a10: 966f df9c f7ee ac07 0fce 1bcb af3d 5751  .o...........=WQ
+00001a20: 7820 c3f5 7ad3 a0ef f48a b6eb 3cdd e075  x ..z.......<..u
+00001a30: 59b7 38af 5729 becc d72b 7c95 b4ab b65a  Y.8.W)...+|....Z
+00001a40: e56d 92a6 3f50 14ac 7590 710d da79 3f9e  .m..?P..u.q..y?.
+00001a50: 11e2 d88e 2b70 b119 b90e 2f85 b10a 7c28  ....+p..../...|(
+00001a60: ed96 1821 24e3 1bc3 f68a 6b4f 524a 1784  ...!$.....kORJ..
+00001a70: ed83 bdba 5303 5a4e f3dc 777f e0c2 3d2e  ....S.ZN..w...=.
+00001a80: a7d1 f656 3e71 5192 59e3 8cf0 3133 eac1  ...V>qQ.Y...13..
+00001a90: e05e 5871 0fd3 7684 19ed 83dd edb7 9123  .^Xq..v........#
+00001aa0: f262 aaa3 0d0b 5a2f b923 93d3 a5f7 5676  .b....Z/.#....Vv
+00001ab0: 7bcf dd29 8fc3 e110 1fb2 398f 1040 42ee  {..)......9..@B.
+00001ac0: 6ede 7d9c 237b 95e1 9e15 ed4a ba80 85c8  n.}.#{.....J....
+00001ad0: 302d 4587 f32e ab70 55d0 0243 5916 0b56  0-E....pU..CY..V
+00001ae0: 2575 97c3 b3cd 34a9 12e8 8b12 1775 91e2  %u....4......u..
+00001af0: 9c86 3b10 2070 4933 e853 9ad5 c0aa ff5f  ..;. pI3.S....._
+00001b00: a77f 00e5 0634 6cf9 8c8c 0f1f f164 c2bf  .....4l......d..
+00001b10: 083c ca86 d4c2 8ce0 7713 2425 790f d66b  .<......w.$%y..k
+00001b20: 6ed7 0111 6b86 bf56 3ec2 f608 ec73 98f2  n...k..V>....s..
+00001b30: 097b 96e3 dfa8 9cca 64dc db61 26a3 6784  .{......d..a&.g.
+00001b40: 0ff3 ca8e 2471 42fe a5d1 73ab dcc9 8ee3  ....$qB...s.....
+00001b50: 21c9 7054 ac86 8198 ae9f 3cc9 1f47 72aa  !.pT......<..Gr.
+00001b60: 1ffd 3296 3f01 0000 ffff 0300 504b 0304  ..2.?.......PK..
+00001b70: 1400 0600 0800 0000 2100 5c96 2722 c300  ........!.\.'"..
+00001b80: 0000 2801 0000 1e00 0801 6375 7374 6f6d  ..(.......custom
+00001b90: 586d 6c2f 5f72 656c 732f 6974 656d 322e  Xml/_rels/item2.
+00001ba0: 786d 6c2e 7265 6c73 20a2 0401 28a0 0001  xml.rels ...(...
 00001bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c70: 0000 0000 0000 0000 0000 0084 cfc1 6ac3  ..............j.
-00001c80: 300c 06e0 7ba1 ef60 745f 9cf6 304a 89d3  0...{..`t_..0J..
-00001c90: 4b19 e436 460b bd1a 4749 4c63 cb58 4a69  K..6F...GILc.XJi
-00001ca0: df7e a6a7 1606 3b4a 42df 2f35 877b 98d5  .~....;JB./5.{..
-00001cb0: 0d33 7b8a 0636 550d 0aa3 a3de c7d1 c0f9  .3{..6U.........
-00001cc0: f4f5 b103 c562 636f 678a 68e0 810c 8776  .....bcog.h....v
-00001cd0: bd6a 7e70 b652 9678 f289 5551 221b 9844  .j~p.R.x..UQ"..D
-00001ce0: d25e 6b76 1306 cb15 258c 6532 500e 564a  .^kv....%.e2P.VJ
-00001cf0: 9947 9dac bbda 11f5 b6ae 3f75 7e35 a07d  .G........?u~5.}
-00001d00: 3355 d71b c85d bf01 757a a492 fcbf 4dc3  3U...]..uz....M.
-00001d10: e01d 1ec9 2d01 a3fc 11a1 ddc2 42e1 12e6  ....-.......B...
-00001d20: ef4c 898b 6cf3 8862 c00b 8667 6b5b 957b  .L..l..b...gk[.{
-00001d30: 41b7 8d7e fbaf fd05 0000 ffff 0300 504b  A..~..........PK
-00001d40: 0304 1400 0600 0800 0000 2100 743f 397a  ..........!.t?9z
-00001d50: c200 0000 2801 0000 1e00 0801 6375 7374  ....(.......cust
-00001d60: 6f6d 586d 6c2f 5f72 656c 732f 6974 656d  omXml/_rels/item
-00001d70: 312e 786d 6c2e 7265 6c73 20a2 0401 28a0  1.xml.rels ...(.
-00001d80: 0001 0000 0000 0000 0000 0000 0000 0000  ................
-00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cb0: 84cf c16a c330 0c06 e07b a1ef 6074 5f9c  ...j.0...{..`t_.
+00001cc0: f630 4a89 d34b 19e4 3646 0bbd 1a47 494c  .0J..K..6F...GIL
+00001cd0: 63cb 584a 69df 7ea6 a716 063b 4a42 df2f  c.XJi.~....;JB./
+00001ce0: 3587 7b98 d50d 337b 8a06 3655 0d0a a3a3  5.{...3{..6U....
+00001cf0: dec7 d1c0 f9f4 f5b1 03c5 6263 6f67 8a68  ..........bcog.h
+00001d00: e081 0c87 76bd 6a7e 70b6 5296 78f2 8955  ....v.j~p.R.x..U
+00001d10: 5122 1b98 44d2 5e6b 7613 06cb 1525 8c65  Q"..D.^kv....%.e
+00001d20: 3250 0e56 4a99 479d acbb da11 f5b6 ae3f  2P.VJ.G........?
+00001d30: 757e 35a0 7d33 55d7 1bc8 5dbf 0175 7aa4  u~5.}3U...]..uz.
+00001d40: 92fc bf4d c3e0 1d1e c92d 01a3 fc11 a1dd  ...M.....-......
+00001d50: c242 e112 e6ef 4c89 8b6c f388 62c0 0b86  .B....L..l..b...
+00001d60: 676b 5b95 7b41 b78d 7efb affd 0500 00ff  gk[.{A..~.......
+00001d70: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00001d80: 0074 3f39 7ac2 0000 0028 0100 001e 0008  .t?9z....(......
+00001d90: 0163 7573 746f 6d58 6d6c 2f5f 7265 6c73  .customXml/_rels
+00001da0: 2f69 7465 6d31 2e78 6d6c 2e72 656c 7320  /item1.xml.rels 
+00001db0: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
 00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e80: 0000 84cf c18a 0231 0c06 e0bb e03b 94dc  .......1.....;..
-00001e90: 9dce 7810 91e9 7859 16bc 89b8 e0b5 7432  ..x...xY......t2
-00001ea0: 33c5 6953 9a28 faf6 164f 2b2c ec31 09f9  3.iS.(...O+,.1..
-00001eb0: fea4 dd3f c2ac ee98 d953 34d0 5435 288c  ...?.....S4.T5(.
-00001ec0: 8e7a 1f47 033f e7ef d516 148b 8dbd 9d29  .z.G.?.........)
-00001ed0: a281 2732 ecbb e5a2 3de1 6ca5 2cf1 e413  ..'2....=.l.,...
-00001ee0: aba2 4436 3089 a49d d6ec 260c 962b 4a18  ..D60.....&..+J.
-00001ef0: cb64 a01c ac94 328f 3a59 77b5 23ea 755d  .d....2.:Yw.#.u]
-00001f00: 6f74 fe6d 40f7 61aa 436f 201f fa06 d4f9  ot.m@.a.Co .....
-00001f10: 994a f2ff 360d 8377 f845 ee16 30ca 1f11  .J..6..w.E..0...
-00001f20: dadd 5828 5cc2 7ccc 94b8 c836 8f28 06bc  ..X(\.|....6.(..
-00001f30: 6078 b79a aadc 0bba 6bf5 c77f dd0b 0000  `x......k.......
-00001f40: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00001f50: 2100 bd84 6223 9000 0000 db00 0000 1300  !...b#..........
-00001f60: 2800 6375 7374 6f6d 586d 6c2f 6974 656d  (.customXml/item
-00001f70: 312e 786d 6c20 a224 0028 a020 0000 0000  1.xml .$.(. ....
-00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f90: 0000 0000 0000 0000 0000 0000 006c 8e3b  .............l.;
-00001fa0: 0ec2 3010 05af 82d2 932d e8d0 e234 810a  ..0......-...4..
-00001fb0: 51e5 02c6 388a a5ac d7f2 2e1f df1e 0741  Q...8..........A
-00001fc0: 8194 7a9e 661e 7624 bc75 1cd5 471d 4af2  ..z.f.v$.u..G.J.
-00001fd0: 9dc1 1367 1a3c a5d9 aa97 cd8b e628 8766  ...g.<.......(.f
-00001fe0: 524d 7b00 7193 272b 2d05 9759 78d4 d631  RM{.q.'+-..Yx..1
-00001ff0: 814c 36fb c421 2a3c 76f0 b569 b5c1 585d  .L6..!*<v..i..X]
-00002000: d218 ec83 545f 313d bb3b d5d4 395c b3cd  ....T_1=.;..9\..
-00002010: 6549 21fc 201e 6f41 d727 1f82 17ff 5cc7  eI!. .oA.'....\.
-00002020: 0b40 f83b 6ede 0000 00ff ff03 0050 4b03  .@.;n........PK.
-00002030: 0414 0006 0008 0000 0021 00b0 c375 79f4  .........!...uy.
-00002040: 0000 004f 0100 0018 0028 0063 7573 746f  ...O.....(.custo
-00002050: 6d58 6d6c 2f69 7465 6d50 726f 7073 312e  mXml/itemProps1.
-00002060: 786d 6c20 a224 0028 a020 0000 0000 0000  xml .$.(. ......
-00002070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002080: 0000 0000 0000 0000 0000 0064 9041 6b83  ...........d.Ak.
-00002090: 4010 85ef 85fe 07d9 bbae 9a26 3541 0d46  @..........&5A.F
-000020a0: 2de4 5a1a e875 5967 e382 bb23 3b6b 6829  -.Z..uYg...#;kh)
-000020b0: fdef 5de9 29ed 6978 f398 f73d a63c 7e98  ..].).ix...=.<~.
-000020c0: 29ba 8123 8db6 6259 92b2 08ac c441 db6b  )..#..bY.....A.k
-000020d0: c52e 6f2f 71c1 22f2 c20e 6242 0b15 b3c8  ..o/q."...bB....
-000020e0: 8ef5 e343 39d0 6110 5e90 4707 670f 260a  ...C9.a.^.G.g.&.
-000020f0: 0b1d e6b9 abd8 575f 14cd f369 d7c4 79b6  ......W_...i..y.
-00002100: efe2 a76d 91c7 a7cd 3e8b f3a6 c9fb acdd  ...m....>.......
-00002110: f67d db7e b328 a06d 88a1 8a8d decf 07ce  .}.~.(.m........
-00002120: 498e 6004 2538 830d a642 6784 0fd2 5d39  I.`.%8...Bg...]9
-00002130: 2aa5 2574 2817 03d6 f33c 4d77 5c2e 016f  *.%t(....<Mw\..o
-00002140: decd c4ea b5cf eff5 2b28 ba97 6bb5 c5e9  ........+(..k...
-00002150: 7f14 a3a5 4342 e513 8986 d328 1ccc a843  ....CB.....(...C
-00002160: f86d c325 5a1f 38fe 7306 bed6 20c6 eb92  .m.%Z.8.s... ...
-00002170: ff81 acfa ee09 f50f 0000 00ff ff03 0050  ...............P
-00002180: 4b03 0414 0006 0008 0000 0021 00a0 5a86  K..........!..Z.
-00002190: 4d8a 0100 0007 0300 0010 0008 0164 6f63  M............doc
-000021a0: 5072 6f70 732f 6170 702e 786d 6c20 a204  Props/app.xml ..
-000021b0: 0128 a000 0100 0000 0000 0000 0000 0000  .(..............
-000021c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001eb0: 0000 0000 0000 0084 cfc1 8a02 310c 06e0  ............1...
+00001ec0: bbe0 3b94 dc9d ce78 1091 e978 5916 bc89  ..;....x...xY...
+00001ed0: b8e0 b574 3233 c569 539a 28fa f616 4f2b  ...t23.iS.(...O+
+00001ee0: 2cec 3109 f9fe a4dd 3fc2 acee 98d9 5334  ,.1.....?.....S4
+00001ef0: d054 3528 8c8e 7a1f 4703 3fe7 efd5 1614  .T5(..z.G.?.....
+00001f00: 8b8d bd9d 29a2 8127 32ec bbe5 a23d e16c  ....)..'2....=.l
+00001f10: a52c f1e4 13ab a244 3630 89a4 9dd6 ec26  .,.....D60.....&
+00001f20: 0c96 2b4a 18cb 64a0 1cac 9432 8f3a 5977  ..+J..d....2.:Yw
+00001f30: b523 ea75 5d6f 74fe 6d40 f761 aa43 6f20  .#.u]ot.m@.a.Co 
+00001f40: 1ffa 06d4 f999 4af2 ff36 0d83 77f8 45ee  ......J..6..w.E.
+00001f50: 1630 ca1f 11da dd58 285c c27c cc94 b8c8  .0.....X(\.|....
+00001f60: 368f 2806 bc60 78b7 9aaa dc0b ba6b f5c7  6.(..`x......k..
+00001f70: 7fdd 0b00 00ff ff03 0050 4b03 0414 0006  .........PK.....
+00001f80: 0008 0000 0021 00bd 8462 2390 0000 00db  .....!...b#.....
+00001f90: 0000 0013 0028 0063 7573 746f 6d58 6d6c  .....(.customXml
+00001fa0: 2f69 7465 6d31 2e78 6d6c 20a2 2400 28a0  /item1.xml .$.(.
+00001fb0: 2000 0000 0000 0000 0000 0000 0000 0000   ...............
+00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fd0: 0000 6c8e 3b0e c230 1005 af82 d293 2de8  ..l.;..0......-.
+00001fe0: d0e2 3481 0a51 e502 c638 8aa5 acd7 f22e  ..4..Q...8......
+00001ff0: 1fdf 1e07 4181 947a 9e66 1e76 24bc 751c  ....A..z.f.v$.u.
+00002000: d547 1d4a f29d c113 671a 3ca5 d9aa 97cd  .G.J....g.<.....
+00002010: 8be6 2887 6652 4d7b 0071 9327 2b2d 0597  ..(.fRM{.q.'+-..
+00002020: 5978 d4d6 3181 4c36 fbc4 212a 3c76 f0b5  Yx..1.L6..!*<v..
+00002030: 69b5 c158 5dd2 18ec 8354 5f31 3dbb 3bd5  i..X]....T_1=.;.
+00002040: d439 5cb3 cd65 4921 fc20 1e6f 41d7 271f  .9\..eI!. .oA.'.
+00002050: 8217 ff5c c70b 40f8 3b6e de00 0000 ffff  ...\..@.;n......
+00002060: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00002070: 5a69 9b33 f400 0000 4f01 0000 1800 2800  Zi.3....O.....(.
+00002080: 6375 7374 6f6d 586d 6c2f 6974 656d 5072  customXml/itemPr
+00002090: 6f70 7331 2e78 6d6c 20a2 2400 28a0 2000  ops1.xml .$.(. .
+000020a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020c0: 6490 416b 8340 1085 ef85 fe07 99bb 5913  d.Ak.@........Y.
+000020d0: d344 831a 6a34 906b 69a1 d765 1de3 82bb  .D..j4.ki..e....
+000020e0: 23bb 6368 29fd ef5d e929 ed69 78f3 98f7  #.ch)..].).ix...
+000020f0: 3da6 387e 9831 baa1 f39a 6c09 eb55 0211  =.8~.1....l..U..
+00002100: 5a45 9db6 d712 de5e cf71 0691 6769 3b39  ZE.....^.q..gi;9
+00002110: 92c5 122c c1b1 7a7c 283a 7fe8 244b cfe4  ...,..z|(:..$K..
+00002120: f0c2 68a2 b0d0 615e 9a12 bed6 cd73 7dce  ..h...a^.....s}.
+00002130: db5d 5cb7 cd26 dee6 a753 9c65 4f6d dca6  .]\..&...S.eOm..
+00002140: dbbc cef6 499b a7fb 6f88 02da 8618 5fc2  ....I...o....._.
+00002150: c03c 1d84 f06a 4023 fd8a 26b4 c1ec c919  .<...j@#..&.....
+00002160: c941 baab a0be d70a 1b52 b341 cb62 9324  .A.......R.A.b.$
+00002170: 3ba1 e680 37ef 6684 6ae9 f37b fd82 bdbf  ;...7.f.j..{....
+00002180: 974b b5d9 e97f 14a3 9523 4f3d af14 19e1  .K.......#O=....
+00002190: 07e9 7022 1dc2 6fa9 5064 3970 f873 42b1  ..p"..o.Pd9p.sB.
+000021a0: d4f0 20aa 42fc 812c faee 09d5 0f00 0000  .. .B..,........
+000021b0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+000021c0: 2100 a05a 864d 8a01 0000 0703 0000 1000  !..Z.M..........
+000021d0: 0801 646f 6350 726f 7073 2f61 7070 2e78  ..docProps/app.x
+000021e0: 6d6c 20a2 0401 28a0 0001 0000 0000 0000  ml ...(.........
 000021f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000022a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022b0: 0000 0000 009c 92c1 6e13 3110 86ef 48bc  ........n.1...H.
-000022c0: 83e5 7be3 4d41 158a bcae 500b ca01 44a4  ..{.MA....P...D.
-000022d0: a4bd 1b7b 3631 38f6 ca33 5925 bc0d cfc2  ...{618..3Y%....
-000022e0: 8b31 bbab a69b 9613 b799 f967 fffd fcdb  .1.........g....
-000022f0: faf6 b88f a283 8221 a75a ce67 9514 905c  .......!.Z.g...\
-00002300: f621 6d6b f9b0 f97c f541 0a24 9bbc 8d39  .!mk...|.A.$...9
-00002310: 412d 4f80 f2d6 bc7d a357 25b7 5028 000a  A-O....}.W%.P(..
-00002320: b648 58cb 1d51 bb50 0add 0ef6 1667 2c27  .HX..Q.P.....g,'
-00002330: 569a 5cf6 96b8 2d5b 959b 2638 b8cf eeb0  V.\...-[..&8....
-00002340: 8744 eaba aa6e 141c 0992 077f d59e 0de5  .D...n..........
-00002350: e8b8 e8e8 7f4d 7d76 3d1f 3e6e 4e2d 031b  .....M}v=.>nN-..
-00002360: fdb1 6d63 7096 f894 e66b 7025 636e 487c  ..mcp....kp%cnH|
-00002370: 3a3a 885a 4d45 cd74 6b70 8712 e864 2aad  ::.ZME.tkp...d*.
-00002380: a6ad 5e3b 1be1 8e8d 4d63 2382 56cf 03bd  ..^;....Mc#.V...
-00002390: 04db 87b6 b2a1 a0d1 1d2d 3a70 948b c0f0  .........-:p....
-000023a0: 8b63 bb96 e2bb 45e8 716a d9d9 126c 22c6  .c....E.qj...l".
-000023b0: ead7 c666 a863 8b54 cc32 ffb0 283c 08f7  ...f.c.T.2..(<..
-000023c0: e777 7487 98b5 e2bd 511b cae9 27d3 3abc  .wt.....Q...'.:.
-000023d0: 37f3 6181 8bcb c5de 60e4 61e1 9274 1328  7.a.....`.a..t.(
-000023e0: 027e 6b56 b6d0 3fc0 e753 f081 61c4 1e71  .~kV..?..S..a..q
-000023f0: c697 51fc 2bc2 e1ec fcaf 17ee 5f42 fa89  ..Q.+......._B..
-00002400: 0fed 26df 5b82 a710 2f87 7abd b305 3ce7  ..&.[.../.z...<.
-00002410: 7e0e f93c d04b ceaf c4de e46e 67d3 16fc  ~..<.K.....ng...
-00002420: d3ce 6ba1 bff2 c7f1 5d9b f9cd ac7a 57f1  ..k.....]....zW.
-00002430: 6d4e 665a 3dbf 60f3 1700 00ff ff03 0050  mNfZ=.`........P
-00002440: 4b03 0414 0006 0008 0000 0021 0097 1e91  K..........!....
-00002450: 564b 0100 0069 0200 0011 0008 0164 6f63  VK...i.......doc
-00002460: 5072 6f70 732f 636f 7265 2e78 6d6c 20a2  Props/core.xml .
-00002470: 0401 28a0 0001 0000 0000 0000 0000 0000  ..(.............
-00002480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022e0: 0000 0000 0000 0000 0000 9c92 c16e 1331  .............n.1
+000022f0: 1086 ef48 bc83 e57b e34d 4115 8abc ae50  ...H...{.MA....P
+00002300: 0bca 0144 a4a4 bd1b 7b36 3138 f6ca 3359  ...D....{618..3Y
+00002310: 25bc 0dcf c28b 31bb aba6 9b96 13b7 99f9  %.....1.........
+00002320: 67ff fdfc dbfa f6b8 8fa2 8382 21a7 5ace  g...........!.Z.
+00002330: 6795 1490 5cf6 216d 6bf9 b0f9 7cf5 410a  g...\.!mk...|.A.
+00002340: 249b bc8d 3941 2d4f 80f2 d6bc 7da3 5725  $...9A-O....}.W%
+00002350: b750 2800 0ab6 4858 cb1d 51bb 500a dd0e  .P(...HX..Q.P...
+00002360: f616 672c 2756 9a5c f696 b82d 5b95 9b26  ..g,'V.\...-[..&
+00002370: 38b8 cfee b087 44ea baaa 6e14 1c09 9207  8.....D...n.....
+00002380: 7fd5 9e0d e5e8 b8e8 e87f 4d7d 763d 1f3e  ..........M}v=.>
+00002390: 6e4e 2d03 1bfd b16d 6370 96f8 94e6 6b70  nN-....mcp....kp
+000023a0: 2563 6e48 7c3a 3a88 5a4d 45cd 746b 7087  %cnH|::.ZME.tkp.
+000023b0: 12e8 642a ada6 ad5e 3b1b e18e 8d4d 6323  ..d*...^;....Mc#
+000023c0: 8256 cf03 bd04 db87 b6b2 a1a0 d11d 2d3a  .V............-:
+000023d0: 7094 8bc0 f08b 63bb 96e2 bb45 e871 6ad9  p.....c....E.qj.
+000023e0: d912 6c22 c6ea d7c6 66a8 638b 54cc 32ff  ..l"....f.c.T.2.
+000023f0: b028 3c08 f7e7 7774 8798 b5e2 bd51 1bca  .(<...wt.....Q..
+00002400: e927 d33a bc37 f361 818b cbc5 de60 e461  .'.:.7.a.....`.a
+00002410: e192 7413 2802 7e6b 56b6 d03f c0e7 53f0  ..t.(.~kV..?..S.
+00002420: 8161 c41e 71c6 9751 fc2b c2e1 ecfc af17  .a..q..Q.+......
+00002430: ee5f 42fa 890f ed26 df5b 82a7 102f 877a  ._B....&.[.../.z
+00002440: bdb3 053c e77e 0ef9 3cd0 4bce afc4 dee4  ...<.~..<.K.....
+00002450: 6e67 d316 fcd3 ce6b a1bf f2c7 f15d 9bf9  ng.....k.....]..
+00002460: cdac 7a57 f16d 4e66 5a3d bf60 f317 0000  ..zW.mNfZ=.`....
+00002470: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+00002480: 2100 e04f 8b29 4a01 0000 6902 0000 1100  !..O.)J...i.....
+00002490: 0801 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
+000024a0: 786d 6c20 a204 0128 a000 0100 0000 0000  xml ...(........
 000024b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002570: 0000 0000 0000 8492 5d4b c330 1885 ef05  ........]K.0....
-00002580: ff43 c97d 9b7e 6c73 0b6d 0753 76e5 40b0  .C.}.~ls.m.Sv.@.
-00002590: a278 1792 775b b149 4a92 d9ed df9b b65b  .x..w[.IJ......[
-000025a0: ad4e 1072 939c 9327 e7bc 245d 1e45 e57d  .N.r...'..$].E.}
-000025b0: 8236 a592 198a 8210 7920 99e2 a5dc 65e8  .6......y ....e.
-000025c0: a558 fb73 e419 4b25 a795 9290 a113 18b4  .X.s..K%........
-000025d0: cc6f 6f52 5613 a634 3c69 5583 b625 18cf  .ooRV..4<iU..%..
-000025e0: 91a4 21ac ced0 deda 9a60 6cd8 1e04 3581  ..!......`l...5.
-000025f0: 7348 276e 9516 d4ba adde e19a b20f ba03  sH'n............
-00002600: 1c87 e10c 0bb0 9453 4b71 0bf4 eb81 88ce  .......SKq......
-00002610: 48ce 0664 7dd0 5507 e00c 4305 02a4 3538  H..d}.U...C...58
-00002620: 0a22 fced b5a0 85f9 f342 a78c 9ca2 b4a7  .".......B......
-00002630: da75 3ac7 1db3 39eb c5c1 7d34 e560 6c9a  .u:...9...}4.`l.
-00002640: 2668 922e 86cb 1fe1 b7cd e373 57d5 2f65  &h.........sW./e
-00002650: 3b2b 0628 4f39 234c 03b5 4ae7 2b7d 90ca  ;+.(O9#L..J.+}..
-00002660: 5b6b a7a8 148f 8476 8815 3576 e3e6 bd2d  [k.....v..5v...-
-00002670: 81af 4ebf bcd7 bae3 7635 7a38 70cf 0523  ..N.....v5z8p..#
-00002680: 7d8d 8bf2 9adc 3f14 6b94 c761 9cf8 a15b  }.....?.k..a...[
-00002690: b322 ba23 9305 89ee dedb e77f dc6f 83f6  .".#.........o..
-000026a0: 07e2 1ce2 5fe2 d48f 2745 3427 d182 24d3  ...._...'E4'..$.
-000026b0: 11f1 02c8 537c f539 f22f 0000 00ff ff03  ....S|.9./......
-000026c0: 0050 4b03 0414 0006 0008 0000 0021 0055  .PK..........!.U
-000026d0: 9f35 f5d4 0900 008c 3000 0013 0028 0063  .5......0....(.c
-000026e0: 7573 746f 6d58 6d6c 2f69 7465 6d32 2e78  ustomXml/item2.x
-000026f0: 6d6c 20a2 2400 28a0 2000 0000 0000 0000  ml .$.(. .......
-00002700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002710: 0000 0000 0000 0000 0000 ec5b dd92 9b46  ...........[...F
-00002720: 16be 4f55 de81 d25e 3380 4002 5496 5363  ..OU...^3.@.T.Sc
-00002730: 8dbd eb8a 1dbb 32da ecde a59a a619 b146  ......2........F
-00002740: 80e9 6646 53a9 7da4 7d8a bc58 4e77 f38f  ..fFS.}.}..XNw..
-00002750: 7e00 4d36 a9ad 4d2e 3292 38a7 4f9f fff3  ~.M6..M.2.8.O...
-00002760: 1df2 eabb c33e 521e 4946 c324 5ecf 8c1b  .....>R.IF.$^...
-00002770: 7da6 9018 277e 183f ac67 390b 5467 f6dd  }...'~.?.g9.Tg..
-00002780: eb57 98ad 7012 3312 b3ed 734a eef1 8eec  .W..p.3...sJ....
-00002790: 9102 5ffe bc9e cd94 3daa fedb 78e8 07b4  .._.....=...x...
-000027a0: 27eb d95d 82f3 3d90 25e2 b1c6 cfef efd6  '..]..=.%.......
-000027b0: 33fd a01b f0af fece 340d c37d b39c 6f4c  3.......4..}..oL
-000027c0: 7b61 59ae 7b67 6fde 59ce adbb b973 96ce  {aY.{go.Y....s..
-000027d0: 62d9 a5fd a912 d7e8 fe74 4728 cec2 9489  b........tG(....
-000027e0: db6c 3282 3225 cec9 63a2 f8a5 2037 5d92  .l2.2%..c... 7].
-000027f0: 7b9c a420 a9f8 ba50 0417 ce70 e6fe 7cae  {.. ...P...p..|.
-00002800: 9bba 6706 4bd3 5dce 1d82 75ec 2cdc 39b6  ..g.K.]...u.,.9.
-00002810: 5cdd 013d 81e6 62ba c26c 3ddb 3196 ae34  \..=..b..l=.1..4
-00002820: 8d0a bdd0 9b7d 88b3 8426 01bb c1c9 5e4b  .....}...&....^K
-00002830: 8220 c444 9beb fa52 db13 867c c490 d6d0  . .D...R...|....
-00002840: 44c9 688f a630 4a33 903e 6321 a182 f92d  D.h..0J3.>c!...-
-00002850: 6359 e8e5 8cd0 d9eb 6fbf 7975 a0fe 4a4a  cY......o.yu..JJ
-00002860: a530 943d 10c6 ad42 5384 e1c2 e385 aecf  .0.=...BS.......
-00002870: 12ca ca92 04ee ceb2 9c88 8f41 4822 9f0a  ...........AH"..
-00002880: bb9a ae63 9300 e9a6 6b39 0bcf 3175 ddf4  ...c....k9..1u..
-00002890: 3dec baf3 b94d 40a7 3325 a673 e933 3135  =....M@.3%.s.315
-000028a0: e51f 5299 206f 25d8 d3d3 d3cd 9379 9364  ..R. o%......y.d
-000028b0: 0f5c 7786 f6cf 8f1f a4e3 950a 3bd0 e1cf  .\w.........;...
-000028c0: a6d7 de57 ca07 72af 679e ad2f d132 3055  ...W..r.g../.20U
-000028d0: dd0e 3cd5 f24c 4775 16fa 4245 b6bd 5862  ..<..LGu..BE..Xb
-000028e0: c770 3d0b 9532 c2fd c0cf 0dc7 40fe c256  .p=..2......@..V
-000028f0: 17ee 62ae 5a3a fc85 0214 a8b6 6e22 1f5c  ..b.Z:......n".\
-00002900: cc45 d8a9 cc15 eed3 2463 4a5c 1b6a d079  .E......$cJ\.j.y
-00002910: 5a69 ee3e fda0 e32b 7a12 111e b042 80f5  Zi.>...+z....B..
-00002920: ac61 f2f2 00f0 e934 2207 9e08 2a17 235f  .a.....4"...*.#_
-00002930: 73c8 1ad5 e736 8f32 f43e a218 3d08 e6d5  s....6.2.>..=...
-00002940: 658f f042 5154 b22d d964 2458 cfb8 cb7c  e..BQT.-.d$X...|
-00002950: 247e 88ee 49f6 0801 f5b1 0825 f0bd 30fe  $~..I......%..0.
-00002960: 8471 9e81 3be8 b3de 3d8e 12bf 4394 5dc5  .q..;...=...C.].
-00002970: e01e 320b de7d ae82 6fb0 1411 0eec 6560  ..2..}..o.....e`
-00002980: 2c16 98f8 96ef 63cf d25d db30 ad20 30b1  ,.....c..].0. 0.
-00002990: 69ce 8381 8ccc d516 1d36 88e1 dd6d 144d  i........6...m.M
-000029a0: 52c1 a7cd 8f93 e8fe 4a62 9221 9e60 b7e1  R.......Jb.!.`..
-000029b0: 9e47 fe78 edbf 7d04 07fb 1ba2 bb4d e20f  .G.x..}......M..
-000029c0: e560 aeee 7728 23fe 3f42 b6fb 3b85 0230  .`..w(#.?B..;..0
-000029d0: 5851 35dd 1db8 4c18 1da5 d478 a62c 5c4f  XQ5...L....x.,\O
-000029e0: fcdd f14c f15d e18f dc3d c567 da70 fbe1  ...L.]...=.g.p..
-000029f0: 44a2 485c 4ace c372 4c21 d0bb 24db df41  D.H\J..rL!..$..A
-00002a00: becd 23c8 c75f 7314 8590 8bfd 3a4d fe4e  ..#.._s.....:M.N
-00002a10: 39d5 dfd7 09f8 72e9 eb67 018d 410a 016b  9.....r..g..A..k
-00002a20: c8d4 9ae2 6129 3a8c 8324 456c c78b 82ad  ....a):..$El....
-00002a30: 7d46 1903 7fdc 4073 9225 60da d359 7070  }F....@s.%`..Ypp
-00002a40: b93b 29e8 9914 3b84 f979 c14f e4df 1319  .;)...;..y.O....
-00002a50: 0fad c2d8 2787 f5cc 815a 1a46 11f2 22a8  ....'....Z.F..".
-00002a60: e855 29f6 439a 46e8 59b6 6027 59ec 42df  .U).C.F.Y.`'Y.B.
-00002a70: 27d0 f455 6421 7478 598c a20b 74d0 55f9  '..Ud!txY...t.U.
-00002a80: 9fe2 e8b9 a0ac 5c19 2a4f 449a 6521 2314  ......\.*OD.e!#.
-00002a90: ba11 cc73 85e2 210a 1282 cbac 7e48 1891  ...s..!.....~H..
-00002aa0: 695a 0651 8bac 1b67 3c2c dbd5 a479 9d4e  iZ.Q...g<,...y.N
-00002ab0: 1aaf b4e2 8ed3 4a8f cd08 cdf4 68ff 3cda  ......J.....h.<.
-00002ac0: 3952 a32a 0d19 bc09 1be1 3847 798d 50d3  9R.*......8Gy.P.
-00002ad0: 51fa 3f56 5503 2a71 adae f951 7531 7448  Q.?VU.*q...Qu1tH
-00002ae0: e264 5f46 029f 84da 3134 e88c 92cb 3bde  .d_F....14....;.
-00002af0: 40f7 63ef fd1e baa6 2d7a e075 0bad 5aa1  @.c.....-z.u..Z.
-00002b00: fd96 85d0 7831 4415 9f28 217f 2e96 9d79  ....x1D..(!....y
-00002b10: 15a1 018a 68a3 3d7f 0fa5 e097 45d1 82a8  ....h.=.....E...
-00002b20: bc07 5179 13a2 f22e 446d b621 ff16 7c4a  ..Qy....Dm.!..|J
-00002b30: c93e 4265 091b 8982 d294 73b2 bd85 6e3b  .>Be......s...n;
-00002b40: 84a8 aeeb 4123 8c3d 5d45 c476 557f 1e58  ....A#.=]E.vU..X
-00002b50: c4b4 7d37 702c c987 64fb 7bc2 388d ee3a  ..}7p,..d.{.8..:
-00002b60: 8685 7d53 5d2c 1da2 06c4 d555 fe8d eaf8  ..}S],.....U....
-00002b70: cbb9 1104 4ee0 1534 28c6 bb24 e324 8187  ....N..4(..$.$..
-00002b80: 1656 e099 2a36 8901 248e c15b eda5 8a91  .V..*6..$..[....
-00002b90: e52d 5dc3 72b0 05c5 0e74 0393 502b 9dd1  .-].r....t..P+..
-00002ba0: efc9 f353 9271 1642 0d13 3a58 d13d a678  ...S.q.B..:X.=.x
-00002bb0: b585 1b74 1b07 38f2 5036 9ec6 ecb5 ec09  ...t..8.P6......
-00002bc0: aeed 11ce 273c d9b4 d56e 09ea bd14 c56f  ....'<...n.....o
-00002bd0: 0f2c 4398 115f d992 0313 7a3a 9de7 4bfe  .,C.._....z:..K.
-00002be0: 2f11 99a5 b641 4b1f 48fc c076 ca23 8a72  /....AK.H..v.#.r
-00002bf0: 2802 f3c5 a291 ff1b 45a2 6eac aea8 09bd  (.......E.n.....
-00002c00: feb4 d6d6 625c ce3b c269 44c6 3b42 7da5  ....b\.;.iD.;B}.
-00002c10: 5685 fd44 9f70 75e1 ec76 e0b5 8e00 6c19  V..D.pu..v....l.
-00002c20: 5317 fa8c 46a8 a84f fcdf d490 54e2 a06e  S...F..O....T..n
-00002c30: 7cd0 04ad fcbf 1bff 5fef c6db 3377 1d34  |......._...3w.4
-00002c40: e6e5 a001 52d1 2a28 6268 5760 6a57 3649  ....R.*(bhW`jW6I
-00002c50: 94ef 65c1 ee05 4d14 5298 e57e 316c ddd6  ..e...M.R..~1l..
-00002c60: 03ec ab73 db41 aa45 a064 7a4b c353 1d2f  ...s.A.E.dzK.S./
-00002c70: 9807 b66f 99b6 b590 a5ba 9dd3 bb82 d25d  ...o...........]
-00002c80: f224 da8b f5ac 040d ee00 8614 d5e0 8978  .$.............x
-00002c90: 2321 aa23 a84d f115 9fc3 60b6 af00 9c03  #!.#.M....`.....
-00002ca0: 7ce2 c872 a3fd 17bd c466 9700 84f3 2149  |..r.....f....!I
-00002cb0: bee4 690d 549e 4591 7ee2 c563 a6f0 9951  ..i.T.E.~..c...Q
-00002cc0: ce11 0575 b30a e7b1 97e4 3018 f176 a009  ...u......0..v..
-00002cd0: 4b74 535a 2389 7647 78a8 9152 e4aa 18f5  KtSZ#.vGx..R....
-00002ce0: af36 64d6 efd7 f13e 7e51 3b90 7dd9 8136  .6d....>~Q;.}..6
-00002cf0: 00bb c1b0 1bfa 8902 e0f1 913a 7e8c ff89  ...........:~...
-00002d00: 7c7a 9501 39fa 228c 38d0 70fc f9f7 30b4  |z..9.".8.p...0.
-00002d10: 776d d2e8 9e6a bb4d 0619 efea 91b7 7412  wm...j.M......t.
-00002d20: 017e c300 1a3f 5cc2 8a38 d8ba 9edd 620c  .~...?\..8....b.
-00002d30: de03 5d6a d3cb 84f4 83fc a96f f182 211f  ..]j.......o..!.
-00002d40: 8987 c974 05aa f447 f871 8da7 d59e 3c00  ...t...G.q....<.
-00002d50: 90e0 6451 44c4 d092 53ee cea5 679f f5ea  ..dQD...S...g...
-00002d60: e669 7fea fe74 4463 d1c1 8df8 0003 6858  .i...tDc......hX
-00002d70: 0078 1e62 54ac 3e60 57f3 05e6 bade fa28  .x.bT.>`W......(
-00002d80: 236a 731d 73a1 f740 e55a a805 15e6 7103  #js.s..@.Z....q.
-00002d90: 2cf4 a204 7fa9 50c4 bf80 850a 64ae 07cb  ,.....P.....d...
-00002da0: 4d97 72d2 9207 06cf 424d 2737 426a 1853  M.r.....BM'7Bj.S
-00002db0: 0603 2384 993c c2af c1c4 34cf 22a1 491f  ..#..<....4.".I.
-00002dc0: 6b85 96a8 66dc 185a fd2c a05e 0d28 b349  k...f..Z.,.^.(.I
-00002dd0: 207e a99e 4c00 1abc 0052 9665 584b 3cff   ~..L....R.eXK<.
-00002de0: 3218 7946 3609 a87e 48b0 80da ab53 fddc  2.yF6..~H....S..
-00002df0: 8b42 d8cf 6644 dca9 805d 35b8 35d5 bec2  .B..fD...]5.5...
-00002e00: 0d01 1435 35dd d2f4 b9e6 e31b 4849 f542  ...55.......HI.B
-00002e10: a4bf 182a d47a ecc2 2f71 bc50 5e5b 8636  ...*.z../q.P^[.6
-00002e20: 94c7 afd1 5ca1 c8da bed9 fedc f9a1 c246  ....\..........F
-00002e30: 1b75 abd8 4ff5 1f2e 2bc8 a93d 928f 5718  .u..O...+..=..W.
-00002e40: d207 4bb2 3305 c938 b147 f261 9006 5f91  ..K.3..8.G.a.._.
-00002e50: 1cfa 6d46 0b10 38be 8982 e343 405d 1987  ..mF..8....C@]..
-00002e60: e847 4a20 ab54 6b73 dcee 725a c717 9d52  .GJ .Tks..rZ...R
-00002e70: ab08 5669 1ad0 bf2e 96b4 0d53 d892 13de  ..Vi.......S....
-00002e80: 5c40 0704 6dc6 4915 ac58 c8a2 eede a60d  \@..m.I..X......
-00002e90: 8648 244c 20d4 1201 6ac1 56db 5fff c3f2  .H$L ...j.V._...
-00002ea0: e8cc 0134 f7fe 4530 072b 5a5d dc30 f5fa  ...4..E0.+Z].0..
-00002eb0: f52b 00e3 1848 fd7e 9198 d179 b0a7 afdc  .+...H.~...y....
-00002ec0: 93d6 8e50 fc90 4306 9f22 0b04 3f79 48b2  ...P..C.."..?yH.
-00002ed0: e7b3 b403 6491 372b 5e6e 7819 6619 790c  ....d.7+^nx.f.y.
-00002ee0: 7967 3f92 5b15 9d71 9c30 91da ca6f cab5  yg?.[..q.0...o..
-00002ef0: 4bf9 a572 e29f ed2e a412 4952 6007 1272  K..r......IR`..r
-00002f00: 1551 85ed 08bc e7b1 f748 a624 8142 d123  .Q.......H.$.B.#
-00002f10: 7c97 644a 2924 bd51 b6f0 044a d388 13f0  |.dJ)$.Q...J....
-00002f20: 8104 9800 f294 2630 9ec0 ee44 8192 abe4  ......&0...D....
-00002f30: 29bc 9a01 dd22 70ab 8e40 0104 bc42 10de  )...."p..@...B..
-00002f40: 55cc 6ebe fde6 9868 12fe ebde 427e 8b5a  U.n....h....B~.Z
-00002f50: b7bd bce3 88f8 7a1a dec1 e16b bc37 575b  ......z....k.7W[
-00002f60: 5f60 9865 e6da 176c 27b9 a39c eeee c170  _`.e...l'......p
-00002f70: f9a4 f818 b465 95a5 47ba c555 2faf 9c5f  .....e..G..U/.._
-00002f80: b85d 826b 06b4 4c2f b9b8 2c1a 9741 efb4  .].k..L/..,..A..
-00002f90: 14ba 6917 d3cf b013 8770 2c7e eb4d 78ab  ..i......p,~.Mx.
-00002fa0: e6b2 fa40 aba5 5a09 70b7 e6a7 56da 15c0  ...@..Z.p...V...
-00002fb0: 76f9 7ce7 e892 ba31 3a4d a595 53d2 796a  v.|....1:M..S.yj
-00002fc0: f09f d63d f8e7 fea2 fe84 ac32 091e 9d13  ...=.......2....
-00002fd0: 577c 4f09 63e2 b9ab 9e98 11b9 4423 89db  W|O.c.......D#..
-00002fe0: f3e0 70f2 3777 9b5b 4a13 1c42 caf3 df42  ..p.7w.[J..B...B
-00002ff0: 0bc1 9e27 9b1b 7815 1c4e d7d8 c654 ced3  ...'..x..N...T..
-00003000: 5853 ad5d 43c0 af55 bc40 a284 d775 6067  XS.]C..U.@...u`g
-00003010: 220f a8de 382b b45b 3d57 b8d2 39ba c124  "...8+.[=W..9..$
-00003020: f7cf 9491 fdfb 620a e047 0e26 2d55 0a45  ......b..G.&-U.E
-00003030: e114 dd20 37ab ef21 3da5 7bfb aa4c b70d  ... 7..!=.{..L..
-00003040: 7e5a 1d5d 3635 8430 8ec3 11dd 4c94 a5ab  ~Z.]65.0....L...
-00003050: aa81 6cda 79aa f6bc a9a9 4a6a f6ba 8425  ..l.y.....Jj...%
-00003060: 7994 0ef3 2309 48c6 5f60 eb54 c521 a9af  y...#.H._`.T.!..
-00003070: e0e4 f357 519b ddea 185a d82e 4fa6 05ec  ...WQ....Z..O...
-00003080: 7932 2def cda7 ca0c cbb4 df3d 591f b1b4  y2-........=Y...
-00003090: 9c11 c764 dd93 a69e cc8a db7a 3a31 187b  ...d.......z:1.{
-000030a0: 3a31 587b 3a31 987b 3a31 d87b 3cb1 5c9b  :1X{:1.{:1.{<.\.
-000030b0: 4f0d 744e 3d1c 39be 54a3 2634 0b95 00d7  O.tN=.9.T.&4....
-000030c0: dc40 5495 f171 26ce ee02 cfbd a4f2 021d  .@T..q&.........
-000030d0: 113f 48ca 38cd be35 5e7e 262a 859c d5ae  .?H.8..5^~&*....
-000030e0: 553b f6ff 13bc fe0d 0000 ffff 0300 504b  U;............PK
-000030f0: 0102 2d00 1400 0600 0800 0000 2100 bac4  ..-.........!...
-00003100: 8506 7901 0000 9805 0000 1300 0000 0000  ..y.............
-00003110: 0000 0000 0000 0000 0000 0000 5b43 6f6e  ............[Con
-00003120: 7465 6e74 5f54 7970 6573 5d2e 786d 6c50  tent_Types].xmlP
-00003130: 4b01 022d 0014 0006 0008 0000 0021 00b5  K..-.........!..
-00003140: 5530 23f4 0000 004c 0200 000b 0000 0000  U0#....L........
-00003150: 0000 0000 0000 0000 00b2 0300 005f 7265  ............._re
-00003160: 6c73 2f2e 7265 6c73 504b 0102 2d00 1400  ls/.relsPK..-...
-00003170: 0600 0800 0000 2100 9e81 d450 1101 0000  ......!....P....
-00003180: d603 0000 1a00 0000 0000 0000 0000 0000  ................
-00003190: 0000 d706 0000 786c 2f5f 7265 6c73 2f77  ......xl/_rels/w
-000031a0: 6f72 6b62 6f6f 6b2e 786d 6c2e 7265 6c73  orkbook.xml.rels
-000031b0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-000031c0: e619 1dd3 2302 0000 4104 0000 0f00 0000  ....#...A.......
-000031d0: 0000 0000 0000 0000 0000 2809 0000 786c  ..........(...xl
-000031e0: 2f77 6f72 6b62 6f6f 6b2e 786d 6c50 4b01  /workbook.xmlPK.
-000031f0: 022d 0014 0006 0008 0000 0021 009c 6391  .-.........!..c.
-00003200: 4caa 0000 00ea 0000 0014 0000 0000 0000  L...............
-00003210: 0000 0000 0000 0078 0b00 0078 6c2f 7368  .......x...xl/sh
-00003220: 6172 6564 5374 7269 6e67 732e 786d 6c50  aredStrings.xmlP
-00003230: 4b01 022d 0014 0006 0008 0000 0021 001a  K..-.........!..
-00003240: e8a8 b791 0600 00e5 1b00 0013 0000 0000  ................
-00003250: 0000 0000 0000 0000 0054 0c00 0078 6c2f  .........T...xl/
-00003260: 7468 656d 652f 7468 656d 6531 2e78 6d6c  theme/theme1.xml
-00003270: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00003280: e97d fce0 0e03 0000 1e08 0000 0d00 0000  .}..............
-00003290: 0000 0000 0000 0000 0000 1613 0000 786c  ..............xl
-000032a0: 2f73 7479 6c65 732e 786d 6c50 4b01 022d  /styles.xmlPK..-
-000032b0: 0014 0006 0008 0000 0021 00fb ed03 d299  .........!......
-000032c0: 0200 00ad 0500 0018 0000 0000 0000 0000  ................
-000032d0: 0000 0000 004f 1600 0078 6c2f 776f 726b  .....O...xl/work
-000032e0: 7368 6565 7473 2f73 6865 6574 312e 786d  sheets/sheet1.xm
-000032f0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00003300: 00d7 3478 30bb 0100 007d 0400 0018 0000  ..4x0....}......
-00003310: 0000 0000 0000 0000 0000 001e 1900 0063  ...............c
-00003320: 7573 746f 6d58 6d6c 2f69 7465 6d50 726f  ustomXml/itemPro
-00003330: 7073 322e 786d 6c50 4b01 022d 0014 0006  ps2.xmlPK..-....
-00003340: 0008 0000 0021 005c 9627 22c3 0000 0028  .....!.\.'"....(
-00003350: 0100 001e 0000 0000 0000 0000 0000 0000  ................
-00003360: 0037 1b00 0063 7573 746f 6d58 6d6c 2f5f  .7...customXml/_
-00003370: 7265 6c73 2f69 7465 6d32 2e78 6d6c 2e72  rels/item2.xml.r
-00003380: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
-00003390: 0021 0074 3f39 7ac2 0000 0028 0100 001e  .!.t?9z....(....
-000033a0: 0000 0000 0000 0000 0000 0000 003e 1d00  .............>..
-000033b0: 0063 7573 746f 6d58 6d6c 2f5f 7265 6c73  .customXml/_rels
-000033c0: 2f69 7465 6d31 2e78 6d6c 2e72 656c 7350  /item1.xml.relsP
-000033d0: 4b01 022d 0014 0006 0008 0000 0021 00bd  K..-.........!..
-000033e0: 8462 2390 0000 00db 0000 0013 0000 0000  .b#.............
-000033f0: 0000 0000 0000 0000 0044 1f00 0063 7573  .........D...cus
-00003400: 746f 6d58 6d6c 2f69 7465 6d31 2e78 6d6c  tomXml/item1.xml
-00003410: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00003420: b0c3 7579 f400 0000 4f01 0000 1800 0000  ..uy....O.......
-00003430: 0000 0000 0000 0000 0000 2d20 0000 6375  ..........- ..cu
-00003440: 7374 6f6d 586d 6c2f 6974 656d 5072 6f70  stomXml/itemProp
-00003450: 7331 2e78 6d6c 504b 0102 2d00 1400 0600  s1.xmlPK..-.....
-00003460: 0800 0000 2100 a05a 864d 8a01 0000 0703  ....!..Z.M......
-00003470: 0000 1000 0000 0000 0000 0000 0000 0000  ................
-00003480: 7f21 0000 646f 6350 726f 7073 2f61 7070  .!..docProps/app
-00003490: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-000034a0: 0000 2100 971e 9156 4b01 0000 6902 0000  ..!....VK...i...
-000034b0: 1100 0000 0000 0000 0000 0000 0000 3f24  ..............?$
-000034c0: 0000 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
-000034d0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-000034e0: 0021 0055 9f35 f5d4 0900 008c 3000 0013  .!.U.5......0...
-000034f0: 0000 0000 0000 0000 0000 0000 00c1 2600  ..............&.
-00003500: 0063 7573 746f 6d58 6d6c 2f69 7465 6d32  .customXml/item2
-00003510: 2e78 6d6c 504b 0506 0000 0000 1000 1000  .xmlPK..........
-00003520: 2604 0000 ee30 0000 0000                 &....0....
+00002570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000025a0: 0000 0000 0000 0000 0000 0084 9251 4bc3  .............QK.
+000025b0: 3014 85df 05ff 43c9 7b9b 6675 9b86 b683  0.....C.{.fu....
+000025c0: 297b 7220 5851 7c0b c9dd 566c 9292 6476  ){r XQ|...Vl..dv
+000025d0: fbf7 a6ed 56ab 1384 bc24 e7e4 cb39 97a4  ....V....$...9..
+000025e0: 8b83 ac82 4f30 b6d4 2a43 248a 5100 8a6b  ....O0..*C$.Q..k
+000025f0: 51aa 6d86 5e8a 5578 8b02 eb98 12ac d20a  Q.m.^.Ux........
+00002600: 3274 048b 16f9 f555 ca6b cab5 8127 a36b  2t.....U.k...'.k
+00002610: 30ae 041b 7892 b294 d719 da39 5753 8c2d  0...x......9WS.-
+00002620: df81 6436 f20e e5c5 8d36 9239 bf35 5b5c  ..d6.....6.9.5[\
+00002630: 33fe c1b6 8027 713c c312 1c13 cc31 dc02  3....'q<.....1..
+00002640: c37a 20a2 1352 f001 59ef 4dd5 0104 c750  .z ..R..Y.M....P
+00002650: 8104 e52c 2611 c1df 5e07 46da 3f2f 74ca  ...,&...^.F.?/t.
+00002660: c829 4b77 ac7d a753 dc31 5bf0 5e1c dc07  .)Kw.}.S.1[.^...
+00002670: 5b0e c6a6 69a2 26e9 62f8 fc04 bfad 1f9f  [...i.&.b.......
+00002680: bbaa 61a9 da59 7140 792a 38e5 0698 d326  ..a..Yq@y*8....&
+00002690: 5f9a bdd2 c1ca 7845 a778 24b4 43ac 9875  _.....xE.x$.C..u
+000026a0: 6b3f ef4d 0962 79fc e5bd d43d b7ab d1c3  k?.M.by....=....
+000026b0: 4104 3e18 ed6b 9c95 d7e4 fea1 58a1 7c12  A.>..k......X.|.
+000026c0: 4f92 30f6 6b56 9039 bdb9 a364 fede 3eff  O.0.kV.9...d..>.
+000026d0: e37e 1bb4 3f90 a710 ff12 a761 420a 32a5  .~..?......aB.2.
+000026e0: 7142 e3d9 8878 06e4 29be f81c f917 0000  qB...x..).......
+000026f0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00002700: 0021 0055 9f35 f5d4 0900 008c 3000 0013  .!.U.5......0...
+00002710: 0028 0063 7573 746f 6d58 6d6c 2f69 7465  .(.customXml/ite
+00002720: 6d32 2e78 6d6c 20a2 2400 28a0 2000 0000  m2.xml .$.(. ...
+00002730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002740: 0000 0000 0000 0000 0000 0000 0000 ec5b  ...............[
+00002750: dd92 9b46 16be 4f55 de81 d25e 3380 4002  ...F..OU...^3.@.
+00002760: 5496 5363 8dbd eb8a 1dbb 32da ecde a59a  T.Sc......2.....
+00002770: a619 b146 80e9 6646 53a9 7da4 7d8a bc58  ...F..fFS.}.}..X
+00002780: 4e77 f38f 7e00 4d36 a9ad 4d2e 3292 38a7  Nw..~.M6..M.2.8.
+00002790: 4f9f fff3 1df2 eabb c33e 521e 4946 c324  O........>R.IF.$
+000027a0: 5ecf 8c1b 7da6 9018 277e 183f ac67 390b  ^...}...'~.?.g9.
+000027b0: 5467 f6dd eb57 98ad 7012 3312 b3ed 734a  Tg...W..p.3...sJ
+000027c0: eef1 8eec 9102 5ffe bc9e cd94 3daa fedb  ......_.....=...
+000027d0: 78e8 07b4 27eb d95d 82f3 3d90 25e2 b1c6  x...'..]..=.%...
+000027e0: cfef efd6 33fd a01b f0af fece 340d c37d  ....3.......4..}
+000027f0: b39c 6f4c 7b61 59ae 7b67 6fde 59ce adbb  ..oL{aY.{go.Y...
+00002800: b973 96ce 62d9 a5fd a912 d7e8 fe74 4728  .s..b........tG(
+00002810: cec2 9489 db6c 3282 3225 cec9 63a2 f8a5  .....l2.2%..c...
+00002820: 2037 5d92 7b9c a420 a9f8 ba50 0417 ce70   7].{.. ...P...p
+00002830: e6fe 7cae 9bba 6706 4bd3 5dce 1d82 75ec  ..|...g.K.]...u.
+00002840: 2cdc 39b6 5cdd 013d 81e6 62ba c26c 3ddb  ,.9.\..=..b..l=.
+00002850: 3196 ae34 8d0a bdd0 9b7d 88b3 8426 01bb  1..4.....}...&..
+00002860: c1c9 5e4b 8220 c444 9beb fa52 db13 867c  ..^K. .D...R...|
+00002870: c490 d6d0 44c9 688f a630 4a33 903e 6321  ....D.h..0J3.>c!
+00002880: a182 f92d 6359 e8e5 8cd0 d9eb 6fbf 7975  ...-cY......o.yu
+00002890: a0fe 4a4a a530 943d 10c6 ad42 5384 e1c2  ..JJ.0.=...BS...
+000028a0: e385 aecf 12ca ca92 04ee ceb2 9c88 8f41  ...............A
+000028b0: 4822 9f0a bb9a ae63 9300 e9a6 6b39 0bcf  H".....c....k9..
+000028c0: 3175 ddf4 3dec baf3 b94d 40a7 3325 a673  1u..=....M@.3%.s
+000028d0: e933 3135 e51f 5299 206f 25d8 d3d3 d3cd  .315..R. o%.....
+000028e0: 9379 9364 0f5c 7786 f6cf 8f1f a4e3 950a  .y.d.\w.........
+000028f0: 3bd0 e1cf a6d7 de57 ca07 72af 679e ad2f  ;......W..r.g../
+00002900: d132 3055 dd0e 3cd5 f24c 4775 16fa 4245  .20U..<..LGu..BE
+00002910: b6bd 5862 c770 3d0b 9532 c2fd c0cf 0dc7  ..Xb.p=..2......
+00002920: 40fe c256 17ee 62ae 5a3a fc85 0214 a8b6  @..V..b.Z:......
+00002930: 6e22 1f5c cc45 d8a9 cc15 eed3 2463 4a5c  n".\.E......$cJ\
+00002940: 1b6a d079 5a69 ee3e fda0 e32b 7a12 111e  .j.yZi.>...+z...
+00002950: b042 80f5 ac61 f2f2 00f0 e934 2207 9e08  .B...a.....4"...
+00002960: 2a17 235f 73c8 1ad5 e736 8f32 f43e a218  *.#_s....6.2.>..
+00002970: 3d08 e6d5 658f f042 5154 b22d d964 2458  =...e..BQT.-.d$X
+00002980: cfb8 cb7c 247e 88ee 49f6 0801 f5b1 0825  ...|$~..I......%
+00002990: f0bd 30fe 8471 9e81 3be8 b3de 3d8e 12bf  ..0..q..;...=...
+000029a0: 4394 5dc5 e01e 320b de7d ae82 6fb0 1411  C.]...2..}..o...
+000029b0: 0eec 6560 2c16 98f8 96ef 63cf d25d db30  ..e`,.....c..].0
+000029c0: ad20 30b1 69ce 8381 8ccc d516 1d36 88e1  . 0.i........6..
+000029d0: dd6d 144d 52c1 a7cd 8f93 e8fe 4a62 9221  .m.MR.......Jb.!
+000029e0: 9e60 b7e1 9e47 fe78 edbf 7d04 07fb 1ba2  .`...G.x..}.....
+000029f0: bb4d e20f e560 aeee 7728 23fe 3f42 b6fb  .M...`..w(#.?B..
+00002a00: 3b85 0230 5851 35dd 1db8 4c18 1da5 d478  ;..0XQ5...L....x
+00002a10: a62c 5c4f fcdd f14c f15d e18f dc3d c567  .,\O...L.]...=.g
+00002a20: da70 fbe1 44a2 485c 4ace c372 4c21 d0bb  .p..D.H\J..rL!..
+00002a30: 24db df41 becd 23c8 c75f 7314 8590 8bfd  $..A..#.._s.....
+00002a40: 3a4d fe4e 39d5 dfd7 09f8 72e9 eb67 018d  :M.N9.....r..g..
+00002a50: 410a 016b c8d4 9ae2 6129 3a8c 8324 456c  A..k....a):..$El
+00002a60: c78b 82ad 7d46 1903 7fdc 4073 9225 60da  ....}F....@s.%`.
+00002a70: d359 7070 b93b 29e8 9914 3b84 f979 c14f  .Ypp.;)...;..y.O
+00002a80: e4df 1319 0fad c2d8 2787 f5cc 815a 1a46  ........'....Z.F
+00002a90: 11f2 22a8 e855 29f6 439a 46e8 59b6 6027  .."..U).C.F.Y.`'
+00002aa0: 59ec 42df 27d0 f455 6421 7478 598c a20b  Y.B.'..Ud!txY...
+00002ab0: 74d0 55f9 9fe2 e8b9 a0ac 5c19 2a4f 449a  t.U.......\.*OD.
+00002ac0: 6521 2314 ba11 cc73 85e2 210a 1282 cbac  e!#....s..!.....
+00002ad0: 7e48 1891 695a 0651 8bac 1b67 3c2c dbd5  ~H..iZ.Q...g<,..
+00002ae0: a479 9d4e 1aaf b4e2 8ed3 4a8f cd08 cdf4  .y.N......J.....
+00002af0: 68ff 3cda 3952 a32a 0d19 bc09 1be1 3847  h.<.9R.*......8G
+00002b00: 798d 50d3 51fa 3f56 5503 2a71 adae f951  y.P.Q.?VU.*q...Q
+00002b10: 7531 7448 e264 5f46 029f 84da 3134 e88c  u1tH.d_F....14..
+00002b20: 92cb 3bde 40f7 63ef fd1e baa6 2d7a e075  ..;.@.c.....-z.u
+00002b30: 0bad 5aa1 fd96 85d0 7831 4415 9f28 217f  ..Z.....x1D..(!.
+00002b40: 2e96 9d79 15a1 018a 68a3 3d7f 0fa5 e097  ...y....h.=.....
+00002b50: 45d1 82a8 bc07 5179 13a2 f22e 446d b621  E.....Qy....Dm.!
+00002b60: ff16 7c4a c93e 4265 091b 8982 d294 73b2  ..|J.>Be......s.
+00002b70: bd85 6e3b 84a8 aeeb 4123 8c3d 5d45 c476  ..n;....A#.=]E.v
+00002b80: 557f 1e58 c4b4 7d37 702c c987 64fb 7bc2  U..X..}7p,..d.{.
+00002b90: 388d ee3a 8685 7d53 5d2c 1da2 06c4 d555  8..:..}S],.....U
+00002ba0: fe8d eaf8 cbb9 1104 4ee0 1534 28c6 bb24  ........N..4(..$
+00002bb0: e324 8187 1656 e099 2a36 8901 248e c15b  .$...V..*6..$..[
+00002bc0: eda5 8a91 e52d 5dc3 72b0 05c5 0e74 0393  .....-].r....t..
+00002bd0: 502b 9dd1 efc9 f353 9271 1642 0d13 3a58  P+.....S.q.B..:X
+00002be0: d13d a678 b585 1b74 1b07 38f2 5036 9ec6  .=.x...t..8.P6..
+00002bf0: ecb5 ec09 aeed 11ce 273c d9b4 d56e 09ea  ........'<...n..
+00002c00: bd14 c56f 0f2c 4398 115f d992 0313 7a3a  ...o.,C.._....z:
+00002c10: 9de7 4bfe 2f11 99a5 b641 4b1f 48fc c076  ..K./....AK.H..v
+00002c20: ca23 8a72 2802 f3c5 a291 ff1b 45a2 6eac  .#.r(.......E.n.
+00002c30: aea8 09bd feb4 d6d6 625c ce3b c269 44c6  ........b\.;.iD.
+00002c40: 3b42 7da5 5685 fd44 9f70 75e1 ec76 e0b5  ;B}.V..D.pu..v..
+00002c50: 8e00 6c19 5317 fa8c 46a8 a84f fcdf d490  ..l.S...F..O....
+00002c60: 54e2 a06e 7cd0 04ad fcbf 1bff 5fef c6db  T..n|......._...
+00002c70: 3377 1d34 e6e5 a001 52d1 2a28 6268 5760  3w.4....R.*(bhW`
+00002c80: 6a57 3649 94ef 65c1 ee05 4d14 5298 e57e  jW6I..e...M.R..~
+00002c90: 316c ddd6 03ec ab73 db41 aa45 a064 7a4b  1l.....s.A.E.dzK
+00002ca0: c353 1d2f 9807 b66f 99b6 b590 a5ba 9dd3  .S./...o........
+00002cb0: bb82 d25d f224 da8b f5ac 040d ee00 8614  ...].$..........
+00002cc0: d5e0 8978 2321 aa23 a84d f115 9fc3 60b6  ...x#!.#.M....`.
+00002cd0: af00 9c03 7ce2 c872 a3fd 17bd c466 9700  ....|..r.....f..
+00002ce0: 84f3 2149 bee4 690d 549e 4591 7ee2 c563  ..!I..i.T.E.~..c
+00002cf0: a6f0 9951 ce11 0575 b30a e7b1 97e4 3018  ...Q...u......0.
+00002d00: f176 a009 4b74 535a 2389 7647 78a8 9152  .v..KtSZ#.vGx..R
+00002d10: e4aa 18f5 af36 64d6 efd7 f13e 7e51 3b90  .....6d....>~Q;.
+00002d20: 7dd9 8136 00bb c1b0 1bfa 8902 e0f1 913a  }..6...........:
+00002d30: 7e8c ff89 7c7a 9501 39fa 228c 38d0 70fc  ~...|z..9.".8.p.
+00002d40: f9f7 30b4 776d d2e8 9e6a bb4d 0619 efea  ..0.wm...j.M....
+00002d50: 91b7 7412 017e c300 1a3f 5cc2 8a38 d8ba  ..t..~...?\..8..
+00002d60: 9edd 620c de03 5d6a d3cb 84f4 83fc a96f  ..b...]j.......o
+00002d70: f182 211f 8987 c974 05aa f447 f871 8da7  ..!....t...G.q..
+00002d80: d59e 3c00 90e0 6451 44c4 d092 53ee cea5  ..<...dQD...S...
+00002d90: 679f f5ea e669 7fea fe74 4463 d1c1 8df8  g....i...tDc....
+00002da0: 0003 6858 0078 1e62 54ac 3e60 57f3 05e6  ..hX.x.bT.>`W...
+00002db0: bade fa28 236a 731d 73a1 f740 e55a a805  ...(#js.s..@.Z..
+00002dc0: 15e6 7103 2cf4 a204 7fa9 50c4 bf80 850a  ..q.,.....P.....
+00002dd0: 64ae 07cb 4d97 72d2 9207 06cf 424d 2737  d...M.r.....BM'7
+00002de0: 426a 1853 0603 2384 993c c2af c1c4 34cf  Bj.S..#..<....4.
+00002df0: 22a1 491f 6b85 96a8 66dc 185a fd2c a05e  ".I.k...f..Z.,.^
+00002e00: 0d28 b349 207e a99e 4c00 1abc 0052 9665  .(.I ~..L....R.e
+00002e10: 584b 3cff 3218 7946 3609 a87e 48b0 80da  XK<.2.yF6..~H...
+00002e20: ab53 fddc 8b42 d8cf 6644 dca9 805d 35b8  .S...B..fD...]5.
+00002e30: 35d5 bec2 0d01 1435 35dd d2f4 b9e6 e31b  5......55.......
+00002e40: 4849 f542 a4bf 182a d47a ecc2 2f71 bc50  HI.B...*.z../q.P
+00002e50: 5e5b 8636 94c7 afd1 5ca1 c8da bed9 fedc  ^[.6....\.......
+00002e60: f9a1 c246 1b75 abd8 4ff5 1f2e 2bc8 a93d  ...F.u..O...+..=
+00002e70: 928f 5718 d207 4bb2 3305 c938 b147 f261  ..W...K.3..8.G.a
+00002e80: 9006 5f91 1cfa 6d46 0b10 38be 8982 e343  .._...mF..8....C
+00002e90: 405d 1987 e847 4a20 ab54 6b73 dcee 725a  @]...GJ .Tks..rZ
+00002ea0: c717 9d52 ab08 5669 1ad0 bf2e 96b4 0d53  ...R..Vi.......S
+00002eb0: d892 13de 5c40 0704 6dc6 4915 ac58 c8a2  ....\@..m.I..X..
+00002ec0: eede a60d 8648 244c 20d4 1201 6ac1 56db  .....H$L ...j.V.
+00002ed0: 5fff c3f2 e8cc 0134 f7fe 4530 072b 5a5d  _......4..E0.+Z]
+00002ee0: dc30 f5fa f52b 00e3 1848 fd7e 9198 d179  .0...+...H.~...y
+00002ef0: b0a7 afdc 93d6 8e50 fc90 4306 9f22 0b04  .......P..C.."..
+00002f00: 3f79 48b2 e7b3 b403 6491 372b 5e6e 7819  ?yH.....d.7+^nx.
+00002f10: 6619 790c 7967 3f92 5b15 9d71 9c30 91da  f.y.yg?.[..q.0..
+00002f20: ca6f cab5 4bf9 a572 e29f ed2e a412 4952  .o..K..r......IR
+00002f30: 6007 1272 1551 85ed 08bc e7b1 f748 a624  `..r.Q.......H.$
+00002f40: 8142 d123 7c97 644a 2924 bd51 b6f0 044a  .B.#|.dJ)$.Q...J
+00002f50: d388 13f0 8104 9800 f294 2630 9ec0 ee44  ..........&0...D
+00002f60: 8192 abe4 29bc 9a01 dd22 70ab 8e40 0104  ....)...."p..@..
+00002f70: bc42 10de 55cc 6ebe fde6 9868 12fe ebde  .B..U.n....h....
+00002f80: 427e 8b5a b7bd bce3 88f8 7a1a dec1 e16b  B~.Z......z....k
+00002f90: bc37 575b 5f60 9865 e6da 176c 27b9 a39c  .7W[_`.e...l'...
+00002fa0: eeee c170 f9a4 f818 b465 95a5 47ba c555  ...p.....e..G..U
+00002fb0: 2faf 9c5f b85d 826b 06b4 4c2f b9b8 2c1a  /.._.].k..L/..,.
+00002fc0: 9741 efb4 14ba 6917 d3cf b013 8770 2c7e  .A....i......p,~
+00002fd0: eb4d 78ab e6b2 fa40 aba5 5a09 70b7 e6a7  .Mx....@..Z.p...
+00002fe0: 56da 15c0 76f9 7ce7 e892 ba31 3a4d a595  V...v.|....1:M..
+00002ff0: 53d2 796a f09f d63d f8e7 fea2 fe84 ac32  S.yj...=.......2
+00003000: 091e 9d13 577c 4f09 63e2 b9ab 9e98 11b9  ....W|O.c.......
+00003010: 4423 89db f3e0 70f2 3777 9b5b 4a13 1c42  D#....p.7w.[J..B
+00003020: caf3 df42 0bc1 9e27 9b1b 7815 1c4e d7d8  ...B...'..x..N..
+00003030: c654 ced3 5853 ad5d 43c0 af55 bc40 a284  .T..XS.]C..U.@..
+00003040: d775 6067 220f a8de 382b b45b 3d57 b8d2  .u`g"...8+.[=W..
+00003050: 39ba c124 f7cf 9491 fdfb 620a e047 0e26  9..$......b..G.&
+00003060: 2d55 0a45 e114 dd20 37ab ef21 3da5 7bfb  -U.E... 7..!=.{.
+00003070: aa4c b70d 7e5a 1d5d 3635 8430 8ec3 11dd  .L..~Z.]65.0....
+00003080: 4c94 a5ab aa81 6cda 79aa f6bc a9a9 4a6a  L.....l.y.....Jj
+00003090: f6ba 8425 7994 0ef3 2309 48c6 5f60 eb54  ...%y...#.H._`.T
+000030a0: c521 a9af e0e4 f357 519b ddea 185a d82e  .!.....WQ....Z..
+000030b0: 4fa6 05ec 7932 2def cda7 ca0c cbb4 df3d  O...y2-........=
+000030c0: 591f b1b4 9c11 c764 dd93 a69e cc8a db7a  Y......d.......z
+000030d0: 3a31 187b 3a31 587b 3a31 987b 3a31 d87b  :1.{:1X{:1.{:1.{
+000030e0: 3cb1 5c9b 4f0d 744e 3d1c 39be 54a3 2634  <.\.O.tN=.9.T.&4
+000030f0: 0b95 00d7 dc40 5495 f171 26ce ee02 cfbd  .....@T..q&.....
+00003100: a4f2 021d 113f 48ca 38cd be35 5e7e 262a  .....?H.8..5^~&*
+00003110: 859c d5ae 553b f6ff 13bc fe0d 0000 ffff  ....U;..........
+00003120: 0300 504b 0102 2d00 1400 0600 0800 0000  ..PK..-.........
+00003130: 2100 bac4 8506 7901 0000 9805 0000 1300  !.....y.........
+00003140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003150: 5b43 6f6e 7465 6e74 5f54 7970 6573 5d2e  [Content_Types].
+00003160: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+00003170: 0021 00b5 5530 23f4 0000 004c 0200 000b  .!..U0#....L....
+00003180: 0000 0000 0000 0000 0000 0000 00b2 0300  ................
+00003190: 005f 7265 6c73 2f2e 7265 6c73 504b 0102  ._rels/.relsPK..
+000031a0: 2d00 1400 0600 0800 0000 2100 9e81 d450  -.........!....P
+000031b0: 1101 0000 d603 0000 1a00 0000 0000 0000  ................
+000031c0: 0000 0000 0000 d706 0000 786c 2f5f 7265  ..........xl/_re
+000031d0: 6c73 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e  ls/workbook.xml.
+000031e0: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
+000031f0: 0000 2100 e619 1dd3 2302 0000 4104 0000  ..!.....#...A...
+00003200: 0f00 0000 0000 0000 0000 0000 0000 2809  ..............(.
+00003210: 0000 786c 2f77 6f72 6b62 6f6f 6b2e 786d  ..xl/workbook.xm
+00003220: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+00003230: 009c 6391 4caa 0000 00ea 0000 0014 0000  ..c.L...........
+00003240: 0000 0000 0000 0000 0000 0078 0b00 0078  ...........x...x
+00003250: 6c2f 7368 6172 6564 5374 7269 6e67 732e  l/sharedStrings.
+00003260: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+00003270: 0021 001a e8a8 b791 0600 00e5 1b00 0013  .!..............
+00003280: 0000 0000 0000 0000 0000 0000 0054 0c00  .............T..
+00003290: 0078 6c2f 7468 656d 652f 7468 656d 6531  .xl/theme/theme1
+000032a0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+000032b0: 0000 2100 e97d fce0 0e03 0000 1e08 0000  ..!..}..........
+000032c0: 0d00 0000 0000 0000 0000 0000 0000 1613  ................
+000032d0: 0000 786c 2f73 7479 6c65 732e 786d 6c50  ..xl/styles.xmlP
+000032e0: 4b01 022d 0014 0006 0008 0000 0021 00fe  K..-.........!..
+000032f0: ec43 95cc 0200 0091 0600 0018 0000 0000  .C..............
+00003300: 0000 0000 0000 0000 004f 1600 0078 6c2f  .........O...xl/
+00003310: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00003320: 312e 786d 6c50 4b01 022d 0014 0006 0008  1.xmlPK..-......
+00003330: 0000 0021 0039 34ab 99bd 0100 007d 0400  ...!.94......}..
+00003340: 0018 0000 0000 0000 0000 0000 0000 0051  ...............Q
+00003350: 1900 0063 7573 746f 6d58 6d6c 2f69 7465  ...customXml/ite
+00003360: 6d50 726f 7073 322e 786d 6c50 4b01 022d  mProps2.xmlPK..-
+00003370: 0014 0006 0008 0000 0021 005c 9627 22c3  .........!.\.'".
+00003380: 0000 0028 0100 001e 0000 0000 0000 0000  ...(............
+00003390: 0000 0000 006c 1b00 0063 7573 746f 6d58  .....l...customX
+000033a0: 6d6c 2f5f 7265 6c73 2f69 7465 6d32 2e78  ml/_rels/item2.x
+000033b0: 6d6c 2e72 656c 7350 4b01 022d 0014 0006  ml.relsPK..-....
+000033c0: 0008 0000 0021 0074 3f39 7ac2 0000 0028  .....!.t?9z....(
+000033d0: 0100 001e 0000 0000 0000 0000 0000 0000  ................
+000033e0: 0073 1d00 0063 7573 746f 6d58 6d6c 2f5f  .s...customXml/_
+000033f0: 7265 6c73 2f69 7465 6d31 2e78 6d6c 2e72  rels/item1.xml.r
+00003400: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
+00003410: 0021 00bd 8462 2390 0000 00db 0000 0013  .!...b#.........
+00003420: 0000 0000 0000 0000 0000 0000 0079 1f00  .............y..
+00003430: 0063 7573 746f 6d58 6d6c 2f69 7465 6d31  .customXml/item1
+00003440: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00003450: 0000 2100 5a69 9b33 f400 0000 4f01 0000  ..!.Zi.3....O...
+00003460: 1800 0000 0000 0000 0000 0000 0000 6220  ..............b 
+00003470: 0000 6375 7374 6f6d 586d 6c2f 6974 656d  ..customXml/item
+00003480: 5072 6f70 7331 2e78 6d6c 504b 0102 2d00  Props1.xmlPK..-.
+00003490: 1400 0600 0800 0000 2100 a05a 864d 8a01  ........!..Z.M..
+000034a0: 0000 0703 0000 1000 0000 0000 0000 0000  ................
+000034b0: 0000 0000 b421 0000 646f 6350 726f 7073  .....!..docProps
+000034c0: 2f61 7070 2e78 6d6c 504b 0102 2d00 1400  /app.xmlPK..-...
+000034d0: 0600 0800 0000 2100 e04f 8b29 4a01 0000  ......!..O.)J...
+000034e0: 6902 0000 1100 0000 0000 0000 0000 0000  i...............
+000034f0: 0000 7424 0000 646f 6350 726f 7073 2f63  ..t$..docProps/c
+00003500: 6f72 652e 786d 6c50 4b01 022d 0014 0006  ore.xmlPK..-....
+00003510: 0008 0000 0021 0055 9f35 f5d4 0900 008c  .....!.U.5......
+00003520: 3000 0013 0000 0000 0000 0000 0000 0000  0...............
+00003530: 00f5 2600 0063 7573 746f 6d58 6d6c 2f69  ..&..customXml/i
+00003540: 7465 6d32 2e78 6d6c 504b 0506 0000 0000  tem2.xmlPK......
+00003550: 1000 1000 2604 0000 2231 0000 0000       ....&..."1....
```

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/data_base_MM.xlsx` & `dp4plus_app-0.1.4/src/dp4plus_app/data_base_MM.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/data_base_QM.xlsx` & `dp4plus_app-0.1.4/src/dp4plus_app/data_base_QM.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/dp4_module.py` & `dp4plus_app-0.1.4/src/dp4plus_app/dp4_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,18 +170,18 @@
     uns_p, sca_p = calc_prob_matr (uns_e, sca_e, df_selections, parameters)
         
     results = calc_results(uns_p, sca_p, df_selections, isom_list)
    
     return {'exp': exp_data,
             'results': results,
             'tens' : tens,
-            'p_sca': sca_p,
+            #'p_sca': sca_p,
             'd_sca': sca,
             'e_sca': sca_e,
-            'p_uns': uns_p,
+            #'p_uns': uns_p,
             'd_uns': uns,
             'e_uns': uns_e}
```

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/logo_CONICET.png` & `dp4plus_app-0.1.4/src/dp4plus_app/logo_CONICET.png`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/logo_INGEBIO.png` & `dp4plus_app-0.1.4/src/dp4plus_app/logo_INGEBIO.png`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/main.py` & `dp4plus_app-0.1.4/src/dp4plus_app/main.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/main_gui_module.py` & `dp4plus_app-0.1.4/src/dp4plus_app/main_gui_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx`

 * *Files 20% similar despite different names*

```diff
@@ -147,2150 +147,2155 @@
 00000920: 0b67 529a 1bbc 59b8 6036 3337 6ae3 6c54  .gR...Y.`637j.lT
 00000930: 3477 a342 17ce a434 3734 ca79 6bc2 991b  4w.B...474.yk...
 00000940: e574 663d 33cc da79 6b26 b506 4b65 217b  .tf=3..yk&..Ke!{
 00000950: 23cb b314 2f4f 7c94 76d1 ac66 b666 e5b4  #.../O|.v..f.f..
 00000960: 8617 c374 7318 a9ab 7991 0c63 ef37 76e9  ...ts...y..c.7v.
 00000970: 2f67 3663 e982 799c 1286 7857 c2c5 8a3e  /g6c..y...xW...>
 00000980: 94fd 7778 3872 b46c 931f 0000 00ff ff03  ..wx8r.l........
-00000990: 0050 4b03 0414 0006 0008 0000 0021 009d  .PK..........!..
-000009a0: dbc5 4f55 0200 002d 0500 000f 0000 0078  ..OU...-.......x
+00000990: 0050 4b03 0414 0006 0008 0000 0021 00da  .PK..........!..
+000009a0: d77d d486 0200 008a 0500 000f 0000 0078  .}.............x
 000009b0: 6c2f 776f 726b 626f 6f6b 2e78 6d6c a454  l/workbook.xml.T
-000009c0: 4d8f da30 10bd 57ea 7fb0 7c87 9010 d825  M..0..W...|....%
-000009d0: 22ac 5ab6 55b9 54ab 8a5d 2e48 2bc7 31c4  ".Z.U.T..].H+.1.
-000009e0: c21f a9ed 2cf0 ef77 9c6c 4204 97ad 7a49  ....,..w.lB...zI
-000009f0: 3ce3 e737 9e37 339e 3f9c a440 6fcc 58ae  <..7.73.?..@o.X.
-00000a00: 558a c3e1 0823 a6a8 ceb9 daa7 f879 fd73  U....#.......y.s
-00000a10: 708f 9175 44e5 4468 c552 7c66 163f 2cbe  p..uD.Dh.R|f.?,.
-00000a20: 7e99 1fb5 3964 5a1f 1010 289b e2c2 b932  ~...9dZ...(....2
-00000a30: 0902 4b0b 2689 1dea 9229 d8d9 6923 8903  ..K.&....)..i#..
-00000a40: d3ec 035b 1a46 725b 30e6 a408 a2d1 681a  ...[.Fr[0.....h.
-00000a50: 48c2 156e 1812 f319 0ebd db71 ca1e 35ad  H..n.......q..5.
-00000a60: 2453 ae21 314c 1007 d7b7 052f 6dcb 26e9  $S.!1L...../m.&.
-00000a70: 67e8 2431 87aa 1c50 2d4b a0c8 b8e0 ee5c  g.$1...P-K.....\
-00000a80: 9362 2469 b2da 2b6d 4826 20ed 5338 6999  .b$i..+mH& .S8i.
-00000a90: 6179 432d 3935 daea 9d1b 0255 d05c f226  ayC-95.....U.\.&
-00000aa0: df70 1484 6193 f262 bee3 82bd 34b2 2352  .p..a..b....4.#R
-00000ab0: 96bf 89f4 5104 4682 58f7 23e7 8ee5 299e  ....Q.F.X.#...).
-00000ac0: 82a9 8fec e288 3132 55f9 bde2 0276 c338  ......12U....v.8
-00000ad0: 8e46 3858 74a5 7832 082a c71a ae75 c1ed  .F8Xt.x2.*...u..
-00000ae0: e6a3 4618 e56c 472a e1d6 509c 362c 1044  ..F..lG*..P.6,.D
-00000af0: 7114 4d3d 0324 fb4d 3866 1471 6ca9 9503  q.M=.$.M8f.ql...
-00000b00: 6d3f aaf2 bf3a d6dc cb42 43d5 d01f f6b7  m?...:...BC.....
-00000b10: e286 41b3 7839 1773 f812 9a90 cc3e 1157  ..A.x9.s.....>.W
-00000b20: a0ca 8814 2f93 edb3 0559 b699 a994 7e2d  ..../....Y....~-
-00000b30: f243 74a8 b2ed a33e 2aa1 a179 b64a 9a57  .Ct....>*..y.J.W
-00000b40: 5a59 a7e5 b657 1072 5bed 7f28 09a1 5e83  ZY...W.r[..(..^.
-00000b50: 0044 682e daac af05 59cc 7dbb bf70 76b4  .Dh.....Y.}..pv.
-00000b60: 17c9 bd89 4e1b ae72 7d4c f120 9c8d a124  ....N..r}L. ...$
-00000b70: e8dc 3966 601d ebdd 0dcf 5d01 9acf e2b8  ..9f`.....].....
-00000b80: f3fd 627c 5f38 704e c209 3809 75fc 8dad  ..b|_8pN..8.u...
-00000b90: 4996 e2bb fa46 bd80 f5d8 40e0 fa8f 54dd  I....F....@...T.
-00000ba0: 2e21 8ca6 9fa6 956f 0638 6f12 0e2b b3ca  .!.....o.8o..+..
-00000bb0: 437f ba8f 8cfa c871 0f19 5d23 61f3 c209  C......q..]#a...
-00000bc0: c73a cef1 3512 7af1 82f4 8dd9 468f af91  .:..5.z.....F...
-00000bd0: 303a 1724 181d 7272 8d84 86bf 20c1 e890  0:.$..rr.... ...
-00000be0: 7597 f633 baeb 23c1 e890 b572 7da4 7fc0  u..3..#....r}...
-00000bf0: 3a95 c0e8 90f7 b5c6 adb0 9408 ea07 087e  :..............~
-00000c00: b59e 9368 12d6 3a06 ed4b b778 0700 00ff  ...h..:..K.x....
-00000c10: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00000c20: 0091 31ef ca11 0900 0011 2f00 0018 0000  ..1......./.....
-00000c30: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00000c40: 6865 6574 342e 786d 6cac 9adb 72e3 3612  heet4.xml...r.6.
-00000c50: 86ef b76a df41 c5fb 5022 29cb 96cb f2d4  ...j.A..P").....
-00000c60: 6824 0a93 4a52 a91c af69 89b6 b923 895a  h$..JR...i...#.Z
-00000c70: 929e 439e 3e00 ba01 02dd 1e64 b616 b998  ..C.>......d....
-00000c80: 588d ee26 f4b1 01fc 8070 f7e6 f3e9 38f9  X..&.....p....8.
-00000c90: 5877 7dd3 9e57 4996 ce92 497d deb7 87e6  Xw}..WI...I}....
-00000ca0: fcb4 4a7e ffad fcee 2699 f443 753e 54c7  ..J~....&..Cu>T.
-00000cb0: f65c af92 2f75 9fbc b9ff f7bf ee3e b5dd  .\../u.......>..
-00000cc0: 87fe b9ae 8789 cc70 ee57 c9f3 305c 6ea7  .......p.W..0\n.
-00000cd0: d37e ff5c 9faa 3e6d 2ff5 59b6 3cb6 dda9  .~.\..>m/.Y.<...
-00000ce0: 1ae4 c7ee 69da 5fba ba3a e8a0 d371 9acf  ....i._..:...q..
-00000cf0: 668b e9a9 6ace 0964 b8ed be25 47fb f8d8  f...j..d...%G...
-00000d00: eceb 4dbb 7f39 d5e7 0192 74f5 b11a 64ff  ..M..9....t...d.
-00000d10: fbe7 e6d2 9b6c a7fd b7a4 3b55 dd87 97cb  .....l....;U....
-00000d20: 77fb f674 9129 1e9a 6333 7cd1 4993 c969  w..t.)..c3|.I..i
-00000d30: 7ffb fee9 dc76 d5c3 517e efcf d9bc da9b  .....v..Q~......
-00000d40: dcfa 034b 7f6a f65d dbb7 8f43 2ad3 4da1  ...K.j.]...C*.M.
-00000d50: a3fc 3b2f a7cb a9cc 747f a739 fcdc 4d24  ..;/....t..9..M$
-00000d60: ecfa a7ea 249f 21da ff54 f364 7a7f 7768  ....$.!..T.dz.wh
-00000d70: e497 536f 64d2 d58f abe4 6d76 2b8a a56a  ..Sod.....mv+..j
-00000d80: d031 7f34 f5a7 def9 7b32 b497 1fea c7e1  .1.4....{2......
-00000d90: 5d7d 3c4a e73c 4f26 7fb5 ede9 d77d a53a  ]}<J.<O&.....}.:
-00000da0: be94 6fd4 7efc 49bd 0de9 a48c ea05 3eb4  ..o.~.I.......>.
-00000db0: ed07 95ee fd61 95cc 549f ea63 bd57 2827  .....a..T..c.W('
-00000dc0: 95fc dfc7 1a52 7e5f 5ccb 22f8 afee 8bfa  .....R~_\.".....
-00000dd0: 5b76 646a 7be2 fe6d 7a55 ea97 2ebf db43  [vdj{..mzU.....C
-00000de0: d5d7 efda e39f cd61 7896 d525 9f7a a81f  .......ax..%.z..
-00000df0: ab97 e3f0 4bfb 49d4 cdd3 f320 ad8b f42a  ....K.I.... ...*
-00000e00: 99ec 5ffa a13d 599b 24ad 80df 1ebe 6cea  .._..=Y.$.....l.
-00000e10: 7e2f dfb4 ec5f 9aab 27ef dba3 7c8c fc77  ~/..._..'...|..w
-00000e20: 726a 54c5 ca17 557d 5659 8a9b b9fc 52f8  rjT...U}VY....R.
-00000e30: a42c 9de7 57d7 3759 2e53 f7c3 1705 a2d0  .,..W.7Y.S......
-00000e40: fd86 70dd fb4d 3554 f777 5dfb 6922 2b4f  ..p..M5T.w].i"+O
-00000e50: e6e9 2f95 aae3 ec56 96fc ffda 31d9 2395  ../....V....1.#.
-00000e60: 65ad d2ac 12f9 50d9 e15e 02fd 783f bb9b  e.....P..^..x?..
-00000e70: 7e94 8cf6 e8f1 8e7b 64be c786 7be4 bec7  ~......{d...{...
-00000e80: 967b 14be 47c9 3de6 bec7 8e7b 5cf9 1e82  .{..G.=....{\...
-00000e90: 7b2c acc7 5462 b3ec 64c1 4560 f756 a559  {,..Tb..d.E`.V.Y
-00000ea0: 25b9 a646 98ac a1cd e57a 4db8 1a0f c59c  %..F.....zM.....
-00000eb0: 1285 b605 64be cad2 25e1 6962 5579 a9d7  ....d...%.ibUy..
-00000ec0: 5882 e15a 0710 b43b ea2c 1c83 87a5 8883  X..Z...;.,......
-00000ed0: 45a5 3158 4821 aca1 2d84 c578 bc86 05da  E.1XH!..-..x....
-00000ee0: 104b 7e93 126c 5b13 6bb1 8001 b010 e71d  .K~..l[.k.......
-00000ef0: 7516 8ec1 c322 4769 8c6a 5169 0c16 f28a  u...."Gi.jQi....
-00000f00: d6d0 16c2 623c 5ec3 026d 88e5 e68a 558b  ....b<^..m....U.
-00000f10: 89b5 58c0 0058 c621 a22b 6947 9d85 63f0  ..X..X.!.+iG..c.
-00000f20: b0a8 89ea ff9f 80de aa34 060b 19f2 6b68  .........4....kh
-00000f30: 0b61 311e af61 8136 532d 57ac 5a4c acc5  .a1..a.6S-W.ZL..
-00000f40: 0206 c042 46eb 8e3a 0bc7 e061 59c4 c1a2  ...BF..:...aY...
-00000f50: d218 2c64 9e5b 435b 088b f178 0d0b b421  ..,d.[C[...x...!
-00000f60: 96c5 3c25 b5b8 35b1 160b 1800 cb0d 9994  ..<%..5.........
-00000f70: a9b3 700c 1e16 b520 47a8 1695 c660 2195  ..p.... G....`!.
-00000f80: bb86 b610 16e3 61be da06 0cc0 225f a6a4  ......a....."_..
-00000f90: feb6 d4bf 0403 a020 73f2 8e3a 0bc7 e0a1  ....... s..:....
-00000fa0: 5002 3502 0a95 c6a0 20d5 ba86 b610 0ae3  P.5..... .......
-00000fb0: 6151 8001 5014 4403 6ca9 7709 069c 5849  aQ..P.D.l.w...XI
-00000fc0: 7dee a8b7 700c 1e89 651c 122a 8d21 410a  }...p...e..*.!A.
-00000fd0: 740d 6d21 12c6 c392 0003 9228 5851 50ff  t.m!.......(XQP.
-00000fe0: 120c c882 2ebe d45b 3806 8f85 d29a 31ca  .......[8.....1.
-00000ff0: 42e7 3134 488d aeb1 3184 c3ba 581e 6801  B.14H...1...X.h.
-00001000: 208b 454a 106f 5944 8916 4442 34c0 8ef9   .EJ.oYD..DB4...
-00001010: 0bd7 e243 89a3 72df 6620 0d51 aa91 ea5e  ...C..r.f .Q...^
-00001020: 636b 908a d196 2315 b000 95f9 9cad 2e36  ck....#........6
-00001030: a99d 47d1 0254 e898 61ee c2b5 f850 22c9  ..G..T..a....P".
-00001040: d7cc d3af 54c0 626b 100a 5596 1b0c c252  ....T.bk..U....R
-00001050: c9d9 da62 938e 503c e54a 351a f317 aec5  ...b..P<.J5.....
-00001060: a712 49bd 66ae 7ccd a87e c5d6 2015 2a2c  ..I.f.|..~.. .*,
-00001070: 3718 8433 4a9e 9277 bfb5 4947 2aae 70cd  7..3J..w..IG*.p.
-00001080: e9a2 cbfc 856b f1a9 4412 af99 ab5e 332a  .....k..D....^3*
-00001090: 5fb1 3548 85ea ca0d 06e1 005a f001 c464  _.5H.......Z...d
-000010a0: 2b46 c000 caa9 42b3 9d30 1485 6bf1 a928  +F....B..0..k..(
-000010b0: f116 6109 ce40 04e2 b442 d52b b606 a950  ..a..@...B.+...P
-000010c0: 59b9 c120 a472 c36b 8546 9418 8154 d8bc  Y.. .r.k.F...T..
-000010d0: c284 abed 963a 1571 77c5 5924 e9aa f3d8  .....:.qw.Y$....
-000010e0: 7d31 15af d81a a442 55e5 0683 7004 6529  }1.....BU...p.e)
-000010f0: 917e 5b9b 741c 41ae 6a2d e8aa ccfc 856b  .~[.t.A.j-.....k
-00001100: f1a9 4452 ae99 2b5d 33aa 5db1 3548 85a9  ..DR..+]3.].5H..
-00001110: 570c c25a c9d9 becf 261d a9b8 02b6 a05b  W..Z....&......[
-00001120: 3fe6 2f5c 8b4f 2592 88cd 5c15 9b51 198b  ?./\.O%...\..Q..
-00001130: ad41 2a46 5bbe b6d5 c178 d4f7 393d 2eb0  .A*F[....x..9=..
-00001140: e947 3eae ae2d d8bc cb84 ad9b c1e7 1349  .G>..-.........I
-00001150: da66 aeb6 cda8 b8c5 d620 1f26 6f31 c86c  .f....... .&o1.l
-00001160: 0053 027d 6b93 8e54 5c85 3b27 ea69 c7fc  .S.}k..T\.;'.i..
-00001170: 856b f1a8 e491 34ae ce63 6718 2a72 b135  .k....4..cg.*r.5
-00001180: 44c5 ba58 3987 162c 9582 5161 1125 5a50  D..X9..,..Qa.%ZP
-00001190: e4d2 dd20 f317 aec5 a712 49e4 e646 e48e  ... ......I..F..
-000011a0: 67b9 3963 c3cf 48d9 b924 93ba 9818 2be6  g.9c..H..$....+.
-000011b0: 3acd 66ee 7f74 54a1 f795 3efb 86c3 49c8  :.f..tT...>...I.
-000011c0: 08a4 e6f4 5c97 f90b d7e2 938a 7570 0ba2  ....\.......up..
-000011d0: f3e6 f593 5b68 9435 6f8f c4c9 b87b a77e  ....[h.5o....{.~
-000011e0: b190 3bce e56b f11b 6c94 7b1a 3525 c9df  ..;..k..l.{.5%..
-000011f0: 0ad8 e1ad 89b6 03cc 8464 3a84 01a2 fec2  .........d:.....
-00001200: 3e9f 2ee1 7924 11ac f3ac 1200 4435 3036  >...y$......D506
-00001210: 0601 817e fd0a 2068 b480 3206 c844 8f80  ...~.. h..2..D..
-00001220: 3004 00d1 0da5 ed90 557e aec5 afa0 487a  0.......U~....Hz
-00001230: 3807 710a 80a8 f0c3 c620 2088 ff0a 2068  8.q......  ... h
-00001240: 1c01 d173 29fb 8011 1086 0020 ba50 ec58  ...s)...... .P.X
-00001250: 8070 2d3e a148 da58 ff90 a54a 681c 46f4  .p->.H.X...Jh.F.
-00001260: 5869 8d3e 4150 a05f f58f 89fa 807a 8341  Xi.>AP._.....z.A
-00001270: 4827 4faf d904 4443 4a13 8274 e82e d376  H'O...DCJ..t...v
-00001280: 63ac 1f27 854f 2792 46ce 419e 7a74 d84f  c..'.O'.F.A.zt.O
-00001290: 48e0 13a4 635c c675 0c2c 96ce 7ce9 4dd6  H...c\.u.,..|.M.
-000012a0: f487 39ec c788 b744 8b3c 7dd0 8a8a aef6  ..9....D.<}.....
-000012b0: 2c40 b816 9f55 24e5 9c83 68f5 58b1 3909  ,@...U$...h.X.9.
-000012c0: 7c82 ac8c cbc8 0a2c 232b 7ab2 854f 76e9  |......,#+z..Ov.
-000012d0: 6008 d2a1 7b50 1620 5c8b 4f27 9282 ce41  `...{P. \.O'...A
-000012e0: 947a 74e8 fe1c 7d82 7420 8d3b cec0 8274  .zt...}.t .;...t
-000012f0: b234 67b3 100d 29f1 39a6 76e8 fec2 7663  .4g...).9.v...vc
-00001300: 1c67 4e0a 9f4e 24fd 9c83 7485 799a ca67  .gN..N$...t.y..g
-00001310: 6c0c 6281 7817 0b58 6cd1 d05d c2d6 661d  l.b.x..Xl..]..f.
-00001320: 2767 0cc1 a261 eb3b 7d86 7053 7858 8a48  'g...a.;}.pSxX.H
-00001330: 025a e731 eb7b 4627 1e6c 0d71 b12e 7630  .Z.1.{F'.l.q..v0
-00001340: a105 b914 694e 7f57 6221 a509 012e 055d  ....iN.Wb!.....]
-00001350: d659 8070 2d3e 9748 12ba 00a5 ea0d 26ba  .Y.p->.H......&.
-00001360: baa3 4f90 0ea4 71aa 0683 6cd5 b0bd a8cd  ..O...q...l.....
-00001370: 6aab c684 201d 3a11 b300 e15a 7c3a 9164  j... .:....Z|:.d
-00001380: 7361 64b3 b3a4 d3e3 1df4 09d2 a17a 7683  sad..........zv.
-00001390: 4176 aa59 b0da 6192 d984 a022 a4db 2fdb  Av.Y..a...."../.
-000013a0: 0d3b d5b8 169f 4e24 cd5c 8046 c54d 05ab  .;....N$.\.F.M..
-000013b0: 1aa3 69bf beab c004 6ed5 784a 594e c1f4  ..i.....n.xJYN..
-000013c0: e498 8594 68c1 2938 a753 300b 10ae c5e7  ....h.)8.S0.....
-000013d0: 1249 2a17 462a 3b55 438f bfd0 2758 3546  .I*.F*;UC...'X5F
-000013e0: 318f 338e 2793 f357 e8d0 9012 9f83 740a  1.3.'..W......t.
-000013f0: 3a13 db6e 8c55 e3a4 f0e9 4492 c905 284d  :..n.U....D...(M
-00001400: 6fc6 a1c7 60e8 13a4 c364 3206 8dcb 371b  o...`....d2...7.
-00001410: 534c 269b 109c 71e8 51b2 edc6 48e7 6b32  SL&...q.Q...H.k2
-00001420: b988 2493 751e bb4e b1aa f967 818c 09dc  ..$.u..N...g....
-00001430: 3145 04f2 8c8a 3e16 52a2 c554 0d15 7d2c  1E....>.R..T..},
-00001440: 40b8 16bf 6a22 4962 7dbf d172 a1ba 065b  @...j"Ib}..r...[
-00001450: 83f5 c2c4 3006 d97a 99b1 cb55 34a4 3421  ....0..z...U4.4!
-00001460: 786c c12e 5899 00b5 9198 93d5 5dd8 4eea  xl..X.......].N.
-00001470: d6b1 387d 5e91 4472 6144 b2de d3d0 4331  ..8}^.DraD....C1
-00001480: 6c0d f262 f218 832c af39 9b9b 993c 3621  l..b...,.9...<6!
-00001490: b866 b115 dd04 a84e 5281 206c 2775 eb48  .f.....NR. l'u.H
-000014a0: d3e7 1549 36cb cbbb ea80 cb9d 95d8 5122  ...I6.........Q"
-000014b0: fa04 a931 f58c 4196 1a3b fbb1 5947 1de4  ...1..A..;..YG..
-000014c0: a967 8a79 6703 741d 9129 42dd 421e 4fea  .g.yg.t..)B.B.O.
-000014d0: e6e3 c805 6a70 2918 aed5 5eaa a7fa c7aa  ....jp)...^.....
-000014e0: 7b6a cefd e428 2f27 abfb bbb2 803b b8f3  {j...(/'.....;..
-000014f0: abff 96d7 96b5 55ce 7a0f ed20 6fff 9a4f  ......U.z.. o..O
-00001500: cff2 9678 2daf 61ce 52b9 603f b6ed 603e  ...x-.a.R.`?..`>
-00001510: c82f a1f2 fe5a 0f2f 9749 db35 f25e b0be  ./...Z./.I.5.^..
-00001520: f8bd 4a2e 6d37 7455 33c8 9bbb d2fe 572b  ..J.m7tU3.....W+
-00001530: 1b8e 9b4b 236f fd2e a4c6 97f7 db87 465e  ...K#o........F^
-00001540: 871e 2ddd 6d23 af3c 77ef 0f99 be15 6c2f  ..-.m#.<w.....l/
-00001550: b3df ff0d 0000 ffff 0300 504b 0304 1400  ..........PK....
-00001560: 0600 0800 0000 2100 3e65 cd63 2207 0000  ......!.>e.c"...
-00001570: 3c21 0000 1800 0000 786c 2f77 6f72 6b73  <!......xl/works
-00001580: 6865 6574 732f 7368 6565 7432 2e78 6d6c  heets/sheet2.xml
-00001590: ac9a 5993 9b46 10c7 df53 95ef 40f1 6e24  ..Y..F...S..@.n$
-000015a0: d0b5 52ad d665 ad0e 5c95 b852 718e 6716  ..R..e..\..Rq.g.
-000015b0: a115 b1d0 28c0 5efe f4e9 a17b 8699 1e99  ....(.^....{....
-000015c0: 3815 f6c1 96fa 62f8 d133 fc61 74fb feb5  8.....b..3.at...
-000015d0: 3879 cf59 59e5 e2bc f4c3 60e8 7bd9 3915  8y.YY.....`.{.9.
-000015e0: fbfc fcb8 f47f ff6d fbee c6f7 aa3a 39ef  .......m.....:9.
-000015f0: 9393 3867 4bff 2dab fcf7 773f fe70 fb22  ..8gK.-...w?.p."
-00001600: ca2f d531 cb6a 0f2a 9cab a57f aceb cb62  ./.1.j.*.......b
-00001610: 30a8 d263 5624 5520 2ed9 193c 0751 1649  0..cV$U ...<.Q.I
-00001620: 0d5f cbc7 4175 29b3 64df 2415 a741 341c  ._..Au).d.$..A4.
-00001630: 4e07 4592 9f7d acb0 28bf a786 381c f234  N.E..}..(...8..4
-00001640: 5b8b f4a9 c8ce 3516 29b3 5352 c3f8 ab63  [.....5.).SR...c
-00001650: 7ea9 54b5 22fd 9e72 4552 7e79 babc 4b45  ~.T."..rER~y..KE
-00001660: 7181 120f f929 afdf 9aa2 be57 a48b 8f8f  q....).....W....
-00001670: 6751 260f 2738 efd7 709c a4aa 76f3 c529  gQ&.'8..p...v..)
-00001680: 5fe4 6929 2a71 a803 2837 c081 bae7 3c1f  _.i)*q..(7....<.
-00001690: cc07 50e9 eeb6 e1f0 4be9 01ec ec53 52c0  ..P.....K....SR.
-000016a0: 3162 f157 32f2 0777 b7fb 1c4e 4e5e 11af  1b.W2..w...NN^..
-000016b0: cc0e 4bff 43b8 88a3 a974 3439 7fe4 d94b  ..K.C....t49...K
-000016c0: 657c f66a 71f9 293b d4f7 d9e9 04c1 33df  e|.jq.);......3.
-000016d0: fb2a 44f1 394d e4b8 e770 41f5 d74f f262  .*D.9M...pA..O.b
-000016e0: 408c 34ca ebf7 20c4 1759 ede3 7ee9 0fe5  @.4... ..Y..~...
-000016f0: 90b2 5396 4a92 5e02 ff3d 6758 7117 45d0  ..S.J.^..=gXq.E.
-00001700: 037f 3743 919f 611c 033d 10f3 b31a d4b6  ..7C..a..=......
-00001710: b9e6 706a 0f49 95dd 8bd3 9ff9 be3e 4273  ..pj.I.......>Bs
-00001720: c151 f7d9 2179 3ad5 bf8a 9738 cb1f 8f35  .Q..!y:....8...5
-00001730: 58a7 c1c4 f7d2 a7aa 1685 b601 68c9 7bb1  X...........h.{.
-00001740: 7f5b 6755 0a17 1ac6 1734 474e c509 0e03  .[gU.....4GN....
-00001750: ff7a 452e 1b16 ae53 f22a ab8c 6ec6 7052  .zE....S.*..n.pR
-00001760: 74a4 3018 4793 d94d 1841 e9aa 7e93 201a  t.0.G..M.A..~. .
-00001770: b003 4c6f 46bf 4eea e4ee b614 2f1e 341e  ..LoF.N...../.4.
-00001780: d4a9 2e89 6ce3 7001 1dff 5f07 0623 9255  ....l.p..._..#.U
-00001790: 56b2 ccd2 8783 c280 2b00 fa7c 37bc 1d3c  V.......+..|7..<
-000017a0: 03a3 9422 eedd 88d0 8e58 bb11 911d b171  ...".....X.....q
-000017b0: 2346 76c4 d68d 18db 113b 3762 6247 c46e  #Fv......;7bbG.n
-000017c0: c454 470c 009b 6627 bbe3 ffb3 fb20 cb2c  .TG...f'..... .,
-000017d0: fda8 a1c6 ce78 853e 93eb 8c71 5511 9239  .....x.>...qU..9
-000017e0: 278a be69 5339 1c87 c174 6efe 31b8 aa10  '..iS9...tn.1...
-000017f0: 7479 734d b768 9861 36bb 9c3b 1e1d 1b06  tysM.h.a6..;....
-00001800: 0bd2 a81f 48b2 8c82 c42e fa0a 7d5d 9054  ....H.......}].T
-00001810: c435 48e8 2348 7252 322e 2a57 7341 0372  .5H.#HrR2.*WsA.r
-00001820: 99b3 eee2 c1b1 61b0 b0c0 9ced a377 6419  ......a......wd.
-00001830: 89a5 9d77 111b ff0a 43ba e8a8 886b 74d0  ...w....C....kt.
-00001840: 4774 a269 d04e 85a6 4936 2a57 d341 03d2  Gt.i.N..I6*W.A..
-00001850: 61bd bae3 c1b1 61b0 e8c8 d5ab 8799 25cb  a.....a.......%.
-00001860: a8a6 61eb c00a 7d5d 5854 c435 2ce8 5358  ..a...}]XT.5,.SX
-00001870: 6601 eb83 8dca d558 d080 5858 ffee 7870  f......X..XX..xp
-00001880: 6c18 2c2c d37e b0c8 32ac 69d8 655d 6148  l.,,.~..2.i.e]aH
-00001890: 171d 1571 8d0e fa88 ce68 1484 5deb 8e2a  ...q.....h..]..*
-000018a0: a451 a101 51b1 71ed 7870 6c18 2c54 2006  .Q..Q.q.xpl.,T .
-000018b0: fae8 2059 4675 109f 58e8 eb62 a422 d4a9  .. YFu..X..b."..
-000018c0: add1 8060 a299 b3d4 f0f8 2d1a 6809 e66b  ...`......-.h..k
-000018d0: 0d8f 8e0d 83c5 422a d91e 6693 2ca3 58f0  ......B*..f.,.X.
-000018e0: 7e41 5f17 0b15 a159 a001 598c c280 ddbb  ~A_....Y..Y.....
-000018f0: 363c 7e8b 0662 c1fb 8247 c786 c162 31ef  6<~..b...G...b1.
-00001900: 8785 2ca3 58b0 556e 85be 2e16 2ae2 dadc  ..,.X.Un....*...
-00001910: 419f 5a59 2601 5b2c 362a 574f 1734 1017  A.ZY&.[,6*WO.4..
-00001920: ae76 7874 6c18 2c2e 52a3 f6d1 244d 1d45  .vxtl.,.R...$M.E
-00001930: e6c6 be3b aec8 d985 4687 5c63 434e 05e7  ...;....F.\cCN..
-00001940: a67b 61d1 a534 2ab2 102b a6b5 764e 7c6c  .{a..4*..+..vN|l
-00001950: 5a6c 5afd c8e6 0f21 6a4d ebfe cddb 8962  ZlZ....!jM.....b
-00001960: 3aa1 29c9 7a15 1a3a d56a cc84 dc46 976f  :.).z..:.j...F.o
-00001970: 2961 0252 628b dece 098f 4d8b 0da9 277d  )a.Rb.....M...'}
-00001980: 1c9a 0299 2d82 2b72 76d2 e992 c894 4f74  ....-.+rv.....Ot
-00001990: 86ee 9aac 0fd0 f231 85b1 d344 8e30 360b  .......1...D.06.
-000019a0: d87c 7a92 c6a1 d2c6 8608 7466 debf 6b64  .|z.......tf..kd
-000019b0: 2a33 41bd cf9f cd2c 953c 1907 6ca1 d9e8  *3A....,.<..l...
-000019c0: ec16 93a9 939d a730 4728 9b05 6c4c 3d49  .......0G(..lL=I
-000019d0: e550 69e5 6692 b069 b022 6f67 1f71 f9ba  .Pi.f..i."og.q..
-000019e0: a624 6a9e 7930 1d9a 7ffc 8ea6 0fd1 2232  .$j.y0........"2
-000019f0: c572 c4ef ef4e 7c6c 5a6c 4652 31f6 708b  .r...N|lZlFR1.p.
-00001a00: 0f51 79e2 b368 c84e 6045 de4e 465c cbae  .Qy..h.N`E.NF\..
-00001a10: 2949 3d84 3af7 795d b4a5 626a 65fe 38b3  )I=.:.y]..bje.8.
-00001a20: 73e2 63d3 6253 e949 2f87 4a30 379d c31f  s.c.bS.I/.J07...
-00001a30: d1c9 db49 85cb d635 25a9 a74e 773a 39aa  ...I...5%..Nw:9.
-00001a40: 9832 7055 8ed8 a5d9 e941 288a b169 b1a9  .2pU.....A(..i..
-00001a50: f424 8d43 949b 3757 df5b 9013 d486 7e21  .$.C..7W.[....~!
-00001a60: c496 a47b 1d72 f5a6 85c5 e106 2cbd b360  ...{.r......,..`
-00001a70: c465 90ce 6edb 8652 425c c01c 42e8 9ecb  .e..n..RB\..B...
-00001a80: b778 cda3 6b6c 96b0 09f5 2498 4314 a148  .x..kl....$.C..H
-00001a90: 883f 3d90 b393 10e6 b743 5e53 1261 1905  .?=......C^S.a..
-00001aa0: 23fe 38ae abb6 58b0 08dc a525 c988 bfc7  #.8...X....%....
-00001ab0: 7112 62d3 6263 e949 3b87 a841 615c ba37  q.b.bc.I;..Aa\.7
-00001ac0: 9cbb 3a86 74c2 5121 fa81 82ea 129c 2898  ..:.t.Q!......(.
-00001ad0: 3a3d c353 b62a 857a 86bf af20 b7d9 3346  :=.S.*.z... ..3F
-00001ae0: 090b 4ed4 937e 6eea 2c7d 134e c8ef 5514  ..N..~n.,}.N..U.
-00001af0: d345 4787 683a 64d1 7422 eb99 7cce 66e7  .EG.h:d.t"..|.f.
-00001b00: c629 b055 0588 154b d839 09b1 69b1 59f5  .).U...K.9..i.Y.
-00001b10: a49e 2314 aa38 bfb8 6c26 6727 24cc 9f5f  ..#..8..l&g'$.._
-00001b20: 553c 944f bc26 c19c 2b1e 7d00 3dd5 540a  U<.O.&..+.}.=.T.
-00001b30: 11e2 d2d9 4988 4d8b 4da8 af57 cba8 4691  ....I.M.M..W..F.
-00001b40: 10d7 84cd ee06 ec89 74ac d13a e4ea db65  ........t..:...e
-00001b50: 2c4e 84e0 c5a9 4308 03da e9b3 a57a b418  ,N....C......z..
-00001b60: 85fc 4598 3e9c 5ea3 4d8b 4da8 27f1 1ca1  ..E.>.^.M.M.'...
-00001b70: 1045 427c 1922 6727 21cc ff46 0fa1 53df  .EB|."g'!..F..S.
-00001b80: c586 fcdd b23e 40db 4394 423d c45e 2f3b  .....>@.C.B=.^/;
-00001b90: f1b1 69b1 01f5 249b 23d4 a808 c85d 8ad0  ..i...$.#....]..
-00001ba0: db49 4885 b44b 115a 080b bcfa 99d8 6b11  .IH..K.Z......k.
-00001bb0: df98 e005 b634 266a a391 b337 a112 64d7  .....4&j...7..d.
-00001bc0: 8e98 1088 2919 afd8 a855 7336 bd9e 0475  ....)....Us6...u
-00001bd0: b30f 2797 f366 0271 414d de4e 7a28 860d  ..'..f.qAM.Nz(..
-00001be0: 0d40 49df becd e9aa 6d53 6111 a501 f8cb  .@I.....mSa.....
-00001bf0: 339d d028 04b6 90c6 b6b7 5d44 6c5e 3d49  3..(......]Dl^=I
-00001c00: 6dd8 ed95 2fd6 8897 b31b 86de 4e5e 2aa4  m.../.......N^*.
-00001c10: ed36 b468 5e63 6799 e229 5b1a 85e2 c59f  .6.h^cg..)[.....
-00001c20: f1c9 8d1d 14b1 454c 6e58 cb53 206f 7b30  ......ELnX.S o{0
-00001c30: e485 1bc8 b805 7b49 1eb3 9f93 f231 3f57  ......{I.....1?W
-00001c40: de09 f6b1 e55e 2fa8 d412 f787 9bcf b0c3  .....^/.........
-00001c50: dd58 e102 3e88 1a76 8ad5 b723 fca0 2083  .X..>..v...#.. .
-00001c60: 9dd7 6100 0bc6 4188 5a7d 81f3 9675 3f67  ..a...A.Z}...u?g
-00001c70: f5d3 c513 650e 7bc8 cd6f 0496 fe45 9475  ....e.{..o...E.u
-00001c80: 99e4 35ec f282 fdab 00c7 697d c961 8778  ..5.......i}.a.x
-00001c90: 0ae2 057e 0a51 e7b0 75de 5aca 450e dbe3  ...~.Q..u.Z.E...
-00001ca0: e5c7 7dd8 ec7c ebdf 3ddc fd03 0000 ffff  ..}..|..=.......
-00001cb0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00001cc0: 3b6d 324b c100 0000 4201 0000 2300 0000  ;m2K....B...#...
-00001cd0: 786c 2f77 6f72 6b73 6865 6574 732f 5f72  xl/worksheets/_r
-00001ce0: 656c 732f 7368 6565 7431 2e78 6d6c 2e72  els/sheet1.xml.r
-00001cf0: 656c 7384 8fc1 8ac2 3014 45f7 03fe 4378  els.....0.E...Cx
-00001d00: 7b93 d685 0c43 5337 22b8 55e7 0362 fada  {....CS7".U..b..
-00001d10: 06db 9790 f714 fd7b b31c 65c0 e5e5 70cf  .......{..e...p.
-00001d20: e536 9bfb 3ca9 1b66 0e91 2cd4 ba02 85e4  .6..<..f..,.....
-00001d30: 6317 68b0 f07b da2d bf41 b138 eadc 1409  c.h..{.-.A.8....
-00001d40: 2d3c 9061 d32e be9a 034e 4e4a 89c7 9058  -<.a.....NNJ...X
-00001d50: 150b b185 5124 fd18 c37e c4d9 b18e 09a9  ....Q$...~......
-00001d60: 903e e6d9 4989 7930 c9f9 8b1b d0ac aa6a  .>..I.y0.......j
-00001d70: 6df2 5f07 b42f 4eb5 ef2c e47d 5783 3a3d  m._../N..,.}W.:=
-00001d80: 5259 feec 8e7d 1f3c 6ea3 bfce 48f2 cf84  RY...}.<n...H...
-00001d90: 4939 9060 3ea2 4839 c845 edf2 8062 41eb  I9.`>.H9.E...bA.
-00001da0: 77f6 9e6b 7d0e 04a6 6dcc cbf3 f609 0000  w..k}...m.......
-00001db0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00001dc0: 2100 13c4 2c13 c200 0000 4201 0000 2300  !...,.....B...#.
-00001dd0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00001de0: 5f72 656c 732f 7368 6565 7432 2e78 6d6c  _rels/sheet2.xml
-00001df0: 2e72 656c 7384 8fc1 6ac3 3010 44ef 85fc  .rels...j.0.D...
-00001e00: 83d8 7b24 3b87 508a 255f 4a21 d726 fd00  ..{$;.P.%_J!.&..
-00001e10: 455e dba2 f64a 68b7 25f9 fbe8 d884 428e  E^...Jh.%.....B.
-00001e20: c363 de30 5d7f 5917 f58b 8563 220b ad6e  .c.0].Y....c"..n
-00001e30: 4021 8534 449a 2c7c 9d3e b6af a058 3c0d  @!.4D.,|.>...X<.
-00001e40: 7e49 8416 aec8 d0bb cd4b f789 8b97 5ae2  ~I.......K....Z.
-00001e50: 3966 56d5 426c 6116 c96f c670 9871 f5ac  9fV.Bla..o.p.q..
-00001e60: 5346 aa64 4c65 f552 6399 4cf6 e1db 4f68  SF.dLe.Rc.L...Oh
-00001e70: 764d b337 e5af 03dc 9d53 1d06 0be5 30b4  vM.7.....S....0.
-00001e80: a04e d75c 979f bbd3 38c6 80ef 29fc ac48  .N.\....8...)..H
-00001e90: f2cf 84c9 2592 6039 a248 3dc8 55ed cb84  ....%.`9.H=.U...
-00001ea0: 6241 eb47 f698 77fa 1c09 8ceb ccdd 7377  bA.G..w.......sw
-00001eb0: 0300 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00001ec0: 0000 0021 0034 a109 92c2 0000 0042 0100  ...!.4.......B..
-00001ed0: 0023 0000 0078 6c2f 776f 726b 7368 6565  .#...xl/workshee
-00001ee0: 7473 2f5f 7265 6c73 2f73 6865 6574 332e  ts/_rels/sheet3.
-00001ef0: 786d 6c2e 7265 6c73 848f c16a c330 1044  xml.rels...j.0.D
-00001f00: ef81 fc83 d87b 2427 8552 82e5 5c42 20d7  .....{$'.R..\B .
-00001f10: 36fd 0055 5ecb 22f6 4a68 b7a5 f9fb ea58  6..U^.".Jh.....X
-00001f20: 9b42 8fc3 63de 30ed e97b 9ed4 1716 8e89  .B..c.0..{......
-00001f30: 2cec 7503 0ac9 a73e 52b0 f07e bbec 5e40  ,.u....>R..~..^@
-00001f40: b138 eadd 9408 2d3c 90e1 d46d 37ed 2b4e  .8....-<...m7.+N
-00001f50: 4e6a 89c7 9859 550b b185 5124 1f8d 613f  Nj...YU...Q$..a?
-00001f60: e2ec 58a7 8c54 c990 caec a4c6 124c 76fe  ..X..T.......Lv.
-00001f70: ee02 9a43 d33c 9bf2 db01 ddc2 a9ae bd85  ...C.<..........
-00001f80: 72ed f7a0 6e8f 5c97 ff77 a761 881e cfc9  r...n.\..w.a....
-00001f90: 7fce 48f2 c784 c925 9260 7943 917a 90ab  ..H....%.`yC.z..
-00001fa0: da95 8062 41eb 355b e727 fd11 094c d79a  ...bA.5[.'...L..
-00001fb0: c5f3 ee07 0000 ffff 0300 504b 0304 1400  ..........PK....
-00001fc0: 0600 0800 0000 2100 4396 11a3 c200 0000  ......!.C.......
-00001fd0: 4201 0000 2300 0000 786c 2f77 6f72 6b73  B...#...xl/works
-00001fe0: 6865 6574 732f 5f72 656c 732f 7368 6565  heets/_rels/shee
-00001ff0: 7434 2e78 6d6c 2e72 656c 7384 8fc1 6ac3  t4.xml.rels...j.
-00002000: 3010 44ef 81fc 83d8 7b24 2794 5282 e55c  0.D.....{$'.R..\
-00002010: 4220 d736 fd00 555e cb22 f64a 68b7 a5f9  B .6..U^.".Jh...
-00002020: fbea 589b 428f c363 de30 ede9 7b9e d417  ..X.B..c.0..{...
-00002030: 168e 892c ec75 030a c9a7 3e52 b0f0 7ebb  ...,.u....>R..~.
-00002040: ec5e 40b1 38ea dd94 082d 3c90 e1d4 6d37  .^@.8....-<...m7
-00002050: ed2b 4e4e 6a89 c798 5955 0bb1 8551 241f  .+NNj...YU...Q$.
-00002060: 8d61 3fe2 ec58 a78c 54c9 90ca eca4 c612  .a?..X..T.......
-00002070: 4c76 feee 029a 43d3 3c9b f2db 01dd c2a9  Lv....C.<.......
-00002080: aebd 8572 edf7 a06e 8f5c 97ff 77a7 6188  ...r...n.\..w.a.
-00002090: 1ecf c97f ce48 f2c7 84c9 2592 6079 4391  .....H....%.`yC.
-000020a0: 7a90 abda 9580 6241 eb35 5be7 27fd 1109  z.....bA.5[.'...
-000020b0: 4cd7 9ac5 f3ee 0700 00ff ff03 0050 4b03  L............PK.
-000020c0: 0414 0006 0008 0000 0021 0064 f334 22c2  .........!.d.4".
-000020d0: 0000 0042 0100 0023 0000 0078 6c2f 776f  ...B...#...xl/wo
-000020e0: 726b 7368 6565 7473 2f5f 7265 6c73 2f73  rksheets/_rels/s
-000020f0: 6865 6574 352e 786d 6c2e 7265 6c73 848f  heet5.xml.rels..
-00002100: c16a c330 1044 ef81 fc83 d87b 2427 d052  .j.0.D.....{$'.R
-00002110: 82e5 5c42 20d7 36fd 0055 5ecb 22f6 4a68  ..\B .6..U^.".Jh
-00002120: b7a5 f9fb ea58 9b42 8fc3 63de 30ed e97b  .....X.B..c.0..{
-00002130: 9ed4 1716 8e89 2cec 7503 0ac9 a73e 52b0  ......,.u....>R.
-00002140: f07e bbec 5e40 b138 eadd 9408 2d3c 90e1  .~..^@.8....-<..
-00002150: d46d 37ed 2b4e 4e6a 89c7 9859 550b b185  .m7.+NNj...YU...
-00002160: 5124 1f8d 613f e2ec 58a7 8c54 c990 caec  Q$..a?..X..T....
-00002170: a4c6 124c 76fe ee02 9a43 d33c 9bf2 db01  ...Lv....C.<....
-00002180: ddc2 a9ae bd85 72ed f7a0 6e8f 5c97 ff77  ......r...n.\..w
-00002190: a761 881e cfc9 7fce 48f2 c784 c925 9260  .a......H....%.`
-000021a0: 7943 917a 90ab da95 8062 41eb 355b e727  yC.z.....bA.5[.'
-000021b0: fd11 094c d79a c5f3 ee07 0000 ffff 0300  ...L............
-000021c0: 504b 0304 1400 0600 0800 0000 2100 4c5a  PK..........!.LZ
-000021d0: 2a7a c200 0000 4201 0000 2300 0000 786c  *z....B...#...xl
-000021e0: 2f77 6f72 6b73 6865 6574 732f 5f72 656c  /worksheets/_rel
-000021f0: 732f 7368 6565 7436 2e78 6d6c 2e72 656c  s/sheet6.xml.rel
-00002200: 7384 8fc1 6ac3 3010 44ef 85fc 83d8 7b24  s...j.0.D.....{$
-00002210: a707 538a e55c 4a20 d726 fd00 555e dba2  ..S..\J .&..U^..
-00002220: f64a 6837 21fe fbe8 589b 428f c363 de30  .Jh7!...X.B..c.0
-00002230: cdf1 314f ea8e 9943 240b 075d 8142 f2b1  ..1O...C$..].B..
-00002240: 0b34 58f8 ba9e f66f a058 1c75 6e8a 8416  .4X....o.X.un...
-00002250: 1664 38b6 bb97 e613 2727 a5c4 6348 ac8a  .d8.....''..cH..
-00002260: 85d8 c228 92de 8d61 3fe2 ec58 c784 5448  ...(...a?..X..TH
-00002270: 1ff3 eca4 c43c 98e4 fc8f 1bd0 bc56 556d  .....<.......VUm
-00002280: f26f 07b4 2ba7 3a77 16f2 b93b 80ba 2ea9  .o..+.:w...;....
-00002290: 2cff ef8e 7d1f 3c7e 447f 9b91 e48f 0993  ,...}.<~D.......
-000022a0: 7220 c17c 4191 7290 8bda e501 c582 d65b  r .|A.r........[
-000022b0: b6cd b5fe 0e04 a66d ccea 79fb 0400 00ff  .......m..y.....
-000022c0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-000022d0: 006b 3f0f fbc3 0000 0042 0100 0023 0000  .k?......B...#..
-000022e0: 0078 6c2f 776f 726b 7368 6565 7473 2f5f  .xl/worksheets/_
-000022f0: 7265 6c73 2f73 6865 6574 372e 786d 6c2e  rels/sheet7.xml.
-00002300: 7265 6c73 848f c16a c330 1044 ef81 fc83  rels...j.0.D....
-00002310: d87b 2427 87b6 04cb b984 40ae 6dfa 01aa  .{$'......@.m...
-00002320: bc96 45ec 95d0 6e4b f3f7 d5b1 3685 1e87  ..E...nK....6...
-00002330: c7bc 61da d3f7 3ca9 2f2c 1c13 59d8 eb06  ..a...<./,..Y...
-00002340: 1492 4f7d a460 e1fd 76d9 bd80 6271 d4bb  ..O}.`..v...bq..
-00002350: 2911 5a78 20c3 a9db 6eda 579c 9cd4 128f  ).Zx ...n.W.....
-00002360: 31b3 aa16 620b a348 3e1a c37e c4d9 b14e  1...b..H>..~...N
-00002370: 19a9 9221 95d9 498d 2598 ecfc dd05 3487  ...!..I.%.....4.
-00002380: a679 32e5 b703 ba85 535d 7b0b e5da ef41  .y2.....S]{....A
-00002390: dd1e b92e ffef 4ec3 103d 9e93 ff9c 91e4  ......N..=......
-000023a0: 8f09 934b 24c1 f286 22f5 2057 b52b 01c5  ...K$...". W.+..
-000023b0: 82d6 6bb6 cecf fa23 1298 ae35 8be7 dd0f  ..k....#...5....
-000023c0: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-000023d0: 0000 0021 00a2 341a 18c2 0000 0042 0100  ...!..4......B..
-000023e0: 0023 0000 0078 6c2f 776f 726b 7368 6565  .#...xl/workshee
-000023f0: 7473 2f5f 7265 6c73 2f73 6865 6574 382e  ts/_rels/sheet8.
-00002400: 786d 6c2e 7265 6c73 848f c18a c230 1445  xml.rels.....0.E
-00002410: f782 ff10 de7e 92ea 6210 69ea 4606 ba75  .....~..b.i.F..u
-00002420: f403 62fa da06 db97 90f7 6698 fefd 64a9  ..b.......f...d.
-00002430: 22b8 bc1c eeb9 dcfa f037 4fea 1733 8748  "........7O..3.H
-00002440: 1636 ba02 85e4 6317 68b0 7039 7f7d ec40  .6....c.h.p9.}.@
-00002450: b138 eadc 1409 2d2c c870 68d6 abfa 8493  .8....-,.ph.....
-00002460: 9352 e231 2456 c542 6c61 1449 7b63 d88f  .R.1$V.Bla.I{c..
-00002470: 383b d631 2115 d2c7 3c3b 2931 0f26 397f  8;.1!...<;)1.&9.
-00002480: 7303 9a6d 557d 9a7c ef80 e6c1 a9da ce42  s..mU}.|.......B
-00002490: 6ebb 0da8 f392 caf2 7b77 ecfb e0f1 18fd  n.......{w......
-000024a0: cf8c 242f 264c ca81 04f3 378a 9483 5cd4  ..$/&L....7...\.
-000024b0: 2e0f 2816 b47e 66cf 79a7 af81 c034 b579  ..(..~f.y....4.y
-000024c0: 78de fc03 0000 ffff 0300 504b 0304 1400  x.........PK....
-000024d0: 0600 0800 0000 2100 6706 faad cc09 0000  ......!.g.......
-000024e0: 9c34 0000 1800 0000 786c 2f77 6f72 6b73  .4......xl/works
-000024f0: 6865 6574 732f 7368 6565 7433 2e78 6d6c  heets/sheet3.xml
-00002500: ac9b 4d73 db38 1286 ef5b b5ff 41c5 7b28  ..Ms.8...[..A.{(
-00002510: 9194 f5e1 b29c b242 49cc 61a7 b676 bece  .......BI.a..v..
-00002520: b444 dbdc 48a2 96a4 e364 7efd 02ec 06d8  .D..H....d~.....
-00002530: e8d6 d099 1ae4 e058 8dee 06f4 b001 bc04  .......X........
-00002540: cdbb 8fdf 4ec7 d1d7 a26e caea bc0a a270  ....N....n.....p
-00002550: 128c 8af3 be3a 94e7 e755 f0eb 2fdb 0f8b  .....:...U../...
-00002560: 60d4 b4f9 f990 1fab 73b1 0abe 174d f0f1  `.......s....M..
-00002570: fe9f ffb8 7bab ea2f cd4b 51b4 2395 e1dc  ....{../.KQ.#...
-00002580: ac82 97b6 bddc 8ec7 cdfe a538 e54d 585d  ...........8.MX]
-00002590: 8ab3 6a79 aaea 53de aa8f f5f3 b8b9 d445  ..jy..S........E
-000025a0: 7ee8 824e c771 3c99 ccc6 a7bc 3c07 90e1  ~..N.q<.....<...
-000025b0: b6fe 911c d5d3 53b9 2fd2 6aff 7a2a ce2d  ......S./.j.z*.-
-000025c0: 24a9 8b63 deaa f137 2fe5 a531 d94e fb1f  $..c...7/..1.N..
-000025d0: 4977 caeb 2faf 970f fbea 7451 291e cb63  Iw../.....tQ)..c
-000025e0: d97e ef92 06a3 d3fe f6f3 f3b9 aaf3 c7a3  .~..............
-000025f0: fade dfa2 69be 37b9 bb0f 22fd a9dc d755  ....i.7..."....U
-00002600: 533d b5a1 4a37 8681 caef bc1c 2fc7 2ad3  S=..J7....../.*.
-00002610: fd5d c7e1 dff5 48c1 2e7e ca4f aa8f acfa  .]....H..~.O....
-00002620: 6f1e 07e3 fbbb 43a9 be9c be22 a3ba 785a  o.....C...."..xZ
-00002630: 050f d16d 369d ea86 2ee6 b7b2 786b c8ef  ...m6.......xk..
-00002640: a33f aaea f4f3 3ed7 c35c aaeb 673f fea4  .?....>..\..g?..
-00002650: d91f c1a8 2fd7 6355 7dd1 c19f 0fab 60a2  ..../.cU}.....`.
-00002660: 4750 1c8b bd06 37ca d57f 5f8b 4fc5 5179  GP....7..._.O.Qy
-00002670: efe2 99ba e4ff eb7a d6bf ab6e c7b6 5ffa  .......z...n.._.
-00002680: bb19 c3b6 bbc4 ea9b 3ce6 4df1 a93a fe5e  ........<.M..:.^
-00002690: 1eda 1755 4b6a 2887 e229 7f3d b6ff a9de  ...UKj(..).=....
-000026a0: b2a2 7c7e 6995 7516 de04 a3fd 6bd3 5627  ..|~i.u.....k.V'
-000026b0: 6b53 5c35 dedb c3f7 b468 f6ea baaa f185  kS\5.....h......
-000026c0: 1d89 7d75 54dd a89f a353 a9eb 535d 96fc  ..}uT....S..S]..
-000026d0: 9bce 922c a6c1 e80d 7b8a c269 7c33 5f44  ...,....{..i|3_D
-000026e0: b14a ddb4 df35 88a4 1b37 8477 a34f f336  .J...5...7.w.O.6
-000026f0: bfbf abab b791 aa33 95a7 b9e4 ba6a a35b  .......3.....j.[
-00002700: 55e0 7f75 606a 443a cb5a a759 05aa 5335  U..u`jD:.Z.Y..S5
-00002710: e046 01fd 7a3f b91b 7f55 8cf6 e8f1 497a  .F..z?...U....Iz
-00002720: 44ae 472a 3d62 d763 233d 12d7 632b 3da6  D.G*=b.c#=..c+=.
-00002730: aec7 4e7a dcb8 1e99 f498 598f b1c2 66d9  ..Nz......Y...f.
-00002740: c55e d83d e834 ab20 eea8 3126 6b68 a35c  .^.=.4. ..1&kh.\
-00002750: e78c abf1 d0cc 3951 689b 41e6 380e 394f  ......9Qh.A.8.9O
-00002760: 13ab 0abb bb8c 5b30 ccbb 00e6 bce3 ce19  ......[0........
-00002770: 3138 5812 3f58 741a 8385 8d65 0d6d 4358  18X.?Xt....e.mCX
-00002780: 8cc7 352c d066 b04c 0516 136b b180 01b0  ..5,.f.L...k....
-00002790: b06a d971 e78c 181c 2c6a 967a 9869 0f3a  .j.q....,j.z.i.:
-000027a0: 8dc1 c2aa 7f0d 6d43 588c c735 2cd0 66b0  ......mCX..5,.f.
-000027b0: 2c42 f64d 3726 d662 0103 60e9 a748 5749  ,B.M7&.b..`..HWI
-000027c0: 3bee 9c11 8383 452f 547f 7f01 7ad0 690c  ;.....E/T...z.i.
-000027d0: 1636 e5d7 d036 84c5 785c c302 6d88 452d  .6...6..x\..m.E-
-000027e0: da7c 1299 588b 050c 8085 5da1 1d77 ce88  .|..X.....]..w..
-000027f0: c1c1 a277 1e0f 5874 1a83 855d cf35 b40d  ...w..Xt...].5..
-00002800: 6131 1ed7 b040 1b62 99c6 61b4 a4ff d8c2  a1...@.b..a.....
-00002810: 6d12 5946 6000 466c 45db 71e7 8c18 1c46  m.YF`.FlE.q....F
-00002820: 733f 8c74 1ac3 8895 f11a da86 1819 8f6b  s?.t...........k
-00002830: 8ca0 0d19 2571 b898 907f 6cb1 de98 4496  ....%q....l...D.
-00002840: 1118 8011 dfc5 b873 460c 0e23 2d5a 3dd4  .......sF..#-Z=.
-00002850: 914e 6318 b1eb b586 b621 46c6 c37c b514  .Nc......!F..|..
-00002860: 0c00 e626 0a97 ac5c b8ff 160c 8022 62e0  ...&...\....."b.
-00002870: 76dc 3b23 0687 c5d2 0f0b 9dc6 b058 b823  v.;#.........X.#
-00002880: 5f43 db10 0be3 6159 8001 58cc 2621 2f0b  _C....aY..X.&!/.
-00002890: eebf 0503 b2e0 9b34 f7ce 88c1 61a1 35a9  .......4....a.5.
-000028a0: 8fc2 e8f2 58f5 c244 df1a 5b87 7858 976b  ....X..D..[.xX.k
-000028b0: 1308 1b71 06cd 9621 5b4f 3736 dace 1ab4  ...q...![O76....
-000028c0: e0f2 cb6b 45f8 67d4 e212 f223 8d1f 22d0  ...kE.g....#..".
-000028d0: 93a8 efb8 c0c3 d641 4246 90da 92c1 20c0  .......ABF.... .
-000028e0: a2d6 5ebe 53db a43d 15c8 8154 b886 11fe  ..^.S..=...T....
-000028f0: 19b5 b854 3c89 dec8 51bd 5cdf 61eb 2015  ...T<...Q.\.a. .
-00002900: ae47 530c 022a f379 78e3 ec48 6c05 ddd8  .GS..*.yx..Hl...
-00002910: 2e7a 4654 fd26 7ce7 16fe 19b5 b88c 3c29  .zFT.&|.......<)
-00002920: e088 4ae0 888b 3d6c 1d64 c4c5 698a 4158  ..J...=l.d..i.AX
-00002930: 390b 2166 6cd2 9e0a 15bf 91a8 1c21 7f69  9.!fl........!.i
-00002940: 0697 8a27 011c 5105 1c71 ad87 ad83 54b8  ...'..Q..q....T.
-00002950: 364d 3108 a824 51c8 54c0 c626 eda9 50ed  6M1..$Q.T..&..P.
-00002960: 1b71 0523 fc33 6a71 a968 01e8 6183 8e40  .q.#.3jq.h..a..@
-00002970: 48e2 2ac3 a51e b60e 52e1 d234 c520 a012  H.*.....R..4. ..
-00002980: cfc4 2e6d 93f6 54a8 f48d d8ae be13 fe19  ...m..T.........
-00002990: b5b8 543c c9df 88ea df88 8b3b 6c1d a4c2  ..T<.......;l...
-000029a0: c568 8a41 76bf 1667 1442 eb62 04de 55f3  .h.Av..g.B.b..U.
-000029b0: 1ddb 0ec2 50cc a8c5 a5e2 49f0 4654 f1f2  ....P.....I.FT..
-000029c0: e25d 63eb 2015 2e3f 530c b23b 129b 111b  .]c. ..?S..;....
-000029d0: 9bb4 af15 2a6f 63a6 a376 c23f a316 978a  ....*oc..v.?....
-000029e0: 2789 1b51 8d1b 7161 87ad 8354 84cc c520  '..Q..qa...T... 
-000029f0: d4b9 13a9 5e84 d0c5 08ac 15b1 da0a a96b  ....^..........k
-00002a00: 87a5 b8ba 543c 89dd 88aa dd58 e8bb f7f5  ....T<.....X....
-00002a10: 2e26 b8d1 a790 ddd1 408a 16a4 12cb 7545  .&......@.....uE
-00002a20: 485e 8cc0 5b21 4145 885e daa7 4325 f6a4  H^..[!AE.^..C%..
-00002a30: 7abb 3cf6 704a 1cda e95e dcd3 5071 6a67  z.<.pJ...^..Pqjg
-00002a40: 5cae 1edb 41a3 b9b7 9e88 fd08 bbef 996e  \...A..........n
-00002a50: d182 fa8e afbc c23f a316 9790 27d5 1b53  .......?....'..S
-00002a60: d51b 737d 87ad 43b3 c9ba 5c25 04d9 9150  ..s}..C...\%...P
-00002a70: 3c97 279b 5c33 6f31 1fd6 102b e49d edcd  <.'.\3o1...+....
-00002a80: aec2 d4e2 12f2 75ec 4b15 70cc d55d fc03  ......u.K.p..]..
-00002a90: 27bf 4201 6310 ee4d d377 14b0 edc2 aec9  '.B.c..M.w......
-00002aa0: 6841 46fc de49 f867 d4e2 32f2 a480 6390  hAF..I.g..2...c.
-00002ab0: 978b eb67 e3d0 a866 bf7d e8c0 56ed 4f18  ...g...f.}..V.O.
-00002ac0: bfbc 169f 62a3 ba01 d425 360f b93e d8d8  ....b....%6..>..
-00002ad0: e81e 1074 a9ee 8eae 54e5 4ef8 67d4 e202  ...t....T.N.g...
-00002ae0: f224 8663 d0a1 0048 cc32 681c 0464 5cae  .$.c...H.2h..d\.
-00002af0: ce32 68ec 01b1 631a ec7c 6997 f62d 5a90  .2h...c..|i..-Z.
-00002b00: 0fdf d485 7f46 2d2e 1f4f b2b8 7b0e b60a  .....F-..O..{...
-00002b10: 808f 9863 2057 07f9 1897 ab7c a0d1 f289  ...c W.....|....
-00002b20: f97d 38f6 4e01 6108 1490 58a7 4d6f fd2a  .}8.N.a...X.Mo.*
-00002b30: 442c 2e20 4f0a b97b c469 00f1 9b29 6c1c  D,. O..{.i...)l.
-00002b40: 0404 72f7 4f66 1834 22a0 4538 e107 7db6  ..r.Of.4".E8..}.
-00002b50: 837e 8661 08ce 30b1 4e9b ee7a 42c4 e212  .~.a..0.N..zB...
-00002b60: f2a4 9663 10aa 5042 5c16 62e3 2021 88ef  ...c..PB\.b. !..
-00002b70: 8b20 c520 c492 840b 5137 3c64 6b42 100b  . . ....Q7<dkB..
-00002b80: 3f9c b0c3 e8b1 9014 2e16 4f72 3906 2daa  ?.........Or9.-.
-00002b90: 7eda d597 9fcc aed1 6790 0ea4 a174 c082  ~.......g....t..
-00002ba0: 74e2 70c6 ef25 6cd6 be68 3004 e824 fc59  t.p..%l..h0..$.Y
-00002bb0: 9408 c8a8 c5a5 e349 36c7 a049 1d3a 6279  .......I6..I.:by
-00002bc0: 069f 413a c6c5 8a67 4c6c 6b87 33df a003  ..A:...gLlk.3...
-00002bd0: 5d73 2009 2eca 093f ac10 0119 b538 7412  ]s ....?.....8t.
-00002be0: 4ff2 b9cb 6316 9d48 3cdc 05f9 3bc4 0513  O...c..H<...;...
-00002bf0: 90aa 410b 7251 cf74 d94c dd88 90ad 09c1  ..A.rQ.t.L......
-00002c00: aae1 8f58 4440 462d 2e17 4fa2 3901 d58a  ...XD@F-..O.9...
-00002c10: 7287 6f57 d83a c805 1250 2e60 412e 5118  r.oW.:...P.`A.Q.
-00002c20: f3d9 64b3 dad9 8416 2372 f86c 1201 19b5  ..d.....#r.l....
-00002c30: b85c 3c49 e504 942e 72e1 bb14 b60e 7281  .\<I....r.....r.
-00002c40: 0494 0b58 fa79 c4d7 609b b5e7 8221 b806  ...X.y..`....!..
-00002c50: 7375 2302 326a 71b9 7892 c789 91c7 640d  su#.2jq.x.....d.
-00002c60: 1655 f3be 4ac6 3494 0eea 5c90 c6ea 8f8a  .U..J.4...\.....
-00002c70: 041d 93b5 a7e3 4863 7e52 b013 7d64 d4e2  ......Hc~R..}d..
-00002c80: d2f1 a48d 13a3 8d09 1d51 3bef 4b64 4c43  .........Q;.KdLC
-00002c90: e938 ba38 0e13 41c7 64ed e960 08d4 4ecc  .8.8..A.d..`..N.
-00002ca0: 6fad 441f 19b5 b874 3c29 e304 9425 ce29  o.D....t<)...%.)
-00002cb0: 7e34 8aad 8373 8a8b d514 83ec 9c5a f2a7  ~4...s.......Z..
-00002cc0: 7536 6bcf c5d1 c3fc 2e78 2702 326a 71b9  u6k......x'.2jq.
-00002cd0: 7812 c409 e849 67e7 e6c7 e9e8 3348 870b  x....Ig.....3H..
-00002ce0: d514 83ec 4abc 103b 140f d99a 10dc a1b8  ....J..;........
-00002cf0: 18b6 c3b0 aa8f 5a5c 3a9e c470 62c4 3099  ......Z\:..pb.0.
-00002d00: 53a2 768c f4fc f3fb 724c 43e7 1404 f574  S.v.....rLC....t
-00002d10: f8ad 8208 d9a2 05f7 a998 df4c 8980 8c5a  ...........L...Z
-00002d20: 5c3a 9e34 7172 4513 f3bf 9640 9fc1 da11  \:.4qrE....@....
-00002d30: 9a18 83fa dd4a d0e1 215b 1382 2b0e 577d  .....J..![..+.W}
-00002d40: 7618 7ded 9014 2e1d 4f9a 38b9 a289 f9fd  v.}.....O.8.....
-00002d50: 14fa 0cd2 119a 1883 ec1d c39c 3f93 b159  ............?..Y
-00002d60: fb75 c7d1 c4b1 d038 bc8f 8ca6 70e8 4c3d  .u.....8....p.L=
-00002d70: 69e2 2e8f d6c4 6466 b1ab bc46 9f21 3ad6  i.....df...F.!:.
-00002d80: c5de 31a0 c5d2 5970 0528 42b6 2604 6a67  ..1...Yp.(B.&.jg
-00002d90: 2afe b6cf 0874 5b3b 3485 4bc7 9332 9e1a  *....t[;4.K..2..
-00002da0: 65dc d311 0f23 d067 908e d0c7 1864 6796  e....#.g.....dg.
-00002db0: 80c3 23b6 2602 e1f0 8965 47d1 c321 295c  ..#.&....eG..!)\
-00002dc0: 389e e4f1 94ca 6371 d68e ad83 588c 3cbe  8.....cq....X.<.
-00002dd0: fa67 a18e 52be 118f 6b6c 7e3b b9d0 820b  .g..R...kl~;....
-00002de0: f394 df58 8980 8c5a 5c42 9e84 f254 0a65  ...X...Z\B...T.e
-00002df0: aec1 d6e8 33c8 89ab de14 83ec 6de7 44d4  ....3.......m.D.
-00002e00: 8f10 ca26 04eb 873f 0fb6 c3e8 eb87 a470  ...&...?.......p
-00002e10: e978 12ca ea8d 0afd bc8a 2e3d b28a de17  .x.........=....
-00002e20: ca98 866c ea68 b174 a2c4 f993 1cc1 4ac8  ...l.h.t......J.
-00002e30: 6693 0059 f163 2fd1 a37e 3944 7f95 6e0c  f..Y.c/..~9D..n.
-00002e40: c00a ded8 8077 1e2e f973 f1af bc7e 2ecf  .....w...s...~..
-00002e50: cde8 583c 752f 5728 dd51 c30b 1993 50fd  ..X<u/W(.Q....P.
-00002e60: de56 17fd cac5 5ce9 d2c7 aa55 af66 984f  .V....\....U.f.O
-00002e70: 2fea 859d 42bd eaa0 9ee2 06a3 a7aa 6acd  /...B.........j.
-00002e80: 0775 9d74 de9f 8bf6 f532 aaea 52bd b4d1  .u.t.....2..R...
-00002e90: bd83 b30a 2e55 ddd6 79d9 aad7 2a94 fd8f  .....U..y...*...
-00002ea0: 4a35 1cd3 4ba9 5ec9 98a9 1554 bd6a d496  J5..K.^....T.j..
-00002eb0: ea5d 95de 52df 96ea 7d94 faf3 21ea 5ed9  .]..R...}...!.^.
-00002ec0: b0ef 15dd ff1f 0000 ffff 0300 504b 0304  ............PK..
-00002ed0: 1400 0600 0800 0000 2100 5208 6b4e d304  ........!.R.kN..
-00002ee0: 0000 ec12 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
-00002ef0: 6b73 6865 6574 732f 7368 6565 7431 2e78  ksheets/sheet1.x
-00002f00: 6d6c ac98 4d93 a336 1086 efa9 ca7f a0b8  ml..M..6........
-00002f10: 2f18 7fdb 657b cb1e 1b33 876c a5b2 bbc9  /...e{...3.l....
-00002f20: 59c6 b24d 0610 0179 3ef6 d7a7 a546 181a  Y..M...y>....F..
-00002f30: 976b 53e1 3263 badf 6e89 472d 2169 f1f9  .kS.2c..n.G-!i..
-00002f40: 3d89 ad57 9e17 9148 97b6 e7f4 6c8b a7a1  =..W...H....l...
-00002f50: 3846 e979 697f ffe6 7f9a da56 2159 7a64  8F.yi......V!Yzd
-00002f60: b148 f9d2 fee0 85fd 79f5 eb2f 8b37 91bf  .H......y../.7..
-00002f70: 1417 cea5 0519 d262 695f a4cc e6ae 5b84  .......bi_....[.
-00002f80: 179e b0c2 1119 4fc1 7312 79c2 243c e667  ......O.s.y.$<.g
-00002f90: b7c8 72ce 8e3a 2889 dd7e af37 7613 16a5  ..r..:(..~.7v...
-00002fa0: 3666 98e7 3f93 439c 4e51 c8b7 22bc 263c  6f..?.C.NQ..".&<
-00002fb0: 9598 24e7 3193 d0ff e212 6585 c996 843f  ..$.1.....e....?
-00002fc0: 932e 61f9 cb35 fb14 8a24 8314 8728 8ee4  ..a..5...$...(..
-00002fd0: 874e 6a5b 4938 7f3e a722 6787 18de fbdd  .Nj[I8.>."g.....
-00002fe0: 1bb2 d0e4 d60f adf4 4914 e6a2 1027 e940  ........I....'.@
-00002ff0: 3a17 3bda 7ee7 993b 7321 d36a a139 fc9e  :.;.~..;s!.j.9..
-00003000: 5b00 9b7f 6109 b411 88bf 9967 bbab c531  [...a......g...1
-00003010: 8297 5323 62e5 fcb4 b4d7 de3c f046 caa1  ..S#b......<.F..
-00003020: 63fe 8cf8 5b51 fb6d fd10 22f9 1a32 d5cd  c...[Q.m.."..2..
-00003030: 198c 5ff5 f845 b18f d1a8 86eb 20c4 8b0a  .._..E...... ...
-00003040: 7e3e 2eed 9eea 018f 79a8 c059 0cfe bdf2  ~>......y..Y....
-00003050: 271e 83da 5723 fe8f 6ed8 9f42 c303 d5b0  '...W#..n..B....
-00003060: 5bb5 5cff 6d7a e1eb 4186 7739 b082 3f89  [.\.mz..A.w9..?.
-00003070: f8af e828 2f50 4dd0 9923 3fb1 6b2c ff10  ...(/PM..#?.k,..
-00003080: 6f01 8fce 1709 d6b1 33b2 adf0 5a48 9154  o.......3...ZH.T
-00003090: 3620 ab00 cf8f 1f5b 5e84 30b2 d043 a7af  6 .....[^.0..C..
-000030a0: 5a0e 450c cdc0 5f2b 8954 85c2 c0b0 7795  Z.E..._+.T....w.
-000030b0: 6530 1dda d65b d992 e70c fba3 c9d4 eb43  e0...[.........C
-000030c0: ea42 7e28 14d8 6f0c d7bd df32 c956 8b5c  .B~(..o....2.V.\
-000030d0: bc59 5069 90a7 c898 aa5b 6f0e 2ffc 5f3b  .YPi.....[o./._;
-000030e0: 063d 5259 362a cdd2 8646 a1c3 0520 7d5d  .=RY6*...F... }]
-000030f0: f516 ee2b 300a 4bc5 535b e135 15db b6a2  ...+0.K.S[.5....
-00003100: df54 ecda 8a41 53e1 b715 c3a6 62df 568c  .T...AS.....b.V.
-00003110: 9a8a a0ad 1857 0a17 b055 ecfa 9db0 5bab  .....W...U....[.
-00003120: 344b bbaf a911 261b f4d5 b94e 0857 a350  4K....&....N.W.P
-00003130: 25a2 8662 8b86 31a6 eb41 4110 8834 c047  %..b..1..AA..4.G
-00003140: c344 0710 9e7b 2a0e 6a86 068b 4137 2c54  .D...{*.j...A7,T
-00003150: 1ac3 828c fe06 7d8f 5818 85aa 3f5a 5de8  ......}.X...?Z].
-00003160: 2bb1 4ca7 ce6d 4c35 b69d 8935 1c7d 3420  +.L..mL5...5.}4 
-00003170: 1622 de53 7150 3334 b0c0 d4ec 607a ad55  .".SqP34....`z.U
-00003180: 1a83 850c d106 7d8f b018 c53d 2ce8 2bb1  ......}....=,.+.
-00003190: f461 4922 d562 622b 2c68 402c a416 f754  .aI".bb+,h@,...T
-000031a0: 1cd4 0c0d 2c6a 75fa ffab ce5a a531 5848  ....,ju....Z.1XH
-000031b0: 996f d0f7 088b 51dc c382 be12 cb70 ea90  .o....Q......p..
-000031c0: 6ada 99d8 0a0b 1a10 0b5d 72a8 38a8 191a  j........]r.8...
-000031d0: 58c6 dd60 5169 0c16 329e 1bf4 3dc2 6214  X..`Qi..2...=.b.
-000031e0: d582 8206 6431 f15a 1542 f53e 1a10 0599  ....d1.Z.B.>....
-000031f0: c37b 2a0e 6a86 068a 4937 2854 1a83 824c  .{*.j...I7(T...L
-00003200: e20d fa1e a130 8a0a 051a 10c5 78ec 90a9  .....0......x...
-00003210: b8a3 7a1f 0d88 c2a3 2ca8 3aa8 191a 2cd4  ..z.....,.:...,.
-00003220: 46a4 83d9 a2d2 2ced e9dd ef0c fa66 b5ef  F.....,......f..
-00003230: f794 7c67 8ca2 6281 06d8 dba8 f933 7206  ..|g..b......3r.
-00003240: 7441 a501 7a3f 05db 0caf fc32 91ef 3295  tA..z?.....2..2.
-00003250: 0735 4383 0674 b20b 1a2a 8da1 4197 54f4  .5C..t...*..A.T.
-00003260: 3da2 6114 f7d6 0ef4 9560 c60e 1df7 9d89  =.a......`......
-00003270: add6 8e32 00c1 10ee 7baa 0e6a 8606 17b5  ...2....{..j....
-00003280: cbec 028c ce63 c8d0 55b5 743e 4253 49ee  .....c..U.t>BSI.
-00003290: b129 9d25 9c89 d327 9f90 5d15 5dd1 3121  .).%...'..].].1!
-000032a0: 8887 ac67 fb96 3ea8 5b9a 80ba d9eb aea1  ...g..>.[.......
-000032b0: 826f a543 d7d7 d2f9 1010 c6cf f4ae 5e6f  .o.C..........^o
-000032c0: d9ca 2033 97e8 ae97 ea7d a32f a752 8b09  .. 3.....}./.R..
-000032d0: 0d08 aa5e a923 4c7d 0beb 75b4 87d5 794c  ...^.#L}..u...yL
-000032e0: d1d0 85b6 743e 6482 fbca 3a13 b494 4c06  ....t>d...:...L.
-000032f0: cea4 5529 34c4 2fdb 312b 0cdd cb56 dd30  ..U)4./.1+...V.0
-00003300: a515 d42d 4d2c 1d6d 67e1 d078 2b95 1616  ...-M,.mg..x+...
-00003310: 743e c462 24d5 aa5b 66ac b0cc 68b1 d008  t>.b$..[f...h...
-00003320: df44 94c5 d23a 0fd1 0075 d255 9dd6 63d1  .D...:...u.U..c.
-00003330: a4d2 cd6e 76e3 99ed ac79 ab5d cbe2 9796  ...nv....y.]....
-00003340: a13e 7437 2ab6 9bbd e306 2e12 706b 7043  .>t7*.......pkpC
-00003350: 8b16 7df3 8067 82ba 0649 e0f9 1f4f d019  ..}..g...I...O..
-00003360: 3bf3 df58 7e8e d2c2 8af9 491f d5e1 139e  ;..X~.....I.....
-00003370: e3f1 bee7 c06f 2932 7580 9f40 e683 9070  .....o)2u..@...p
-00003380: d037 4f17 b800 e270 5aeb 3900 fb24 8434  .7O....pZ.9..$.4
-00003390: 0fd0 1b95 f72b 97d7 cc12 7904 5700 fa4e  .....+....y.W..N
-000033a0: 6769 6722 9739 8b24 1cd2 c1fe 4380 23de  gig".9.$....C.#.
-000033b0: 6611 1cf0 c7b0 f2c3 d595 8ce0 eee3 66c9  f.............f.
-000033c0: e711 dc6f e4cf 47fd 426e 754f b5fa 1700  ...o..G.BnuO....
-000033d0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-000033e0: 0021 0020 e613 543e 0900 0056 3000 0018  .!. ..T>...V0...
-000033f0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00003400: 2f73 6865 6574 382e 786d 6cac 9bdb 6ee3  /sheet8.xml...n.
-00003410: 3812 86ef 1798 7730 743f b229 d98e 1dc4  8.....w0t?.)....
-00003420: 19c4 9dc8 6a60 77b0 d8de c3b5 622b 89a6  ....j`w.....b+..
-00003430: 6dcb 2b29 7d98 a75f 9255 a4c8 aa84 db83  m.+)}.._.U......
-00003440: 612e 1a49 b1aa 447f 2a92 3f69 f6cd 2fdf  a..I..D.*.?i../.
-00003450: 4ec7 c997 baeb 9bf6 bc49 443a 4b26 f579  N........ID:K&.y
-00003460: df1e 9af3 f326 f9d7 3f8b 9f57 c9a4 1faa  .....&..?..W....
-00003470: f3a1 3ab6 e77a 937c affb e497 db9f fe72  ..:..z.|.......r
-00003480: f3b5 ed3e f72f 753d 4c64 8673 bf49 5e86  ...>./u=Ld.s.I^.
-00003490: e172 3d9d f6fb 97fa 54f5 697b a9cf b2e5  .r=.....T.i{....
-000034a0: a9ed 4ed5 20ff ec9e a7fd a5ab ab83 0e3a  ..N. ..........:
-000034b0: 1da7 d96c b69c 9eaa e69c 4086 ebee 4772  ...l......@...Gr
-000034c0: b44f 4fcd bebe 6ff7 afa7 fa3c 4092 ae3e  .OO...o....<@..>
-000034d0: 5683 ec7f ffd2 5c7a 93ed b4ff 9174 a7aa  V.....\z.....t..
-000034e0: fbfc 7af9 79df 9e2e 32c5 6373 6c86 ef3a  ..z.y...2.csl..:
-000034f0: 6932 39ed af3f 3e9f dbae 7a3c cacf fd4d  i29..?>...z<...M
-00003500: ccab bdc9 adff 60e9 4fcd be6b fbf6 6948  ......`.O..k..iH
-00003510: 65ba 2974 947f e6f5 743d 9599 6e6f 3487  e.)t....t=..no4.
-00003520: bf77 1309 bbfe b53a c967 94ed 6fd5 2a99  .w.....:.g..o.*.
-00003530: dede 1c1a f9e1 d41b 9974 f5d3 26b9 13d7  .........t..&...
-00003540: e57c a61a 74cc bf9b fa6b effc 3e19 aac7  .|..t....k..>...
-00003550: 4ff5 b1de 0ff5 41be c264 32b4 97bf d64f  O.....A..d2....O
-00003560: c387 fa78 94c1 d922 99fc deb6 a74f fb4a  ...x...".....O.J
-00003570: 7d90 b57c c3f6 cf5f d5db 914e caa8 5ee8  }..|..._...N..^.
-00003580: 63db 7e56 e93f ca44 33d5 479d 5675 a4da  c.~V.?.D3.G.Vu..
-00003590: 0fcd 971a 527e cc54 51fc 57f7 4dfd 2e3b  ....R~.TQ.W.M..;
-000035a0: 36b5 3d73 7f37 bd2c 7411 c8cf fa58 f5f5  6.=s.7.,t....X..
-000035b0: 87f6 f89f e630 bcc8 aeca a71e eaa7 eaf5  .....0..........
-000035c0: 38fc a3fd 5ad6 cdf3 cb20 adcb 54f6 78ff  8...Z.... ..T.x.
-000035d0: da0f edc9 da24 79f5 02ae 0fdf efeb 7e2f  .....$y.......~/
-000035e0: dfbc ec5f 9aa9 27ef dba3 7c8c fc77 726a  ..._..'...|..wrj
-000035f0: 5405 cb17 577d 5359 f2d5 5c7e 287c 9248  T...W}SY..\~(|.H
-00003600: e7d9 e26a 2514 8c7e f8ae 40e4 badf 10ae  ...j%..~..@.....
-00003610: 7b7f 5f0d d5ed 4dd7 7e9d c84a 9479 fa4b  {._...M.~..J.y.K
-00003620: a5ea 5a5c cb4f fb47 3b26 7ba4 b26c 559a  ..Z\.O.G;&{..lU.
-00003630: 4d22 1f2a 3bdc 4ba0 5f6e 6737 d32f 92d1  M".*;.K._ng7./..
-00003640: 1e3d 3e70 0fe1 7bdc 738f ccf7 78e0 1eb9  .=>p..{.s...x...
-00003650: ef51 708f b9ef b1e3 1e0b dfa3 e41e 4beb  .Qp...........K.
-00003660: 3195 d82c bb2c 0abb 3b95 6693 649a 1a61  1..,.,..;.f.d..a
-00003670: b285 3697 eb15 e16a 3c54 89a8 5771 0f86  ..6....j<T..Wq..
-00003680: a54e 97cf d215 6148 fd0b 305c 697f 027c  .N....aH..0\i..|
-00003690: 479d 4bc7 e0a1 c8e3 a050 690c 0ad2 972d  G.K......Pi....-
-000036a0: b485 5018 0f8b 020c 8862 9e92 17fd 40fd  ..P......b....@.
-000036b0: 0b30 000a 5a37 d4b9 740c 1e0a 391a 238c  .0..Z7..t...9.#.
-000036c0: a83b 95c6 a020 55be 85b6 100a e3a1 4622  .;... U.......F"
-000036d0: 1d67 d006 5432 b160 584c acc1 5880 01b0  .g..T2.`XL..X...
-000036e0: 0832 ae77 d4bb 740c 1e17 3523 fdf9 99e6  .2.w..t...5#....
-000036f0: 4ea5 315c c83b da42 5b88 8bf1 b025 0206  N.1\.;.B[....%..
-00003700: 8031 bf62 a385 fa17 6000 1664 28ee a873  .1.b....`..d(..s
-00003710: e918 3c14 cb38 2854 1a83 82d4 f616 da42  ..<..8(T.......B
-00003720: 288c 8745 0106 44b1 6228 a87f 0106 4041  (..E..D.b(....@A
-00003730: 6699 1d75 2e1d 8387 e22a 0e0a 95c6 a018  f..u.....*......
-00003740: 676b 589b a02d 84c2 7858 1460 c021 92a5  gkX..-..xX.`.!..
-00003750: 6404 3d50 ff02 0c38 87d2 1142 bd4b c7e0  d.=P...8...B.K..
-00003760: b150 6a23 c208 5169 0c0b 52a2 5b68 0bb1  .Pj#..Qi..R.[h..
-00003770: 301e 9605 1890 c52a 2519 1fa8 7f01 0664  0......*%......d
-00003780: 4167 51ea 5d3a 068f c53a 0e0b 95c6 b020  AgQ.]:...:..... 
-00003790: 35ba 85b6 100b e361 5980 e15d 16d4 bf00  5......aY..]....
-000037a0: 03b2 a0d3 05f5 2e1d 83c7 42e9 c718 85a1  ..........B.....
-000037b0: f318 1a6b 5f17 6cb1 3184 c3ba 581e 6801  ...k_.l.1...X.h.
-000037c0: 202b 3e67 b088 022d 8884 2c6c 3be6 5fba   +>g...-..,l;._.
-000037d0: 161f 4a1c e57a 2740 eea1 fc22 6377 8bad  ..J..z'@..."cw..
-000037e0: 412a 462f 8e54 c082 33a9 600b ac4d 6a57  A*F/.T..3.`..MjW
-000037f0: 58b4 0015 f266 76cc bd74 2d3e 9448 9254  X....fv..t->.H.T
-00003800: 789a 948a 526c 0d42 61b2 1483 cc9c 4a95  x...Rl.Ba.....J.
-00003810: 3d93 a5e8 8f62 8c74 6167 bb60 1096 aec5  =....b.tag.`....
-00003820: 6712 499b 0a57 9c0a aa4e b135 c884 e953  g.I..W...N.5...S
-00003830: 0c02 2622 4fd9 7e87 2954 8c00 2a39 1b3e  ..&"O.~.)T..*9.>
-00003840: 4ca4 da6e a9bd abbb 7711 9164 aace 6377  L..n....w..d..cw
-00003850: 2f54 a862 6b90 0a15 90f7 1884 54e6 6cf5  /T.bk.......T.l.
-00003860: b549 c7e1 e32a d48c 8d1f 2651 dd0c 3e15  .I...*....&Q..>.
-00003870: a5d8 222c c102 941f 4e2a 54a6 626b 900a  ..",....N*T.bk..
-00003880: d592 f718 84e3 67c9 6b85 4614 1881 ba9d  ......g.k.F.....
-00003890: 6eed 6c27 c611 f49e 5c15 91f4 aace 636b  n.l'....\.....ck
-000038a0: 852a 566c 0d52 619a 1583 cc66 8689 569b  .*Vl.Ra....f..V.
-000038b0: 74ac 1557 b60a a215 77cc bf74 2d7e ad44  t..W....w..t-~.D
-000038c0: 92ae c268 d7f1 ec64 4e25 2cfa 04d9 1855  ...h...dN%,....U
-000038d0: f9d6 960f e371 482d c930 7db0 e947 4aae  .....qH-.0}..GJ.
-000038e0: a2cd d988 6292 d6cd e053 8a24 6a85 51b5  ....b....S.$j.Q.
-000038f0: 0e25 2a6e d127 48c9 e8cd 3729 b952 77bd  .%*n.'H...7).Rw.
-00003900: e213 0fd3 baf8 445c a4a8 f0b7 fd19 87d8  ......D\........
-00003910: 7b72 5744 d2bb 3a8f 1a62 0e26 aa7b d127  {rWD..:..b.&.{.'
-00003920: 88c9 48d1 3731 b92a 58ac 669c 13d3 c1f8  ..H.71.*X.f.....
-00003930: 48e0 b460 5311 53c2 b68b 74d9 ca22 4961  H..`S.S...t.."Ia
-00003940: 9d87 70a2 8a18 7d42 9cac cb5b 9cb0 1107  ..p...}B...[....
-00003950: 9d10 2979 c083 8db6 c30e 2dc8 89d6 13f3  ..)y......-.....
-00003960: 2f5d 8b7f 3419 491d 6746 1d8f f5b4 a01a  /]..4.I.gF......
-00003970: 197d 829c 8c46 7e93 932b 97c5 7296 2ed7  .}...F~..+..r...
-00003980: ee0f 3dbf a472 bbc0 e7e3 2024 cbca cef6  ..=..r.... $....
-00003990: ce0e 42d7 e243 8b75 a06b d4b3 038d 1dec  ..B..C.u.k......
-000039a0: fec0 c92e 3fda 75cf 76c5 3aa5 f378 c60f  ....?.u.v.:..x..
-000039b0: 77dd d35d baac ec98 7fe9 5a7c 3691 5474  w..]......Z|6.Tt
-000039c0: 0612 75f5 f669 3734 cae9 c07e 8d40 26af  ..u..i74...~.@&.
-000039d0: 0f18 bfd6 5f89 c079 3704 c98d a22a ae2c  ...._..y7....*.,
-000039e0: 9d51 15cd 420a b4c8 6dd4 1bf5 b863 fea5  .Q..B...m....c..
-000039f0: 6bf1 a944 52d1 1948 d477 a840 6390 8a71  k..DR..H.w.@c..q
-00003a00: b17b 50cc e850 f106 15fb 5680 2628 4c02  .{P..P....V.&(L.
-00003a10: 6044 771a d83a be86 d2b5 f88c 2269 6afd  `Dw..:......"ij.
-00003a20: 95d6 2601 4674 fb85 8d41 4620 6fdd ca01  ..&.Ft...AF o...
-00003a30: 8b65 3467 9543 430a 7c0e 560e 558f b617  .e4g.CC.|.V.U...
-00003a40: e35c e364 f0a9 44d2 d419 c8d9 77a8 4063  .\.d..D.....w.@c
-00003a50: 908a 7119 2b07 2c96 0a3d f0c3 278e 1c0b  ..q.+.,..=..'...
-00003a60: b420 1436 01d3 2794 6e06 1f4a 2449 9d81  . .6..'.n..J$I..
-00003a70: 3e05 2874 9f81 8d41 2810 ef96 0a58 108a  >.(t...A(....X..
-00003a80: 60a7 a036 e9b8 9463 048c 9f8c 1e90 b380  `..6...c........
-00003a90: d2b5 f854 2249 68fd 6db6 1940 7487 818d  ...T"Ih.m..@t...
-00003aa0: 412a 205e 5d2a 60b1 5496 6c00 d190 029f  A* ^]*`.T.l.....
-00003ab0: 83b5 92b1 2f1c 6940 693b c6a4 6024 c99c  ..../.i@i;..`$..
-00003ac0: 81fa 8462 6158 a031 88c5 b88c 2308 2c23  ...baX.1....#.,#
-00003ad0: 16fa fd01 3ed2 1d42 1882 d542 8fbb 5840  ....>..B...B..X@
-00003ae0: e95a bc6a c923 2964 9dc7 540b dd69 6163  .Z.j.#)d..T..iac
-00003af0: 088b 75b1 58d0 62b1 6414 0b0b 294c 0862  ..u.X.b.d...)L.b
-00003b00: a153 0b0b 285d 8b8f 2592 20ce 417e 42b5  .S..(]..%. .A~B.
-00003b10: 302c d018 c462 5c46 2c60 b158 d6e4 b8e8  0,...b\F,`.X....
-00003b20: 011f e954 0b5a cc20 a2cb 100b 285d 8b8f  ...T.Z. ....(]..
-00003b30: 2592 e4cd 4167 0216 bae1 c4c6 2016 8877  %...Ag...... ..w
-00003b40: e616 0cb2 cb10 2b16 1a51 9808 542c f4eb  ......+..Q..T,..
-00003b50: 16db 0bbb 38bb 169f 4a24 b19b 7b62 976e  ....8...J$..{b.n
-00003b60: 01b0 3588 c508 e2b1 5a3c b52b f794 ec52  ..5.....Z<.+...R
-00003b70: 030d 29f0 3958 2d73 2ae5 6c37 462e 4e0a  ..).9X-s*.l7F.N.
-00003b80: 9f4b 24b9 9b7b 7297 71f9 ff7a 1713 b8e5  .K$..{r.q..z....
-00003b90: 0241 b65c 1654 e1b2 9002 2d86 0b5d 8a58  .A.\.T....-..].X
-00003ba0: 40e9 5a7c 2e91 246e 0e6a 11b7 01ec 028c  @.Z|..$n.j......
-00003bb0: d192 efef 8e30 81cb c5d3 b822 cda8 9c63  .....0....."...c
-00003bc0: 2105 5a90 4bce 2ec2 986e a8bd 534e 2f4f  !.Z.K....n..SN/O
-00003bd0: d974 baf5 9d8b 5379 24f1 abf3 9835 4ad0  .t....Sy$....5J.
-00003be0: 2f1f b035 38be 98fa c5a0 7191 a287 3636  /..58.....q...66
-00003bf0: ab55 7a26 04e7 1d7a 6a63 0334 1152 eca5  .Uz&...zjc.4.R..
-00003c00: df3a be72 bfbe 22e9 e2dc d5c5 827e 2d81  .:.r.."......~-.
-00003c10: ad41 5e4c 1863 90e5 25c4 ccfd 61b3 364d  .A^L.c..%...a.6M
-00003c20: 5098 04b8 1767 b393 09d0 3b75 d2e5 d276  P....g....;u...v
-00003c30: 59b7 8eb5 e8d3 8ba4 9f73 d0a6 383a e9b6  Y........s..8:..
-00003c40: 025b 83f4 9880 c620 4b6f b60e d363 72da  .[..... Ko...cr.
-00003c50: 2440 7a6c cd33 019a 0f99 124b db65 dd3a  $@zl.3.....K.e.:
-00003c60: 16ba 4f2f 92cc ce8d cc76 4ea6 e989 2bfa  ..O/.....vN...+.
-00003c70: 0419 1ab5 fdd6 4922 c623 ce45 ba66 8b00  ......I".#.E.f..
-00003c80: d5ea 8509 0180 0b2a bc6d 8fc6 c5d1 49e1  .......*.m....I.
-00003c90: 8192 3797 e35c fc53 79d4 a416 383d d4cf  ..7..\.Sy...8=..
-00003ca0: 92d7 9903 0765 d6c5 4a07 b4d8 2592 e96f  .....e..J...%..o
-00003cb0: 1652 9810 a033 a7e5 6503 d4cb 98d3 f2f2  .R...3..e.......
-00003cc0: 5b69 79c1 4d6a b88b 7ca9 9eeb bf55 dd73  [iy.Mj..|....U.s
-00003cd0: 73ee 2747 79a3 5b5d 7a96 e3be 838b d2fa  s.'Gy.[]z.......
-00003ce0: 7779 d75b 5be5 e2f3 d80e f2ca b4f9 eb45  wy.[[..........E
-00003cf0: 5eb5 afe5 bdd7 592a 55cb 53db 0ee6 0ff9  ^.....Y*U.S.....
-00003d00: b955 de4f f5f0 7a99 b45d 232f 53eb dbf3  .U.O..z..]#/S...
-00003d10: 9be4 d276 4357 3583 bcee 2ced bfb7 b2e1  ...vCW5...,.....
-00003d20: 787f 69e4 55e9 a564 2fff 93c0 d0c8 3be4  x.i.U..d/.....;.
-00003d30: a3a5 bb6e e43d f1ee e341 e8ab d4f6 7f04  ...n.=...A......
-00003d40: dcfe 0f00 00ff ff03 0050 4b03 0414 0006  .........PK.....
-00003d50: 0008 0000 0021 00a0 ba2d d1ee 0700 0015  .....!...-......
-00003d60: 2700 0018 0000 0078 6c2f 776f 726b 7368  '......xl/worksh
-00003d70: 6565 7473 2f73 6865 6574 372e 786d 6cac  eets/sheet7.xml.
-00003d80: 9adf 73db 360c c7df 77b7 ffc1 a7f7 ca96  ..s.6...w.......
-00003d90: 64c7 712e ce2e 8e23 ab77 5b6f b7ee c7b3  d.q....#.w[o....
-00003da0: 62cb 8956 dbf2 2425 69fa d70f 2440 8a04  b..V..$%i...$@..
-00003db0: 36b5 bba9 0fa9 0d02 10f5 1148 7e45 f3fa  6..........H~E..
-00003dc0: 87cf c7c3 e8a5 a89b b23a 2d83 289c 04a3  .........:-.(...
-00003dd0: e2b4 ad76 e5e9 7119 fcf6 6bfa ee32 1835  ...v..q...k..2.5
-00003de0: 6d7e dae5 87ea 542c 83b7 a209 7eb8 f9fe  m~....T,....~...
-00003df0: bbeb d7aa fed4 3c15 453b 820c a766 193c  ......<.E;...f.<
-00003e00: b5ed f96a 3c6e b64f c531 6fc2 ea5c 9ca0  ...j<n.O.1o..\..
-00003e10: 655f d5c7 bc85 aff5 e3b8 39d7 45be d341  e_........9.E..A
-00003e20: c7c3 389e 4c2e c6c7 bc3c 0598 e1aa fe96  ..8.L....<......
-00003e30: 1cd5 7e5f 6e8b 75b5 7d3e 16a7 1693 d4c5  ..~_n.u.}>......
-00003e40: 216f a1ff cd53 796e 4cb6 e3f6 5bd2 1df3  !o...SynL...[...
-00003e50: fad3 f3f9 ddb6 3a9e 21c5 4379 28db 379d  ......:.!.Cy(.7.
-00003e60: 3418 1db7 57ef 1f4f 559d 3f1c e0be 3f47  4...W..OU.?...?G
-00003e70: d37c 6b72 eb2f 22fd b1dc d655 53ed db10  .|kr./"....US...
-00003e80: d28d b1a3 f29e 17e3 c518 32dd 5c6b 0e3f  ..........2.\k.?
-00003e90: d723 805d 7cc8 8f70 8dac fa33 9f07 e39b  .#.]|..p...3....
-00003ea0: eb5d 0937 a79e c8a8 2ef6 cbe0 36ba ca92  .].7........6...
-00003eb0: 5835 e898 dfcb e2b5 713e 8fda eafc 63b1  X5......q>....c.
-00003ec0: 6fef 8ac3 4139 27c1 e84b 551d 3f6e 73d5  o...A9'..KU.?ns.
-00003ed0: f105 3c51 fbf5 837a 1ae0 a48c ea01 3e54  ..<Q...z......>T
-00003ee0: d527 95ee fd6e 194c 549f 8a43 b155 2847  .'...n.LT..C.U(G
-00003ef0: 39fc f752 60ca f7f1 1c8a e02f dd17 f519  9..R`....../....
-00003f00: 3a32 b63d 713f 9b5e a5fa a1c3 bd3d e44d  :2.=q?.^.....=.M
-00003f10: 7157 1dfe 2877 ed13 5417 5c75 57ec f3e7  qW..(w..T.\uW...
-00003f20: 43fb 4bf5 9a15 e5e3 530b d68b 7016 8cb6  C.K.....S...p...
-00003f30: cf4d 5b1d ad0d 482b e057 bbb7 75d1 6ce1  .M[...H+.W..u.l.
-00003f40: 4943 ff42 8d60 5b1d e032 f077 742c 55c5  IC.B.`[..2.wt,U.
-00003f50: c283 ca3f ab2c c9e5 146e 8aae 1485 d378  ...?.,...n.....x
-00003f60: 36bf 8c62 48dd b46f 0a44 a2fb 8de1 baf7  6..bH..o.D......
-00003f70: ebbc cd6f aeeb ea75 0495 0779 9a73 aeea  ...o...u...y.s..
-00003f80: 38ba 8292 ffaf 1d83 1ea9 2c2b 9566 19c0  8.........,+.f..
-00003f90: 45a1 c30d 007d b999 5c8f 5f80 d196 3cee  E....}..\._...<.
-00003fa0: a447 e47b aca5 47ec 7bdc 4b8f c4f7 48a5  .G.{..G.{.K...H.
-00003fb0: c7d4 f7d8 488f 99ef 9149 8f0b eb31 066c  ....H....I...1.l
-00003fc0: 965d 3c08 bb5b 9566 19c4 9a1a 63b2 c236  .]<..[.f....c..6
-00003fd0: 97eb 9c71 351e 509c fa51 acd1 70a1 d3cd  ...q5.P..Q..p...
-00003fe0: 2621 cb78 cffd 5334 ccb5 7f77 a33a d786  &!.x..S4...w.:..
-00003ff0: 3b67 8ec1 4301 636f 8032 ba55 6914 8aae  ;g..C.co.2.Ui...
-00004000: 8c92 4bff 7e57 e8d2 47c4 7858 2268 4022  ..K.~W..G.xX"h@"
-00004010: f134 5cb0 aae2 fe29 1a90 082b b00d 77ce  .4\....)...+..w.
-00004020: 1c83 4704 06e5 1044 541a 4684 f57f 852e  ..G....DT.F.....
-00004030: 7d44 8c87 2582 0624 92cc 0411 ee9f a201  }D..%..$........
-00004040: 8944 aca2 36dc 3b73 0c1e 1235 27fd ffb9  .D..6.;s...5'...
-00004050: e656 a531 e385 8dee 15b6 f5b1 301e 9605  .V.1........0...
-00004060: 1a90 4534 9985 2ce5 3d0f 48d1 4030 787d  ..E4..,.=.H.@0x}
-00004070: 70ef cc31 7830 2e86 81a1 d218 186c 225b  p..1x0.......l"[
-00004080: 615b 1f0c e361 61a0 0161 2c92 904d 36f7  a[...aa..a,..M6.
-00004090: dc3f 4503 b2e0 332d 77ce 1c83 8742 adb2  .?E...3-w....B..
-000040a0: 03d4 854a 6350 b089 6c85 6d7d 288c 8745  ...JcP..l.m}(..E
-000040b0: 8106 4431 5f84 0cee 3df7 4fd1 8028 98f3  ..D1_...=.O..(..
-000040c0: 863b 678e c143 a154 e700 2854 1a83 823d  .;g..C.T..(T...=
-000040d0: c315 b6f5 a130 1e16 051a 10c5 9483 e0de  .....0..........
-000040e0: 291a 687c b0d5 973b 678e c103 b118 0684  ).h|...;g.......
-000040f0: 4ae3 4f9f 5326 4c56 e8d2 c7c3 7858 1e68  J.O.S&LV....xX.h
-00004100: a005 2511 3306 f74f d180 44d8 ecbd e1ce  ..%.3..O..D.....
-00004110: 9963 f088 2815 3944 6de8 3c8c 0997 1de4  .c..(.9Dm.<.....
-00004120: d307 c5ba 582a 64a1 5525 09d9 18bc 1711  ....X*d.U%......
-00004130: 2959 100c 5be8 37c2 3d73 2d3e 9a61 54ec  )Y..[.7.=s->.aT.
-00004140: 6d84 d28f a418 2f14 6aed 8562 b463 0705  m...../.j..b.c..
-00004150: 2d04 652e a611 9bd4 44a4 6441 286c f06e  -.e.....D.dA(l.n
-00004160: 847b e65a 7c28 03c9 d3c8 d3a7 a252 beae  .{.Z|(.......R..
-00004170: 5029 c14c bd87 a044 250b 4189 85fe 1011  P).L...D%.A.....
-00004180: 2959 100a 7b2d d808 f7cc b5f8 5006 12aa  )Y..{-......P...
-00004190: ea65 b313 edac 432b 6aed ad14 a31b d5bb  .e....C+j.......
-000041a0: 9278 1372 156b 348f 8588 b717 e8aa c613  .x.r.k4.........
-000041b0: ad7c 9211 fe99 6bf1 090d 245c 23a3 5cf5  .|....k...$\#.\.
-000041c0: 0d32 99b4 a2d6 5e42 42b5 5210 49b5 584e  .2....^BB.R.I.XN
-000041d0: 3042 b752 04ad 456c 406f 6c27 0cc5 ccb5  0B.R..El@ol'....
-000041e0: f854 948c 1b60 618e 500e d20c c3d5 2bb5  .T...`a.P.....+.
-000041f0: f652 e102 734d 4144 6511 b279 f4de 26ed  .R..sMADe..y..&.
-00004200: 6ac5 53b0 6234 0909 eb66 f0a9 0c24 6223  j.S.b4...f...$b#
-00004210: 57c5 465c c652 6b2f 1521 6429 88d6 e859  W.F\.Rk/.!d)...Y
-00004220: 28b6 1284 94a5 08aa 15b1 6d20 d4ac ed96  (.........m ....
-00004230: da16 72b7 05a2 81f4 acce b30c 2eff 7163  ..r...........qc
-00004240: 801a 412c d81d 17f6 e0ef ac4b 37ef a2ec  ..A,.......K7...
-00004250: 8475 540f ca30 e1af c222 2425 0bac 322a  .uT..0..."$%..2*
-00004260: 2416 c582 1917 766e cfdc 143e 9681 b46d  $.....vn...>...m
-00004270: 8492 11fe da3b 179b 04e4 d34b 07d3 743d  .....;.....K..t=
-00004280: 5f53 10d1 1105 c3fd 53e3 4f68 c4ec c203  _S......S.Oh....
-00004290: 32db 2b51 3103 a9dd 08b5 a38b 662a d626  2.+Q1.......f*.&
-000042a0: f4e9 4563 5cba c241 8b2d 9c29 7f31 a42b  ..Ec\..A.-.).1.+
-000042b0: 7734 53b2 50e1 4462 45e2 d7c8 dc14 5ee1  w4S.P.DbE.....^.
-000042c0: c403 095f 9d47 8d27 a770 f85e 0af9 f4d1  ..._.G.'.p.^....
-000042d0: b12e 960e 594c e184 d364 e2fe e395 2412  ....YL...d....$.
-000042e0: a426 0156 52c2 3758 4440 e65a 7c56 0329  .&.VR.7XD@.Z|V.)
-000042f0: e118 65ab 5749 7c0d 279f 5e56 98c6 1964  ..e.WI|.'.^V...d
-00004300: 1464 594d f85b 82cd 6a97 2b13 4274 f814  .dYM.[..j.+.Bt..
-00004310: 2402 32d7 e2d3 196a c716 452f cecc 7cb9  $.2....j..E/..|.
-00004320: 8ab1 b117 8b71 e94a 082d 8465 165e 0a2c  .....q.J.-.e.^.,
-00004330: 3c24 a5eb 9899 5914 0d0f c86c c7f8 f413  <$....Y....l....
-00004340: 0f24 8a75 1eb3 60f1 6d07 6aec c582 1ad6  .$.u..`.m.j.....
-00004350: ad16 b4d8 7967 2eb0 f090 94ae 63e6 1dfe  ....yg......c...
-00004360: 0265 bb61 359f 6bf1 ab65 2025 1ca3 2cf5  .e.a5.k..e %..,.
-00004370: c612 7fb7 249f 5e3a 98c6 a583 164b e792  ....$.^:.....K..
-00004380: 4b3f 9bb5 1b4b 1442 6b96 d8ef e7d7 c8dc  K?...K.Bk.......
-00004390: 143e 9d81 14b1 fea5 ca9f 95a7 5c17 934f  .>..........\..O
-000043a0: 2f1d 54ad 2e1d b458 3a13 4187 87a4 741d  /.T....X:.A...t.
-000043b0: 33a4 44ed f080 cc76 4c0c a981 9471 8cb2  3.D....vL....q..
-000043c0: d3ab 1df1 1b11 faf4 d231 2edd 8483 966e  .........1.....n
-000043d0: 6409 3a3c 24a5 be18 3a5c 2153 b323 055d  d.:<$...:\!S.#.]
-000043e0: 8b5f 3b03 2964 fdfb 2cab 1d31 1d1b 85fa  ._;.)d..,..1....
-000043f0: ef42 99d2 b8b5 c384 b2ac 1dae 7b53 4a62  .B..........{SJb
-00004400: e8f0 1d60 718d ccb5 f874 0612 cab1 11ca  ...`q....t......
-00004410: 5aec 8b19 c7c8 d31e 2e42 2253 ca4e 070a  Z........B"S.N..
-00004420: 6d23 54b2 09a1 1987 ff5e 42cd 6ed5 3829  m#T......^B.n.8)
-00004430: 7c2e 03a9 e4d8 a864 cd45 8ca6 afeb 634a  |......d.E....cJ
-00004440: e0d6 8ba7 8fe5 8eb0 8848 c962 9629 bef9  .........H.b.)..
-00004450: 2902 32d7 e261 4906 92c7 3a8f 7ddd e462  ).2..aI...:.}..b
-00004460: 8f5a fb26 19eb 6227 19b2 d872 89f9 8fd1  .Z.&..b'...r....
-00004470: 2224 3521 542e 9c8b 0dd0 6fa3 4cbd 675e  "$5!T.....o.L.g^
-00004480: 6bd2 55bc cf6b 2089 9c18 89ac cb88 2f59  k.U..k ......./Y
-00004490: d4da cb4b 8863 0a32 bcf8 efd4 dc3f 35fe  ...K.c.2.....?5.
-000044a0: a48c c56f d526 40f5 3061 3dcc 6c0f 756b  ...o.&@.0a=.l.uk
-000044b0: 375f f9b0 0652 cc70 8c47 ed97 d25e 069f  7_...R.p.G...^..
-000044c0: a3a9 b517 9690 cc14 d4cd 45fc 8729 9bd5  ..........E..)..
-000044d0: aa1f 1342 bcb8 fab1 019a 085b fdd5 4924  ...B.......[..I$
-000044e0: 750b 0bbd 11e2 ec38 202f 3c18 8447 6bce  u......8 /<..Gk.
-000044f0: f963 f153 5e3f 96a7 6674 8003 4aea 0c0f  .c.S^?..ft..J...
-00004500: ac17 359e fbd1 9fe1 e892 b682 a278 a85a  ..5..........x.Z
-00004510: 3801 64be 3dc1 49b1 024e d44c 4250 b6fb  8.d.=.I..N.LBP..
-00004520: aa6a cd17 b809 95f7 63d1 3e9f 4755 5dc2  .j......c.>.GU].
-00004530: d920 7df8 6b19 9cab baad f3b2 85d3 3b60  . }.k.........;`
-00004540: ff52 41c3 617d 2ee1 e4cf 054c 0d70 c6ad  .RA.a}.....L.p..
-00004550: 2de1 4854 67a9 af4a 38f6 54bf df45 fa64  -.HTg..J8.T..E.d
-00004560: 903d d076 f337 0000 00ff ff03 0050 4b03  .=.v.7.......PK.
-00004570: 0414 0006 0008 0000 0021 0054 35ba 6999  .........!.T5.i.
-00004580: 0600 00ff 1d00 0018 0000 0078 6c2f 776f  ...........xl/wo
-00004590: 726b 7368 6565 7473 2f73 6865 6574 362e  rksheets/sheet6.
-000045a0: 786d 6cac 995b 6fa3 3814 c7df 57da ef80  xml..[o.8...W...
-000045b0: 781f 08e4 d644 4d47 4d93 864a b3a3 d5ce  x....DMGM..J....
-000045c0: 5e9e 2971 1ab6 1067 81de e6d3 ef31 c736  ^.)q...g.....1.6
-000045d0: f671 8466 b5f4 6126 9c1b e6e7 0b7f eceb  .q.f..a&........
-000045e0: cfef 65e1 bdb2 aace f969 e547 c1c8 f7d8  ..e......i.G....
-000045f0: 29e3 fbfc f4b4 f2ff f8fd fed3 95ef d54d  )..............M
-00004600: 7ada a705 3fb1 95ff c16a fff3 cdcf 3f5d  z...?....j....?]
-00004610: bff1 eab9 3e32 d678 50e1 54af fc63 d39c  ....>2.xP.T..c..
-00004620: 9761 5867 4756 a675 c0cf ec04 9e03 afca  .aXgGV.u........
-00004630: b481 cbea 29ac cf15 4bf7 6d52 5984 f168  ....)...K.mRY..h
-00004640: 340b cb34 3ff9 5861 59fd 480d 7e38 e419  4..4?.XaY.H.~8..
-00004650: dbf0 eca5 64a7 068b 54ac 481b 687f 7dcc  ....d...T.H.h.}.
-00004660: cfb5 aa56 663f 52ae 4cab e797 f3a7 8c97  ...Vf?R.L.......
-00004670: 6728 f198 1779 f3d1 16f5 bd32 5b3e 3c9d  g(...y.....2[><.
-00004680: 7895 3e16 f0dc efd1 24cd 54ed f6c2 295f  x.>.....$.T...)_
-00004690: e659 c56b 7e68 0228 1762 43dd 675e 848b  .Y.k~h.(.bC.g^..
-000046a0: 102a dd5c b71c 7ead 3c80 cdbe a625 dc23  .*.\..~.<....%.#
-000046b0: e17f a733 3fbc b9de e7f0 70a2 47bc 8a1d  ...3?.....p.G...
-000046c0: 56fe 6db4 4ce2 b170 b439 7fe6 ecad 367e  V.m.L..p.9....6~
-000046d0: 7b0d 3f7f 6187 e68e 1585 081e fbde 77ce  {.?.a.........w.
-000046e0: cb6f 592a 1abe 801e d597 5f45 6f40 9030  .oY*......_Eo@.0
-000046f0: 8a0e 7ce4 fc59 947b d8af fc91 6813 2b58  ..|..Y.{....h.+X
-00004700: 2650 7a29 fcf7 cab0 e483 1803 ffb4 4d81  &Pz)..........M.
-00004710: 9fd0 8c50 b7c3 fcad da74 df76 393c d963  ...P.....t.v9<.c
-00004720: 5ab3 3b5e fc95 ef9b 238c 2db8 e79e 1dd2  Z.;^....#.-.....
-00004730: 97a2 f98d bf25 2c7f 3a36 609d 0553 dfcb  .....%,.:6`..S..
-00004740: 5eea 8697 da06 9c05 eee5 fe63 c3ea 0cfa  ^..........c....
-00004750: 195a 17c4 e2ce 192f e036 f0af 57e6 62bc  .Z...../.6..W.b.
-00004760: 4237 a5ef a2ca f86a 028f 24ef 1405 9378  B7.....j..$....x
-00004770: 3abf 8a62 285d 371f 0243 8b2f c4f4 b6f5  :..b(]7..C./....
-00004780: 9bb4 496f ae2b fee6 c1b8 833a f539 15a3  ..Io.+.....:.9..
-00004790: 385a c2c3 fed7 8641 8b44 95b5 28b3 f2e1  8Z.....A.D..(...
-000047a0: a6d0 e01a 70be de8c aec3 5760 94c9 883b  ....p.....W`...;
-000047b0: 3722 b223 366e 446c 476c dd88 b11d 71ef  7".#6nDlGl....q.
-000047c0: 464c ec88 9d1b 31b5 2312 3762 a623 42c0  FL....1.#.7b.#B.
-000047d0: a6d9 c583 b0bb 1565 567e dc52 234f bc46  .......eV~.R#O.F
-000047e0: 9fc9 754e b8aa 08c1 9c12 45df acad 1c4d  ..uN......E....M
-000047f0: a641 f71c 6daf 6d55 ae18 5ea2 1bef d130  .A..m.mU..^....0
-00004800: c7a6 906a 3b1a 9d18 068b 0b4c c301 c6d4  ...j;......L....
-00004810: ad28 a3b8 907e 5ea3 af8f 8b8a b8c4 057d  .(...~^........}
-00004820: 92cb 551c 9027 ddaa 5ccd 050d c825 5a90  ..U..'..\....%Z.
-00004830: 1145 a313 c360 7181 793a 0417 5146 70e9  .E...`q.y:..QFp.
-00004840: e65a 4c86 f01a 43fa f0a8 884b 78d0 27f1  .ZL...C....Kx.'.
-00004850: 448b 80c0 dfaa 5c8d 070d 8887 8cb1 1d0d  D.....\.........
-00004860: 4e0c 8345 47ac 58ff 7f25 ba15 65d4 a821  N..EG.X..%..e..!
-00004870: 737f 8dbe 3e2c 2ae2 1216 f449 2cf1 c419  s...>,*....I,...
-00004880: 352a 5763 4103 6221 3db4 a3c1 8961 b0b0  5*WcA.b!=....a..
-00004890: cc86 c122 ca28 2c74 b4a0 af0f 8b8a b884  ...".(,t........
-000048a0: 057d 0acb 2820 d5b7 2a57 6341 835c 64c8  .}..( ..*WcA.\d.
-000048b0: 5ca2 c189 61b0 b0cc 87c1 22ca d873 694a  \...a....."..siJ
-000048c0: 9760 0ce9 a3a3 222e d141 9f5a 82a3 603c  .`...."..A.Z..`<
-000048d0: 32fe e8ba a30a 6954 6840 54f4 4546 8313  2.....iTh@T.EF..
-000048e0: c360 a112 1a66 8089 25ca a811 4426 f91a  .`...f..%...D&..
-000048f0: 7d7d 8c54 c425 46e8 ebd6 1b3a 8254 aec6  }}.T.%F....:.T..
-00004900: 8206 c442 5763 1a9c 1806 0bcb 6218 2ca2  ...BWc......b.,.
-00004910: 8cc2 42de cd6b f4f5 6151 1197 b0a0 4f62  ..B..k..aQ....Ob
-00004920: 99ce 82d9 c2fc 23d2 4815 d28c d020 5f59  ......#.H.... _Y
-00004930: f455 4ea3 13c3 6041 12d2 7588 c1d3 d651  .UN...`A..u....Q
-00004940: 9848 97ad a5b3 8f93 0eb9 044a 3ad5 249b  .H.........J:.$.
-00004950: 0551 1f29 5d4a a392 16c9 8a74 e2ce 894f  .Q.)]J.....t...O
-00004960: 4c8b 4d6b 1835 7d1b a104 b55e f157 7687  L.Mk.5}....^.Wv.
-00004970: af65 4c2f 34a5 642f 4243 a79a 7513 471c  .eL/4.d/BC..u.G.
-00004980: ea1b 749c 3005 3939 98d4 cd54 7862 16b0  ..t.0.99...Txb..
-00004990: 310d 249c 23a5 9c3b 2534 a542 51c6 f462  1.$.#..;%4.BQ..b
-000049a0: ea93 d032 5f62 9a91 4578 abcb 7790 4c0d  ...2_b..Ex..w.L.
-000049b0: 4d5a b373 c213 d362 431a 4845 8b8f 62bd  MZ.s...bC.HE..b.
-000049c0: 4045 6421 584b 6f2f 9e3e 252d f325 9ef1  @Ed!XKo/.>%-.%..
-000049d0: b87f 91d2 77eb 6899 ca3a 26af de9d 139f  ....w.h..:&.....
-000049e0: 9816 1bd7 40e2 3a52 eaba 9d33 540b 486f  ....@.:R...3T.Ho
-000049f0: 2f2e 2a78 3732 4932 9a3b 0249 17ed a898  /.*x72I2.;.I....
-00004a00: 823a 7666 9a23 a9cd 0a36 15a1 2a07 78f7  .:vf.#...6..*.x.
-00004a10: 47a8 4ef1 1b35 72e6 98d2 aedd 3ca4 5fa9  G.N..5r.....<._.
-00004a20: b2c0 b4dd c910 9f9a 1b69 412a f128 185b  .........iA*.(.[
-00004a30: 6b36 7945 6c9d fc7b 6991 32d2 9968 8ebe  k6yEl..{i.2..h..
-00004a40: 362b d88c 0652 d891 29b1 23b2 fdb1 96de  6+...R..).#.....
-00004a50: de91 43c5 ef46 2649 4693 8050 ddea a2dd  ..C..F&IF..P....
-00004a60: c831 c575 e4cc 2747 5e9b 156c 2a03 09ec  .1.u..'G^..l*...
-00004a70: 0855 e955 bba5 40bf c7a4 13c4 87de 3622  .U.U..@.......6"
-00004a80: afb9 3b1d 72f1 1d86 c5e1 7d2c bcf3 8024  ..;.r.....},...$
-00004a90: 6f75 72c7 4766 446d 0689 df39 f189 69b1  our.GfDm...9..i.
-00004aa0: f90c a4aa 2394 a7c8 877e 9849 672f 1fcc  ....#....~.Ig/..
-00004ab0: 5fe0 1e0f dd51 43a7 e633 a6ca 5adf a003  _....QC..3..Z...
-00004ac0: 2453 1010 d58d 4e7c 625a 6c40 03e9 eb08  $S....N|bZl@....
-00004ad0: a529 0272 9423 3a7b 01a9 908b 0308 9d12  .).r.#:{........
-00004ae0: d022 a01f 7f5b 79f7 855e b7ee a505 c44d  ."...[y..^.....M
-00004af0: 5bd0 1942 ea76 9d0c 322c 16a1 7820 6ddd  [..B.v..2,..x m.
-00004b00: d659 f948 887e 9949 671f 211d 7271 0b51  .Y.H.~.Ig.!.rq.Q
-00004b10: 34b2 ddc2 c629 e610 d2d9 7a08 498b 2244  4....)....z.I."D
-00004b20: 56c2 9d93 9098 169b d040 7a3a 466d 8a84  V........@z:Fm..
-00004b30: 9ca5 597a 7b11 6181 6e18 6c64 921c 3971  ..Yz{.a.n.ld..9q
-00004b40: 30a7 ca50 57ed b860 11c5 85be b274 42db  0..PW..`.....tB.
-00004b50: 0da4 5c62 7bbb 796c f31a 6a47 1a35 ace4  ..\b{.yl..jG.5..
-00004b60: e5ec 49a3 b797 970a 510f bf89 d1a2 794d  ..I.....Q.....yM
-00004b70: ac8d 9011 dde9 97e1 c6bc 5305 70de c574  ..........S.p..t
-00004b80: dee9 0441 2f26 eb44 6279 c7dd 88b4 e90d  ...A/&.Dby......
-00004b90: a4b8 e1c0 4a4c 1949 8f8a 25e9 eda5 8705  ....JL.I..%.....
-00004ba0: ccd1 8616 4d8f 6ef8 6e75 d56e b4c9 14c9  ....M.n.nu.n....
-00004bb0: 8bee 1ee9 8496 173d 02b1 bdf4 f803 0fc1  .......=........
-00004bc0: f018 e99c 3eb1 5fd2 ea29 3fd5 5e01 4771  ....>._..)?.^.Gq
-00004bd0: e2bc 0ade b115 9e71 b5bf e190 aeb5 82f6  .......q........
-00004be0: 79e4 0d9c 76a9 ab23 9c89 32d0 8220 fe7c  y...v..#..2.. .|
-00004bf0: efc0 79a3 2ee0 2144 dd6f ac79 397b bcca  ..y...!D.o.y9{..
-00004c00: e11c ac3d e65c f967 5e35 559a 3770 5205  ...=.\.g^5U.7pR.
-00004c10: f6ef 1c1c c5e6 9cc3 29d7 0c16 2a38 cd6d  ........)...*8.m
-00004c20: 7238 fceb 2cd5 3287 03be ea61 1fb5 a777  r8..,.2....a...w
-00004c30: fae8 f6e6 5f00 0000 ffff 0300 504b 0304  ...._.......PK..
-00004c40: 1400 0600 0800 0000 2100 573a 6683 5806  ........!.W:f.X.
-00004c50: 0000 071d 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
-00004c60: 6b73 6865 6574 732f 7368 6565 7435 2e78  ksheets/sheet5.x
-00004c70: 6d6c ac99 5b6f a338 14c7 df57 daef 8078  ml..[o.8...W...x
-00004c80: 1f08 e4d2 246a 3a6a 9a0b 23cd 8e56 3b7b  ....$j:j..#..V;{
-00004c90: 79a6 c469 d881 380b f436 9f7e 8f39 b6b1  y..i..8..6.~.9..
-00004ca0: 8f5b 34ab 651e 3ac9 b961 7e3e 367f e2eb  .[4.e.:..a~>6...
-00004cb0: 8f2f 65e1 3db1 aace f979 e547 c1c8 f7d8  ./e.=....y.G....
-00004cc0: 39e3 87fc fcb0 f2ff f87d f761 ee7b 7593  9........}.a.{u.
-00004cd0: 9e0f 69c1 cf6c e5bf b2da ff78 f3f3 4fd7  ..i..l.....x..O.
-00004ce0: cfbc fa56 9f18 6b3c a870 ae57 fea9 692e  ...V..k<.p.W..i.
-00004cf0: cb30 acb3 132b d33a e017 7606 cf91 5765  .0...+.:..v...We
-00004d00: dac0 d7ea 21ac 2f15 4b0f 6d52 5984 f168  ....!./.K.mRY..h
-00004d10: 340b cb34 3ffb 5861 59fd 480d 7e3c e619  4..4?.XaY.H.~<..
-00004d20: dbf0 ecb1 64e7 068b 54ac 481b 187f 7dca  ....d...T.H...}.
-00004d30: 2fb5 aa56 663f 52ae 4cab 6f8f 970f 192f  /..Vf?R.L.o..../
-00004d40: 2f50 e23e 2ff2 e6b5 2dea 7b65 b6fc f470  /P.>/...-.{e...p
-00004d50: e655 7a5f c07d bf44 9334 53b5 db2f 4ef9  .Uz_.}.D.4S../N.
-00004d60: 32cf 2a5e f363 1340 b910 07ea def3 225c  2.*^.c.@......"\
-00004d70: 8450 e9e6 bae5 f06b e501 6cf6 252d e11a  .P.....k..l.%-..
-00004d80: 09ff 3b9d fae1 cdf5 2187 9b13 33e2 55ec  ..;.....!...3.U.
-00004d90: b8f2 6fa3 6512 8f85 a3cd f933 67cf b5f1  ..o.e......3g...
-00004da0: d96b f8e5 333b 3677 ac28 44f0 d8f7 be73  .k..3;6w.(D....s
-00004db0: 5e7e cd52 31f0 05cc a8fe fa45 cc06 0409  ^~.R1......E....
-00004dc0: a398 c07b cebf 8972 9f0e 2b7f 24c6 c40a  ...{...r..+.$...
-00004dd0: 9609 945e 0aff 3d31 2cb9 8fae a009 fe69  ...^..=1,......i
-00004de0: c722 3ec3 4042 3d12 f3b3 1ad5 ae9d 74b8  .">.@B=.......t.
-00004df0: b7fb b466 77bc f82b 3f34 27e8 2eb8 ea81  ...fw..+?4'.....
-00004e00: 1dd3 c7a2 f98d 3f27 2c7f 3835 609d 0553  ......?',.85`..S
-00004e10: dfcb 1eeb 8697 da06 a405 f0e5 e175 c3ea  .............u..
-00004e20: 0c66 1ac6 17c4 e2ca 192f e032 f0d7 2b73  .f......./.2..+s
-00004e30: d1b1 3051 e98b a832 9e4f e0a6 e495 a260  ..0Q...2.O.....`
-00004e40: 124f afe6 510c a5eb e655 8068 0186 98de  .O..Q....U.h....
-00004e50: 8e7e 9336 e9cd 75c5 9f3d e83c a853 5f52  .~.6..u..=.<.S_R
-00004e60: d1c7 d112 5afe bf0e 0c46 24aa ac45 9995  ....Z....F$..E..
-00004e70: 0f17 8501 d700 f4e9 6674 1d3e 01a3 4c46  ........ft.>..LF
-00004e80: dcb9 1191 1db1 7123 623b 62eb 468c ed88  ......q#b;b.F...
-00004e90: 9d1b 31b1 23f6 6ec4 d48e 48dc 8899 8e08  ..1.#.n...H.....
-00004ea0: 019b 6617 0fc2 ee56 9459 f971 4b8d 3059  ..f....V.Y.qK.0Y
-00004eb0: a3cf e47a 45b8 aa08 d122 622a 3668 98b5  ...zE...."b*6h..
-00004ec0: e526 b380 dcff 96c6 efd0 70d5 c693 e27b  .&........p....{
-00004ed0: 1a9c 1806 0b05 acbd 01da e856 9451 28c8  ...........V.Q(.
-00004ee0: e4af d1d7 8742 4568 1468 9028 a280 4cf4  .....BEh.h.(..L.
-00004ef0: 96c6 efd0 8028 22da 3834 3a31 0c16 0b58  .....(".84:1...X
-00004f00: 8e43 b010 6514 0bd2 e66b f4f5 b150 119a  .C..e....k...P..
-00004f10: 051a 90c5 741a 9046 dbd2 f81d 1a24 0b32  ....t..F.....$.2
-00004f20: 177b 1a9d 1806 8b85 d886 feff f672 2bca  .{...........r+.
-00004f30: 2816 645e d6e8 eb63 a122 340b 34c8 be98  (.d^...c."4.4...
-00004f40: 3a7d 41e3 7768 4016 a489 f634 3831 0c16  :}A.wh@....481..
-00004f50: 8ad9 3028 4419 8582 8c65 8dbe 3e14 2a42  ..0(D....e..>.*B
-00004f60: ecd0 74ff 451f 5289 c6dd 9ed7 6e2b 5b95  ..t.E.R.....n+[.
-00004f70: a920 eed0 201b 846c b234 3831 0c16 14f1  . .. ..l.481....
-00004f80: 801d a03f 4419 0585 0c7c 8dbe 3e28 2ae2  ...?D....|..>(*.
-00004f90: 2d28 e853 50e8 0349 656a 2868 4028 64d1  -(.SP..Iej(h@(d.
-00004fa0: ee69 7062 182c 2842 7a0e 0045 9451 50c8  .ipb.,(Bz..E.QP.
-00004fb0: c6be 465f 1f14 15f1 1614 f4bd 0745 656a  ..F_.........Eej
-00004fc0: 2868 909d b220 ad42 a313 c360 5159 0c43  (h... .B...`QY.C
-00004fd0: 4594 5154 e6f6 58d6 e8eb a3a2 22de a282  E.QT..X....."...
-00004fe0: 3e45 856e b02a 5353 4103 5289 49f4 9e46  >E.n.*SSA.R.I..F
-00004ff0: 2786 c1a2 22b4 e510 cdd2 d651 5cc8 1cad  '..."......Q\...
-00005000: a5b3 0f8c 0ed1 9bac b420 8ff1 2420 45b7  ......... ..$ E.
-00005010: 4ec6 4e5a 64a3 9075 bc77 e213 d362 4319  N.NZd..u.w...bC.
-00005020: 46d5 de46 2805 a534 238a 762d bdbd 5494  F..F(..4#.v-..T.
-00005030: 96ec a8a0 453e 8747 ceb3 4717 d57d 222d  ....E>.G..G..}"-
-00005040: 4885 ae1e 273c 312d 3694 81e4 6a84 1a70  H...'<1-6...j..p
-00005050: fea6 5e95 4ee8 56fd 2240 16d9 9d0e e998  ..^.N.V."@......
-00005060: 6045 984e b1ac e260 4e76 abad 93b2 9316  `E.N...`Nv......
-00005070: b859 9142 2eb1 77e2 13d3 6253 1948 b98a  .Y.B..w...bS.H..
-00005080: b74f d857 900a 95ae d2d9 4b05 f317 edab  .O.W......K.....
-00005090: 5eab e365 92a6 7245 9e27 5b5d b56b 152c  ^..e..rE.'[].k.,
-000050a0: 22a9 4454 aa38 0989 69b1 b10c 2462 2314  ".DT.8..i...$b#.
-000050b0: 8688 85aa 58e9 ecc5 82f9 2616 b448 2ce3  ....X.....&..H,.
-000050c0: 806e 9d5b 5db5 c322 53b0 5922 fa5c 7612  .n.[].."S.Y".\v.
-000050d0: 12d3 6263 1948 cf46 2812 110b 15b4 d2d9  ..bc.H.F(.......
-000050e0: 8b05 f34d 2c68 e9ba 85ac 89ad aeda 6191  ...M,h........a.
-000050f0: 2988 c5d9 6ee9 2512 b382 4d65 2069 1ba1  )...n.%...Me i..
-00005100: 4a44 2a54 db4a 672f 15cc 5fbc b533 6d64  JD*T.Jg/.._..3md
-00005110: be04 340d 16ce 7252 d91d 20b4 c8e5 44df  ..4...rR.. ...D.
-00005120: 81f4 8054 7c62 5a6c 4003 c9dc f6f7 28b5  ...T|bZl@.....(.
-00005130: c950 9d2b 9dbd 8050 71be 0308 9d1d 20a7  .P.+...Pq..... .
-00005140: 8354 7607 48a6 6007 39bf b4d0 f844 0f11  .Tv.H.`.9....D..
-00005150: 2ad8 8006 92bc 118a 47ec 20aa 79a5 b317  *.......G. .y...
-00005160: 10e6 bf03 089d 1ad0 c451 342a bb03 2453  .........Q4*..$S
-00005170: 1050 4c14 c45e 8fa8 6b21 a384 4d68 20f9  .PL..^..k!..Mh .
-00005180: 1ba1 9044 4254 ff4a 672f 21cc 7f87 103a  ...DBT.Jg/!....:
-00005190: 7b08 a9ec 8e90 4c91 849c 4546 1312 3d46  {.....L...EF..=F
-000051a0: da43 f140 4ab8 ada3 1619 55c2 d2d9 4748  .C.@J.....U...GH
-000051b0: 8768 7d23 2d12 4b14 cce8 6ba4 93b2 5329  .h}#-.K...k...S)
-000051c0: f291 4505 8e93 9098 16ab 71e2 81b4 705b  ..E.......q...p[
-000051d0: e75d 2ca8 6a7b b1a8 900e 0b5a f423 2b9a  .],.j{.....Z.#+.
-000051e0: 8fcc 7f0e 245a 6027 87a4 e48e f3e3 254d  ....$Z`'......%M
-000051f0: 4864 42fb d8b4 210d f553 aed2 c69d fc8d  HdB...!..S......
-00005200: e9e3 3dc6 985e 562a a463 6549 64f8 959f  ..=..^V*.ceId...
-00005210: 6ece baaa 5e59 d2a2 e8d0 bdc7 4948 4c8b  n...^Y......IHL.
-00005220: 4d67 208d 0c67 39a8 910d 3a54 13ca 985e  Mg ..g9...:T...^
-00005230: 3a8e 5496 497a 81d1 47bb 2eda c1b1 9532  :.T.Iz..G......2
-00005240: 7dfd 7612 c439 9418 bbd1 3a78 1484 8729  }.v..9....:x...)
-00005250: 97f4 81fd 9256 0ff9 b9f6 0a38 9212 a736  .....V.....8...6
-00005260: f0f4 abf0 a4a7 fd0c 8755 ad15 64d5 3d6f  .........U..d.=o
-00005270: e0cc 477d 3bc1 d920 831f ee47 015c e2c8  ..G};.. ...G.\..
-00005280: 79a3 bec0 6045 ddaf ac79 bc78 bcca e134  y...`E...y.x...4
-00005290: a83d ee5b f917 5e35 559a 3770 5e03 f6ef  .=.[..^5U.7p^...
-000052a0: 1c1c c5e6 92c3 59cf 0c36 4138 d56c 7238  ......Y..6A8.lr8
-000052b0: 04eb 2cd5 3287 83ae ead3 216a cfb0 f411  ..,.2.....!j....
-000052c0: e6cd bf00 0000 ffff 0300 504b 0304 1400  ..........PK....
-000052d0: 0600 0800 0000 2100 9893 84db cb03 0000  ......!.........
-000052e0: 390f 0000 0d00 0000 786c 2f73 7479 6c65  9.......xl/style
-000052f0: 732e 786d 6ccc 5759 6fdb 3810 7e2f b0ff  s.xml.WYo.8.~/..
-00005300: 41e0 bba2 c396 6a19 968a 388e 8002 dda2  A.....j...8.....
-00005310: 4052 a0af b444 d944 7918 149d 95bb d8ff  @R...D.Dy.......
-00005320: de21 25d9 4a73 2949 8ff5 8bc5 d1f0 9b6f  .!%.Js)I.......o
-00005330: 0ecd 908b 770d 67ce 0d51 3595 2245 c199  ....w.g..Q5."E..
-00005340: 8f1c 220a 5952 b149 d1e7 ebdc 9d21 a7d6  ..".YR.I.....!..
-00005350: 5894 9849 4152 7420 357a 97fd f566 51eb  X..IARt 5z...fQ.
-00005360: 0323 575b 42b4 0310 a24e d156 ebdd dcf3  .#W[B....N.V....
-00005370: ea62 4b38 aecf e48e 0878 5349 c5b1 86a5  .bK8.....xSI....
-00005380: da78 f54e 115c d666 1367 5ee8 fbb1 c731  .x.N.\.f.g^....1
-00005390: 15a8 4598 f362 0c08 c7ea eb7e e716 92ef  ..E..b.....~....
-000053a0: b0a6 6bca a83e 582c e4f0 62fe 7e23 a4c2  ..k..>X,..b.~#..
-000053b0: 6b06 549b 608a 0ba7 0962 15f6 16ac e88e  k.T.`....b......
-000053c0: 114e 0b25 6b59 e933 00f5 6455 d182 dce5  .N.%kY.3..dU....
-000053d0: 9a78 8987 8b13 12c0 be0c 2988 3c3f 6c1d  .x........).<?l.
-000053e0: cf16 9514 ba76 0ab9 173a 4513 4037 a4e7  .....v...:E.@7..
-000053f0: 5f85 fc47 e4e6 15e4 04b5 5ad9 a2fe e6dc  _..G......Z.....
-00005400: 6006 9200 79d9 a290 4c2a 4743 b0c1 572b  `...y...L*GC..W+
-00005410: 1198 9356 e302 33ba 56d4 a855 9853 7668  ...V..3.V..U.Svh
-00005420: c5a1 11d8 fc74 7a9c 42b4 8cd0 333c eed8  .....tz.B...3<..
-00005430: b1fa 8fd9 3957 14b3 7bad 3c09 a836 eb14  ....9W..{.<..6..
-00005440: e5b9 6f7f 06e2 c4fe 4954 0b5e 035d cad8  ..o.....IT.^.]..
-00005450: 3178 5313 2710 640b a80b 4d94 c861 e174  1xS.'.d...M..a.t
-00005460: cfd7 871d 4449 4009 b7de 5abd 27b4 370a  ....DI@...Z.'.7.
-00005470: 1f82 301a bfa1 968c 9686 c5e6 6298 1bdf  ..0.........b...
-00005480: 20ac 3b19 1525 6948 99a2 786a 8107 5c4d   .;..%iH..xj..\M
-00005490: 16c6 f07a c04c 8c1c 4d4d 15f9 6751 02bf  ...z.L..MM..gQ..
-000054a0: c92c 89c3 6416 f8d3 99f5 e139 0c2c 1108  .,..d......9.,..
-000054b0: f05a aa12 7a43 5f9f 2138 d78a b205 2395  .Z..zC_.!8....#.
-000054c0: 06bf 14dd 6ccd bf96 3be3 a5d4 1a3e a16c  ....l...;....>.l
-000054d0: 5152 bc91 0233 535a fd8e e14e e829 d03e  QR...3SZ...N.).>
-000054e0: 52a4 b7f0 f9f7 b5fc 636c 8c89 cec2 287d  R.......cl....(}
-000054f0: cbc5 5219 a50e 947b c6a3 f45b e7ee f7ad  ..R....{...[....
-00005500: 7312 4256 10c6 ae8c 735f aa63 dccc 27dc  s.BV....s_.c..'.
-00005510: 548e d8f3 9ceb f790 7ce8 b2e6 83eb 1f21  T.......|......!
-00005520: ebdd 631b a376 6162 3744 6bb1 87b0 261f  ..c..vab7Dk...&.
-00005530: cfc7 759a ea68 e0a1 dd01 10ec 5841 f31c  ..u..h......XA..
-00005540: b23a ee76 f06e c70e a649 99f6 d3ad 60cf  .:.v.n...I....`.
-00005550: 6975 cee8 4670 d22a 640b e849 edd2 cc1b  iu..Fp.*d..I....
-00005560: 4d0b d3ca 0a78 4bda 0ed4 540f 3bf3 6be9  M....xK...T.;.k.
-00005570: 6ca5 a2df c08f df47 0852 7b2b f2c6 bfae  l......G.R{+....
-00005580: 1e46 bbfa 71cf d744 e576 bc0e 32f0 927c  .F..q..D.v..2..|
-00005590: fcc4 0000 fdbe bc9e 2e90 a56d 2f23 0ae6  ...........m/#..
-000055a0: 0504 a16c efad e0df 4670 6495 8f48 fd1d  ...l....Fpd..H..
-000055b0: cacf 4ffd af8c f4a0 62e1 00f3 b37b c5eb  ..O.....b....{..
-000055c0: 6af3 16a1 ff63 6dfe 1982 afaa cdc7 29ff  j....cm.......).
-000055d0: 99da b483 1246 e360 fede 9abe c739 ea98  .....F.`.....9..
-000055e0: 6366 8a3e 9ab6 c906 bd6a bda7 0c8e 4ff7  cf.>.....j....O.
-000055f0: 4c5e c02c 9bd3 2cb7 a739 6d6e 1876 ca1f  L^.,..,..9mn.v..
-00005600: adc0 482f 4985 f74c 5f1f 5fa6 e8f4 fc37  ..H/I..L_._....7
-00005610: 29e9 9e27 47ad 4ff4 466a 0b91 a2d3 f307  )..'G.O.Fj......
-00005620: 739c 0a62 7334 248d fe50 c3f9 07fe 9dbd  s..bs4$..P......
-00005630: a229 faf7 72f9 3659 5de6 a13b f397 3377  .)..r.6Y]..;..3w
-00005640: 3a21 919b 44cb 951b 4d2f 96ab 559e f8a1  :!..D...M/..U...
-00005650: 7ff1 dfe0 aaf3 8a8b 8ebd 96c1 900a a6f3  ................
-00005660: 9ac1 7548 75ce 762e 5e9d 6429 1a2c 5afa  ..uHu.v.^.d).,Z.
-00005670: f660 0bb4 87dc 9330 f6cf a3c0 77f3 891f  .`.....0....w...
-00005680: b8d3 18cf dc59 3c89 dc3c 0ac2 553c 5d5e  .....Y<..<..U<]^
-00005690: 4679 34e0 1ebd f06a e57b 41d0 5fad 9a20  Fy4....j.{A._.. 
-000056a0: 9a6b ca09 a3a2 cf55 9fa1 a114 9204 cb47  .k.....U.......G
-000056b0: 9cf0 fa4c 78a7 3b6f f61d 0000 ffff 0300  ...Lx.;o........
-000056c0: 504b 0304 1400 0600 0800 0000 2100 e1cd  PK..........!...
-000056d0: 299a 3b01 0000 aa04 0000 1400 0000 786c  ).;...........xl
-000056e0: 2f73 6861 7265 6453 7472 696e 6773 2e78  /sharedStrings.x
-000056f0: 6d6c 6cd4 416b 8330 18c6 f1fb 60df 21e4  mll.Ak.0....`.!.
-00005700: 3228 ac31 895a 1d6a 0f85 d10f b09d 47aa  2(.1.Z.j......G.
-00005710: efaa a0d1 9938 ba6f 3f47 2f23 8f47 7ffe  .....8.o?G/#.G..
-00005720: 7d8d 462c 8eb7 a167 df34 bb6e b425 97fb  }.F,...g.4.n.%..
-00005730: 8833 b2f5 d874 f65a f2f7 b7d7 e78c 33e7  .3...t.Z......3.
-00005740: 8d6d 4c3f 5a2a f90f 397e ac1e 1f0a e73c  .mL?Z*..9~.....<
-00005750: 5baf b5ae e4ad f7d3 8b10 ae6e 6930 6e3f  [..........ni0n?
-00005760: 4e64 d733 9fe3 3c18 bf1e ce57 e1a6 994c  Nd.3..<....W...L
-00005770: e35a 223f f442 4551 2a06 d359 ceea 71b1  .Z"?.BEQ*..Y..q.
-00005780: bee4 3a56 9c2d b6fb 5ae8 7497 24e6 55e1  ..:V.-..Z.t.$.U.
-00005790: baaa f095 5dea 9eba 42f8 aa10 7f72 5737  ....]...B....rW7
-000057a0: a990 e836 7d34 c61b f4ba 35f6 4aa1 f7e6  ...6}4....5.J...
-000057b0: 423d 93db 0cd3 efb5 0eeb 5308 e710 5258  B=........S...RX
-000057c0: 507a 091b 2921 9212 ab04 ab04 ab03 5607  Pz..)!........V.
-000057d0: ac32 ac32 a854 0495 8ab0 d258 69bc 235e  .2.2.T.....Xi.#^
-000057e0: 2871 3c8e 8a61 382e 3dc7 8749 4f67 d8ac  (q<..a8.=..IOg..
-000057f0: 7407 9bb3 033a 6c08 9054 5b84 966c 1118  t....:l..T[..l..
-00005800: 0ed3 d064 20f9 c61c 208d 0f98 21e5 48f2  ...d ... ...!.H.
-00005810: 297c 570a 4483 c420 0948 8a0d 6c5f feef  )|W.D.. .H..l_..
-00005820: f311 ebbf a6fa 0500 00ff ff03 0050 4b03  .............PK.
-00005830: 0414 0006 0008 0000 0021 001a e8a8 b791  .........!......
-00005840: 0600 00e5 1b00 0013 0000 0078 6c2f 7468  ...........xl/th
-00005850: 656d 652f 7468 656d 6531 2e78 6d6c ec59  eme/theme1.xml.Y
-00005860: cd6e 1b37 10be 17e8 3b10 7b4f 2cd9 9263  .n.7....;.{O,..c
-00005870: 1991 034b 96e2 3671 62d8 4a8a 1ca9 15b5  ...K..6qb.J.....
-00005880: cb98 bb5c 9094 1ddd 8ae4 58a0 40d1 b4e8  ...\......X.@...
-00005890: a540 6f3d 146d 0324 402f e9d3 b84d d1a6  .@o=.m.$@/...M..
-000058a0: 405e a143 7225 9116 15db 8981 fec5 066c  @^.Cr%.........l
-000058b0: 89fb 7166 383f 1f87 dcab d71e 640c 1d12  ..qf8?......d...
-000058c0: 2129 cf9b 51f5 7225 4224 8ff9 80e6 4933  !)..Q.r%B$....I3
-000058d0: bad3 eb5e 5a8b 9054 381f 60c6 73d2 8cc6  ...^Z..T8.`.s...
-000058e0: 4446 d736 de7f ef2a 5e57 29c9 0882 f9b9  DF.6...*^W).....
-000058f0: 5cc7 cd28 55aa 585f 5a92 310c 6379 9917  \..(U.X_Z.1.cy..
-00005900: 2487 6743 2e32 ace0 ab48 9606 021f 81dc  $.gC.2...H......
-00005910: 8c2d 2d57 2aab 4b19 a679 8472 9c81 d81e  .--W*.K..y.r....
-00005920: cc41 0382 6e0f 8734 26d1 c644 7c87 818e  .A..n..4&..D|...
-00005930: 5c49 3d10 33b1 af85 9372 8e83 1d1c 5435  \I=.3....r....T5
-00005940: 428e 659b 0974 8859 3302 4d03 7ed4 230f  B.e..t.Y3.M.~.#.
-00005950: 5484 1896 0a1e 34a3 8af9 8996 36ae 2ee1  T.....4.....6...
-00005960: f572 1253 0be6 3af3 bae6 a79c 574e 181c  .r.S..:.....WN..
-00005970: 2c1b 9d22 e94f 9556 bbb5 c695 ada9 7c03  ,..".O.V......|.
-00005980: 606a 1ed7 e974 da9d ea54 9e01 e038 8695  `j...t...T...8..
-00005990: 5a5b 5c99 b5ee 5ab5 3591 e980 ecc7 79d9  Z[\...Z.5.....y.
-000059a0: ed4a bd52 f3f1 8efc 9539 9b1b ad56 abde  .J.R.....9...V..
-000059b0: 286d b142 0dc8 7eac cde1 d72a abb5 cd65  (m.B..~....*...e
-000059c0: 0f6f 4016 5f9f c3d7 5a9b edf6 aa87 3720  .o@._...Z.....7 
-000059d0: 8b5f 9dc3 77af 3456 6b3e de80 5246 f383  ._..w.4Vk>..RF..
-000059e0: 39b4 0e68 b75b 4a9f 4286 9c6d 07e1 6b00  9..h.[J.B..m..k.
-000059f0: 5fab 94f0 190a b261 9a5d 5ac5 90e7 6a51  _......a.]Z...jQ
-00005a00: ae65 f83e 175d 0068 20c3 8ae6 488d 0b32  .e.>.].h ...H..2
-00005a10: c431 e471 1b67 7d41 7184 0a9c 7309 0395  .1.q.g}Aq...s...
-00005a20: e54a b7b2 027f f56f cd7c aa69 f578 9d60  .J.....o.|.i.x.`
-00005a30: 679e 1d8a e5dc 90b6 04c9 58d0 4235 a30f  g.........X.B5..
-00005a40: 416a e440 5e3d fffe d5f3 a7e8 d5f3 27c7  Aj.@^=........'.
-00005a50: 0f9f 1d3f fce9 f8d1 a3e3 873f 5a59 dec4  ...?.......?ZY..
-00005a60: 6d9c 27ee c497 df7e f6e7 d71f a33f 9e7e  m.'....~.....?.~
-00005a70: f3f2 f117 61bc 74f1 bffe f0c9 2f3f 7f1e  ....a.t...../?..
-00005a80: 0642 7dcd d6ff e2cb 27bf 3d7b f2e2 ab4f  .B}.....'.={...O
-00005a90: 7fff ee71 00be 2970 df85 f768 4624 ba45  ...q..)p...hF$.E
-00005aa0: 8ed0 1ecf 606d c631 bee5 a42f ce37 a397  ....`m.1.../.7..
-00005ab0: 62ea cdc0 29c8 0e88 eea8 d403 de1a 6316  b...).........c.
-00005ac0: c2b5 88ef bcbb 02a8 2504 bc3e baef d9ba  ........%..>....
-00005ad0: 9f8a 91a2 01cd 37d2 cc03 ee70 ce5a 5c04  ......7....p.Z\.
-00005ae0: 1d70 43eb 723c dc1b e549 58b9 18b9 b83d  .pC.r<...IX....=
-00005af0: 8c0f 43ba db38 f742 db19 15c0 a990 b2f3  ..C..8.B........
-00005b00: be6f a7c4 3373 97e1 5ce1 84e4 4421 fd8c  .o..3s..\...D!..
-00005b10: 1f10 1298 768f 52cf af3b 3416 5cf2 a142  ....v.R..;4.\..B
-00005b20: f728 6a61 1a74 498f f6bd 449a 4dda a619  .(ja.tI...D.M...
-00005b30: c465 1c32 1042 edf9 66e7 2e6a 7116 5af5  .e.2.B..f..jq.Z.
-00005b40: 1639 f491 5010 9805 8cef 11e6 b9f1 3a1e  .9..P.........:.
-00005b50: 299c 8544 f670 c65c 87df c42a 0d19 b93f  )..D.p.\...*...?
-00005b60: 16b1 8beb 4805 914e 08e3 a833 2052 86e6  ....H..N...3 R..
-00005b70: dc16 b05e 27e8 3730 b059 30ec 3b6c 9cf9  ...^'.70.Y0.;l..
-00005b80: 48a1 e841 48e6 4dcc b98b dce2 07ed 1467  H..AH.M........g
-00005b90: 45d0 669a a72e f603 7900 298a d12e 5721  E.f.....y.)...W!
-00005ba0: f80e f72b 447f 8738 e07c 61b8 ef52 e285  ...+D..8.|a..R..
-00005bb0: fb74 22b8 4313 cfa4 5982 e827 2311 88e5  .t".C...Y..'#...
-00005bc0: 75c2 fd7a 1cb3 2126 8665 80f0 3d1e cf68  u..z..!&.e..=..h
-00005bd0: fe3a 5267 1458 fd04 a9d7 df91 badd 954e  .:Rg.X.........N
-00005be0: 92fa 266c 80a1 d2da 3e41 e58b 70ff 4202  ..&l....>A..p.B.
-00005bf0: dfc2 a37c 9740 cdcc 93e8 3bfe 7ec7 dfd1  ...|.@....;.~...
-00005c00: 7f9e bf17 d5f2 c5b3 f68c a881 c367 7dba  .............g}.
-00005c10: e9da b385 4dfb 9032 b6af c68c dc94 a66f  ....M..2.......o
-00005c20: 97b0 3d0d ba30 680e 14e6 5439 3dc4 1529  ..=..0h...T9=..)
-00005c30: 7c2c 8f08 1e2e 11d8 cc41 82ab 8fa8 4af7  |,.......A....J.
-00005c40: 535c 408b 5f35 c7d5 4496 a213 890a 2ea1  S\@._5..D.......
-00005c50: f337 c3e6 384c 4ec8 36c7 5b0a 8dbd 39a9  .7..8LN.6.[...9.
-00005c60: d6f5 19c6 3287 c46a 870f ecf0 8a7b 569d  ....2..j.....{V.
-00005c70: 8a31 27d7 c49c 8727 8a56 b480 b32a 5bb9  .1'....'.V...*[.
-00005c80: f276 caaa d6aa 856e f397 5635 a619 52f4  .v.....n..V5..R.
-00005c90: 9636 5d32 c470 7e69 3038 f526 f43d 08ba  .6]2.p~i08.&.=..
-00005ca0: 25f0 f22a 5c1a 68db e134 8419 1968 bfdb  %..*\.h..4...h..
-00005cb0: 73fc 242c 5af5 8586 48a6 18ae 246c 8cf4  s.$,Z...H...$l..
-00005cc0: bae7 6354 3541 9ae4 ca24 8d02 31d2 e7ce  ..cT5A...$..1...
-00005cd0: 5362 e468 6b68 b16f a1ed 2c41 72d5 d516  Sb.hkh.o..,Ar...
-00005ce0: a89b 44ef 6da2 3439 6ccf a2a4 ebf6 4439  ..D.m.49l.....D9
-00005cf0: b2dc 2d4e 96a3 a366 d4a8 2fd7 2314 e3a2  ..-N...f../.#...
-00005d00: 190d e198 0d1f b302 a22e 75ab 8959 02b7  ..........u..Y..
-00005d10: 55b1 1236 ed4f 2d66 93ae b368 36c2 6959  U..6.O-f...h6.iY
-00005d20: 859b 13eb f7b9 057b 3c50 08a9 b6b0 4c6d  .......{<P....Lm
-00005d30: 6a98 4765 0ab0 dc5c 0a18 fb97 ebe0 d68b  j.Ge...\........
-00005d40: 5a80 cdf4 37b0 6265 0d92 e16f b302 fce8  Z...7.be...o....
-00005d50: 8796 0c87 2456 6eb0 9d11 732b 6200 2595  ....$Vn...s+b.%.
-00005d60: f291 2262 3f1d 1ca1 3e1b 893d 0ce1 d7a9  .."b?...>..=....
-00005d70: 0aeb 1950 09f7 2186 11f4 17b8 dad3 de36  ...P..!........6
-00005d80: 8f7c 722e 8bce bd50 3338 3b8e 5991 e292  .|r....P38;.Y...
-00005d90: 6e75 894e 2ad9 c24d 1d4f 6d30 dfac b5c6  nu.N*..M.Om0....
-00005da0: 3c58 5bd0 76b3 b8f3 2fc5 94fc 052d c54d  <X[.v.../....-.M
-00005db0: e3ff d952 f47e 0217 142b 031d 8118 ee96  ...R.~...+......
-00005dc0: 0546 ba5e 9b11 172a e5c0 4245 4ae3 ae80  .F.^...*..BEJ...
-00005dd0: 6b35 c31d 902d 703d 0c8f 21a9 e086 dbfc  k5...-p=..!.....
-00005de0: 17e4 50ff b735 6765 98b2 8673 a6da a309  ..P..5ge...s....
-00005df0: 1214 f623 950a 4276 8196 4cf6 9d22 ac5a  ...#..Bv..L..".Z
-00005e00: ee5d 5624 2b05 998c 72cc 9585 35bb 4f0e  .]V$+...r...5.O.
-00005e10: 09eb 690e 5cd5 7b7b 8452 4875 c326 250d  ..i.\.{{.RHu.&%.
-00005e20: 18dc c9fc f3bf 9715 d44f 7493 f34f ed7c  .........Ot..O.|
-00005e30: 6c31 9fb7 3dd0 dd81 6db1 ecfc 33f6 2235  l1..=...m...3."5
-00005e40: 87f4 9dad a011 dcfb 4c4f 35a5 83d7 6cec  ........LO5...l.
-00005e50: e7dc 6a2d 63cd ad78 b97e e6ad b680 6b26  ..j-c..x.~....k&
-00005e60: b85d 5690 1331 1531 b32f 4bf4 86da e37b  .]V..1.1./K....{
-00005e70: c0ad 08de 7dd8 f60a 4156 5fb2 8d07 d204  ....}...AV_.....
-00005e80: 69e9 b10f 8d93 1db4 c9a4 45d9 86a5 ec6e  i.........E....n
-00005e90: 2fbc 8d82 1bf2 b2d3 9dea 852a 7d93 4ef7  /..........*}.N.
-00005ea0: 9cce 9e36 67be 3aaf 165f df7d 9ecf d9a5  ...6g.:.._.}....
-00005eb0: 873d 5fbb 9d6e c0d5 50b4 274b 54b7 4793  .=_..n..P.'KT.G.
-00005ec0: 838c 098c 79cf e6be 08e3 fdfb 10e8 2d78  ....y.........-x
-00005ed0: e530 624a da97 090f e052 114e 19f6 a505  .0bJ.....R.N....
-00005ee0: 14bf 0dae 99ba f117 0000 00ff ff03 0050  ...............P
-00005ef0: 4b03 0414 0006 0008 0000 0021 0075 84b7  K..........!.u..
-00005f00: f963 0100 007c 0400 0027 0000 0078 6c2f  .c...|...'...xl/
-00005f10: 7072 696e 7465 7253 6574 7469 6e67 732f  printerSettings/
-00005f20: 7072 696e 7465 7253 6574 7469 6e67 7335  printerSettings5
-00005f30: 2e62 696e ec53 cd4a c340 10fe b611 512f  .bin.S.J.@....Q/
-00005f40: 7af4 50a4 788a 8742 4d53 5b8f 6993 4a24  z.P.x..BMS[.i.J$
-00005f50: c996 6cea 3dd2 8506 4212 d214 fcc1 9b0f  ..l.=...B.......
-00005f60: d237 f145 7c02 0fbe 82ce 5685 0a22 14bd  .7.E|.....V.."..
-00005f70: 08ce b2fb 4dbe 99f9 76b3 cb38 1841 8023  ....M...v..8.A.#
-00005f80: c029 6cf4 d1a1 d946 033a 3cc2 0e8d 06c5  .)l....F.:<.....
-00005f90: 254a 24b4 ce70 84cf c636 b4cd 472c 34ed  %J$..p...6..G,4.
-00005fa0: 0135 0686 a79d 7c6b 42b8 8b29 ab11 4e99  .5....|kB..)..N.
-00005fb0: 46ab 47b5 150d a5f3 7363 ef12 0a6b 3415  F.G.....sc...k4.
-00005fc0: be90 9db9 c25c 55b7 dd60 7c08 9ddd 6b75  .....\U..`|...ku
-00005fd0: 2c9e a707 dfed bcbd 1254 7a1f 7bfc c271  ,........Tz.{..q
-00005fe0: ff25 fec8 0dac f3e6 3a25 0b3f 3a57 bfb6  .%......:%.?:W..
-00005ff0: 877d 768b 215a d43b 0e06 3060 5137 3589  .}v.!Z.;..0`Q75.
-00006000: 31e8 db20 cf44 173d eaaf 26f1 5dca 50d1  1.. .D.=..&.].P.
-00006010: e325 6750 97a9 9c1e 55b7 89ef e08e 14dd  .%gP....U.......
-00006020: ac98 57fd 24c3 9087 bee0 e370 e020 7484  ..W.$......p. t.
-00006030: ed79 1867 4929 67ca e365 22b3 2aae 923c  .y.gI)g..e".*..<
-00006040: c388 8751 68b9 1142 39cb d3f9 92e3 8582  ...Qh..B9.......
-00006050: f649 0ba3 b890 a548 6e24 2c13 833c cd4b  .I.....Hn$,..<.K
-00006060: 3f9f c837 cf30 2f8b 42b9 695c 49f0 00be  ?..7.0/.B.i\I...
-00006070: 9c24 7174 5d48 88c8 0a6c 2bb4 61cf 8b54  .$qt]H...l+.a..T
-00006080: 5e21 e081 b3ee 53d6 a9e0 c2b4 fdaf eef6  ^!....S.........
-00006090: 1500 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-000060a0: 0000 0021 0075 84b7 f963 0100 007c 0400  ...!.u...c...|..
-000060b0: 0027 0000 0078 6c2f 7072 696e 7465 7253  .'...xl/printerS
-000060c0: 6574 7469 6e67 732f 7072 696e 7465 7253  ettings/printerS
-000060d0: 6574 7469 6e67 7331 2e62 696e ec53 cd4a  ettings1.bin.S.J
-000060e0: c340 10fe b611 512f 7af4 50a4 788a 8742  .@....Q/z.P.x..B
-000060f0: 4d53 5b8f 6993 4a24 c996 6cea 3dd2 8506  MS[.i.J$..l.=...
-00006100: 4212 d214 fcc1 9b0f d237 f145 7c02 0fbe  B........7.E|...
-00006110: 82ce 5685 0a22 14bd 08ce b2fb 4dbe 99f9  ..V.."......M...
-00006120: 76b3 cb38 1841 8023 c029 6cf4 d1a1 d946  v..8.A.#.)l....F
-00006130: 033a 3cc2 0e8d 06c5 254a 24b4 ce70 84cf  .:<.....%J$..p..
-00006140: c636 b4cd 472c 34ed 0135 0686 a79d 7c6b  .6..G,4..5....|k
-00006150: 42b8 8b29 ab11 4e99 46ab 47b5 150d a5f3  B..)..N.F.G.....
-00006160: 7363 ef12 0a6b 3415 be90 9db9 c25c 55b7  sc...k4......\U.
-00006170: dd60 7c08 9ddd 6b75 2c9e a707 dfed bcbd  .`|...ku,.......
-00006180: 1254 7a1f 7bfc c271 ff25 fec8 0dac f3e6  .Tz.{..q.%......
-00006190: 3a25 0b3f 3a57 bfb6 877d 768b 215a d43b  :%.?:W...}v.!Z.;
-000061a0: 0e06 3060 5137 3589 31e8 db20 cf44 173d  ..0`Q75.1.. .D.=
-000061b0: eaaf 26f1 5dca 50d1 e325 6750 97a9 9c1e  ..&.].P..%gP....
-000061c0: 55b7 89ef e08e 14dd ac98 57fd 24c3 9087  U.........W.$...
-000061d0: bee0 e370 e020 7484 ed79 1867 4929 67ca  ...p. t..y.gI)g.
-000061e0: e365 22b3 2aae 923c c388 8751 68b9 1142  .e".*..<...Qh..B
-000061f0: 39cb d3f9 92e3 8582 f649 0ba3 b890 a548  9........I.....H
-00006200: 6e24 2c13 833c cd4b 3f9f c837 cf30 2f8b  n$,..<.K?..7.0/.
-00006210: 42b9 695c 49f0 00be 9c24 7174 5d48 88c8  B.i\I....$qt]H..
-00006220: 0a6c 2bb4 61cf 8b54 5e21 e081 b3ee 53d6  .l+.a..T^!....S.
-00006230: a9e0 c2b4 fdaf eef6 1500 00ff ff03 0050  ...............P
-00006240: 4b03 0414 0006 0008 0000 0021 005c 9627  K..........!.\.'
-00006250: 22c3 0000 0028 0100 001e 0008 0163 7573  "....(.......cus
-00006260: 746f 6d58 6d6c 2f5f 7265 6c73 2f69 7465  tomXml/_rels/ite
-00006270: 6d32 2e78 6d6c 2e72 656c 7320 a204 0128  m2.xml.rels ...(
-00006280: a000 0100 0000 0000 0000 0000 0000 0000  ................
-00006290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000062a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000062b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000062c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000062d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000009c0: 5d4f db30 147d 9fb4 ff60 f975 6add a449  ]O.0.}...`.uj..I
+000009d0: 81aa 2982 b20f a469 42ac 8347 e43a b78d  ..)....iB..G.:..
+000009e0: 8563 7bb6 43e1 dfef 2621 6956 5e98 f692  .c{.C...&!iV^...
+000009f0: f8da c7e7 dae7 dceb c5f9 73a9 c813 382f  ..........s...8/
+00000a00: 8dce 6834 9e50 025a 985c ea5d 467f adbf  ..h4.P.Z.\.]F...
+00000a10: 8c4e 29f1 81eb 9c2b a321 a32f e0e9 f9f2  .N)....+.!./....
+00000a20: e387 c5de b8c7 8d31 8f04 09b4 cf68 1182  .......1.....h..
+00000a30: 9d33 e645 0125 f763 6341 e3ca d6b8 9207  .3.E.%.ccA......
+00000a40: 0cdd 8e79 eb80 e7be 0008 a562 f164 3263  ...y.......b.d2c
+00000a50: 2597 9ab6 0c73 f71e 0eb3 dd4a 0157 4654  %....s.....J.WFT
+00000a60: 25e8 d092 3850 3ce0 f17d 21ad efd8 4af1  %...8P<..}!...J.
+00000a70: 1eba 92bb c7ca 8e84 292d 526c a492 e1a5  ........)-Rl....
+00000a80: 21a5 a414 f3eb 9d36 8e6f 145e fb39 4a3b  !......6.o.^.9J;
+00000a90: 661c bea1 2ea5 70c6 9b6d 1823 156b 0ff9  f.....p..m.#.k..
+00000aa0: e6be d184 4551 7be5 e562 2b15 dcb5 b213  ....EQ{..b+.....
+00000ab0: 6eed 0f5e d659 1425 8afb f039 9701 f28c  n..^.Y.%...9....
+00000ac0: ce30 347b 384c 2494 b8ca 5e56 52e1 6a94  .04{8L$...^VR.j.
+00000ad0: 24f1 84b2 656f c58d 23e8 1cb4 5ceb 42fa  $...eo..#...\.B.
+00000ae0: fb57 8f28 c961 cb2b 15d6 684e 9716 09e2  .W.(.a.+..hN....
+00000af0: 248e 6735 035e f642 0570 9a07 5819 1d50  $.g5.^.B.p..X..P
+00000b00: db57 57fe 57c7 867b 5518 748d dcc2 ef4a  .WW.W..{U.t....J
+00000b10: 3ac0 62a9 e55c 2ef0 cbc5 9c6f fc0d 0f05  :.b..\.....o....
+00000b20: a99c 6a75 f558 4695 e066 3a4b c7be e00e  ..ju.XF..f:K....
+00000b30: ac91 ba55 d6a3 2e9e dd5e 4ab3 5a7d e71b  ...U.....^J.Z}..
+00000b40: d615 82f1 7873 f4d0 0599 1bcf be82 06c7  ....xs..........
+00000b50: 15bb ba49 3e91 0b6b d9c5 e827 9ab3 472e  ...I>..k...'..G.
+00000b60: 96db c4aa ca3f a0e8 cc3b f157 ac4b f720  .....?...;.W.K. 
+00000b70: 2a1f d0c3 81db fc6d 29fd 83df 5cd4 0233  *......m)...\..3
+00000b80: 54b8 55a1 1d1f abbd 5cd4 bd74 2761 ef0f  T.U.....\..t'a..
+00000b90: 7ed6 2179 be97 3a37 fb8c 8ea2 b329 fa4d  ~.!y..:7.....).M
+00000ba0: 5efa 8933 8cf6 cdea bdcc 4381 869e 2549  ^..3......C...%I
+00000bb0: 3ff7 0de4 ae08 3899 4629 4e72 11e4 13ac  ?.....8.F)Nr....
+00000bc0: f926 a349 73a2 41c2 a627 3171 f327 baa9  .&.Is.A..'1q.'..
+00000bd0: c508 fbbe 6ed5 ebba d270 bf9b 4b1c b9eb  ....n....p..K...
+00000be0: 3caa 770f 91f1 1039 1d20 e363 242e 1e38  <.w....9. .c$..8
+00000bf0: 715b cf39 3d46 62a1 1f90 75d5 77d9 9bb3  q[.9=Fb...u.w...
+00000c00: 0fb3 635f 1e90 18f4 c8f4 9813 bbe9 80c4  ..c_............
+00000c10: a047 362d 30e4 3c19 2231 e891 27c7 9cf5  .G6-0.<."1..'...
+00000c20: ebd8 ab84 418f 3c6d 34ee 8415 5c89 ba3b  ....A.<m4...\..;
+00000c30: f1d7 e899 c669 d4e8 c8ba 6774 f907 0000  .....i....gt....
+00000c40: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+00000c50: 2100 b621 0fa0 1a09 0000 342f 0000 1800  !..!......4/....
+00000c60: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00000c70: 7368 6565 7434 2e78 6d6c ac9a 5d6f eb36  sheet4.xml..]o.6
+00000c80: 1286 ef17 e87f 3074 5fd9 921c 270e e214  ......0t_...'...
+00000c90: 756c 5907 d82d 8ab6 bb7b add8 4aa2 1edb  ulY..-...{..J...
+00000ca0: f24a caf9 e8af ef90 33a4 c819 1fb5 0bb0  .J......3.......
+00000cb0: 17a7 f170 6644 3f1a 922f 693e fcf0 e574  ...pfD?../i>...t
+00000cc0: 9c7c aada ae6e ceab 2889 67d1 a43a ef9b  .|...n..(.g..:..
+00000cd0: 437d 7e5d 45ff fe2d fffe 2e9a 747d 793e  C}~]E..-....t}y>
+00000ce0: 94c7 e65c ada2 af55 17fd f0f8 dd3f 1e3e  ...\...U.....?.>
+00000cf0: 37ed c7ee adaa fa09 6438 77ab e8ad ef2f  7.......d8w..../
+00000d00: f7d3 69b7 7fab 4e65 1737 97ea 0c2d 2f4d  ..i...Ne.7...-/M
+00000d10: 7b2a 7bf8 d8be 4ebb 4b5b 9507 1d74 3a4e  {*{...N.K[...t:N
+00000d20: d3d9 6c31 3d95 f539 c20c f7ed dfc9 d1bc  ..l1=..9........
+00000d30: bcd4 fb6a d3ec df4f d5b9 c724 6d75 2c7b  ...j...O...$mu,{
+00000d40: e87f f756 5f3a 93ed b4ff 3be9 4e65 fbf1  ...V_:....;.Ne..
+00000d50: fdf2 fdbe 395d 20c5 737d acfb af3a 6934  ....9] .s}...:i4
+00000d60: 39ed ef3f bc9e 9bb6 7c3e c2f7 fe92 cccb  9..?....|>......
+00000d70: bdc9 ad3f 88f4 a77a df36 5df3 d2c7 906e  ...?...z.6]....n
+00000d80: 8a1d 95df 7939 5d4e 21d3 e383 e6f0 733b  ....y9]N!.....s;
+00000d90: 01d8 d54f e509 9e51 34bf 97f3 68fa f870  ...O...Q4...h..p
+00000da0: a8e1 cba9 3732 69ab 9755 f463 725f 644b  ....72i..U.cr_dK
+00000db0: d5a0 63fe 5357 9f3b e7ef 49df 5cfe 59bd  ..c.SW.;..I.\.Y.
+00000dc0: f44f d5f1 08ce 691a 4dfe 689a d3af fb52  .O....i.M.h....R
+00000dd0: 757c 096f d47e fc49 bd0d 7052 46f5 029f  u|.o.~.I..pRF...
+00000de0: 9be6 a34a f7e1 b08a 66aa 4fd5 b1da 2b94  ...J....f.O...+.
+00000df0: 9312 fef7 a9c2 944f 892a 82ff e9be a8bf  .......O.*......
+00000e00: a123 53db 13f7 6fd3 ab5c bf74 f86e cf65  .#S...o..\.t.n.e
+00000e10: 573d 35c7 ffd6 87fe 0daa 0b9e 7aa8 5eca  W=5.........z.^.
+00000e20: f763 ff4b f3b9 a8ea d7b7 1eac 8bf8 269a  .c.K..........&.
+00000e30: ecdf bbbe 3959 1b90 56c0 ef0f 5f37 55b7  ....9Y..V..._7U.
+00000e40: 8737 0dfd 8b53 f5e4 7d73 84c7 c0bf 9353  .7...S..}s.....S
+00000e50: ad2a 165e 54f9 4565 c9ee e6f0 a5e8 4949  .*.^T.Ee......II
+00000e60: 3c4f 6f6e ef92 1452 77fd 5705 22d3 fdc6  <Oon...Rw.W."...
+00000e70: 70dd fb4d d997 8f0f 6df3 7902 9507 79ba  p..M....m.y...y.
+00000e80: 4ba9 ea38 b987 6ffb ff76 0c7a a4b2 fca8  K..8..o..v.z....
+00000e90: d2a8 474d a0c3 1d00 fdf4 7833 7f98 7e02  ..GM......x3..~.
+00000ea0: 487b 7259 a30b f4cb bacc 7c8f 27e9 91f8  H{rY......|.'...
+00000eb0: 1e1b e991 fa1e 5be9 91f9 1eb9 f460 3ddd  ......[......`=.
+00000ec0: 498f 1b3f 4721 3d16 d663 0a64 2d5e a8c9  I..?G!=..c.d-^..
+00000ed0: 1078 559a 5594 6ab0 8cc9 1adb 5cae b78c  .xU.U.j.....\...
+00000ee0: abf1 50af 8513 c5b6 0566 be49 e225 e369  ..P......f.I.%.i
+00000ef0: 6255 05aa 379d a3e1 5607 30b4 3bee 5c38  bU..7...V.0.;.\8
+00000f00: 060f 0b14 4a08 2c2a 8dc1 c20a 618d 6d63  ....J.,*....a.mc
+00000f10: 588c c735 2cd8 4658 d2bb 9861 db9a 588b  X..5,.FX...a..X.
+00000f20: 050d 8885 39ef b873 e118 3c2c 3090 4360  ....9..s..<,0.C`
+00000f30: 5169 0c16 f68a d6d8 3686 c578 5cc3 826d  Qi......6..x\..m
+00000f40: 84e5 ee46 548b 89b5 58d0 8058 8621 a22b  ...FT...X..X.!.+
+00000f50: 69c7 9d0b c7e0 6151 7359 8039 4aa5 3158  i.....aQsY.9J.1X
+00000f60: f8e4 846d 6358 8cc7 352c d866 aae5 4654  ...mcX..5,.f..FT
+00000f70: 8b89 b558 d080 58d8 68dd 71e7 c231 7858  ...X..X.h.q..1xX
+00000f80: 1661 b0a8 3406 0b9b e7d6 d836 86c5 785c  .a..4......6..x\
+00000f90: c382 6d84 6531 8f59 2d6e 4dac c582 06c4  ..m.e1.Y-nM.....
+00000fa0: 72e7 4f44 3bee 5c38 060f cb6d 182c 2a8d  r.OD;.\8...m.,*.
+00000fb0: c1c2 2a77 8d6d 6358 8c87 f96a 1b34 208b  ..*w.mcX...j.4 .
+00000fc0: 7419 b3fa db72 ff1c 0d88 82cd c93b ee5c  t....r.......;.\
+00000fd0: 3806 0f85 922f 0106 8e4a 6350 b06a 5d63  8..../...JcP.j]c
+00000fe0: db18 0ae3 6151 a001 5164 4c03 6cb9 778e  ....aQ..QdL.l.w.
+00000ff0: 069a 5859 7dee b877 e118 3c12 cb30 2454  ..XY}..w..<..0$T
+00001000: 1a43 8215 e81a dbc6 4818 0f4b 020d 4422  .C......H..K..D"
+00001010: 1345 c1fd 7334 100b bef8 72ef c231 782c  .E..s4....r..1x,
+00001020: 941c 0da2 f954 1e43 83d5 e85a 3f64 158d  .....T.C...Z?d..
+00001030: e1b0 2e96 0759 10c8 6211 33c4 5b11 9193  .....Y..b.3.[...
+00001040: 8590 300d b013 fe85 6bf1 a184 12c2 280d  ..0.....k.....(.
+00001050: 49aa b1ea 5e27 5238 72b1 665d 062a 1884  I...^'R8r.f].*..
+00001060: 54e6 73b1 ba88 889c 2c48 858f 19e1 5eb8  T.s.....,H....^.
+00001070: 161f 4a20 f99a 78fa 950b 586a 1d2d 15ae  ..J ..x...Xj.-..
+00001080: 2c37 1444 a592 8ab5 c526 b58b 0b59 48b9  ,7.D.....&...YH.
+00001090: 728d 26fc 0bd7 e253 09a4 5e13 57be 265c  r.&....S..^.W.&\
+000010a0: bf52 eb28 152e 2c37 1444 334a 1ab3 77bf  .R.(..,7.D3J..w.
+000010b0: b549 072a ae70 4df9 a22b fc0b d7e2 5309  .I.*.pM..+....S.
+000010c0: 245e 1357 bd26 5cbe 52eb 2815 ae2b 3714  $^.W.&\.R.(..+7.
+000010d0: 4403 6821 0790 90ad 1481 b592 7285 663b  D.h!........r.f;
+000010e0: 6128 16ae c5a7 a2c4 5b88 fd35 8a40 9a56  a(......[..5.@.V
+000010f0: c4d6 da48 c461 6f2d a615 2e2b 3709 5a88  ...H.ao-...+7.Z.
+00001100: ca9d ac15 1e91 5304 5111 f38a 10ae e47f  ......S.Q.......
+00001110: a30f 20dc 5d71 1248 baea 3c76 5fcc c52b  .. .]q.H..<v_..+
+00001120: b58e d60a 5795 1b0a a211 94c4 4cfa 6d6d  ....W.......L.mm
+00001130: d261 04b9 aa35 e3ab b2f0 2f5c 8b5f 2b81  .a...5..../\._+.
+00001140: 946b e24a d784 6b57 6a1d a522 d42b 0551  .k.J..kWj..".+.Q
+00001150: ada4 62df 6793 0e54 5c01 9bf1 ad9f f02f  ..b.g..T\....../
+00001160: 5c8b 4f25 9088 d567 79b6 56b8 8ca5 d651  \.O%...gy.V....Q
+00001170: 2a46 5b5e dbea 503c e9fb 941f 17d8 f403  *F[^..P<........
+00001180: 1f57 d766 62de 15c2 d6cd e0f3 0924 6d13  .W.fb........$m.
+00001190: 57db 265c dc52 eb28 1f21 6f29 c86c 0063  W.&\.R.(.!o).l.c
+000011a0: 067d 6b93 0e54 5c85 3b67 ea69 27fc 0bd7  .}k..T\.;g.i'...
+000011b0: e251 4903 695c 9dc7 560d 17b9 d43a 46c5  .QI.i\..V....:F.
+000011c0: ba58 3947 162a 954c 5011 1139 5948 e4f2  .X9G.*.LP..9YH..
+000011d0: dda0 f02f 5c8b 4f25 90c8 4d8d c81d d69b  .../\.O%..M.....
+000011e0: 54b0 f96b a94b 69f4 faa0 8f84 3664 a18a  T..k.Ki.....6d..
+000011f0: b98d 9399 fb1f 1f55 223e 270b 929a f373  .......U">'....s
+00001200: 5de1 5fb8 169f 54a8 835b 14ae 77d7 4f6e  ]._...T..[..w.On
+00001210: b111 6ade 1e89 b371 f7a4 7ed4 803d d6f2  ..j....q..~..=..
+00001220: 5afc 861a 614f a3a6 24f8 3941 1cde 9a68  Z...aO..$.9A...h
+00001230: 3bc0 4c48 a243 0420 ee5f d8e7 4306 1f50  ;.LH.C. ._..C..P
+00001240: 2011 9ca2 fe44 405c 0353 e328 208c ff06   ....D@\.S.( ...
+00001250: 206c b480 1201 c844 0f80 2804 01f1 0da5   l.....D..(.....
+00001260: ed90 557e aec5 0714 480f a728 4e11 1017  ..U~....H..(N...
+00001270: 7ed4 380a 08e3 bf01 081b 0740 fc5c ca3e  ~.8........@.\.>
+00001280: 6000 4421 0888 2f14 3b11 50b8 169f 5020  `.D!../.;.P...P 
+00001290: 6dac 7feb 5a45 b064 da61 c48f 95d6 e433  m...ZE.d.a.....3
+000012a0: 0a0a f5ab febd 9166 23b4 109d 34be 1513  .......f#...4...
+000012b0: 100f c9e9 39b0 a3d6 2a81 ef32 6d37 86fa  ....9...*..2m7..
+000012c0: 7152 f874 0269 e414 e5a9 4747 fc84 843e  qR.t.i....GG...>
+000012d0: a374 8ccb b08e a1c5 d299 2fbd c99a ff30  .t......../....0
+000012e0: 47fd 18f0 e664 31ac f86a 2f02 0ad7 e2b3  G....d1..j/.....
+000012f0: 0aa4 9c53 14ad 1e2b 3127 a1cf 282b e332  ...S...+1'..(+.2
+00001300: b042 cbc0 8a9f 6cd1 935d 3a14 4295 c4f7  .B....l..]:.B...
+00001310: a022 a070 2d3e 9d40 0a3a 4551 ead1 e1fb  .".p->.@.:EQ....
+00001320: 73f2 19a5 8369 dc71 8616 a293 c4a9 9885  s....i.q........
+00001330: 7848 4ecf 31b5 c3f7 17b6 1bc3 3873 52f8  xHN.1.......8sR.
+00001340: 7402 e9e7 14a5 2bce d35c 3e53 e328 168c  t.....+..\>S.(..
+00001350: 77b1 a0c5 160d df25 6c6d d661 72a6 102a  w......%lm.ar..*
+00001360: 1ab1 bef3 6714 6e0a 0f4b 1648 40eb 3c6a  ....g.n..K.H@.<j
+00001370: 72be 361f aea9 758c 8b75 b183 892c c425  r.6...u..u...,.%
+00001380: 8b53 febb 9208 c94d 0872 c9f8 b22e 020a  .S.....M.r......
+00001390: d7e2 7309 24a1 3394 c7de 60e2 ab3b f98c  ..s.$.3...`..;..
+000013a0: d2c1 344e d550 90ad 1ab1 17b5 596d d598  ..4N.P......Ym..
+000013b0: 10a2 c327 6211 50b8 169f 4e20 d99c 19d9  ...'b.P...N ....
+000013c0: ec2c e9fc 7887 7c46 e970 3dbb a120 3bd5  .,..x.|F.p=.. ;.
+000013d0: 2c44 ed08 c96c 4248 11f2 ed97 ed86 9d6a  ,D...lBH.......j
+000013e0: 5c8b 4f27 9066 ce5c cd9c 88aa 319a f6db  \.O'.f.\....1...
+000013f0: bb0a 4ae0 568d a794 610a e627 c722 2427  ..J.V...a..'."$'
+00001400: 0b4d c129 9f82 4540 e15a 7c2e 81a4 7266  .M.)..E@.Z|...rf
+00001410: a4b2 5335 fcf8 8b7c 46ab c628 e661 c6f1  ..S5...|F..(.a..
+00001420: 6472 7a85 0e0f c9e9 3944 27e3 33b1 edc6  drz.....9D'.3...
+00001430: 5035 4e0a 9f4e 2099 9ca1 d2f4 661c 7e0c  P5N..N .....f.~.
+00001440: 463e a374 844c a6a0 61f9 1663 4ac8 6413  F>.t.L..a..cJ.d.
+00001450: 4233 0e3f 4ab6 dd18 e87c 4b26 6781 64b2  B3.?J....|K&g.d.
+00001460: ce63 d729 5135 7f2d 9029 813b a698 409e  .c.)Q5.-.).;..@.
+00001470: 71d1 2742 72b2 98aa e1a2 4f04 14ae c5af  q.'Br.....O.....
+00001480: 9a40 9238 3392 58af df5c d750 eb68 bd08  .@.83.X..\.P.h..
+00001490: 314c 41b6 5e66 e272 150f c94d 081d 5b88  1LA.^f.r...M..[.
+000014a0: 0b56 2640 7572 ce56 f7c2 7652 b70e c5e9  .V&@ur.V..vR....
+000014b0: f30a 2492 3323 9235 2f7e 2846 ada3 bc84  ..$.3#.5/~(F....
+000014c0: 3ca6 20cb 6b2e e666 218f 4d08 ad59 6245  <. .k..f!.M..YbE
+000014d0: 3701 aa93 5c20 14b6 93ba 75a0 e9f3 0a24  7...\ ....u....$
+000014e0: 9be1 7eaf 3ae0 7267 2571 9448 3ea3 d484  ..~.:.rg%q.H>...
+000014f0: 7aa6 204b 4d9c fdd8 ac83 0ef2 d433 c7bc  z. KM........3..
+00001500: b301 ba8e d814 a12e 2a0f 2775 f361 e422  ........*.'u.a."
+00001510: 35bc 378c 376f 2fe5 6bf5 afb2 7dad cfdd  5.7.7o/.k...}...
+00001520: e408 f797 d515 5f28 e016 af05 ebbf e166  ......_(.......f
+00001530: b3b6 c2ac f7dc f470 41d8 7c7a 838b e415  .......pA.|z....
+00001540: 5cc3 9cc5 b060 bf34 4d6f 3ec0 9750 797f  \....`.4Mo>..Py.
+00001550: adfa f7cb a469 6bb8 3aac ef86 afa2 4bd3  .....ik.:.....K.
+00001560: f66d 59f7 70b9 17ec 7f34 d070 dc5c 6ab8  .mY.p....4.p.\j.
+00001570: adbb 008d 0f57 e0fb 1a6e 4c0f 96f6 be86  .....W...nL.....
+00001580: 5bd1 ed87 43a2 7fb7 b3f7 dd1f ff04 0000  [...C...........
+00001590: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+000015a0: 2100 e158 495a 2a07 0000 5f21 0000 1800  !..XIZ*..._!....
+000015b0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+000015c0: 7368 6565 7432 2e78 6d6c ac9a 5b73 9b46  sheet2.xml..[s.F
+000015d0: 14c7 df3b d3ef c0f0 1e24 d0c5 96c6 72a6  ...;.....$....r.
+000015e0: b22e 64a6 cd74 9a5e 9e31 4216 0d68 55c0  ..d..t.^.1B..hU.
+000015f0: 769c 4fdf b39c b3cb ee59 85a6 33f8 2191  v.O......Y..3.!.
+00001600: ce8d e5c7 d9e5 0fab bbf7 5fca c27b c9aa  .........._..{..
+00001610: 3a17 e795 1f06 63df cbce a938 e4e7 a795  :.....c....8....
+00001620: ffc7 efbb 77b7 be57 37c9 f990 14e2 9cad  ....w..W7.......
+00001630: fcb7 acf6 dfdf fff8 c3dd aba8 3ed7 a72c  ............>..,
+00001640: 6b3c a870 ae57 fea9 692e cbd1 a84e 4f59  k<.p.W..i....NOY
+00001650: 99d4 81b8 6467 f01c 4555 260d 7cad 9e46  ....dg..EU&.|..F
+00001660: f5a5 ca92 439b 5416 a368 3c9e 8fca 243f  ....C.T..h<...$?
+00001670: fb58 6159 7d4f 0d71 3ce6 69b6 11e9 7399  .XaY}O.q<.i...s.
+00001680: 9d1b 2c52 6545 d2c0 f8eb 537e a955 b532  ..,ReE....S~.U.2
+00001690: fd9e 7265 527d 7ebe bc4b 4579 8112 8f79  ..reR}~..KEy...y
+000016a0: 9137 6f6d 51df 2bd3 e587 a7b3 a892 c702  .7omQ.+.........
+000016b0: cefb 4b38 4d52 55bb fde2 942f f3b4 12b5  ..K8MRU..../....
+000016c0: 3836 0194 1be1 40dd 735e 8c16 23a8 747f  86....@.s^..#.t.
+000016d0: d772 f8b5 f200 76f6 3129 e118 b1f8 3b99  .r....v.1)....;.
+000016e0: f8a3 fbbb 430e 2727 af88 5765 c795 ff53  ....C.''..We...S
+000016f0: b88c a3b9 74b4 397f e6d9 6b6d 7cf6 1a71  ....t.9...km|..q
+00001700: f939 3b36 0f59 5140 f08d ef7d 15a2 fc94  .9;6.YQ@...}....
+00001710: 2672 dc0b b8a0 faeb 4779 3120 461a e5f5  &r......Gy1 F...
+00001720: 7b14 e2b3 acf6 e1b0 f2c7 7248 5991 a592  {.........rHY...
+00001730: a497 c07f 2f19 567c 0865 0ffc d30e 457e  ..../.V|.e....E~
+00001740: 8671 8cf4 40cc cf6a 50bb f69a c3a9 3d26  .q..@..jP.....=&
+00001750: 75f6 208a bff2 4373 82e6 82a3 1eb2 63f2  u. ...Cs......c.
+00001760: 5c34 bf89 d738 cb9f 4e0d 58e7 c1cc f7d2  \4...8..N.X.....
+00001770: e7ba 11a5 b601 68c9 7b79 78db 6475 0a17  ......h.{yx.du..
+00001780: 1ac6 1744 f2c8 a928 e030 f0af 57e6 b261  ...D...(.0..W..a
+00001790: e13a 255f 6495 c9ed 144e 8a8e 1406 d368  .:%_d....N.....h
+000017a0: 7673 1b46 50ba 6ede 2488 16ec 08d3 dbd1  vs.FP.n.$.......
+000017b0: 6f92 26b9 bfab c4ab 078d 0775 ea4b 22db  o.&........u.K".
+000017c0: 385c c2d9 fedf 81c1 8864 959f 6419 7928  8\.......d..d.y(
+000017d0: 0f06 5c03 d097 fbd9 f46e f402 9052 0a59  ..\......n...R.Y
+000017e0: 6308 8c4b 878c ed88 0737 22b4 2336 6e44  c..K.....7".#6nD
+000017f0: 6447 6cdd 8889 1db1 7323 d848 f76e c4cc  dGl.....s#.H.n..
+00001800: ae11 bb11 731d 3102 b21a 6f34 0c5e 5966  ....s.1...o4.^Yf
+00001810: e547 2d58 76c6 6bf4 995c 6f18 5715 212f  .G-Xv.k..\o.W.!/
+00001820: 0b27 8abe 795b 399c 86c1 7c61 fe31 b8aa  .'..y[9...|a.1..
+00001830: 906c 4779 d977 68b8 c16c 7639 f73c 3a36  .lGy.wh..lv9.<:6
+00001840: 0c16 2468 9b21 7a50 9651 90d8 455f a3af  ..$h.!zP.Q..E_..
+00001850: 0f92 8ab8 0609 7d04 49ce 5bc6 45e5 6a2e  ......}.I.[.E.j.
+00001860: 6840 2e0b 3b78 cf83 63c3 6061 8169 3d04  h@..;x..c.`a.i=.
+00001870: 1659 4662 e9e6 5dc4 c6bf c690 3e3a 2ae2  .YFb..].....>:*.
+00001880: 1a1d f411 9d68 1e74 53a1 6d92 adca d574  .....h.tS.m....t
+00001890: d080 7458 afee 7970 6c18 2c3a 7281 1b60  ..tX..ypl.,:r..`
+000018a0: e192 6554 d3f0 150b 7d7d 5854 c435 2ce8  ..eT....}}XT.5,.
+000018b0: 5358 6e02 d607 5b95 abb1 a001 b1b0 fedd  SXn...[.........
+000018c0: f3e0 d830 5858 e6c3 6091 6558 d3b0 cbba  ...0XX..`.eX....
+000018d0: c690 3e3a 2ae2 1a1d f411 9dc9 2408 fbd6  ..>:*.......$...
+000018e0: 1d55 48a3 4203 a262 e3da f3e0 d830 58a8  .UH.B..b.....0X.
+000018f0: 402f 0cd1 41b2 8cea 203e b1d0 d7c7 4845  @/..A... >....HE
+00001900: a853 dba0 01c1 4437 ce52 c3e3 7768 a025  .S....D7.R..wh.%
+00001910: 98af 353c 3a36 0c16 0b29 7406 984d b28c  ..5<:6...)t..M..
+00001920: 62c1 fb05 7d7d 2c54 8466 8106 6431 0903  b...}},T.f..d1..
+00001930: 76ef daf2 f81d 1a88 05ef 0b1e 1d1b 068b  v...............
+00001940: c562 1816 b28c 62c1 56b9 35fa fa58 a888  .b....b.V.5..X..
+00001950: 6b73 077d 6a65 9905 6cb1 d8aa 5c3d 5dd0  ks.}je..l...\=].
+00001960: 405c b8da e1d1 b161 b0b8 4819 3b88 5694  @\.....a..H.;.V.
+00001970: 7514 995b ae12 d1d9 87a6 1dc7 ca9f a1ea  u..[............
+00001980: e00a 11f3 159c dbfe 8545 97d2 a8c8 42ac  .........E....B.
+00001990: 98d6 da3b f1b1 69b1 690d a5ac 516b 5af7  ...;..i.i...QkZ.
+000019a0: 6fde 4ea1 ab47 b906 d421 d71a 8a9c 6a35  o.N..G...!....j5
+000019b0: 6642 6eab 733b 4a78 40a4 c416 bdbd 131e  fBn.s;Jx@.......
+000019c0: 9b16 1bd2 40fa 3834 0532 5b04 d7e4 ec6d  ....@.84.2[....m
+000019d0: a93e 894c f944 67ec aec9 fa00 1d1f 5318  .>.L.Dg.......S.
+000019e0: 3b4d e408 63b3 80cd 6720 691c 2a6d 6c88  ;M..c...g i.*ml.
+000019f0: 4067 e6fd b746 a632 df98 7996 4a9e 4d03  @g...F.2..y.J.M.
+00001a00: b6d0 6c75 7687 c9d4 c9ce 5398 2394 cd02  ..luv.....S.#...
+00001a10: 36a6 81a4 72a8 b472 3b49 d834 5893 b7b7  6...r..r;I.4X...
+00001a20: 8fb8 7cdd 5012 35cf 2298 8fcd 3f7e 47d3  ..|.P.5."...?~G.
+00001a30: 87e8 1099 6239 e2f7 7727 3e36 2d36 23a9  ....b9..w'>6-6#.
+00001a40: 1887 78d2 47e5 89cf a221 3b81 75a8 7469  ..x.G....!;.u.ti
+00001a50: d768 ce4a c4b5 ec86 92d4 43a8 739f d745  .h.J......C.s..E
+00001a60: 3b2a a656 e68f 337b 273e 362d 3695 81f4  ;*.V..3{'>6-6...
+00001a70: 72a8 0473 db39 fc11 9dbc bd9d c365 eb86  r..s.9.......e..
+00001a80: 92d4 53a7 3b9d 1c55 4c19 b82a 47ec d2ec  ..S.;..UL..*G...
+00001a90: f520 14c5 d8b4 d854 0692 c621 cacd dbab  . .....T...!....
+00001aa0: ef2d c809 6a43 bf10 624b d283 0eb9 7ad3  .-..jC..bK....z.
+00001ab0: c2e2 7003 96de 9b60 c265 90ce eeda 8652  ..p....`.e.....R
+00001ac0: 4294 0e0e 2174 2fda d76d f2fd 466c 96b0  B...!t/..m..Fl..
+00001ad0: 090d 2498 db37 8c2b 1f09 f1a7 0772 f612  ..$..7.+.....r..
+00001ae0: 4211 db0d 7943 4984 6512 4cf8 e3b8 aeda  B...yCI.e.L.....
+00001af0: 61c1 2270 9796 2423 fe1e c749 884d 8b8d  a."p..$#...I.M..
+00001b00: 6520 ed1c a206 8571 e9de 70ee ea18 d20b  e .....q..p.....
+00001b10: 4785 e807 0aaa 4b70 a260 eef4 0c4f d9a9  G.....Kp.`...O..
+00001b20: 14ea 19fe be82 dc66 cf18 252c 38d1 40fa  .......f..%,8.@.
+00001b30: b9ad 237b a683 13f2 7b15 c5f4 d1d1 219a  ..#{....{.....!.
+00001b40: 0e59 349d c87a 265f b0d9 b975 0aec 5401  .Y4..z&_...u..T.
+00001b50: 62c5 12f6 4e42 6c5a 6c56 03a9 e708 852a  b...NBlZlV.....*
+00001b60: ce2f 2e9b c9d9 0b09 f317 579f 3528 9f78  ./........W.5(.x
+00001b70: cd82 0557 3cfa 007a aaa9 1422 c4a5 b393  ...W<..z..."....
+00001b80: 109b 169b d050 af96 518d 2221 ae09 2374  .....P..Q."!..#t
+00001b90: f612 5221 57df 2ea3 9308 c18b 5387 90ca  ..R!W.......S...
+00001ba0: ee08 510a 11e2 2fc2 f488 f45d ccb4 d884  ..Q.../....]....
+00001bb0: 0612 cf11 0a51 24c4 9721 72f6 12c2 fc6f  .....Q$..!r....o
+00001bc0: f410 3af5 5d6c ccdf 2deb 0374 8428 8508  ..:.]l..-..t.(..
+00001bd0: b1d7 cb4e 7c6c 5a6c 4003 c9e6 0835 2a02  ...N|lZl@....5*.
+00001be0: 7297 22f4 f612 5221 dd52 8416 c202 af7e  r."...R!.R.....~
+00001bf0: 66f6 5ac4 3726 7881 1d8d 89ee 6913 676f  f.Z.7&x.....i.go
+00001c00: 4225 c8ae 9d30 2110 5332 5eb1 49a7 e66c  B%...0!.S2^.I..l
+00001c10: 7a03 09ea 76ab 4e49 0047 5093 b797 1e8a  z...v.NI.GP.....
+00001c20: 6143 0350 d2b7 6f73 ba6a d754 5844 6900  aC.P..os.j.TXDi.
+00001c30: fef2 4c27 b40a 812d a4b1 eded 1611 9bd7  ..L'...-........
+00001c40: 4052 1b36 84e5 eb23 ea36 6737 0cbd bdbc  @R.6...#.6g7....
+00001c50: 5448 d76d 68d1 bca6 ce32 c553 7634 0ac5  TH.mh....2.Sv4..
+00001c60: 8b3f e393 1b3b 2862 8b98 dcd3 96a7 40de  .?...;(b......@.
+00001c70: ee60 c80b f798 7197 f692 3c65 bf24 d553  .`....q...<e.$.S
+00001c80: 7eae bd02 b6ba e576 30a8 d40a b790 dbcf  ~......v0.......
+00001c90: b009 de5a e102 3e8a 0636 93d5 b713 fce6  ...Z..>..6......
+00001ca0: 2003 153b 0e60 c138 0ad1 a82f 70de b2ee   ..;.`.8.../p...
+00001cb0: a7ac 79be 78a2 ca61 9bb9 fd19 c1ca bf88  ..y.x..a........
+00001cc0: aaa9 92bc 818d 60b0 7f15 e028 3697 1c76  ......`....(6..v
+00001cd0: 76e7 205e e0d7 124d 0ebb eb9d a55a e6b0  v. ^...M.....Z..
+00001ce0: 835e 7d38 84ed e6b8 fe69 c4fd bf00 0000  .^}8.....i......
+00001cf0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+00001d00: 2100 3b6d 324b c100 0000 4201 0000 2300  !.;m2K....B...#.
+00001d10: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00001d20: 5f72 656c 732f 7368 6565 7431 2e78 6d6c  _rels/sheet1.xml
+00001d30: 2e72 656c 7384 8fc1 8ac2 3014 45f7 03fe  .rels.....0.E...
+00001d40: 4378 7b93 d685 0c43 5337 22b8 55e7 0362  Cx{....CS7".U..b
+00001d50: fada 06db 9790 f714 fd7b b31c 65c0 e5e5  .........{..e...
+00001d60: 70cf e536 9bfb 3ca9 1b66 0e91 2cd4 ba02  p..6..<..f..,...
+00001d70: 85e4 6317 68b0 f07b da2d bf41 b138 eadc  ..c.h..{.-.A.8..
+00001d80: 1409 2d3c 9061 d32e be9a 034e 4e4a 89c7  ..-<.a.....NNJ..
+00001d90: 9058 150b b185 5124 fd18 c37e c4d9 b18e  .X....Q$...~....
+00001da0: 09a9 903e e6d9 4989 7930 c9f9 8b1b d0ac  ...>..I.y0......
+00001db0: aa6a 6df2 5f07 b42f 4eb5 ef2c e47d 5783  .jm._../N..,.}W.
+00001dc0: 3a3d 5259 feec 8e7d 1f3c 6ea3 bfce 48f2  :=RY...}.<n...H.
+00001dd0: cf84 4939 9060 3ea2 4839 c845 edf2 8062  ..I9.`>.H9.E...b
+00001de0: 41eb 77f6 9e6b 7d0e 04a6 6dcc cbf3 f609  A.w..k}...m.....
+00001df0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00001e00: 0000 2100 13c4 2c13 c200 0000 4201 0000  ..!...,.....B...
+00001e10: 2300 0000 786c 2f77 6f72 6b73 6865 6574  #...xl/worksheet
+00001e20: 732f 5f72 656c 732f 7368 6565 7432 2e78  s/_rels/sheet2.x
+00001e30: 6d6c 2e72 656c 7384 8fc1 6ac3 3010 44ef  ml.rels...j.0.D.
+00001e40: 85fc 83d8 7b24 3b87 508a 255f 4a21 d726  ....{$;.P.%_J!.&
+00001e50: fd00 455e dba2 f64a 68b7 25f9 fbe8 d884  ..E^...Jh.%.....
+00001e60: 428e c363 de30 5d7f 5917 f58b 8563 220b  B..c.0].Y....c".
+00001e70: ad6e 4021 8534 449a 2c7c 9d3e b6af a058  .n@!.4D.,|.>...X
+00001e80: 3c0d 7e49 8416 aec8 d0bb cd4b f789 8b97  <.~I.......K....
+00001e90: 5ae2 3966 56d5 426c 6116 c96f c670 9871  Z.9fV.Bla..o.p.q
+00001ea0: f5ac 5346 aa64 4c65 f552 6399 4cf6 e1db  ..SF.dLe.Rc.L...
+00001eb0: 4f68 764d b337 e5af 03dc 9d53 1d06 0be5  OhvM.7.....S....
+00001ec0: 30b4 a04e d75c 979f bbd3 38c6 80ef 29fc  0..N.\....8...).
+00001ed0: ac48 f2cf 84c9 2592 6039 a248 3dc8 55ed  .H....%.`9.H=.U.
+00001ee0: cb84 6241 eb47 f698 77fa 1c09 8ceb ccdd  ..bA.G..w.......
+00001ef0: 7377 0300 00ff ff03 0050 4b03 0414 0006  sw.......PK.....
+00001f00: 0008 0000 0021 0034 a109 92c2 0000 0042  .....!.4.......B
+00001f10: 0100 0023 0000 0078 6c2f 776f 726b 7368  ...#...xl/worksh
+00001f20: 6565 7473 2f5f 7265 6c73 2f73 6865 6574  eets/_rels/sheet
+00001f30: 332e 786d 6c2e 7265 6c73 848f c16a c330  3.xml.rels...j.0
+00001f40: 1044 ef81 fc83 d87b 2427 8552 82e5 5c42  .D.....{$'.R..\B
+00001f50: 20d7 36fd 0055 5ecb 22f6 4a68 b7a5 f9fb   .6..U^.".Jh....
+00001f60: ea58 9b42 8fc3 63de 30ed e97b 9ed4 1716  .X.B..c.0..{....
+00001f70: 8e89 2cec 7503 0ac9 a73e 52b0 f07e bbec  ..,.u....>R..~..
+00001f80: 5e40 b138 eadd 9408 2d3c 90e1 d46d 37ed  ^@.8....-<...m7.
+00001f90: 2b4e 4e6a 89c7 9859 550b b185 5124 1f8d  +NNj...YU...Q$..
+00001fa0: 613f e2ec 58a7 8c54 c990 caec a4c6 124c  a?..X..T.......L
+00001fb0: 76fe ee02 9a43 d33c 9bf2 db01 ddc2 a9ae  v....C.<........
+00001fc0: bd85 72ed f7a0 6e8f 5c97 ff77 a761 881e  ..r...n.\..w.a..
+00001fd0: cfc9 7fce 48f2 c784 c925 9260 7943 917a  ....H....%.`yC.z
+00001fe0: 90ab da95 8062 41eb 355b e727 fd11 094c  .....bA.5[.'...L
+00001ff0: d79a c5f3 ee07 0000 ffff 0300 504b 0304  ............PK..
+00002000: 1400 0600 0800 0000 2100 4396 11a3 c200  ........!.C.....
+00002010: 0000 4201 0000 2300 0000 786c 2f77 6f72  ..B...#...xl/wor
+00002020: 6b73 6865 6574 732f 5f72 656c 732f 7368  ksheets/_rels/sh
+00002030: 6565 7434 2e78 6d6c 2e72 656c 7384 8fc1  eet4.xml.rels...
+00002040: 6ac3 3010 44ef 81fc 83d8 7b24 2794 5282  j.0.D.....{$'.R.
+00002050: e55c 4220 d736 fd00 555e cb22 f64a 68b7  .\B .6..U^.".Jh.
+00002060: a5f9 fbea 589b 428f c363 de30 ede9 7b9e  ....X.B..c.0..{.
+00002070: d417 168e 892c ec75 030a c9a7 3e52 b0f0  .....,.u....>R..
+00002080: 7ebb ec5e 40b1 38ea dd94 082d 3c90 e1d4  ~..^@.8....-<...
+00002090: 6d37 ed2b 4e4e 6a89 c798 5955 0bb1 8551  m7.+NNj...YU...Q
+000020a0: 241f 8d61 3fe2 ec58 a78c 54c9 90ca eca4  $..a?..X..T.....
+000020b0: c612 4c76 feee 029a 43d3 3c9b f2db 01dd  ..Lv....C.<.....
+000020c0: c2a9 aebd 8572 edf7 a06e 8f5c 97ff 77a7  .....r...n.\..w.
+000020d0: 6188 1ecf c97f ce48 f2c7 84c9 2592 6079  a......H....%.`y
+000020e0: 4391 7a90 abda 9580 6241 eb35 5be7 27fd  C.z.....bA.5[.'.
+000020f0: 1109 4cd7 9ac5 f3ee 0700 00ff ff03 0050  ..L............P
+00002100: 4b03 0414 0006 0008 0000 0021 0064 f334  K..........!.d.4
+00002110: 22c2 0000 0042 0100 0023 0000 0078 6c2f  "....B...#...xl/
+00002120: 776f 726b 7368 6565 7473 2f5f 7265 6c73  worksheets/_rels
+00002130: 2f73 6865 6574 352e 786d 6c2e 7265 6c73  /sheet5.xml.rels
+00002140: 848f c16a c330 1044 ef81 fc83 d87b 2427  ...j.0.D.....{$'
+00002150: d052 82e5 5c42 20d7 36fd 0055 5ecb 22f6  .R..\B .6..U^.".
+00002160: 4a68 b7a5 f9fb ea58 9b42 8fc3 63de 30ed  Jh.....X.B..c.0.
+00002170: e97b 9ed4 1716 8e89 2cec 7503 0ac9 a73e  .{......,.u....>
+00002180: 52b0 f07e bbec 5e40 b138 eadd 9408 2d3c  R..~..^@.8....-<
+00002190: 90e1 d46d 37ed 2b4e 4e6a 89c7 9859 550b  ...m7.+NNj...YU.
+000021a0: b185 5124 1f8d 613f e2ec 58a7 8c54 c990  ..Q$..a?..X..T..
+000021b0: caec a4c6 124c 76fe ee02 9a43 d33c 9bf2  .....Lv....C.<..
+000021c0: db01 ddc2 a9ae bd85 72ed f7a0 6e8f 5c97  ........r...n.\.
+000021d0: ff77 a761 881e cfc9 7fce 48f2 c784 c925  .w.a......H....%
+000021e0: 9260 7943 917a 90ab da95 8062 41eb 355b  .`yC.z.....bA.5[
+000021f0: e727 fd11 094c d79a c5f3 ee07 0000 ffff  .'...L..........
+00002200: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00002210: 4c5a 2a7a c200 0000 4201 0000 2300 0000  LZ*z....B...#...
+00002220: 786c 2f77 6f72 6b73 6865 6574 732f 5f72  xl/worksheets/_r
+00002230: 656c 732f 7368 6565 7436 2e78 6d6c 2e72  els/sheet6.xml.r
+00002240: 656c 7384 8fc1 6ac3 3010 44ef 85fc 83d8  els...j.0.D.....
+00002250: 7b24 a707 538a e55c 4a20 d726 fd00 555e  {$..S..\J .&..U^
+00002260: dba2 f64a 6837 21fe fbe8 589b 428f c363  ...Jh7!...X.B..c
+00002270: de30 cdf1 314f ea8e 9943 240b 075d 8142  .0..1O...C$..].B
+00002280: f2b1 0b34 58f8 ba9e f66f a058 1c75 6e8a  ...4X....o.X.un.
+00002290: 8416 1664 38b6 bb97 e613 2727 a5c4 6348  ...d8.....''..cH
+000022a0: ac8a 85d8 c228 92de 8d61 3fe2 ec58 c784  .....(...a?..X..
+000022b0: 5448 1ff3 eca4 c43c 98e4 fc8f 1bd0 bc56  TH.....<.......V
+000022c0: 556d f26f 07b4 2ba7 3a77 16f2 b93b 80ba  Um.o..+.:w...;..
+000022d0: 2ea9 2cff ef8e 7d1f 3c7e 447f 9b91 e48f  ..,...}.<~D.....
+000022e0: 0993 7220 c17c 4191 7290 8bda e501 c582  ..r .|A.r.......
+000022f0: d65b b6cd b5fe 0e04 a66d ccea 79fb 0400  .[.......m..y...
+00002300: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00002310: 0021 006b 3f0f fbc3 0000 0042 0100 0023  .!.k?......B...#
+00002320: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00002330: 2f5f 7265 6c73 2f73 6865 6574 372e 786d  /_rels/sheet7.xm
+00002340: 6c2e 7265 6c73 848f c16a c330 1044 ef81  l.rels...j.0.D..
+00002350: fc83 d87b 2427 87b6 04cb b984 40ae 6dfa  ...{$'......@.m.
+00002360: 01aa bc96 45ec 95d0 6e4b f3f7 d5b1 3685  ....E...nK....6.
+00002370: 1e87 c7bc 61da d3f7 3ca9 2f2c 1c13 59d8  ....a...<./,..Y.
+00002380: eb06 1492 4f7d a460 e1fd 76d9 bd80 6271  ....O}.`..v...bq
+00002390: d4bb 2911 5a78 20c3 a9db 6eda 579c 9cd4  ..).Zx ...n.W...
+000023a0: 128f 31b3 aa16 620b a348 3e1a c37e c4d9  ..1...b..H>..~..
+000023b0: b14e 19a9 9221 95d9 498d 2598 ecfc dd05  .N...!..I.%.....
+000023c0: 3487 a679 32e5 b703 ba85 535d 7b0b e5da  4..y2.....S]{...
+000023d0: ef41 dd1e b92e ffef 4ec3 103d 9e93 ff9c  .A......N..=....
+000023e0: 91e4 8f09 934b 24c1 f286 22f5 2057 b52b  .....K$...". W.+
+000023f0: 01c5 82d6 6bb6 cecf fa23 1298 ae35 8be7  ....k....#...5..
+00002400: dd0f 0000 00ff ff03 0050 4b03 0414 0006  .........PK.....
+00002410: 0008 0000 0021 00a2 341a 18c2 0000 0042  .....!..4......B
+00002420: 0100 0023 0000 0078 6c2f 776f 726b 7368  ...#...xl/worksh
+00002430: 6565 7473 2f5f 7265 6c73 2f73 6865 6574  eets/_rels/sheet
+00002440: 382e 786d 6c2e 7265 6c73 848f c18a c230  8.xml.rels.....0
+00002450: 1445 f782 ff10 de7e 92ea 6210 69ea 4606  .E.....~..b.i.F.
+00002460: ba75 f403 62fa da06 db97 90f7 6698 fefd  .u..b.......f...
+00002470: 64a9 22b8 bc1c eeb9 dcfa f037 4fea 1733  d."........7O..3
+00002480: 8748 1636 ba02 85e4 6317 68b0 7039 7f7d  .H.6....c.h.p9.}
+00002490: ec40 b138 eadc 1409 2d2c c870 68d6 abfa  .@.8....-,.ph...
+000024a0: 8493 9352 e231 2456 c542 6c61 1449 7b63  ...R.1$V.Bla.I{c
+000024b0: d88f 383b d631 2115 d2c7 3c3b 2931 0f26  ..8;.1!...<;)1.&
+000024c0: 397f 7303 9a6d 557d 9a7c ef80 e6c1 a9da  9.s..mU}.|......
+000024d0: ce42 6ebb 0da8 f392 caf2 7b77 ecfb e0f1  .Bn.......{w....
+000024e0: 18fd cf8c 242f 264c ca81 04f3 378a 9483  ....$/&L....7...
+000024f0: 5cd4 2e0f 2816 b47e 66cf 79a7 af81 c034  \...(..~f.y....4
+00002500: b579 78de fc03 0000 ffff 0300 504b 0304  .yx.........PK..
+00002510: 1400 0600 0800 0000 2100 962f 4caa d009  ........!../L...
+00002520: 0000 bf34 0000 1800 0000 786c 2f77 6f72  ...4......xl/wor
+00002530: 6b73 6865 6574 732f 7368 6565 7433 2e78  ksheets/sheet3.x
+00002540: 6d6c ac9b 4b73 e336 12c7 efa9 daef c0e2  ml..Ks.6........
+00002550: 3d94 48ea e9b2 9c8a ac07 e790 546a b38f  =.H.........Tj..
+00002560: 332d d136 7724 5121 e9f1 4c3e 7d00 7603  3-.6w$Q!..L>}.v.
+00002570: 6c74 2bf4 6c15 e6e0 b11a dd4d e8c7 06f0  lt+.l......M....
+00002580: 0768 deff f4f5 7c0a be14 7553 5697 5518  .h....|...uSV.U.
+00002590: 47e3 3028 2e87 ea58 5e5e 56e1 bfff b5fb  G.0(...X^^V.....
+000025a0: 7111 064d 9b5f 8ef9 a9ba 14ab f05b d184  q..M._.......[..
+000025b0: 3f3d fce3 87fb f7aa fedc bc16 451b a80c  ?=..........E...
+000025c0: 9766 15be b6ed f56e 346a 0eaf c539 6fa2  .f.....n4j...9o.
+000025d0: ea5a 5c54 cb73 559f f356 7dac 5f46 cdb5  .Z\T.sU..V}._F..
+000025e0: 2ef2 6317 743e 8d92 f178 363a e7e5 2584  ..c.t>...x6:..%.
+000025f0: 0c77 f5f7 e4a8 9e9f cb43 b1a9 0e6f e7e2  .w.......C...o..
+00002600: d242 92ba 38e5 adea 7ff3 5a5e 1b93 ed7c  .B..8.....Z^...|
+00002610: f89e 74e7 bcfe fc76 fdf1 509d af2a c553  ..t....v..P..*.S
+00002620: 792a db6f 5dd2 3038 1fee 3ebd 5caa 3a7f  y*.o].08..>.\.:.
+00002630: 3aa9 effd 359e e407 93bb fb20 d29f cb43  :...5...... ...C
+00002640: 5d35 d573 1ba9 7423 e8a8 fcce cbd1 72a4  ]5.s..t#......r.
+00002650: 323d dc77 1c7e ab03 05bb f835 3fab 6b64  2=.w.~.....5?.kd
+00002660: d5ff f224 1c3d dc1f 4bf5 e5f4 1d09 eae2  ...$.=..K.......
+00002670: 7915 fe1c df65 9389 6ee8 62fe 5316 ef0d  y....e..n.b.S...
+00002680: f93d f8b3 aace bf1f 72dd cda5 ba7f f6e3  .=......r.......
+00002690: af9a fd09 8cfa 763d 55d5 671d fce9 b80a  ......v=U.g.....
+000026a0: c7ba 07c5 a938 6870 41ae fefb 523c 1627  .....8hpA...R<.'
+000026b0: e5fd 18eb 5bfe 4777 65fd bbba ecc8 5e97  ....[.Gwe.....^.
+000026c0: fe6e fab0 eb6e b1fa 264f 7953 3c56 a7ff  .n...n..&OyS<V..
+000026d0: 96c7 f655 d592 eaca b178 cedf 4eed 3fab  ...U.....x..N.?.
+000026e0: f7ac 285f 5e5b 659d 45d3 3038 bc35 6d75  ..(_^[e.E.08.5mu
+000026f0: b636 c555 e3bd 3b7e db14 cd41 dd57 d5bf  .6.U..;~...A.W..
+00002700: a823 71a8 4eea 32ea 6770 2e75 7daa db92  .#q.N.2.gp.u}...
+00002710: 7fd5 59d2 c524 0cde f14a 7134 49a6 f345  ..Y..$...Jq4I..E
+00002720: 9ca8 d44d fb4d 8348 bb7e 4378 d7fb 4dde  ...M.M.H.~Cx..M.
+00002730: e60f f775 f51e a83a 5379 9a6b aeab 36be  ...u...:Sy.k..6.
+00002740: 53df f6ff ed98 ea91 cef2 b34e a32f 15a8  S..........N./..
+00002750: 0e37 0ae8 9787 e9e4 7ef4 4541 3aa0 cb1a  .7......~.EA:...
+00002760: 5c54 bfac cbd8 f578 941e b1eb b191 1e89  \T.....x........
+00002770: ebb1 951e a9eb b193 1eac a77b e931 7573  ...........{.1us
+00002780: 64d2 6366 3d46 8aac c59b f8c1 abd3 acc2  d.cf=F..........
+00002790: a403 cb98 aca1 8d72 9d33 aec6 43df 164e  .......r.3..C..N
+000027a0: 14da 6690 3949 22ce d3c4 aada efee f40e  ..f.9I".........
+000027b0: 0cf3 2e80 39ef b973 460c 0e16 5528 3eaa  ....9..sF...U(>.
+000027c0: 4ea7 3158 585f d6d0 3684 c578 dcc2 026d  N.1XX_..6..x...m
+000027d0: 06cb 4460 31b1 160b 1800 0bab 963d 77ce  ..D`1........=w.
+000027e0: 88c1 c1a2 06b2 0f2c 3a8d c1c2 aa7f 0d6d  .......,:......m
+000027f0: 4358 8cc7 2d2c d066 b02c 22f6 4db7 26d6  CX..-,.f.,".M.&.
+00002800: 6201 0360 e987 4857 497b ee9c 1183 8345  b..`..HWI{.....E
+00002810: cf65 1ee6 289d c660 e193 13b4 0d61 311e  .e..(..`.....a1.
+00002820: b7b0 401b 6251 f33a 1f44 26d6 6201 0360  ..@.bQ.:.D&.b..`
+00002830: 6177 68cf 9d33 6270 b0cc fc60 d169 0c16  awh..3bp...`.i..
+00002840: 763f d7d0 3684 c578 dcc2 026d 8865 9244  v?..6..x...m.e.D
+00002850: f192 fe63 13b7 4964 1981 0118 b119 6dcf  ...c..Id......m.
+00002860: 9d33 6270 18cd fd30 d269 0c23 56c6 6b68  .3bp...0.i.#V.kh
+00002870: 1b62 643c 6e31 8236 6494 26d1 624c feb1  .bd<n1.6d.&.bL..
+00002880: c97a 6b12 5946 6000 467c 15e3 ce19 3138  .zk.YF`.F|....18
+00002890: 8cb4 c8f1 30bc 741a c388 ddaf 35b4 0d31  ....0.t.....5..1
+000028a0: 321e e6ab 6dc0 0060 a671 b464 e5c2 fd77  2...m..`.q.d...w
+000028b0: 6000 1431 03b7 e7de 1931 382c 967e 58e8  `..1.....18,.~X.
+000028c0: 3486 c582 e920 681b 6261 3c2c 0b30 008b  4.... h.ba<,.0..
+000028d0: d938 e265 c1fd 7760 4016 7c91 e6de 1931  .8.e..w`@.|....1
+000028e0: 382c b46c f5a2 0d75 1eab 5e98 e85b 7757  8,.l...u..^..[wW
+000028f0: 5985 433c accb ad01 848d 3882 66cb 88cd  Y.C<......8.f...
+00002900: a75b 1b6d 470d 5a70 fae5 b522 fc33 6a71  .[.mG.Zp...".3jq
+00002910: 09f9 52cf a027 51df 7181 174b b5c9 159e  ..R..'Q.q..K....
+00002920: 75b1 2583 16c0 a2e6 5ebe 528b 881d 5a90  u.%.....^.R...Z.
+00002930: 0ad7 30c2 3fa3 1697 8a27 d11b 3baa 97eb  ..0.?....'..;...
+00002940: 3b6c 1dac 1bae 4737 1804 54e6 f368 eaac  ;l....G7..T..h..
+00002950: 486c 06dd da4b f495 43d5 6fca 576e e19f  Hl...K..C.o.Wn..
+00002960: 518b cbc8 9302 8ea9 048e b9d8 c3d6 4146  Q.............AF
+00002970: 5c9c 6e30 082b 6721 c48c 4dda 53a1 e237  \.n0.+g!..M.S..7
+00002980: 1695 23e4 2fcd e052 f124 8063 aa80 63b1  ..#./..R.$.c..c.
+00002990: 11fd 5803 6382 a9de 3a77 6275 8316 a092  ..X.c...:wbu....
+000029a0: c611 5301 5b11 b143 0bce c25c c108 ff8c  ..S.[..C...\....
+000029b0: 5a5c 2a5a 00fa d8a3 8390 c459 864b bdd8  Z\*Z.......Y.K..
+000029c0: c8cc 7e7f 2e66 192e 4d37 1804 5492 9958  ..~..f..M7..T..X
+000029d0: a56d d2be 56a8 f48d d9aa be17 fe19 b5b8  .m..V...........
+000029e0: 543c c9df 98ea df98 8b3b 6c1d 1c41 5c8c  T<.......;l..A\.
+000029f0: 6e30 c8ae d7e2 8c42 685d 8cc0 5d35 5fb1  n0.....Bh]..]5_.
+00002a00: 6d27 0cc5 8c5a 5c2a 9e04 6f4c 156f cce5  m'...Z\*..oL.o..
+00002a10: 1cb6 0e52 e1f2 7383 4176 4562 49b7 3669  ...R..s.AvEbI.6i
+00002a20: 5f2b 54de 264c 47ed 857f 462d 2e15 4f12  _+T.&LG...F-..O.
+00002a30: b73b 0fb4 4a86 0b3b 6c1d a422 642e 06a1  .;..J..;l.."d...
+00002a40: ce1d 4bf5 2284 2e46 60ad 88d9 5648 5ddb  ..K."..F`...VH].
+00002a50: 2dc5 d5a5 e249 ecc6 54ed 2642 df7d ac77  -....I..T.&B.}.w
+00002a60: 3101 9d6d a9e2 9d26 725e 1192 1773 e056  1..m...&r^...s.V
+00002a70: 4850 11a2 975e d3a1 9278 52bd 5d1e 7b38  HP...^...xR.].{8
+00002a80: 250e ed40 130f d50a 2698 de3a f4db 60a3  %..@....&..:..`.
+00002a90: d95b 8fc5 7a64 a3ed 6842 0bea 3b3e f30a  .[..zd..hB..;>..
+00002aa0: ff8c 5a5c 429e 546f 4255 6fc2 f51d b60e  ..Z\B.ToBUo.....
+00002ab0: 1232 c2f8 e6c1 2634 9ab3 aab9 3cd9 34d1  .2....&4....<.4.
+00002ac0: 3d21 b060 0db1 42de db0e d959 985a 5c42  =!.`..B....Y.Z\B
+00002ad0: be8e 7da9 024e b8ba 4bbe e3e4 5728 600c  ..}..N..K...W(`.
+00002ae0: c2b5 69f2 8102 b697 e819 5105 3ce1 7b27  ..i.......Q.<.{'
+00002af0: e19f 518b cbc8 9302 4e40 5e2e 6e9f 8d43  ..Q.....N@^.n..C
+00002b00: a31a fdf6 a103 9bb5 1f31 7e79 7b98 41bc  .........1~y{.A.
+00002b10: da00 ea12 9b47 5c1f 6c6d 740f 0843 e25b  .....G\.lmt..C.[
+00002b20: 09f7 c23f a316 1790 2731 9c80 dc05 4062  ...?....'1....@b
+00002b30: 9441 e320 20e3 7273 9441 630f 881d d3e0  .A.  .rs.Ac.....
+00002b40: c597 5648 efd0 a276 8f3a 1f5f d485 7f46  ..VH...v.:._...F
+00002b50: 2d2e 1f4f b2b8 7b54 b60a 818f 1863 2057  -..O..{T.....c W
+00002b60: 07f9 1897 9b7c a0d1 f249 f83e 1caf 4e01  .....|...I.>..N.
+00002b70: 6108 0012 f3b4 b95a 3f0b 118b 0bc8 9342  a......Z?......B
+00002b80: 4e40 ae02 20be 99c2 c641 4010 ff37 230c  N@.. ....A@..7#.
+00002b90: 1a11 d022 1af3 833e 7b81 7e84 6108 8e30  ..."...>{.~.a..0
+00002ba0: 314f 9bcb f584 88c5 25e4 492d 2720 5481  1O......%.I-' T.
+00002bb0: 1097 85d8 3848 08e2 fb22 d860 1062 49a3  ....8H...".`.bI.
+00002bc0: 85a8 1b1e b233 2188 851f 4ed8 6ef4 5848  .....3!...N.n.XH
+00002bd0: 0a17 8b27 b99c 8016 553f edec cb4f 66d7  ...'....U?...Of.
+00002be0: e833 4807 d250 3a60 413a 4934 e37b 099b  .3H..P:`A:I4.{..
+00002bf0: b52f 1a0c 013a 297f 1625 0232 6a71 e978  ./...:)..%.2jq.x
+00002c00: 92cd 0968 5287 8e98 9ec1 6790 8e71 b147  ...hR.....g..q.G
+00002c10: 1598 d8d6 0e67 be45 073a e740 129c 9453  .....g.E.:.@...S
+00002c20: 7e58 2102 326a 71e8 a49e e473 97c7 ccca  ~X!.2jq....s....
+00002c30: b178 b80b f279 880b 2620 5583 16e4 a29e  .x...y..& U.....
+00002c40: e9b2 91ba 1521 3b13 8255 c31f b188 808c  .....!;..U......
+00002c50: 5a5c 2e9e 4473 0a1a 15e5 0e5f aeb0 7590  Z\..Ds....._..u.
+00002c60: 0b24 a05c c082 5ce2 28e1 a3c9 66b5 a309  .$.\..\.(...f...
+00002c70: 2d58 2f5c 15ed 4540 462d 2e17 4f52 3905  -X/\..E@F-..OR9.
+00002c80: 5d8a 5cf8 2a85 ad83 5c20 01e5 0296 7e1c  ].\.*...\ ....~.
+00002c90: f139 d866 edb9 6008 cec1 5cdd 8880 8c5a  .9.f..`...\....Z
+00002ca0: 5c2e 9ee4 716a e431 9983 45d5 7cac 9231  \...qj.1..E.|..1
+00002cb0: 0da5 e348 63f5 7747 828e c9da d371 a431  ...Hc.wG.....q.1
+00002cc0: 3f29 d88b 6b64 d4e2 d2f1 a48d 53a3 8d09  ?)..kd......S...
+00002cd0: 1d51 3b1f 4b64 4c43 e938 ba38 8952 41c7  .Q;.KdLC.8.8.RA.
+00002ce0: 64ed e960 08d4 4ec2 b756 e21a 19b5 b874  d..`..N..V.....t
+00002cf0: 3c29 e314 9425 8e29 7e34 8aad 8363 8a8b  <)...%.)~4...c..
+00002d00: d50d 06d9 31b5 e44f eb6c d69e 8ba3 87f9  ....1..O.l......
+00002d10: 2e78 2f02 326a 71b9 7812 c4a9 11c4 a46a  .x/.2jq.x......j
+00002d20: f871 3afa 0cd2 e142 7583 4176 265e 8815  .q:....Bu.Av&^..
+00002d30: 8a87 ec4c 08ae 505c 0cdb 6e58 d547 2d2e  ...L..P\..nX.G-.
+00002d40: 1d4f 6238 3562 98d0 11b5 63a4 e7df efcb  .Ob85b....c.....
+00002d50: 310d 1d53 10d4 d3e1 5b05 11b2 430b ae53  1..S....[...C..S
+00002d60: 09df 4c89 808c 5a5c 3a9e 3471 7a43 13f3  ..L...Z\:.4qzC..
+00002d70: e375 f419 ac1d a189 31a8 5fad 041d 1eb2  .u......1._.....
+00002d80: 3321 38e3 70d5 67bb d1d7 0e49 e1d2 f1a4  3!8.p.g....I....
+00002d90: 89d3 1b9a 98ef a7d0 6790 8ed0 c418 6477  ........g.....dw
+00002da0: 0c73 fe4c c666 ede7 1d47 1327 7cc7 2002  .s.L.f...G.'|. .
+00002db0: 326a 71e8 4c3c 69e2 2e8f d6c4 6464 b1bb  2jq.L<i.....dd..
+00002dc0: bc46 9f21 3ad6 c5ee 18d0 62e9 2cb8 0214  .F.!:.....b.,...
+00002dd0: 213b 1302 b533 117f db67 04ba ad1d 9ac2  !;...3...g......
+00002de0: a5e3 4919 4f8c 32ee e988 8711 e833 4847  ..I.O.2......3HG
+00002df0: e863 0cb2 234b c0e1 113b 1381 70f8 c0b2  .c..#K...;..p...
+00002e00: bde8 e190 142e 1c4f f278 42e5 b138 6bc7  .......O.xB..8k.
+00002e10: d641 2c46 1edf fcb3 5047 294f c5e3 1a9b  .A,F....PG)O....
+00002e20: df0e 2eb4 e0c4 3ce1 1b2b 1190 518b 4bc8  ......<..+..Q.K.
+00002e30: 9350 9e48 a1cc 35d8 1a7d 0639 71d5 bbc1  .P.H..5..}.9q...
+00002e40: 20bb ed1c 8bfa 1142 d984 60fd f0e7 c1b6   ......B..`.....
+00002e50: 1b7d fd90 142e 1d4f 4259 bd74 a1ff 868b  .}.....OBY.t....
+00002e60: 4e3d b28a 3e16 ca98 862c ea68 b174 e2d4  N=..>....,.h.t..
+00002e70: f993 1cc1 4ac8 6693 0059 f163 2f71 45fd  ....J.f..Y.c/qE.
+00002e80: fe88 fe2a 5d1f 8015 bcd4 01af 455c f397  ...*].......E\..
+00002e90: e297 bc7e 292f 4d70 2a9e bbf7 2f94 eea8  ...~)/Mp*.../...
+00002ea0: e19d 8d71 a47e 6fab ab7e 2b63 ae74 e953  ...q.~o..~+c.t.S
+00002eb0: d5aa b737 cca7 57f5 4e4f a1de 8650 4f71  ...7..W.NO...POq
+00002ec0: c3e0 b9aa 5af3 41dd 279d f7f7 a27d bb06  ....Z.A.'....}..
+00002ed0: 555d aaf7 3aba d774 56e1 b5aa db3a 2f5b  U]..:..tV....:/[
+00002ee0: f5e6 85b2 ff59 a986 d3e6 5aaa 5729 666a  .....Y....Z.W)fj
+00002ef0: 0655 6f23 b5a5 7a9d a5b7 d477 a57a 65a5  .Uo#..z....w.ze.
+00002f00: fe74 8cbb b73a ecab 470f 7f01 0000 ffff  .t...:..G.......
+00002f10: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00002f20: fcab ce49 d904 0000 0d13 0000 1800 0000  ...I............
+00002f30: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00002f40: 6565 7431 2e78 6d6c ac98 4d8f a338 1086  eet1.xml..M..8..
+00002f50: ef2b ed7f 40dc 0742 be13 2519 4d3a 21f4  .+..@..B..%.M:!.
+00002f60: 6146 ab9d fd38 3bc4 49d8 06cc 82d3 e99e  aF...8;.I.......
+00002f70: 5fbf 6517 a6a1 88d0 acc4 a53b 94df 2a8a  _.e........;..*.
+00002f80: c785 297b f5f9 2d89 ad57 9e17 9148 d7b6  ..){..-..W...H..
+00002f90: e70c 6c8b a7a1 3845 e965 6dff f987 ff69  ..l...8E.em....i
+00002fa0: 6e5b 8564 e989 c522 e56b fb9d 17f6 e7cd  n[.d...".k......
+00002fb0: afbf acee 227f 29ae 9c4b 0b22 a4c5 dabe  ....".)..K."....
+00002fc0: 4a99 2d5d b708 af3c 6185 2332 9ec2 c859  J.-]...<a.#2...Y
+00002fd0: e409 9370 995f dc22 cb39 3b69 a724 7687  ...p._.".9;i.$v.
+00002fe0: 83c1 d44d 5894 da18 6199 ff4c 0c71 3e47  ...MX...a..L.q>G
+00002ff0: 21df 89f0 96f0 5462 909c c74c 42fe c535  !.....Tb...LB..5
+00003000: ca0a 132d 097f 265c c2f2 975b f629 1449  ...-..&\...[.).I
+00003010: 0621 8e51 1cc9 771d d4b6 9270 f97c 4945  .!.Q..w....p.|IE
+00003020: ce8e 313c f79b 3766 a189 ad2f 5ae1 9328  ..1<..7f.../Z..(
+00003030: cc45 21ce d281 702e 26da 7ee6 85bb 7021  .E!...p.&.~...p!
+00003040: d266 a539 fc96 5b00 9b7f 6309 dc23 10ff  .f.9..[...c..#..
+00003050: 30cf 7637 ab53 040f a766 c4ca f979 6d7f  0.v7.S...f...ym.
+00003060: f196 8137 5103 dae7 af88 df8b da6f eb87  ...7Q........o..
+00003070: 10c9 f790 a934 1730 7fd5 e537 c53e 46a3  .....4.0...7.>F.
+00003080: 9aae a310 2fca f9f9 b4b6 072a 031e f350  ..../......*...P
+00003090: 81b3 18fc 7be5 4f3c 06f5 93a7 a6fc 5f7d  ....{.O<......_}
+000030a0: 67f5 1b6e eb56 f7ad ff36 39f8 7a8a e149  g..n.V...69.z..I
+000030b0: 8eac e04f 22fe 3b3a c92b d412 a472 e267  ...O".;:.+...r.g
+000030c0: 768b e5ef e21e f0e8 7295 609d 3a13 db0a  v.......r.`.:...
+000030d0: 6f85 1449 6503 ae0a eff2 f4be e345 08f3  o..Ie........E..
+000030e0: 0af9 3943 75e7 50c4 701b f86b 2591 aa4f  ..9Cu.P.p..k%..O
+000030f0: 9816 f6a6 a28c e663 dbba 9777 f29c f170  .......c...w...p
+00003100: 329b 7b43 085d c877 0562 a4f3 4677 9dfd  2.{C.].w.b..Fw..
+00003110: 8e49 b659 e5e2 6e41 9d41 9c22 63aa 6abd  .I.Y..nA.A."c.j.
+00003120: 253c edff 4d0c 3252 51be a830 ea56 1624  %<..M.2RQ..0.V.$
+00003130: 5c00 d0d7 cd64 bc72 5f01 5258 4ab6 2881  \....d.r_.RXJ.(.
+00003140: bc2a c9a0 a978 6a2b bca6 62d7 560c 9b8a  .*...xj+..b.V...
+00003150: 7d5b 316a 2afc b682 647a 682b 26cd 1841  }[1j*...dzh+&..A
+00003160: 5b31 ad14 2e90 adf0 0efb c1ab c2ac eda1  [1..............
+00003170: 064b 986c 71ac ce75 46b8 1a85 aa22 355b  .K.lq..uF...."5[
+00003180: 3b34 4c31 dc00 6a86 40a4 0e3e 1a66 da81  ;4L1..j.@..>.f..
+00003190: f03c 5071 5033 3458 4075 f451 6a2a 8c61  .<PqP34X@u.Qj*.a
+000031a0: 4166 7f8b 635d 2c8c 4295 28ad 2e1c 2bb1  Af..c],.B.(...+.
+000031b0: cce7 cec7 9c6a 6c7b e36b 38fa 6840 2c44  .....jl{.k8.h@,D
+000031c0: 7ca0 e2a0 6668 6081 b7b7 0f2c 2a8c c142  |...fh`....,*..B
+000031d0: a668 8b63 5d58 8ce2 1116 1c2b b10c 61d5  .h.c]X.....+..a.
+000031e0: 22d5 627c 2b2c 6840 2ca4 160f 541c d40c  ".b|+,h@,...T...
+000031f0: 0d2c 6a01 eb61 6152 610c 16ba 22e1 5817  .,j..aaRa...".X.
+00003200: 16a3 7884 05c7 4a2c e3b9 43aa 696f 7c2b  ..x...J,..C.io|+
+00003210: 2c68 402c 74c9 a1e2 a066 6860 99f6 8345  ,h@,t....fh`...E
+00003220: 8531 58c8 7c6e 71ac 0b8b 5154 0b0a 1a90  .1X.|nq...QT....
+00003230: c5cc 6b55 08d5 fb68 4014 e41d 3e50 7150  ..kU...h@...>PqP
+00003240: 3334 50cc fa41 a1c2 1814 e425 dee2 5817  34P..A.....%..X.
+00003250: 0aa3 a850 a001 514c a70e 7915 f754 efa3  ...P..QL..y..T..
+00003260: 0151 7894 0555 0735 4383 856a 547a 785b  .Qx..U.5C..jTzx[
+00003270: 5498 b53d 7ff8 9dc1 b145 edfb 3d27 df19  T..=.....E..='..
+00003280: a3a8 58a0 01da 1fdd 1038 23ba a052 07bf  ..X......8#..R..
+00003290: 74f0 ca2f 5333 fe81 ca83 9aa1 4103 92ec  t../S3......A...
+000032a0: 8386 0a63 68d0 2515 c7ba 6818 c5a3 b503  ...ch.%...h.....
+000032b0: c74a 3053 87ce fbde f856 6b47 e980 6008  .J0S.....VkG..`.
+000032c0: f703 5507 3543 838b 6a44 7be9 f654 1c43  ..U.5C..jD{..T.C
+000032d0: a6d5 e7e1 6017 1a9d 0774 e38f ea6c 570e  ....`....t...lW.
+000032e0: 9670 66ce 907c 42f6 9577 45c7 b820 1eb2  .pf..|B..wE.. ..
+000032f0: 9e1d 5afa a06e 6902 eaab 1dc6 0611 5f24  ..Z..ni......._$
+00003300: babe 7a38 d809 c848 aa57 a974 32ef 12ed  ..z8...H.W.t2...
+00003310: 7aa9 de37 faf2 556a 31a1 0e41 9595 dae5  z..7..Uj1..A....
+00003320: d45b 58af a71e 56c7 3145 4317 da72 b093  .[X...V.1EC..r..
+00003330: 09f6 950b bd19 d26d 6ce9 5432 1939 b356  .......ml.T2.9.V
+00003340: a550 17df b894 5868 2f5b a561 b807 754b  .P....Xh/[.a..uK
+00003350: 134b 4fed ac87 7d21 964a 0b0b 0e76 6231  .KO...}!.J...vb1
+00003360: 928f 5241 4b85 6541 8b85 7af8 650e 5002  ..RAK.eA..z.e.P.
+00003370: 7ab1 6aed 87a8 4350 3ae8 b968 52e9 a79b  z.j...CP:..hR...
+00003380: dd7a a69d 354f b56f 59fc d232 d6fb db46  .z..5O.oY..2...F
+00003390: c5f6 d33b 6ee1 a401 5b83 0fb4 68d1 4713  ...;n...[...h.G.
+000033a0: b827 a86b 9004 1e11 e026 3b63 17fe 95e5  .'.k.....&;c....
+000033b0: 9728 2dac 989f f56e 1e3e e139 9e00 0c1c  .(-....n.>.9....
+000033c0: f82d 45a6 f6f8 3388 7c14 12ce 02cc d515  .-E...3.|.......
+000033d0: 4e88 38ec d606 0ee0 3f0b 21cd 0564 a3e2  N.8.....?.!..d..
+000033e0: 7ee7 f296 5922 8fe0 9440 1ffa aced 4ce4  ~...Y"...@....L.
+000033f0: 3267 9184 7d3c d87f 0818 8877 5904 1bf3  2g..}<.....wY...
+00003400: 292c ca70 b625 2338 1cf9 b0e4 cb08 0e40  ),.p.%#8.......@
+00003410: f2e7 937e 20b7 3ac8 dafc 0700 00ff ff03  ...~ .:.........
+00003420: 0050 4b03 0414 0006 0008 0000 0021 004a  .PK..........!.J
+00003430: 6587 bc32 0900 0057 3000 0018 0000 0078  e..2...W0......x
+00003440: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
+00003450: 6574 382e 786d 6cac 9b4d 73db 3812 86ef  et8.xml..Ms.8...
+00003460: 5b35 ff41 c5fb 5002 29c9 92cb f2d4 c836  [5.A..P.)......6
+00003470: c51c 766a 6a3e 76cf b444 db9c 48a2 96a4  ..vjj>v..D..H...
+00003480: e364 7efd 02e8 0608 74db d86c 1572 48ec  .d~.....t..l.rH.
+00003490: 4677 137a d800 5e40 c8cd 4f5f 4fc7 c997  Fw.z..^@..O_O...
+000034a0: baeb 9bf6 bc49 443a 4b26 f579 df1e 9af3  .....ID:K&.y....
+000034b0: f326 f9f3 8fe2 c755 32e9 87ea 7ca8 8eed  .&.....U2...|...
+000034c0: b9de 24df ea3e f9e9 f687 7fdc bcb5 dde7  ..$..>..........
+000034d0: fea5 ae87 89cc 70ee 37c9 cb30 5cae a7d3  ......p.7..0\...
+000034e0: 7eff 529f aa3e 6d2f f559 b63c b5dd a91a  ~.R..>m/.Y.<....
+000034f0: e4af ddf3 b4bf 7475 75d0 41a7 e334 9bcd  ......tuu.A..4..
+00003500: 96d3 53d5 9c13 c870 dd7d 4f8e f6e9 a9d9  ..S....p.}O.....
+00003510: d7f7 edfe f554 9f07 48d2 d5c7 6a90 fdef  .....T..H...j...
+00003520: 5f9a 4b6f b29d f6df 93ee 5475 9f5f 2f3f  _.Ko......Tu._/?
+00003530: eedb d345 a678 6c8e cdf0 4d27 4d26 a7fd  ...E.xl...M'M&..
+00003540: f5a7 e773 db55 8f47 f9b9 bf8a 79b5 37b9  ...s.U.G....y.7.
+00003550: f52f 2cfd a9d9 776d df3e 0da9 4c37 858e  ./,...wm.>..L7..
+00003560: f2cf bc9e aea7 32d3 ed8d e6f0 6b37 91b0  ......2.....k7..
+00003570: eb5f aa93 7c46 d9fe 55ad 92e9 edcd a191  ._..|F..U.......
+00003580: 1f4e bd91 4957 3f6d 929f c575 399f a906  .N..IW?m...u9...
+00003590: 1df3 afa6 7eeb 9d9f 277f b7ed e9f7 7da5  ....~...'.....}.
+000035a0: bab9 96ef cffe fa8b 627f 04a3 7a5d 8f6d  ........b...z].m
+000035b0: fb59 057f 3a6c 9299 ea41 7dac f70a dca4  .Y..:l...A}.....
+000035c0: 92ff 7ca9 efea a3f4 be13 ea95 ff47 3f59  ..|..........G?Y
+000035d0: fd2c 1f3b b5cf 757f 367d 28f4 2b96 9fe4  .,.;..u.6}(.+...
+000035e0: b1ea ebbb f6f8 efe6 30bc c85a 925d 39d4  ........0..Z.]9.
+000035f0: 4fd5 eb71 f8ad 7d2b ebe6 f965 90d6 65ba  O..q..}+...e..e.
+00003600: 4826 fbd7 7e68 4fd6 26b9 2abc d787 6ff7  H&..~hO.&.*...o.
+00003610: 75bf 97ef 55f6 2fcd d493 f7ed 513e 46fe  u...U./.....Q>F.
+00003620: 3d39 35aa 3ee5 6ba9 beaa 2cf9 6a9e 4cde  =95.>.k...,.j.L.
+00003630: f049 229d 678b ab95 c864 ea7e f8a6 40e4  .I".g....d.~..@.
+00003640: badf 10ae 7b7f 5f0d d5ed 4dd7 be4d 649d  ....{._...M..Md.
+00003650: c93c fda5 5255 2bae e5a7 fd7f 3b26 7ba4  .<..RU+.....;&{.
+00003660: b2fc acd2 a847 4d64 877b 09f4 cbed 627e  .....GMd.{....b~
+00003670: 33fd 2221 edd1 650b 2eb2 5fd6 65e6 7bdc  3."!..e..._.e.{.
+00003680: 710f e17b dc73 8fcc f778 e01e b9ef 5170  q..{.s...x....Qp
+00003690: 0fd2 d31d f758 f839 4aee b1b4 1e53 49d6  .....X.9J....SI.
+000036a0: e2cd e2e0 5569 3649 a6c1 1226 5b68 73b9  ....Ui6I...&[hs.
+000036b0: 5e11 aec6 4355 917a 5bf7 6058 ea74 f92c  ^...CU.z[.`X.t.,
+000036c0: 5d11 86d4 bf00 c395 f627 c077 d4b9 740c  ]........'.w..t.
+000036d0: 1e0a 591c 312a 4da5 3128 485f b6d0 1642  ..Y.1*M.1(H_...B
+000036e0: 613c 2c0a 3020 8a79 4a5e f403 f52f c000  a<,.0 .yJ^.../..
+000036f0: 2868 dd50 e7d2 3178 28e4 808d 8142 a531  (h.P..1x(....B.1
+00003700: 2848 956f a12d 84c2 78a8 c14a c719 b401  (H.o.-..x..J....
+00003710: 954c 2c18 1613 6b30 1660 002c 828c eb1d  .L,...k0.`.,....
+00003720: f52e 1d83 c745 4d5a 1126 2395 c670 a1b3  .....EMZ.&#..p..
+00003730: 10b4 85b8 180f 5b22 6000 18f3 2b36 5aa8  ......["`...+6Z.
+00003740: 7f01 0660 4186 e28e 3a97 8ec1 43b1 8c83  ...`A...:...C...
+00003750: 42a5 3128 486d 6fa1 2d84 c278 5814 6040  B.1(Hmo.-..xX.`@
+00003760: 142b 8682 fa17 6000 1464 96d9 51e7 d231  .+....`..d..Q..1
+00003770: 7828 aee2 a050 690c 8a71 b6d6 13e2 16da  x(...Pi..q......
+00003780: 4228 8c87 4501 061c 2259 4a46 d003 f52f  B(..E..."YJF.../
+00003790: c080 7328 1d21 d4bb 740c 1e0b 2548 228c  ..s(.!..t...%H".
+000037a0: 1095 c6b0 2025 ba85 b610 0be3 6159 8001  .... %......aY..
+000037b0: 59ac 5292 f181 fa17 6040 1674 16a5 dea5  Y.R.....`@.t....
+000037c0: 63f0 58ac e3b0 5069 0c0b 52a3 5b68 0bb1  c.X...Pi..R.[h..
+000037d0: 301e 9605 183e 6441 fd0b 3020 0b3a 5d50  0....>dA..0 .:]P
+000037e0: efd2 3178 2c94 c48c a2e3 541e 4363 4d15  ..1x,.....T.CcM.
+000037f0: 1c34 8670 e87e 6c92 8556 ac5a 6ba0 0580  .4.p.~l..V.Zk...
+00003800: acf8 9cc1 220a b420 12b2 b0ed 987f e95a  ....".. .......Z
+00003810: 7c28 b1c4 2dc8 3d94 5f64 ec6e 0517 8354  |(..-.=._d.n...T
+00003820: 8059 175b 2568 c199 54b0 0596 4514 6801  .Y.[%h..T...E.h.
+00003830: 2ae4 cdec 987b e95a 7c28 9124 a9f0 3429  *....{.Z|(.$..4)
+00003840: 15a5 d81a 2c15 264b 31c8 cca9 54d9 3359  ....,.&K1...T.3Y
+00003850: 8afe 28c6 4817 76b6 0b06 7ae9 5a7c 2691  ..(.H.v...z.Z|&.
+00003860: b4a9 70c5 a9a0 ea14 5b83 4c98 3ec5 2060  ..p.....[.L.>. `
+00003870: 22f2 94ed 7798 42c5 08a0 92b3 e1c3 44aa  "...w.B.......D.
+00003880: ed96 dade ba7b 1711 49a6 ea3c 76f7 4285  .....{..I..<v.B.
+00003890: 2ab6 06a9 5001 798f 4148 65ce 565f 9bd4  *...P.y.AHe.V_..
+000038a0: 0a54 b4e0 a4c2 c60f 93a8 6e06 9f8a 526c  .T........n...Rl
+000038b0: 3176 cca0 fc70 5261 9b65 a30b c7dd 329b  1v...pRa.e....2.
+000038c0: 54a8 96bc 1760 c1f1 b3e4 b542 230a 8c40  T....`.....B#..@
+000038d0: dd4e b776 d83a 4ee6 a56b f1a9 44d2 abc2  .N.v.:N..k..D...
+000038e0: 15ac 822a 566c 0dd6 0ad3 ac18 6436 334c  ...*Vl......d63L
+000038f0: b4da a463 adb8 b255 10ad b863 fea5 6bf1  ...c...U...c..k.
+00003900: a944 92ae c268 d7b1 1ae6 54c2 a24f 908d  .D...h....T..O..
+00003910: 5195 ef6d f930 1e87 d492 0cd3 079b 7ea4  Q..m.0........~.
+00003920: e42a da9c 8d28 2669 dd0c 3ea5 48a2 569f  .*...(&i..>.H.V.
+00003930: d6a9 79c6 a144 c52d fa04 2919 bdf9 2e25  ..y..D.-..)....%
+00003940: 57ea ae57 7ce2 615a 179f 888b 1415 feb6  W..W|.aZ........
+00003950: 3fe3 22f5 91dc 1591 f4ae ce43 3051 dd8b  ?."........C0Q..
+00003960: 3e41 4c46 8abe 8bc9 55c1 6235 e39c 980e  >ALF....U.b5....
+00003970: c647 02a7 059b 8a98 12b6 5da4 cb56 1649  .G........]..V.I
+00003980: 0aeb 3c84 1355 c4e8 13e2 645d dee3 848d  ..<..U....d]....
+00003990: 38e8 8448 c903 1e6c b41d 7668 414e b49e  8..H...l..vhAN..
+000039a0: 987f e95a bc61 9745 52c7 3a8f cf69 4135  ...Z.a.ER.:..iA5
+000039b0: 32fa 0439 1919 fd2e 2768 3493 d32c 5dae  2..9....'h4..,].
+000039c0: dd3f f4fc d2a4 1aa1 8105 0721 5956 76b6  .?.........!YVv.
+000039d0: 7776 10ba 161f 5aac 035d a39e 9d03 7376  wv....Z..]....sv
+000039e0: b0fb 1d27 bbfc 68d7 3ddb 15eb 94ce e319  ...'..h.=.......
+000039f0: 3fdc 754f 77e9 b2b2 63fe a56b f1d9 4452  ?.uOw...c..k..DR
+00003a00: d119 48d4 d5fb a7dd d028 a703 fb35 0299  ..H......(...5..
+00003a10: bcee 307e 3dee 41d1 2237 8aaa b8b2 7446  ..0~=.A."7....tF
+00003a20: 5534 0b29 4c88 78af 173b e65f ba16 9f4a  U4.)L.x..;._...J
+00003a30: 2415 9d81 44fd 800a 3406 a918 17bb 07c5  $...D...4.......
+00003a40: 8c0e 156f 50b1 6f05 6882 c224 0046 74a7  ...oP.o.h..$.Ft.
+00003a50: 81ad e36b 285d 8bcf 2892 a6d6 df7a 6d12  ...k(]..(....zm.
+00003a60: 6044 b75f d818 6404 02d9 ad1c b058 4673  `D._..d......XFs
+00003a70: 5639 34a4 c0e7 c80d b82a 36aa 1e6d 2fc6  V94......*6..m/.
+00003a80: b9c6 c9e0 5389 a4a9 3390 b31f 5081 c620  ....S...3...P.. 
+00003a90: 15e3 3256 0e58 2c15 7ae0 874f 1c39 1668  ..2V.X,.z..O.9.h
+00003aa0: 4128 6c02 a64f 28dd 0c3e 9448 923a 037d  A(l..O(..>.H.:.}
+00003ab0: 0a50 e83e 031b 8350 20de 2d15 b020 14c1  .P.>...P .-.. ..
+00003ac0: 4e41 6dd2 7155 c208 a894 8c1e 90b3 80d2  NAm.qU..........
+00003ad0: b5f8 5422 49e8 0cc4 2750 a13b 0c6c 0c52  ..T"I...'P.;.l.R
+00003ae0: 8178 970a 582c 9525 1b40 34a4 c0e7 60ad  .x..X,.%.@4...`.
+00003af0: 64ec 0b47 1a50 da8e 3129 1849 3267 a03e  d..G.P..1).I2g.>
+00003b00: 3fc0 028d 412c c665 1c41 6019 b1d0 ef0f  ?...A,.e.A`.....
+00003b10: f091 ee10 c210 ac16 7adc c502 4ad7 e255  ........z...J..U
+00003b20: 4b1e 4921 eb3c 66ba a53b 2d6c 0c61 b12e  K.I!.<f..;-l.a..
+00003b30: 160b 5a2c 968c 6261 2185 0941 2c74 6a61  ..Z,..ba!..A,tja
+00003b40: 01a5 6bf1 b144 12c4 3988 4da8 1686 051a  ..k..D..9.M.....
+00003b50: 8358 8ccb 8805 2c16 cb9a 1c17 3de0 239d  .X....,.....=.#.
+00003b60: 6a41 8b19 4474 1962 01a5 6bf1 b144 92bc  jA..Dt.b..k..D..
+00003b70: 39e8 4cc0 4237 9cd8 18c4 02f1 cedc 8241  9.L.B7.........A
+00003b80: 7619 62c5 4223 0a13 818a 857e dd62 7b61  v.b.B#.....~.b{a
+00003b90: 1767 d7e2 5389 2476 734f ecd2 2d00 b606  .g..S.$vsO..-...
+00003ba0: b118 413c 560b 58c6 6a61 971a 6848 81cf  ..A<V.X.ja..hH..
+00003bb0: c16a 9953 2967 bb31 7271 52f8 5c22 c9dd  .j.S)g.1rqR.\"..
+00003bc0: dc93 bb8c cbff d6bb 98c0 2d17 08b2 e5b2  ..........-.....
+00003bd0: a00a 9785 1468 315c e852 c402 4ad7 e273  .....h1\.R..J..s
+00003be0: 8924 7173 508b b80d 6017 608c 96fc 7877  .$qsP...`.`...xw
+00003bf0: 8409 5c2e 9ec6 1569 46e5 1c0b 29d0 825c  ..\....iF...)..\
+00003c00: 7276 11c6 7443 29e0 9c5e 9eb2 e974 eb07  rv..tC)..^...t..
+00003c10: 17a7 f248 e257 e731 6b94 a05f 3e60 6b70  ...H.W.1k.._>`kp
+00003c20: 7c31 f58b 41e3 2245 0f6d 6c56 abf4 4c08  |1..A."E.mlV..L.
+00003c30: ce3b f4d4 c606 6822 a4d8 4bbf 757c e57e  .;....h"..K.u|.~
+00003c40: 7d45 d2c5 b9ab 8b05 fd5a 025b 83bc 9830  }E.......Z.[...0
+00003c50: c620 cb4b 8899 fb87 cdda 3441 6112 e05e  . .K......4Aa..^
+00003c60: 9ccd 4e26 409f 1c91 2e97 b6cb ba75 ac45  ..N&@........u.E
+00003c70: 9f5e 24fd 9cbb fa99 7d7d 81ad 417a 4c40  .^$.....}}..AzL@
+00003c80: 6390 a537 5b87 e931 396d 1220 3db6 e699  c..7[..19m. =...
+00003c90: 00cd 874c 89a5 edb2 6e1d 0bdd a717 4966  ...L....n.....If
+00003ca0: e746 663b 07f8 f4c4 157d 820c 8dda 7eef  .Ff;.....}....~.
+00003cb0: 2411 e311 e722 5db3 4580 6af5 c284 00c0  $...."].E.j.....
+00003cc0: 0515 deb6 47e3 e2e8 a4f0 40c9 abcb 712e  ....G.....@...q.
+00003cd0: fec1 450c f9e6 c6eb b674 89d4 cf92 379e  ..E......t....7.
+00003ce0: 0307 65d6 c54a 07b4 d825 92e9 6f16 5298  ..e..J...%..o.R.
+00003cf0: 10a0 33a7 e565 03d4 cb98 d3f2 f25b 6979  ..3..e.......[iy
+00003d00: c165 6bb8 ae7c a99e eb7f 56dd 7373 ee27  .ek..|....V.ss.'
+00003d10: c7fa 49df 8b96 e3be 83bb d4b3 54fe 3cb4  ..I.........T.<.
+00003d20: 1775 5bfa 4a2e 3e8f ed20 6f55 9bdf 5ee4  .u[.J.>.. oU..^.
+00003d30: 5dfb 5ade 7b9d a552 b53c b5ed 607e 919f  ].Z.{..R.<..`~..
+00003d40: 5be5 fdbd 1e5e 2f93 b66b e47d 6b7d 7d7e  [....^/..k.}k}}~
+00003d50: 935c da6e e8aa 6690 37a2 a5fd ef56 361c  .\.n..f.7....V6.
+00003d60: ef2f 8dbc e2bc 94ec e5ff 1218 1a79 cd7c  ./...........y.|
+00003d70: b474 d78d bc4a de7d 3a08 7ddb dafe 9780  .t...J.}:.}.....
+00003d80: dbff 0200 00ff ff03 0050 4b03 0414 0006  .........PK.....
+00003d90: 0008 0000 0021 0007 3a3d 1bee 0700 0038  .....!..:=.....8
+00003da0: 2700 0018 0000 0078 6c2f 776f 726b 7368  '......xl/worksh
+00003db0: 6565 7473 2f73 6865 6574 372e 786d 6cac  eets/sheet7.xml.
+00003dc0: 5adf 6fdb 3610 7e1f b0ff 41d0 7b65 4bb2  Z.o.6.~...A.{eK.
+00003dd0: e338 8853 d449 6415 d88a 61dd 8f67 4596  .8.S.Id...a..gE.
+00003de0: 13ad 96e5 494a d3f4 af1f c93b 52e4 dda6  ....IJ.....;R...
+00003df0: 7600 fb90 dac7 ef8e d4a7 e3f1 23cd ebb7  v...........#...
+00003e00: 5f9a 63f0 b9ea faba 3d6d c238 9a87 4175  _.c.....=m.8..Au
+00003e10: 2adb 7d7d 7adc 84bf ff96 bdb9 0c83 7e28  *.}}z.........~(
+00003e20: 4efb e2d8 9eaa 4df8 5af5 e1db 9b1f 7fb8  N.....M.Z.......
+00003e30: 7e69 bb4f fd53 550d 8188 70ea 37e1 d330  ~i.O.SU...p.7..0
+00003e40: 9caf 66b3 be7c aa9a a28f da73 7512 2d87  ..f..|.....su.-.
+00003e50: b66b 8a41 7ced 1e67 fdb9 ab8a bd72 6a8e  .k.A|..g.....rj.
+00003e60: b364 3ebf 9835 457d 0a21 c255 f73d 31da  .d>..5E}.!.U.=1.
+00003e70: c3a1 2eab bbb6 7c6e aad3 0041 baea 580c  ......|n...A..X.
+00003e80: 62fc fd53 7dee 75b4 a6fc 9e70 4dd1 7d7a  b..S}.u....pM.}z
+00003e90: 3ebf 29db e62c 423c d4c7 7a78 5541 c3a0  >.)..,B<..zxUA..
+00003ea0: 29af de3f 9eda ae78 388a e7fe 122f 8a52  )..?...x8..../.R
+00003eb0: c756 5f58 f8a6 2ebb b66f 0f43 24c2 cd60  .V_X.....o.C$..`
+00003ec0: a0fc 99d7 b3f5 4c44 bab9 563c fcd2 0582  ......LD..V<....
+00003ed0: ecea 43d1 883e f2f6 af62 15ce 6eae f7b5  ..C..>...b..n...
+00003ee0: 7838 f946 82ae 3a6c c277 f155 9e26 b241  x8.F..:l.w.U.&.A
+00003ef0: f9fc 5157 2fbd f539 18da f34f d561 b8ad  ..QW/..9...O.a..
+00003f00: 8e47 094e c3e0 6bdb 361f cb42 0e7c 2dde  .G.N..k.6..B.|-.
+00003f10: a8f9 fa41 be0d 0192 46f9 021f daf6 930c  ...A....F.......
+00003f20: f77e bf09 e772 4cd5 b12a 2595 4121 fefb  .~...rL..*%.A!..
+00003f30: 5c41 c8db 5826 c1df 6a2c f2b3 18c8 cc8c  \A..X&..j,......
+00003f40: c4fe ac47 95a9 972e 9eed a1e8 abdb f6f8  ...G............
+00003f50: 67bd 1f9e 4476 895e f7d5 a178 3e0e bfb6  g...Dv.^...x>...
+00003f60: 2f79 553f 3e0d c27a 112d c3a0 7cee 87b6  /yU?>..z.-..|...
+00003f70: 3136 c1b4 24fc 6aff 7a57 f5a5 78d3 627c  16..$.j.zW..x.b|
+00003f80: 91a2 a06c 8fa2 1bf1 3768 6a99 b1e2 4515  ...l....7hj...E.
+00003f90: 5f64 94f4 7221 1e0a 7b8a a345 b25c 5dc6  _d..r!..{..E.\].
+00003fa0: 8908 dd0f af92 8854 8d1b dcd5 e8ef 8aa1  .......T........
+00003fb0: b8b9 eeda 9740 649e 88d3 9f0b 99c7 f195  .....@d.........
+00003fc0: 78da ff3b 3031 2219 e59d 0c23 bb0a c480  x..;01"....#....
+00003fd0: 7b41 e8e7 9be5 e27a f659 9054 2264 0b10  {A.....z.Y.T"d..
+00003fe0: 312e 0399 bb88 5b8e 885d c41d 4724 2ee2  1.....[..]..G$..
+00003ff0: 9e23 5217 9171 0419 e98e 2396 6e8c 9c23  .#R..q....#.n..#
+00004000: 2e0c 6226 9835 f426 7ee8 9561 3661 a288  ..b&.5.&~..a6a..
+00004010: 259c 6ca1 cde6 7545 78d5 0891 bfea 6ddd  %.l...uEx.....m.
+00004020: 81e1 02de d33c 2211 ef29 3e03 c34a e1c7  .....<"..)>..J..
+00004030: 0755 b176 149c 5b06 870a 911c 3e32 4d86  .U.v..[.....>2M.
+00004040: 9154 8c69 945e 924c 03c8 1423 1a61 1801  .T.i.^.L...#.a..
+00004050: 0330 922c a235 c92a 8acf c000 8c90 04db  .0.,.5.*........
+00004060: 5170 6e19 1c46 c4bc f5c1 880c 4318 21e3  Qpn..F......C.!.
+00004070: df02 648a 118d 308c 8001 1849 978c 118a  ..d...0....I....
+00004080: cfc0 008c c424 a376 149d 5b06 8712 59b6  .....$.v..[...Y.
+00004090: 3c94 2319 46cf 175a 87a0 6d8a 0b8d 305c  <.#.F..Z..m...0\
+000040a0: 8001 b888 e7cb 8884 bca7 0e19 1890 0c9a  ................
+000040b0: 1f14 9d5b 0687 8c0b 3f64 c830 9a0c 52c8  ...[....?d.0..R.
+000040c0: b6d0 3645 8646 1832 c000 64ac d388 149b  ..6E.F.2..d.....
+000040d0: 7b8a cfc0 005c d04a 4bc1 b965 70a8 58f9  {....\.JK..ep.X.
+000040e0: a142 86d1 5490 42b6 85b6 292a 34c2 5001  .B..T.B...)*4.P.
+000040f0: 06a0 62b5 8e08 b9f7 149f 8101 a820 e01d  ..b.......... ..
+00004100: 05e7 96c1 a142 6a12 0f53 4486 d154 9077  .....Bj..SD..T.w
+00004110: b885 b629 2a34 c250 0106 a062 4189 a0e8  ...)*4.P...bA...
+00004120: 0c0c 383f dc5a bba3 e0dc 3238 44ac fd10  ..8?.Z....28D...
+00004130: 21c3 b8e5 7341 84c9 1620 537c 6884 e103  !...sA... S|h...
+00004140: 0cb8 a0a4 ac62 507c 0606 6084 54ef 1d05  .....bP|..`.T...
+00004150: e796 c161 440a 4d2f 6a4e c621 9c50 d9a1  ...aD.M/jN.!.P..
+00004160: fada 8453 a418 8861 052d b8aa a411 9983  ...S...a.-......
+00004170: f7cc 2343 0b10 4316 fa1d 83e7 b6c5 a5c6  ..#C..C.........
+00004180: 97d0 05e9 8752 8c26 4acc 8521 1563 0632  .....R.&J..!.c.2
+00004190: 9202 4e48 ca8a 9511 e691 a105 4821 1dec  ..NH........H!..
+000041a0: 183c b72d 2e29 9ee4 69ec e853 9629 df56  .<.-.)..i..S.).V
+000041b0: a818 6029 b72a 2051 d182 a424 4c7f 308f  ..`).* Q...$L.0.
+000041c0: 0c2d 400a d916 ec18 3cb7 2d2e 299e 84aa  .-@.....<.-.)...
+000041d0: dc8f 8ea2 9d0c 688b ad93 d347 eb46 b99d  ......h....G.F..
+000041e0: 623b 215b b1c6 ab84 8978 d381 a634 430b  b;![.....x...4C.
+000041f0: 8a56 5a64 183e b72d 2e43 9e84 6bac 95ab  .VZd.>.-.C..k...
+00004200: 7a40 2293 b6d8 3ac9 1053 ade8 8452 2de1  z@"...:..S...R-.
+00004210: 0586 e956 f4c0 b588 4ce8 9d19 8466 31b7  ...V....L....f1.
+00004220: 2d2e 2b52 c6f9 d84a 831c c40a c376 d15a  -.+R...J.....v.Z
+00004230: 2c8e fb1f 5661 987e 8d1d 01bb 8e48 1dbd  ,...Va.~.....H..
+00004240: c7f6 71fa 6568 4156 d86c 6212 d68e e0b2  ..q.ehAV.lb.....
+00004250: e249 c4c6 b68a 8da9 8cc5 d6c9 5c61 4216  .I..........\aB.
+00004260: 9d70 8d5e 46ec 2881 4959 f440 56d8 b101  .p.^F.(.IY.@V...
+00004270: 53b3 6658 f2e4 c83e 1688 3de9 5915 6713  S.fX...>..=.Y.g.
+00004280: 5efe ebc1 0036 0ab1 604e 5cc8 8bbf 3590  ^....6..`N\...5.
+00004290: b1ee 82ec 14eb a89a 9451 4ab7 c2cc 2543  .........QJ...%C
+000042a0: 8b58 65a4 4bc2 9205 22ae 4d6d cfed 102e  .Xe.K...".Mm....
+000042b0: 2d9e b4ad 3ab7 93b4 4c1c 1220 6692 1d50  -...:...L.. f..P
+000042c0: 9ee3 c8ef d009 d961 0943 f199 c623 35ac  .......a.C...#5.
+000042d0: ba50 87dc 8c8a 658c 27b5 1b83 76b4 a959  .P....e.'...v..Y
+000042e0: b0b5 0930 93d4 68c8 9838 6031 89b3 a01b  ...0..h..8`1....
+000042f0: 43ec 7964 3343 0b26 4ecc 5624 da47 6e87  C.yd3C.&N.V$.Gn.
+00004300: 7012 27f1 247c 551c 9238 f42c 0531 53ec  p.'.$|U..8.,.1S.
+00004310: 1888 6107 2d3a 71a2 453a b7ff d14c 6201  ..a.-:q.E:...Lb.
+00004320: 321d 0032 29a5 072c cc21 b72d 2e57 9e94  2..2)..,.!.-.W..
+00004330: 7002 b2d5 c924 ba86 2366 922b 0863 4d32  p....$..#f.+.cM2
+00004340: 7432 5ccd e92e c144 35d2 46bb 203b b404  t2\....D5.F. ;..
+00004350: 3187 dcb6 b8ec f83a b105 d10b 9599 2e57  1......:.......W
+00004360: 0934 4ed2 a221 630a 8105 6959 4697 8c16  .4N..!c...iYF...
+00004370: ea92 613f ba32 b3a4 a10e b919 182d 3f89  ..a?.2.......-?.
+00004380: 2751 ace2 e805 8b1e 3b60 e324 2d20 7bed  'Q......;`.$- {.
+00004390: 6c01 8ba9 3b2b 460b 75c9 b01f 5d77 e806  l...;+F.u...]w..
+000043a0: ca0c c368 3edb e266 8b27 259c 802c 75e6  ...h>..f.'%..,u.
+000043b0: 12dd 5b22 6692 1d08 63b3 0316 c3ce 2595  ..["f...c.....%.
+000043c0: 7e26 ea38 97d0 05d7 2c76 de4f fbc8 ed10  ~&.8....,v.O....
+000043d0: 2e3b 9e14 b1fa 31cb adca 0baa 8b11 33c9  .;....1.......3.
+000043e0: 0ea8 569b 1db0 1876 e68c 1dea 9261 3f7a  ..V....v.....a?z
+000043f0: 4ab1 dca1 0eb9 1918 9b52 9e94 7102 b2d3  J........R..q...
+00004400: c91d f61b 1160 26d9 d190 b1e0 8065 9c59  .....`&......e.Y
+00004410: 8c1d ea92 e158 343b 5421 63b3 2505 6d8b  .....X4;T!c.%.m.
+00004420: 9b3b 9e14 7202 ead3 6187 9563 ad50 ff5b  .;..r...a..c.P.[
+00004430: 2863 183b 7788 50e6 b943 756f 8641 343b  (c.;w.P..Cuo.A4;
+00004440: f404 98f5 91db 1697 1d4f 4239 0101 8afb  .........OB9....
+00004450: 0756 71b4 3c9d e085 4964 0c39 ea40 a66d  .Vq.<...Id.9.@.m
+00004460: 984a d62e 5871 e8ef 25d8 6c67 8d15 c2e5  .J..Xq..%.lg....
+00004470: c593 4a4e b44a 569b 2036 9bbe ad8f 3180  ..JN.JV. 6....1.
+00004480: 9d2f 8e3e e627 c2cc 2343 8b5e a6e8 e127  ./.>.'..#C.^...'
+00004490: 73c8 6d8b 434b ea49 1eab 3866 bb49 c51e  s.m.CK.I..8f.I..
+000044a0: b64e 1519 0331 4506 2d26 5d12 fa63 3473  .N...1E.-&]..c4s
+000044b0: c9b4 0ba6 0be5 c538 a8dd 2851 efb9 d39a  .......8..(Q....
+000044c0: 8e19 eff2 e549 22a7 5a22 ab34 a24b 16b6  .....I".Z".4.K..
+000044d0: 4ef2 c5c4 313a 69be e8ef d414 9f69 3c2a  N...1:i......i<*
+000044e0: 63f6 5bb5 7690 234c c908 7333 42d5 3ad6  c.[.v.#L..s3B.:.
+000044f0: 2b97 2c4f 8a59 dcf4 91e7 a558 8b68 8dc6  +.,O.Y.....X.h..
+00004500: d649 b298 6446 a7b1 16d1 1fa6 4c54 a37e  .I..dF......LT.~
+00004510: b40b f245 d58f 7150 8c90 d55f 5e56 928f  ...E..qP..._^V..
+00004520: b056 0721 d6b5 04e0 0bee 0ec1 ed9b 73f1  .V.!..........s.
+00004530: 58fd 5c74 8ff5 a90f 8ee2 0e93 bce6 23d6  X.\t..........#.
+00004540: 8b0e ae06 a9cf e276 93b2 0a45 f1d0 0ee2  .......v...E....
+00004550: 9290 fef6 242e 9355 e2d2 cd3c 12ca f6d0  ....$..U...<....
+00004560: b683 fe22 1e42 c6fd 580d cfe7 a0ed 6a71  ...".B..X.....jq
+00004570: 7d48 dd0f db84 e7b6 1bba a21e c405 1f61  }H.............a
+00004580: ffda 8a86 e3dd b916 3776 2e44 6910 d7e0  ........7v.Di...
+00004590: 865a dc9a 1a2d dd55 2d6e 4675 eff7 b1ba  .Z...-.U-nFu....
+000045a0: 3c64 eebc ddfc 0300 00ff ff03 0050 4b03  <d...........PK.
+000045b0: 0414 0006 0008 0000 0021 005f 4cd6 4a9e  .........!._L.J.
+000045c0: 0600 0024 1e00 0018 0000 0078 6c2f 776f  ...$.......xl/wo
+000045d0: 726b 7368 6565 7473 2f73 6865 6574 362e  rksheets/sheet6.
+000045e0: 786d 6cac 995b 6fdb 3614 c7df 07ec 3b08  xml..[o.6.....;.
+000045f0: 7aaf 6cc9 b7d8 8853 d4b1 6315 e88a 61dd  z.l....S..c...a.
+00004600: e559 91e9 58ab 647a 9292 34fd f43b e421  .Y..X.dz..4..;.!
+00004610: 29f2 d013 3a40 7968 ed73 13f5 d321 f537  )...:@yh.s...!.7
+00004620: 79fb fe5b 5506 2fac 6e0a 7e5e 8771 340e  y..[U./.n.~^.q4.
+00004630: 0376 cef9 a138 3fad c33f 7e7f 7877 1306  .v...8?..?~.xw..
+00004640: 4d9b 9d0f 59c9 cf6c 1dbe b126 7c7f f7f3  M...Y..l...&|...
+00004650: 4fb7 afbc feda 9c18 6b03 a870 6ed6 e1a9  O.......k..pn...
+00004660: 6d2f abd1 a8c9 4fac ca9a 885f d819 3c47  m/....O...._..<G
+00004670: 5e57 590b 5feb a751 73a9 5976 9049 5539  ^WY._..Qs.Yv.IU9
+00004680: 4ac6 e3f9 a8ca 8a73 8815 56f5 8fd4 e0c7  J......s..V.....
+00004690: 6391 b32d cf9f 2b76 6eb1 48cd caac 85f1  c..-..+vn.H.....
+000046a0: 37a7 e2d2 e86a 55fe 23e5 aaac fefa 7c79  7....jU.#.....|y
+000046b0: 97f3 ea02 251e 8bb2 68df 64d1 30a8 f2d5  ....%...h.d.0...
+000046c0: c7a7 33af b3c7 12ee fb5b 3ccd 725d 5b7e  ..3......[<.r][~
+000046d0: f1ca 5745 5ef3 861f db08 ca8d 70a0 fe3d  ..WE^.......p..=
+000046e0: 2f47 cb11 54ba bb95 1c7e ad03 80cd 3e67  /G..T....~....>g
+000046f0: 155c 23e5 7f67 f370 7477 7b28 e0e6 c413  .\#..g.ptw{(....
+00004700: 096a 765c 871f e255 9a4c 8443 e6fc 59b0  .jv\...U.L.C..Y.
+00004710: d7c6 fa1c b4fc f289 1ddb 7b56 9622 7812  ..........{V."x.
+00004720: 06df 39af bee4 9918 f812 9ea8 f9fa 593c  ..9...........Y<
+00004730: 0d08 1246 f100 1f39 ff2a ca7d 3cac c3b1  ...F...9.*.}<...
+00004740: 1813 2b59 2e50 0619 fcf7 c2b0 e47d 2c9a  ..+Y.P.......},.
+00004750: e01f 3916 f119 0632 3223 b13f eb51 3dc8  ..9....22#.?.Q=.
+00004760: 870e f7f6 9835 ec9e 977f 1587 f604 dd05  .....5..........
+00004770: 573d b063 f65c b6bf f1d7 9415 4fa7 16ac  W=.c.\......O...
+00004780: f368 1606 f973 d3f2 cad8 80b4 00be 3abc  .h...s........:.
+00004790: 6d59 93c3 9386 f145 89b8 72ce 4bb8 0cfc  mY.....E..r.K...
+000047a0: 1b54 85e8 5878 50d9 3751 6572 3385 9b52  .T..XxP.7Qer3..R
+000047b0: 578a a369 325b dcc4 0994 6eda 3701 4202  W..i2[....n.7.B.
+000047c0: 1c61 ba1c fd36 6bb3 bbdb 9abf 06d0 7950  .a...6k.......yP
+000047d0: a7b9 64a2 8fe3 15dc edff 1d18 8c48 54f9  ..d..........HT.
+000047e0: 20ca 884b 0530 e006 80be dccd a6b7 a317   ..K.0..........
+000047f0: 8094 ab90 0d86 c0b8 4cc8 d88d b8f7 2362  ........L.....#b
+00004800: 3762 eb47 246e c4ce 8f98 b811 0f7e 0419  7b.G$n.......~..
+00004810: e9de 8f98 b935 523f 626e 2246 40d6 e04d  .....5R?bn"F@..M
+00004820: 86c1 2bca acc3 4482 2577 bc41 9fcd 7541  ..+...D.%w.A..uA
+00004830: b8ea 08f1 5828 51f4 cd65 e578 3a8b bafb  ....X(Q..e.x:...
+00004840: 900f 76a7 7345 078a 27fd 8086 050e 8554  ..v.sE..'......T
+00004850: dbd3 e8d4 3238 5ca0 5386 683b 5146 7321  ....28\.S.h;QFs!
+00004860: cf79 83be 3e2e 3ae2 1a17 f429 2e37 4944  .y..>.:....).7ID
+00004870: ee74 a773 0d17 3420 9778 e93e 813d 8d4e  .t.s..4 .x.>.=.N
+00004880: 2d83 c305 a6f2 105c 4419 c1a5 9b6b 0969  -......\D....k.i
+00004890: e10d 86f4 e1d1 11d7 f0a0 4fe1 8997 1181  ..........O.....
+000048a0: bfd3 b906 0f1a 100f e9b1 3d0d 4e2d 8343  ..........=.N-.C
+000048b0: 472c 6a03 2c56 a28c ee1a ba4a a1af 0f8b  G,j.,V.....J....
+000048c0: 8eb8 8605 7d0a 4b32 f5ba 46e7 1a2c 6840  ....}.K2..F..,h@
+000048d0: 2ce4 09ed 6970 6a19 1c2c f361 b088 321a  ,...ipj..,.a..2.
+000048e0: 0bed 16f4 f561 d111 d7b0 a04f 6319 47a4  .....a.....Oc.G.
+000048f0: fa4e e71a 2c68 508b 0c99 4b34 38b5 0c0e  .N..,hP...K48...
+00004900: 96c5 3058 4419 772e cde8 128c 217d 7474  ..0XD.w.....!}tt
+00004910: c435 3ae8 d34b 701c 4dc6 d61f 5d77 7421  .5:..Kp.M...]wt!
+00004920: 830a 0d88 8abe c868 706a 191c 5442 e70c  .......hpj..TB..
+00004930: 30b1 4419 dd41 6492 6fd0 d7c7 4847 5c63  0.D..Ad.o...HG\c
+00004940: 84be 6ebd a11d a473 0d16 3420 16ba 1ad3  ..n....s..4 ....
+00004950: e0d4 3238 5896 c360 1165 3416 f26e dea0  ..28X..`.e4..n..
+00004960: af0f 8b8e b886 057d 0acb 6c1e cd97 f61f  .......}..l.....
+00004970: 9146 ba90 6184 06f5 caa2 af72 1a9d 5a06  .F..a......r..Z.
+00004980: 0792 50b7 8348 4851 4763 228f 6c23 2fb2  ..P..HHQGc".l#/.
+00004990: 0efb 3899 906b a094 534f b279 14f7 9132  ..8..k..SO.y...2
+000049a0: a50c 2a65 51ac c843 dc7b f1a9 6d71 690d  ..*eQ..C.{..mqi.
+000049b0: 25b8 5182 3aaf f81b aab8 7d99 4aa5 61ac  %.Q.:.....}.J.a.
+000049c0: 43ae 4243 a79e 7553 4f1c 9aec 8e13 a620  C.BC..uSO...... 
+000049d0: 270f 93be 980e 4fed 022e a681 8473 ac95  '.....O......s..
+000049e0: b3f5 c384 0a45 15d3 db5b 7d12 5ae5 2b4c  .....E...[}.Z.+L
+000049f0: 73b2 08ef 4cf9 0e92 ada1 c968 f65e 786a  s...L......h.^xj
+00004a00: 5b5c 4803 a968 f1cb d9cc bc98 2c04 1be5  [\H..h......,...
+00004a10: edc5 d3a7 a455 bec2 3399 f42f 52e6 6a1d  .....U..3../R.j.
+00004a20: 2d5b 5927 e4d5 bbf7 e253 dbe2 e21a 485c  -[Y'.....S....H\
+00004a30: c75a 5dcb 3943 b580 f2f6 e2a2 8277 ab92  .Z].9C.......w..
+00004a40: 14a3 8527 904c d18e 8a2d a813 6fa6 7992  ...'.L...-..o.y.
+00004a50: daae e052 11aa 7288 1d00 54a7 f81b 35f6  ...R..r...T...5.
+00004a60: e698 d6ae dd3c f496 22aa 77b7 315a 904a  .....<..".w.1Z.J
+00004a70: 328e 26ce 9a4d 5e11 3b15 3d93 9b25 f2a7  2.&..M^.;.=..%..
+00004a80: aab2 2819 e94d 344f 5fdb 155c 4603 29ec  ..(..M4O_..\F.).
+00004a90: d896 d831 d9fe d828 6f6f e750 f1bb 5549  ...1...(oo.P..UI
+00004aa0: 8ad1 3422 5477 a668 d739 b6b8 8ebd f9e4  ..4"Tw.h.9......
+00004ab0: c96b bb82 4b65 2081 1da3 2abd 915b 0ade  .k..Ke ...*..[..
+00004ac0: ae11 3a41 7c98 6d23 f29a bb57 f94b dcc3  ..:A|.m#...W.K..
+00004ad0: a03b 4698 0fef 6331 5b17 1149 de99 e48e  .;F...c1[..I....
+00004ae0: 8fca 8865 0689 df7b f1a9 6d71 f90c a4aa  ...e...{..mq....
+00004af0: e52e e43a 443e f487 9972 f6f2 4179 fb1f  ...:D>...r..Ay..
+00004b00: 7cd0 69f8 4ca8 b236 17e8 00a9 1404 4475  |.i.L..6......Du
+00004b10: a317 9fda 1617 d040 fa3a 4669 8a80 3ce5  .......@.:Fi..<.
+00004b20: 88ce 5e40 3ae4 aa08 42a7 02b4 8ce8 8fbf  ..^@:...B.......
+00004b30: 9dba fad2 5a77 548a 02e4 b590 be5c 2783  ....ZwT......\'.
+00004b40: 2c8b 4328 1948 5bcb 3aba 85e8 2f33 e5ec  ,.C(.H[.:.../3..
+00004b50: 2364 42ae 6e21 a270 372d e411 32d9 a685  #dB.n!.p7-..2...
+00004b60: 9405 e49f 2c48 56c2 bd97 90da 1697 d040  ....,HV........@
+00004b70: 7a3a 416d 8a3d e42d cdca db8b 080b 746d  z:Am.=.-......tm
+00004b80: b055 498a 4b12 2da8 3234 553b 2e58 4473  .UI.K.-.24U;.XDs
+00004b90: a1af 2c93 20a9 9172 a9eb ede6 b1cb 6ba8  ..,. ..r......k.
+00004ba0: 1d69 d4b0 8a97 b727 8dde 5e5e 3a44 dffc  .i.....'..^^:D..
+00004bb0: 3641 8be1 3575 3642 c674 a75f 855b f34e  6A..5u6B.t._.[.N
+00004bc0: 17c0 ae4a e8bc 3309 825e 42d6 89d4 f14e  ...J..3..^B....N
+00004bd0: ba8e 74e9 0da4 b8e1 544b 286e 458f 8a25  ..t.....TK(nE..%
+00004be0: e5ed a587 05ec 6e43 8ba1 4737 7c77 a66a  ......nC..G7|w.j
+00004bf0: d76d 2a45 f1a2 bb47 2641 f2a2 4720 ae97  .m*E...G&A..G ..
+00004c00: 1e7f e039 199e 345d b227 f64b 563f 15e7  ...9..4].'.KV?..
+00004c10: 2628 e1bc 4e1c 69c1 3bb6 c663 30f9 194e  &(..N.i.;..c0..N
+00004c20: f2a4 15b4 cf23 6fe1 404c 7f3b c1c1 2983  .....#o.@L.;..).
+00004c30: 6307 107f 6170 e4bc d55f e026 44dd 2fac  c...ap..._.&D./.
+00004c40: 7dbe 04bc 2ee0 a84c 9e85 aec3 0baf db3a  }......L.......:
+00004c50: 2b5a 38cc 02fb 770e 8e72 7b29 e074 6a0e  +Z8...w..r{).tj.
+00004c60: 0b15 1cf9 b605 9c10 7696 7a55 c029 60fd  ........v.zU.)`.
+00004c70: f110 cb03 3e73 be7b f72f 0000 00ff ff03  ....>s.{./......
+00004c80: 0050 4b03 0414 0006 0008 0000 0021 00f4  .PK..........!..
+00004c90: 2a3e 2362 0600 0028 1d00 0018 0000 0078  *>#b...(.......x
+00004ca0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
+00004cb0: 6574 352e 786d 6cac 994d 73a3 3810 86ef  et5.xml..Ms.8...
+00004cc0: 5bb5 ff81 e23e 6088 edd8 ae38 53e3 d898  [....>`....8S...
+00004cd0: 39cc d4d6 ce7e 9c09 9663 76c0 f282 f235  9....~...cv....5
+00004ce0: bf7e 5bb4 2450 2ba1 66ab c821 6577 bfdd  .~[.$P+.f..!ew..
+00004cf0: c88f 5aa2 4137 1f5f aad2 7b62 7553 f0f3  ..Z.A7._..{buS..
+00004d00: da8f 8289 efb1 73ce 0fc5 f961 edff f947  ......s....a...G
+00004d10: f261 e17b 8dc8 ce87 ace4 67b6 f65f 59e3  .a.{......g.._Y.
+00004d20: 7fbc fdf5 979b 675e 7f6f 4e8c 090f 329c  ......g^.oN...2.
+00004d30: 9bb5 7f12 e2b2 0ac3 263f b12a 6b02 7e61  ........&?.*k.~a
+00004d40: 67f0 1c79 5d65 02be d60f 6173 a959 7668  g..y]e....as.Yvh
+00004d50: 83aa 328c 2793 7958 65c5 d9c7 0cab fa67  ..2.'.yXe......g
+00004d60: 72f0 e3b1 c8d9 96e7 8f15 3b0b 4c52 b332  r.........;.LR.2
+00004d70: 1330 fee6 545c 1a9d adca 7f26 5d95 d5df  .0..T\.....&]...
+00004d80: 1f2f 1f72 5e5d 20c5 7d51 16e2 b54d ea7b  ./.r^] .}Q...M.{
+00004d90: 55be fafc 70e6 7576 5fc2 ef7e 89a6 59ae  U...p.uv_..~..Y.
+00004da0: 73b7 5f9c f455 91d7 bce1 4711 40ba 1007  s._..U....G.@...
+00004db0: eafe e665 b80c 21d3 ed4d cbe1 b7da 03d8  ...e..!..M......
+00004dc0: ec6b 56c1 3552 fe4f 36f3 c3db 9b43 013f  .kV.5R.O6....C.?
+00004dd0: 4ece 8857 b3e3 daff 14ad d2f8 4a3a da98  N..W........J:..
+00004de0: bf0a f6dc f43e 7b22 bbff c64a 960b 7680  .....>{"...J..v.
+00004df0: 29f4 bd1f 9c57 dff2 4c0e 7b09 f369 be7e  )....W..L.{..i.~
+00004e00: 9573 51a2 514e df3d e7df 65b2 cf10 3691  .sQ.QN.=..e...6.
+00004e10: 236a 93c8 cb66 b928 9ed8 1d2b 419d c44b  #j...f.(...+A..K
+00004e20: 2881 7fdb 91c8 cf30 8cd0 8ca3 ff59 8f29  (......0.....Y.)
+00004e30: 69a7 1c7e d97d d6b0 3b5e fe5d 1cc4 0906  i..~.}..;^.]....
+00004e40: 0643 39b0 63f6 588a dff9 73ca 8a87 9300  .C9.c.X...s.....
+00004e50: eb3c 98f9 5efe d808 5e19 1b70 96b8 5787  .<..^...^..p..W.
+00004e60: d72d 6b72 9867 185f 10cb 2be7 bc84 cbc0  .-kr.g._..+.....
+00004e70: 7faf 2a64 bdc2 3465 2f32 cbd5 62ea 7bcf  ..*d..4e/2..b.{.
+00004e80: ea4a 5130 8d67 d78b 2886 d48d 7895 205a  .JQ0.g..(...x. Z
+00004e90: 7c21 86b7 a3df 6622 bbbd a9f9 b307 7507  |!....f"......u.
+00004ea0: 799a 4b26 ab38 5a41 c1ff df81 c188 6496  y.K&.8ZA......d.
+00004eb0: 4f32 8dbc 9407 036e 00e8 d3ed 6c7a 133e  O2.....n....lz.>
+00004ec0: 01a4 5c49 3628 8171 19c9 c456 dcb9 8ac8  ..\I6(.q...V....
+00004ed0: 566c 5d45 6c2b 76ae e2ca 5624 ae82 8c74  Vl]El+v...V$...t
+00004ee0: ef2a 6676 8ed4 55cc 8d22 04b2 066f 3c0e  .*fv..U.."...o<.
+00004ef0: 5e99 66ed c72d 58c2 6483 be3e d76b c255  ^.f..-X.d..>.k.U
+00004f00: 2b64 15c9 d9da a261 dea6 9bce 03f2 fb77  +d.....a.......w
+00004f10: 549f a0e1 bad5 93e4 7b2a 4e7b 060b 0514  T.......{*N{....
+00004f20: c718 9526 d368 1464 f237 e81b 42a1 1506  ...&.h.d.7..B...
+00004f30: 051a 148a 2820 13bd a3fa 040d 8822 a285  ....( ......."..
+00004f40: 43d5 69cf 60b1 8015 3b06 0b99 46b3 2065  C.i.`...;...F. e
+00004f50: be41 df10 0bad 302c d080 2c66 b380 14da  .A....0,..,f....
+00004f60: 8eea 1334 2816 642e f654 9df6 0c16 0bb9  ...4(.d..T......
+00004f70: 538d b003 c934 9a05 dd7a d037 c442 2b0c  S....4...z.7.B+.
+00004f80: 0b34 a8ba 9839 7541 f509 1a90 0529 a23d  .4...9uA.....).=
+00004f90: 15a7 3d83 8562 3e0e 0a99 46a3 2063 d9a0  ..=..b>...F. c..
+00004fa0: 6f08 8556 c84d 9cee bfe8 432a d155 b7e7  o..V.M....C*.U..
+00004fb0: b5db ca4e 476a 8809 1a54 81d8 9bd2 9e8a  ...NGj...T......
+00004fc0: d39e c182 723d 0e14 9946 4321 03df a06f  ....r=...FC!...o
+00004fd0: 088a 56bc 0505 7d1a 0abd 21e9 4803 050d  ..V...}...!.H...
+00004fe0: 0885 2cda 3d15 a73d 8305 45f6 a623 2c1a  ..,.=..=..E..#,.
+00004ff0: 9946 4321 1bfb 067d 4350 b4e2 2d28 e87b  .FC!...}CP..-(.{
+00005000: 0f8a 8e34 50d0 a02a 6549 4a85 aad3 9ec1  ...4P..*eIJ.....
+00005010: a222 dbb5 11a8 c834 9aca 8274 31e8 1ba2  .".....4...t1...
+00005020: a215 6f51 419f a642 3758 1d69 a8a0 01a9  ..oQA..B7X.i....
+00005030: c444 bda7 eab4 67b0 a8c8 f673 941e 4fe6  .D....g....s..O.
+00005040: d15c c81c 6dda 8bac fd21 3046 6236 5965  .\..m....!0Fb6Ye
+00005050: 411e 57d3 8024 dd39 1189 b2a8 4221 eb78  A.W..$.9....B!.x
+00005060: efe8 d3be c586 3256 e38b ada0 6acd 4847  ......2V....j.HG
+00005070: bb89 dc46 9136 6746 d251 c120 751f 9e38  ...F.6gF.Q. u..8
+00005080: f71e 2722 5116 a442 578f 234f fb16 1bca  ..'"Q..BW.#O....
+00005090: 48ed 6a84 3de0 e2cd 7e55 39a1 5acd 8300  H.j.=...~U9.Z...
+000050a0: 5964 7746 d231 c18c 309d 7259 c5c1 8260  YdwF.1..0.rY...`
+000050b0: dc39 2189 b2c0 8f95 21e4 127b 479f f62d  .9!.....!..{G..-
+000050c0: 3695 913a d708 bb41 a442 5b57 e51c a482  6..:...A.B[W....
+000050d0: f1ed 7328 f6f1 2ac8 50b9 26f7 939d c96a  ..s(..*.P.&....j
+000050e0: b614 1d82 5422 daaa 3801 69df 6263 19a9  ....T"..8.i.bc..
+000050f0: 898d b031 442c b48b 55ce 412c 18df c782  ...1D,..U.A,....
+00005100: 1685 e52a a05b e7ce 64ed b0a8 1085 85de  ...*.[..d.......
+00005110: 979d 80b4 6fb1 b18c d4cf 46d8 2422 16e7  ....o.....F.$"..
+00005120: 591a 9d83 58b4 a45b 4368 e9aa 85ac 899d  Y...X..[Ch......
+00005130: ba64 4732 5116 b586 9ced 965e 22ed 67b0  .dG2Q......^".g.
+00005140: a98c d4da 46d8 2522 15da db2a e720 158c  ....F.%"...*. ..
+00005150: 5fbe b533 6d55 bc02 340b 96ce 72d2 d15d  _..3mU..4...r..]
+00005160: dda0 4501 a2cf 4066 405a 9ff6 2d36 a091  ..E...@f@Z..-6..
+00005170: dadc 083b 4604 44fb 5ce5 1c04 84f1 ef00  ...;F.D.\.......
+00005180: 4267 07c8 a920 1ddd 0152 21b8 b09c 372d  Bg... ...R!...7-
+00005190: 549f 9a21 4206 1bd0 482d 6f84 cd23 02a2  T..!B...H-o..#..
+000051a0: 3daf 720e 02c2 f877 00a1 d300 9a3a 1d8d  =.r....w.....:..
+000051b0: 8eee 00a9 1004 1493 0e62 6f46 d495 502f  .........boF..P/
+000051c0: 854d 68a4 f637 c246 1209 d1fe 5739 0709  .Mh..7.F....W9..
+000051d0: 61fc 3b84 d039 4048 4777 8454 8822 e42c  a.;..9@HGw.T.".,
+000051e0: 321a 909a 31d2 1a8a 47ea 84db 3c6b 1f09  2...1...G...<k..
+000051f0: d14e 5839 8708 1989 d99b 9545 6189 8239  .NX9.......Ea..9
+00005200: 7d8c 7442 121d a26e 59b4 c171 02d2 bec5  }.tB...nY..q....
+00005210: 2a9c 78a4 5eb8 cdf3 2e16 ec6a 07b1 6849  *.x.^......j..hI
+00005220: 8705 2de6 9615 2d26 fd3f 0712 4d90 a821  ..-...-&.?..M..!
+00005230: a9fd 3972 5e5e d280 5405 e0cb 7eeb 4dee  ..9r^^..T...~.M.
+00005240: 58af 7275 6fdc b5bf 31bd bdc7 a819 64a5  X.ruo...1.....d.
+00005250: 251d 2bab 4586 8300 ba39 9bac 6665 298b  %.+.E....9..fe).
+00005260: a643 f71e 2720 ed5b ec12 1aa9 4786 c31e  .C..' .[....G...
+00005270: f98c 095b 9c79 3888 694f a834 8374 9c56  ...[.y8.iO.4.t.V
+00005280: 5905 9905 466f ed26 6907 0773 6838 f4f1  Y...Fo.&i..sh8..
+00005290: db09 9007 5572 ecbd d2c1 d322 3c6f b964  ....Ur....."<o.d
+000052a0: 0fec 4b56 3f14 e7c6 2bd9 b13d d881 bb5f  ..KV?...+..=..._
+000052b0: 8d87 4193 003e 0b7e 91c7 3dd7 d056 dd73  ..A..>.~..=..V.s
+000052c0: 01c7 42fa db09 0e0f 19bc b89f 0470 8923  ..B..........p.#
+000052d0: e742 7f81 c1ca bcdf 9878 bc78 bc2e e0c0  .B.......x.x....
+000052e0: a83d 0f5c fb17 5e8b 3a2b 041c e980 fd07  .=.\..^.:+......
+000052f0: 0747 b9bd 1470 4633 874d 108e 3d45 01e7  .G...pF3.M..=E..
+00005300: 649d a55e 1570 1656 7f3e 44ed 3197 39e3  d..^.p.V.>D.1.9.
+00005310: bcfd 0f00 00ff ff03 0050 4b03 0414 0006  .........PK.....
+00005320: 0008 0000 0021 0098 9384 dbcb 0300 0039  .....!.........9
+00005330: 0f00 000d 0000 0078 6c2f 7374 796c 6573  .......xl/styles
+00005340: 2e78 6d6c cc57 596f db38 107e 2fb0 ff41  .xml.WYo.8.~/..A
+00005350: e0bb a2c3 966a 1996 8a38 8e80 02dd a240  .....j...8.....@
+00005360: 52a0 afb4 44d9 4479 1814 9d95 bbd8 ffde  R...D.Dy........
+00005370: 2125 d94a 7329 498f f58b c5d1 f09b 6f0e  !%.Js)I.......o.
+00005380: cd90 8b77 0d67 ce0d 5135 9522 45c1 998f  ...w.g..Q5."E...
+00005390: 1c22 0a59 52b1 49d1 e7eb dc9d 21a7 d658  .".YR.I.....!..X
+000053a0: 9498 4941 5274 2035 7a97 fdf5 6651 eb03  ..IARt 5z...fQ..
+000053b0: 2357 5b42 b403 10a2 4ed1 56eb dddc f3ea  #W[B....N.V.....
+000053c0: 624b 38ae cfe4 8e08 7853 49c5 b186 a5da  bK8.....xSI.....
+000053d0: 78f5 4e11 5cd6 6613 675e e8fb b1c7 3115  x.N.\.f.g^....1.
+000053e0: a845 98f3 620c 08c7 eaeb 7ee7 1692 efb0  .E..b.....~.....
+000053f0: a66b caa8 3e58 2ce4 f062 fe7e 23a4 c26b  .k..>X,..b.~#..k
+00005400: 0654 9b60 8a0b a709 6215 f616 ace8 8e11  .T.`....b.......
+00005410: 4e0b 256b 59e9 3300 f564 55d1 82dc e59a  N.%kY.3..dU.....
+00005420: 7889 878b 1312 c0be 0c29 883c 3f6c 1dcf  x........).<?l..
+00005430: 1695 14ba 760a b917 3a45 1340 37a4 e75f  ....v...:E.@7.._
+00005440: 85fc 47e4 e615 e404 b55a d9a2 fee6 dc60  ..G......Z.....`
+00005450: 0692 0079 d9a2 904c 2a47 43b0 c157 2b11  ...y...L*GC..W+.
+00005460: 9893 56e3 0233 ba56 d4a8 5598 5376 68c5  ..V..3.V..U.Svh.
+00005470: a111 d8fc 747a 9c42 b48c d033 3cee d8b1  ....tz.B...3<...
+00005480: fa8f d939 5714 b37b ad3c 09a8 36eb 14e5  ...9W..{.<..6...
+00005490: b96f 7f06 e2c4 fe49 540b 5e03 5dca d831  .o.....IT.^.]..1
+000054a0: 7853 1327 1064 0ba8 0b4d 94c8 61e1 74cf  xS.'.d...M..a.t.
+000054b0: d787 1d44 4940 09b7 de5a bd27 b437 0a1f  ...DI@...Z.'.7..
+000054c0: 8230 1abf a196 8c96 86c5 e662 981b df20  .0.........b... 
+000054d0: ac3b 1915 2569 4899 a278 6a81 075c 4d16  .;..%iH..xj..\M.
+000054e0: c6f0 7ac0 4c8c 1c4d 4d15 f967 5102 bfc9  ..z.L..MM..gQ...
+000054f0: 2c89 c364 16f8 d399 f5e1 390c 2c11 08f0  ,..d......9.,...
+00005500: 5aaa 127a 435f 9f21 38d7 8ab2 0523 9506  Z..zC_.!8....#..
+00005510: bf14 dd6c cdbf 963b e3a5 d41a 3ea1 6c51  ...l...;....>.lQ
+00005520: 52bc 9102 3353 5afd 8ee1 4ee8 29d0 3e52  R...3SZ...N.).>R
+00005530: a4b7 f0f9 f7b5 fc63 6c8c 89ce c228 7dcb  .......cl....(}.
+00005540: c552 19a5 0e94 7bc6 a3f4 5be7 eef7 ad73  .R....{...[....s
+00005550: 1242 5610 c6ae 8c73 5faa 63dc cc27 dc54  .BV....s_.c..'.T
+00005560: 8ed8 f39c ebf7 907c e8b2 e683 eb1f 21eb  .......|......!.
+00005570: dd63 1ba3 7661 6237 446b b187 b026 1fcf  .c..vab7Dk...&..
+00005580: c775 9aea 68e0 a1dd 0110 ec58 41f3 1cb2  .u..h......XA...
+00005590: 3aee 76f0 6ec7 0ea6 4999 f6d3 ad60 cf69  :.v.n...I....`.i
+000055a0: 75ce e846 70d2 2a64 0be8 49ed d2cc 1b4d  u..Fp.*d..I....M
+000055b0: 0bd3 ca0a 784b da0e d454 0f3b f36b e96c  ....xK...T.;.k.l
+000055c0: a5a2 dfc0 8fdf 4708 527b 2bf2 c6bf ae1e  ......G.R{+.....
+000055d0: 46bb fa71 cfd7 44e5 76bc 0e32 f092 7cfc  F..q..D.v..2..|.
+000055e0: c400 00fd bebc 9e2e 90a5 6d2f 230a e605  ..........m/#...
+000055f0: 04a1 6cef ade0 df46 7064 958f 48fd 1dca  ..l....Fpd..H...
+00005600: cf4f fdaf 8cf4 a062 e100 f3b3 7bc5 eb6a  .O.....b....{..j
+00005610: f316 a1ff 636d fe19 82af aacd c729 ff99  ....cm.......)..
+00005620: dab4 8312 46e3 60fe de9a bec7 39ea 9863  ....F.`.....9..c
+00005630: 668a 3e9a b6c9 06bd 6abd a70c 8e4f f74c  f.>.....j....O.L
+00005640: 5ec0 2c9b d32c b7a7 396d 6e18 76ca 1fad  ^.,..,..9mn.v...
+00005650: c048 2f49 85f7 4c5f 1f5f a6e8 f4fc 3729  .H/I..L_._....7)
+00005660: e99e 2747 ad4f f446 6a0b 91a2 d3f3 0773  ..'G.O.Fj......s
+00005670: 9c0a 6273 3424 8dfe 50c3 f907 fe9d bda2  ..bs4$..P.......
+00005680: 29fa f772 f936 595d e6a1 3bf3 9733 773a  )..r.6Y]..;..3w:
+00005690: 2191 9b44 cb95 1b4d 2f96 ab55 9ef8 a17f  !..D...M/..U....
+000056a0: f1df e0aa f38a 8b8e bd96 c190 0aa6 f39a  ................
+000056b0: c175 4875 ce76 2e5e 9d64 291a 2c5a faf6  .uHu.v.^.d).,Z..
+000056c0: 600b b487 dc93 30f6 cfa3 c077 f389 1fb8  `.....0....w....
+000056d0: d318 cfdc 593c 89dc 3c0a c255 3c5d 5e46  ....Y<..<..U<]^F
+000056e0: 7934 e01e bdf0 6ae5 7b41 d05f ad9a 209a  y4....j.{A._.. .
+000056f0: 6bca 09a3 a2cf 559f a1a1 1492 04cb 479c  k.....U.......G.
+00005700: f0fa 4c78 a73b 6ff6 1d00 00ff ff03 0050  ..Lx.;o........P
+00005710: 4b03 0414 0006 0008 0000 0021 000c 1434  K..........!...4
+00005720: 0041 0100 00bf 0400 0014 0000 0078 6c2f  .A...........xl/
+00005730: 7368 6172 6564 5374 7269 6e67 732e 786d  sharedStrings.xm
+00005740: 6c6c d441 6b83 3018 c6f1 fb60 df41 7219  ll.Ak.0....`.Ar.
+00005750: 14d6 18d3 581d 6a0f 85d1 0fb0 9d47 aaef  ....X.j......G..
+00005760: 6a40 a333 7174 df7e 0e0f 833c 1efd f9f7  j@.3qt.~...<....
+00005770: 351a b138 ddfb 2efa a6c9 99c1 964c ec63  5..8.........L.c
+00005780: 1691 ad87 c6d8 5bc9 dedf 5e9f 3316 39af  ......[...^.3.9.
+00005790: 6da3 bbc1 52c9 7ec8 b153 f5f8 5038 e7a3  m...R.~..S..P8..
+000057a0: e55a eb4a d67a 3fbe 70ee ea96 7aed f6c3  .Z.J.z?.p...z...
+000057b0: 4876 39f3 394c bdf6 cbe1 74e3 6e9c 4837  Hv9.9L....t.n.H7
+000057c0: ae25 f27d c793 384e 79af 8d65 513d ccd6  .%.}..8Ny..eQ=..
+000057d0: 974c aae5 beb3 355f 339d 5751 8a55 8533  .L....5_3.WQ.U.3
+000057e0: 55e1 2b3b d71d 9982 fbaa e07f b2aa 1b93  U.+;............
+000057f0: 90e8 3e7e 34da 6bf4 bad5 f646 a177 fa4a  ..>~4.k....F.w.J
+00005800: 5d24 b619 a6af b50c eb73 0897 1052 5850  ]$.......s...RXP
+00005810: 7a0d 1b21 2012 022b 8595 c2ea 88d5 11ab  z..! ..+........
+00005820: 0cab 0caa 2486 2a89 b192 5849 bc23 5e28  ....$.*...XI.#^(
+00005830: 703c 8e3a c070 5c7a 8e0f 939e 2fb0 59e9  p<.:.p\z..../.Y.
+00005840: 0e36 6707 74dc 1020 916c 119a da22 301c  .6g.t.. .l..."0.
+00005850: 26a1 c940 f28d 3940 121f 3043 ca91 c453  &..@..9@..0C...S
+00005860: f8ae 1210 0972 0051 2029 36b0 7d39 7c3e  .....r.Q )6.}9|>
+00005870: c636 74ff 5f12 5f7e 40d5 2f00 0000 ffff  .6t._._~@./.....
+00005880: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00005890: 1ae8 a8b7 9106 0000 e51b 0000 1300 0000  ................
+000058a0: 786c 2f74 6865 6d65 2f74 6865 6d65 312e  xl/theme/theme1.
+000058b0: 786d 6cec 59cd 6e1b 3710 be17 e83b 107b  xml.Y.n.7....;.{
+000058c0: 4f2c d992 6319 9103 4b96 e236 7162 d84a  O,..c...K..6qb.J
+000058d0: 8a1c a915 b5cb 98bb 5c90 941d dd8a e458  ........\......X
+000058e0: a040 d1b4 e8a5 406f 3d14 6d03 2440 2fe9  .@....@o=.m.$@/.
+000058f0: d3b8 4dd1 a640 5ea1 4372 2591 1615 db89  ..M..@^.Cr%.....
+00005900: 81fe c506 6c89 fb71 6638 3f1f 87dc abd7  ....l..qf8?.....
+00005910: 1e64 0c1d 1221 29cf 9b51 f572 2542 248f  .d...!)..Q.r%B$.
+00005920: f980 e649 33ba d3eb 5e5a 8b90 5438 1f60  ...I3...^Z..T8.`
+00005930: c673 d28c c644 46d7 36de 7fef 2a5e 5729  .s...DF.6...*^W)
+00005940: c908 82f9 b95c c7cd 2855 aa58 5f5a 9231  .....\..(U.X_Z.1
+00005950: 0c63 7999 1724 8767 432e 32ac e0ab 4896  .cy..$.gC.2...H.
+00005960: 0602 1f81 dc8c 2d2d 572a ab4b 19a6 7984  ......--W*.K..y.
+00005970: 729c 81d8 1ecc 4103 826e 0f87 3426 d1c6  r.....A..n..4&..
+00005980: 447c 8781 8e5c 493d 1033 b1af 8593 728e  D|...\I=.3....r.
+00005990: 831d 1c54 3542 8e65 9b09 7488 5933 024d  ...T5B.e..t.Y3.M
+000059a0: 037e d423 0f54 8418 960a 1e34 a38a f989  .~.#.T.....4....
+000059b0: 9636 ae2e e1f5 7212 530b e63a f3ba e6a7  .6....r.S..:....
+000059c0: 9c57 4e18 1c2c 1b9d 22e9 4f95 56bb b5c6  .WN..,..".O.V...
+000059d0: 95ad a97c 0360 6a1e d7e9 74da 9dea 549e  ...|.`j...t...T.
+000059e0: 01e0 3886 955a 5b5c 99b5 ee5a b535 91e9  ..8..Z[\...Z.5..
+000059f0: 80ec c779 d9ed 4abd 52f3 f18e fc95 399b  ...y..J.R.....9.
+00005a00: 1bad 56ab de28 6db1 420d c87e accd e1d7  ..V..(m.B..~....
+00005a10: 2aab b5cd 650f 6f40 165f 9fc3 d75a 9bed  *...e.o@._...Z..
+00005a20: f6aa 8737 208b 5f9d c377 af34 566b 3ede  ...7 ._..w.4Vk>.
+00005a30: 8052 46f3 8339 b40e 68b7 5b4a 9f42 869c  .RF..9..h.[J.B..
+00005a40: 6d07 e16b 005f ab94 f019 0ab2 619a 5d5a  m..k._......a.]Z
+00005a50: c590 e76a 51ae 65f8 3e17 5d00 6820 c38a  ...jQ.e.>.].h ..
+00005a60: e648 8d0b 32c4 31e4 711b 677d 4171 840a  .H..2.1.q.g}Aq..
+00005a70: 9c73 0903 95e5 4ab7 b202 7ff5 6fcd 7caa  .s....J.....o.|.
+00005a80: 69f5 789d 6067 9e1d 8ae5 dc90 b604 c958  i.x.`g.........X
+00005a90: d042 35a3 0f41 6ae4 405e 3dff fed5 f3a7  .B5..Aj.@^=.....
+00005aa0: e8d5 f327 c70f 9f1d 3ffc e9f8 d1a3 e387  ...'....?.......
+00005ab0: 3f5a 59de c46d 9c27 eec4 97df 7ef6 e7d7  ?ZY..m.'....~...
+00005ac0: 1fa3 3f9e 7ef3 f2f1 1761 bc74 f1bf fef0  ..?.~....a.t....
+00005ad0: c92f 3f7f 1e06 427d cdd6 ffe2 cb27 bf3d  ./?...B}.....'.=
+00005ae0: 7bf2 e2ab 4f7f ffee 7100 be29 70df 85f7  {...O...q..)p...
+00005af0: 6846 24ba 458e d01e cf60 6dc6 31be e5a4  hF$.E....`m.1...
+00005b00: 2fce 37a3 9762 eacd c029 c80e 88ee a8d4  /.7..b...)......
+00005b10: 03de 1a63 16c2 b588 efbc bb02 a825 04bc  ...c.........%..
+00005b20: 3eba efd9 ba9f 8a91 a201 cd37 d2cc 03ee  >..........7....
+00005b30: 70ce 5a5c 041d 7043 eb72 3cdc 1be5 4958  p.Z\..pC.r<...IX
+00005b40: b918 b9b8 3d8c 0f43 badb 38f7 42db 1915  ....=..C..8.B...
+00005b50: c0a9 90b2 f3be 6fa7 c433 7397 e15c e184  ......o..3s..\..
+00005b60: e444 21fd 8c1f 1012 9876 8f52 cfaf 3b34  .D!......v.R..;4
+00005b70: 165c f2a1 42f7 286a 611a 7449 8ff6 bd44  .\..B.(ja.tI...D
+00005b80: 9a4d daa6 19c4 651c 3210 42ed f966 e72e  .M....e.2.B..f..
+00005b90: 6a71 165a f516 39f4 9150 1098 058c ef11  jq.Z..9..P......
+00005ba0: e6b9 f13a 1e29 9c85 44f6 70c6 5c87 dfc4  ...:.)..D.p.\...
+00005bb0: 2a0d 19b9 3f16 b18b eb48 0591 4e08 e3a8  *...?....H..N...
+00005bc0: 3320 5286 e6dc 16b0 5e27 e837 30b0 5930  3 R.....^'.70.Y0
+00005bd0: ec3b 6c9c f948 a1e8 4148 e64d ccb9 8bdc  .;l..H..AH.M....
+00005be0: e207 ed14 6745 d066 9aa7 2ef6 0379 0029  ....gE.f.....y.)
+00005bf0: 8ad1 2e57 21f8 0ef7 2b44 7f87 38e0 7c61  ...W!...+D..8.|a
+00005c00: b8ef 52e2 85fb 7422 b843 13cf a459 82e8  ..R...t".C...Y..
+00005c10: 2723 1188 e575 c2fd 7a1c b321 2686 6580  '#...u..z..!&.e.
+00005c20: f03d 1ecf 68fe 3a52 6714 58fd 04a9 d7df  .=..h.:Rg.X.....
+00005c30: 91ba dd95 4e92 fa26 6c80 a1d2 da3e 41e5  ....N..&l....>A.
+00005c40: 8b70 ff42 02df c2a3 7c97 40cd cc93 e83b  .p.B....|.@....;
+00005c50: fe7e c7df d17f 9ebf 17d5 f2c5 b3f6 8ca8  .~..............
+00005c60: 81c3 677d bae9 dab3 854d fb90 32b6 afc6  ..g}.....M..2...
+00005c70: 8cdc 94a6 6f97 b03d 0dba 3068 0e14 e654  ....o..=..0h...T
+00005c80: 393d c415 297c 2c8f 081e 2e11 d8cc 4182  9=..)|,.......A.
+00005c90: ab8f a84a f753 5c40 8b5f 35c7 d544 96a2  ...J.S\@._5..D..
+00005ca0: 1389 0a2e a1f3 37c3 e638 4c4e c836 c75b  ......7..8LN.6.[
+00005cb0: 0a8d bd39 a9d6 f519 c632 87c4 6a87 0fec  ...9.....2..j...
+00005cc0: f08a 7b56 9d8a 3127 d7c4 9c87 278a 56b4  ..{V..1'....'.V.
+00005cd0: 80b3 2a5b b9f2 76ca aad6 aa85 6ef3 9756  ..*[..v.....n..V
+00005ce0: 35a6 1952 f496 365d 32c4 707e 6930 38f5  5..R..6]2.p~i08.
+00005cf0: 26f4 3d08 ba25 f0f2 2a5c 1a68 dbe1 3484  &.=..%..*\.h..4.
+00005d00: 1919 68bf db73 fc24 2c5a f585 8648 a618  ..h..s.$,Z...H..
+00005d10: ae24 6c8c f4ba e763 5435 419a e4ca 248d  .$l....cT5A...$.
+00005d20: 0231 d2e7 ce53 62e4 686b 68b1 6fa1 ed2c  .1...Sb.hkh.o..,
+00005d30: 4172 d5d5 16a8 9b44 ef6d a234 396c cfa2  Ar.....D.m.49l..
+00005d40: a4eb f644 39b2 dc2d 4e96 a3a3 66d4 a82f  ...D9..-N...f../
+00005d50: d723 14e3 a219 0de1 980d 1fb3 02a2 2e75  .#.............u
+00005d60: ab89 5902 b755 b112 36ed 4f2d 6693 aeb3  ..Y..U..6.O-f...
+00005d70: 6836 c269 5985 9b13 ebf7 b905 7b3c 5008  h6.iY.......{<P.
+00005d80: a9b6 b04c 6d6a 9847 650a b0dc 5c0a 18fb  ...Lmj.Ge...\...
+00005d90: 97eb e0d6 8b5a 80cd f437 b062 650d 92e1  .....Z...7.be...
+00005da0: 6fb3 02fc e887 960c 8724 566e b09d 1173  o........$Vn...s
+00005db0: 2b62 0025 95f2 9122 623f 1d1c a13e 1b89  +b.%..."b?...>..
+00005dc0: 3d0c e1d7 a90a eb19 5009 f721 8611 f417  =.......P..!....
+00005dd0: b8da d3de 368f 7c72 2e8b cebd 5033 383b  ....6.|r....P38;
+00005de0: 8e59 91e2 926e 7589 4e2a d9c2 4d1d 4f6d  .Y...nu.N*..M.Om
+00005df0: 30df acb5 c63c 585b d076 b3b8 f32f c594  0....<X[.v.../..
+00005e00: fc05 2dc5 4de3 ffd9 52f4 7e02 1714 2b03  ..-.M...R.~...+.
+00005e10: 1d81 18ee 9605 46ba 5e9b 1117 2ae5 c042  ......F.^...*..B
+00005e20: 454a e3ae 806b 35c3 1d90 2d70 3d0c 8f21  EJ...k5...-p=..!
+00005e30: a9e0 86db fc17 e450 ffb7 3567 6598 b286  .......P..5ge...
+00005e40: 73a6 daa3 0912 14f6 2395 0a42 7681 964c  s.......#..Bv..L
+00005e50: f69d 22ac 5aee 5d56 242b 0599 8c72 cc95  ..".Z.]V$+...r..
+00005e60: 8535 bb4f 0e09 eb69 0e5c d57b 7b84 5248  .5.O...i.\.{{.RH
+00005e70: 75c3 2625 0d18 dcc9 fcf3 bf97 15d4 4f74  u.&%..........Ot
+00005e80: 93f3 4fed 7c6c 319f b73d d0dd 816d b1ec  ..O.|l1..=...m..
+00005e90: fc33 f622 3587 f49d ada0 11dc fb4c 4f35  .3."5........LO5
+00005ea0: a583 d76c ece7 dc6a 2d63 cdad 78b9 7ee6  ...l...j-c..x.~.
+00005eb0: adb6 806b 26b8 5d56 9013 3115 31b3 2f4b  ...k&.]V..1.1./K
+00005ec0: f486 dae3 7bc0 ad08 de7d d8f6 0a41 565f  ....{....}...AV_
+00005ed0: b28d 07d2 0469 e9b1 0f8d 931d b4c9 a445  .....i.........E
+00005ee0: d986 a5ec 6e2f bc8d 821b f2b2 d39d ea85  ....n/..........
+00005ef0: 2a7d 934e f79c ce9e 3667 be3a af16 5fdf  *}.N....6g.:.._.
+00005f00: 7d9e cfd9 a587 3d5f bb9d 6ec0 d550 b427  }.....=_..n..P.'
+00005f10: 4b54 b747 9383 8c09 8c79 cfe6 be08 e3fd  KT.G.....y......
+00005f20: fb10 e82d 78e5 3062 4ada 9709 0fe0 5211  ...-x.0bJ.....R.
+00005f30: 4e19 f6a5 0514 bf0d ae99 baf1 1700 0000  N...............
+00005f40: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+00005f50: 2100 7584 b7f9 6301 0000 7c04 0000 2700  !.u...c...|...'.
+00005f60: 0000 786c 2f70 7269 6e74 6572 5365 7474  ..xl/printerSett
+00005f70: 696e 6773 2f70 7269 6e74 6572 5365 7474  ings/printerSett
+00005f80: 696e 6773 352e 6269 6eec 53cd 4ac3 4010  ings5.bin.S.J.@.
+00005f90: feb6 1151 2f7a f450 a478 8a87 424d 535b  ...Q/z.P.x..BMS[
+00005fa0: 8f69 934a 24c9 966c ea3d d285 0642 12d2  .i.J$..l.=...B..
+00005fb0: 14fc c19b 0fd2 37f1 457c 020f be82 ce56  ......7.E|.....V
+00005fc0: 850a 2214 bd08 ceb2 fb4d be99 f976 b3cb  .."......M...v..
+00005fd0: 3818 4180 23c0 296c f4d1 a1d9 4603 3a3c  8.A.#.)l....F.:<
+00005fe0: c20e 8d06 c525 4a24 b4ce 7084 cfc6 36b4  .....%J$..p...6.
+00005ff0: cd47 2c34 ed01 3506 86a7 9d7c 6b42 b88b  .G,4..5....|kB..
+00006000: 29ab 114e 9946 ab47 b515 0da5 f373 63ef  )..N.F.G.....sc.
+00006010: 120a 6b34 15be 909d b9c2 5c55 b7dd 607c  ..k4......\U..`|
+00006020: 089d dd6b 752c 9ea7 07df edbc bd12 547a  ...ku,........Tz
+00006030: 1f7b fcc2 71ff 25fe c80d acf3 e63a 250b  .{..q.%......:%.
+00006040: 3f3a 57bf b687 7d76 8b21 5ad4 3b0e 0630  ?:W...}v.!Z.;..0
+00006050: 6051 3735 8931 e8db 20cf 4417 3dea af26  `Q75.1.. .D.=..&
+00006060: f15d ca50 d1e3 2567 5097 a99c 1e55 b789  .].P..%gP....U..
+00006070: efe0 8e14 ddac 9857 fd24 c390 87be e0e3  .......W.$......
+00006080: 70e0 2074 84ed 7918 6749 2967 cae3 6522  p. t..y.gI)g..e"
+00006090: b32a ae92 3cc3 8887 5168 b911 4239 cbd3  .*..<...Qh..B9..
+000060a0: f992 e385 82f6 490b a3b8 90a5 486e 242c  ......I.....Hn$,
+000060b0: 1383 3ccd 4b3f 9fc8 37cf 302f 8b42 b969  ..<.K?..7.0/.B.i
+000060c0: 5c49 f000 be9c 2471 745d 4888 c80a 6c2b  \I....$qt]H...l+
+000060d0: b461 cf8b 545e 21e0 81b3 ee53 d6a9 e0c2  .a..T^!....S....
+000060e0: b4fd afee f615 0000 ffff 0300 504b 0304  ............PK..
+000060f0: 1400 0600 0800 0000 2100 7584 b7f9 6301  ........!.u...c.
+00006100: 0000 7c04 0000 2700 0000 786c 2f70 7269  ..|...'...xl/pri
+00006110: 6e74 6572 5365 7474 696e 6773 2f70 7269  nterSettings/pri
+00006120: 6e74 6572 5365 7474 696e 6773 312e 6269  nterSettings1.bi
+00006130: 6eec 53cd 4ac3 4010 feb6 1151 2f7a f450  n.S.J.@....Q/z.P
+00006140: a478 8a87 424d 535b 8f69 934a 24c9 966c  .x..BMS[.i.J$..l
+00006150: ea3d d285 0642 12d2 14fc c19b 0fd2 37f1  .=...B........7.
+00006160: 457c 020f be82 ce56 850a 2214 bd08 ceb2  E|.....V..".....
+00006170: fb4d be99 f976 b3cb 3818 4180 23c0 296c  .M...v..8.A.#.)l
+00006180: f4d1 a1d9 4603 3a3c c20e 8d06 c525 4a24  ....F.:<.....%J$
+00006190: b4ce 7084 cfc6 36b4 cd47 2c34 ed01 3506  ..p...6..G,4..5.
+000061a0: 86a7 9d7c 6b42 b88b 29ab 114e 9946 ab47  ...|kB..)..N.F.G
+000061b0: b515 0da5 f373 63ef 120a 6b34 15be 909d  .....sc...k4....
+000061c0: b9c2 5c55 b7dd 607c 089d dd6b 752c 9ea7  ..\U..`|...ku,..
+000061d0: 07df edbc bd12 547a 1f7b fcc2 71ff 25fe  ......Tz.{..q.%.
+000061e0: c80d acf3 e63a 250b 3f3a 57bf b687 7d76  .....:%.?:W...}v
+000061f0: 8b21 5ad4 3b0e 0630 6051 3735 8931 e8db  .!Z.;..0`Q75.1..
+00006200: 20cf 4417 3dea af26 f15d ca50 d1e3 2567   .D.=..&.].P..%g
+00006210: 5097 a99c 1e55 b789 efe0 8e14 ddac 9857  P....U.........W
+00006220: fd24 c390 87be e0e3 70e0 2074 84ed 7918  .$......p. t..y.
+00006230: 6749 2967 cae3 6522 b32a ae92 3cc3 8887  gI)g..e".*..<...
+00006240: 5168 b911 4239 cbd3 f992 e385 82f6 490b  Qh..B9........I.
+00006250: a3b8 90a5 486e 242c 1383 3ccd 4b3f 9fc8  ....Hn$,..<.K?..
+00006260: 37cf 302f 8b42 b969 5c49 f000 be9c 2471  7.0/.B.i\I....$q
+00006270: 745d 4888 c80a 6c2b b461 cf8b 545e 21e0  t]H...l+.a..T^!.
+00006280: 81b3 ee53 d6a9 e0c2 b4fd afee f615 0000  ...S............
+00006290: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+000062a0: 2100 5c96 2722 c300 0000 2801 0000 1e00  !.\.'"....(.....
+000062b0: 0801 6375 7374 6f6d 586d 6c2f 5f72 656c  ..customXml/_rel
+000062c0: 732f 6974 656d 322e 786d 6c2e 7265 6c73  s/item2.xml.rels
+000062d0: 20a2 0401 28a0 0001 0000 0000 0000 0000   ...(...........
 000062e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000062f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006380: 0000 0084 cfc1 6ac3 300c 06e0 7ba1 ef60  ......j.0...{..`
-00006390: 745f 9cf6 304a 89d3 4b19 e436 460b bd1a  t_..0J..K..6F...
-000063a0: 4749 4c63 cb58 4a69 df7e a6a7 1606 3b4a  GILc.XJi.~....;J
-000063b0: 42df 2f35 877b 98d5 0d33 7b8a 0636 550d  B./5.{...3{..6U.
-000063c0: 0aa3 a3de c7d1 c0f9 f4f5 b103 c562 636f  .............bco
-000063d0: 678a 68e0 810c 8776 bd6a 7e70 b652 9678  g.h....v.j~p.R.x
-000063e0: f289 5551 221b 9844 d25e 6b76 1306 cb15  ..UQ"..D.^kv....
-000063f0: 258c 6532 500e 564a 9947 9dac bbda 11f5  %.e2P.VJ.G......
-00006400: b6ae 3f75 7e35 a07d 3355 d71b c85d bf01  ..?u~5.}3U...]..
-00006410: 757a a492 fcbf 4dc3 e01d 1ec9 2d01 a3fc  uz....M.....-...
-00006420: 11a1 ddc2 42e1 12e6 ef4c 898b 6cf3 8862  ....B....L..l..b
-00006430: c00b 8667 6b5b 957b 41b7 8d7e fbaf fd05  ...gk[.{A..~....
-00006440: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00006450: 0000 2100 743f 397a c200 0000 2801 0000  ..!.t?9z....(...
-00006460: 1e00 0801 6375 7374 6f6d 586d 6c2f 5f72  ....customXml/_r
-00006470: 656c 732f 6974 656d 312e 786d 6c2e 7265  els/item1.xml.re
-00006480: 6c73 20a2 0401 28a0 0001 0000 0000 0000  ls ...(.........
-00006490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000064a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000064b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000064c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000064d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000063a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000063b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000063c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000063d0: 0000 0000 0000 0000 84cf c16a c330 0c06  ...........j.0..
+000063e0: e07b a1ef 6074 5f9c f630 4a89 d34b 19e4  .{..`t_..0J..K..
+000063f0: 3646 0bbd 1a47 494c 63cb 584a 69df 7ea6  6F...GILc.XJi.~.
+00006400: a716 063b 4a42 df2f 3587 7b98 d50d 337b  ...;JB./5.{...3{
+00006410: 8a06 3655 0d0a a3a3 dec7 d1c0 f9f4 f5b1  ..6U............
+00006420: 03c5 6263 6f67 8a68 e081 0c87 76bd 6a7e  ..bcog.h....v.j~
+00006430: 70b6 5296 78f2 8955 5122 1b98 44d2 5e6b  p.R.x..UQ"..D.^k
+00006440: 7613 06cb 1525 8c65 3250 0e56 4a99 479d  v....%.e2P.VJ.G.
+00006450: acbb da11 f5b6 ae3f 757e 35a0 7d33 55d7  .......?u~5.}3U.
+00006460: 1bc8 5dbf 0175 7aa4 92fc bf4d c3e0 1d1e  ..]..uz....M....
+00006470: c92d 01a3 fc11 a1dd c242 e112 e6ef 4c89  .-.......B....L.
+00006480: 8b6c f388 62c0 0b86 676b 5b95 7b41 b78d  .l..b...gk[.{A..
+00006490: 7efb affd 0500 00ff ff03 0050 4b03 0414  ~..........PK...
+000064a0: 0006 0008 0000 0021 0074 3f39 7ac2 0000  .......!.t?9z...
+000064b0: 0028 0100 001e 0008 0163 7573 746f 6d58  .(.......customX
+000064c0: 6d6c 2f5f 7265 6c73 2f69 7465 6d31 2e78  ml/_rels/item1.x
+000064d0: 6d6c 2e72 656c 7320 a204 0128 a000 0100  ml.rels ...(....
 000064e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000064f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006580: 0000 0000 0000 0000 0000 84cf c18a 0231  ...............1
-00006590: 0c06 e0bb e03b 94dc 9dce 7810 91e9 7859  .....;....x...xY
-000065a0: 16bc 89b8 e0b5 7432 33c5 6953 9a28 faf6  ......t23.iS.(..
-000065b0: 164f 2b2c ec31 09f9 fea4 dd3f c2ac ee98  .O+,.1.....?....
-000065c0: d953 34d0 5435 288c 8e7a 1f47 033f e7ef  .S4.T5(..z.G.?..
-000065d0: d516 148b 8dbd 9d29 a281 2732 ecbb e5a2  .......)..'2....
-000065e0: 3de1 6ca5 2cf1 e413 aba2 4436 3089 a49d  =.l.,.....D60...
-000065f0: d6ec 260c 962b 4a18 cb64 a01c ac94 328f  ..&..+J..d....2.
-00006600: 3a59 77b5 23ea 755d 6f74 fe6d 40f7 61aa  :Yw.#.u]ot.m@.a.
-00006610: 436f 201f fa06 d4f9 994a f2ff 360d 8377  Co ......J..6..w
-00006620: f845 ee16 30ca 1f11 dadd 5828 5cc2 7ccc  .E..0.....X(\.|.
-00006630: 94b8 c836 8f28 06bc 6078 b79a aadc 0bba  ...6.(..`x......
-00006640: 6bf5 c77f dd0b 0000 ffff 0300 504b 0304  k...........PK..
-00006650: 1400 0600 0800 0000 2100 7584 b7f9 6301  ........!.u...c.
-00006660: 0000 7c04 0000 2700 0000 786c 2f70 7269  ..|...'...xl/pri
-00006670: 6e74 6572 5365 7474 696e 6773 2f70 7269  nterSettings/pri
-00006680: 6e74 6572 5365 7474 696e 6773 322e 6269  nterSettings2.bi
-00006690: 6eec 53cd 4ac3 4010 feb6 1151 2f7a f450  n.S.J.@....Q/z.P
-000066a0: a478 8a87 424d 535b 8f69 934a 24c9 966c  .x..BMS[.i.J$..l
-000066b0: ea3d d285 0642 12d2 14fc c19b 0fd2 37f1  .=...B........7.
-000066c0: 457c 020f be82 ce56 850a 2214 bd08 ceb2  E|.....V..".....
-000066d0: fb4d be99 f976 b3cb 3818 4180 23c0 296c  .M...v..8.A.#.)l
-000066e0: f4d1 a1d9 4603 3a3c c20e 8d06 c525 4a24  ....F.:<.....%J$
-000066f0: b4ce 7084 cfc6 36b4 cd47 2c34 ed01 3506  ..p...6..G,4..5.
-00006700: 86a7 9d7c 6b42 b88b 29ab 114e 9946 ab47  ...|kB..)..N.F.G
-00006710: b515 0da5 f373 63ef 120a 6b34 15be 909d  .....sc...k4....
-00006720: b9c2 5c55 b7dd 607c 089d dd6b 752c 9ea7  ..\U..`|...ku,..
-00006730: 07df edbc bd12 547a 1f7b fcc2 71ff 25fe  ......Tz.{..q.%.
-00006740: c80d acf3 e63a 250b 3f3a 57bf b687 7d76  .....:%.?:W...}v
-00006750: 8b21 5ad4 3b0e 0630 6051 3735 8931 e8db  .!Z.;..0`Q75.1..
-00006760: 20cf 4417 3dea af26 f15d ca50 d1e3 2567   .D.=..&.].P..%g
-00006770: 5097 a99c 1e55 b789 efe0 8e14 ddac 9857  P....U.........W
-00006780: fd24 c390 87be e0e3 70e0 2074 84ed 7918  .$......p. t..y.
-00006790: 6749 2967 cae3 6522 b32a ae92 3cc3 8887  gI)g..e".*..<...
-000067a0: 5168 b911 4239 cbd3 f992 e385 82f6 490b  Qh..B9........I.
-000067b0: a3b8 90a5 486e 242c 1383 3ccd 4b3f 9fc8  ....Hn$,..<.K?..
-000067c0: 37cf 302f 8b42 b969 5c49 f000 be9c 2471  7.0/.B.i\I....$q
-000067d0: 745d 4888 c80a 6c2b b461 cf8b 545e 21e0  t]H...l+.a..T^!.
-000067e0: 81b3 ee53 d6a9 e0c2 b4fd afee f615 0000  ...S............
-000067f0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00006800: 2100 7584 b7f9 6301 0000 7c04 0000 2700  !.u...c...|...'.
-00006810: 0000 786c 2f70 7269 6e74 6572 5365 7474  ..xl/printerSett
-00006820: 696e 6773 2f70 7269 6e74 6572 5365 7474  ings/printerSett
-00006830: 696e 6773 332e 6269 6eec 53cd 4ac3 4010  ings3.bin.S.J.@.
-00006840: feb6 1151 2f7a f450 a478 8a87 424d 535b  ...Q/z.P.x..BMS[
-00006850: 8f69 934a 24c9 966c ea3d d285 0642 12d2  .i.J$..l.=...B..
-00006860: 14fc c19b 0fd2 37f1 457c 020f be82 ce56  ......7.E|.....V
-00006870: 850a 2214 bd08 ceb2 fb4d be99 f976 b3cb  .."......M...v..
-00006880: 3818 4180 23c0 296c f4d1 a1d9 4603 3a3c  8.A.#.)l....F.:<
-00006890: c20e 8d06 c525 4a24 b4ce 7084 cfc6 36b4  .....%J$..p...6.
-000068a0: cd47 2c34 ed01 3506 86a7 9d7c 6b42 b88b  .G,4..5....|kB..
-000068b0: 29ab 114e 9946 ab47 b515 0da5 f373 63ef  )..N.F.G.....sc.
-000068c0: 120a 6b34 15be 909d b9c2 5c55 b7dd 607c  ..k4......\U..`|
-000068d0: 089d dd6b 752c 9ea7 07df edbc bd12 547a  ...ku,........Tz
-000068e0: 1f7b fcc2 71ff 25fe c80d acf3 e63a 250b  .{..q.%......:%.
-000068f0: 3f3a 57bf b687 7d76 8b21 5ad4 3b0e 0630  ?:W...}v.!Z.;..0
-00006900: 6051 3735 8931 e8db 20cf 4417 3dea af26  `Q75.1.. .D.=..&
-00006910: f15d ca50 d1e3 2567 5097 a99c 1e55 b789  .].P..%gP....U..
-00006920: efe0 8e14 ddac 9857 fd24 c390 87be e0e3  .......W.$......
-00006930: 70e0 2074 84ed 7918 6749 2967 cae3 6522  p. t..y.gI)g..e"
-00006940: b32a ae92 3cc3 8887 5168 b911 4239 cbd3  .*..<...Qh..B9..
-00006950: f992 e385 82f6 490b a3b8 90a5 486e 242c  ......I.....Hn$,
-00006960: 1383 3ccd 4b3f 9fc8 37cf 302f 8b42 b969  ..<.K?..7.0/.B.i
-00006970: 5c49 f000 be9c 2471 745d 4888 c80a 6c2b  \I....$qt]H...l+
-00006980: b461 cf8b 545e 21e0 81b3 ee53 d6a9 e0c2  .a..T^!....S....
-00006990: b4fd afee f615 0000 ffff 0300 504b 0304  ............PK..
-000069a0: 1400 0600 0800 0000 2100 7584 b7f9 6301  ........!.u...c.
-000069b0: 0000 7c04 0000 2700 0000 786c 2f70 7269  ..|...'...xl/pri
-000069c0: 6e74 6572 5365 7474 696e 6773 2f70 7269  nterSettings/pri
-000069d0: 6e74 6572 5365 7474 696e 6773 362e 6269  nterSettings6.bi
-000069e0: 6eec 53cd 4ac3 4010 feb6 1151 2f7a f450  n.S.J.@....Q/z.P
-000069f0: a478 8a87 424d 535b 8f69 934a 24c9 966c  .x..BMS[.i.J$..l
-00006a00: ea3d d285 0642 12d2 14fc c19b 0fd2 37f1  .=...B........7.
-00006a10: 457c 020f be82 ce56 850a 2214 bd08 ceb2  E|.....V..".....
-00006a20: fb4d be99 f976 b3cb 3818 4180 23c0 296c  .M...v..8.A.#.)l
-00006a30: f4d1 a1d9 4603 3a3c c20e 8d06 c525 4a24  ....F.:<.....%J$
-00006a40: b4ce 7084 cfc6 36b4 cd47 2c34 ed01 3506  ..p...6..G,4..5.
-00006a50: 86a7 9d7c 6b42 b88b 29ab 114e 9946 ab47  ...|kB..)..N.F.G
-00006a60: b515 0da5 f373 63ef 120a 6b34 15be 909d  .....sc...k4....
-00006a70: b9c2 5c55 b7dd 607c 089d dd6b 752c 9ea7  ..\U..`|...ku,..
-00006a80: 07df edbc bd12 547a 1f7b fcc2 71ff 25fe  ......Tz.{..q.%.
-00006a90: c80d acf3 e63a 250b 3f3a 57bf b687 7d76  .....:%.?:W...}v
-00006aa0: 8b21 5ad4 3b0e 0630 6051 3735 8931 e8db  .!Z.;..0`Q75.1..
-00006ab0: 20cf 4417 3dea af26 f15d ca50 d1e3 2567   .D.=..&.].P..%g
-00006ac0: 5097 a99c 1e55 b789 efe0 8e14 ddac 9857  P....U.........W
-00006ad0: fd24 c390 87be e0e3 70e0 2074 84ed 7918  .$......p. t..y.
-00006ae0: 6749 2967 cae3 6522 b32a ae92 3cc3 8887  gI)g..e".*..<...
-00006af0: 5168 b911 4239 cbd3 f992 e385 82f6 490b  Qh..B9........I.
-00006b00: a3b8 90a5 486e 242c 1383 3ccd 4b3f 9fc8  ....Hn$,..<.K?..
-00006b10: 37cf 302f 8b42 b969 5c49 f000 be9c 2471  7.0/.B.i\I....$q
-00006b20: 745d 4888 c80a 6c2b b461 cf8b 545e 21e0  t]H...l+.a..T^!.
-00006b30: 81b3 ee53 d6a9 e0c2 b4fd afee f615 0000  ...S............
-00006b40: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00006b50: 2100 7584 b7f9 6301 0000 7c04 0000 2700  !.u...c...|...'.
-00006b60: 0000 786c 2f70 7269 6e74 6572 5365 7474  ..xl/printerSett
-00006b70: 696e 6773 2f70 7269 6e74 6572 5365 7474  ings/printerSett
-00006b80: 696e 6773 372e 6269 6eec 53cd 4ac3 4010  ings7.bin.S.J.@.
-00006b90: feb6 1151 2f7a f450 a478 8a87 424d 535b  ...Q/z.P.x..BMS[
-00006ba0: 8f69 934a 24c9 966c ea3d d285 0642 12d2  .i.J$..l.=...B..
-00006bb0: 14fc c19b 0fd2 37f1 457c 020f be82 ce56  ......7.E|.....V
-00006bc0: 850a 2214 bd08 ceb2 fb4d be99 f976 b3cb  .."......M...v..
-00006bd0: 3818 4180 23c0 296c f4d1 a1d9 4603 3a3c  8.A.#.)l....F.:<
-00006be0: c20e 8d06 c525 4a24 b4ce 7084 cfc6 36b4  .....%J$..p...6.
-00006bf0: cd47 2c34 ed01 3506 86a7 9d7c 6b42 b88b  .G,4..5....|kB..
-00006c00: 29ab 114e 9946 ab47 b515 0da5 f373 63ef  )..N.F.G.....sc.
-00006c10: 120a 6b34 15be 909d b9c2 5c55 b7dd 607c  ..k4......\U..`|
-00006c20: 089d dd6b 752c 9ea7 07df edbc bd12 547a  ...ku,........Tz
-00006c30: 1f7b fcc2 71ff 25fe c80d acf3 e63a 250b  .{..q.%......:%.
-00006c40: 3f3a 57bf b687 7d76 8b21 5ad4 3b0e 0630  ?:W...}v.!Z.;..0
-00006c50: 6051 3735 8931 e8db 20cf 4417 3dea af26  `Q75.1.. .D.=..&
-00006c60: f15d ca50 d1e3 2567 5097 a99c 1e55 b789  .].P..%gP....U..
-00006c70: efe0 8e14 ddac 9857 fd24 c390 87be e0e3  .......W.$......
-00006c80: 70e0 2074 84ed 7918 6749 2967 cae3 6522  p. t..y.gI)g..e"
-00006c90: b32a ae92 3cc3 8887 5168 b911 4239 cbd3  .*..<...Qh..B9..
-00006ca0: f992 e385 82f6 490b a3b8 90a5 486e 242c  ......I.....Hn$,
-00006cb0: 1383 3ccd 4b3f 9fc8 37cf 302f 8b42 b969  ..<.K?..7.0/.B.i
-00006cc0: 5c49 f000 be9c 2471 745d 4888 c80a 6c2b  \I....$qt]H...l+
-00006cd0: b461 cf8b 545e 21e0 81b3 ee53 d6a9 e0c2  .a..T^!....S....
-00006ce0: b4fd afee f615 0000 ffff 0300 504b 0304  ............PK..
-00006cf0: 1400 0600 0800 0000 2100 7584 b7f9 6301  ........!.u...c.
-00006d00: 0000 7c04 0000 2700 0000 786c 2f70 7269  ..|...'...xl/pri
-00006d10: 6e74 6572 5365 7474 696e 6773 2f70 7269  nterSettings/pri
-00006d20: 6e74 6572 5365 7474 696e 6773 382e 6269  nterSettings8.bi
-00006d30: 6eec 53cd 4ac3 4010 feb6 1151 2f7a f450  n.S.J.@....Q/z.P
-00006d40: a478 8a87 424d 535b 8f69 934a 24c9 966c  .x..BMS[.i.J$..l
-00006d50: ea3d d285 0642 12d2 14fc c19b 0fd2 37f1  .=...B........7.
-00006d60: 457c 020f be82 ce56 850a 2214 bd08 ceb2  E|.....V..".....
-00006d70: fb4d be99 f976 b3cb 3818 4180 23c0 296c  .M...v..8.A.#.)l
-00006d80: f4d1 a1d9 4603 3a3c c20e 8d06 c525 4a24  ....F.:<.....%J$
-00006d90: b4ce 7084 cfc6 36b4 cd47 2c34 ed01 3506  ..p...6..G,4..5.
-00006da0: 86a7 9d7c 6b42 b88b 29ab 114e 9946 ab47  ...|kB..)..N.F.G
-00006db0: b515 0da5 f373 63ef 120a 6b34 15be 909d  .....sc...k4....
-00006dc0: b9c2 5c55 b7dd 607c 089d dd6b 752c 9ea7  ..\U..`|...ku,..
-00006dd0: 07df edbc bd12 547a 1f7b fcc2 71ff 25fe  ......Tz.{..q.%.
-00006de0: c80d acf3 e63a 250b 3f3a 57bf b687 7d76  .....:%.?:W...}v
-00006df0: 8b21 5ad4 3b0e 0630 6051 3735 8931 e8db  .!Z.;..0`Q75.1..
-00006e00: 20cf 4417 3dea af26 f15d ca50 d1e3 2567   .D.=..&.].P..%g
-00006e10: 5097 a99c 1e55 b789 efe0 8e14 ddac 9857  P....U.........W
-00006e20: fd24 c390 87be e0e3 70e0 2074 84ed 7918  .$......p. t..y.
-00006e30: 6749 2967 cae3 6522 b32a ae92 3cc3 8887  gI)g..e".*..<...
-00006e40: 5168 b911 4239 cbd3 f992 e385 82f6 490b  Qh..B9........I.
-00006e50: a3b8 90a5 486e 242c 1383 3ccd 4b3f 9fc8  ....Hn$,..<.K?..
-00006e60: 37cf 302f 8b42 b969 5c49 f000 be9c 2471  7.0/.B.i\I....$q
-00006e70: 745d 4888 c80a 6c2b b461 cf8b 545e 21e0  t]H...l+.a..T^!.
-00006e80: 81b3 ee53 d6a9 e0c2 b4fd afee f615 0000  ...S............
-00006e90: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00006ea0: 2100 559f 35f5 d409 0000 8c30 0000 1300  !.U.5......0....
-00006eb0: 2800 6375 7374 6f6d 586d 6c2f 6974 656d  (.customXml/item
-00006ec0: 312e 786d 6c20 a224 0028 a020 0000 0000  1.xml .$.(. ....
-00006ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006ee0: 0000 0000 0000 0000 0000 0000 00ec 5bdd  ..............[.
-00006ef0: 929b 4616 be4f 55de 81d2 5e33 8040 0254  ..F..OU...^3.@.T
-00006f00: 9653 638d bdeb 8a1d bb32 daec dea5 9aa6  .Sc......2......
-00006f10: 19b1 4680 e966 4653 a97d a47d 8abc 584e  ..F..fFS.}.}..XN
-00006f20: 77f3 8f7e 004d 36a9 ad4d 2e32 9238 a74f  w..~.M6..M.2.8.O
-00006f30: 9fff f31d f2ea bbc3 3e52 1e49 46c3 245e  ........>R.IF.$^
-00006f40: cf8c 1b7d a690 1827 7e18 3fac 6739 0b54  ...}...'~.?.g9.T
-00006f50: 67f6 ddeb 5798 ad70 1233 12b3 ed73 4aee  g...W..p.3...sJ.
-00006f60: f18e ec91 025f febc 9ecd 943d aafe db78  ....._.....=...x
-00006f70: e807 b427 ebd9 5d82 f33d 9025 e2b1 c6cf  ...'..]..=.%....
-00006f80: efef d633 fda0 1bf0 affe ce34 0dc3 7db3  ...3.......4..}.
-00006f90: 9c6f 4c7b 6159 ae7b 676f de59 cead bbb9  .oL{aY.{go.Y....
-00006fa0: 7396 ce62 d9a5 fda9 12d7 e8fe 7447 28ce  s..b........tG(.
-00006fb0: c294 89db 6c32 8232 25ce c963 a2f8 a520  ....l2.2%..c... 
-00006fc0: 375d 927b 9ca4 20a9 f8ba 5004 17ce 70e6  7].{.. ...P...p.
-00006fd0: fe7c ae9b ba67 064b d35d ce1d 8275 ec2c  .|...g.K.]...u.,
-00006fe0: dc39 b65c dd01 3d81 e662 bac2 6c3d db31  .9.\..=..b..l=.1
-00006ff0: 96ae 348d 0abd d09b 7d88 b384 2601 bbc1  ..4.....}...&...
-00007000: c95e 4b82 20c4 449b ebfa 52db 1386 7cc4  .^K. .D...R...|.
-00007010: 90d6 d044 c968 8fa6 304a 3390 3e63 21a1  ...D.h..0J3.>c!.
-00007020: 82f9 2d63 59e8 e58c d0d9 eb6f bf79 75a0  ..-cY......o.yu.
-00007030: fe4a 4aa5 3094 3d10 c6ad 4253 84e1 c2e3  .JJ.0.=...BS....
-00007040: 85ae cf12 caca 9204 eece b29c 888f 4148  ..............AH
-00007050: 229f 0abb 9aae 6393 00e9 a66b 390b cf31  ".....c....k9..1
-00007060: 75dd f43d ecba f3b9 4d40 a733 25a6 73e9  u..=....M@.3%.s.
-00007070: 3331 35e5 1f52 9920 6f25 d8d3 d3d3 cd93  315..R. o%......
-00007080: 7993 640f 5c77 86f6 cf8f 1fa4 e395 0a3b  y.d.\w.........;
-00007090: d0e1 cfa6 d7de 57ca 0772 af67 9ead 2fd1  ......W..r.g../.
-000070a0: 3230 55dd 0e3c d5f2 4c47 7516 fa42 45b6  20U..<..LGu..BE.
-000070b0: bd58 62c7 703d 0b95 32c2 fdc0 cf0d c740  .Xb.p=..2......@
-000070c0: fec2 5617 ee62 ae5a 3afc 8502 14a8 b66e  ..V..b.Z:......n
-000070d0: 221f 5ccc 45d8 a9cc 15ee d324 634a 5c1b  ".\.E......$cJ\.
-000070e0: 6ad0 795a 69ee 3efd a0e3 2b7a 1211 1eb0  j.yZi.>...+z....
-000070f0: 4280 f5ac 61f2 f200 f0e9 3422 079e 082a  B...a.....4"...*
-00007100: 1723 5f73 c81a d5e7 368f 32f4 3ea2 183d  .#_s....6.2.>..=
-00007110: 08e6 d565 8ff0 4251 54b2 2dd9 6424 58cf  ...e..BQT.-.d$X.
-00007120: b8cb 7c24 7e88 ee49 f608 01f5 b108 25f0  ..|$~..I......%.
-00007130: bd30 fe84 719e 813b e8b3 de3d 8e12 bf43  .0..q..;...=...C
-00007140: 945d c5e0 1e32 0bde 7dae 826f b014 110e  .]...2..}..o....
-00007150: ec65 602c 1698 f896 ef63 cfd2 5ddb 30ad  .e`,.....c..].0.
-00007160: 2030 b169 ce83 818c ccd5 161d 3688 e1dd   0.i........6...
-00007170: 6d14 4d52 c1a7 cd8f 93e8 fe4a 6292 219e  m.MR.......Jb.!.
-00007180: 60b7 e19e 47fe 78ed bf7d 0407 fb1b a2bb  `...G.x..}......
-00007190: 4de2 0fe5 60ae ee77 2823 fe3f 42b6 fb3b  M...`..w(#.?B..;
-000071a0: 8502 3058 5135 dd1d b84c 181d a5d4 78a6  ..0XQ5...L....x.
-000071b0: 2c5c 4ffc ddf1 4cf1 5de1 8fdc 3dc5 67da  ,\O...L.]...=.g.
-000071c0: 70fb e144 a248 5c4a cec3 724c 21d0 bb24  p..D.H\J..rL!..$
-000071d0: dbdf 41be cd23 c8c7 5f73 1485 908b fd3a  ..A..#.._s.....:
-000071e0: 4dfe 4e39 d5df d709 f872 e9eb 6701 8d41  M.N9.....r..g..A
-000071f0: 0a01 6bc8 d49a e261 293a 8c83 2445 6cc7  ..k....a):..$El.
-00007200: 8b82 ad7d 4619 037f dc40 7392 2560 dad3  ...}F....@s.%`..
-00007210: 5970 70b9 3b29 e899 143b 84f9 79c1 4fe4  Ypp.;)...;..y.O.
-00007220: df13 190f adc2 d827 87f5 cc81 5a1a 4611  .......'....Z.F.
-00007230: f222 a8e8 5529 f643 9a46 e859 b660 2759  ."..U).C.F.Y.`'Y
-00007240: ec42 df27 d0f4 5564 2174 7859 8ca2 0b74  .B.'..Ud!txY...t
-00007250: d055 f99f e2e8 b9a0 ac5c 192a 4f44 9a65  .U.......\.*OD.e
-00007260: 2123 14ba 11cc 7385 e221 0a12 82cb ac7e  !#....s..!.....~
-00007270: 4818 9169 5a06 518b ac1b 673c 2cdb d5a4  H..iZ.Q...g<,...
-00007280: 799d 4e1a afb4 e28e d34a 8fcd 08cd f468  y.N......J.....h
-00007290: ff3c da39 52a3 2a0d 19bc 091b e138 4779  .<.9R.*......8Gy
-000072a0: 8d50 d351 fa3f 5655 032a 71ad aef9 5175  .P.Q.?VU.*q...Qu
-000072b0: 3174 48e2 645f 4602 9f84 da31 34e8 8c92  1tH.d_F....14...
-000072c0: cb3b de40 f763 effd 1eba a62d 7ae0 750b  .;.@.c.....-z.u.
-000072d0: ad5a a1fd 9685 d078 3144 159f 2821 7f2e  .Z.....x1D..(!..
-000072e0: 969d 7915 a101 8a68 a33d 7f0f a5e0 9745  ..y....h.=.....E
-000072f0: d182 a8bc 0751 7913 a2f2 2e44 6db6 21ff  .....Qy....Dm.!.
-00007300: 167c 4ac9 3e42 6509 1b89 82d2 9473 b2bd  .|J.>Be......s..
-00007310: 856e 3b84 a8ae eb41 238c 3d5d 45c4 7655  .n;....A#.=]E.vU
-00007320: 7f1e 58c4 b47d 3770 2cc9 8764 fb7b c238  ..X..}7p,..d.{.8
-00007330: 8dee 3a86 857d 535d 2c1d a206 c4d5 55fe  ..:..}S],.....U.
-00007340: 8dea f8cb b911 044e e015 3428 c6bb 24e3  .......N..4(..$.
-00007350: 2481 8716 56e0 992a 3689 0124 8ec1 5bed  $...V..*6..$..[.
-00007360: a58a 91e5 2d5d c372 b005 c50e 7403 9350  ....-].r....t..P
-00007370: 2b9d d1ef c9f3 5392 7116 420d 133a 58d1  +.....S.q.B..:X.
-00007380: 3da6 78b5 851b 741b 0738 f250 369e c6ec  =.x...t..8.P6...
-00007390: b5ec 09ae ed11 ce27 3cd9 b4d5 6e09 eabd  .......'<...n...
-000073a0: 14c5 6f0f 2c43 9811 5fd9 9203 137a 3a9d  ..o.,C.._....z:.
-000073b0: e74b fe2f 1199 a5b6 414b 1f48 fcc0 76ca  .K./....AK.H..v.
-000073c0: 238a 7228 02f3 c5a2 91ff 1b45 a26e acae  #.r(.......E.n..
-000073d0: a809 bdfe b4d6 d662 5cce 3bc2 6944 c63b  .......b\.;.iD.;
-000073e0: 427d a556 85fd 449f 7075 e1ec 76e0 b58e  B}.V..D.pu..v...
-000073f0: 006c 1953 17fa 8c46 a8a8 4ffc dfd4 9054  .l.S...F..O....T
-00007400: e2a0 6e7c d004 adfc bf1b ff5f efc6 db33  ..n|......._...3
-00007410: 771d 34e6 e5a0 0152 d12a 2862 6857 606a  w.4....R.*(bhW`j
-00007420: 5736 4994 ef65 c1ee 054d 1452 98e5 7e31  W6I..e...M.R..~1
-00007430: 6cdd d603 ecab 73db 41aa 45a0 647a 4bc3  l.....s.A.E.dzK.
-00007440: 531d 2f98 07b6 6f99 b6b5 90a5 ba9d d3bb  S./...o.........
-00007450: 82d2 5df2 24da 8bf5 ac04 0dee 0086 14d5  ..].$...........
-00007460: e089 7823 21aa 23a8 4df1 159f c360 b6af  ..x#!.#.M....`..
-00007470: 009c 037c e2c8 72a3 fd17 bdc4 6697 0084  ...|..r.....f...
-00007480: f321 49be e469 0d54 9e45 917e e2c5 63a6  .!I..i.T.E.~..c.
-00007490: f099 51ce 1105 75b3 0ae7 b197 e430 18f1  ..Q...u......0..
-000074a0: 76a0 094b 7453 5a23 8976 4778 a891 52e4  v..KtSZ#.vGx..R.
-000074b0: aa18 f5af 3664 d6ef d7f1 3e7e 513b 907d  ....6d....>~Q;.}
-000074c0: d981 3600 bbc1 b01b fa89 02e0 f191 3a7e  ..6...........:~
-000074d0: 8cff 897c 7a95 0139 fa22 8c38 d070 fcf9  ...|z..9.".8.p..
-000074e0: f730 b477 6dd2 e89e 6abb 4d06 19ef ea91  .0.wm...j.M.....
-000074f0: b774 1201 7ec3 001a 3f5c c28a 38d8 ba9e  .t..~...?\..8...
-00007500: dd62 0cde 035d 6ad3 cb84 f483 fca9 6ff1  .b...]j.......o.
-00007510: 8221 1f89 87c9 7405 aaf4 47f8 718d a7d5  .!....t...G.q...
-00007520: 9e3c 0090 e064 5144 c4d0 9253 eece a567  .<...dQD...S...g
-00007530: 9ff5 eae6 697f eafe 7444 63d1 c18d f800  ....i...tDc.....
-00007540: 0368 5800 781e 6254 ac3e 6057 f305 e6ba  .hX.x.bT.>`W....
-00007550: defa 2823 6a73 1d73 a1f7 40e5 5aa8 0515  ..(#js.s..@.Z...
-00007560: e671 032c f4a2 047f a950 c4bf 8085 0a64  .q.,.....P.....d
-00007570: ae07 cb4d 9772 d292 0706 cf42 4d27 3742  ...M.r.....BM'7B
-00007580: 6a18 5306 0323 8499 3cc2 afc1 c434 cf22  j.S..#..<....4."
-00007590: a149 1f6b 8596 a866 dc18 5afd 2ca0 5e0d  .I.k...f..Z.,.^.
-000075a0: 28b3 4920 7ea9 9e4c 001a bc00 5296 6558  (.I ~..L....R.eX
-000075b0: 4b3c ff32 1879 4636 09a8 7e48 b080 daab  K<.2.yF6..~H....
-000075c0: 53fd dc8b 42d8 cf66 44dc a980 5d35 b835  S...B..fD...]5.5
-000075d0: d5be c20d 0114 3535 ddd2 f4b9 e6e3 1b48  ......55.......H
-000075e0: 49f5 42a4 bf18 2ad4 7aec c22f 71bc 505e  I.B...*.z../q.P^
-000075f0: 5b86 3694 c7af d15c a1c8 dabe d9fe dcf9  [.6....\........
-00007600: a1c2 461b 75ab d84f f51f 2e2b c8a9 3d92  ..F.u..O...+..=.
-00007610: 8f57 18d2 074b b233 05c9 38b1 47f2 6190  .W...K.3..8.G.a.
-00007620: 065f 911c fa6d 460b 1038 be89 82e3 4340  ._...mF..8....C@
-00007630: 5d19 87e8 474a 20ab 546b 73dc ee72 5ac7  ]...GJ .Tks..rZ.
-00007640: 179d 52ab 0856 691a d0bf 2e96 b40d 53d8  ..R..Vi.......S.
-00007650: 9213 de5c 4007 046d c649 15ac 58c8 a2ee  ...\@..m.I..X...
-00007660: dea6 0d86 4824 4c20 d412 016a c156 db5f  ....H$L ...j.V._
-00007670: ffc3 f2e8 cc01 34f7 fe45 3007 2b5a 5ddc  ......4..E0.+Z].
-00007680: 30f5 faf5 2b00 e318 48fd 7e91 98d1 79b0  0...+...H.~...y.
-00007690: a7af dc93 d68e 50fc 9043 069f 220b 043f  ......P..C.."..?
-000076a0: 7948 b2e7 b3b4 0364 9137 2b5e 6e78 1966  yH.....d.7+^nx.f
-000076b0: 1979 0c79 673f 925b 159d 719c 3091 daca  .y.yg?.[..q.0...
-000076c0: 6fca b54b f9a5 72e2 9fed 2ea4 1249 5260  o..K..r......IR`
-000076d0: 0712 7215 5185 ed08 bce7 b1f7 48a6 2481  ..r.Q.......H.$.
-000076e0: 42d1 237c 9764 4a29 24bd 51b6 f004 4ad3  B.#|.dJ)$.Q...J.
-000076f0: 8813 f081 0498 00f2 9426 309e c0ee 4481  .........&0...D.
-00007700: 92ab e429 bc9a 01dd 2270 ab8e 4001 04bc  ...)...."p..@...
-00007710: 4210 de55 cc6e befd e698 6812 feeb de42  B..U.n....h....B
-00007720: 7e8b 5ab7 bdbc e388 f87a 1ade c1e1 6bbc  ~.Z......z....k.
-00007730: 3757 5b5f 6098 65e6 da17 6c27 b9a3 9cee  7W[_`.e...l'....
-00007740: eec1 70f9 a4f8 18b4 6595 a547 bac5 552f  ..p.....e..G..U/
-00007750: af9c 5fb8 5d82 6b06 b44c 2fb9 b82c 1a97  .._.].k..L/..,..
-00007760: 41ef b414 ba69 17d3 cfb0 1387 702c 7eeb  A....i......p,~.
-00007770: 4d78 abe6 b2fa 40ab a55a 0970 b7e6 a756  Mx....@..Z.p...V
-00007780: da15 c076 f97c e7e8 92ba 313a 4da5 9553  ...v.|....1:M..S
-00007790: d279 6af0 9fd6 3df8 e7fe a2fe 84ac 3209  .yj...=.......2.
-000077a0: 1e9d 1357 7c4f 0963 e2b9 ab9e 9811 b944  ...W|O.c.......D
-000077b0: 2389 dbf3 e070 f237 779b 5b4a 131c 42ca  #....p.7w.[J..B.
-000077c0: f3df 420b c19e 279b 1b78 151c 4ed7 d8c6  ..B...'..x..N...
-000077d0: 54ce d358 53ad 5d43 c0af 55bc 40a2 84d7  T..XS.]C..U.@...
-000077e0: 7560 6722 0fa8 de38 2bb4 5b3d 57b8 d239  u`g"...8+.[=W..9
-000077f0: bac1 24f7 cf94 91fd fb62 0ae0 470e 262d  ..$......b..G.&-
-00007800: 550a 45e1 14dd 2037 abef 213d a57b fbaa  U.E... 7..!=.{..
-00007810: 4cb7 0d7e 5a1d 5d36 3584 308e c311 dd4c  L..~Z.]65.0....L
-00007820: 94a5 abaa 816c da79 aaf6 bca9 a94a 6af6  .....l.y.....Jj.
-00007830: ba84 2579 940e f323 0948 c65f 60eb 54c5  ..%y...#.H._`.T.
-00007840: 21a9 afe0 e4f3 5751 9bdd ea18 5ad8 2e4f  !.....WQ....Z..O
-00007850: a605 ec79 322d efcd a7ca 0ccb b4df 3d59  ...y2-........=Y
-00007860: 1fb1 b49c 11c7 64dd 93a6 9ecc 8adb 7a3a  ......d.......z:
-00007870: 3118 7b3a 3158 7b3a 3198 7b3a 31d8 7b3c  1.{:1X{:1.{:1.{<
-00007880: b15c 9b4f 0d74 4e3d 1c39 be54 a326 340b  .\.O.tN=.9.T.&4.
-00007890: 9500 d7dc 4054 95f1 7126 ceee 02cf bda4  ....@T..q&......
-000078a0: f202 1d11 3f48 ca38 cdbe 355e 7e26 2a85  ....?H.8..5^~&*.
-000078b0: 9cd5 ae55 3bf6 ff13 bcfe 0d00 00ff ff03  ...U;...........
-000078c0: 0050 4b03 0414 0006 0008 0000 0021 0021  .PK..........!.!
-000078d0: 8e30 52bb 0100 007d 0400 0018 0028 0063  .0R....}.....(.c
-000078e0: 7573 746f 6d58 6d6c 2f69 7465 6d50 726f  ustomXml/itemPro
-000078f0: 7073 312e 786d 6c20 a224 0028 a020 0000  ps1.xml .$.(. ..
-00007900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007910: 0000 0000 0000 0000 0000 0000 0000 00b4  ................
-00007920: 94dd 6adc 3010 85ef 0b7d 07a3 7b59 f2bf  ..j.0....}..{Y..
-00007930: 36c4 1bca ae03 8106 4a9a 406e c7b2 bc2b  6.......J.@n...+
-00007940: 6a49 4692 bb2d a5ef 5ed9 4929 6936 6c4a  jIF..-..^.I)i6lJ
-00007950: db2b 7964 66ce ccd1 279d 5f7c 5143 f459  .+ydf...'._|QC.Y
-00007960: 5827 8dae 5112 5314 09cd 4d27 f5ae 4677  X'..Q.S...M'..Fw
-00007970: b797 98a1 c879 d01d 0c46 8b1a 6983 2ed6  .....y...F..i...
-00007980: 6fdf 9c77 eeac 030f ce1b 2bae bc50 51d8  o..w......+..PQ.
-00007990: 9061 bdda d6e8 1b2b d9b6 69d2 0c17 6c53  .a.....+..i...lS
-000079a0: e2fc b2d8 e215 cb18 ce92 324f 9a26 df34  ..........2O.&.4
-000079b0: 79fa 1d45 415a 8732 ae46 7bef c733 421c  y..EAZ.2.F{..3B.
-000079c0: df0b 052e 36a3 d0e1 676f ac02 1f42 bb23  ....6...go...B.#
-000079d0: a6ef 2517 5bc3 2725 b427 29a5 25e1 5390  ..%.[.'%.').%.S.
-000079e0: 57f7 6a40 ebb9 9f87 ec1b d1bb a7e1 dcda  W.j@............
-000079f0: 64e5 3315 25b9 35ce f43e e646 3d0a 3c14  d.3.%.5..>.F=.<.
-00007a00: 56c2 c33c 1de1 46fb 2077 fb75 1488 fcb3  V..<..F. w.u....
-00007a10: aaa3 0d03 5a2f 8523 b3d2 3bef ad6c 272f  ....Z/.#..;..l'/
-00007a20: dc29 8dc3 e110 1fb2 c58f 6040 42ee afdf  .)........`@B...
-00007a30: 7f5c 2cfb 2fcd bd58 b4ad 6809 659f 615a  .\,./..X..h.e.aZ
-00007a40: f52d cedb 70b2 aca0 0586 aa2a 4ace 9255  .-..p......*J..U
-00007a50: 9bc3 8bc9 3461 0974 4585 8b55 91e2 9c86  ....4a.tE..U....
-00007a60: 2fe8 a1c7 15cd a04b 69b6 02ce fe7e 9cee  /......Ki....~..
-00007a70: 1194 6bd0 b013 0b32 3e1c e249 877f 1278  ..k....2>..I...x
-00007a80: 940d a97b 3382 dfcf 9054 e403 58af 85dd  ...{3....T..X...
-00007a90: 0444 ac19 5e5d f908 db23 f04f a1cb 67ec  .D..^]...#.O..g.
-00007aa0: 5981 7fa1 72ca 9371 b2c3 4246 c789 1896  Y...r..q..BF....
-00007ab0: 911d 49e2 84fc 49a2 1756 b993 19c7 4d92  ..I...I..V....M.
-00007ac0: e1aa 580d 0331 6d37 6b92 dfae e41c 3f79  ..X..1m7k.....?y
-00007ad0: 32d6 3f00 0000 ffff 0300 504b 0304 1400  2.?.......PK....
-00007ae0: 0600 0800 0000 2100 bd84 6223 9000 0000  ......!...b#....
-00007af0: db00 0000 1300 2800 6375 7374 6f6d 586d  ......(.customXm
-00007b00: 6c2f 6974 656d 322e 786d 6c20 a224 0028  l/item2.xml .$.(
-00007b10: a020 0000 0000 0000 0000 0000 0000 0000  . ..............
-00007b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007b30: 0000 006c 8e3b 0ec2 3010 05af 82d2 932d  ...l.;..0......-
-00007b40: e8d0 e234 810a 51e5 02c6 388a a5ac d7f2  ...4..Q...8.....
-00007b50: 2e1f df1e 0741 8194 7a9e 661e 7624 bc75  .....A..z.f.v$.u
-00007b60: 1cd5 471d 4af2 9dc1 1367 1a3c a5d9 aa97  ..G.J....g.<....
-00007b70: cd8b e628 8766 524d 7b00 7193 272b 2d05  ...(.fRM{.q.'+-.
-00007b80: 9759 78d4 d631 814c 36fb c421 2a3c 76f0  .Yx..1.L6..!*<v.
-00007b90: b569 b5c1 585d d218 ec83 545f 313d bb3b  .i..X]....T_1=.;
-00007ba0: d5d4 395c b3cd 6549 21fc 201e 6f41 d727  ..9\..eI!. .oA.'
-00007bb0: 1f82 17ff 5cc7 0b40 f83b 6ede 0000 00ff  ....\..@.;n.....
-00007bc0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00007bd0: 0087 aef1 14f2 0000 004f 0100 0018 0028  .........O.....(
-00007be0: 0063 7573 746f 6d58 6d6c 2f69 7465 6d50  .customXml/itemP
-00007bf0: 726f 7073 322e 786d 6c20 a224 0028 a020  rops2.xml .$.(. 
-00007c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007c20: 0064 904f 6b84 3010 c5ef 857e 0799 bbc6  .d.Ok.0....~....
-00007c30: 7f54 5dd4 45d6 2dec b5b4 d06b 8893 3560  .T].E.-....k..5`
-00007c40: 3292 c4a5 a5f4 bb37 d2d3 b6a7 e1cd 63de  2......7......c.
-00007c50: ef31 edf1 432f d10d ad53 643a c892 1422  .1..C/...Sd:..."
-00007c60: 3482 2665 ae1d bcbd 3ec7 3544 ce73 33f1  4.&e....>.5D.s3.
-00007c70: 850c 7660 088e fde3 433b b9c3 c43d 779e  ..v`....C;...=w.
-00007c80: 2c5e 3cea 282c 5498 97b1 83af b129 ca73  ,^<.(,T......).s
-00007c90: 5e34 f190 8f79 5c36 7519 0fcd 298f ab73  ^4...y\6u...)..s
-00007ca0: 3d9c 8aac aac6 acfa 8628 a04d 8871 1dcc  =........(.M.q..
-00007cb0: deaf 07c6 9c98 5173 97d0 8a26 9892 ace6  ......Qs...&....
-00007cc0: 3e48 7b65 24a5 1238 92d8 341a cff2 347d  >H{e$..8..4...4}
-00007cd0: 6262 0b78 fdae 17e8 f73e bfd7 2f28 ddbd  bb.x.....>../(..
-00007ce0: dcab 6d56 fda3 6825 2c39 923e 11a4 999b  ..mV..h%,9.>....
-00007cf0: b9c5 9554 08bf 154c 90f1 81e3 3f57 647b  ...T...L....?Wd{
-00007d00: 0d07 ac6f d91f c8ae ef9e d0ff 0000 00ff  ...o............
-00007d10: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00007d20: 0090 64ba 9b53 0100 0065 0200 0011 0008  ..d..S...e......
-00007d30: 0164 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
-00007d40: 6d6c 20a2 0401 28a0 0001 0000 0000 0000  ml ...(.........
-00007d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000065a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000065b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000065c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000065d0: 0000 0000 0000 0000 0000 0000 0000 0084  ................
+000065e0: cfc1 8a02 310c 06e0 bbe0 3b94 dc9d ce78  ....1.....;....x
+000065f0: 1091 e978 5916 bc89 b8e0 b574 3233 c569  ...xY......t23.i
+00006600: 539a 28fa f616 4f2b 2cec 3109 f9fe a4dd  S.(...O+,.1.....
+00006610: 3fc2 acee 98d9 5334 d054 3528 8c8e 7a1f  ?.....S4.T5(..z.
+00006620: 4703 3fe7 efd5 1614 8b8d bd9d 29a2 8127  G.?.........)..'
+00006630: 32ec bbe5 a23d e16c a52c f1e4 13ab a244  2....=.l.,.....D
+00006640: 3630 89a4 9dd6 ec26 0c96 2b4a 18cb 64a0  60.....&..+J..d.
+00006650: 1cac 9432 8f3a 5977 b523 ea75 5d6f 74fe  ...2.:Yw.#.u]ot.
+00006660: 6d40 f761 aa43 6f20 1ffa 06d4 f999 4af2  m@.a.Co ......J.
+00006670: ff36 0d83 77f8 45ee 1630 ca1f 11da dd58  .6..w.E..0.....X
+00006680: 285c c27c cc94 b8c8 368f 2806 bc60 78b7  (\.|....6.(..`x.
+00006690: 9aaa dc0b ba6b f5c7 7fdd 0b00 00ff ff03  .....k..........
+000066a0: 0050 4b03 0414 0006 0008 0000 0021 0075  .PK..........!.u
+000066b0: 84b7 f963 0100 007c 0400 0027 0000 0078  ...c...|...'...x
+000066c0: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
+000066d0: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
+000066e0: 7332 2e62 696e ec53 cd4a c340 10fe b611  s2.bin.S.J.@....
+000066f0: 512f 7af4 50a4 788a 8742 4d53 5b8f 6993  Q/z.P.x..BMS[.i.
+00006700: 4a24 c996 6cea 3dd2 8506 4212 d214 fcc1  J$..l.=...B.....
+00006710: 9b0f d237 f145 7c02 0fbe 82ce 5685 0a22  ...7.E|.....V.."
+00006720: 14bd 08ce b2fb 4dbe 99f9 76b3 cb38 1841  ......M...v..8.A
+00006730: 8023 c029 6cf4 d1a1 d946 033a 3cc2 0e8d  .#.)l....F.:<...
+00006740: 06c5 254a 24b4 ce70 84cf c636 b4cd 472c  ..%J$..p...6..G,
+00006750: 34ed 0135 0686 a79d 7c6b 42b8 8b29 ab11  4..5....|kB..)..
+00006760: 4e99 46ab 47b5 150d a5f3 7363 ef12 0a6b  N.F.G.....sc...k
+00006770: 3415 be90 9db9 c25c 55b7 dd60 7c08 9ddd  4......\U..`|...
+00006780: 6b75 2c9e a707 dfed bcbd 1254 7a1f 7bfc  ku,........Tz.{.
+00006790: c271 ff25 fec8 0dac f3e6 3a25 0b3f 3a57  .q.%......:%.?:W
+000067a0: bfb6 877d 768b 215a d43b 0e06 3060 5137  ...}v.!Z.;..0`Q7
+000067b0: 3589 31e8 db20 cf44 173d eaaf 26f1 5dca  5.1.. .D.=..&.].
+000067c0: 50d1 e325 6750 97a9 9c1e 55b7 89ef e08e  P..%gP....U.....
+000067d0: 14dd ac98 57fd 24c3 9087 bee0 e370 e020  ....W.$......p. 
+000067e0: 7484 ed79 1867 4929 67ca e365 22b3 2aae  t..y.gI)g..e".*.
+000067f0: 923c c388 8751 68b9 1142 39cb d3f9 92e3  .<...Qh..B9.....
+00006800: 8582 f649 0ba3 b890 a548 6e24 2c13 833c  ...I.....Hn$,..<
+00006810: cd4b 3f9f c837 cf30 2f8b 42b9 695c 49f0  .K?..7.0/.B.i\I.
+00006820: 00be 9c24 7174 5d48 88c8 0a6c 2bb4 61cf  ...$qt]H...l+.a.
+00006830: 8b54 5e21 e081 b3ee 53d6 a9e0 c2b4 fdaf  .T^!....S.......
+00006840: eef6 1500 00ff ff03 0050 4b03 0414 0006  .........PK.....
+00006850: 0008 0000 0021 0075 84b7 f963 0100 007c  .....!.u...c...|
+00006860: 0400 0027 0000 0078 6c2f 7072 696e 7465  ...'...xl/printe
+00006870: 7253 6574 7469 6e67 732f 7072 696e 7465  rSettings/printe
+00006880: 7253 6574 7469 6e67 7333 2e62 696e ec53  rSettings3.bin.S
+00006890: cd4a c340 10fe b611 512f 7af4 50a4 788a  .J.@....Q/z.P.x.
+000068a0: 8742 4d53 5b8f 6993 4a24 c996 6cea 3dd2  .BMS[.i.J$..l.=.
+000068b0: 8506 4212 d214 fcc1 9b0f d237 f145 7c02  ..B........7.E|.
+000068c0: 0fbe 82ce 5685 0a22 14bd 08ce b2fb 4dbe  ....V.."......M.
+000068d0: 99f9 76b3 cb38 1841 8023 c029 6cf4 d1a1  ..v..8.A.#.)l...
+000068e0: d946 033a 3cc2 0e8d 06c5 254a 24b4 ce70  .F.:<.....%J$..p
+000068f0: 84cf c636 b4cd 472c 34ed 0135 0686 a79d  ...6..G,4..5....
+00006900: 7c6b 42b8 8b29 ab11 4e99 46ab 47b5 150d  |kB..)..N.F.G...
+00006910: a5f3 7363 ef12 0a6b 3415 be90 9db9 c25c  ..sc...k4......\
+00006920: 55b7 dd60 7c08 9ddd 6b75 2c9e a707 dfed  U..`|...ku,.....
+00006930: bcbd 1254 7a1f 7bfc c271 ff25 fec8 0dac  ...Tz.{..q.%....
+00006940: f3e6 3a25 0b3f 3a57 bfb6 877d 768b 215a  ..:%.?:W...}v.!Z
+00006950: d43b 0e06 3060 5137 3589 31e8 db20 cf44  .;..0`Q75.1.. .D
+00006960: 173d eaaf 26f1 5dca 50d1 e325 6750 97a9  .=..&.].P..%gP..
+00006970: 9c1e 55b7 89ef e08e 14dd ac98 57fd 24c3  ..U.........W.$.
+00006980: 9087 bee0 e370 e020 7484 ed79 1867 4929  .....p. t..y.gI)
+00006990: 67ca e365 22b3 2aae 923c c388 8751 68b9  g..e".*..<...Qh.
+000069a0: 1142 39cb d3f9 92e3 8582 f649 0ba3 b890  .B9........I....
+000069b0: a548 6e24 2c13 833c cd4b 3f9f c837 cf30  .Hn$,..<.K?..7.0
+000069c0: 2f8b 42b9 695c 49f0 00be 9c24 7174 5d48  /.B.i\I....$qt]H
+000069d0: 88c8 0a6c 2bb4 61cf 8b54 5e21 e081 b3ee  ...l+.a..T^!....
+000069e0: 53d6 a9e0 c2b4 fdaf eef6 1500 00ff ff03  S...............
+000069f0: 0050 4b03 0414 0006 0008 0000 0021 0075  .PK..........!.u
+00006a00: 84b7 f963 0100 007c 0400 0027 0000 0078  ...c...|...'...x
+00006a10: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
+00006a20: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
+00006a30: 7336 2e62 696e ec53 cd4a c340 10fe b611  s6.bin.S.J.@....
+00006a40: 512f 7af4 50a4 788a 8742 4d53 5b8f 6993  Q/z.P.x..BMS[.i.
+00006a50: 4a24 c996 6cea 3dd2 8506 4212 d214 fcc1  J$..l.=...B.....
+00006a60: 9b0f d237 f145 7c02 0fbe 82ce 5685 0a22  ...7.E|.....V.."
+00006a70: 14bd 08ce b2fb 4dbe 99f9 76b3 cb38 1841  ......M...v..8.A
+00006a80: 8023 c029 6cf4 d1a1 d946 033a 3cc2 0e8d  .#.)l....F.:<...
+00006a90: 06c5 254a 24b4 ce70 84cf c636 b4cd 472c  ..%J$..p...6..G,
+00006aa0: 34ed 0135 0686 a79d 7c6b 42b8 8b29 ab11  4..5....|kB..)..
+00006ab0: 4e99 46ab 47b5 150d a5f3 7363 ef12 0a6b  N.F.G.....sc...k
+00006ac0: 3415 be90 9db9 c25c 55b7 dd60 7c08 9ddd  4......\U..`|...
+00006ad0: 6b75 2c9e a707 dfed bcbd 1254 7a1f 7bfc  ku,........Tz.{.
+00006ae0: c271 ff25 fec8 0dac f3e6 3a25 0b3f 3a57  .q.%......:%.?:W
+00006af0: bfb6 877d 768b 215a d43b 0e06 3060 5137  ...}v.!Z.;..0`Q7
+00006b00: 3589 31e8 db20 cf44 173d eaaf 26f1 5dca  5.1.. .D.=..&.].
+00006b10: 50d1 e325 6750 97a9 9c1e 55b7 89ef e08e  P..%gP....U.....
+00006b20: 14dd ac98 57fd 24c3 9087 bee0 e370 e020  ....W.$......p. 
+00006b30: 7484 ed79 1867 4929 67ca e365 22b3 2aae  t..y.gI)g..e".*.
+00006b40: 923c c388 8751 68b9 1142 39cb d3f9 92e3  .<...Qh..B9.....
+00006b50: 8582 f649 0ba3 b890 a548 6e24 2c13 833c  ...I.....Hn$,..<
+00006b60: cd4b 3f9f c837 cf30 2f8b 42b9 695c 49f0  .K?..7.0/.B.i\I.
+00006b70: 00be 9c24 7174 5d48 88c8 0a6c 2bb4 61cf  ...$qt]H...l+.a.
+00006b80: 8b54 5e21 e081 b3ee 53d6 a9e0 c2b4 fdaf  .T^!....S.......
+00006b90: eef6 1500 00ff ff03 0050 4b03 0414 0006  .........PK.....
+00006ba0: 0008 0000 0021 0075 84b7 f963 0100 007c  .....!.u...c...|
+00006bb0: 0400 0027 0000 0078 6c2f 7072 696e 7465  ...'...xl/printe
+00006bc0: 7253 6574 7469 6e67 732f 7072 696e 7465  rSettings/printe
+00006bd0: 7253 6574 7469 6e67 7337 2e62 696e ec53  rSettings7.bin.S
+00006be0: cd4a c340 10fe b611 512f 7af4 50a4 788a  .J.@....Q/z.P.x.
+00006bf0: 8742 4d53 5b8f 6993 4a24 c996 6cea 3dd2  .BMS[.i.J$..l.=.
+00006c00: 8506 4212 d214 fcc1 9b0f d237 f145 7c02  ..B........7.E|.
+00006c10: 0fbe 82ce 5685 0a22 14bd 08ce b2fb 4dbe  ....V.."......M.
+00006c20: 99f9 76b3 cb38 1841 8023 c029 6cf4 d1a1  ..v..8.A.#.)l...
+00006c30: d946 033a 3cc2 0e8d 06c5 254a 24b4 ce70  .F.:<.....%J$..p
+00006c40: 84cf c636 b4cd 472c 34ed 0135 0686 a79d  ...6..G,4..5....
+00006c50: 7c6b 42b8 8b29 ab11 4e99 46ab 47b5 150d  |kB..)..N.F.G...
+00006c60: a5f3 7363 ef12 0a6b 3415 be90 9db9 c25c  ..sc...k4......\
+00006c70: 55b7 dd60 7c08 9ddd 6b75 2c9e a707 dfed  U..`|...ku,.....
+00006c80: bcbd 1254 7a1f 7bfc c271 ff25 fec8 0dac  ...Tz.{..q.%....
+00006c90: f3e6 3a25 0b3f 3a57 bfb6 877d 768b 215a  ..:%.?:W...}v.!Z
+00006ca0: d43b 0e06 3060 5137 3589 31e8 db20 cf44  .;..0`Q75.1.. .D
+00006cb0: 173d eaaf 26f1 5dca 50d1 e325 6750 97a9  .=..&.].P..%gP..
+00006cc0: 9c1e 55b7 89ef e08e 14dd ac98 57fd 24c3  ..U.........W.$.
+00006cd0: 9087 bee0 e370 e020 7484 ed79 1867 4929  .....p. t..y.gI)
+00006ce0: 67ca e365 22b3 2aae 923c c388 8751 68b9  g..e".*..<...Qh.
+00006cf0: 1142 39cb d3f9 92e3 8582 f649 0ba3 b890  .B9........I....
+00006d00: a548 6e24 2c13 833c cd4b 3f9f c837 cf30  .Hn$,..<.K?..7.0
+00006d10: 2f8b 42b9 695c 49f0 00be 9c24 7174 5d48  /.B.i\I....$qt]H
+00006d20: 88c8 0a6c 2bb4 61cf 8b54 5e21 e081 b3ee  ...l+.a..T^!....
+00006d30: 53d6 a9e0 c2b4 fdaf eef6 1500 00ff ff03  S...............
+00006d40: 0050 4b03 0414 0006 0008 0000 0021 0075  .PK..........!.u
+00006d50: 84b7 f963 0100 007c 0400 0027 0000 0078  ...c...|...'...x
+00006d60: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
+00006d70: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
+00006d80: 7338 2e62 696e ec53 cd4a c340 10fe b611  s8.bin.S.J.@....
+00006d90: 512f 7af4 50a4 788a 8742 4d53 5b8f 6993  Q/z.P.x..BMS[.i.
+00006da0: 4a24 c996 6cea 3dd2 8506 4212 d214 fcc1  J$..l.=...B.....
+00006db0: 9b0f d237 f145 7c02 0fbe 82ce 5685 0a22  ...7.E|.....V.."
+00006dc0: 14bd 08ce b2fb 4dbe 99f9 76b3 cb38 1841  ......M...v..8.A
+00006dd0: 8023 c029 6cf4 d1a1 d946 033a 3cc2 0e8d  .#.)l....F.:<...
+00006de0: 06c5 254a 24b4 ce70 84cf c636 b4cd 472c  ..%J$..p...6..G,
+00006df0: 34ed 0135 0686 a79d 7c6b 42b8 8b29 ab11  4..5....|kB..)..
+00006e00: 4e99 46ab 47b5 150d a5f3 7363 ef12 0a6b  N.F.G.....sc...k
+00006e10: 3415 be90 9db9 c25c 55b7 dd60 7c08 9ddd  4......\U..`|...
+00006e20: 6b75 2c9e a707 dfed bcbd 1254 7a1f 7bfc  ku,........Tz.{.
+00006e30: c271 ff25 fec8 0dac f3e6 3a25 0b3f 3a57  .q.%......:%.?:W
+00006e40: bfb6 877d 768b 215a d43b 0e06 3060 5137  ...}v.!Z.;..0`Q7
+00006e50: 3589 31e8 db20 cf44 173d eaaf 26f1 5dca  5.1.. .D.=..&.].
+00006e60: 50d1 e325 6750 97a9 9c1e 55b7 89ef e08e  P..%gP....U.....
+00006e70: 14dd ac98 57fd 24c3 9087 bee0 e370 e020  ....W.$......p. 
+00006e80: 7484 ed79 1867 4929 67ca e365 22b3 2aae  t..y.gI)g..e".*.
+00006e90: 923c c388 8751 68b9 1142 39cb d3f9 92e3  .<...Qh..B9.....
+00006ea0: 8582 f649 0ba3 b890 a548 6e24 2c13 833c  ...I.....Hn$,..<
+00006eb0: cd4b 3f9f c837 cf30 2f8b 42b9 695c 49f0  .K?..7.0/.B.i\I.
+00006ec0: 00be 9c24 7174 5d48 88c8 0a6c 2bb4 61cf  ...$qt]H...l+.a.
+00006ed0: 8b54 5e21 e081 b3ee 53d6 a9e0 c2b4 fdaf  .T^!....S.......
+00006ee0: eef6 1500 00ff ff03 0050 4b03 0414 0006  .........PK.....
+00006ef0: 0008 0000 0021 00bd 8462 2390 0000 00db  .....!...b#.....
+00006f00: 0000 0013 0028 0063 7573 746f 6d58 6d6c  .....(.customXml
+00006f10: 2f69 7465 6d31 2e78 6d6c 20a2 2400 28a0  /item1.xml .$.(.
+00006f20: 2000 0000 0000 0000 0000 0000 0000 0000   ...............
+00006f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006f40: 0000 6c8e 3b0e c230 1005 af82 d293 2de8  ..l.;..0......-.
+00006f50: d0e2 3481 0a51 e502 c638 8aa5 acd7 f22e  ..4..Q...8......
+00006f60: 1fdf 1e07 4181 947a 9e66 1e76 24bc 751c  ....A..z.f.v$.u.
+00006f70: d547 1d4a f29d c113 671a 3ca5 d9aa 97cd  .G.J....g.<.....
+00006f80: 8be6 2887 6652 4d7b 0071 9327 2b2d 0597  ..(.fRM{.q.'+-..
+00006f90: 5978 d4d6 3181 4c36 fbc4 212a 3c76 f0b5  Yx..1.L6..!*<v..
+00006fa0: 69b5 c158 5dd2 18ec 8354 5f31 3dbb 3bd5  i..X]....T_1=.;.
+00006fb0: d439 5cb3 cd65 4921 fc20 1e6f 41d7 271f  .9\..eI!. .oA.'.
+00006fc0: 8217 ff5c c70b 40f8 3b6e de00 0000 ffff  ...\..@.;n......
+00006fd0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00006fe0: 87ae f114 f200 0000 4f01 0000 1800 2800  ........O.....(.
+00006ff0: 6375 7374 6f6d 586d 6c2f 6974 656d 5072  customXml/itemPr
+00007000: 6f70 7331 2e78 6d6c 20a2 2400 28a0 2000  ops1.xml .$.(. .
+00007010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007030: 6490 4f6b 8430 10c5 ef85 7e07 99bb c67f  d.Ok.0....~.....
+00007040: 545d d445 d62d ecb5 b4d0 6b88 9335 6032  T].E.-....k..5`2
+00007050: 92c4 a5a5 f4bb 37d2 d3b6 a7e1 cd63 deef  ......7......c..
+00007060: 31ed f143 2fd1 0dad 5364 3ac8 9214 2234  1..C/...Sd:..."4
+00007070: 8226 65ae 1dbc bd3e c735 44ce 7333 f185  .&e....>.5D.s3..
+00007080: 0c76 6008 8efd e343 3bb9 c3c4 3d77 9e2c  .v`....C;...=w.,
+00007090: 5e3c ea28 2c54 9897 b183 afb1 29ca 735e  ^<.(,T......).s^
+000070a0: 34f1 908f 795c 3675 190f cd29 8fab 733d  4...y\6u...)..s=
+000070b0: 9c8a acaa c6ac fa86 28a0 4d88 711d ccde  ........(.M.q...
+000070c0: af07 c69c 9851 7397 d08a 2698 92ac e63e  .....Qs...&....>
+000070d0: 487b 6524 a512 3892 d834 1acf f234 7d62  H{e$..8..4...4}b
+000070e0: 620b 78fd ae17 e8f7 3ebf d72f 28dd bddc  b.x.....>../(...
+000070f0: ab6d 56fd a368 252c 3992 3e11 a499 9bb9  .mV..h%,9.>.....
+00007100: c595 5408 bf15 4c90 f181 e33f 5764 7b0d  ..T...L....?Wd{.
+00007110: 07ac 6fd9 1fc8 aeef 9ed0 ff00 0000 ffff  ..o.............
+00007120: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00007130: 559f 35f5 d409 0000 8c30 0000 1300 2800  U.5......0....(.
+00007140: 6375 7374 6f6d 586d 6c2f 6974 656d 322e  customXml/item2.
+00007150: 786d 6c20 a224 0028 a020 0000 0000 0000  xml .$.(. ......
+00007160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007170: 0000 0000 0000 0000 0000 00ec 5bdd 929b  ............[...
+00007180: 4616 be4f 55de 81d2 5e33 8040 0254 9653  F..OU...^3.@.T.S
+00007190: 638d bdeb 8a1d bb32 daec dea5 9aa6 19b1  c......2........
+000071a0: 4680 e966 4653 a97d a47d 8abc 584e 77f3  F..fFS.}.}..XNw.
+000071b0: 8f7e 004d 36a9 ad4d 2e32 9238 a74f 9fff  .~.M6..M.2.8.O..
+000071c0: f31d f2ea bbc3 3e52 1e49 46c3 245e cf8c  ......>R.IF.$^..
+000071d0: 1b7d a690 1827 7e18 3fac 6739 0b54 67f6  .}...'~.?.g9.Tg.
+000071e0: ddeb 5798 ad70 1233 12b3 ed73 4aee f18e  ..W..p.3...sJ...
+000071f0: ec91 025f febc 9ecd 943d aafe db78 e807  ..._.....=...x..
+00007200: b427 ebd9 5d82 f33d 9025 e2b1 c6cf efef  .'..]..=.%......
+00007210: d633 fda0 1bf0 affe ce34 0dc3 7db3 9c6f  .3.......4..}..o
+00007220: 4c7b 6159 ae7b 676f de59 cead bbb9 7396  L{aY.{go.Y....s.
+00007230: ce62 d9a5 fda9 12d7 e8fe 7447 28ce c294  .b........tG(...
+00007240: 89db 6c32 8232 25ce c963 a2f8 a520 375d  ..l2.2%..c... 7]
+00007250: 927b 9ca4 20a9 f8ba 5004 17ce 70e6 fe7c  .{.. ...P...p..|
+00007260: ae9b ba67 064b d35d ce1d 8275 ec2c dc39  ...g.K.]...u.,.9
+00007270: b65c dd01 3d81 e662 bac2 6c3d db31 96ae  .\..=..b..l=.1..
+00007280: 348d 0abd d09b 7d88 b384 2601 bbc1 c95e  4.....}...&....^
+00007290: 4b82 20c4 449b ebfa 52db 1386 7cc4 90d6  K. .D...R...|...
+000072a0: d044 c968 8fa6 304a 3390 3e63 21a1 82f9  .D.h..0J3.>c!...
+000072b0: 2d63 59e8 e58c d0d9 eb6f bf79 75a0 fe4a  -cY......o.yu..J
+000072c0: 4aa5 3094 3d10 c6ad 4253 84e1 c2e3 85ae  J.0.=...BS......
+000072d0: cf12 caca 9204 eece b29c 888f 4148 229f  ............AH".
+000072e0: 0abb 9aae 6393 00e9 a66b 390b cf31 75dd  ....c....k9..1u.
+000072f0: f43d ecba f3b9 4d40 a733 25a6 73e9 3331  .=....M@.3%.s.31
+00007300: 35e5 1f52 9920 6f25 d8d3 d3d3 cd93 7993  5..R. o%......y.
+00007310: 640f 5c77 86f6 cf8f 1fa4 e395 0a3b d0e1  d.\w.........;..
+00007320: cfa6 d7de 57ca 0772 af67 9ead 2fd1 3230  ....W..r.g../.20
+00007330: 55dd 0e3c d5f2 4c47 7516 fa42 45b6 bd58  U..<..LGu..BE..X
+00007340: 62c7 703d 0b95 32c2 fdc0 cf0d c740 fec2  b.p=..2......@..
+00007350: 5617 ee62 ae5a 3afc 8502 14a8 b66e 221f  V..b.Z:......n".
+00007360: 5ccc 45d8 a9cc 15ee d324 634a 5c1b 6ad0  \.E......$cJ\.j.
+00007370: 795a 69ee 3efd a0e3 2b7a 1211 1eb0 4280  yZi.>...+z....B.
+00007380: f5ac 61f2 f200 f0e9 3422 079e 082a 1723  ..a.....4"...*.#
+00007390: 5f73 c81a d5e7 368f 32f4 3ea2 183d 08e6  _s....6.2.>..=..
+000073a0: d565 8ff0 4251 54b2 2dd9 6424 58cf b8cb  .e..BQT.-.d$X...
+000073b0: 7c24 7e88 ee49 f608 01f5 b108 25f0 bd30  |$~..I......%..0
+000073c0: fe84 719e 813b e8b3 de3d 8e12 bf43 945d  ..q..;...=...C.]
+000073d0: c5e0 1e32 0bde 7dae 826f b014 110e ec65  ...2..}..o.....e
+000073e0: 602c 1698 f896 ef63 cfd2 5ddb 30ad 2030  `,.....c..].0. 0
+000073f0: b169 ce83 818c ccd5 161d 3688 e1dd 6d14  .i........6...m.
+00007400: 4d52 c1a7 cd8f 93e8 fe4a 6292 219e 60b7  MR.......Jb.!.`.
+00007410: e19e 47fe 78ed bf7d 0407 fb1b a2bb 4de2  ..G.x..}......M.
+00007420: 0fe5 60ae ee77 2823 fe3f 42b6 fb3b 8502  ..`..w(#.?B..;..
+00007430: 3058 5135 dd1d b84c 181d a5d4 78a6 2c5c  0XQ5...L....x.,\
+00007440: 4ffc ddf1 4cf1 5de1 8fdc 3dc5 67da 70fb  O...L.]...=.g.p.
+00007450: e144 a248 5c4a cec3 724c 21d0 bb24 dbdf  .D.H\J..rL!..$..
+00007460: 41be cd23 c8c7 5f73 1485 908b fd3a 4dfe  A..#.._s.....:M.
+00007470: 4e39 d5df d709 f872 e9eb 6701 8d41 0a01  N9.....r..g..A..
+00007480: 6bc8 d49a e261 293a 8c83 2445 6cc7 8b82  k....a):..$El...
+00007490: ad7d 4619 037f dc40 7392 2560 dad3 5970  .}F....@s.%`..Yp
+000074a0: 70b9 3b29 e899 143b 84f9 79c1 4fe4 df13  p.;)...;..y.O...
+000074b0: 190f adc2 d827 87f5 cc81 5a1a 4611 f222  .....'....Z.F.."
+000074c0: a8e8 5529 f643 9a46 e859 b660 2759 ec42  ..U).C.F.Y.`'Y.B
+000074d0: df27 d0f4 5564 2174 7859 8ca2 0b74 d055  .'..Ud!txY...t.U
+000074e0: f99f e2e8 b9a0 ac5c 192a 4f44 9a65 2123  .......\.*OD.e!#
+000074f0: 14ba 11cc 7385 e221 0a12 82cb ac7e 4818  ....s..!.....~H.
+00007500: 9169 5a06 518b ac1b 673c 2cdb d5a4 799d  .iZ.Q...g<,...y.
+00007510: 4e1a afb4 e28e d34a 8fcd 08cd f468 ff3c  N......J.....h.<
+00007520: da39 52a3 2a0d 19bc 091b e138 4779 8d50  .9R.*......8Gy.P
+00007530: d351 fa3f 5655 032a 71ad aef9 5175 3174  .Q.?VU.*q...Qu1t
+00007540: 48e2 645f 4602 9f84 da31 34e8 8c92 cb3b  H.d_F....14....;
+00007550: de40 f763 effd 1eba a62d 7ae0 750b ad5a  .@.c.....-z.u..Z
+00007560: a1fd 9685 d078 3144 159f 2821 7f2e 969d  .....x1D..(!....
+00007570: 7915 a101 8a68 a33d 7f0f a5e0 9745 d182  y....h.=.....E..
+00007580: a8bc 0751 7913 a2f2 2e44 6db6 21ff 167c  ...Qy....Dm.!..|
+00007590: 4ac9 3e42 6509 1b89 82d2 9473 b2bd 856e  J.>Be......s...n
+000075a0: 3b84 a8ae eb41 238c 3d5d 45c4 7655 7f1e  ;....A#.=]E.vU..
+000075b0: 58c4 b47d 3770 2cc9 8764 fb7b c238 8dee  X..}7p,..d.{.8..
+000075c0: 3a86 857d 535d 2c1d a206 c4d5 55fe 8dea  :..}S],.....U...
+000075d0: f8cb b911 044e e015 3428 c6bb 24e3 2481  .....N..4(..$.$.
+000075e0: 8716 56e0 992a 3689 0124 8ec1 5bed a58a  ..V..*6..$..[...
+000075f0: 91e5 2d5d c372 b005 c50e 7403 9350 2b9d  ..-].r....t..P+.
+00007600: d1ef c9f3 5392 7116 420d 133a 58d1 3da6  ....S.q.B..:X.=.
+00007610: 78b5 851b 741b 0738 f250 369e c6ec b5ec  x...t..8.P6.....
+00007620: 09ae ed11 ce27 3cd9 b4d5 6e09 eabd 14c5  .....'<...n.....
+00007630: 6f0f 2c43 9811 5fd9 9203 137a 3a9d e74b  o.,C.._....z:..K
+00007640: fe2f 1199 a5b6 414b 1f48 fcc0 76ca 238a  ./....AK.H..v.#.
+00007650: 7228 02f3 c5a2 91ff 1b45 a26e acae a809  r(.......E.n....
+00007660: bdfe b4d6 d662 5cce 3bc2 6944 c63b 427d  .....b\.;.iD.;B}
+00007670: a556 85fd 449f 7075 e1ec 76e0 b58e 006c  .V..D.pu..v....l
+00007680: 1953 17fa 8c46 a8a8 4ffc dfd4 9054 e2a0  .S...F..O....T..
+00007690: 6e7c d004 adfc bf1b ff5f efc6 db33 771d  n|......._...3w.
+000076a0: 34e6 e5a0 0152 d12a 2862 6857 606a 5736  4....R.*(bhW`jW6
+000076b0: 4994 ef65 c1ee 054d 1452 98e5 7e31 6cdd  I..e...M.R..~1l.
+000076c0: d603 ecab 73db 41aa 45a0 647a 4bc3 531d  ....s.A.E.dzK.S.
+000076d0: 2f98 07b6 6f99 b6b5 90a5 ba9d d3bb 82d2  /...o...........
+000076e0: 5df2 24da 8bf5 ac04 0dee 0086 14d5 e089  ].$.............
+000076f0: 7823 21aa 23a8 4df1 159f c360 b6af 009c  x#!.#.M....`....
+00007700: 037c e2c8 72a3 fd17 bdc4 6697 0084 f321  .|..r.....f....!
+00007710: 49be e469 0d54 9e45 917e e2c5 63a6 f099  I..i.T.E.~..c...
+00007720: 51ce 1105 75b3 0ae7 b197 e430 18f1 76a0  Q...u......0..v.
+00007730: 094b 7453 5a23 8976 4778 a891 52e4 aa18  .KtSZ#.vGx..R...
+00007740: f5af 3664 d6ef d7f1 3e7e 513b 907d d981  ..6d....>~Q;.}..
+00007750: 3600 bbc1 b01b fa89 02e0 f191 3a7e 8cff  6...........:~..
+00007760: 897c 7a95 0139 fa22 8c38 d070 fcf9 f730  .|z..9.".8.p...0
+00007770: b477 6dd2 e89e 6abb 4d06 19ef ea91 b774  .wm...j.M......t
+00007780: 1201 7ec3 001a 3f5c c28a 38d8 ba9e dd62  ..~...?\..8....b
+00007790: 0cde 035d 6ad3 cb84 f483 fca9 6ff1 8221  ...]j.......o..!
+000077a0: 1f89 87c9 7405 aaf4 47f8 718d a7d5 9e3c  ....t...G.q....<
+000077b0: 0090 e064 5144 c4d0 9253 eece a567 9ff5  ...dQD...S...g..
+000077c0: eae6 697f eafe 7444 63d1 c18d f800 0368  ..i...tDc......h
+000077d0: 5800 781e 6254 ac3e 6057 f305 e6ba defa  X.x.bT.>`W......
+000077e0: 2823 6a73 1d73 a1f7 40e5 5aa8 0515 e671  (#js.s..@.Z....q
+000077f0: 032c f4a2 047f a950 c4bf 8085 0a64 ae07  .,.....P.....d..
+00007800: cb4d 9772 d292 0706 cf42 4d27 3742 6a18  .M.r.....BM'7Bj.
+00007810: 5306 0323 8499 3cc2 afc1 c434 cf22 a149  S..#..<....4.".I
+00007820: 1f6b 8596 a866 dc18 5afd 2ca0 5e0d 28b3  .k...f..Z.,.^.(.
+00007830: 4920 7ea9 9e4c 001a bc00 5296 6558 4b3c  I ~..L....R.eXK<
+00007840: ff32 1879 4636 09a8 7e48 b080 daab 53fd  .2.yF6..~H....S.
+00007850: dc8b 42d8 cf66 44dc a980 5d35 b835 d5be  ..B..fD...]5.5..
+00007860: c20d 0114 3535 ddd2 f4b9 e6e3 1b48 49f5  ....55.......HI.
+00007870: 42a4 bf18 2ad4 7aec c22f 71bc 505e 5b86  B...*.z../q.P^[.
+00007880: 3694 c7af d15c a1c8 dabe d9fe dcf9 a1c2  6....\..........
+00007890: 461b 75ab d84f f51f 2e2b c8a9 3d92 8f57  F.u..O...+..=..W
+000078a0: 18d2 074b b233 05c9 38b1 47f2 6190 065f  ...K.3..8.G.a.._
+000078b0: 911c fa6d 460b 1038 be89 82e3 4340 5d19  ...mF..8....C@].
+000078c0: 87e8 474a 20ab 546b 73dc ee72 5ac7 179d  ..GJ .Tks..rZ...
+000078d0: 52ab 0856 691a d0bf 2e96 b40d 53d8 9213  R..Vi.......S...
+000078e0: de5c 4007 046d c649 15ac 58c8 a2ee dea6  .\@..m.I..X.....
+000078f0: 0d86 4824 4c20 d412 016a c156 db5f ffc3  ..H$L ...j.V._..
+00007900: f2e8 cc01 34f7 fe45 3007 2b5a 5ddc 30f5  ....4..E0.+Z].0.
+00007910: faf5 2b00 e318 48fd 7e91 98d1 79b0 a7af  ..+...H.~...y...
+00007920: dc93 d68e 50fc 9043 069f 220b 043f 7948  ....P..C.."..?yH
+00007930: b2e7 b3b4 0364 9137 2b5e 6e78 1966 1979  .....d.7+^nx.f.y
+00007940: 0c79 673f 925b 159d 719c 3091 daca 6fca  .yg?.[..q.0...o.
+00007950: b54b f9a5 72e2 9fed 2ea4 1249 5260 0712  .K..r......IR`..
+00007960: 7215 5185 ed08 bce7 b1f7 48a6 2481 42d1  r.Q.......H.$.B.
+00007970: 237c 9764 4a29 24bd 51b6 f004 4ad3 8813  #|.dJ)$.Q...J...
+00007980: f081 0498 00f2 9426 309e c0ee 4481 92ab  .......&0...D...
+00007990: e429 bc9a 01dd 2270 ab8e 4001 04bc 4210  .)...."p..@...B.
+000079a0: de55 cc6e befd e698 6812 feeb de42 7e8b  .U.n....h....B~.
+000079b0: 5ab7 bdbc e388 f87a 1ade c1e1 6bbc 3757  Z......z....k.7W
+000079c0: 5b5f 6098 65e6 da17 6c27 b9a3 9cee eec1  [_`.e...l'......
+000079d0: 70f9 a4f8 18b4 6595 a547 bac5 552f af9c  p.....e..G..U/..
+000079e0: 5fb8 5d82 6b06 b44c 2fb9 b82c 1a97 41ef  _.].k..L/..,..A.
+000079f0: b414 ba69 17d3 cfb0 1387 702c 7eeb 4d78  ...i......p,~.Mx
+00007a00: abe6 b2fa 40ab a55a 0970 b7e6 a756 da15  ....@..Z.p...V..
+00007a10: c076 f97c e7e8 92ba 313a 4da5 9553 d279  .v.|....1:M..S.y
+00007a20: 6af0 9fd6 3df8 e7fe a2fe 84ac 3209 1e9d  j...=.......2...
+00007a30: 1357 7c4f 0963 e2b9 ab9e 9811 b944 2389  .W|O.c.......D#.
+00007a40: dbf3 e070 f237 779b 5b4a 131c 42ca f3df  ...p.7w.[J..B...
+00007a50: 420b c19e 279b 1b78 151c 4ed7 d8c6 54ce  B...'..x..N...T.
+00007a60: d358 53ad 5d43 c0af 55bc 40a2 84d7 7560  .XS.]C..U.@...u`
+00007a70: 6722 0fa8 de38 2bb4 5b3d 57b8 d239 bac1  g"...8+.[=W..9..
+00007a80: 24f7 cf94 91fd fb62 0ae0 470e 262d 550a  $......b..G.&-U.
+00007a90: 45e1 14dd 2037 abef 213d a57b fbaa 4cb7  E... 7..!=.{..L.
+00007aa0: 0d7e 5a1d 5d36 3584 308e c311 dd4c 94a5  .~Z.]65.0....L..
+00007ab0: abaa 816c da79 aaf6 bca9 a94a 6af6 ba84  ...l.y.....Jj...
+00007ac0: 2579 940e f323 0948 c65f 60eb 54c5 21a9  %y...#.H._`.T.!.
+00007ad0: afe0 e4f3 5751 9bdd ea18 5ad8 2e4f a605  ....WQ....Z..O..
+00007ae0: ec79 322d efcd a7ca 0ccb b4df 3d59 1fb1  .y2-........=Y..
+00007af0: b49c 11c7 64dd 93a6 9ecc 8adb 7a3a 3118  ....d.......z:1.
+00007b00: 7b3a 3158 7b3a 3198 7b3a 31d8 7b3c b15c  {:1X{:1.{:1.{<.\
+00007b10: 9b4f 0d74 4e3d 1c39 be54 a326 340b 9500  .O.tN=.9.T.&4...
+00007b20: d7dc 4054 95f1 7126 ceee 02cf bda4 f202  ..@T..q&........
+00007b30: 1d11 3f48 ca38 cdbe 355e 7e26 2a85 9cd5  ..?H.8..5^~&*...
+00007b40: ae55 3bf6 ff13 bcfe 0d00 00ff ff03 0050  .U;............P
+00007b50: 4b03 0414 0006 0008 0000 0021 0021 8e30  K..........!.!.0
+00007b60: 52bb 0100 007d 0400 0018 0028 0063 7573  R....}.....(.cus
+00007b70: 746f 6d58 6d6c 2f69 7465 6d50 726f 7073  tomXml/itemProps
+00007b80: 322e 786d 6c20 a224 0028 a020 0000 0000  2.xml .$.(. ....
+00007b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007ba0: 0000 0000 0000 0000 0000 0000 00b4 94dd  ................
+00007bb0: 6adc 3010 85ef 0b7d 07a3 7b59 f2bf 36c4  j.0....}..{Y..6.
+00007bc0: 1bca ae03 8106 4a9a 406e c7b2 bc2b 6a49  ......J.@n...+jI
+00007bd0: 4692 bb2d a5ef 5ed9 4929 6936 6c4a db2b  F..-..^.I)i6lJ.+
+00007be0: 7964 66ce ccd1 279d 5f7c 5143 f459 5827  ydf...'._|QC.YX'
+00007bf0: 8dae 5112 5314 09cd 4d27 f5ae 4677 b797  ..Q.S...M'..Fw..
+00007c00: 98a1 c879 d01d 0c46 8b1a 6983 2ed6 6fdf  ...y...F..i...o.
+00007c10: 9c77 eeac 030f ce1b 2bae bc50 51d8 9061  .w......+..PQ..a
+00007c20: bdda d6e8 1b2b d9b6 69d2 0c17 6c53 e2fc  .....+..i...lS..
+00007c30: b2d8 e215 cb18 ce92 324f 9a26 df34 79fa  ........2O.&.4y.
+00007c40: 1d45 415a 8732 ae46 7bef c733 421c df0b  .EAZ.2.F{..3B...
+00007c50: 052e 36a3 d0e1 676f ac02 1f42 bb23 a6ef  ..6...go...B.#..
+00007c60: 2517 5bc3 2725 b427 29a5 25e1 5390 57f7  %.[.'%.').%.S.W.
+00007c70: 6a40 ebb9 9f87 ec1b d1bb a7e1 dcda 64e5  j@............d.
+00007c80: 3315 25b9 35ce f43e e646 3d0a 3c14 56c2  3.%.5..>.F=.<.V.
+00007c90: c33c 1de1 46fb 2077 fb75 1488 fcb3 aaa3  .<..F. w.u......
+00007ca0: 0d03 5a2f 8523 b3d2 3bef ad6c 272f dc29  ..Z/.#..;..l'/.)
+00007cb0: 8dc3 e110 1fb2 c58f 6040 42ee afdf 7f5c  ........`@B....\
+00007cc0: 2cfb 2fcd bd58 b4ad 6809 659f 615a f52d  ,./..X..h.e.aZ.-
+00007cd0: cedb 70b2 aca0 0586 aa2a 4ace 9255 9bc3  ..p......*J..U..
+00007ce0: 8bc9 3461 0974 4585 8b55 91e2 9c86 2fe8  ..4a.tE..U..../.
+00007cf0: a1c7 15cd a04b 69b6 02ce fe7e 9cee 1194  .....Ki....~....
+00007d00: 6bd0 b013 0b32 3e1c e249 877f 1278 940d  k....2>..I...x..
+00007d10: a97b 3382 dfcf 9054 e403 58af 85dd 0444  .{3....T..X....D
+00007d20: ac19 5e5d f908 db23 f04f a1cb 67ec 5981  ..^]...#.O..g.Y.
+00007d30: 7fa1 72ca 9371 b2c3 4246 c789 1896 911d  ..r..q..BF......
+00007d40: 49e2 84fc 49a2 1756 b993 19c7 4d92 e1aa  I...I..V....M...
+00007d50: 580d 0331 6d37 6b92 dfae e41c 3f79 32d6  X..1m7k.....?y2.
+00007d60: 3f00 0000 ffff 0300 504b 0304 1400 0600  ?.......PK......
+00007d70: 0800 0000 2100 40c9 df51 5201 0000 6502  ....!.@..QR...e.
+00007d80: 0000 1100 0801 646f 6350 726f 7073 2f63  ......docProps/c
+00007d90: 6f72 652e 786d 6c20 a204 0128 a000 0100  ore.xml ...(....
 00007da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007e40: 0000 0000 0000 0000 0000 7c92 5f4f c230  ..........|._O.0
-00007e50: 14c5 df4d fc0e 4bdf b7ae 9ba0 34db 48d0  ...M..K.....4.H.
-00007e60: f024 8989 188d 6f4d 7b81 c5f5 4fda 22e0  .$....oM{...O.".
-00007e70: a7b7 1b30 4734 3ef6 9ed3 5fcf b969 31dd  ...0G4>..._..i1.
-00007e80: cb26 fa04 eb6a ad4a 4492 1445 a0b8 16b5  .&...j.JD..E....
-00007e90: 5a97 e865 398f ef50 e43c 5382 355a 4189  Z..e9..P.<S.5ZA.
-00007ea0: 0ee0 d0b4 babe 2ab8 a15c 5b78 b2da 80f5  ......*..\[x....
-00007eb0: 35b8 2890 94a3 dc94 68e3 bda1 183b be01  5.(.....h....;..
-00007ec0: c95c 121c 2a88 2b6d 25f3 e168 d7d8 30fe  .\..*.+m%..h..0.
-00007ed0: c1d6 80b3 341d 6309 9e09 e619 6e81 b1e9  ....4.c.....n...
-00007ee0: 89e8 8414 bc47 9aad 6d3a 80e0 181a 90a0  .....G..m:......
-00007ef0: bcc3 2421 f8c7 ebc1 4af7 e785 4e19 3865  ..$!....J...N.8e
-00007f00: ed0f 2674 3ac5 1db2 053f 8abd 7bef eade  ..&t:....?..{...
-00007f10: b8db ed92 5dde c508 f909 7e5b 3c3e 7755  ....].....~[<>wU
-00007f20: e35a b5bb e280 aa42 70ca 2d30 af6d 25bf  .Z.....Bp.-0.m%.
-00007f30: 9862 56d4 051e 0cdb 0536 ccf9 45d8 f5aa  .bV......6..E...
-00007f40: 0631 3b54 33bb 553a 9adb 40d0 05fe ad07  .1;T3.U:..@.....
-00007f50: 6657 e108 0611 8550 f458 e1ac bce6 f70f  fW.....P.X......
-00007f60: cb39 aab2 944c e274 1493 7c49 c634 bfa5  .9...L.t..|I.4..
-00007f70: a3ec bd7d fee2 7e1b f238 90a7 10ff 12b3  ...}..~..8......
-00007f80: 3c4e f398 8c96 6442 b311 2537 03e2 1950  <N....dB..%7...P
-00007f90: 75b9 2f3f 46f5 0d00 00ff ff03 0050 4b03  u./?F........PK.
-00007fa0: 0414 0006 0008 0000 0021 0045 d9f0 6aaa  .........!.E..j.
-00007fb0: 0100 00ad 0300 0010 0008 0164 6f63 5072  ...........docPr
-00007fc0: 6f70 732f 6170 702e 786d 6c20 a204 0128  ops/app.xml ...(
-00007fd0: a000 0100 0000 0000 0000 0000 0000 0000  ................
-00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007e90: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
+00007ea0: 9251 4bc3 3014 85df 05ff 43c9 7b9b a6dd  .QK.0.....C.{...
+00007eb0: a686 b683 297b 7220 3851 7c0b c9dd 566c  ....){r 8Q|...Vl
+00007ec0: 9292 6476 f3d7 9bb6 5bed 507c cc3d 275f  ..dv....[.P|.='_
+00007ed0: ceb9 249b 1f64 157c 82b1 a556 3922 518c  ..$..d.|...V9"Q.
+00007ee0: 0250 5c8b 526d 73f4 b25e 86b7 28b0 8e29  .P\.Rms..^..(..)
+00007ef0: c12a ad20 4747 b068 5e5c 5f65 bca6 5c1b  .*. GG.h^\_e..\.
+00007f00: 7832 ba06 e34a b081 2729 4b79 9da3 9d73  x2...J..')Ky...s
+00007f10: 35c5 d8f2 1d48 6623 ef50 5edc 6823 99f3  5....Hf#.P^.h#..
+00007f20: 47b3 c535 e31f 6c0b 3889 e319 96e0 9860  G..5..l.8......`
+00007f30: 8ee1 1618 d603 119d 9082 0fc8 7a6f aa0e  ............zo..
+00007f40: 2038 860a 2428 6731 8908 fef1 3a30 d2fe   8..$(g1....:0..
+00007f50: 79a1 5346 4e59 ba63 ed3b 9de2 8ed9 82f7  y.SFNY.c.;......
+00007f60: e2e0 3ed8 7230 364d 1335 6917 c3e7 27f8  ..>.r06M.5i...'.
+00007f70: 6df5 f8dc 550d 4bd5 ee8a 032a 32c1 2937  m...U.K....*2.)7
+00007f80: c09c 3685 fc62 8a19 5166 7834 6c17 5831  ..6..b..Qfx4l.X1
+00007f90: eb56 7ed7 9b12 c4e2 582c cc5e e960 693c  .V~.....X,.^.`i<
+00007fa0: 4167 f8b7 ee99 5d85 1e0c 22f0 a168 5fe1  Ag....]..."..h_.
+00007fb0: acbc a6f7 0feb 252a 9298 dc85 f134 24e9  ......%*.....4$.
+00007fc0: 9acc 687a 43a7 c97b fbfc c5fd 3664 3f90  ..hzC..{....6d?.
+00007fd0: a710 ff12 93b4 25a6 644d 2674 7247 d3d9  ......%.dM&trG..
+00007fe0: 8878 0614 5dee cb8f 517c 0300 00ff ff03  .x..]...Q|......
+00007ff0: 0050 4b03 0414 0006 0008 0000 0021 0045  .PK..........!.E
+00008000: d9f0 6aaa 0100 00ad 0300 0010 0008 0164  ..j............d
+00008010: 6f63 5072 6f70 732f 6170 702e 786d 6c20  ocProps/app.xml 
+00008020: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
 00008030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000080a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000080b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000080c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000080d0: 0000 009c 93c1 6edb 300c 86ef 03fa 0e82  ......n.0.......
-000080e0: ee8d 9cb4 cd8a 4056 31a4 1b72 e8b0 0049  ......@V1..r...I
-000080f0: 7b57 653a d12a 4b82 a418 c9de 66cf b217  {We:.*K.....f...
-00008100: 1b6d a38e b3f9 d41b f5ff 14f1 89a4 f8c3  .m..............
-00008110: b132 a486 10b5 b339 9d4e 324a c02a 5768  .2.....9.N2J.*Wh
-00008120: bbcb e9f3 f6db f53d 2531 495b 48e3 2ce4  .......=%1I[H.,.
-00008130: f404 913e 88ab 4f7c 1d9c 8790 3444 8225  ...>..O|....4D.%
-00008140: 6ccc e93e 25bf 602c aa3d 5432 4ed0 b6e8  l..>%.`,.=T2N...
-00008150: 942e 5432 e131 ec98 2b4b ade0 d1a9 4305  ..T2.1..+K....C.
-00008160: 36b1 5996 cd19 1c13 d802 8a6b df17 a45d  6.Y........k...]
-00008170: c545 9d3e 5ab4 70aa e18b 2fdb 9347 60c1  .E.>Z.p.../..G`.
-00008180: bf78 6fb4 9209 5f29 be6b 155c 7465 225f  .xo..._).k.\te"_
-00008190: 8f0a 0c67 4393 23dd 06d4 21e8 7412 1967  ...gC.#...!.t..g
-000081a0: c323 df28 6960 8985 4529 4d04 cece 025f  .#.(i`..E)M...._
-000081b0: 816c 9ab6 963a 44c1 ebb4 a841 2517 48d4  .l...:D....A%.H.
-000081c0: bfb0 6d33 4a5e 6584 0627 a7b5 0c5a da84  ..m3J^e..'...Z..
-000081d0: 584d 5a77 6863 e363 0a62 e57e ca48 0a20  XMZwhc.c.b.~.H. 
-000081e0: eacf 6fa3 0ec6 7186 799d d786 c32b c358  ..o...q.y....+.X
-000081f0: df8a fb36 0183 cbc4 a640 c783 c625 e956  ...6.....@...%.V
-00008200: 2703 f147 b996 218d 80e3 f8cf e02d 4387  '..G..!......-C.
-00008210: dde1 4c87 683d e46c 54bd 1955 6f47 d5bb  ..L.h=.lT..UoG..
-00008220: 5175 3eaa 7e1e 55bb 460c 9bd6 8e03 9fff  Qu>.~.U.F.......
-00008230: cf83 97ae f2d2 9ed0 e8a3 276d dfe2 b3df  ..........'m....
-00008240: ba47 99e0 7dd4 9722 dfec 6580 02b7 a35f  .G..}.."..e...._
-00008250: 855e e02b 9c72 304d 91e5 5eda 1d14 ef39  .^.+.r0M..^....9
-00008260: ff1b cd62 be74 bf4f 4ce7 93ec 26c3 9d1b  ...b.t.OL...&...
-00008270: 689c 9dff 99f8 0b00 00ff ff03 0050 4b03  h............PK.
-00008280: 0414 0006 0008 0000 0021 0075 84b7 f963  .........!.u...c
-00008290: 0100 007c 0400 0027 0000 0078 6c2f 7072  ...|...'...xl/pr
-000082a0: 696e 7465 7253 6574 7469 6e67 732f 7072  interSettings/pr
-000082b0: 696e 7465 7253 6574 7469 6e67 7334 2e62  interSettings4.b
-000082c0: 696e ec53 cd4a c340 10fe b611 512f 7af4  in.S.J.@....Q/z.
-000082d0: 50a4 788a 8742 4d53 5b8f 6993 4a24 c996  P.x..BMS[.i.J$..
-000082e0: 6cea 3dd2 8506 4212 d214 fcc1 9b0f d237  l.=...B........7
-000082f0: f145 7c02 0fbe 82ce 5685 0a22 14bd 08ce  .E|.....V.."....
-00008300: b2fb 4dbe 99f9 76b3 cb38 1841 8023 c029  ..M...v..8.A.#.)
-00008310: 6cf4 d1a1 d946 033a 3cc2 0e8d 06c5 254a  l....F.:<.....%J
-00008320: 24b4 ce70 84cf c636 b4cd 472c 34ed 0135  $..p...6..G,4..5
-00008330: 0686 a79d 7c6b 42b8 8b29 ab11 4e99 46ab  ....|kB..)..N.F.
-00008340: 47b5 150d a5f3 7363 ef12 0a6b 3415 be90  G.....sc...k4...
-00008350: 9db9 c25c 55b7 dd60 7c08 9ddd 6b75 2c9e  ...\U..`|...ku,.
-00008360: a707 dfed bcbd 1254 7a1f 7bfc c271 ff25  .......Tz.{..q.%
-00008370: fec8 0dac f3e6 3a25 0b3f 3a57 bfb6 877d  ......:%.?:W...}
-00008380: 768b 215a d43b 0e06 3060 5137 3589 31e8  v.!Z.;..0`Q75.1.
-00008390: db20 cf44 173d eaaf 26f1 5dca 50d1 e325  . .D.=..&.].P..%
-000083a0: 6750 97a9 9c1e 55b7 89ef e08e 14dd ac98  gP....U.........
-000083b0: 57fd 24c3 9087 bee0 e370 e020 7484 ed79  W.$......p. t..y
-000083c0: 1867 4929 67ca e365 22b3 2aae 923c c388  .gI)g..e".*..<..
-000083d0: 8751 68b9 1142 39cb d3f9 92e3 8582 f649  .Qh..B9........I
-000083e0: 0ba3 b890 a548 6e24 2c13 833c cd4b 3f9f  .....Hn$,..<.K?.
-000083f0: c837 cf30 2f8b 42b9 695c 49f0 00be 9c24  .7.0/.B.i\I....$
-00008400: 7174 5d48 88c8 0a6c 2bb4 61cf 8b54 5e21  qt]H...l+.a..T^!
-00008410: e081 b3ee 53d6 a9e0 c2b4 fdaf eef6 1500  ....S...........
-00008420: 00ff ff03 0050 4b01 022d 0014 0006 0008  .....PK..-......
-00008430: 0000 0021 000c c96c 1cac 0100 00c4 0900  ...!...l........
-00008440: 0013 0000 0000 0000 0000 0000 0000 0000  ................
-00008450: 0000 005b 436f 6e74 656e 745f 5479 7065  ...[Content_Type
-00008460: 735d 2e78 6d6c 504b 0102 2d00 1400 0600  s].xmlPK..-.....
-00008470: 0800 0000 2100 b555 3023 f400 0000 4c02  ....!..U0#....L.
-00008480: 0000 0b00 0000 0000 0000 0000 0000 0000  ................
-00008490: e503 0000 5f72 656c 732f 2e72 656c 7350  ...._rels/.relsP
-000084a0: 4b01 022d 0014 0006 0008 0000 0021 00fd  K..-.........!..
-000084b0: dd3f 7547 0100 00b5 0700 001a 0000 0000  .?uG............
-000084c0: 0000 0000 0000 0000 000a 0700 0078 6c2f  .............xl/
-000084d0: 5f72 656c 732f 776f 726b 626f 6f6b 2e78  _rels/workbook.x
-000084e0: 6d6c 2e72 656c 7350 4b01 022d 0014 0006  ml.relsPK..-....
-000084f0: 0008 0000 0021 009d dbc5 4f55 0200 002d  .....!....OU...-
-00008500: 0500 000f 0000 0000 0000 0000 0000 0000  ................
-00008510: 0091 0900 0078 6c2f 776f 726b 626f 6f6b  .....xl/workbook
-00008520: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-00008530: 0000 2100 9131 efca 1109 0000 112f 0000  ..!..1......./..
-00008540: 1800 0000 0000 0000 0000 0000 0000 130c  ................
-00008550: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00008560: 7368 6565 7434 2e78 6d6c 504b 0102 2d00  sheet4.xmlPK..-.
-00008570: 1400 0600 0800 0000 2100 3e65 cd63 2207  ........!.>e.c".
-00008580: 0000 3c21 0000 1800 0000 0000 0000 0000  ..<!............
-00008590: 0000 0000 5a15 0000 786c 2f77 6f72 6b73  ....Z...xl/works
-000085a0: 6865 6574 732f 7368 6565 7432 2e78 6d6c  heets/sheet2.xml
-000085b0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-000085c0: 3b6d 324b c100 0000 4201 0000 2300 0000  ;m2K....B...#...
-000085d0: 0000 0000 0000 0000 0000 b21c 0000 786c  ..............xl
-000085e0: 2f77 6f72 6b73 6865 6574 732f 5f72 656c  /worksheets/_rel
-000085f0: 732f 7368 6565 7431 2e78 6d6c 2e72 656c  s/sheet1.xml.rel
-00008600: 7350 4b01 022d 0014 0006 0008 0000 0021  sPK..-.........!
-00008610: 0013 c42c 13c2 0000 0042 0100 0023 0000  ...,.....B...#..
-00008620: 0000 0000 0000 0000 0000 00b4 1d00 0078  ...............x
-00008630: 6c2f 776f 726b 7368 6565 7473 2f5f 7265  l/worksheets/_re
-00008640: 6c73 2f73 6865 6574 322e 786d 6c2e 7265  ls/sheet2.xml.re
-00008650: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
-00008660: 2100 34a1 0992 c200 0000 4201 0000 2300  !.4.......B...#.
-00008670: 0000 0000 0000 0000 0000 0000 b71e 0000  ................
-00008680: 786c 2f77 6f72 6b73 6865 6574 732f 5f72  xl/worksheets/_r
-00008690: 656c 732f 7368 6565 7433 2e78 6d6c 2e72  els/sheet3.xml.r
-000086a0: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
-000086b0: 0021 0043 9611 a3c2 0000 0042 0100 0023  .!.C.......B...#
-000086c0: 0000 0000 0000 0000 0000 0000 00ba 1f00  ................
-000086d0: 0078 6c2f 776f 726b 7368 6565 7473 2f5f  .xl/worksheets/_
-000086e0: 7265 6c73 2f73 6865 6574 342e 786d 6c2e  rels/sheet4.xml.
-000086f0: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
-00008700: 0000 2100 64f3 3422 c200 0000 4201 0000  ..!.d.4"....B...
-00008710: 2300 0000 0000 0000 0000 0000 0000 bd20  #.............. 
-00008720: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00008730: 5f72 656c 732f 7368 6565 7435 2e78 6d6c  _rels/sheet5.xml
-00008740: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
-00008750: 0000 0021 004c 5a2a 7ac2 0000 0042 0100  ...!.LZ*z....B..
-00008760: 0023 0000 0000 0000 0000 0000 0000 00c0  .#..............
-00008770: 2100 0078 6c2f 776f 726b 7368 6565 7473  !..xl/worksheets
-00008780: 2f5f 7265 6c73 2f73 6865 6574 362e 786d  /_rels/sheet6.xm
-00008790: 6c2e 7265 6c73 504b 0102 2d00 1400 0600  l.relsPK..-.....
-000087a0: 0800 0000 2100 6b3f 0ffb c300 0000 4201  ....!.k?......B.
-000087b0: 0000 2300 0000 0000 0000 0000 0000 0000  ..#.............
-000087c0: c322 0000 786c 2f77 6f72 6b73 6865 6574  ."..xl/worksheet
-000087d0: 732f 5f72 656c 732f 7368 6565 7437 2e78  s/_rels/sheet7.x
-000087e0: 6d6c 2e72 656c 7350 4b01 022d 0014 0006  ml.relsPK..-....
-000087f0: 0008 0000 0021 00a2 341a 18c2 0000 0042  .....!..4......B
-00008800: 0100 0023 0000 0000 0000 0000 0000 0000  ...#............
-00008810: 00c7 2300 0078 6c2f 776f 726b 7368 6565  ..#..xl/workshee
-00008820: 7473 2f5f 7265 6c73 2f73 6865 6574 382e  ts/_rels/sheet8.
-00008830: 786d 6c2e 7265 6c73 504b 0102 2d00 1400  xml.relsPK..-...
-00008840: 0600 0800 0000 2100 6706 faad cc09 0000  ......!.g.......
-00008850: 9c34 0000 1800 0000 0000 0000 0000 0000  .4..............
-00008860: 0000 ca24 0000 786c 2f77 6f72 6b73 6865  ...$..xl/workshe
-00008870: 6574 732f 7368 6565 7433 2e78 6d6c 504b  ets/sheet3.xmlPK
-00008880: 0102 2d00 1400 0600 0800 0000 2100 5208  ..-.........!.R.
-00008890: 6b4e d304 0000 ec12 0000 1800 0000 0000  kN..............
-000088a0: 0000 0000 0000 0000 cc2e 0000 786c 2f77  ............xl/w
-000088b0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-000088c0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-000088d0: 0000 2100 20e6 1354 3e09 0000 5630 0000  ..!. ..T>...V0..
-000088e0: 1800 0000 0000 0000 0000 0000 0000 d533  ...............3
-000088f0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00008900: 7368 6565 7438 2e78 6d6c 504b 0102 2d00  sheet8.xmlPK..-.
-00008910: 1400 0600 0800 0000 2100 a0ba 2dd1 ee07  ........!...-...
-00008920: 0000 1527 0000 1800 0000 0000 0000 0000  ...'............
-00008930: 0000 0000 493d 0000 786c 2f77 6f72 6b73  ....I=..xl/works
-00008940: 6865 6574 732f 7368 6565 7437 2e78 6d6c  heets/sheet7.xml
-00008950: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00008960: 5435 ba69 9906 0000 ff1d 0000 1800 0000  T5.i............
-00008970: 0000 0000 0000 0000 0000 6d45 0000 786c  ..........mE..xl
-00008980: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00008990: 7436 2e78 6d6c 504b 0102 2d00 1400 0600  t6.xmlPK..-.....
-000089a0: 0800 0000 2100 573a 6683 5806 0000 071d  ....!.W:f.X.....
-000089b0: 0000 1800 0000 0000 0000 0000 0000 0000  ................
-000089c0: 3c4c 0000 786c 2f77 6f72 6b73 6865 6574  <L..xl/worksheet
-000089d0: 732f 7368 6565 7435 2e78 6d6c 504b 0102  s/sheet5.xmlPK..
-000089e0: 2d00 1400 0600 0800 0000 2100 9893 84db  -.........!.....
-000089f0: cb03 0000 390f 0000 0d00 0000 0000 0000  ....9...........
-00008a00: 0000 0000 0000 ca52 0000 786c 2f73 7479  .......R..xl/sty
-00008a10: 6c65 732e 786d 6c50 4b01 022d 0014 0006  les.xmlPK..-....
-00008a20: 0008 0000 0021 00e1 cd29 9a3b 0100 00aa  .....!...).;....
-00008a30: 0400 0014 0000 0000 0000 0000 0000 0000  ................
-00008a40: 00c0 5600 0078 6c2f 7368 6172 6564 5374  ..V..xl/sharedSt
-00008a50: 7269 6e67 732e 786d 6c50 4b01 022d 0014  rings.xmlPK..-..
-00008a60: 0006 0008 0000 0021 001a e8a8 b791 0600  .......!........
-00008a70: 00e5 1b00 0013 0000 0000 0000 0000 0000  ................
-00008a80: 0000 002d 5800 0078 6c2f 7468 656d 652f  ...-X..xl/theme/
-00008a90: 7468 656d 6531 2e78 6d6c 504b 0102 2d00  theme1.xmlPK..-.
-00008aa0: 1400 0600 0800 0000 2100 7584 b7f9 6301  ........!.u...c.
-00008ab0: 0000 7c04 0000 2700 0000 0000 0000 0000  ..|...'.........
-00008ac0: 0000 0000 ef5e 0000 786c 2f70 7269 6e74  .....^..xl/print
-00008ad0: 6572 5365 7474 696e 6773 2f70 7269 6e74  erSettings/print
-00008ae0: 6572 5365 7474 696e 6773 352e 6269 6e50  erSettings5.binP
-00008af0: 4b01 022d 0014 0006 0008 0000 0021 0075  K..-.........!.u
-00008b00: 84b7 f963 0100 007c 0400 0027 0000 0000  ...c...|...'....
-00008b10: 0000 0000 0000 0000 0097 6000 0078 6c2f  ..........`..xl/
-00008b20: 7072 696e 7465 7253 6574 7469 6e67 732f  printerSettings/
-00008b30: 7072 696e 7465 7253 6574 7469 6e67 7331  printerSettings1
-00008b40: 2e62 696e 504b 0102 2d00 1400 0600 0800  .binPK..-.......
-00008b50: 0000 2100 5c96 2722 c300 0000 2801 0000  ..!.\.'"....(...
-00008b60: 1e00 0000 0000 0000 0000 0000 0000 3f62  ..............?b
-00008b70: 0000 6375 7374 6f6d 586d 6c2f 5f72 656c  ..customXml/_rel
-00008b80: 732f 6974 656d 322e 786d 6c2e 7265 6c73  s/item2.xml.rels
-00008b90: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00008ba0: 743f 397a c200 0000 2801 0000 1e00 0000  t?9z....(.......
-00008bb0: 0000 0000 0000 0000 0000 4664 0000 6375  ..........Fd..cu
-00008bc0: 7374 6f6d 586d 6c2f 5f72 656c 732f 6974  stomXml/_rels/it
-00008bd0: 656d 312e 786d 6c2e 7265 6c73 504b 0102  em1.xml.relsPK..
-00008be0: 2d00 1400 0600 0800 0000 2100 7584 b7f9  -.........!.u...
-00008bf0: 6301 0000 7c04 0000 2700 0000 0000 0000  c...|...'.......
-00008c00: 0000 0000 0000 4c66 0000 786c 2f70 7269  ......Lf..xl/pri
-00008c10: 6e74 6572 5365 7474 696e 6773 2f70 7269  nterSettings/pri
-00008c20: 6e74 6572 5365 7474 696e 6773 322e 6269  nterSettings2.bi
-00008c30: 6e50 4b01 022d 0014 0006 0008 0000 0021  nPK..-.........!
-00008c40: 0075 84b7 f963 0100 007c 0400 0027 0000  .u...c...|...'..
-00008c50: 0000 0000 0000 0000 0000 00f4 6700 0078  ............g..x
-00008c60: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
-00008c70: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
-00008c80: 7333 2e62 696e 504b 0102 2d00 1400 0600  s3.binPK..-.....
-00008c90: 0800 0000 2100 7584 b7f9 6301 0000 7c04  ....!.u...c...|.
-00008ca0: 0000 2700 0000 0000 0000 0000 0000 0000  ..'.............
-00008cb0: 9c69 0000 786c 2f70 7269 6e74 6572 5365  .i..xl/printerSe
-00008cc0: 7474 696e 6773 2f70 7269 6e74 6572 5365  ttings/printerSe
-00008cd0: 7474 696e 6773 362e 6269 6e50 4b01 022d  ttings6.binPK..-
-00008ce0: 0014 0006 0008 0000 0021 0075 84b7 f963  .........!.u...c
-00008cf0: 0100 007c 0400 0027 0000 0000 0000 0000  ...|...'........
-00008d00: 0000 0000 0044 6b00 0078 6c2f 7072 696e  .....Dk..xl/prin
-00008d10: 7465 7253 6574 7469 6e67 732f 7072 696e  terSettings/prin
-00008d20: 7465 7253 6574 7469 6e67 7337 2e62 696e  terSettings7.bin
-00008d30: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00008d40: 7584 b7f9 6301 0000 7c04 0000 2700 0000  u...c...|...'...
-00008d50: 0000 0000 0000 0000 0000 ec6c 0000 786c  ...........l..xl
-00008d60: 2f70 7269 6e74 6572 5365 7474 696e 6773  /printerSettings
-00008d70: 2f70 7269 6e74 6572 5365 7474 696e 6773  /printerSettings
-00008d80: 382e 6269 6e50 4b01 022d 0014 0006 0008  8.binPK..-......
-00008d90: 0000 0021 0055 9f35 f5d4 0900 008c 3000  ...!.U.5......0.
-00008da0: 0013 0000 0000 0000 0000 0000 0000 0094  ................
-00008db0: 6e00 0063 7573 746f 6d58 6d6c 2f69 7465  n..customXml/ite
-00008dc0: 6d31 2e78 6d6c 504b 0102 2d00 1400 0600  m1.xmlPK..-.....
-00008dd0: 0800 0000 2100 218e 3052 bb01 0000 7d04  ....!.!.0R....}.
-00008de0: 0000 1800 0000 0000 0000 0000 0000 0000  ................
-00008df0: c178 0000 6375 7374 6f6d 586d 6c2f 6974  .x..customXml/it
-00008e00: 656d 5072 6f70 7331 2e78 6d6c 504b 0102  emProps1.xmlPK..
-00008e10: 2d00 1400 0600 0800 0000 2100 bd84 6223  -.........!...b#
-00008e20: 9000 0000 db00 0000 1300 0000 0000 0000  ................
-00008e30: 0000 0000 0000 da7a 0000 6375 7374 6f6d  .......z..custom
-00008e40: 586d 6c2f 6974 656d 322e 786d 6c50 4b01  Xml/item2.xmlPK.
-00008e50: 022d 0014 0006 0008 0000 0021 0087 aef1  .-.........!....
-00008e60: 14f2 0000 004f 0100 0018 0000 0000 0000  .....O..........
-00008e70: 0000 0000 0000 00c3 7b00 0063 7573 746f  ........{..custo
-00008e80: 6d58 6d6c 2f69 7465 6d50 726f 7073 322e  mXml/itemProps2.
-00008e90: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-00008ea0: 0021 0090 64ba 9b53 0100 0065 0200 0011  .!..d..S...e....
-00008eb0: 0000 0000 0000 0000 0000 0000 0013 7d00  ..............}.
-00008ec0: 0064 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
-00008ed0: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-00008ee0: 2100 45d9 f06a aa01 0000 ad03 0000 1000  !.E..j..........
-00008ef0: 0000 0000 0000 0000 0000 0000 9d7f 0000  ................
-00008f00: 646f 6350 726f 7073 2f61 7070 2e78 6d6c  docProps/app.xml
-00008f10: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00008f20: 7584 b7f9 6301 0000 7c04 0000 2700 0000  u...c...|...'...
-00008f30: 0000 0000 0000 0000 0000 7d82 0000 786c  ..........}...xl
-00008f40: 2f70 7269 6e74 6572 5365 7474 696e 6773  /printerSettings
-00008f50: 2f70 7269 6e74 6572 5365 7474 696e 6773  /printerSettings
-00008f60: 342e 6269 6e50 4b05 0600 0000 0027 0027  4.binPK......'.'
-00008f70: 0040 0b00 0025 8400 0000 00              .@...%.....
+000080d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000080e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000080f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008120: 0000 0000 0000 009c 93c1 6edb 300c 86ef  ..........n.0...
+00008130: 03fa 0e82 ee8d 9cb4 cd8a 4056 31a4 1b72  ..........@V1..r
+00008140: e8b0 0049 7b57 653a d12a 4b82 a418 c9de  ...I{We:.*K.....
+00008150: 66cf b217 1b6d a38e b3f9 d41b f5ff 14f1  f....m..........
+00008160: 89a4 f8c3 b132 a486 10b5 b339 9d4e 324a  .....2.....9.N2J
+00008170: c02a 5768 bbcb e9f3 f6db f53d 2531 495b  .*Wh.......=%1I[
+00008180: 48e3 2ce4 f404 913e 88ab 4f7c 1d9c 8790  H.,....>..O|....
+00008190: 3444 8225 6ccc e93e 25bf 602c aa3d 5432  4D.%l..>%.`,.=T2
+000081a0: 4ed0 b6e8 942e 5432 e131 ec98 2b4b ade0  N.....T2.1..+K..
+000081b0: d1a9 4305 36b1 5996 cd19 1c13 d802 8a6b  ..C.6.Y........k
+000081c0: df17 a45d c545 9d3e 5ab4 70aa e18b 2fdb  ...].E.>Z.p.../.
+000081d0: 9347 60c1 bf78 6fb4 9209 5f29 be6b 155c  .G`..xo..._).k.\
+000081e0: 7465 225f 8f0a 0c67 4393 23dd 06d4 21e8  te"_...gC.#...!.
+000081f0: 7412 1967 c323 df28 6960 8985 4529 4d04  t..g.#.(i`..E)M.
+00008200: cece 025f 816c 9ab6 963a 44c1 ebb4 a841  ..._.l...:D....A
+00008210: 2517 48d4 bfb0 6d33 4a5e 6584 0627 a7b5  %.H...m3J^e..'..
+00008220: 0c5a da84 584d 5a77 6863 e363 0a62 e57e  .Z..XMZwhc.c.b.~
+00008230: ca48 0a20 eacf 6fa3 0ec6 7186 799d d786  .H. ..o...q.y...
+00008240: c32b c358 df8a fb36 0183 cbc4 a640 c783  .+.X...6.....@..
+00008250: c625 e956 2703 f147 b996 218d 80e3 f8cf  .%.V'..G..!.....
+00008260: e02d 4387 dde1 4c87 683d e46c 54bd 1955  .-C...L.h=.lT..U
+00008270: 6f47 d5bb 5175 3eaa 7e1e 55bb 460c 9bd6  oG..Qu>.~.U.F...
+00008280: 8e03 9fff cf83 97ae f2d2 9ed0 e8a3 276d  ..............'m
+00008290: dfe2 b3df ba47 99e0 7dd4 9722 dfec 6580  .....G..}.."..e.
+000082a0: 02b7 a35f 855e e02b 9c72 304d 91e5 5eda  ..._.^.+.r0M..^.
+000082b0: 1d14 ef39 ff1b cd62 be74 bf4f 4ce7 93ec  ...9...b.t.OL...
+000082c0: 26c3 9d1b 689c 9dff 99f8 0b00 00ff ff03  &...h...........
+000082d0: 0050 4b03 0414 0006 0008 0000 0021 0075  .PK..........!.u
+000082e0: 84b7 f963 0100 007c 0400 0027 0000 0078  ...c...|...'...x
+000082f0: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
+00008300: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
+00008310: 7334 2e62 696e ec53 cd4a c340 10fe b611  s4.bin.S.J.@....
+00008320: 512f 7af4 50a4 788a 8742 4d53 5b8f 6993  Q/z.P.x..BMS[.i.
+00008330: 4a24 c996 6cea 3dd2 8506 4212 d214 fcc1  J$..l.=...B.....
+00008340: 9b0f d237 f145 7c02 0fbe 82ce 5685 0a22  ...7.E|.....V.."
+00008350: 14bd 08ce b2fb 4dbe 99f9 76b3 cb38 1841  ......M...v..8.A
+00008360: 8023 c029 6cf4 d1a1 d946 033a 3cc2 0e8d  .#.)l....F.:<...
+00008370: 06c5 254a 24b4 ce70 84cf c636 b4cd 472c  ..%J$..p...6..G,
+00008380: 34ed 0135 0686 a79d 7c6b 42b8 8b29 ab11  4..5....|kB..)..
+00008390: 4e99 46ab 47b5 150d a5f3 7363 ef12 0a6b  N.F.G.....sc...k
+000083a0: 3415 be90 9db9 c25c 55b7 dd60 7c08 9ddd  4......\U..`|...
+000083b0: 6b75 2c9e a707 dfed bcbd 1254 7a1f 7bfc  ku,........Tz.{.
+000083c0: c271 ff25 fec8 0dac f3e6 3a25 0b3f 3a57  .q.%......:%.?:W
+000083d0: bfb6 877d 768b 215a d43b 0e06 3060 5137  ...}v.!Z.;..0`Q7
+000083e0: 3589 31e8 db20 cf44 173d eaaf 26f1 5dca  5.1.. .D.=..&.].
+000083f0: 50d1 e325 6750 97a9 9c1e 55b7 89ef e08e  P..%gP....U.....
+00008400: 14dd ac98 57fd 24c3 9087 bee0 e370 e020  ....W.$......p. 
+00008410: 7484 ed79 1867 4929 67ca e365 22b3 2aae  t..y.gI)g..e".*.
+00008420: 923c c388 8751 68b9 1142 39cb d3f9 92e3  .<...Qh..B9.....
+00008430: 8582 f649 0ba3 b890 a548 6e24 2c13 833c  ...I.....Hn$,..<
+00008440: cd4b 3f9f c837 cf30 2f8b 42b9 695c 49f0  .K?..7.0/.B.i\I.
+00008450: 00be 9c24 7174 5d48 88c8 0a6c 2bb4 61cf  ...$qt]H...l+.a.
+00008460: 8b54 5e21 e081 b3ee 53d6 a9e0 c2b4 fdaf  .T^!....S.......
+00008470: eef6 1500 00ff ff03 0050 4b01 022d 0014  .........PK..-..
+00008480: 0006 0008 0000 0021 000c c96c 1cac 0100  .......!...l....
+00008490: 00c4 0900 0013 0000 0000 0000 0000 0000  ................
+000084a0: 0000 0000 0000 005b 436f 6e74 656e 745f  .......[Content_
+000084b0: 5479 7065 735d 2e78 6d6c 504b 0102 2d00  Types].xmlPK..-.
+000084c0: 1400 0600 0800 0000 2100 b555 3023 f400  ........!..U0#..
+000084d0: 0000 4c02 0000 0b00 0000 0000 0000 0000  ..L.............
+000084e0: 0000 0000 e503 0000 5f72 656c 732f 2e72  ........_rels/.r
+000084f0: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
+00008500: 0021 00fd dd3f 7547 0100 00b5 0700 001a  .!...?uG........
+00008510: 0000 0000 0000 0000 0000 0000 000a 0700  ................
+00008520: 0078 6c2f 5f72 656c 732f 776f 726b 626f  .xl/_rels/workbo
+00008530: 6f6b 2e78 6d6c 2e72 656c 7350 4b01 022d  ok.xml.relsPK..-
+00008540: 0014 0006 0008 0000 0021 00da d77d d486  .........!...}..
+00008550: 0200 008a 0500 000f 0000 0000 0000 0000  ................
+00008560: 0000 0000 0091 0900 0078 6c2f 776f 726b  .........xl/work
+00008570: 626f 6f6b 2e78 6d6c 504b 0102 2d00 1400  book.xmlPK..-...
+00008580: 0600 0800 0000 2100 b621 0fa0 1a09 0000  ......!..!......
+00008590: 342f 0000 1800 0000 0000 0000 0000 0000  4/..............
+000085a0: 0000 440c 0000 786c 2f77 6f72 6b73 6865  ..D...xl/workshe
+000085b0: 6574 732f 7368 6565 7434 2e78 6d6c 504b  ets/sheet4.xmlPK
+000085c0: 0102 2d00 1400 0600 0800 0000 2100 e158  ..-.........!..X
+000085d0: 495a 2a07 0000 5f21 0000 1800 0000 0000  IZ*..._!........
+000085e0: 0000 0000 0000 0000 9415 0000 786c 2f77  ............xl/w
+000085f0: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
+00008600: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00008610: 0000 2100 3b6d 324b c100 0000 4201 0000  ..!.;m2K....B...
+00008620: 2300 0000 0000 0000 0000 0000 0000 f41c  #...............
+00008630: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00008640: 5f72 656c 732f 7368 6565 7431 2e78 6d6c  _rels/sheet1.xml
+00008650: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
+00008660: 0000 0021 0013 c42c 13c2 0000 0042 0100  ...!...,.....B..
+00008670: 0023 0000 0000 0000 0000 0000 0000 00f6  .#..............
+00008680: 1d00 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00008690: 2f5f 7265 6c73 2f73 6865 6574 322e 786d  /_rels/sheet2.xm
+000086a0: 6c2e 7265 6c73 504b 0102 2d00 1400 0600  l.relsPK..-.....
+000086b0: 0800 0000 2100 34a1 0992 c200 0000 4201  ....!.4.......B.
+000086c0: 0000 2300 0000 0000 0000 0000 0000 0000  ..#.............
+000086d0: f91e 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+000086e0: 732f 5f72 656c 732f 7368 6565 7433 2e78  s/_rels/sheet3.x
+000086f0: 6d6c 2e72 656c 7350 4b01 022d 0014 0006  ml.relsPK..-....
+00008700: 0008 0000 0021 0043 9611 a3c2 0000 0042  .....!.C.......B
+00008710: 0100 0023 0000 0000 0000 0000 0000 0000  ...#............
+00008720: 00fc 1f00 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+00008730: 7473 2f5f 7265 6c73 2f73 6865 6574 342e  ts/_rels/sheet4.
+00008740: 786d 6c2e 7265 6c73 504b 0102 2d00 1400  xml.relsPK..-...
+00008750: 0600 0800 0000 2100 64f3 3422 c200 0000  ......!.d.4"....
+00008760: 4201 0000 2300 0000 0000 0000 0000 0000  B...#...........
+00008770: 0000 ff20 0000 786c 2f77 6f72 6b73 6865  ... ..xl/workshe
+00008780: 6574 732f 5f72 656c 732f 7368 6565 7435  ets/_rels/sheet5
+00008790: 2e78 6d6c 2e72 656c 7350 4b01 022d 0014  .xml.relsPK..-..
+000087a0: 0006 0008 0000 0021 004c 5a2a 7ac2 0000  .......!.LZ*z...
+000087b0: 0042 0100 0023 0000 0000 0000 0000 0000  .B...#..........
+000087c0: 0000 0002 2200 0078 6c2f 776f 726b 7368  ...."..xl/worksh
+000087d0: 6565 7473 2f5f 7265 6c73 2f73 6865 6574  eets/_rels/sheet
+000087e0: 362e 786d 6c2e 7265 6c73 504b 0102 2d00  6.xml.relsPK..-.
+000087f0: 1400 0600 0800 0000 2100 6b3f 0ffb c300  ........!.k?....
+00008800: 0000 4201 0000 2300 0000 0000 0000 0000  ..B...#.........
+00008810: 0000 0000 0523 0000 786c 2f77 6f72 6b73  .....#..xl/works
+00008820: 6865 6574 732f 5f72 656c 732f 7368 6565  heets/_rels/shee
+00008830: 7437 2e78 6d6c 2e72 656c 7350 4b01 022d  t7.xml.relsPK..-
+00008840: 0014 0006 0008 0000 0021 00a2 341a 18c2  .........!..4...
+00008850: 0000 0042 0100 0023 0000 0000 0000 0000  ...B...#........
+00008860: 0000 0000 0009 2400 0078 6c2f 776f 726b  ......$..xl/work
+00008870: 7368 6565 7473 2f5f 7265 6c73 2f73 6865  sheets/_rels/she
+00008880: 6574 382e 786d 6c2e 7265 6c73 504b 0102  et8.xml.relsPK..
+00008890: 2d00 1400 0600 0800 0000 2100 962f 4caa  -.........!../L.
+000088a0: d009 0000 bf34 0000 1800 0000 0000 0000  .....4..........
+000088b0: 0000 0000 0000 0c25 0000 786c 2f77 6f72  .......%..xl/wor
+000088c0: 6b73 6865 6574 732f 7368 6565 7433 2e78  ksheets/sheet3.x
+000088d0: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+000088e0: 2100 fcab ce49 d904 0000 0d13 0000 1800  !....I..........
+000088f0: 0000 0000 0000 0000 0000 0000 122f 0000  ............./..
+00008900: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00008910: 6565 7431 2e78 6d6c 504b 0102 2d00 1400  eet1.xmlPK..-...
+00008920: 0600 0800 0000 2100 4a65 87bc 3209 0000  ......!.Je..2...
+00008930: 5730 0000 1800 0000 0000 0000 0000 0000  W0..............
+00008940: 0000 2134 0000 786c 2f77 6f72 6b73 6865  ..!4..xl/workshe
+00008950: 6574 732f 7368 6565 7438 2e78 6d6c 504b  ets/sheet8.xmlPK
+00008960: 0102 2d00 1400 0600 0800 0000 2100 073a  ..-.........!..:
+00008970: 3d1b ee07 0000 3827 0000 1800 0000 0000  =.....8'........
+00008980: 0000 0000 0000 0000 893d 0000 786c 2f77  .........=..xl/w
+00008990: 6f72 6b73 6865 6574 732f 7368 6565 7437  orksheets/sheet7
+000089a0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+000089b0: 0000 2100 5f4c d64a 9e06 0000 241e 0000  ..!._L.J....$...
+000089c0: 1800 0000 0000 0000 0000 0000 0000 ad45  ...............E
+000089d0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+000089e0: 7368 6565 7436 2e78 6d6c 504b 0102 2d00  sheet6.xmlPK..-.
+000089f0: 1400 0600 0800 0000 2100 f42a 3e23 6206  ........!..*>#b.
+00008a00: 0000 281d 0000 1800 0000 0000 0000 0000  ..(.............
+00008a10: 0000 0000 814c 0000 786c 2f77 6f72 6b73  .....L..xl/works
+00008a20: 6865 6574 732f 7368 6565 7435 2e78 6d6c  heets/sheet5.xml
+00008a30: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00008a40: 9893 84db cb03 0000 390f 0000 0d00 0000  ........9.......
+00008a50: 0000 0000 0000 0000 0000 1953 0000 786c  ...........S..xl
+00008a60: 2f73 7479 6c65 732e 786d 6c50 4b01 022d  /styles.xmlPK..-
+00008a70: 0014 0006 0008 0000 0021 000c 1434 0041  .........!...4.A
+00008a80: 0100 00bf 0400 0014 0000 0000 0000 0000  ................
+00008a90: 0000 0000 000f 5700 0078 6c2f 7368 6172  ......W..xl/shar
+00008aa0: 6564 5374 7269 6e67 732e 786d 6c50 4b01  edStrings.xmlPK.
+00008ab0: 022d 0014 0006 0008 0000 0021 001a e8a8  .-.........!....
+00008ac0: b791 0600 00e5 1b00 0013 0000 0000 0000  ................
+00008ad0: 0000 0000 0000 0082 5800 0078 6c2f 7468  ........X..xl/th
+00008ae0: 656d 652f 7468 656d 6531 2e78 6d6c 504b  eme/theme1.xmlPK
+00008af0: 0102 2d00 1400 0600 0800 0000 2100 7584  ..-.........!.u.
+00008b00: b7f9 6301 0000 7c04 0000 2700 0000 0000  ..c...|...'.....
+00008b10: 0000 0000 0000 0000 445f 0000 786c 2f70  ........D_..xl/p
+00008b20: 7269 6e74 6572 5365 7474 696e 6773 2f70  rinterSettings/p
+00008b30: 7269 6e74 6572 5365 7474 696e 6773 352e  rinterSettings5.
+00008b40: 6269 6e50 4b01 022d 0014 0006 0008 0000  binPK..-........
+00008b50: 0021 0075 84b7 f963 0100 007c 0400 0027  .!.u...c...|...'
+00008b60: 0000 0000 0000 0000 0000 0000 00ec 6000  ..............`.
+00008b70: 0078 6c2f 7072 696e 7465 7253 6574 7469  .xl/printerSetti
+00008b80: 6e67 732f 7072 696e 7465 7253 6574 7469  ngs/printerSetti
+00008b90: 6e67 7331 2e62 696e 504b 0102 2d00 1400  ngs1.binPK..-...
+00008ba0: 0600 0800 0000 2100 5c96 2722 c300 0000  ......!.\.'"....
+00008bb0: 2801 0000 1e00 0000 0000 0000 0000 0000  (...............
+00008bc0: 0000 9462 0000 6375 7374 6f6d 586d 6c2f  ...b..customXml/
+00008bd0: 5f72 656c 732f 6974 656d 322e 786d 6c2e  _rels/item2.xml.
+00008be0: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
+00008bf0: 0000 2100 743f 397a c200 0000 2801 0000  ..!.t?9z....(...
+00008c00: 1e00 0000 0000 0000 0000 0000 0000 9b64  ...............d
+00008c10: 0000 6375 7374 6f6d 586d 6c2f 5f72 656c  ..customXml/_rel
+00008c20: 732f 6974 656d 312e 786d 6c2e 7265 6c73  s/item1.xml.rels
+00008c30: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00008c40: 7584 b7f9 6301 0000 7c04 0000 2700 0000  u...c...|...'...
+00008c50: 0000 0000 0000 0000 0000 a166 0000 786c  ...........f..xl
+00008c60: 2f70 7269 6e74 6572 5365 7474 696e 6773  /printerSettings
+00008c70: 2f70 7269 6e74 6572 5365 7474 696e 6773  /printerSettings
+00008c80: 322e 6269 6e50 4b01 022d 0014 0006 0008  2.binPK..-......
+00008c90: 0000 0021 0075 84b7 f963 0100 007c 0400  ...!.u...c...|..
+00008ca0: 0027 0000 0000 0000 0000 0000 0000 0049  .'.............I
+00008cb0: 6800 0078 6c2f 7072 696e 7465 7253 6574  h..xl/printerSet
+00008cc0: 7469 6e67 732f 7072 696e 7465 7253 6574  tings/printerSet
+00008cd0: 7469 6e67 7333 2e62 696e 504b 0102 2d00  tings3.binPK..-.
+00008ce0: 1400 0600 0800 0000 2100 7584 b7f9 6301  ........!.u...c.
+00008cf0: 0000 7c04 0000 2700 0000 0000 0000 0000  ..|...'.........
+00008d00: 0000 0000 f169 0000 786c 2f70 7269 6e74  .....i..xl/print
+00008d10: 6572 5365 7474 696e 6773 2f70 7269 6e74  erSettings/print
+00008d20: 6572 5365 7474 696e 6773 362e 6269 6e50  erSettings6.binP
+00008d30: 4b01 022d 0014 0006 0008 0000 0021 0075  K..-.........!.u
+00008d40: 84b7 f963 0100 007c 0400 0027 0000 0000  ...c...|...'....
+00008d50: 0000 0000 0000 0000 0099 6b00 0078 6c2f  ..........k..xl/
+00008d60: 7072 696e 7465 7253 6574 7469 6e67 732f  printerSettings/
+00008d70: 7072 696e 7465 7253 6574 7469 6e67 7337  printerSettings7
+00008d80: 2e62 696e 504b 0102 2d00 1400 0600 0800  .binPK..-.......
+00008d90: 0000 2100 7584 b7f9 6301 0000 7c04 0000  ..!.u...c...|...
+00008da0: 2700 0000 0000 0000 0000 0000 0000 416d  '.............Am
+00008db0: 0000 786c 2f70 7269 6e74 6572 5365 7474  ..xl/printerSett
+00008dc0: 696e 6773 2f70 7269 6e74 6572 5365 7474  ings/printerSett
+00008dd0: 696e 6773 382e 6269 6e50 4b01 022d 0014  ings8.binPK..-..
+00008de0: 0006 0008 0000 0021 00bd 8462 2390 0000  .......!...b#...
+00008df0: 00db 0000 0013 0000 0000 0000 0000 0000  ................
+00008e00: 0000 00e9 6e00 0063 7573 746f 6d58 6d6c  ....n..customXml
+00008e10: 2f69 7465 6d31 2e78 6d6c 504b 0102 2d00  /item1.xmlPK..-.
+00008e20: 1400 0600 0800 0000 2100 87ae f114 f200  ........!.......
+00008e30: 0000 4f01 0000 1800 0000 0000 0000 0000  ..O.............
+00008e40: 0000 0000 d26f 0000 6375 7374 6f6d 586d  .....o..customXm
+00008e50: 6c2f 6974 656d 5072 6f70 7331 2e78 6d6c  l/itemProps1.xml
+00008e60: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00008e70: 559f 35f5 d409 0000 8c30 0000 1300 0000  U.5......0......
+00008e80: 0000 0000 0000 0000 0000 2271 0000 6375  .........."q..cu
+00008e90: 7374 6f6d 586d 6c2f 6974 656d 322e 786d  stomXml/item2.xm
+00008ea0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+00008eb0: 0021 8e30 52bb 0100 007d 0400 0018 0000  .!.0R....}......
+00008ec0: 0000 0000 0000 0000 0000 004f 7b00 0063  ...........O{..c
+00008ed0: 7573 746f 6d58 6d6c 2f69 7465 6d50 726f  ustomXml/itemPro
+00008ee0: 7073 322e 786d 6c50 4b01 022d 0014 0006  ps2.xmlPK..-....
+00008ef0: 0008 0000 0021 0040 c9df 5152 0100 0065  .....!.@..QR...e
+00008f00: 0200 0011 0000 0000 0000 0000 0000 0000  ................
+00008f10: 0068 7d00 0064 6f63 5072 6f70 732f 636f  .h}..docProps/co
+00008f20: 7265 2e78 6d6c 504b 0102 2d00 1400 0600  re.xmlPK..-.....
+00008f30: 0800 0000 2100 45d9 f06a aa01 0000 ad03  ....!.E..j......
+00008f40: 0000 1000 0000 0000 0000 0000 0000 0000  ................
+00008f50: f17f 0000 646f 6350 726f 7073 2f61 7070  ....docProps/app
+00008f60: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00008f70: 0000 2100 7584 b7f9 6301 0000 7c04 0000  ..!.u...c...|...
+00008f80: 2700 0000 0000 0000 0000 0000 0000 d182  '...............
+00008f90: 0000 786c 2f70 7269 6e74 6572 5365 7474  ..xl/printerSett
+00008fa0: 696e 6773 2f70 7269 6e74 6572 5365 7474  ings/printerSett
+00008fb0: 696e 6773 342e 6269 6e50 4b05 0600 0000  ings4.binPK.....
+00008fc0: 0027 0027 0040 0b00 0079 8400 0000 00    .'.'.@...y.....
```

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/custom_molecules_set.docx` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/custom_molecules_set.docx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_TMS_optB.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_optB.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_optB.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_optB.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_optB.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_optB.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_optB.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_optB.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_optB.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/0_TMS_Custom_MMFF.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_MMFF.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_MMFF.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_MMFF.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_MMFF.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_MMFF.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_MMFF.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_MMFF.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_MMFF.gjc` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a - copia.xlsx` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a - copia.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.4/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/output_module.py` & `dp4plus_app-0.1.4/src/dp4plus_app/output_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         #for programming porpuse it's recommended to get the output at desktop
         #desktop = os.path.normpath(os.path.expanduser("~/Desktop"))
         #cwf = os.getcwd().split('\\')[-1]   #current work folder 
         #time = strftime("%H%M", gmtime())
         #output_file = os.path.join(desktop,f'{cwf}_results_{time}.xlsx')
         
     outputs['results'] = rearrange_results (outputs['results'])
-        
+    
     with pd.ExcelWriter(output_file) as writer: 
     
         for sheet, matrix in outputs.items(): 
             if 'exp' in sheet : 
                 exp_highlights = warn.exp_data_control(matrix)
                 continue
```

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app/validation_module.py` & `dp4plus_app-0.1.4/src/dp4plus_app/validation_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app.egg-info/PKG-INFO` & `dp4plus_app-0.1.4/src/dp4plus_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp4plus-app
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool to simplify your DP4+ calculations
 Home-page: https://github.com/RosarioCCLab/DP4plus-App
 Author: Bruno A. Franco
 Author-email: bruno.agustin.franco@gmail.com
 License: MIT
 Keywords: nmr
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dp4plus_app-0.1.3/src/dp4plus_app.egg-info/SOURCES.txt` & `dp4plus_app-0.1.4/src/dp4plus_app.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -23,32 +23,44 @@
 src/dp4plus_app.egg-info/requires.txt
 src/dp4plus_app.egg-info/top_level.txt
 src/dp4plus_app/UserGuide/UserGuide.docx
 src/dp4plus_app/UserGuide/UserGuide.pdf
 src/dp4plus_app/UserGuide/UserGuideFigures.pptx
 src/dp4plus_app/nmr_custom/Data_traning_set.xlsx
 src/dp4plus_app/nmr_custom/custom_molecules_set.docx
-src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_TMS_optB.gjc
-src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_optB.gjc
-src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_optB.gjc
-src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_optB.gjc
-src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_optB.gjc
-src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_optB.gjc
-src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_optB.gjc
-src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_optB.gjc
-src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_optB.gjc
-src/dp4plus_app/nmr_custom/opt_MMFF/0_TMS_Custom_MMFF.gjc
-src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_MMFF.gjc
-src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_MMFF.gjc
-src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_MMFF.gjc
-src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_MMFF.gjc
-src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_MMFF.gjc
-src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_MMFF.gjc
-src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_MMFF.gjc
-src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc
+src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc
+src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc
 src/dp4plus_app/nmr_examples/73a - copia.xlsx
 src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log
 src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log
 src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log
 src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log
 src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log
 src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log
```

