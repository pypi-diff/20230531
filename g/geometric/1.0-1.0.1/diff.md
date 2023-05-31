# Comparing `tmp/geometric-1.0.tar.gz` & `tmp/geometric-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geometric-1.0.tar", last modified: Wed Oct 12 18:28:08 2022, max compression
+gzip compressed data, was "geometric-1.0.1.tar", last modified: Wed May 31 04:19:31 2023, max compression
```

## Comparing `geometric-1.0.tar` & `geometric-1.0.1.tar`

### file list

```diff
@@ -1,114 +1,113 @@
-drwxrwxr-x   0 leeping   (1000) leeping   (1000)        0 2022-10-12 18:28:08.069453 geometric-1.0/
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1717 2022-07-07 22:43:37.000000 geometric-1.0/LICENSE
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      322 2020-03-10 22:26:43.000000 geometric-1.0/MANIFEST.in
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     3155 2022-10-12 18:28:08.069453 geometric-1.0/PKG-INFO
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     2665 2022-10-04 16:36:18.000000 geometric-1.0/README.md
-drwxrwxr-x   0 leeping   (1000) leeping   (1000)        0 2022-10-12 18:28:08.069453 geometric-1.0/geometric/
--rw-rw-r--   0 leeping   (1000) leeping   (1000)   105233 2019-03-09 19:11:45.000000 geometric-1.0/geometric/PDB.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     2115 2020-03-10 22:26:43.000000 geometric-1.0/geometric/__init__.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      495 2022-10-12 18:28:08.069453 geometric-1.0/geometric/_version.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     3883 2022-10-11 01:28:47.000000 geometric-1.0/geometric/ase_engine.py
-drwxrwxr-x   0 leeping   (1000) leeping   (1000)        0 2022-10-12 18:28:08.065453 geometric-1.0/geometric/config/
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      838 2022-09-23 01:34:27.000000 geometric-1.0/geometric/config/log.ini
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      409 2022-09-23 01:36:45.000000 geometric-1.0/geometric/config/logConsole.ini
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      334 2022-10-03 21:04:29.000000 geometric-1.0/geometric/config/logJson.ini
-drwxrwxr-x   0 leeping   (1000) leeping   (1000)        0 2022-10-12 18:28:08.069453 geometric-1.0/geometric/data/
-drwxrwxr-x   0 leeping   (1000) leeping   (1000)        0 2022-10-12 18:28:08.069453 geometric-1.0/geometric/data/TrashBox/
--rw-r--r--   0 leeping   (1000) leeping   (1000)     2811 2022-09-10 17:44:45.000000 geometric-1.0/geometric/data/TrashBox/alatet.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      566 2022-09-08 23:01:53.000000 geometric-1.0/geometric/data/TrashBox/gal-glc-cons-test.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     2632 2022-09-08 23:00:56.000000 geometric-1.0/geometric/data/TrashBox/gal-glc-cons-test.xyz
-drwxrwxr-x   0 leeping   (1000) leeping   (1000)        0 2022-10-12 18:28:08.061453 geometric-1.0/geometric/data/TrashBox/hcn_hessian/
-drwxrwxr-x   0 leeping   (1000) leeping   (1000)        0 2022-10-12 18:28:08.069453 geometric-1.0/geometric/data/TrashBox/hcn_hessian/hessian/
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     2065 2020-07-04 19:38:17.000000 geometric-1.0/geometric/data/TrashBox/hcn_hessian/hessian/hessian.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    36030 2022-09-10 16:37:43.000000 geometric-1.0/geometric/data/TrashBox/reaction_003_deci.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      165 2022-09-09 16:00:01.000000 geometric-1.0/geometric/data/TrashBox/test.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1437 2020-07-04 23:46:20.000000 geometric-1.0/geometric/data/adamantane.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1929 2019-03-09 19:11:45.000000 geometric-1.0/geometric/data/ala.pdb
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1879 2019-03-09 19:11:45.000000 geometric-1.0/geometric/data/ala_a99sb_min.pdb
--rw-rw-r--   0 leeping   (1000) leeping   (1000)       42 2019-03-09 19:11:45.000000 geometric-1.0/geometric/data/ala_constraints.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     2738 2019-03-09 19:11:45.000000 geometric-1.0/geometric/data/alaglu.gro
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      887 2019-03-12 04:43:12.000000 geometric-1.0/geometric/data/assort.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1227 2020-07-04 23:46:20.000000 geometric-1.0/geometric/data/bicyclo222octane.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      227 2022-09-07 23:46:30.000000 geometric-1.0/geometric/data/bucky-argmin-indices.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1343 2022-09-07 23:40:01.000000 geometric-1.0/geometric/data/bucky-energies.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     3266 2020-07-04 23:46:20.000000 geometric-1.0/geometric/data/c60.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1815 2019-04-17 14:17:13.000000 geometric-1.0/geometric/data/captan.pdb
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    33354 2019-04-17 14:17:13.000000 geometric-1.0/geometric/data/captan.xml
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     2964 2020-07-04 23:46:20.000000 geometric-1.0/geometric/data/cholesterol.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1975 2020-07-04 23:46:20.000000 geometric-1.0/geometric/data/coronene.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      893 2020-07-04 23:46:20.000000 geometric-1.0/geometric/data/cubane.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      877 2022-07-09 22:33:34.000000 geometric-1.0/geometric/data/ethanol.pdb
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     7071 2022-07-09 22:33:34.000000 geometric-1.0/geometric/data/ethanol.xml
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     5792 2020-07-04 23:46:20.000000 geometric-1.0/geometric/data/fenestradiene.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      490 2019-03-12 04:43:12.000000 geometric-1.0/geometric/data/h2o2_h2o.pdb
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     2859 2019-03-12 04:43:12.000000 geometric-1.0/geometric/data/h2o2_h2o_system.xml
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      201 2020-07-04 23:46:20.000000 geometric-1.0/geometric/data/hcn_ts_optim.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      283 2022-10-11 01:28:47.000000 geometric-1.0/geometric/data/hcn_ts_optim_xtb.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      134 2022-10-11 01:28:47.000000 geometric-1.0/geometric/data/hcn_tsguess.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     2068 2022-09-11 15:25:51.000000 geometric-1.0/geometric/data/hcn_tsguess_hessian.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)       25 2021-01-12 04:23:09.000000 geometric-1.0/geometric/data/linalg_torsion_constraints.txt
--rw-r--r--   0 leeping   (1000) leeping   (1000)     2435 2022-09-10 17:52:34.000000 geometric-1.0/geometric/data/naphthax.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     2828 2021-01-12 04:23:09.000000 geometric-1.0/geometric/data/neu5ac.pdb
--rw-rw-r--   0 leeping   (1000) leeping   (1000)       34 2021-01-12 04:23:09.000000 geometric-1.0/geometric/data/parser_options.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1974 2020-07-04 23:46:20.000000 geometric-1.0/geometric/data/porphin.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      417 2022-09-09 17:28:55.000000 geometric-1.0/geometric/data/propynimine-ts-optimized.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    11261 2022-09-09 17:18:13.000000 geometric-1.0/geometric/data/propynimine-tsguess-hessian.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    25496 2022-09-09 19:04:35.000000 geometric-1.0/geometric/data/randn_1k.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    60976 2022-09-10 16:42:57.000000 geometric-1.0/geometric/data/reaction_000_deci.xyz
--rw-r--r--   0 leeping   (1000) leeping   (1000)    29266 2022-09-10 17:18:38.000000 geometric-1.0/geometric/data/spc216.gro
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      466 2020-07-04 23:46:20.000000 geometric-1.0/geometric/data/tetrahedrane.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    20220 2022-09-14 02:44:13.000000 geometric-1.0/geometric/data/triclinic.gro
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    14137 2020-07-04 23:46:20.000000 geometric-1.0/geometric/data/vancomycin.pdb
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     3063 2022-09-10 17:35:10.000000 geometric-1.0/geometric/data/water12.pdb
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1951 2022-09-13 16:28:56.000000 geometric-1.0/geometric/data/water12.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      789 2019-03-09 19:11:45.000000 geometric-1.0/geometric/data/water3.pdb
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1721 2019-03-11 21:48:06.000000 geometric-1.0/geometric/data/water5.xyz
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1530 2019-03-09 19:11:45.000000 geometric-1.0/geometric/data/water6.pdb
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    71747 2022-10-11 01:42:45.000000 geometric-1.0/geometric/engine.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     2664 2021-01-12 04:23:09.000000 geometric-1.0/geometric/errors.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     8080 2022-09-13 18:14:41.000000 geometric-1.0/geometric/ic_tools.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     6662 2022-09-11 20:45:27.000000 geometric-1.0/geometric/info.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)   144769 2022-10-11 01:30:19.000000 geometric-1.0/geometric/internal.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)   215190 2022-09-23 02:44:56.000000 geometric-1.0/geometric/molecule.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    63390 2022-09-23 01:33:33.000000 geometric-1.0/geometric/nifty.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    37979 2022-09-09 17:12:11.000000 geometric-1.0/geometric/normal_modes.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    54988 2022-10-03 20:44:21.000000 geometric-1.0/geometric/optimize.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    27236 2022-10-11 01:28:47.000000 geometric-1.0/geometric/params.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    28783 2022-10-12 17:53:47.000000 geometric-1.0/geometric/prepare.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    35766 2022-09-10 23:08:41.000000 geometric-1.0/geometric/rotate.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    11589 2022-10-03 21:02:51.000000 geometric-1.0/geometric/run_json.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    33411 2022-09-09 02:00:53.000000 geometric-1.0/geometric/step.py
-drwxrwxr-x   0 leeping   (1000) leeping   (1000)        0 2022-10-12 18:28:08.069453 geometric-1.0/geometric/tests/
--rw-rw-r--   0 leeping   (1000) leeping   (1000)        0 2018-03-10 18:10:00.000000 geometric-1.0/geometric/tests/__init__.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     4176 2022-10-11 01:28:47.000000 geometric-1.0/geometric/tests/addons.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      455 2022-09-23 01:23:03.000000 geometric-1.0/geometric/tests/conftest.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     2785 2022-10-11 01:28:47.000000 geometric-1.0/geometric/tests/test_ase_engine.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     8291 2022-09-23 01:37:34.000000 geometric-1.0/geometric/tests/test_batch_opt.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1778 2022-10-03 20:44:24.000000 geometric-1.0/geometric/tests/test_customengine.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      995 2019-03-20 00:37:57.000000 geometric-1.0/geometric/tests/test_diff.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     4326 2021-01-12 04:23:09.000000 geometric-1.0/geometric/tests/test_errors.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     7001 2022-10-12 17:58:28.000000 geometric-1.0/geometric/tests/test_gaussian.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     4687 2022-10-03 20:44:24.000000 geometric-1.0/geometric/tests/test_hessian.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     3226 2022-09-13 19:28:52.000000 geometric-1.0/geometric/tests/test_internal.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      871 2022-09-13 18:43:54.000000 geometric-1.0/geometric/tests/test_minimize.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    24313 2022-09-14 18:22:00.000000 geometric-1.0/geometric/tests/test_molecule.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    15611 2022-09-23 02:11:49.000000 geometric-1.0/geometric/tests/test_nifty.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    12992 2022-09-07 16:55:50.000000 geometric-1.0/geometric/tests/test_openmm.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      839 2022-09-09 15:25:14.000000 geometric-1.0/geometric/tests/test_params.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     4721 2022-10-03 20:44:24.000000 geometric-1.0/geometric/tests/test_prepare.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1207 2020-03-09 20:51:44.000000 geometric-1.0/geometric/tests/test_qcengine.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     4565 2022-09-23 01:38:07.000000 geometric-1.0/geometric/tests/test_rotate.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    12894 2022-10-03 21:11:30.000000 geometric-1.0/geometric/tests/test_run_json.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     4596 2022-09-11 15:14:12.000000 geometric-1.0/geometric/tests/test_terachem.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     7711 2022-10-11 01:28:47.000000 geometric-1.0/geometric/tests/test_transition.py
-drwxrwxr-x   0 leeping   (1000) leeping   (1000)        0 2022-10-12 18:28:08.065453 geometric-1.0/geometric.egg-info/
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     3155 2022-10-12 18:28:07.000000 geometric-1.0/geometric.egg-info/PKG-INFO
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     3013 2022-10-12 18:28:08.000000 geometric-1.0/geometric.egg-info/SOURCES.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)        1 2022-10-12 18:28:08.000000 geometric-1.0/geometric.egg-info/dependency_links.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)       63 2022-10-12 18:28:08.000000 geometric-1.0/geometric.egg-info/entry_points.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)       25 2022-10-12 18:28:08.000000 geometric-1.0/geometric.egg-info/requires.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)       10 2022-10-12 18:28:08.000000 geometric-1.0/geometric.egg-info/top_level.txt
--rw-rw-r--   0 leeping   (1000) leeping   (1000)        1 2018-08-29 02:16:34.000000 geometric-1.0/geometric.egg-info/zip-safe
--rw-rw-r--   0 leeping   (1000) leeping   (1000)      329 2022-10-12 18:28:08.069453 geometric-1.0/setup.cfg
--rw-rw-r--   0 leeping   (1000) leeping   (1000)     1123 2022-10-12 18:27:14.000000 geometric-1.0/setup.py
--rw-rw-r--   0 leeping   (1000) leeping   (1000)    68611 2018-04-04 19:08:24.000000 geometric-1.0/versioneer.py
+drwxrwxr-x   0 leeping   (1001) leeping   (1001)        0 2023-05-31 04:19:31.081202 geometric-1.0.1/
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1717 2023-05-31 04:14:33.000000 geometric-1.0.1/LICENSE
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      322 2023-05-29 17:46:29.000000 geometric-1.0.1/MANIFEST.in
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     3123 2023-05-31 04:19:31.081202 geometric-1.0.1/PKG-INFO
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2665 2023-05-31 04:14:33.000000 geometric-1.0.1/README.md
+drwxrwxr-x   0 leeping   (1001) leeping   (1001)        0 2023-05-31 04:19:31.082202 geometric-1.0.1/geometric/
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)   105233 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/PDB.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2115 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/__init__.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      497 2023-05-31 04:19:31.082202 geometric-1.0.1/geometric/_version.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     3883 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/ase_engine.py
+drwxrwxr-x   0 leeping   (1001) leeping   (1001)        0 2023-05-31 04:19:30.964201 geometric-1.0.1/geometric/config/
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      838 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/config/log.ini
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      409 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/config/logConsole.ini
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      334 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/config/logJson.ini
+drwxrwxr-x   0 leeping   (1001) leeping   (1001)        0 2023-05-31 04:19:31.048202 geometric-1.0.1/geometric/data/
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1437 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/adamantane.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1929 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/data/ala.pdb
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1879 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/data/ala_a99sb_min.pdb
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)       42 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/data/ala_constraints.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2738 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/data/alaglu.gro
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      887 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/data/assort.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1227 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/bicyclo222octane.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      227 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/bucky-argmin-indices.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1343 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/bucky-energies.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     3266 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/c60.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1815 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/data/captan.pdb
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    33354 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/data/captan.xml
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2964 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/cholesterol.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1975 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/coronene.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      893 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/cubane.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      877 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/ethanol.pdb
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     7071 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/ethanol.xml
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     5792 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/fenestradiene.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      490 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/data/h2o2_h2o.pdb
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2859 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/data/h2o2_h2o_system.xml
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      201 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/hcn_ts_optim.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      283 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/hcn_ts_optim_xtb.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      134 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/hcn_tsguess.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2068 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/hcn_tsguess_hessian.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)       25 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/linalg_torsion_constraints.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2435 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/naphthax.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2828 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/neu5ac.pdb
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)       34 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/parser_options.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1974 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/porphin.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      417 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/propynimine-ts-optimized.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    11261 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/propynimine-tsguess-hessian.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    25496 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/randn_1k.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    60976 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/reaction_000_deci.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    29266 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/spc216.gro
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      466 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/tetrahedrane.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    20220 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/triclinic.gro
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    14137 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/vancomycin.pdb
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     3063 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/water12.pdb
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1951 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/data/water12.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2065 2023-05-24 18:04:26.000000 geometric-1.0.1/geometric/data/water1_hessian_gfn2-xtb.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      789 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/data/water3.pdb
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1721 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/data/water5.xyz
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1530 2020-01-15 19:56:02.000000 geometric-1.0.1/geometric/data/water6.pdb
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    71916 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/engine.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2664 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/errors.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     8080 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/ic_tools.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     6662 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/info.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)   144769 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/internal.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     4701 2023-04-04 00:16:32.000000 geometric-1.0.1/geometric/internal1.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     4318 2023-04-03 23:24:43.000000 geometric-1.0.1/geometric/internal2.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)   177776 2023-04-19 17:03:46.000000 geometric-1.0.1/geometric/internal3.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)   171772 2023-04-19 17:03:35.000000 geometric-1.0.1/geometric/internal4.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2472 2023-05-02 17:26:34.000000 geometric-1.0.1/geometric/internal_exp.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)   147996 2023-03-25 04:43:15.000000 geometric-1.0.1/geometric/internal_heepark.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)   215190 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/molecule.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    63390 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/nifty.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    37979 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/normal_modes.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    54988 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/optimize.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    27236 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/params.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    28783 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/prepare.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    35766 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/rotate.py
+-rwxrwxr-x   0 leeping   (1001) leeping   (1001)     2125 2023-05-21 16:58:18.000000 geometric-1.0.1/geometric/run_ase.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    11589 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/run_json.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    33411 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/step.py
+drwxrwxr-x   0 leeping   (1001) leeping   (1001)        0 2023-05-31 04:19:31.080202 geometric-1.0.1/geometric/tests/
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)        0 2023-05-28 04:31:27.000000 geometric-1.0.1/geometric/tests/__init__.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     4176 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/tests/addons.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      455 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/tests/conftest.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2785 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/tests/test_ase_engine.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     8291 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/tests/test_batch_opt.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1778 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/tests/test_customengine.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      995 2023-05-28 04:31:27.000000 geometric-1.0.1/geometric/tests/test_diff.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     4326 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/tests/test_errors.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     7001 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/tests/test_gaussian.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     4687 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/tests/test_hessian.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     3226 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/tests/test_internal.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      871 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/tests/test_minimize.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    24313 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/tests/test_molecule.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    15611 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/tests/test_nifty.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    12992 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/tests/test_openmm.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      839 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/tests/test_params.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     4721 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/tests/test_prepare.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1207 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/tests/test_qcengine.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     4565 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/tests/test_rotate.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    12894 2023-05-29 17:46:29.000000 geometric-1.0.1/geometric/tests/test_run_json.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     4596 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/tests/test_terachem.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     7711 2023-05-31 04:14:34.000000 geometric-1.0.1/geometric/tests/test_transition.py
+drwxrwxr-x   0 leeping   (1001) leeping   (1001)        0 2023-05-31 04:19:30.944201 geometric-1.0.1/geometric.egg-info/
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     3123 2023-05-31 04:19:30.000000 geometric-1.0.1/geometric.egg-info/PKG-INFO
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     2963 2023-05-31 04:19:30.000000 geometric-1.0.1/geometric.egg-info/SOURCES.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)        1 2023-05-31 04:19:30.000000 geometric-1.0.1/geometric.egg-info/dependency_links.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)       63 2023-05-31 04:19:30.000000 geometric-1.0.1/geometric.egg-info/entry_points.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)       25 2023-05-31 04:19:30.000000 geometric-1.0.1/geometric.egg-info/requires.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)       10 2023-05-31 04:19:30.000000 geometric-1.0.1/geometric.egg-info/top_level.txt
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)        1 2020-02-16 04:49:40.000000 geometric-1.0.1/geometric.egg-info/zip-safe
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)      329 2023-05-31 04:19:31.082202 geometric-1.0.1/setup.cfg
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)     1083 2023-05-31 04:14:34.000000 geometric-1.0.1/setup.py
+-rw-rw-r--   0 leeping   (1001) leeping   (1001)    68611 2020-01-15 19:56:02.000000 geometric-1.0.1/versioneer.py
```

### Comparing `geometric-1.0/LICENSE` & `geometric-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geometric-1.0/PKG-INFO` & `geometric-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: geometric
-Version: 1.0
+Version: 1.0.1
 Summary: Geometry optimization for quantum chemistry
 Home-page: https://github.com/leeping/geomeTRIC
 Author: Lee-Ping Wang, Chenchen Song
