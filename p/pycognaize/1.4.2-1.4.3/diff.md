# Comparing `tmp/pycognaize-1.4.2.tar.gz` & `tmp/pycognaize-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycognaize-1.4.2.tar", last modified: Tue May 30 15:47:36 2023, max compression
+gzip compressed data, was "pycognaize-1.4.3.tar", last modified: Wed May 31 13:08:29 2023, max compression
```

## Comparing `pycognaize-1.4.2.tar` & `pycognaize-1.4.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 15:47:36.147830 pycognaize-1.4.2/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    31591 2023-05-30 15:26:02.000000 pycognaize-1.4.2/CHANGELOG.md
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    35137 2022-11-15 12:53:10.000000 pycognaize-1.4.2/LICENSE.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    33359 2023-05-30 15:47:36.147830 pycognaize-1.4.2/PKG-INFO
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1310 2023-02-20 13:34:43.000000 pycognaize-1.4.2/README.md
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 15:47:36.139830 pycognaize-1.4.2/pycognaize/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      361 2023-05-30 15:26:02.000000 pycognaize-1.4.2/pycognaize/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      210 2023-04-28 11:57:35.000000 pycognaize-1.4.2/pycognaize/cli.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2168 2023-01-11 08:15:39.000000 pycognaize-1.4.2/pycognaize/clidriver.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 15:47:36.143830 pycognaize-1.4.2/pycognaize/common/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 12:53:10.000000 pycognaize-1.4.2/pycognaize/common/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      968 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/common/classification_labels.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2359 2023-03-07 12:26:57.000000 pycognaize-1.4.2/pycognaize/common/confidence.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1650 2022-11-15 12:53:10.000000 pycognaize-1.4.2/pycognaize/common/decorators.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5138 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/common/enums.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      394 2022-12-06 11:01:27.000000 pycognaize-1.4.2/pycognaize/common/exceptions.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1750 2022-12-06 11:01:27.000000 pycognaize-1.4.2/pycognaize/common/field_collection.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2352 2022-12-06 11:01:27.000000 pycognaize-1.4.2/pycognaize/common/lazy_dict.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2096 2022-12-06 11:01:27.000000 pycognaize-1.4.2/pycognaize/common/lazy_group_dict.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6826 2023-01-26 10:20:57.000000 pycognaize-1.4.2/pycognaize/common/numeric_parser.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3903 2023-05-04 16:18:45.000000 pycognaize-1.4.2/pycognaize/common/table_utils.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    22777 2023-04-28 14:56:56.000000 pycognaize-1.4.2/pycognaize/common/utils.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      285 2022-11-15 12:53:10.000000 pycognaize-1.4.2/pycognaize/common/white_pixel.jpeg
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 15:47:36.143830 pycognaize-1.4.2/pycognaize/document/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      129 2022-11-15 12:53:10.000000 pycognaize-1.4.2/pycognaize/document/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    23603 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/document/document.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 15:47:36.143830 pycognaize-1.4.2/pycognaize/document/field/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      674 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/document/field/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3367 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/document/field/area_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2818 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/document/field/date_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3200 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/document/field/field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3996 2023-05-30 15:45:37.000000 pycognaize-1.4.2/pycognaize/document/field/link_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3566 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/document/field/numeric_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4238 2023-05-30 15:26:02.000000 pycognaize-1.4.2/pycognaize/document/field/section_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2825 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/document/field/span_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5242 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/document/field/table_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4051 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/document/field/text_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2904 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/document/html_info.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    21421 2023-02-20 13:34:43.000000 pycognaize-1.4.2/pycognaize/document/page.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3349 2023-04-28 14:56:56.000000 pycognaize-1.4.2/pycognaize/document/snapshot.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 15:47:36.147830 pycognaize-1.4.2/pycognaize/document/tag/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      116 2022-11-15 12:53:10.000000 pycognaize-1.4.2/pycognaize/document/tag/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3449 2022-11-15 12:53:10.000000 pycognaize-1.4.2/pycognaize/document/tag/cell.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6090 2023-05-29 14:26:12.000000 pycognaize-1.4.2/pycognaize/document/tag/extraction_tag.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    14209 2023-05-04 16:18:45.000000 pycognaize-1.4.2/pycognaize/document/tag/html_tag.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2657 2023-05-30 10:47:37.000000 pycognaize-1.4.2/pycognaize/document/tag/section_tag.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1794 2022-12-06 11:01:27.000000 pycognaize-1.4.2/pycognaize/document/tag/span_tag.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     8858 2023-01-27 15:01:05.000000 pycognaize-1.4.2/pycognaize/document/tag/table_tag.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    14977 2023-05-29 14:03:01.000000 pycognaize-1.4.2/pycognaize/document/tag/tag.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2863 2022-11-15 12:53:10.000000 pycognaize-1.4.2/pycognaize/index.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3866 2023-05-29 08:03:29.000000 pycognaize-1.4.2/pycognaize/login.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    21992 2023-05-04 16:18:45.000000 pycognaize-1.4.2/pycognaize/model.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 15:47:36.147830 pycognaize-1.4.2/pycognaize/model_registry/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      133 2023-04-28 11:57:35.000000 pycognaize-1.4.2/pycognaize/model_registry/__init__.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 15:47:36.147830 pycognaize-1.4.2/pycognaize/model_registry/db/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2023-04-28 11:57:35.000000 pycognaize-1.4.2/pycognaize/model_registry/db/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      787 2023-04-28 11:57:35.000000 pycognaize-1.4.2/pycognaize/model_registry/db/models.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      598 2023-04-28 11:57:35.000000 pycognaize-1.4.2/pycognaize/model_registry/login.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4687 2023-04-28 11:57:35.000000 pycognaize-1.4.2/pycognaize/model_registry/submit.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 15:47:36.139830 pycognaize-1.4.2/pycognaize.egg-info/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    33359 2023-05-30 15:47:36.000000 pycognaize-1.4.2/pycognaize.egg-info/PKG-INFO
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1852 2023-05-30 15:47:36.000000 pycognaize-1.4.2/pycognaize.egg-info/SOURCES.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        1 2023-05-30 15:47:36.000000 pycognaize-1.4.2/pycognaize.egg-info/dependency_links.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       53 2023-05-30 15:47:36.000000 pycognaize-1.4.2/pycognaize.egg-info/entry_points.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      160 2023-05-30 15:47:36.000000 pycognaize-1.4.2/pycognaize.egg-info/requires.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       11 2023-05-30 15:47:36.000000 pycognaize-1.4.2/pycognaize.egg-info/top_level.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      896 2023-05-30 15:47:36.147830 pycognaize-1.4.2/setup.cfg
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1005 2023-04-28 11:57:35.000000 pycognaize-1.4.2/setup.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.123175 pycognaize-1.4.3/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    31663 2023-05-31 13:07:33.000000 pycognaize-1.4.3/CHANGELOG.md
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    35137 2022-11-15 12:53:10.000000 pycognaize-1.4.3/LICENSE.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    33431 2023-05-31 13:08:29.123175 pycognaize-1.4.3/PKG-INFO
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1310 2023-02-20 13:34:43.000000 pycognaize-1.4.3/README.md
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.119175 pycognaize-1.4.3/pycognaize/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      361 2023-05-31 13:07:33.000000 pycognaize-1.4.3/pycognaize/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      210 2023-04-28 11:57:35.000000 pycognaize-1.4.3/pycognaize/cli.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2168 2023-01-11 08:15:39.000000 pycognaize-1.4.3/pycognaize/clidriver.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.119175 pycognaize-1.4.3/pycognaize/common/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/common/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      968 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/common/classification_labels.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2359 2023-03-07 12:26:57.000000 pycognaize-1.4.3/pycognaize/common/confidence.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1650 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/common/decorators.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5138 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/common/enums.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      394 2022-12-06 11:01:27.000000 pycognaize-1.4.3/pycognaize/common/exceptions.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1750 2022-12-06 11:01:27.000000 pycognaize-1.4.3/pycognaize/common/field_collection.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2352 2022-12-06 11:01:27.000000 pycognaize-1.4.3/pycognaize/common/lazy_dict.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2096 2022-12-06 11:01:27.000000 pycognaize-1.4.3/pycognaize/common/lazy_group_dict.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6826 2023-01-26 10:20:57.000000 pycognaize-1.4.3/pycognaize/common/numeric_parser.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3903 2023-05-04 16:18:45.000000 pycognaize-1.4.3/pycognaize/common/table_utils.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    22777 2023-04-28 14:56:56.000000 pycognaize-1.4.3/pycognaize/common/utils.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      285 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/common/white_pixel.jpeg
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.119175 pycognaize-1.4.3/pycognaize/document/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      129 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/document/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    23788 2023-05-31 09:56:30.000000 pycognaize-1.4.3/pycognaize/document/document.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.123175 pycognaize-1.4.3/pycognaize/document/field/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      674 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3367 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/area_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2818 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/date_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3200 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3996 2023-05-30 15:45:37.000000 pycognaize-1.4.3/pycognaize/document/field/link_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3566 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/numeric_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4437 2023-05-31 13:07:33.000000 pycognaize-1.4.3/pycognaize/document/field/section_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2825 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/span_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5242 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/table_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4051 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/text_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2904 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/html_info.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    21421 2023-02-20 13:34:43.000000 pycognaize-1.4.3/pycognaize/document/page.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3349 2023-04-28 14:56:56.000000 pycognaize-1.4.3/pycognaize/document/snapshot.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.123175 pycognaize-1.4.3/pycognaize/document/tag/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      116 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/document/tag/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3449 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/document/tag/cell.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6090 2023-05-29 14:26:12.000000 pycognaize-1.4.3/pycognaize/document/tag/extraction_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    14209 2023-05-04 16:18:45.000000 pycognaize-1.4.3/pycognaize/document/tag/html_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2657 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/tag/section_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1794 2022-12-06 11:01:27.000000 pycognaize-1.4.3/pycognaize/document/tag/span_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     8858 2023-01-27 15:01:05.000000 pycognaize-1.4.3/pycognaize/document/tag/table_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    14977 2023-05-29 14:03:01.000000 pycognaize-1.4.3/pycognaize/document/tag/tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2863 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/index.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3866 2023-05-29 08:03:29.000000 pycognaize-1.4.3/pycognaize/login.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    21992 2023-05-04 16:18:45.000000 pycognaize-1.4.3/pycognaize/model.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.123175 pycognaize-1.4.3/pycognaize/model_registry/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      133 2023-04-28 11:57:35.000000 pycognaize-1.4.3/pycognaize/model_registry/__init__.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.123175 pycognaize-1.4.3/pycognaize/model_registry/db/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2023-04-28 11:57:35.000000 pycognaize-1.4.3/pycognaize/model_registry/db/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      787 2023-04-28 11:57:35.000000 pycognaize-1.4.3/pycognaize/model_registry/db/models.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      598 2023-04-28 11:57:35.000000 pycognaize-1.4.3/pycognaize/model_registry/login.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4687 2023-04-28 11:57:35.000000 pycognaize-1.4.3/pycognaize/model_registry/submit.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.119175 pycognaize-1.4.3/pycognaize.egg-info/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    33431 2023-05-31 13:08:29.000000 pycognaize-1.4.3/pycognaize.egg-info/PKG-INFO
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1852 2023-05-31 13:08:29.000000 pycognaize-1.4.3/pycognaize.egg-info/SOURCES.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        1 2023-05-31 13:08:29.000000 pycognaize-1.4.3/pycognaize.egg-info/dependency_links.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       53 2023-05-31 13:08:29.000000 pycognaize-1.4.3/pycognaize.egg-info/entry_points.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      160 2023-05-31 13:08:29.000000 pycognaize-1.4.3/pycognaize.egg-info/requires.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       11 2023-05-31 13:08:29.000000 pycognaize-1.4.3/pycognaize.egg-info/top_level.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      896 2023-05-31 13:08:29.123175 pycognaize-1.4.3/setup.cfg
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1005 2023-04-28 11:57:35.000000 pycognaize-1.4.3/setup.py
```

### Comparing `pycognaize-1.4.2/CHANGELOG.md` & `pycognaize-1.4.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Changelog
 
 ## [1.4]
 
