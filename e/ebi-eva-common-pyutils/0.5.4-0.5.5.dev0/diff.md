# Comparing `tmp/ebi_eva_common_pyutils-0.5.4.tar.gz` & `tmp/ebi_eva_common_pyutils-0.5.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebi_eva_common_pyutils-0.5.4.tar", last modified: Mon May 22 22:02:46 2023, max compression
+gzip compressed data, was "ebi_eva_common_pyutils-0.5.5.dev0.tar", last modified: Wed May 31 09:49:36 2023, max compression
```

## Comparing `ebi_eva_common_pyutils-0.5.4.tar` & `ebi_eva_common_pyutils-0.5.5.dev0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1706 2023-05-22 22:00:57.000000 ebi_eva_common_pyutils-0.5.4/CHANGELOG.md
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    11357 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/LICENSE
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       28 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/MANIFEST.in
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      512 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/PKG-INFO
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1434 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/README.md
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.156029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     4984 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/archive_directory.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.156029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/assembly/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       66 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/assembly/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1570 2023-04-28 09:52:41.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/assembly/assembly.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     2151 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/command_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1192 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/common_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     2242 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/config.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     8356 2023-05-07 09:15:50.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/config_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.156029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/contig_alias/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/contig_alias/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     3056 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/contig_alias/contig_alias.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1452 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/ena_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1375 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/file_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     4990 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/logger.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    14953 2023-04-28 09:52:41.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/metadata_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     3589 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/mongo_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.156029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/mongodb/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       72 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/mongodb/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     9676 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/mongodb/mongo_database.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     4859 2023-05-07 09:16:05.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/ncbi_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     2285 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/network_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/nextflow/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      120 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/nextflow/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    10114 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     4398 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/pg_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/reference/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      134 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/reference/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    12162 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/reference/assembly.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     3911 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/reference/sequence.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    14347 2023-05-22 11:31:10.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/spring_properties.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/taxonomy/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/taxonomy/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     2259 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/taxonomy/taxonomy.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/variation/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/variation/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     3515 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/variation/assembly_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     5230 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/variation/contig_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.156029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      512 2023-05-22 22:02:46.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1699 2023-05-22 22:02:46.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        1 2023-05-22 22:02:46.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       81 2023-05-22 22:02:46.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/requires.txt
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       23 2023-05-22 22:02:46.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/top_level.txt
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      225 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/setup.cfg
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      907 2023-05-22 22:00:57.000000 ebi_eva_common_pyutils-0.5.4/setup.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1706 2023-05-31 08:16:27.000000 ebi_eva_common_pyutils-0.5.5.dev0/CHANGELOG.md
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    11357 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/LICENSE
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       28 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/MANIFEST.in
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      545 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/PKG-INFO
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1434 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/README.md
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.011066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4984 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/archive_directory.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/assembly/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       66 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/assembly/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1570 2023-05-31 08:16:27.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/assembly/assembly.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2151 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/command_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1192 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/common_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2242 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/config.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     7960 2023-05-31 08:27:23.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/config_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/contig_alias/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/contig_alias/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3056 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/contig_alias/contig_alias.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1452 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/ena_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1375 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/file_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4990 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/logger.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    14953 2023-05-31 08:16:27.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/metadata_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3573 2023-05-31 08:27:23.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/mongo_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/mongodb/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       72 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/mongodb/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     9676 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/mongodb/mongo_database.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4859 2023-05-31 08:16:27.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/ncbi_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2285 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/network_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/nextflow/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      120 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/nextflow/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    10114 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4398 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/pg_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/reference/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      134 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/reference/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    12162 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/reference/assembly.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3911 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/reference/sequence.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    14666 2023-05-31 09:14:28.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/spring_properties.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/taxonomy/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/taxonomy/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2259 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/taxonomy/taxonomy.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/variation/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/variation/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3515 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/variation/assembly_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     5230 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/variation/contig_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.011066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      545 2023-05-31 09:49:34.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1702 2023-05-31 09:49:34.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        1 2023-05-31 09:49:34.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       81 2023-05-31 09:49:34.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/requires.txt
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       23 2023-05-31 09:49:34.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      225 2023-05-31 09:49:36.019066 ebi_eva_common_pyutils-0.5.5.dev0/setup.cfg
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      911 2023-05-31 09:18:33.000000 ebi_eva_common_pyutils-0.5.5.dev0/setup.py
```

### Comparing `ebi_eva_common_pyutils-0.5.4/CHANGELOG.md` & `ebi_eva_common_pyutils-0.5.5.dev0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/LICENSE` & `ebi_eva_common_pyutils-0.5.5.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/PKG-INFO` & `ebi_eva_common_pyutils-0.5.5.dev0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: ebi_eva_common_pyutils
-Version: 0.5.4
+Version: 0.5.5.dev0
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `ebi_eva_common_pyutils-0.5.4/README.md` & `ebi_eva_common_pyutils-0.5.5.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/archive_directory.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/archive_directory.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/assembly/assembly.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/command_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/common_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/common_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/config.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/config.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/config_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/config_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,28 +46,22 @@
     properties = get_properties_from_xml_file(profile_name, settings_xml_file)
     pg_url = properties['eva.evapro.jdbc.url']
     pg_user = properties['eva.evapro.user']
     pg_pass = properties['eva.evapro.password']
     return pg_url, pg_user, pg_pass
 
 
-def get_primary_mongo_creds_for_profile(profile_name: str, settings_xml_file: str):
+def get_mongo_creds_for_profile(profile_name: str, settings_xml_file: str):
     """
     Gets primary host, username, and password for mongo database.
     Useful for filling properties files, for connection purposes it is preferable to use
     `mongo_utils.get_mongo_connection_handle` as that will handle multiple hosts appropriately.
     """
     properties = get_properties_from_xml_file(profile_name, settings_xml_file)
-    # Use the primary mongo host from configuration:
-    # https://github.com/EBIvariation/configuration/blob/master/eva-maven-settings.xml#L111
-    # TODO: revisit once accessioning/variant pipelines can support multiple hosts
-    try:
-        mongo_host = split_hosts(properties['eva.mongo.host'])[1][0]
-    except IndexError:  # some profiles have only one host
-        mongo_host = split_hosts(properties['eva.mongo.host'])[0][0]
+    mongo_host = properties['eva.mongo.host']
     mongo_user = properties['eva.mongo.user']
     mongo_pass = properties['eva.mongo.passwd']
     return mongo_host, mongo_user, mongo_pass
 
 
 def get_accession_pg_creds_for_profile(profile_name: str, settings_xml_file: str):
     """
```

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/contig_alias/contig_alias.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/contig_alias/contig_alias.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/ena_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/ena_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/file_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/logger.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/logger.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/metadata_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/mongo_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/mongo_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import pymongo
 from urllib.parse import quote_plus
 
 from pymongo import ReadPreference
 
 from ebi_eva_common_pyutils.command_utils import run_command_with_output
 from ebi_eva_common_pyutils.common_utils import merge_two_dicts