-Author-email: leeping@ucdavis.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `geometric-1.0/README.md` & `geometric-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/PDB.py` & `geometric-1.0.1/geometric/PDB.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/__init__.py` & `geometric-1.0.1/geometric/__init__.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/ase_engine.py` & `geometric-1.0.1/geometric/ase_engine.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/config/log.ini` & `geometric-1.0.1/geometric/config/log.ini`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/TrashBox/alatet.xyz` & `geometric-1.0.1/geometric/data/naphthax.xyz`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-    42  Alanine Tetrapeptide (Ace-Ala-Ala-Ala-NMe)
-     1  C      0.005761    0.450195   -0.341127   224     2     4     5     6
-     2  C      0.120544    0.322351    1.165729   226     1     3     7
-     3  O      1.184321    0.549314    1.733162   227     2
-     4  H      0.733438   -0.236526   -0.825812   225     1
-     5  H      0.261504    1.488928   -0.643932   225     1
-     6  H     -1.008510    0.213621   -0.729638   225     1
-     7  N     -0.992323   -0.027798    1.848316     7     2     8    11
-     8  CA    -1.056775   -0.212956    3.293146     8     7     9    12    13
-     9  C     -2.225169   -1.145189    3.625187     9     8    10    17
-    10  O     -3.074055   -1.422177    2.777148    11     9
-    11  HN    -1.865312   -0.279878    1.362283    10     7
-    12  H     -0.116506   -0.712433    3.636164    12     8
-    13  C     -1.223418    1.159047    3.990464    13     8    14    15    16
-    14  H     -1.262376    1.060805    5.098007    14    13
-    15  H     -2.156847    1.673200    3.668277    14    13
-    16  H     -0.366699    1.829969    3.752236    14    13
-    17  N     -2.274210   -1.624539    4.888244     7     9    18    21
-    18  CA    -3.325064   -2.476386    5.429285     8    17    19    22    23
-    19  C     -3.410655   -2.256705    6.942229     9    18    20    27
-    20  O     -2.538383   -1.625612    7.539300    11    19
-    21  HN    -1.587938   -1.316944    5.591647    10    17
-    22  H     -4.305219   -2.167336    4.988305    12    18
-    23  C     -3.023686   -3.956131    5.090788    13    18    24    25    26
-    24  H     -3.814671   -4.639937    5.470962    14    23
-    25  H     -2.056767   -4.289228    5.531050    14    23
-    26  H     -2.963698   -4.108258    3.989002    14    23
-    27  N     -4.473347   -2.805309    7.573770     7    19    28    31
-    28  CA    -4.719443   -2.764264    9.009457     8    27    29    32    33
-    29  C     -5.549924   -3.987193    9.408295     9    28    30    37
-    30  O     -6.147470   -4.644980    8.557044    11    29
-    31  HN    -5.154300   -3.376414    7.053692    10    27
-    32  H     -3.739861   -2.825206    9.545519    12    28
-    33  C     -5.452831   -1.451937    9.374660    13    28    34    35    36
-    34  H     -5.645338   -1.375255   10.467369    14    33
-    35  H     -6.436392   -1.373974    8.858394    14    33
-    36  H     -4.848171   -0.561932    9.086426    14    33
-    37  N     -5.594584   -4.265677   10.734292   230    29    38    39
-    38  C     -6.329266   -5.361669   11.320069   232    37    40    41    42
-    39  HN    -5.074009   -3.688342   11.407664   231    37
-    40  H     -5.650081   -6.052809   11.865599   233    38
-    41  H     -6.863900   -5.959689   10.549330   233    38
-    42  H     -7.090201   -4.993077   12.042335   233    38
+    36  Naphthalene Crystal at 92K
+     1  C     -2.549969   -2.857734   -1.221763     2     2     5     6
+     2  C     -1.785110   -1.997028   -1.974659     2     1     3     7
+     3  C     -1.405389   -2.343330   -3.303468     2     2     4    21
+     4  C     -0.619157   -1.472526   -4.107747     2     3     8    23
+     5  C     -2.963925   -4.102164   -1.752002     2     1     9    22
+     6  H     -2.799228   -2.630232   -0.377519     5     1
+     7  H     -1.485838   -1.148202   -1.622832     5     2
+     8  H     -0.344227   -0.663498   -3.748783     5     4
+     9  H     -3.480445   -4.702104   -1.221049     5     5
+    10  C      3.378747    0.112266   -5.914699     2    11    14    15
+    11  C      2.613888    0.972972   -5.161803     2    10    12    16
+    12  C      2.234167    0.626670   -3.832994     2    11    13    30
+    13  C      1.447935    1.497474   -3.028715     2    12    17    32
+    14  C      3.792703   -1.132164   -5.384460     2    10    18    31
+    15  H      3.628006    0.339768   -6.758943     5    10
+    16  H      2.314616    1.821798   -5.513630     5    11
+    17  H      1.173005    2.306502   -3.387679     5    13
+    18  H      4.309223   -1.732104   -5.915413     5    14
+    19  C     -0.675253   -3.082266   -5.914699     2    20    23    24
+    20  C     -1.440112   -3.942972   -5.161803     2    19    21    25
+    21  C     -1.819833   -3.596670   -3.832994     2     3    20    22
+    22  C     -2.606065   -4.467474   -3.028715     2     5    21    26
+    23  C     -0.261297   -1.837836   -5.384460     2     4    19    27
+    24  H     -0.425994   -3.309768   -6.758943     5    19
+    25  H     -1.739384   -4.791798   -5.513630     5    20
+    26  H     -2.880995   -5.276502   -3.387679     5    22
+    27  H      0.255223   -1.237896   -5.915413     5    23
+    28  C      1.504031   -0.112266   -1.221763     2    29    32    33
+    29  C      2.268890   -0.972972   -1.974659     2    28    30    34
+    30  C      2.648611   -0.626670   -3.303468     2    12    29    31
+    31  C      3.434843   -1.497474   -4.107747     2    14    30    35
+    32  C      1.090075    1.132164   -1.752002     2    13    28    36
+    33  H      1.254772   -0.339768   -0.377519     5    28
+    34  H      2.568162   -1.821798   -1.622832     5    29
+    35  H      3.709773   -2.306502   -3.748783     5    31
+    36  H      0.573555    1.732104   -1.221049     5    32
```