+### [1.4.3] - 2023-05-31
+- Fix handling of section field with no tagsc
+
 ### [1.4.2] - 2023-05-30
 - Fix handling of section field value when field does not have tags
 
 ### [1.4.1] - 2023-05-29
 - Add section field and section tag functionality
 
 ### [1.4.0] - 2023-05-25
```

### Comparing `pycognaize-1.4.2/LICENSE.txt` & `pycognaize-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/PKG-INFO` & `pycognaize-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycognaize
-Version: 1.4.2
+Version: 1.4.3
 Home-page: https://github.com/cognaize/pycognaize
 Author: Cognaize
 License: Apache License 2.0
 Project-URL: Source, https://github.com/cognaize/pycognaize
 Project-URL: Reference, https://pycognaize.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/cognaize/pycognaize/blob/master/CHANGELOG.md
 Requires-Python: >= 3.7
@@ -45,14 +45,17 @@
 Have a look at the [quick tutorial](http://pycognaize-docs.com.s3-website.us-east-2.amazonaws.com/tutorials/quick_tutorial.html) 
 for understanding main concepts of the SDK.
 
 # Changelog
 
 ## [1.4]
 
+### [1.4.3] - 2023-05-31
+- Fix handling of section field with no tagsc
+
 ### [1.4.2] - 2023-05-30
 - Fix handling of section field value when field does not have tags
 
 ### [1.4.1] - 2023-05-29
 - Add section field and section tag functionality
 
 ### [1.4.0] - 2023-05-25
```

### Comparing `pycognaize-1.4.2/README.md` & `pycognaize-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/clidriver.py` & `pycognaize-1.4.3/pycognaize/clidriver.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/common/classification_labels.py` & `pycognaize-1.4.3/pycognaize/common/classification_labels.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/common/confidence.py` & `pycognaize-1.4.3/pycognaize/common/confidence.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/common/decorators.py` & `pycognaize-1.4.3/pycognaize/common/decorators.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/common/enums.py` & `pycognaize-1.4.3/pycognaize/common/enums.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/common/field_collection.py` & `pycognaize-1.4.3/pycognaize/common/field_collection.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/common/lazy_dict.py` & `pycognaize-1.4.3/pycognaize/common/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/common/lazy_group_dict.py` & `pycognaize-1.4.3/pycognaize/common/lazy_group_dict.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/common/numeric_parser.py` & `pycognaize-1.4.3/pycognaize/common/numeric_parser.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/common/table_utils.py` & `pycognaize-1.4.3/pycognaize/common/table_utils.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/common/utils.py` & `pycognaize-1.4.3/pycognaize/common/utils.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/document.py` & `pycognaize-1.4.3/pycognaize/document/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -560,7 +560,14 @@
         raise ValueError(f'Wrong opacity value {opacity}')
     color_dict = {"stroke": getColor(color), "fill": getColor(color)}
     annot = page.add_rect_annot(annot_rect)
     annot.set_colors(color_dict)
     annot.set_opacity(opacity)
     annot.update()
     return doc.write()
+
+if __name__ == '__main__':
+    import json
+    with open('/home/atlantx/Downloads/empty_section_hov (1).json') as f:
+        data = json.load(f)
+
+    doc = Document.from_dict(data, '')
```

### Comparing `pycognaize-1.4.2/pycognaize/document/field/__init__.py` & `pycognaize-1.4.3/pycognaize/document/field/__init__.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/field/area_field.py` & `pycognaize-1.4.3/pycognaize/document/field/area_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/field/date_field.py` & `pycognaize-1.4.3/pycognaize/document/field/date_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/field/field.py` & `pycognaize-1.4.3/pycognaize/document/field/field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/field/link_field.py` & `pycognaize-1.4.3/pycognaize/document/field/link_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/field/numeric_field.py` & `pycognaize-1.4.3/pycognaize/document/field/numeric_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/field/section_field.py` & `pycognaize-1.4.3/pycognaize/document/field/section_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from typing import List, Optional, Dict, Type
 
+import bson
 
 from pycognaize.common.enums import (
     IqDocumentKeysEnum,
     ID, START, END,
     IqFieldKeyEnum, IqDataTypesEnum,
 )
 from pycognaize.document.html_info import HTML
@@ -68,17 +69,18 @@
                                 pages=pages,
                                 tag_type=tag_type))
                 except Exception as e:
                     logging.debug(f"Failed creating tag"
                                   f" for field {raw[ID]}: {e}")
 
         return cls(name=raw[IqDocumentKeysEnum.name.value],
-                   value=section_dict[0].get([IqFieldKeyEnum.value.value], ''),
-                   ocr_value=section_dict[0].get(
-                       [IqFieldKeyEnum.ocr_value.value], ''),
+                   value=section_dict[0][
+                       IqFieldKeyEnum.value.value] if section_dict else '',
+                   ocr_value=section_dict[0][
+                       IqFieldKeyEnum.ocr_value.value] if section_dict else '',
                    tags=tags,
                    field_id=str(raw[ID]),
                    group_key=raw.get(IqFieldKeyEnum.group_key.value, ''),
                    group_name=raw.get(IqFieldKeyEnum.group.value, '')
                    )
 
     def to_dict(self) -> dict:
@@ -87,25 +89,26 @@
         field_dict[IqFieldKeyEnum.name.value] = self.name
         field_dict[ID] = self.field_id
         field_dict[IqFieldKeyEnum.group_key.value] = self._group_key
         field_dict[IqFieldKeyEnum.group.value] = self._group_name
         field_dict[IqFieldKeyEnum.value.value] = ''
         field_dict[IqFieldKeyEnum.data_type.value] =\
             IqDataTypesEnum.section.value
-        field_dict[IqFieldKeyEnum.tags.value] = [
-            {
-                ID: self._field_id,
+        field_dict[IqFieldKeyEnum.tags.value] = []
+        if self.start is not None and self.end is not None:
+            tag_data = {
+                ID: str(bson.ObjectId()),
                 IqFieldKeyEnum.value.value: self._value,
                 IqFieldKeyEnum.ocr_value.value: self._ocr_value,
                 IqFieldKeyEnum.section.value: {
                     START: self.start.to_dict(),
                     END: self.end.to_dict()
                 }
             }
-        ]
+            field_dict[IqFieldKeyEnum.tags.value].append(tag_data)
         return field_dict
 
     def __repr__(self):
         return f"<{self.__class__.__name__}: {self.name}>"
 
     def __str__(self):
         return f"<{self.__class__.__name__}: {self.name}>"
```

### Comparing `pycognaize-1.4.2/pycognaize/document/field/span_field.py` & `pycognaize-1.4.3/pycognaize/document/field/span_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/field/table_field.py` & `pycognaize-1.4.3/pycognaize/document/field/table_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/field/text_field.py` & `pycognaize-1.4.3/pycognaize/document/field/text_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/html_info.py` & `pycognaize-1.4.3/pycognaize/document/html_info.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/page.py` & `pycognaize-1.4.3/pycognaize/document/page.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/snapshot.py` & `pycognaize-1.4.3/pycognaize/document/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/tag/cell.py` & `pycognaize-1.4.3/pycognaize/document/tag/cell.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/tag/extraction_tag.py` & `pycognaize-1.4.3/pycognaize/document/tag/extraction_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/tag/html_tag.py` & `pycognaize-1.4.3/pycognaize/document/tag/html_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/tag/section_tag.py` & `pycognaize-1.4.3/pycognaize/document/tag/section_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/tag/span_tag.py` & `pycognaize-1.4.3/pycognaize/document/tag/span_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/tag/table_tag.py` & `pycognaize-1.4.3/pycognaize/document/tag/table_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/document/tag/tag.py` & `pycognaize-1.4.3/pycognaize/document/tag/tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/index.py` & `pycognaize-1.4.3/pycognaize/index.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/login.py` & `pycognaize-1.4.3/pycognaize/login.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/model.py` & `pycognaize-1.4.3/pycognaize/model.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/model_registry/db/models.py` & `pycognaize-1.4.3/pycognaize/model_registry/db/models.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/model_registry/login.py` & `pycognaize-1.4.3/pycognaize/model_registry/login.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize/model_registry/submit.py` & `pycognaize-1.4.3/pycognaize/model_registry/submit.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/pycognaize.egg-info/PKG-INFO` & `pycognaize-1.4.3/pycognaize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycognaize
-Version: 1.4.2
+Version: 1.4.3
 Home-page: https://github.com/cognaize/pycognaize
 Author: Cognaize
 License: Apache License 2.0
 Project-URL: Source, https://github.com/cognaize/pycognaize
 Project-URL: Reference, https://pycognaize.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/cognaize/pycognaize/blob/master/CHANGELOG.md
 Requires-Python: >= 3.7
@@ -45,14 +45,17 @@
 Have a look at the [quick tutorial](http://pycognaize-docs.com.s3-website.us-east-2.amazonaws.com/tutorials/quick_tutorial.html) 
 for understanding main concepts of the SDK.
 
 # Changelog
 
 ## [1.4]
 
+### [1.4.3] - 2023-05-31
+- Fix handling of section field with no tagsc
+
 ### [1.4.2] - 2023-05-30
 - Fix handling of section field value when field does not have tags
 
 ### [1.4.1] - 2023-05-29
 - Add section field and section tag functionality
 
 ### [1.4.0] - 2023-05-25
```

### Comparing `pycognaize-1.4.2/pycognaize.egg-info/SOURCES.txt` & `pycognaize-1.4.3/pycognaize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/setup.cfg` & `pycognaize-1.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.2/setup.py` & `pycognaize-1.4.3/setup.py`

 * *Files identical despite different names*