-from ebi_eva_common_pyutils.config_utils import get_mongo_uri_for_eva_profile, get_primary_mongo_creds_for_profile
+from ebi_eva_common_pyutils.config_utils import get_mongo_uri_for_eva_profile, get_mongo_creds_for_profile
 
 
 class MongoConfig:
     parameters = None
 
     def __init__(self, **kwargs):
         self.parameters = kwargs
@@ -44,15 +44,15 @@
                                w=write_concern)
 
 
 def get_primary_mongo_connection_handle(profile: str, settings_xml_file: str,
                                         read_concern: str = "majority",
                                         read_preference: ReadPreference = ReadPreference.PRIMARY,
                                         write_concern: str = "majority") -> pymongo.MongoClient:
-    host, username, password = get_primary_mongo_creds_for_profile(profile, settings_xml_file)
+    host, username, password = get_mongo_creds_for_profile(profile, settings_xml_file)
     mongo_connection_uri = "mongodb://{0}:{1}@{2}:{3}/{4}".format(username, quote_plus(password), host,
                                                                   27017, "admin")
     return pymongo.MongoClient(mongo_connection_uri,
                                readConcernLevel=read_concern,
                                read_preference=read_preference,
                                w=write_concern)
```

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/mongodb/mongo_database.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/mongodb/mongo_database.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/ncbi_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/ncbi_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/network_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/network_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/pg_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/pg_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/reference/assembly.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/reference/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/reference/sequence.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/reference/sequence.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/spring_properties.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/spring_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from collections import defaultdict
 
-from ebi_eva_common_pyutils.config_utils import get_primary_mongo_creds_for_profile, \
+from ebi_eva_common_pyutils.config_utils import get_mongo_creds_for_profile, \
     get_accession_pg_creds_for_profile, \
     get_count_service_creds_for_profile, get_properties_from_xml_file, get_variant_load_job_tracker_creds_for_profile
 
 
 class SpringPropertiesGenerator:
     """
     Class to generate Spring properties for various Spring Batch pipelines.
@@ -50,19 +50,21 @@
             return None
         elif not param:
             return ''
         else:
             return string.format(param)
 
     def _mongo_properties(self):
-        mongo_host, mongo_user, mongo_pass = get_primary_mongo_creds_for_profile(
+        mongo_host, mongo_user, mongo_pass = get_mongo_creds_for_profile(
             self.maven_profile, self.private_settings_file)
         return {
             'spring.data.mongodb.host': mongo_host,
-            'spring.data.mongodb.port': 27017,
+            # Don't specify port if hosts already have the port encoded in them
+            # Also see https://github.com/EBIvariation/variation-commons/blob/329d4fa18da73bdad419ca5456b9897c059e33f0/variation-commons-mongodb/src/main/java/uk/ac/ebi/eva/commons/mongodb/utils/MongoClientURIBuilder.java#L44
+            'spring.data.mongodb.port': '' if ':' in mongo_host else 27017,
             'spring.data.mongodb.username': mongo_user,
             'spring.data.mongodb.password': mongo_pass,
             'spring.data.mongodb.authentication-database': 'admin',
         }
 
     def _variant_load_job_tracker_properties(self):
         variant_url, variant_user, variant_pass = get_variant_load_job_tracker_creds_for_profile(self.maven_profile,
```

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/taxonomy/taxonomy.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/taxonomy/taxonomy.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/variation/assembly_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/variation/assembly_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/variation/contig_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/variation/contig_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/PKG-INFO` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: ebi-eva-common-pyutils
-Version: 0.5.4
+Version: 0.5.5.dev0
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/SOURCES.txt` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-/home/nkumar2/PycharmProjects/eva-common-pyutils/ebi_eva_common_pyutils/archive_directory.py
+/data/sundarvenkata_work/EVA3253/eva-common-pyutils/ebi_eva_common_pyutils/archive_directory.py
 ebi_eva_common_pyutils/__init__.py
 ebi_eva_common_pyutils/archive_directory.py
 ebi_eva_common_pyutils/command_utils.py
 ebi_eva_common_pyutils/common_utils.py
 ebi_eva_common_pyutils/config.py
 ebi_eva_common_pyutils/config_utils.py
 ebi_eva_common_pyutils/ena_utils.py
```

### Comparing `ebi_eva_common_pyutils-0.5.4/setup.py` & `ebi_eva_common_pyutils-0.5.5.dev0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages
 
 setup(
     name='ebi_eva_common_pyutils',
     scripts=[os.path.join(os.path.dirname(__file__), 'ebi_eva_common_pyutils', 'archive_directory.py')],
     packages=find_packages(),
-    version='0.5.4',
+    version='0.5.5-dev',
     license='Apache',
     description='EBI EVA - Common Python Utilities',
     url='https://github.com/EBIVariation/eva-common-pyutils',
     keywords=['EBI', 'EVA', 'PYTHON', 'UTILITIES'],
     install_requires=['psycopg2-binary', 'requests', 'pymongo', 'lxml', 'pyyaml', 'cached-property', 'retry',
                       'networkx<=2.5'],
     classifiers=[
```