### Comparing `geometric-1.0/geometric/data/TrashBox/gal-glc-cons-test.xyz` & `geometric-1.0.1/geometric/data/water12.xyz`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,38 @@
-48   
-From sugar-elem.mol2: Frame 1 / 1
-H        4.1933210000    6.9754300000   -1.6206110000
-C        3.2013860000    6.6579010000   -1.9246900000
-H        2.5534440000    7.5079470000   -2.1112870000
-H        2.7288480000    6.0495630000   -1.1605840000
-O        3.3526980000    5.9112070000   -3.0980420000
-C        2.0681970000    5.4304370000   -3.5985600000
-H        1.4127150000    6.2750140000   -3.8160770000
-O        1.3872450000    4.5699730000   -2.6264170000
-C        0.0841770000    3.9968410000   -3.0831000000
-H       -0.5942830000    4.8228550000   -3.3063830000
-C       -0.5265990000    3.1522530000   -1.9480650000
-H        0.1240080000    2.3082680000   -1.7142270000
-H       -1.5015940000    2.7630990000   -2.2413990000
-O       -0.6842490000    3.9620040000   -0.7677890000
-H        0.1626130000    4.3725460000   -0.5684830000
-C        0.2858980000    3.1758840000   -4.2796490000
-H        0.8837140000    2.2993420000   -4.0212810000
-C        1.0028290000    3.9762600000   -5.3939710000
-H        0.3379330000    4.7652660000   -5.7515260000
-O        1.2937510000    3.0804870000   -6.5017040000
-H        1.8105290000    3.5795160000   -7.1490060000
-C        2.3191060000    4.6143660000   -4.8967180000
-H        3.0486930000    3.8280100000   -4.6922390000
-O        2.8481670000    5.4841830000   -5.9404020000
-H        3.6312980000    5.9288990000   -5.5909890000
-O       -1.0029700000    2.7328370000   -4.7687640000
-C       -0.8688300000    1.9067440000   -5.9650820000
-H       -0.2682710000    1.0233700000   -5.7431370000
-O       -0.2171350000    2.6315740000   -7.0641160000
-C       -0.1479370000    1.9130140000   -8.3732790000
-H        0.4430460000    1.0060260000   -8.2298410000
-C        0.5734310000    2.7906400000   -9.4115090000
-H        0.0699880000    3.7519490000   -9.5242550000
-H        0.5910900000    2.2932350000  -10.3812390000
-O        1.9250530000    3.0142520000   -8.9778200000
-H        1.8912680000    3.4351960000   -8.1145790000
-C       -1.4503940000    1.5469190000   -8.8528020000
-H       -1.3479720000    0.9469220000   -9.7582270000
-O       -2.2056790000    2.7402430000   -9.1770270000
-H       -3.1071480000    2.4593720000   -9.3857240000
-C       -2.2068490000    0.7283240000   -7.7814510000
-H       -1.6710230000   -0.2112950000   -7.6315460000
-O       -3.5359390000    0.4061010000   -8.2781580000
-H       -4.0035950000   -0.0616460000   -7.5727510000
-C       -2.2913000000    1.4718940000   -6.4275010000
-H       -2.9285630000    2.3527120000   -6.5300590000
-O       -2.8820620000    0.5769020000   -5.4382220000
-H       -2.8649690000    1.0289240000   -4.5858090000
+36   
+
+O        0.3000000000   -1.0910000000   -0.6330000000
+H       -0.4390000000   -0.8620000000   -0.0190000000
+H        0.1740000000   -2.0120000000   -0.8960000000
+O        2.7390000000   -0.2860000000    0.4860000000
+H        3.0390000000   -1.1530000000    0.8770000000
+H        2.0020000000   -0.6110000000   -0.0560000000
+O       -1.9830000000   -0.3050000000    0.7960000000
+H       -2.3370000000    0.5600000000    0.6920000000
+H       -1.9570000000   -0.4760000000    1.7250000000
+O       -1.2230000000    2.6730000000   -1.1160000000
+H       -2.0300000000    2.4590000000   -0.5810000000
+H       -1.1050000000    1.9960000000   -1.7780000000
+O        2.2900000000    2.0170000000    1.8980000000
+H        1.7820000000    2.5870000000    1.2790000000
+H        2.2990000000    1.1700000000    1.4010000000
+O       -0.7930000000    0.5050000000   -2.8710000000
+H       -0.2450000000   -0.2470000000   -2.4870000000
+H       -0.5140000000    0.5970000000   -3.8110000000
+O        1.0520000000    3.7120000000    0.2390000000
+H        0.4740000000    3.1320000000   -0.3620000000
+H        0.4900000000    4.2600000000    0.7660000000
+O       -0.2150000000   -3.2390000000    1.6920000000
+H       -0.4330000000   -2.4170000000    2.1800000000
+H        0.4600000000   -3.6090000000    2.2590000000
+O        0.4560000000   -3.9690000000   -1.0250000000
+H        0.0980000000   -4.1200000000   -0.1650000000
+H        1.4240000000   -4.1060000000   -1.0260000000
+O       -3.4750000000   -2.3860000000   -0.0860000000
+H       -3.5420000000   -2.2880000000   -1.0710000000
+H       -2.9970000000   -1.5740000000    0.1970000000
+O       -3.2060000000    2.2670000000    0.7570000000
+H       -4.1230000000    2.5030000000    0.5310000000
+H       -3.2280000000    2.3890000000    1.7670000000
+O        4.9680000000    0.8690000000   -0.8350000000
+H        4.1300000000    0.5460000000   -0.4170000000
+H        5.6700000000    0.5090000000   -0.3040000000
```

### Comparing `geometric-1.0/geometric/data/adamantane.xyz` & `geometric-1.0.1/geometric/data/adamantane.xyz`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/ala.pdb` & `geometric-1.0.1/geometric/data/ala.pdb`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/ala_a99sb_min.pdb` & `geometric-1.0.1/geometric/data/ala_a99sb_min.pdb`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/alaglu.gro` & `geometric-1.0.1/geometric/data/alaglu.gro`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/assort.xyz` & `geometric-1.0.1/geometric/data/assort.xyz`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/bicyclo222octane.xyz` & `geometric-1.0.1/geometric/data/bicyclo222octane.xyz`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/bucky-energies.txt` & `geometric-1.0.1/geometric/data/bucky-energies.txt`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/c60.xyz` & `geometric-1.0.1/geometric/data/c60.xyz`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/captan.pdb` & `geometric-1.0.1/geometric/data/captan.pdb`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/captan.xml` & `geometric-1.0.1/geometric/data/captan.xml`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/cholesterol.xyz` & `geometric-1.0.1/geometric/data/cholesterol.xyz`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/coronene.xyz` & `geometric-1.0.1/geometric/data/coronene.xyz`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/cubane.xyz` & `geometric-1.0.1/geometric/data/cubane.xyz`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/ethanol.pdb` & `geometric-1.0.1/geometric/data/ethanol.pdb`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/ethanol.xml` & `geometric-1.0.1/geometric/data/ethanol.xml`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/fenestradiene.xyz` & `geometric-1.0.1/geometric/data/fenestradiene.xyz`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/h2o2_h2o_system.xml` & `geometric-1.0.1/geometric/data/h2o2_h2o_system.xml`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/hcn_tsguess_hessian.txt` & `geometric-1.0.1/geometric/data/hcn_tsguess_hessian.txt`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/neu5ac.pdb` & `geometric-1.0.1/geometric/data/neu5ac.pdb`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/porphin.xyz` & `geometric-1.0.1/geometric/data/porphin.xyz`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/propynimine-tsguess-hessian.txt` & `geometric-1.0.1/geometric/data/propynimine-tsguess-hessian.txt`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/randn_1k.txt` & `geometric-1.0.1/geometric/data/randn_1k.txt`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/reaction_000_deci.xyz` & `geometric-1.0.1/geometric/data/reaction_000_deci.xyz`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/spc216.gro` & `geometric-1.0.1/geometric/data/spc216.gro`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/triclinic.gro` & `geometric-1.0.1/geometric/data/triclinic.gro`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/vancomycin.pdb` & `geometric-1.0.1/geometric/data/vancomycin.pdb`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/water12.pdb` & `geometric-1.0.1/geometric/data/water12.pdb`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/water3.pdb` & `geometric-1.0.1/geometric/data/water3.pdb`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/water5.xyz` & `geometric-1.0.1/geometric/data/water5.xyz`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/data/water6.pdb` & `geometric-1.0.1/geometric/data/water6.pdb`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/engine.py` & `geometric-1.0.1/geometric/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     intkeys = ['charge', 'spinmult']
     Answer = OrderedDict()
     # Read from the input if provided
     if fin is not None:
         tcin_dirname = os.path.dirname(os.path.abspath(fin))
         section_mode = False
         for line in open(fin).readlines():
+            line = line.expandtabs(4)
             line = line.split("#")[0].strip()
             if len(line) == 0: continue
             if line == '$end':
                 section_mode = False
                 continue
             elif line.startswith("$"):
                 section_mode = True
@@ -177,15 +178,15 @@
     tcdef['convthre'] = "3.0e-6"
     tcdef['threall'] = "1.0e-13"
     tcdef['scf'] = "diis+a"
     tcdef['maxit'] = "50"
     # tcdef['dftgrid'] = "1"
     # tcdef['precision'] = "mixed"
     # tcdef['threspdp'] = "1.0e-8"
-    tcin = edit_tcin(fin=f_tcin, options={'run':'gradient'}, defaults=tcdef)
+    tcin = edit_tcin(fin=f_tcin, options={'run':'gradient', 'keep_scr':'yes', 'scrdir':'scr'}, defaults=tcdef)
     return tcin
 
 #====================================#
 #| Classes for external codes used  |#
 #| to calculate energy and gradient |#
 #====================================#
 
@@ -373,14 +374,16 @@
     def __init__(self, molecule, tcin, dirname=None):
         self.tcin = tcin.copy()
         # Scratch folder
         if 'scrdir' in self.tcin:
             self.scr = self.tcin['scrdir']
         else:
             self.scr = 'scr'
+        # Always specify the TeraChem scratch folder name
+        self.tcin['scrdir'] = self.scr
         # A few notes about the electronic structure method
         self.casscf = self.tcin.get('casscf', 'no').lower() == 'yes'
         self.unrestricted = (self.tcin['method'][0] == 'u')
         # Build a list of guess files
         if self.casscf and 'casguess' in self.tcin:
             # CASSCF guess uses key 'casguess' and skips SCF entirely
             guessVal = self.tcin['casguess'].split()
```

### Comparing `geometric-1.0/geometric/errors.py` & `geometric-1.0.1/geometric/errors.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/ic_tools.py` & `geometric-1.0.1/geometric/ic_tools.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/info.py` & `geometric-1.0.1/geometric/info.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/internal.py` & `geometric-1.0.1/geometric/internal.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/molecule.py` & `geometric-1.0.1/geometric/molecule.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/nifty.py` & `geometric-1.0.1/geometric/nifty.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/normal_modes.py` & `geometric-1.0.1/geometric/normal_modes.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/optimize.py` & `geometric-1.0.1/geometric/optimize.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/params.py` & `geometric-1.0.1/geometric/params.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/prepare.py` & `geometric-1.0.1/geometric/prepare.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/rotate.py` & `geometric-1.0.1/geometric/rotate.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/run_json.py` & `geometric-1.0.1/geometric/run_json.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/step.py` & `geometric-1.0.1/geometric/step.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/addons.py` & `geometric-1.0.1/geometric/tests/addons.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_ase_engine.py` & `geometric-1.0.1/geometric/tests/test_ase_engine.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_batch_opt.py` & `geometric-1.0.1/geometric/tests/test_batch_opt.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_customengine.py` & `geometric-1.0.1/geometric/tests/test_customengine.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_diff.py` & `geometric-1.0.1/geometric/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_errors.py` & `geometric-1.0.1/geometric/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_gaussian.py` & `geometric-1.0.1/geometric/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_hessian.py` & `geometric-1.0.1/geometric/tests/test_hessian.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_internal.py` & `geometric-1.0.1/geometric/tests/test_internal.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_minimize.py` & `geometric-1.0.1/geometric/tests/test_minimize.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_molecule.py` & `geometric-1.0.1/geometric/tests/test_molecule.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_nifty.py` & `geometric-1.0.1/geometric/tests/test_nifty.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_openmm.py` & `geometric-1.0.1/geometric/tests/test_openmm.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_params.py` & `geometric-1.0.1/geometric/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_prepare.py` & `geometric-1.0.1/geometric/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_qcengine.py` & `geometric-1.0.1/geometric/tests/test_qcengine.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_rotate.py` & `geometric-1.0.1/geometric/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_run_json.py` & `geometric-1.0.1/geometric/tests/test_run_json.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_terachem.py` & `geometric-1.0.1/geometric/tests/test_terachem.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric/tests/test_transition.py` & `geometric-1.0.1/geometric/tests/test_transition.py`

 * *Files identical despite different names*

### Comparing `geometric-1.0/geometric.egg-info/PKG-INFO` & `geometric-1.0.1/geometric.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: geometric
-Version: 1.0
+Version: 1.0.1
 Summary: Geometry optimization for quantum chemistry
 Home-page: https://github.com/leeping/geomeTRIC
 Author: Lee-Ping Wang, Chenchen Song
-Author-email: leeping@ucdavis.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `geometric-1.0/setup.py` & `geometric-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     long_description = fh.read()
 
 setup(
     name='geometric',
     description='Geometry optimization for quantum chemistry',
     url='https://github.com/leeping/geomeTRIC',
     author='Lee-Ping Wang, Chenchen Song',
-    author_email='leeping@ucdavis.edu',
     packages=find_packages(),
     package_data={'': ['*.ini']},
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={'console_scripts': [
         'geometric-optimize = geometric.optimize:main',
```

### Comparing `geometric-1.0/versioneer.py` & `geometric-1.0.1/versioneer.py`

 * *Files identical despite different names*

