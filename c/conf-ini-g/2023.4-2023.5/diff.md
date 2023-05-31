# Comparing `tmp/conf-ini-g-2023.4.tar.gz` & `tmp/conf-ini-g-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf-ini-g-2023.4.tar", last modified: Wed Mar 15 15:21:06 2023, max compression
+gzip compressed data, was "conf-ini-g-2023.5.tar", last modified: Wed May 31 14:48:54 2023, max compression
```

## Comparing `conf-ini-g-2023.4.tar` & `conf-ini-g-2023.5.tar`

### file list

```diff
@@ -1,74 +1,94 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.392511 conf-ini-g-2023.4/
--rw-r--r--   0 eric      (1000) users      (984)      114 2023-03-01 07:58:57.000000 conf-ini-g-2023.4/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4428 2023-03-15 15:21:06.392511 conf-ini-g-2023.4/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2023-03-01 08:10:10.000000 conf-ini-g-2023.4/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 conf-ini-g-2023.4/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     3536 2023-03-01 09:58:27.000000 conf-ini-g-2023.4/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.379177 conf-ini-g-2023.4/conf_ini_g/
--rw-r--r--   0 eric      (1000) users      (984)     1763 2023-03-01 08:07:08.000000 conf-ini-g-2023.4/conf_ini_g/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.382511 conf-ini-g-2023.4/conf_ini_g/activated/
--rw-r--r--   0 eric      (1000) users      (984)     8349 2023-03-14 14:17:12.000000 conf-ini-g-2023.4/conf_ini_g/activated/config.py
--rw-r--r--   0 eric      (1000) users      (984)     5609 2023-03-14 14:17:12.000000 conf-ini-g-2023.4/conf_ini_g/activated/parameter.py
--rw-r--r--   0 eric      (1000) users      (984)     2502 2021-08-24 16:59:54.000000 conf-ini-g-2023.4/conf_ini_g/activated/section.py
--rw-r--r--   0 eric      (1000) users      (984)     2851 2023-03-14 14:17:11.000000 conf-ini-g-2023.4/conf_ini_g/activated/unit.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.379177 conf-ini-g-2023.4/conf_ini_g/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.382511 conf-ini-g-2023.4/conf_ini_g/interface/console/
--rw-r--r--   0 eric      (1000) users      (984)     1635 2021-09-01 08:16:01.000000 conf-ini-g-2023.4/conf_ini_g/interface/console/__init__.py
--rw-r--r--   0 eric      (1000) users      (984)     7440 2023-03-14 14:17:12.000000 conf-ini-g-2023.4/conf_ini_g/interface/console/config.py
--rw-r--r--   0 eric      (1000) users      (984)     1973 2021-08-27 09:24:20.000000 conf-ini-g-2023.4/conf_ini_g/interface/console/generic.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.382511 conf-ini-g-2023.4/conf_ini_g/interface/screen/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.385844 conf-ini-g-2023.4/conf_ini_g/interface/screen/component/
--rw-r--r--   0 eric      (1000) users      (984)     3865 2023-03-14 14:11:35.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/component/boolean.py
--rw-r--r--   0 eric      (1000) users      (984)     3255 2023-03-14 14:11:35.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/component/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     2590 2023-03-14 14:04:17.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/component/default_entry.py
--rw-r--r--   0 eric      (1000) users      (984)     9372 2023-03-14 14:17:12.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/component/file_dialogs.py
--rw-r--r--   0 eric      (1000) users      (984)     2226 2023-03-14 14:18:06.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/component/none.py
--rw-r--r--   0 eric      (1000) users      (984)     5441 2023-03-14 14:11:35.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/component/path.py
--rw-r--r--   0 eric      (1000) users      (984)     7613 2023-03-14 14:17:11.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/component/sequence.py
--rw-r--r--   0 eric      (1000) users      (984)     2651 2021-08-25 09:24:23.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/component/type_options.py
--rw-r--r--   0 eric      (1000) users      (984)    13447 2023-03-14 14:17:11.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/config.py
--rw-r--r--   0 eric      (1000) users      (984)     1860 2021-08-20 12:13:27.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/generic.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.385844 conf-ini-g-2023.4/conf_ini_g/interface/screen/library/
--rw-r--r--   0 eric      (1000) users      (984)     2397 2021-08-21 09:44:03.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/library/pyqt5_constant.py
--rw-r--r--   0 eric      (1000) users      (984)     4577 2023-03-14 14:17:11.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/library/pyqt5_generic.py
--rw-r--r--   0 eric      (1000) users      (984)     3748 2021-08-27 13:15:41.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/library/pyqt5_parameter.py
--rw-r--r--   0 eric      (1000) users      (984)     7923 2023-03-14 14:17:11.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/parameter.py
--rw-r--r--   0 eric      (1000) users      (984)     7429 2023-03-14 14:17:11.000000 conf-ini-g-2023.4/conf_ini_g/interface/screen/section.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.385844 conf-ini-g-2023.4/conf_ini_g/interface/storage/
--rw-r--r--   0 eric      (1000) users      (984)     7653 2023-03-14 14:13:40.000000 conf-ini-g-2023.4/conf_ini_g/interface/storage/config.py
--rw-r--r--   0 eric      (1000) users      (984)     1577 2021-08-24 08:04:39.000000 conf-ini-g-2023.4/conf_ini_g/interface/storage/constant.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.385844 conf-ini-g-2023.4/conf_ini_g/light/
--rw-r--r--   0 eric      (1000) users      (984)     4750 2023-03-14 12:49:00.000000 conf-ini-g-2023.4/conf_ini_g/light/config.py
--rw-r--r--   0 eric      (1000) users      (984)     3857 2023-03-14 13:50:00.000000 conf-ini-g-2023.4/conf_ini_g/light/conversion.py
--rw-r--r--   0 eric      (1000) users      (984)     2590 2023-03-14 13:01:19.000000 conf-ini-g-2023.4/conf_ini_g/light/ini.py
--rw-r--r--   0 eric      (1000) users      (984)     2167 2023-03-14 12:44:12.000000 conf-ini-g-2023.4/conf_ini_g/light/xlsx.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.385844 conf-ini-g-2023.4/conf_ini_g/raw/
--rw-r--r--   0 eric      (1000) users      (984)     3249 2023-03-14 14:17:12.000000 conf-ini-g-2023.4/conf_ini_g/raw/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.389177 conf-ini-g-2023.4/conf_ini_g/specification/
--rw-r--r--   0 eric      (1000) users      (984)     6876 2023-03-14 14:17:12.000000 conf-ini-g-2023.4/conf_ini_g/specification/config.py
--rw-r--r--   0 eric      (1000) users      (984)     1922 2021-08-19 16:55:15.000000 conf-ini-g-2023.4/conf_ini_g/specification/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     9964 2023-03-14 14:17:12.000000 conf-ini-g-2023.4/conf_ini_g/specification/constrained_type.py
--rw-r--r--   0 eric      (1000) users      (984)    12368 2023-03-14 14:17:12.000000 conf-ini-g-2023.4/conf_ini_g/specification/constraint.py
--rw-r--r--   0 eric      (1000) users      (984)     4020 2023-03-14 14:08:15.000000 conf-ini-g-2023.4/conf_ini_g/specification/default.py
--rw-r--r--   0 eric      (1000) users      (984)     2949 2023-03-14 14:17:11.000000 conf-ini-g-2023.4/conf_ini_g/specification/generic.py
--rw-r--r--   0 eric      (1000) users      (984)     6488 2023-03-14 14:14:35.000000 conf-ini-g-2023.4/conf_ini_g/specification/parameter.py
--rw-r--r--   0 eric      (1000) users      (984)     8300 2023-03-14 14:17:12.000000 conf-ini-g-2023.4/conf_ini_g/specification/section.py
--rw-r--r--   0 eric      (1000) users      (984)     2865 2021-08-20 16:45:01.000000 conf-ini-g-2023.4/conf_ini_g/specification/unit.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.392511 conf-ini-g-2023.4/conf_ini_g/standard/
--rw-r--r--   0 eric      (1000) users      (984)     2475 2021-08-20 17:36:42.000000 conf-ini-g-2023.4/conf_ini_g/standard/dtcl_extension.py
--rw-r--r--   0 eric      (1000) users      (984)     3492 2023-03-14 14:14:35.000000 conf-ini-g-2023.4/conf_ini_g/standard/path_extension.py
--rw-r--r--   0 eric      (1000) users      (984)     5946 2023-03-14 14:17:11.000000 conf-ini-g-2023.4/conf_ini_g/standard/str_extension.py
--rw-r--r--   0 eric      (1000) users      (984)     6388 2023-03-14 14:01:22.000000 conf-ini-g-2023.4/conf_ini_g/standard/type_extension.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-03-14 11:56:54.000000 conf-ini-g-2023.4/conf_ini_g/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.379177 conf-ini-g-2023.4/conf_ini_g.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4428 2023-03-15 15:21:06.000000 conf-ini-g-2023.4/conf_ini_g.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     2016 2023-03-15 15:21:06.000000 conf-ini-g-2023.4/conf_ini_g.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-03-15 15:21:06.000000 conf-ini-g-2023.4/conf_ini_g.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       24 2023-03-15 15:21:06.000000 conf-ini-g-2023.4/conf_ini_g.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       11 2023-03-15 15:21:06.000000 conf-ini-g-2023.4/conf_ini_g.egg-info/top_level.txt
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.379177 conf-ini-g-2023.4/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:21:06.392511 conf-ini-g-2023.4/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1982 2023-03-01 10:23:59.000000 conf-ini-g-2023.4/documentation/wiki/description.asciidoc
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 conf-ini-g-2023.4/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-03-15 15:21:06.392511 conf-ini-g-2023.4/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5713 2023-03-14 14:21:05.000000 conf-ini-g-2023.4/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/
+-rw-r--r--   0 eric      (1000) users      (984)      114 2023-03-01 07:58:57.000000 conf-ini-g-2023.5/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4428 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      636 2023-03-01 08:10:10.000000 conf-ini-g-2023.5/README-COPYRIGHT-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 conf-ini-g-2023.5/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     3536 2023-03-01 09:58:27.000000 conf-ini-g-2023.5/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/
+-rw-r--r--   0 eric      (1000) users      (984)     1779 2023-05-12 13:37:01.000000 conf-ini-g-2023.5/conf_ini_g/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/catalog/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/
+-rw-r--r--   0 eric      (1000) users      (984)     2483 2023-05-31 14:28:04.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py
+-rw-r--r--   0 eric      (1000) users      (984)     2534 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/
+-rw-r--r--   0 eric      (1000) users      (984)     1763 2023-05-31 13:56:41.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py
+-rw-r--r--   0 eric      (1000) users      (984)     2118 2023-05-31 13:46:25.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py
+-rw-r--r--   0 eric      (1000) users      (984)     1824 2023-05-31 14:27:49.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     2060 2023-05-31 13:36:33.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py
+-rw-r--r--   0 eric      (1000) users      (984)     1997 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py
+-rw-r--r--   0 eric      (1000) users      (984)     1701 2023-05-31 13:48:26.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     3935 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/boolean.py
+-rw-r--r--   0 eric      (1000) users      (984)     3176 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/choices.py
+-rw-r--r--   0 eric      (1000) users      (984)     2223 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/none.py
+-rw-r--r--   0 eric      (1000) users      (984)     5499 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     7690 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/sequence.py
+-rw-r--r--   0 eric      (1000) users      (984)     2592 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/text.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/catalog/specification/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     2376 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/boolean.py
+-rw-r--r--   0 eric      (1000) users      (984)     2632 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/choices.py
+-rw-r--r--   0 eric      (1000) users      (984)     5180 2023-05-31 14:28:32.000000 conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/number.py
+-rw-r--r--   0 eric      (1000) users      (984)     2534 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     4699 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/sequence.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/instance/
+-rw-r--r--   0 eric      (1000) users      (984)    10398 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/instance/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/instance/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     3374 2023-05-31 14:25:44.000000 conf-ini-g-2023.5/conf_ini_g/instance/parameter/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     5255 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/instance/parameter/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     4773 2023-05-31 14:25:44.000000 conf-ini-g-2023.5/conf_ini_g/instance/parameter/unit.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/interface/console/
+-rw-r--r--   0 eric      (1000) users      (984)     1635 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/interface/console/__init__.py
+-rw-r--r--   0 eric      (1000) users      (984)     6532 2023-05-31 14:28:56.000000 conf-ini-g-2023.5/conf_ini_g/interface/console/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/interface/screen/
+-rw-r--r--   0 eric      (1000) users      (984)    14161 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/interface/screen/config.py
+-rw-r--r--   0 eric      (1000) users      (984)     1945 2023-05-12 12:16:07.000000 conf-ini-g-2023.5/conf_ini_g/interface/screen/generic.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     7467 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     9467 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/path_chooser.py
+-rw-r--r--   0 eric      (1000) users      (984)     2586 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/type_selector.py
+-rw-r--r--   0 eric      (1000) users      (984)     8380 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/interface/screen/section.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/interface/storage/
+-rw-r--r--   0 eric      (1000) users      (984)     6838 2023-05-31 14:29:29.000000 conf-ini-g-2023.5/conf_ini_g/interface/storage/config.py
+-rw-r--r--   0 eric      (1000) users      (984)     1577 2023-05-10 13:30:33.000000 conf-ini-g-2023.5/conf_ini_g/interface/storage/constant.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/light/
+-rw-r--r--   0 eric      (1000) users      (984)     4236 2023-05-31 14:29:35.000000 conf-ini-g-2023.5/conf_ini_g/light/config.py
+-rw-r--r--   0 eric      (1000) users      (984)     3773 2023-05-26 18:53:12.000000 conf-ini-g-2023.5/conf_ini_g/light/conversion.py
+-rw-r--r--   0 eric      (1000) users      (984)     2605 2023-05-31 14:29:41.000000 conf-ini-g-2023.5/conf_ini_g/light/ini.py
+-rw-r--r--   0 eric      (1000) users      (984)     2080 2023-05-26 18:29:02.000000 conf-ini-g-2023.5/conf_ini_g/light/xlsx.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/raw/
+-rw-r--r--   0 eric      (1000) users      (984)     4535 2023-05-31 14:29:46.000000 conf-ini-g-2023.5/conf_ini_g/raw/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/conf_ini_g/specification/
+-rw-r--r--   0 eric      (1000) users      (984)     2821 2023-05-31 14:30:19.000000 conf-ini-g-2023.5/conf_ini_g/specification/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     7977 2023-05-31 12:39:36.000000 conf-ini-g-2023.5/conf_ini_g/specification/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/conf_ini_g/specification/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     3179 2023-05-31 14:29:52.000000 conf-ini-g-2023.5/conf_ini_g/specification/parameter/annotation.py
+-rw-r--r--   0 eric      (1000) users      (984)     4427 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/specification/parameter/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     9497 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/specification/parameter/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     3612 2023-05-31 14:30:01.000000 conf-ini-g-2023.5/conf_ini_g/specification/parameter/unit.py
+-rw-r--r--   0 eric      (1000) users      (984)     2232 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/specification/parameter/value.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/conf_ini_g/specification/section/
+-rw-r--r--   0 eric      (1000) users      (984)     9610 2023-05-31 14:30:13.000000 conf-ini-g-2023.5/conf_ini_g/specification/section/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     1809 2023-05-12 12:45:21.000000 conf-ini-g-2023.5/conf_ini_g/specification/section/unit.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/conf_ini_g/standard/
+-rw-r--r--   0 eric      (1000) users      (984)     3079 2023-05-31 14:30:24.000000 conf-ini-g-2023.5/conf_ini_g/standard/path_extension.py
+-rw-r--r--   0 eric      (1000) users      (984)     3112 2023-05-26 13:22:35.000000 conf-ini-g-2023.5/conf_ini_g/standard/py_extension.py
+-rw-r--r--   0 eric      (1000) users      (984)     7544 2023-05-31 14:32:50.000000 conf-ini-g-2023.5/conf_ini_g/standard/str_extension.py
+-rw-r--r--   0 eric      (1000) users      (984)     3798 2023-05-31 14:30:34.000000 conf-ini-g-2023.5/conf_ini_g/standard/type_extension.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-05-31 14:34:20.000000 conf-ini-g-2023.5/conf_ini_g/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4428 2023-05-31 14:48:54.000000 conf-ini-g-2023.5/conf_ini_g.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     2714 2023-05-31 14:48:54.000000 conf-ini-g-2023.5/conf_ini_g.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-05-31 14:48:54.000000 conf-ini-g-2023.5/conf_ini_g.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       20 2023-05-31 14:48:54.000000 conf-ini-g-2023.5/conf_ini_g.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       11 2023-05-31 14:48:54.000000 conf-ini-g-2023.5/conf_ini_g.egg-info/top_level.txt
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1982 2023-03-01 10:23:59.000000 conf-ini-g-2023.5/documentation/wiki/description.asciidoc
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 conf-ini-g-2023.5/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     6251 2023-05-31 14:48:37.000000 conf-ini-g-2023.5/setup.py
```

### Comparing `conf-ini-g-2023.4/PKG-INFO` & `conf-ini-g-2023.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-ini-g
-Version: 2023.4
+Version: 2023.5
 Summary: App Configuration in INI format with Automatic Command-Line Parser and Graphical Interface Generation
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
```

### Comparing `conf-ini-g-2023.4/README-COPYRIGHT-utf8.txt` & `conf-ini-g-2023.5/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.4/README-LICENCE-utf8.txt` & `conf-ini-g-2023.5/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.4/README.rst` & `conf-ini-g-2023.5/README.rst`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.4/conf_ini_g/__init__.py` & `conf-ini-g-2023.5/conf_ini_g/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from conf_ini_g.specification.config import config_t
-from conf_ini_g.specification.parameter import parameter_t
-from conf_ini_g.specification.section import section_t
+# from conf_ini_g.specification.config import config_t
+# from conf_ini_g.specification.parameter.main import parameter_t
+# from conf_ini_g.specification.section.main import section_t
 
 from conf_ini_g.version import __version__
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/activated/config.py` & `conf-ini-g-2023.5/conf_ini_g/specification/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,205 +27,179 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
+import dataclasses as dtcl
+import textwrap as text
 from typing import Sequence
 
-import conf_ini_g.activated.unit as unia
-import conf_ini_g.specification.unit as unis
-from conf_ini_g.activated.parameter import actual_t
-from conf_ini_g.activated.section import AddUnknownParameter
-from conf_ini_g.interface.console.config import TransferArgumentsToINIConfig
-from conf_ini_g.interface.storage.constant import INI_COMMENT_MARKER
-from conf_ini_g.raw.config import ini_config_h, raw_config_h
-from conf_ini_g.specification.config import config_t
-from conf_ini_g.specification.constant import UNIT_SECTION
-from conf_ini_g.specification.section import section_t
-
-
-STD_UNIT_CONVERSIONS = unis.STD_UNIT_CONVERSIONS
-
-
-def ActivateFromINIConfig(
-    config: config_t,
-    ini_config: ini_config_h,
-    /,
-    *,
-    arguments: raw_config_h = None,
-) -> tuple[Sequence[str] | None, Sequence[tuple[str, str]]]:
-    """"""
-    if arguments is not None:
-        TransferArgumentsToINIConfig(arguments, ini_config, config)
-
-    issues, for_deferred_check = _SetFromINIConfig(config, ini_config)
-    _SetControllerValues(config)
-    _AddDefaults(config)
-
-    issues.extend(_Issues(config))
-    if issues.__len__() == 0:
-        issues = None
-
-    return issues, for_deferred_check
-
-
-def ControllerSectionAndUid(section: section_t, config: config_t) -> tuple[str, int]:
-    """"""
-    controller = section.controller
-    parameter = config[controller.section][controller.parameter]
-
-    return controller.section, parameter.actual.uid
-
-
-def RawConfigWithConsumedUnits(
-    config: config_t, /
-) -> tuple[raw_config_h, Sequence[str] | None]:
-    """"""
-    raw_config = {}
-    issues = []
-
-    if UNIT_SECTION in config:
-        unit_conversions = {
-            _prm.name: _prm.actual.value for _prm in config[UNIT_SECTION]
-        }
-    else:
-        unit_conversions = {}
-    unit_conversions.update(STD_UNIT_CONVERSIONS)
-
-    for section in config:
-        section_as_dict = {}
-
-        for parameter in section.active_parameters:
-            actual = parameter.actual
-            value = actual.value
-            unit = actual.unit
-
-            if unit is None:
-                converted_value = value
-            else:
-                conversion_factor = unit_conversions[unit]
-                if isinstance(value, Sequence):
-                    converted_value = []
-                    success = True
-                    for element in value:
-                        if isinstance(element, (int, float)):
-                            converted_value.append(conversion_factor * element)
-                        else:
-                            success = False
-                            issues.append(
-                                f"{value}: Value of parameter {parameter.name} does not support unit conversion"
-                            )
-                            break
-                    if success:
-                        converted_value = tuple(converted_value)
-                    else:
-                        converted_value = value
-                elif isinstance(value, (int, float)):
-                    converted_value = conversion_factor * value
-                else:
-                    converted_value = value
-                    issues.append(
-                        f"{value}: Value of parameter {parameter.name} does not support unit conversion"
-                    )
-
-            section_as_dict[parameter.name] = converted_value
+from rich import print as rprint
+from rich.text import Text as text_t
 
-        raw_config[section.name] = section_as_dict
-
-    if issues.__len__() == 0:
-        issues = None
+from conf_ini_g.catalog.specification.parameter.choices import choices_t
+from conf_ini_g.specification.parameter.type import type_options_t
+from conf_ini_g.specification.parameter.unit import UNIT_SEPARATOR
+from conf_ini_g.specification.section.main import section_t
+from conf_ini_g.specification.section.unit import UNIT_SECTION
+from conf_ini_g.standard.py_extension import SpecificationPath
+from conf_ini_g.standard.type_extension import TypeAsRichStr
+
+
+@dtcl.dataclass(init=False, repr=False, eq=False)
+class config_t(list[section_t]):
+    spec_path: str = None
+
+    def __init__(self, sections: Sequence[section_t], /) -> None:
+        """
+        Raising exceptions is adapted here since execution cannot proceed without a
+        valid specification.
+        """
+        list.__init__(self, sections)
+        self._SetControllerChoices()  # After __init__ so that self iterator is usable
+        self.spec_path = SpecificationPath(sections)
+
+        issues = self.Issues()
+        if issues.__len__() > 0:
+            rprint(
+                self.spec_path,
+                "[red]Invalid specification[/]",
+                "\n".join(issues),
+                sep="\n",
+            )
+            raise ValueError
 
-    return raw_config, issues
+    def _SetControllerChoices(self) -> None:
+        """"""
+        for section in self:
+            if (controller := section.controller) is None:
+                continue
+
+            controlling_parameter = self[controller.section][controller.parameter]
+            if controlling_parameter.types is not None:
+                raise TypeError(
+                    f"{controller.section}.{controller.parameter}: "
+                    f"Controller parameter must only have a name specified."
+                )
 
+            controlling_parameter.types = type_options_t.NewFromTypes(
+                (choices_t.NewAnnotatedType(section.controlling_values),)
+            )
 
-def _SetFromINIConfig(
-    config: config_t, ini_config: ini_config_h, /
-) -> tuple[list[str], Sequence[tuple[str, str]]]:
-    """"""
-    output = []
-    for_deferred_check = []
-
-    for section_name, parameters in ini_config.items():
-        if section_name in config:
-            section = config[section_name]
-            if unis.IsUnitSection(section_name):
-                unia.AddUnitsToSection(section, parameters)
-
-            for name, value in parameters.items():
-                if name in section:
-                    actual = actual_t.NewFromINIEntry(
-                        value,
-                        INI_COMMENT_MARKER,
-                        section[name].type_options,
-                    )
-                    section[name].actual = actual
-                elif section.accept_unknown_parameters:
-                    AddUnknownParameter(section, name, value)
-                    for_deferred_check.append((section_name, name))
-                else:
+    def AddUnitSection(self) -> None:
+        """"""
+        section = section_t(
+            name=UNIT_SECTION,
+            definition="Unit definitions",
+            description=f"Units can be used in any other section "
+            f"to specify a parameter value as follows: "
+            f"numerical_value{UNIT_SEPARATOR}unit, e.g., 1.5'mm.",
+            basic=True,
+            optional=True,
+            category=UNIT_SECTION,
+            is_growable=True,
+        )
+        self.append(section)
+
+    @property
+    def section_names(self) -> Sequence[str]:
+        """"""
+        return tuple(_sct.name for _sct in self)
+
+    def Issues(self) -> list[str]:
+        """"""
+        output = []
+
+        if self.__len__() == 0:
+            output.append("spec_path: Empty specification")
+            return output
+
+        names = self.section_names
+        if names.__len__() > set(names).__len__():
+            output.append("Specification with repeated section names")
+
+        for section in self:
+            if not isinstance(section, section_t):
+                output.append(
+                    f"{type(section).__name__}: Invalid section type; Expected={section_t.__name__}."
+                )
+                continue
+
+            output.extend(section.Issues())
+            if section.controller is not None:
+                if section.controller.section not in self:
                     output.append(
-                        f"{section_name}.{name}: Attempt to add an unknown parameter to a section accepting none"
+                        f"{section.controller.section}: "
+                        f'Unspecified section declared as controller of section "{section.name}"'
                     )
-        elif unis.IsUnitSection(section_name, possibly_fuzzy=True):
-            output.append(
-                f'{section_name}: Unit section must respect the following case "{UNIT_SECTION}"'
-            )
-        else:
-            output.append(
-                f"{section_name}: Invalid section; Expected={config.valid_section_names}"
-            )
-
-    return output, for_deferred_check
+                else:
+                    controller_section = self[section.controller.section]
+                    if controller_section.controller is not None:
+                        output.append(
+                            f"{section.controller.section}: "
+                            f'Section controlling "{section.name}" is itself controlled'
+                        )
+                    if section.controller.parameter not in controller_section:
+                        output.append(
+                            f"{section.controller.section}.{section.controller.parameter}: "
+                            f'Unspecified parameter declared as controller of section "{section.name}"'
+                        )
+                    else:
+                        controller_parameter = controller_section[
+                            section.controller.parameter
+                        ]
+                        if controller_parameter.optional:
+                            output.append(
+                                f"{section.controller.section}.{section.controller.parameter}: "
+                                f'Optional parameter declared as controller of section "{section.name}"'
+                            )
+                        if (controller_parameter.types is not None) and (
+                            controller_parameter.types.__len__() > 1
+                        ):
+                            output.append(
+                                f"{section.controller.section}.{section.controller.parameter}: "
+                                f'Multi-type parameter declared as controller of section "{section.name}"'
+                            )
 
+        return output
 
-def _SetControllerValues(config: config_t) -> None:
-    """"""
-    for section in config:
-        if (controller := section.controller) is not None:
-            stc_name, prm_name = controller.section, controller.parameter
-            section.controller_value = config[stc_name][prm_name].actual.value
-
-
-def _AddDefaults(config: config_t, /) -> None:
-    #
-    has_default_value = []
-
-    for section in config:
-        for parameter in section.all_parameters:
-            if parameter.optional and (parameter.actual is None):
-                actual = actual_t.NewWithDefaultValue(parameter)
-                parameter.actual = actual
-                has_default_value.append(actual.uid)
-
-    config.has_default_value = tuple(has_default_value)
-
-
-def _Issues(config: config_t, /) -> Sequence[str]:
-    """"""
-    output = []
-
-    valid_units = list(STD_UNIT_CONVERSIONS.keys())
-    if UNIT_SECTION in config:
-        valid_units.extend(_unt.name for _unt in config[UNIT_SECTION])
-
-    for section in config:
-        section_name = section.name
-
-        if unis.IsUnitSection(section_name):
-            issues = unia.Issues(section)
-        else:
-            issues = []
-            for parameter in section:
-                if (actual := parameter.actual) is not None:
-                    issues.extend(actual.Issues(parameter.name, section_name))
-                    if ((unit := actual.unit) is not None) and (
-                        unit not in valid_units
-                    ):
-                        issues.append(
-                            f"{unit}: Invalid unit of parameter {section_name}.{parameter.name}"
-                        )
+    def _Item(self, key: str | int, /) -> section_t | None:
+        """"""
+        if isinstance(key, int):
+            return list.__getitem__(self, key)
+
+        for section in self:
+            if section.name == key:
+                return section
+
+        return None
+
+    def __contains__(self, key: str, /) -> bool:
+        """"""
+        return self._Item(key) is not None
+
+    def __getitem__(self, key: str | int, /) -> section_t:
+        """"""
+        item = self._Item(key)
+        if item is None:
+            raise KeyError(f"{key}: Not a section of config.")
+
+        return item
+
+    def __str__(self) -> str:
+        """"""
+        return text_t.from_markup(self.__rich__()).plain
+
+    def __rich__(self) -> str:
+        """"""
+        output = [
+            TypeAsRichStr(self),
+            f"    [blue]spec_path[/]={self.spec_path}"
+            f"[yellow]:{type(self.spec_path).__name__}[/]",
+        ]
 
-        output.extend(issues)
+        for section in self:
+            output.append(text.indent(section.__rich__(), "    "))
 
-    return output
+        return "\n".join(output)
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/activated/parameter.py` & `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/path.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,155 +27,134 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
-import dataclasses as dtcl
-from typing import Any, Sequence
+from typing import Callable
 
-from conf_ini_g.specification.constant import UNIT_SEPARATOR
-from conf_ini_g.specification.constrained_type import (
-    INVALID_VALUE,
-    constrained_type_t,
-    constrained_types_t,
+import conf_ini_g.interface.screen.parameter.path_chooser as fd_
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.button import button_wgt_t
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import (
+    hbox_lyt_t,
+    library_wgt_t,
 )
-from conf_ini_g.specification.default import missing_required_value_t
-from conf_ini_g.specification.parameter import parameter_t
-from conf_ini_g.standard.dtcl_extension import AsStr
-
-
-@dtcl.dataclass(repr=False, eq=False)
-class actual_t:
-
-    uid: int = None
-    type: constrained_type_t = None
-    value: Any = None
-    unit: str = None
-    comment: str = None
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.text import text_wgt_t
+from conf_ini_g.catalog.specification.parameter.path import path_t
+from conf_ini_g.specification.parameter.main import parameter_t
+from conf_ini_g.specification.parameter.type import type_t
+from conf_ini_g.specification.parameter.value import (
+    MISSING_REQUIRED_VALUE,
+    missing_required_value_t,
+)
+from conf_ini_g.standard.path_extension import path_t as pl_path_t
 
-    @classmethod
-    def _New(cls) -> actual_t:
-        """"""
-        instance = cls()
-        instance.uid = id(instance)
 
-        return instance
+class path_wgt_t(library_wgt_t):
+    __slots__ = (
+        "target_type",
+        "path",
+        "SelectedFile",
+    )
+    target_type: path_t.TARGET_TYPE
+    path: text_wgt_t
+    SelectedFile: Callable[..., pl_path_t | None]
+
+    def __init__(self, parent: library_wgt_t = None) -> None:
+        """"""
+        super().__init__(parent=parent)
+
+        # Do not use self.__class__.__slots__ because it will be the parent slots in case of inheritance
+        for slot in path_wgt_t.__slots__:
+            setattr(self, slot, None)
 
     @classmethod
-    def NewWithDefaultValue(
+    def NewWithDetails(
         cls,
-        parameter: parameter_t,
-    ) -> actual_t:
-        """"""
-        instance = cls._New()
-        instance._SetDefaultTypesAndValue(parameter)
+        value: pl_path_t | None | missing_required_value_t,
+        value_type: type_t,
+        _: parameter_t,
+    ) -> path_wgt_t:
+        """
+        If value_type does not contain the necessary details, the target type is set to any and considered as input, and
+        the selection button label ends with an exclamation point.
+        """
+        output = cls()
 
-        return instance
+        if (value is None) or (value is MISSING_REQUIRED_VALUE):
+            value = ""
+        else:
+            value = str(value)
 
-    @classmethod
-    def NewForProgrammaticEntry(
-        cls,
-        value: str,
-        type_options: constrained_types_t,
-    ) -> actual_t:
-        """"""
-        instance = cls._New()
-        instance.SetTypesAndValueFromString(value, type_options)
+        annotation = value_type.FirstAnnotationWithAttribute(
+            ("target_type", "is_input")
+        )
+        if annotation is None:
+            target_type = path_t.TARGET_TYPE.any
+            is_input = True
+            misses_details = True
+        else:
+            target_type = annotation.target_type
+            is_input = annotation.is_input
+            misses_details = False
+
+        output.target_type = target_type
+        if is_input:
+            output.SelectedFile = fd_.SelectedInputFile
+        else:
+            output.SelectedFile = fd_.SelectedOutputFile
 
-        return instance
+        selector_label = "..."
+        if misses_details:
+            selector_label += "!"
+        path = text_wgt_t(value, parent=output)
+        path_selector = button_wgt_t(selector_label, parent=output)
+        path_selector.SetFunction(output.SelectDocument)
 
-    @classmethod
-    def NewFromINIEntry(
-        cls,
-        value_w_comment: str,
-        comment_marker: str,
-        type_options: constrained_types_t,
-    ) -> actual_t:
-        """"""
-        value, comment = _SplittedValueAndComment(value_w_comment, comment_marker)
+        output.path = path
 
-        instance = cls.NewForProgrammaticEntry(value, type_options)
-        instance.comment = comment
+        path_selector.setFixedWidth(30)
 
-        return instance
+        layout = hbox_lyt_t()
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.addWidget(path)
+        layout.addWidget(path_selector)
+        output.setLayout(layout)
 
-    def _SetDefaultTypesAndValue(self, parameter: parameter_t, /) -> None:
-        """"""
-        value = parameter.default
-        if isinstance(value, missing_required_value_t):
-            att_type = value.main_type
-        else:
-            att_type = parameter.type_options.MatchingTypeOf(type(value))
+        return output
 
-        # TODO: give the meaning of "att"
-        self.type = att_type
-        self.value = value
-
-    def SetTypesAndValueFromString(
-        self, value_w_unit: Any, type_options: constrained_types_t, /
-    ) -> None:
+    def Text(self) -> str:
         """"""
-        if isinstance(value_w_unit, str):
-            value_as_str, unit = _SplittedValueAndUnit(value_w_unit)
-        else:
-            value_as_str, unit = value_w_unit, None
-        value, att_type = type_options.TypedValue(value_as_str)
-
-        self.type = att_type
-        self.value = value
-        self.unit = unit
+        return self.path.Text()
 
-    def Issues(self, name: str, section: str, /) -> Sequence[str]:
+    def Value(self) -> pl_path_t | None:
         """"""
-        if self.value is INVALID_VALUE:
-            return (
-                f"{section}/{name}: No matching type in specification or invalid value",
-            )
+        text = self.Text()
+        if text.__len__() > 0:
+            return pl_path_t(text)
 
-        return ()
+        return None
 
-    def __str__(self) -> str:
+    def SelectDocument(self) -> None:
         """"""
-        output = AsStr(self)
-        intro_length = output.find(":") + 2
-
-        return output[intro_length:]
+        current_path = self.Text()
+        current_doc = pl_path_t(current_path).resolve()
 
+        if self.target_type is path_t.TARGET_TYPE.document:
+            title = "Select File"
+        elif self.target_type is path_t.TARGET_TYPE.folder:
+            title = "Select Folder"
+        else:
+            title = "Select File or Folder"
 
-def _SplittedValueAndComment(
-    value_w_comment: str,
-    comment_marker: str,
-    /,
-) -> tuple[str, str| None]:
-    """"""
-    value, comment = _SplittedElements(value_w_comment, comment_marker)
-    if (comment is not None) and (comment.__len__() == 0):
-        comment = None
-
-    return value, comment
-
-
-def _SplittedValueAndUnit(value_w_unit: str, /) -> tuple[str, str | None]:
-    """"""
-    # if unit.__len__() == 0, do not make it None so that an invalid unit error is noticed later on
-    return _SplittedElements(value_w_unit, UNIT_SEPARATOR, from_left=False)
-
-
-def _SplittedElements(
-    combined: str, separator: str, /, *, from_left: bool = True
-) -> tuple[str, str | None]:
-    """"""
-    if from_left:
-        where_separator = combined.find(separator)
-    else:
-        where_separator = combined.rfind(separator)
-
-    if where_separator != -1:
-        left = combined[:where_separator].strip()
-        right = combined[(where_separator + 1) :].strip()
-    else:
-        left = combined
-        right = None
+        selection = self.SelectedFile(
+            title,
+            title,
+            mode=self.target_type,
+            start_folder=current_doc.parent,
+            initial_selection=current_doc,
+        )
+        if selection is None:
+            return
 
-    return left, right
+        self.path.setText(str(selection))
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/activated/section.py` & `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,31 +25,26 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from conf_ini_g.activated.parameter import actual_t
-from conf_ini_g.specification.parameter import parameter_t
-from conf_ini_g.specification.section import section_t
-from conf_ini_g.standard.type_extension import UNIVERSAL_ANNOTATED_TYPES
-
-
-def AddUnknownParameter(section: section_t, name: str, value: str, /) -> None:
-    """
-    Cannot be a method of specification.section.section_t since a value is set
-    """
-    parameter = parameter_t(
-        name=name,
-        definition="On-the-fly parameter",
-        description="This parameter is not part of the specification. "
-        "It was added programmatically because it was found in the INI document or "
-        "passed as a command-line argument",
-        basic=section.basic,
-        types=UNIVERSAL_ANNOTATED_TYPES,
-        default=None,
-    )
-    actual = actual_t.NewForProgrammaticEntry(value, parameter.type_options)
-    parameter.actual = actual
+import PyQt5.QtWidgets as wdgt
 
-    section.AddParameter(parameter)
+
+class path_chooser_wgt_t(wdgt.QFileDialog):
+    """"""
+
+    def __init__(self, caption: str, /, *, extension_filter: str = None):
+        """"""
+        if extension_filter is None:
+            extension_filter = "Any files (*)"
+        super().__init__(caption=caption, filter=extension_filter)
+
+    def SelectedFile(self) -> str:
+        """"""
+        return self.selectedFiles()[0]
+
+    def RunAndGetClosingStatus(self) -> int:
+        """"""
+        return self.exec_()
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/activated/unit.py` & `conf-ini-g-2023.5/conf_ini_g/standard/py_extension.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,47 +25,50 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Sequence
+import ast as bstr
+import inspect as nspt
+import sys as sstm
 
-from conf_ini_g.specification.constant import UNIT_SECTION
-from conf_ini_g.specification.parameter import parameter_t
-from conf_ini_g.specification.section import section_t
-from conf_ini_g.specification.unit import STD_UNIT_CONVERSIONS
+from conf_ini_g.standard.path_extension import path_t
 
 
-def AddUnitsToSection(section: section_t, units: dict[str, str], /) -> None:
+def SpecificationPath(element: object, /, *, relative_to_home: bool = True) -> str:
     """"""
-    for unit, value in units.items():
-        unit_spec = parameter_t(
-            name=unit,
-            definition="",
-            description="",
-            basic=True,
-            types=(int, float),
-            default=1,
-        )
-        section.AddParameter(unit_spec)
-
-
-def Issues(units: section_t, /) -> Sequence[str]:
-    """"""
-    output = []
-
-    standard_units = tuple(STD_UNIT_CONVERSIONS.keys())
-    for unit in units:
-        if unit.name in standard_units:
-            if unit.actual.value == STD_UNIT_CONVERSIONS[unit.name][-1]:
-                message = "Unit already available among standard units; Please remove unit from INI"
-            else:
-                message = (
-                    "Redefinition of a standard unit; Please use another unit name"
-                )
-            output.append(f"{UNIT_SECTION}/{unit.name}: {message}")
-
-        output.extend(unit.Issues(section=UNIT_SECTION))
+    found = []
+    for module in sstm.modules.copy().values():
+        for attribute in dir(module):
+            value = getattr(module, attribute)
+            if value is element:
+                code = nspt.getsource(module)
+                tree = bstr.parse(code)
+                is_imported = False
+                for node in bstr.walk(tree):
+                    if isinstance(node, bstr.ImportFrom):
+                        for alias in node.names:
+                            if (
+                                (alias.asname is None) and (alias.name == attribute)
+                            ) or (
+                                (alias.asname is not None)
+                                and (alias.asname == attribute)
+                            ):
+                                is_imported = True
+                                break
+                if not is_imported:
+                    path = module.__file__
+                    if relative_to_home:
+                        path = str(path_t(path).relative_to(path_t.home()))
+                    found.append(path)
+
+    if (n_found := found.__len__()) == 0:
+        output = "Unidentified specification file"
+    elif n_found == 1:
+        output = found[0]
+    else:
+        alternatives = ", ".join(found)
+        output = f"Alternatives: {alternatives}"
 
     return output
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/console/__init__.py` & `conf-ini-g-2023.5/conf_ini_g/interface/console/__init__.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/console/config.py` & `conf-ini-g-2023.5/conf_ini_g/interface/console/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,72 +29,72 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import re as rgex
 from argparse import ArgumentParser as argument_parser_t
 from typing import Any, Iterator, Sequence
 
-import colorama as clrm
-
-from conf_ini_g.interface.console.generic import DisplayErrorAndQuit
-from conf_ini_g.raw.config import ini_config_h, raw_config_h
+from conf_ini_g.raw.config import raw_config_h
 from conf_ini_g.specification.config import config_t
-from conf_ini_g.specification.default import missing_required_value_t
+from conf_ini_g.specification.parameter.value import MISSING_REQUIRED_VALUE
+from conf_ini_g.standard.path_extension import path_t
 from conf_ini_g.standard.str_extension import Flattened
 
 
 parsed_arguments_h = dict[str, str]
 
 
 # Specified INI document file is stored in INI_DOCUMENT_VARIABLE
-INI_DOCUMENT_VARIABLE = "ini_document"
+INI_DOCUMENT_VARIABLE = "ini_path"
 
 ADVANCED_MODE_OPTION = "advanced-mode"
 ADVANCED_MODE_VARIABLE = "advanced_mode"
 
 # Usage: {section_name}{SECTION_PARAMETER_SEPARATOR}{parameter_name}
 SECTION_PARAMETER_SEPARATOR = "-"
 
 
 def CommandLineParser(
     description: str | None, specification: config_t, /
 ) -> argument_parser_t:
     """"""
     output = argument_parser_t(description=description, allow_abbrev=False)
+    # TODO: Why is this argument optional?
     output.add_argument(
         dest=INI_DOCUMENT_VARIABLE,
         help="Path to INI configuration file",
         default=None,
         nargs="?",
         metavar="INI_config_file",
     )
 
     for section in specification:
         for parameter in section.all_parameters:
             option = f"{section.name}{SECTION_PARAMETER_SEPARATOR}{parameter.name}"
             if option == ADVANCED_MODE_OPTION:
                 # Raising an exception is adapted here since execution has been launched from command line
-                DisplayErrorAndQuit(
-                    f"{option}: Configuration section and parameter colliding with advanced mode option"
+                raise ValueError(
+                    f"{option}: Command-line option for parameter is identical to advanced mode option. "
+                    f"Please change parameter specification (section name and/or parameter name)."
                 )
 
             attribute = f"{section.name}{SECTION_PARAMETER_SEPARATOR}{parameter.name}"
 
-            # Default is a missing_required_value_t instance to avoid overwriting if in INI but not passed
-            type_options = parameter.type_options
-            default = missing_required_value_t.NewFromConstrainedType(type_options)
+            # Default is a missing_required_value_t instance to avoid overwriting if in
+            # INI but not passed.
+            default = MISSING_REQUIRED_VALUE
 
             if parameter.optional:
                 if isinstance(parameter.default, str):
                     delimiter = '"'
                 else:
                     delimiter = ""
                 types_and_value = (
-                    f"Options: {type_options}. "
-                    f"Default: {clrm.Fore.GREEN}{delimiter}{parameter.default}{delimiter}{clrm.Fore.RESET}"
+                    f"Options: {parameter.types}. "
+                    f"Default: [green]{delimiter}{parameter.default}{delimiter}[/]"
                 )
             else:
                 types_and_value = str(default)
             flattened = Flattened(types_and_value)
             definition = f"{parameter.definition}. {flattened}"
 
             # Type could be PythonTypeOfAnnotated(cmd_line_type). However, to allow passing any of the allowed types,
@@ -115,77 +115,55 @@
     )
 
     return output
 
 
 def ParsedArguments(
     parser: argument_parser_t, /, *, arguments: Sequence[str] = None
-) -> tuple[str | None, bool, raw_config_h]:
+) -> tuple[path_t | None, bool, raw_config_h]:
     """"""
     parsed, unknowns = parser.parse_known_args(args=arguments)
     parsed = vars(parsed)
 
     advanced_mode = parsed[ADVANCED_MODE_VARIABLE]
     del parsed[ADVANCED_MODE_VARIABLE]
 
-    ini_document = parsed[INI_DOCUMENT_VARIABLE]
+    ini_path = parsed[INI_DOCUMENT_VARIABLE]
     del parsed[INI_DOCUMENT_VARIABLE]
+    if ini_path is not None:
+        ini_path = path_t(ini_path).resolve(strict=True)
 
     pattern = rgex.compile(
         r"--(\w+)" + SECTION_PARAMETER_SEPARATOR + r"(\w+)=(.+)", flags=rgex.ASCII
     )
     for unknown in unknowns:
         match = pattern.fullmatch(unknown)
         if match is None:
             # Raising an exception is adapted here since execution has been launched from command line
-            DisplayErrorAndQuit(
+            raise ValueError(
                 f"{unknown}: Invalid option syntax; Expected=--SECTION-PARAMETER=VALUE"
             )
 
         section, parameter, value = match.groups()
         parsed[f"{section}{SECTION_PARAMETER_SEPARATOR}{parameter}"] = value
 
-    parsed_as_ini = {}
+    raw_config = {}
     for sct_name, prm_name, value in _SectionParameterValueIterator(parsed):
-        if sct_name in parsed_as_ini:
-            parsed_as_ini[sct_name][prm_name] = value
+        if sct_name in raw_config:
+            raw_config[sct_name][prm_name] = value
         else:
-            parsed_as_ini[sct_name] = {prm_name: value}
-
-    return ini_document, advanced_mode, parsed_as_ini
+            raw_config[sct_name] = {prm_name: value}
 
-
-def TransferArgumentsToINIConfig(
-    arguments: raw_config_h, config: ini_config_h, specification: config_t
-) -> None:
-    """
-    Raising an exception is adapted here since execution has been launched from command line
-    """
-    for sct_name, parameters in arguments.items():
-        if sct_name not in specification:
-            DisplayErrorAndQuit(
-                f"{sct_name}: Invalid section; Expected={specification.valid_section_names}"
-            )
-        section = specification[sct_name]
-
-        for prm_name, value in parameters.items():
-            if (prm_name in section) or section.accept_unknown_parameters:
-                if sct_name not in config:
-                    config[sct_name] = {}
-                config[sct_name][prm_name] = value
-            else:
-                DisplayErrorAndQuit(
-                    f"{sct_name}.{prm_name}: Attempt to add an unknown parameter to a section accepting none"
-                )
+    return ini_path, advanced_mode, raw_config
 
 
 def _SectionParameterValueIterator(
     arguments: parsed_arguments_h,
 ) -> Iterator[tuple[str, str, Any]]:
     """"""
     for prm_uid, value in arguments.items():
         # See CommandLineParser for why this can happen
-        if isinstance(value, missing_required_value_t):
+        if value is MISSING_REQUIRED_VALUE:
             continue
 
         section, parameter = prm_uid.split(SECTION_PARAMETER_SEPARATOR)
         yield section, parameter, value
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/console/generic.py` & `conf-ini-g-2023.5/conf_ini_g/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,26 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import sys as sstm
-
-import colorama as clrm
-
-
-def DisplayErrorAndQuit(error: str) -> None:
-    """"""
-    separator = error.find(":")
-    if separator == -1:
-        error = clrm.Fore.RED + error + clrm.Fore.RESET
-    else:
-        error = (
-            error[: (separator + 1)]
-            + clrm.Fore.RED
-            + error[(separator + 1) :]
-            + clrm.Fore.RESET
-        )
-    print(error)
-    sstm.exit(-1)
+__version__ = "2023.5"
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/component/boolean.py` & `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/boolean.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,71 +27,81 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
-from conf_ini_g.interface.screen.library.pyqt5_generic import hbox_lyt_t, library_wgt_t
-from conf_ini_g.interface.screen.library.pyqt5_parameter import choices_dots_wgt_t
-from conf_ini_g.specification.constrained_type import constrained_type_t
-from conf_ini_g.specification.default import missing_required_value_t
-from conf_ini_g.specification.parameter import parameter_t
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.choices import (
+    choices_dots_wgt_t,
+)
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import (
+    hbox_lyt_t,
+    library_wgt_t,
+)
+from conf_ini_g.specification.parameter.main import parameter_t
+from conf_ini_g.specification.parameter.type import type_t
+from conf_ini_g.specification.parameter.value import (
+    MISSING_REQUIRED_VALUE,
+    missing_required_value_t,
+)
 
 
 class boolean_wgt_t(library_wgt_t):
-
     __slots__ = ("true_btn",)
     true_btn: choices_dots_wgt_t
 
     def __init__(self, parent: library_wgt_t = None) -> None:
         """"""
         super().__init__(parent=parent)
+
         # Do not use self.__class__.__slots__ because it will be the parent slots in case of inheritance
         for slot in boolean_wgt_t.__slots__:
             setattr(self, slot, None)
 
     @classmethod
     def NewWithDetails(
         cls,
         value: bool | None | missing_required_value_t,
-        att_type: constrained_type_t,
+        value_type: type_t,
         _: parameter_t | None,
     ) -> boolean_wgt_t:
         """
-        If att_type does not contain the necessary details, an exclamation point is added to the default values.
+        If value_type does not contain the necessary details, an exclamation point is added to the default values.
         """
-        instance = cls()
+        output = cls()
 
-        # TODO: can be None: see interface.screen.parameter.NewForParameter. But can it be missing_required_value_t?
-        #     If yes, comment how.
-        if (value is None) or isinstance(value, missing_required_value_t):
+        # TODO: Can be None (see interface.screen.parameter.NewForParameter). But can it
+        #     really be missing_required_value_t? If yes, comment how.
+        if (value is None) or (value is MISSING_REQUIRED_VALUE):
             value = True
 
-        annotation = att_type.FirstConstraintWithAttribute("mode")
+        annotation = value_type.FirstAnnotationWithAttribute("mode")
         if annotation is None:
-            labels = ("True!", "False!")
+            labels = None
         else:
             labels = getattr(annotation.mode, "value", None)
-            if labels is None:
-                labels = ("True!", "False!")
+        if labels is None:
+            labels = ("True!", "False!")
 
-        true_btn = choices_dots_wgt_t(labels[0], parent=instance)
-        false_btn = choices_dots_wgt_t(labels[1], parent=instance)
-        true_btn.SetChecked(value)
-        false_btn.SetChecked(not value)
+        true_btn = choices_dots_wgt_t(labels[0], parent=output)
+        false_btn = choices_dots_wgt_t(labels[1], parent=output)
+        true_btn.setChecked(value)
+        false_btn.setChecked(not value)
 
-        instance.true_btn = true_btn
+        output.true_btn = true_btn
 
         layout = hbox_lyt_t()
-        layout.SetContentsMargins(0, 0, 0, 0)
+        layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(true_btn)
         layout.addWidget(false_btn)
-        instance.setLayout(layout)
+        output.setLayout(layout)
 
-        return instance
+        return output
 
     def Text(self) -> str:
+        """"""
         return str(self.Value())
 
     def Value(self) -> bool:
+        """"""
         return self.true_btn.isChecked()
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/component/choices.py` & `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/choices.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,60 +27,58 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
-from conf_ini_g.interface.screen.library.pyqt5_parameter import choices_list_wgt_t
-from conf_ini_g.specification.constrained_type import constrained_type_t
-from conf_ini_g.specification.default import missing_required_value_t
-from conf_ini_g.specification.parameter import parameter_t
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.choices import (
+    choices_list_wgt_t,
+)
+from conf_ini_g.specification.parameter.main import parameter_t
+from conf_ini_g.specification.parameter.type import type_t
+from conf_ini_g.specification.parameter.value import missing_required_value_t
 
 
 class choices_wgt_t(choices_list_wgt_t):
     """"""
 
     @classmethod
     def NewWithDetails(
         cls,
         value: str | None | missing_required_value_t,
-        att_type: constrained_type_t,
+        value_type: type_t,
         _: parameter_t | None,
     ) -> choices_wgt_t:
         """
-        If att_type does not contain the necessary details, the initial value (if valid) is the only choice, or a unique
+        If value_type does not contain the necessary details, the initial value (if valid) is the only choice, or a unique
         default choice ending with an exclamation point is added.
         """
-        instance = cls()
+        output = cls()
 
-        value_is_invalid = (value is None) or isinstance(
-            value, missing_required_value_t
-        )
+        value_is_valid = isinstance(value, str)
+        if value_is_valid:
+            value = value.strip()
 
-        annotation = att_type.FirstConstraintWithAttribute("options")
+        annotation = value_type.FirstAnnotationWithAttribute("options")
         if annotation is None:
-            if value_is_invalid:
-                choices = ("Default!",)
-            else:
+            if value_is_valid:
                 choices = (value,)
+            else:
+                choices = ("Default!",)
         else:
             choices = annotation.options
 
         for choice in choices:
-            instance.AddItem(choice)
-        if value_is_invalid:
-            instance.SetCurrentIndex(0)
+            output.addItem(choice)
+        if value_is_valid:
+            output.setCurrentText(value)
         else:
-            instance.SetCurrentText(value)
-
-        return instance
+            output.setCurrentIndex(0)
 
-    def Text(self) -> str:
-        """"""
-        return self.CurrentText()
+        return output
 
     def Value(self) -> str:
         """
         Cannot be done using: class.Value = class.Text since the Text method is added to instances, not to the class
         """
         return self.Text()
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/component/default_entry.py` & `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/text.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,39 +29,42 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 from typing import Any
 
-from conf_ini_g.interface.screen.library.pyqt5_parameter import simple_entry_wgt_t
-from conf_ini_g.specification.constrained_type import constrained_type_t
-from conf_ini_g.specification.default import missing_required_value_t
-from conf_ini_g.specification.parameter import parameter_t
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.text import text_wgt_t
+from conf_ini_g.specification.parameter.main import parameter_t
+from conf_ini_g.specification.parameter.type import type_t
+from conf_ini_g.specification.parameter.value import (
+    MISSING_REQUIRED_VALUE,
+    missing_required_value_t,
+)
 
 
-class default_entry_wgt_t(simple_entry_wgt_t):
+class default_entry_wgt_t(text_wgt_t):
     """"""
 
     @classmethod
     def NewWithDetails(
         cls,
         value: Any | None | missing_required_value_t,
-        _: constrained_type_t,
+        _: type_t,
         __: parameter_t,
     ) -> default_entry_wgt_t:
         """"""
-        instance = cls()
+        output = cls()
 
-        if (value is None) or isinstance(value, missing_required_value_t):
+        if (value is None) or (value is MISSING_REQUIRED_VALUE):
             value = ""
         else:
             value = str(value)
-        instance.SetText(value)
+        output.setText(value)
 
-        return instance
+        return output
 
     def Value(self) -> str:
         """
         Cannot be done using: class.Value = class.Text since the Text method is added to instances, not to the class
         """
         return self.Text()
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/component/file_dialogs.py` & `conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/path_chooser.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,33 +27,34 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from typing import Sequence
 
-from conf_ini_g.interface.screen.library.pyqt5_constant import (
+from conf_ini_g.catalog.interface.screen.library.pyqt5.constant import (
     DIALOG_ACCEPT_OPEN,
     DIALOG_ACCEPT_SAVE,
     DIALOG_ACCEPTATION,
     DIALOG_AUTO_OVERWRITE,
     DIALOG_MODE_ANY,
     DIALOG_MODE_EXISTING_FILE,
     DIALOG_MODE_FOLDER,
 )
-from conf_ini_g.interface.screen.library.pyqt5_generic import (
+from conf_ini_g.catalog.interface.screen.library.pyqt5.main import (
     ShowErrorMessage,
-    file_selection_wgt_t,
-    widget_event_loop_t,
+    event_loop_t,
 )
-from conf_ini_g.specification.constraint import path_t
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.path_chooser import (
+    path_chooser_wgt_t,
+)
+from conf_ini_g.catalog.specification.parameter.path import path_t
 from conf_ini_g.standard.path_extension import any_path_h
 from conf_ini_g.standard.path_extension import path_t as pl_path_t
 
-
 """
 valid_types: {"Type": "extension", "Type": ("extension", "extension",...), ...}
 filter: "Image files (*.png *.xpm *.jpg);Text files (*.txt);Any files (*)"
 """
 
 
 valid_types_t = dict[str, str | Sequence[str]]
@@ -75,25 +76,26 @@
     extension_filter, _ = _AllowedTypesElements(valid_types)
     check_existence = False
     if mode is path_t.TARGET_TYPE.document:
         dialog_mode = DIALOG_MODE_EXISTING_FILE
     elif mode is path_t.TARGET_TYPE.folder:
         dialog_mode = DIALOG_MODE_FOLDER
     else:
-        # TODO: check if that allows to select a folder (documentation says "The name of a file, whether it exists or
-        #     not."), so a priori, no. But then how can we allow selection of either a file or a folder?
+        # TODO: Check if that allows to select a folder (documentation says "The name of
+        #     a file, whether it exists or not."). So a priori, no. But then how can we
+        #     allow selection of either a file or a folder?
         dialog_mode = DIALOG_MODE_ANY
         check_existence = True
 
     while True:
         dialog = _GenericFileDialog(
             title, caption, extension_filter, start_folder, initial_selection
         )
-        dialog.SetAcceptMode(DIALOG_ACCEPT_OPEN)
-        dialog.SetFileMode(dialog_mode)
+        dialog.setAcceptMode(DIALOG_ACCEPT_OPEN)
+        dialog.setFileMode(dialog_mode)
 
         output = _SelectedFile(dialog)
         if output is None:
             return None
         if check_existence and not output.exists():
             ShowErrorMessage(f"{output}: Nonexistent file or folder")
             start_folder = _StartFolderFromFolder(output)
@@ -121,18 +123,18 @@
     _EnsureAQAppIsRunning()
 
     extension_filter, allowed_extensions = _AllowedTypesElements(valid_types)
     while True:
         dialog = _GenericFileDialog(
             title, caption, extension_filter, start_folder, initial_selection
         )
-        dialog.SetAcceptMode(DIALOG_ACCEPT_SAVE)
-        dialog.SetFileMode(DIALOG_MODE_ANY)
+        dialog.setAcceptMode(DIALOG_ACCEPT_SAVE)
+        dialog.setFileMode(DIALOG_MODE_ANY)
         if auto_overwrite:
-            dialog.SetOption(DIALOG_AUTO_OVERWRITE)
+            dialog.setOption(DIALOG_AUTO_OVERWRITE)
 
         output = _SelectedFile(dialog)
         if output is None:
             return None
         # The file dialog does not allow to select either a file or a folder. So the solution here is to select a file,
         # and if a folder was needed, take the parent. See (*) below.
         if (mode is path_t.TARGET_TYPE.folder) and output.exists() and output.is_file():
@@ -176,16 +178,16 @@
 #         return overwriting_dialog.exec_() == qw_.QMessageBox.Save
 #
 #     return True
 
 
 def _EnsureAQAppIsRunning() -> None:
     #
-    if widget_event_loop_t.GetInstance() is None:
-        _ = widget_event_loop_t([])  # Empty sys.argv
+    if event_loop_t.GetInstance() is None:
+        _ = event_loop_t([])  # Empty sys.argv
         # Initially, there was a tuple argument: (f"Launched-From-{__name__}",).
         # But PySide2 complains about not being of type typing.Sequence[str].
 
 
 def _AllowedTypesElements(
     valid_types: valid_types_t | None,
 ) -> tuple[str, tuple[str]]:
@@ -227,28 +229,28 @@
 
 def _GenericFileDialog(
     title: str,
     caption: str,
     extension_filter: str,
     start_folder: any_path_h,
     initial_selection: any_path_h,
-) -> file_selection_wgt_t:
+) -> path_chooser_wgt_t:
     #
     # noinspection PyArgumentList
-    output = file_selection_wgt_t(caption, extension_filter=extension_filter)
-    output.SetWindowTitle(title)
+    output = path_chooser_wgt_t(caption, extension_filter=extension_filter)
+    output.setWindowTitle(title)
     if start_folder is not None:
-        output.SetDirectory(str(start_folder))
+        output.setDirectory(str(start_folder))
     if initial_selection is not None:
-        output.SelectFile(str(initial_selection))
+        output.selectFile(str(initial_selection))
 
     return output
 
 
-def _SelectedFile(dialog: file_selection_wgt_t) -> pl_path_t | None:
+def _SelectedFile(dialog: path_chooser_wgt_t) -> pl_path_t | None:
     #
     status = dialog.RunAndGetClosingStatus()
     if status == DIALOG_ACCEPTATION:
         return pl_path_t(dialog.SelectedFile())
 
     return None
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/component/none.py` & `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/none.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,28 +29,28 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 from typing import Any
 
-from conf_ini_g.interface.screen.library.pyqt5_parameter import label_wgt_t
-from conf_ini_g.specification.constrained_type import constrained_type_t
-from conf_ini_g.specification.default import missing_required_value_t
-from conf_ini_g.specification.parameter import parameter_t
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import label_wgt_t
+from conf_ini_g.specification.parameter.main import parameter_t
+from conf_ini_g.specification.parameter.type import type_t
+from conf_ini_g.specification.parameter.value import missing_required_value_t
 
 
 class none_wgt_t(label_wgt_t):
     """"""
 
     @classmethod
     def NewWithDetails(
         cls,
         _: Any | None | missing_required_value_t,
-        __: constrained_type_t,
+        __: type_t,
         ___: parameter_t,
     ) -> label_wgt_t:
         """"""
         return cls("None")
 
     def Value(self) -> None:
         """"""
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/component/sequence.py` & `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/sequence.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,60 +29,66 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 from typing import ClassVar, Sequence
 
-from conf_ini_g.interface.screen.library.pyqt5_generic import hbox_lyt_t, library_wgt_t
-from conf_ini_g.interface.screen.library.pyqt5_parameter import (
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.choices import (
     choices_list_wgt_t,
-    simple_entry_wgt_t,
 )
-from conf_ini_g.specification.constrained_type import constrained_type_t
-from conf_ini_g.specification.constraint import sequence_t
-from conf_ini_g.specification.default import missing_required_value_t
-from conf_ini_g.specification.parameter import parameter_t
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import (
+    hbox_lyt_t,
+    library_wgt_t,
+)
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.text import text_wgt_t
+from conf_ini_g.catalog.specification.parameter.sequence import sequence_t
+from conf_ini_g.specification.parameter.main import parameter_t
+from conf_ini_g.specification.parameter.type import type_t
+from conf_ini_g.specification.parameter.value import (
+    MISSING_REQUIRED_VALUE,
+    missing_required_value_t,
+)
 
 
 class sequence_wgt_t(library_wgt_t):
-
     ENTRY_ANY: ClassVar[str] = "any"
     ENTRIES: ClassVar[tuple[str, ...]] = ("2", "3", "4", "5", "6", ENTRY_ANY)
 
     __slots__ = ("length_selector", "components")
     length_selector: choices_list_wgt_t
-    components: tuple[simple_entry_wgt_t, ...]
+    components: tuple[text_wgt_t, ...]
 
     def __init__(self, parent: library_wgt_t = None):
         """"""
         super().__init__(parent=parent)
+
         # Do not use self.__class__.__slots__ because it will be the parent slots in case of inheritance
         for slot in sequence_wgt_t.__slots__:
             setattr(self, slot, None)
 
     @classmethod
     def NewWithDetails(
         cls,
         value: tuple | None | missing_required_value_t,
-        att_type: constrained_type_t,
+        value_type: type_t,
         _: parameter_t,
     ) -> sequence_wgt_t:
         """
-        If att_type does not contain the necessary details, a simple free-text input widget is used. If the value is not
-        coherent with the details (which should not happen if att_type contains the necessary details and the value has
+        If value_type does not contain the necessary details, a simple free-text input widget is used. If the value is not
+        coherent with the details (which should not happen if value_type contains the necessary details and the value has
         been validated), a choice with the length of the value is added, with an exclamation point.
         """
-        instance = cls()
+        output = cls()
 
-        if (value is None) or isinstance(value, missing_required_value_t):
+        if (value is None) or (value is MISSING_REQUIRED_VALUE):
             value = ()
         length = value.__len__()
 
-        annotation = att_type.FirstConstraintWithAttribute("lengths")
+        annotation = value_type.FirstAnnotationWithAttribute("lengths")
         if annotation is None:
             entries = cls.ENTRIES
             max_entry = int(entries[-2])
         elif (lengths := annotation.lengths) == sequence_t.ANY_LENGTH:
             entries = (cls.ENTRY_ANY,)
             max_entry = None
         else:
@@ -92,50 +98,50 @@
                 # This should never happen since the value must have been validated
                 entries = entries + (str(length) + "!",)
                 max_entry = max(max_entry, length)
 
         if entries.__len__() > 1:
             length_selector = choices_list_wgt_t()
             for entry in entries:
-                length_selector.AddItem(entry)
+                length_selector.addItem(entry)
 
             if (length_as_str := str(length)) in entries:
-                length_selector.SetCurrentText(length_as_str)
+                length_selector.setCurrentText(length_as_str)
             if length_as_str + "!" in entries:
-                length_selector.SetCurrentText(length_as_str + "!")
+                length_selector.setCurrentText(length_as_str + "!")
             else:  # cls.ENTRY_ANY is necessarily in entries
-                length_selector.SetCurrentText(cls.ENTRY_ANY)
+                length_selector.setCurrentText(cls.ENTRY_ANY)
 
-            instance.length_selector = length_selector
-            instance.length_selector.SetFunction(instance.SetLength)
+            output.length_selector = length_selector
+            output.length_selector.SetFunction(output.SetLength)
 
         components = []
         if max_entry is None:
             value_as_str = str(value)[1:-1] if length > 0 else ""
-            widget = simple_entry_wgt_t(value_as_str, parent=None)
+            widget = text_wgt_t(value_as_str, parent=None)
             components.append(widget)
         else:
             for e_idx in range(max_entry):
                 value_as_str = str(value[e_idx]) if e_idx < length else ""
-                widget = simple_entry_wgt_t(value_as_str, parent=None)
+                widget = text_wgt_t(value_as_str, parent=None)
                 if e_idx >= length:
-                    widget.SetVisible(False)
+                    widget.setVisible(False)
                     widget.setEnabled(False)
                 components.append(widget)
-        instance.components = tuple(components)
+        output.components = tuple(components)
 
         layout = hbox_lyt_t()
-        layout.SetContentsMargins(0, 0, 0, 0)
-        if instance.length_selector is not None:
-            layout.AddWidget(instance.length_selector)
-        for component in instance.components:
-            layout.AddWidget(component)
-        instance.SetLayout(layout)
+        layout.setContentsMargins(0, 0, 0, 0)
+        if output.length_selector is not None:
+            layout.addWidget(output.length_selector)
+        for component in output.components:
+            layout.addWidget(component)
+        output.setLayout(layout)
 
-        return instance
+        return output
 
     def SetLength(self, new_index: int) -> None:
         """"""
         new_length = self.length_selector.ItemAt(new_index)
         if new_length == self.__class__.ENTRY_ANY:
             new_length = 1
         elif new_length.endswith("!"):
@@ -149,15 +155,15 @@
         contents = []
         for component in self.components:
             # Do not use "visible" here since setting visible does not really set the property until it is actually
             # shown. The documentation explains about ancestors being visible or not, but it was not clear that the
             # property is apparently not effective immediately.
             if not component.isEnabled():
                 break
-            component_as_str = component.Text().strip()
+            component_as_str = component.Text()
             if component_as_str.__len__() == 0:
                 break
             contents.append(component_as_str)
 
         if contents.__len__() == 0:
             return "()"
         elif contents.__len__() == 1:
@@ -170,18 +176,18 @@
         Value cannot return a true value since there is no indication of the sequence elements type
         Cannot be done using: class.Value = class.Text since the Text method is added to instances, not to the class
         """
         return self.Text()
 
 
 def _AdjustComponents(
-    components: Sequence[simple_entry_wgt_t, ...],
+    components: Sequence[text_wgt_t, ...],
     length: int,
 ) -> None:
     """"""
     for c_idx, component in enumerate(components):
         if c_idx < length:
-            component.SetVisible(True)
+            component.setVisible(True)
             component.setEnabled(True)
         else:
-            component.SetVisible(False)
+            component.setVisible(False)
             component.setEnabled(False)
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/component/type_options.py` & `conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/type_selector.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,43 +27,39 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from typing import Sequence
 
-from conf_ini_g.interface.screen.library.pyqt5_generic import library_wgt_t
-from conf_ini_g.interface.screen.library.pyqt5_parameter import (
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.choices import (
     choices_list_wgt_t,
-    label_wgt_t,
 )
-from conf_ini_g.specification.constrained_type import constrained_type_t
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import library_wgt_t
+from conf_ini_g.specification.parameter.type import type_t
 from conf_ini_g.standard.type_extension import none_t
 
 
-single_type_wgt_t = label_wgt_t
-
-
-class multiple_types_wgt_t(choices_list_wgt_t):
+class type_selector_wgt_t(choices_list_wgt_t):
     """"""
 
     def __init__(
         self,
-        types: Sequence[constrained_type_t],
-        selected_type: constrained_type_t,
+        types: Sequence[type_t],
+        selected_type: type_t,
         parent: library_wgt_t = None,
     ) -> None:
         """"""
         super().__init__(parent=parent)
 
         for type_ in types:
             if type_.py_type is none_t:
-                self.AddItem("None")
+                self.addItem("None")
             else:
-                self.AddItem(type_.py_type.__name__)
-        self.SetCurrentText(selected_type.py_type.__name__)
+                self.addItem(type_.py_type.__name__)
+        self.setCurrentText(selected_type.py_type.__name__)
 
     def Value(self) -> str:
         """
         Cannot be done using: class.Value = class.Text since the Text method is added to instances, not to the class
         """
         return self.Text()
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/config.py` & `conf-ini-g-2023.5/conf_ini_g/interface/screen/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,352 +27,359 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
-from typing import Annotated, Callable, Iterator, Sequence
+from typing import Annotated, Callable, Iterator
 
-import conf_ini_g.activated.config as actv
-import conf_ini_g.interface.screen.component.file_dialogs as fd_
-import conf_ini_g.interface.storage.config as iocf
-from conf_ini_g.interface.screen.component.boolean import boolean_wgt_t
-from conf_ini_g.interface.screen.library.pyqt5_constant import (
-    ALIGNED_HCENTER,
-    SELECTABLE_TEXT,
-)
-from conf_ini_g.interface.screen.library.pyqt5_generic import (
+from conf_ini_g.catalog.interface.screen.library.pyqt5.constant import ALIGNED_HCENTER
+from conf_ini_g.catalog.interface.screen.library.pyqt5.main import (
     ShowErrorMessage,
+    ShowMessage,
+)
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.button import button_wgt_t
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import (
     grid_lyt_t,
     hbox_lyt_t,
+    label_wgt_t,
     library_wgt_t,
+    tabs_wgt_t,
     vbox_lyt_t,
 )
-from conf_ini_g.interface.screen.library.pyqt5_parameter import (
-    button_wgt_t,
-    label_wgt_t,
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.scroll_container import (
     scroll_container_t,
-    tabs_wgt_t,
 )
+from conf_ini_g.catalog.interface.screen.parameter.boolean import boolean_wgt_t
+from conf_ini_g.catalog.specification.parameter.boolean import boolean_t
+from conf_ini_g.catalog.specification.parameter.path import path_t
+from conf_ini_g.instance.config import config_t as config_instance_t
+from conf_ini_g.interface.screen.parameter.path_chooser import SelectedOutputFile
 from conf_ini_g.interface.screen.section import controlled_section_t, section_t
+from conf_ini_g.interface.storage.config import SaveRawConfigToINIDocument
+from conf_ini_g.interface.storage.constant import INI_COMMENT_MARKER
 from conf_ini_g.raw.config import AsStr, ini_config_h, raw_config_h
-from conf_ini_g.specification.config import config_t as config_spec_t
-from conf_ini_g.specification.constrained_type import constrained_type_t
-from conf_ini_g.specification.constraint import boolean_t, path_t
-from conf_ini_g.specification.section import section_t as section_spec_t
-from conf_ini_g.standard.path_extension import any_path_h
+from conf_ini_g.specification.parameter.type import type_t
 from conf_ini_g.standard.path_extension import path_t as pl_path_t
 
 
 class config_t(library_wgt_t):
     __slots__ = (
-        "ini_document",
-        "target",
+        "instance",
         "sections",
     )
-    ini_document: pl_path_t | None
-    target: config_spec_t
-    sections: list[section_t]
+    # Widget might not cooperate well with list, in which case Python raises the
+    # following exception: TypeError: multiple bases have instance lay-out conflict
+    # To be safe, "sections" is field instead of being part of the class definition.
+    sections: dict[str, section_t | controlled_section_t]
+    instance: config_instance_t
+    action_button: button_wgt_t
+    Action: Callable[[raw_config_h], None]
 
-    def __init__(self, title: str | None, /) -> None:
+    def __init__(self) -> None:
         """"""
         super().__init__()
-        if title is not None:
-            self.SetWindowTitle(title)
-
         # Do not use self.__class__.__slots__ because it will be the parent slots in case of inheritance
         for slot in config_t.__slots__:
             setattr(self, slot, None)
 
     @classmethod
     def NewFromConfig(
         cls,
         title: str | None,
-        config: config_spec_t,
+        instance: config_instance_t,
         /,
         *,
         advanced_mode: bool = False,
-        ini_document: any_path_h = None,
         action: tuple[str, Callable[[raw_config_h], None]] = None,
     ) -> config_t:
         """"""
-        instance = cls(title)
-        if is_linked_to_ini := (ini_document is not None):
-            instance.ini_document = pl_path_t(ini_document)
-        instance.target = config
+        output = cls()
+        output.instance = instance
+        output.Action = action[1]
 
         # --- Top-level widgets
         if title is None:
-            title_wgt = None
+            components = []
         else:
-            title_wgt = label_wgt_t("<b>" + title + "</b>")
-            title_wgt.SetAlignment(ALIGNED_HCENTER)
-        advanced_mode_lyt = _AdvancedModeLayout(advanced_mode, instance)
-        button_lyt = _ActionButtonsLayout(is_linked_to_ini, instance, action)
+            components = [title]
+        home = pl_path_t.home()
+        if instance.ini_path is not None:
+            components.append(f"INI:{instance.ini_path.relative_to(home)}")
+        components.append(f"SPEC:{instance.specification.spec_path}")
+        title = "<br/>".join(components)
+
+        title_wgt = label_wgt_t("<b>" + title + "</b>")
+        title_wgt.setAlignment(ALIGNED_HCENTER)
+        advanced_mode_lyt = _AdvancedModeLayout(advanced_mode, output)
+        button_lyt = _ActionButtonsLayout(output, action, instance.ini_path is not None)
 
         # --- Sections
         categories = {}
-        sections = []
+        sections = {}
         controlled_sections = []
 
-        for section in config:
-            if section.controller is None:
-                visual_section = section_t.NewForSection(section)
+        for section_spec in instance.specification:
+            if (controller := section_spec.controller) is None:
+                section = section_t.NewForSection(
+                    section_spec, instance[section_spec.name]
+                )
             else:
-                visual_section = controlled_section_t.NewForSection(section)
-                if visual_section is not None:
-                    controlled_sections.append((visual_section, section))
-            if visual_section is None:
+                section = controlled_section_t.NewForSection(
+                    section_spec,
+                    controller,
+                    instance.GetValueOfController(controller),
+                    instance[section_spec.name],
+                )
+                if section is not None:
+                    controlled_sections.append((section, section_spec))
+            if section is None:
                 continue
 
-            sections.append(visual_section)
+            sections[section_spec.name] = section
 
-            if (category_name := section.category) not in categories:
+            if (category := section_spec.category) not in categories:
                 contents = library_wgt_t(parent=None)
-                layout = vbox_lyt_t()
-                contents.SetLayout(layout)
                 scroll_area = scroll_container_t.NewForWidget(contents)
-                categories[category_name] = (layout, scroll_area)
+                layout = vbox_lyt_t()
+                contents.setLayout(layout)
+                categories[category] = (layout, scroll_area)
 
-            layout = categories[category_name][0]
-            layout.AddWidget(visual_section)
+            layout = categories[category][0]
+            layout.addWidget(section)
 
-        instance.sections = sections
+        output.sections = sections
 
         if categories.__len__() > 1:
             category_selector = tabs_wgt_t()
-            for category_name, (_, scroll_area) in categories.items():
-                category_selector.AddTab(scroll_area, category_name)
+            for category, (_, scroll_area) in categories.items():
+                category_selector.addTab(scroll_area, category)
         else:
-            category_name = tuple(categories.keys())[0]
-            category_selector = categories[category_name][1]
+            category = tuple(categories.keys())[0]
+            category_selector = categories[category][1]
 
-        for visual_section, section_spec in controlled_sections:
-            section_name, uid = actv.ControllerSectionAndUid(section_spec, config)
-            parameter = instance[section_name][uid]
-            widget = parameter.active_value
-            if hasattr(widget, "SetFunction"):
-                widget.SetFunction(visual_section.page_stack.SetCurrentIndex)
+        for section, section_spec in controlled_sections:
+            controller = section_spec.controller
+            parameter = output[controller.section].parameters[controller.parameter]
+            value_wgt = parameter.active_value
+            if hasattr(value_wgt, "SetFunction"):
+                value_wgt.SetFunction(section.page_stack.setCurrentIndex)
             else:
-                controller = section_spec.controller
                 ShowErrorMessage(
                     f'{controller.section}.{controller.parameter}: Controller has no "SetFunction" method; Disabling control'
                 )
 
         # --- Layout...
         layout = grid_lyt_t()
         if title_wgt is None:
             first_available_row = 0
         else:
-            layout.AddWidget(title_wgt, 0, 0, 1, 1)
+            layout.addWidget(title_wgt, 0, 0, 1, 1)
             first_available_row = 1
-        layout.AddWidget(category_selector, first_available_row, 0, 1, 1)
+        layout.addWidget(category_selector, first_available_row, 0, 1, 1)
         layout.addLayout(advanced_mode_lyt, first_available_row + 1, 0, 1, 1)
-        layout.AddLayout(button_lyt, first_available_row + 2, 0, 1, 1)
+        layout.addLayout(button_lyt, first_available_row + 2, 0, 1, 1)
 
-        instance.SetLayout(layout)
+        output.setLayout(layout)
         # --- ...Layout
 
-        instance.ToogleAdvancedMode(advanced_mode)
-
-        return instance
-
-    def UpdateControlOfSection(self, section: section_spec_t, /) -> None:
-        """"""
-        section_name, uid = actv.ControllerSectionAndUid(section, self.target)
-        parameter = self[section_name][uid]
-        value = parameter.Value()
+        output.ToogleAdvancedMode(advanced_mode)
 
-        section.controller_value = value
+        return output
 
     def ToogleAdvancedMode(self, advanced_mode: bool, /) -> None:
         """"""
-        for section_spec, section in zip(self.target, self.sections):
+        for section_name, section in self.sections.items():
+            section_spec = self.instance.specification[section_name]
             if section_spec.basic:
                 should_check_parameters = True
             elif advanced_mode:
-                section.SetVisible(True)
+                section.setVisible(True)
                 should_check_parameters = True
             else:
-                section.SetVisible(False)
+                section.setVisible(False)
                 should_check_parameters = False
 
             if should_check_parameters:
-                active_parameters = section.active_parameters
-                active_uids = (_prm.uid for _prm in active_parameters)
-                parameter_specs = (section_spec[_uid] for _uid in active_uids)
-                for parameter_spec, parameter in zip(
-                    parameter_specs, active_parameters
+                if (controller := section_spec.controller) is None:
+                    parameter_specs = section_spec
+                else:
+                    controller_text = (
+                        self[controller.section].parameters[controller.parameter].Text()
+                    )
+                    parameter_specs = section_spec.ActiveParameters(controller_text)
+                for parameter, parameter_spec in zip(
+                    section.active_parameters.values(), parameter_specs
                 ):
                     if not parameter_spec.basic:
                         if advanced_mode:
-                            parameter.SetVisible(True)
+                            parameter.setVisible(True)
                         else:
-                            parameter.SetVisible(False)
+                            parameter.setVisible(False)
 
-    def AsINIConfig(self) -> ini_config_h:
+    def SynchronizeInstance(self) -> list[str]:
         """"""
-        output = {}
-
-        for section_spec, section in zip(self.target, self):
-            section_name = section_spec.name
-            section_as_dict = {}
+        for section_name, section in self.sections.items():
+            section_spec = self.instance.specification[section_name]
+            if (controller := section_spec.controller) is None:
+                parameter_specs = section_spec
+            else:
+                controller_text = (
+                    self[controller.section].parameters[controller.parameter].Text()
+                )
+                parameter_specs = section_spec.ActiveParameters(controller_text)
+            for parameter, parameter_spec in zip(
+                section.active_parameters.values(), parameter_specs
+            ):
+                if parameter.unit is None:
+                    unit_kwarg = {}
+                else:
+                    unit_kwarg = {"unit": parameter.unit.Text()}
+                instance = self.instance[section_spec.name][parameter_spec.name]
+                instance.SetValue(
+                    parameter.Value(),
+                    INI_COMMENT_MARKER,
+                    parameter_spec.types,
+                    **unit_kwarg,
+                )
 
-            for parameter in section.active_parameters:
-                name = self.target[section_name][parameter.uid].name
-                section_as_dict[name] = parameter.Text()
+        return self.instance.Issues()
 
-            output[section_name] = section_as_dict
+    def AsINIConfig(self) -> ini_config_h | None:
+        """"""
+        issues = self.SynchronizeInstance()
+        if issues.__len__() == 0:
+            output = self.instance.AsINIConfig()
+        else:
+            output = None
+            ShowErrorMessage("\n".join(issues), parent=self)
 
         return output
 
     def ShowInINIFormat(self) -> None:
         """"""
         config = self.AsINIConfig()
-        config = AsStr(config, in_html_format=True)
-        label = label_wgt_t("<tt>" + config + "<tt/>")
-        label.SetStyleSheet("font-weight:bold; padding:20px;")
-        label.SetTextInteractionFlags(SELECTABLE_TEXT)
-        label.show()
-
-    def SaveToTarget(self) -> Sequence[str] | None:
-        """"""
-        for section_spec, section in zip(self.target, self):
-            if section_spec.controller is not None:
-                self.UpdateControlOfSection(section_spec)
-
-            for parameter in section.active_parameters:
-                value = parameter.Value()
-                parameter_spec = section_spec[parameter.uid]
-                parameter_spec.actual.SetTypesAndValueFromString(
-                    value, parameter_spec.type_options
-                )
+        if config is None:
+            return
 
-        return self.target.Issues(pre_units=False)
+        config = AsStr(config, in_html_format=True)
+        ShowMessage("INI Config", "<tt>" + config + "<tt/>")
 
     def SaveConfig(self, new_ini: bool, /) -> None:
-        #
-        do_save = True
-
+        """"""
         if new_ini:
-            doc_name = fd_.SelectedOutputFile(
+            path = SelectedOutputFile(
                 "Save Config As",
                 "Save Config As",
                 mode=path_t.TARGET_TYPE.document,
                 valid_types={"Config files": ("ini", "INI")},
             )
-            if doc_name is None:
-                do_save = False
-            else:
-                self.ini_document = doc_name
         else:
-            pass  # Will overwrite self.ini_document
+            path = self.instance.ini_path  # Will overwrite current INI document
 
-        if do_save:
+        if path is not None:
             config = self.AsINIConfig()
-            error = iocf.SaveRawConfigToINIDocument(config, self.ini_document)
-            if error is not None:
-                ShowErrorMessage(error, self)
-
-    def __getitem__(
-        self, key: str | int
-    ) -> section_t | controlled_section_t:
-        """"""
-        if isinstance(key, str):
-            for section, section_spec in zip(self.sections, self.target):
-                if key == section_spec.name:
-                    return section
+            error = SaveRawConfigToINIDocument(config, path)
+            if error is None:
+                self.instance.ini_path = path
+            else:
+                ShowErrorMessage(error, parent=self)
+
+    def LaunchAction(self) -> None:
+        """"""
+        issues = self.SynchronizeInstance()
+        if issues.__len__() == 0:
+            raw_config, issues = self.instance.AsRawConfig()
+            if issues.__len__() == 0:
+                self.action_button.setEnabled(False)
+                try:
+                    self.Action(raw_config)
+                except Exception as exception:
+                    ShowErrorMessage(str(exception), parent=self)
+                self.action_button.setEnabled(True)
+            else:
+                ShowErrorMessage("\n".join(issues), parent=self)
         else:
-            raise KeyError(
-                f"{self.__class__.__name__}: Not meant to be accessed as a list"
-            )
+            ShowErrorMessage("\n".join(issues), parent=self)
+
+    def __contains__(self, key: str, /) -> bool:
+        """"""
+        return key in self.sections
 
-        raise KeyError(f"{key}: Not an existing section")
+    def __getitem__(self, key: str, /) -> section_t | controlled_section_t:
+        """"""
+        return self.sections[key]
 
-    def __iter__(self) -> Iterator[section_t]:
+    def __iter__(self) -> Iterator[str]:
         """"""
-        return iter(self.sections)
+        return self.sections.keys()
 
 
-def _AdvancedModeLayout(advanced_mode: bool, parent: config_t, /) -> hbox_lyt_t:
+def _AdvancedModeLayout(advanced_mode: bool, config: config_t, /) -> hbox_lyt_t:
     """"""
     output = hbox_lyt_t()
 
     annotated_type = Annotated[bool, boolean_t(mode=boolean_t.MODE.on_off)]
-    att_type = constrained_type_t.NewFromAnnotatedType(annotated_type)
+    value_type = type_t.NewFromAnnotatedType(annotated_type)
     boolean = boolean_wgt_t.NewWithDetails(
         advanced_mode,
-        att_type,
+        value_type,
         None,
     )
-    boolean.true_btn.toggled.connect(parent.ToogleAdvancedMode)
+    boolean.true_btn.SetFunction(config.ToogleAdvancedMode)
 
     output.addWidget(label_wgt_t("<i>Advanced Mode</i>"))
     output.addWidget(boolean)
 
     return output
 
 
 def _ActionButtonsLayout(
-    has_ini_document: bool,
-    parent: config_t,
+    config: config_t,
     action: tuple[str, Callable[[raw_config_h], None]] | None,
+    has_ini_document: bool,
     /,
 ) -> grid_lyt_t:
-    #
+    """"""
+    layout = grid_lyt_t()
+
     buttons = []
     geometries = []
 
     button = button_wgt_t("Show in INI format")
-    button.SetFunction(parent.ShowInINIFormat)
+    button.SetFunction(config.ShowInINIFormat)
     buttons.append(button)
     geometries.append((0, 0, 1, 2))
 
     button = button_wgt_t("Save Config As")
-    button.SetFunction(lambda: parent.SaveConfig(True))
+    button.SetFunction(lambda: config.SaveConfig(True))
     buttons.append(button)
     if has_ini_document:
         geometries.append((1, 0, 1, 1))
 
-        button = button_wgt_t("Save Config (Overwriting)")
-        button.SetFunction(lambda: parent.SaveConfig(False))
+        button = button_wgt_t("Save/Overwrite Config")
+        button.SetFunction(lambda: config.SaveConfig(False))
         buttons.append(button)
         geometries.append((1, 1, 1, 1))
     else:
         geometries.append((1, 0, 1, 2))
 
     if action is None:
         label = "Close"
+        Function = config.Close
     else:
         label = action[0]
-    button = button_wgt_t(label)
-    if action is None:
-        function = parent.Close
-    else:
+        Function = config.LaunchAction
 
-        def function():
-            issues = parent.SaveToTarget()
-            if issues is None:
-                config, issues = actv.RawConfigWithConsumedUnits(parent.target)
-                if issues is None:
-                    button.SetEnabled(False)
-                    try:
-                        action[1](config)
-                    except Exception as exception:
-                        ShowErrorMessage(str(exception), parent)
-                    button.SetEnabled(True)
-                else:
-                    ShowErrorMessage("\n".join(issues), parent)
-            else:
-                ShowErrorMessage("\n".join(issues), parent)
-
-    button.SetFunction(function)
+    button = button_wgt_t(label)
+    button.SetFunction(Function)
     buttons.append(button)
     geometries.append((2, 0, 1, 2))
 
-    layout = grid_lyt_t()
+    config.action_button = button
+
     for button, geometry in zip(buttons, geometries):
-        layout.AddWidget(button, *geometry)
+        layout.addWidget(button, *geometry)
     layout.setContentsMargins(0, 0, 0, 0)
 
     return layout
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/generic.py` & `conf-ini-g-2023.5/conf_ini_g/interface/screen/generic.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,22 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from conf_ini_g.specification.constant import STD_ABBREVIATIONS
+STD_ABBREVIATIONS = {
+    "fct": "function",
+    "mod": "module",
+    "n": "number of",
+    "o": "of",
+    "prm": "parameter",
+    "rng": "range",
+}
 
 
 def FormattedName(name: str, separator: str) -> str:
     """"""
     name_cmps = []
     for component in name.split(separator):
         name_cmps.append(STD_ABBREVIATIONS.get(component, component))
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/library/pyqt5_constant.py` & `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,25 +30,25 @@
 # knowledge of the CeCILL license and that you accept its terms.
 
 import PyQt5.QtCore as core
 import PyQt5.QtGui as visl
 import PyQt5.QtWidgets as wdgt
 
 
-ALIGNED_HCENTER = core.Qt.AlignHCenter
-ALIGNED_RIGHT = core.Qt.AlignRight
-ALIGNED_TOP = core.Qt.AlignTop
+ALIGNED_HCENTER = core.Qt.AlignmentFlag.AlignHCenter
+ALIGNED_RIGHT = core.Qt.AlignmentFlag.AlignRight
+ALIGNED_TOP = core.Qt.AlignmentFlag.AlignTop
 BASE_PALETTE = visl.QPalette.Base
-COLOR_CYAN = core.Qt.cyan
+COLOR_CYAN = visl.QColorConstants.Cyan
 DIALOG_ACCEPTATION = wdgt.QDialog.Accepted
 DIALOG_ACCEPT_OPEN = wdgt.QFileDialog.AcceptOpen
 DIALOG_ACCEPT_SAVE = wdgt.QFileDialog.AcceptSave
 DIALOG_AUTO_OVERWRITE = wdgt.QFileDialog.DontConfirmOverwrite
 DIALOG_MODE_ANY = wdgt.QFileDialog.AnyFile
 DIALOG_MODE_EXISTING_FILE = wdgt.QFileDialog.ExistingFile
 DIALOG_MODE_FOLDER = wdgt.QFileDialog.Directory
-FORMAT_RICH = core.Qt.RichText
-SELECTABLE_TEXT = core.Qt.TextSelectableByMouse
+FORMAT_RICH = core.Qt.TextFormat.RichText
+SELECTABLE_TEXT = core.Qt.TextInteractionFlag.TextSelectableByMouse
 SIZE_EXPANDING = wdgt.QSizePolicy.Expanding
 SIZE_FIXED = wdgt.QSizePolicy.Fixed
 SIZE_MINIMUM = wdgt.QSizePolicy.Minimum
 TAB_POSITION_EAST = wdgt.QTabWidget.East
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/library/pyqt5_generic.py` & `conf-ini-g-2023.5/conf_ini_g/light/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,100 +25,100 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-# Necessary since library_wgt_t is not defined until after the call to CreateClassesWithCapitalizedMethods
 from __future__ import annotations
 
-from types import BuiltinMethodType, MethodType
-from typing import Sequence
+import inspect as nspt
+from typing import Callable
 
-import PyQt5.QtCore as core
-import PyQt5.QtWidgets as wdgt
+from rich.text import Text as text_t
 
-
-# SetCapitalizedMethods does not "see" the methods of the base classes. So for example, calling it on QHBoxLayout has no
-# effect on the methods of QLayout. Therefore, it might be necessary to call it also on QLayout even if QLayout is not
-# use explicitly.
-_CLASSES = (
-    ("library_wgt_t", wdgt.QWidget),
-    ("layout_t", wdgt.QLayout),
-    ("hbox_lyt_t", wdgt.QHBoxLayout),
-    ("vbox_lyt_t", wdgt.QVBoxLayout),
-    ("grid_lyt_t", wdgt.QGridLayout),
+from conf_ini_g.raw.config import ini_config_h
+from conf_ini_g.standard.path_extension import any_path_h, path_t
+from conf_ini_g.standard.str_extension import (
+    AlignedOnSeparator,
+    AsComplexInterpretedObject,
+)
+from conf_ini_g.standard.type_extension import (
+    NameValueTypeAsRichStr,
+    TypeAsRichStr,
+    raw_hint_h,
 )
 
 
-def SetCapitalizedMethods(widget: wdgt.QLayout | library_wgt_t) -> None:
-    """
-    AMethod = wdgt.QSomeWidgetClass.aMethod does not work because the call then misses self
-    """
-    for name in dir(widget):
-        first_letter = name[0]
-        # hasattr test: necessary since this function is called early in the initialization process, so some fields
-        # might not have been set yet.
-        if (
-            (first_letter != "_")
-            and (first_letter == first_letter.lower())
-            and hasattr(widget, name)
-        ):
-            attribute = getattr(widget, name)
-            if isinstance(attribute, (BuiltinMethodType, MethodType)):
-                capitalized = first_letter.upper() + name[1:]
-                if not hasattr(widget, capitalized):
-                    setattr(widget, first_letter.upper() + name[1:], attribute)
-
-
-def CreateClassesWithCapitalizedMethods(
-    classes: Sequence[tuple[str, type]], scope: dict
-) -> None:
-    """"""
-    for new_class, base_class in classes:
+SECTION_PARAMETER_SEPARATOR = "__"
 
-        def InitWithMethodCapitalization(self, *args, **kwargs) -> None:
-            """"""
-            base_class.__init__(self, *args, **kwargs)
-            SetCapitalizedMethods(self)
 
-        cls = type(new_class, (base_class,), {})
-        setattr(cls, "__init__", InitWithMethodCapitalization)
-        scope[new_class] = cls
+class config_t:
+    path: path_t
+    _type_hints: dict[str, raw_hint_h]
 
+    @classmethod
+    def NewFromDictionary(
+        cls, ini_config: ini_config_h, /, *, path: any_path_h = None
+    ) -> config_t:
+        """
+        The dictionary values are already properly typed
+        """
+        output = cls()
 
-CreateClassesWithCapitalizedMethods(_CLASSES, globals())
+        if (path is not None) and isinstance(path, str):
+            path = path_t(path)
 
+        output.path = path
+        output._type_hints = nspt.get_annotations(cls)
 
-class file_selection_wgt_t(wdgt.QFileDialog):
-    """"""
+        issues = []
+        for s_name, section in ini_config.items():
+            for p_name, value in section.items():
+                issues.extend(output.Set(_FullName(s_name, p_name), value))
 
-    def __init__(self, caption: str, extension_filter: str = None):
-        """"""
-        if extension_filter is None:
-            extension_filter = "Any files (*)"
-        super().__init__(caption=caption, filter=extension_filter)
-        SetCapitalizedMethods(self)
+        if issues.__len__() > 0:
+            issues = "\n".join(issues)
+            print(f"{path}: Invalid configuration.\n{issues}")
+            raise ValueError
 
-    def SelectedFile(self) -> str:
-        return self.selectedFiles()[0]
+        return output
 
-    def RunAndGetClosingStatus(self) -> int:
-        return self.exec_()
+    def Set(self, name: str, value: str, /) -> list[str]:
+        """"""
+        expected_type = self._type_hints[name]
+        typed_value, success = AsComplexInterpretedObject(
+            value, expected_type=expected_type
+        )
+        if success:
+            setattr(self, name, typed_value)
+            return []
+
+        return [
+            f"{type(typed_value).__name__}: "
+            f'Incompatible type of value "{typed_value}"; Expected={expected_type}.'
+        ]
 
+    def __str__(self) -> str:
+        """"""
+        return text_t.from_markup(self.__rich__()).plain
 
-class widget_event_loop_t(wdgt.QApplication):
-    """"""
+    def __rich__(self) -> str:
+        """"""
+        output = [TypeAsRichStr(self)]
+
+        AllButCallable = lambda _elm: not isinstance(_elm, Callable)
+        for name, value in nspt.getmembers(self, AllButCallable):
+            if name[0] != "_":
+                name = name.replace(SECTION_PARAMETER_SEPARATOR, ".", 1)
+                output.append(
+                    "    " + NameValueTypeAsRichStr(name, value, separator="@=@")
+                )
 
-    @staticmethod
-    def GetInstance() -> core.QCoreApplication:
-        return widget_event_loop_t.instance()
+        output = AlignedOnSeparator(output, "@=@", " = ")
 
-    @staticmethod
-    def Run() -> int:
-        return wdgt.QApplication.exec_()
+        return "\n".join(output)
 
 
-def ShowErrorMessage(message: str, parent: library_wgt_t = None) -> None:
+def _FullName(section: str, parameter: str, /) -> str:
     """"""
-    wdgt.QMessageBox.critical(parent, "Error", message)
+    return f"{section.strip().lower().replace(' ', '_')}{SECTION_PARAMETER_SEPARATOR}{parameter.strip().lower()}"
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/library/pyqt5_parameter.py` & `conf-ini-g-2023.5/conf_ini_g/instance/parameter/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,95 +25,81 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
-
-from typing import Callable
-
-import PyQt5.QtWidgets as wdgt
-
-from conf_ini_g.interface.screen.library.pyqt5_generic import (
-    CreateClassesWithCapitalizedMethods,
-    SetCapitalizedMethods,
-    library_wgt_t,
-)
-
-
-_CLASSES = (
-    ("label_wgt_t", wdgt.QLabel),
-    ("simple_entry_wgt_t", wdgt.QLineEdit),
-    ("group_wgt_t", wdgt.QGroupBox),
-    ("stack_wgt_t", wdgt.QStackedWidget),
-    ("tabs_wgt_t", wdgt.QTabWidget),
-)
-
-
-class button_wgt_t(wdgt.QPushButton):
-    """"""
-
-    def __init__(self, text: str, parent: library_wgt_t = None):
+import dataclasses as dtcl
+from abc import ABC as abstract_class_t
+from abc import abstractmethod
+from typing import Any
+
+from rich.text import Text as text_t
+
+from conf_ini_g.specification.parameter.type import type_options_t, type_t
+from conf_ini_g.specification.parameter.value import INVALID_VALUE
+
+
+@dtcl.dataclass(repr=False, eq=False)
+class base_t(abstract_class_t):
+    type: type_t = None
+    value: Any = None
+    comment: str = None
+
+    @abstractmethod
+    def SetValue(
+        self,
+        value_w_unit_w_comment: str | Any,
+        comment_marker: str,
+        type_options: type_options_t | None,
+        /,
+        *,
+        unit: str = None,
+    ) -> None:
         """"""
-        super().__init__(text=text, parent=parent)
-        SetCapitalizedMethods(self)
-
-    def SetFunction(self, function: Callable) -> None:
-        self.clicked.connect(function)
-
-
-class choices_dots_wgt_t(wdgt.QRadioButton):
-    """"""
+        ...
 
-    def __init__(self, text: str, parent: library_wgt_t = None):
+    @abstractmethod
+    def Text(self) -> str:
         """"""
-        super().__init__(text=text, parent=parent)
-        SetCapitalizedMethods(self)
+        ...
 
-    def SetFunction(self, function: Callable) -> None:
-        self.clicked.connect(function)
-
-
-class choices_list_wgt_t(wdgt.QComboBox):
-    """"""
-
-    def __init__(self, *args, **kwargs):
+    def Issues(self) -> list[str]:
         """"""
-        super().__init__(*args, **kwargs)
-        SetCapitalizedMethods(self)
-
-    def Selection(self) -> str:
-        return self.currentText()
-
-    def SelectionIndex(self) -> int:
-        return self.currentIndex()
+        if self.value is INVALID_VALUE:
+            return [f"No matching type in specification or invalid value"]
 
-    def ItemAt(self, index: int) -> str:
-        return self.itemText(index)
+        return []
 
-    def SetFunction(self, function: Callable) -> None:
-        self.activated.connect(function)
-        # OR: self.currentTextChanged.connect(function)
-
-
-class scroll_container_t(wdgt.QScrollArea):
-    """"""
-
-    def __init__(self, *args, **kwargs):
+    def __str__(self) -> str:
         """"""
-        super().__init__(*args, **kwargs)
-        SetCapitalizedMethods(self)
+        return text_t.from_markup(self.__rich__()).plain
 
-    @classmethod
-    def NewForWidget(cls, widget: library_wgt_t) -> scroll_container_t:
+    def __rich__(self) -> str:
         """"""
-        instance = cls()
-        instance.setWidget(widget)
-        instance.setWidgetResizable(True)
-        # instance.setBackgroundRole(qg_.QPalette.Dark)
+        if self.type is None:
+            return f"[blue]{type(self).__name__}[/]={self.Text()}"
+
+        return (
+            f"[blue]{type(self).__name__}[/]={self.Text()}"
+            f"[yellow]:{self.type.py_type.__name__}[/]"
+        )
 
-        return instance
 
+def Pieces(
+    combined: str, separator: str, /, *, from_left: bool = True
+) -> tuple[str, str | None]:
+    """"""
+    if from_left:
+        where_separator = combined.find(separator)
+    else:
+        where_separator = combined.rfind(separator)
+
+    if where_separator != -1:
+        left = combined[:where_separator].strip()
+        right = combined[(where_separator + 1) :].strip()
+    else:
+        left = combined
+        right = None
 
-CreateClassesWithCapitalizedMethods(_CLASSES, globals())
+    return left, right
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/screen/parameter.py` & `conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,184 +30,166 @@
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 import dataclasses as dtcl
 from typing import Any, Type
 
-from conf_ini_g.interface.screen.component.boolean import boolean_wgt_t
-from conf_ini_g.interface.screen.component.choices import choices_wgt_t
-from conf_ini_g.interface.screen.component.default_entry import default_entry_wgt_t
-from conf_ini_g.interface.screen.component.none import none_wgt_t
-from conf_ini_g.interface.screen.component.path import path_wgt_t
-from conf_ini_g.interface.screen.component.sequence import sequence_wgt_t
-from conf_ini_g.interface.screen.component.type_options import (
-    multiple_types_wgt_t,
-    single_type_wgt_t,
-)
-from conf_ini_g.interface.screen.generic import FormattedName
-from conf_ini_g.interface.screen.library.pyqt5_constant import (
+from conf_ini_g.catalog.interface.screen.library.pyqt5.constant import (
     SIZE_EXPANDING,
     SIZE_FIXED,
 )
-from conf_ini_g.interface.screen.library.pyqt5_generic import library_wgt_t
-from conf_ini_g.interface.screen.library.pyqt5_parameter import (
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import (
     label_wgt_t,
-    simple_entry_wgt_t,
+    library_wgt_t,
     stack_wgt_t,
 )
-from conf_ini_g.specification.constant import UNIT_SEPARATOR
-from conf_ini_g.specification.constrained_type import (
-    SIMPLE_ATT_TYPES,
-    constrained_type_t,
-)
-from conf_ini_g.specification.parameter import parameter_t as parameter_spec_t
-from conf_ini_g.standard.type_extension import any_type_h
-
-
-_TYPE_WIDGET_TRANSLATOR: dict[constrained_type_t, Type[library_wgt_t]] = {
-    SIMPLE_ATT_TYPES["boolean"]: boolean_wgt_t,
-    SIMPLE_ATT_TYPES["float"]: default_entry_wgt_t,
-    SIMPLE_ATT_TYPES["int"]: default_entry_wgt_t,
-    SIMPLE_ATT_TYPES["choices"]: choices_wgt_t,
-    SIMPLE_ATT_TYPES["path"]: path_wgt_t,
-    SIMPLE_ATT_TYPES["sequence"]: sequence_wgt_t,
-    SIMPLE_ATT_TYPES["None"]: none_wgt_t,
+from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.text import text_wgt_t
+from conf_ini_g.catalog.interface.screen.parameter.boolean import boolean_wgt_t
+from conf_ini_g.catalog.interface.screen.parameter.choices import choices_wgt_t
+from conf_ini_g.catalog.interface.screen.parameter.none import none_wgt_t
+from conf_ini_g.catalog.interface.screen.parameter.path import path_wgt_t
+from conf_ini_g.catalog.interface.screen.parameter.sequence import sequence_wgt_t
+from conf_ini_g.catalog.interface.screen.parameter.text import default_entry_wgt_t
+from conf_ini_g.instance.parameter.main import instance_t
+from conf_ini_g.interface.screen.generic import FormattedName
+from conf_ini_g.interface.screen.parameter.type_selector import type_selector_wgt_t
+from conf_ini_g.specification.parameter.main import parameter_t as parameter_spec_t
+from conf_ini_g.specification.parameter.type import BASIC_TYPES, type_t
+from conf_ini_g.specification.parameter.unit import UNIT_SEPARATOR
+from conf_ini_g.standard.type_extension import any_hint_h
+
+_TYPE_WIDGET_TRANSLATOR: dict[type_t, Type[library_wgt_t]] = {
+    BASIC_TYPES["boolean"]: boolean_wgt_t,
+    BASIC_TYPES["float"]: default_entry_wgt_t,
+    BASIC_TYPES["int"]: default_entry_wgt_t,
+    BASIC_TYPES["choices"]: choices_wgt_t,
+    BASIC_TYPES["path"]: path_wgt_t,
+    BASIC_TYPES["sequence"]: sequence_wgt_t,
+    BASIC_TYPES["None"]: none_wgt_t,
 }
 
 
 @dtcl.dataclass(repr=False, eq=False)
 class parameter_t:
     """
     In order to leave the section widget put the name, type, and input widgets of each parameter in columns,
-    actual_t is not a container widget. Instead, it just store its component widgets for later addition to a layout.
+    parameter_t is not a container widget. Instead, it just stores its component widgets for later addition to a layout.
     """
 
-    uid: int  # Allows to retrieve the parameter specification
-    name: label_wgt_t = None  # Visual version, not functional one
-    type_selector: single_type_wgt_t | multiple_types_wgt_t = None
+    name: label_wgt_t = None
+    type_selector: label_wgt_t | type_selector_wgt_t = None
     value_stack: stack_wgt_t = None
-    unit: simple_entry_wgt_t = None
+    unit: text_wgt_t = None
     comment: str = None
 
     @classmethod
-    def NewForParameter(cls, parameter: parameter_spec_t, /) -> parameter_t:
+    def NewForParameter(
+        cls, parameter_spec: parameter_spec_t, instance: instance_t, /
+    ) -> parameter_t:
         """"""
-        instance = cls(uid=parameter.actual.uid)
+        output = cls()
 
-        formatted_name = FormattedName(parameter.name, " ")
-        comment = (
-            f"{formatted_name}\n{parameter.definition}.\n\n{parameter.description}."
-        )
-        if parameter.actual.comment is not None:
-            comment += f"\n\n{parameter.actual.comment}."
+        formatted_name = FormattedName(parameter_spec.name, " ")
 
-        instance.name = label_wgt_t(formatted_name)
-        instance.comment = comment
-        instance.name.SetToolTip(comment)
-
-        type_options = parameter.type_options
-        if type_options.__len__() > 1:
-            initial_type = parameter.actual.type
-            type_selector = multiple_types_wgt_t(type_options, initial_type)
+        comment = f"{formatted_name}\n{parameter_spec.definition}.\n\n{parameter_spec.description}."
+        if instance.comment is not None:
+            comment += f"\n\n{instance.comment}."
+        output.comment = comment
+
+        output.name = label_wgt_t(formatted_name)
+        output.name.setToolTip(comment)
+
+        types = parameter_spec.types
+        if types is None:
+            type_selector = label_wgt_t("Unspecified")
+            types = (instance.type,)
+        elif types.__len__() > 1:
+            type_selector = type_selector_wgt_t(types, instance.type)
         else:
-            type_selector = single_type_wgt_t(type_options[0].py_type.__name__)
-        instance.type_selector = type_selector
+            type_selector = label_wgt_t(types[0].py_type.__name__)
+        output.type_selector = type_selector
 
         value_stack = stack_wgt_t()
         initial_index = 0
-        for t_idx, att_type in enumerate(type_options):
-            if att_type is parameter.actual.type:
-                initial_value = parameter.actual.value
+        for t_idx, value_type in enumerate(types):
+            if value_type is instance.type:
+                initial_value = instance.value
                 initial_index = t_idx
             else:
                 initial_value = None
-            widget_type = _WidgetTypeForType(att_type)
+            widget_type = _WidgetTypeForType(value_type)
             value = widget_type.NewWithDetails(
                 initial_value,
-                att_type,
-                parameter,
+                value_type,
+                parameter_spec,
             )
-            value_stack.AddWidget(value)
-        value_stack.SetCurrentIndex(initial_index)
-        value_stack.SetSizePolicy(SIZE_EXPANDING, SIZE_FIXED)
-        instance.value_stack = value_stack
+            value_stack.addWidget(value)
+        value_stack.setCurrentIndex(initial_index)
+        value_stack.setSizePolicy(SIZE_EXPANDING, SIZE_FIXED)
+        output.value_stack = value_stack
 
-        if parameter.actual.unit is not None:
-            instance.unit = simple_entry_wgt_t(parameter.actual.unit)
+        if (unit := getattr(instance, "unit", None)) is not None:
+            output.unit = text_wgt_t(unit)
 
         name_style = "padding-right: 5px;"
-        if parameter.optional:
+        if parameter_spec.optional:
             name_style += "color: gray;"
-        instance.name.SetStyleSheet(name_style)
-        instance.type_selector.SetStyleSheet(name_style)
+        output.name.setStyleSheet(name_style)
+        output.type_selector.setStyleSheet(name_style)
 
-        if isinstance(type_selector, multiple_types_wgt_t):
-            type_selector.activated.connect(instance.value_stack.SetCurrentIndex)
+        if isinstance(type_selector, type_selector_wgt_t):
+            type_selector.SetFunction(output.value_stack.setCurrentIndex)
 
-        return instance
+        return output
+
+    def SetVisible(self, visible: bool, /) -> None:
+        """"""
+        self.name.setVisible(visible)
+        self.type_selector.setVisible(visible)
+        self.value_stack.setVisible(visible)
+        if self.unit is not None:
+            self.unit.setVisible(visible)
 
     @property
     def active_value(self) -> library_wgt_t:
         """"""
-        return self.value_stack.CurrentWidget()
+        return self.value_stack.currentWidget()
 
-    def SetVisible(self, visible: bool, /) -> None:
+    def Value(self) -> Any:
         """"""
-        self.name.SetVisible(visible)
-        self.type_selector.SetVisible(visible)
-        self.value_stack.SetVisible(visible)
-        if self.unit is not None:
-            self.unit.SetVisible(visible)
+        return self.active_value.Value()
 
     def Text(self) -> str:
-        #
-        output = self.active_value.Text()
-
-        if self.unit is None:
-            unit = None
-        else:
-            unit = self.unit.Text().strip()
-
-        if (unit is not None) and (unit.__len__() > 0):
-            output += UNIT_SEPARATOR + unit
-
-        return output
-
-    def Value(self) -> Any:
         """"""
-        if self.unit is None:
-            unit = None
-        else:
-            unit = self.unit.Text().strip()
+        text = self.active_value.Text()
 
-        if (unit is not None) and (unit.__len__() > 0):
-            output = self.active_value.Text() + UNIT_SEPARATOR + unit
-        else:
-            output = self.active_value.Value()
+        if self.unit is None:
+            return text
 
-        return output
+        return f"{text}{UNIT_SEPARATOR}{self.unit.Text()}"
 
 
 def RegisterNewTranslation(
-    new_type: any_type_h, widget_type: Type[library_wgt_t], /
+    new_type: any_hint_h, widget_type: Type[library_wgt_t], /
 ) -> None:
     """"""
-    att_type = constrained_type_t.NewFromType(new_type)
-    if att_type in _TYPE_WIDGET_TRANSLATOR:
+    value_type = type_t.NewFromType(new_type)
+    if value_type in _TYPE_WIDGET_TRANSLATOR:
         # Raising an exception is adapted here since it is a developer-oriented function
         raise ValueError(
-            f"{att_type}: Type already registered in type-to-widget translations"
+            f'{value_type}: Type already registered with "{_TYPE_WIDGET_TRANSLATOR[value_type]}" '
+            f"in type-to-widget translations."
         )
 
-    _TYPE_WIDGET_TRANSLATOR[att_type] = widget_type
+    _TYPE_WIDGET_TRANSLATOR[value_type] = widget_type
 
 
-def _WidgetTypeForType(att_type: constrained_type_t, /) -> Type[library_wgt_t]:
+def _WidgetTypeForType(value_type: type_t, /) -> Type[library_wgt_t]:
     """"""
     for registered_type, widget_type in _TYPE_WIDGET_TRANSLATOR.items():
-        if att_type.ContainsOrMatches(
+        if value_type.ContainsOrMatches(
             registered_type.annotations, py_type=registered_type.py_type
         ):
             return widget_type
 
     return default_entry_wgt_t
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/storage/config.py` & `conf-ini-g-2023.5/conf_ini_g/interface/storage/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,57 +25,56 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import configparser as cfpr
 import sys as sstm
 from argparse import ArgumentParser as argument_parser_t
 
-import conf_ini_g.specification.unit as unit
-from conf_ini_g.interface.storage.constant import INI_COMMENT_MARKER
-from conf_ini_g.raw.config import AsStr, any_raw_config_h, ini_config_h
-from conf_ini_g.specification.default import missing_required_value_t
-from conf_ini_g.specification.parameter import parameter_t
-from conf_ini_g.specification.section import section_t
+from conf_ini_g.raw.config import AsStr, INIConfigFromINIDocument, any_raw_config_h
+from conf_ini_g.specification.parameter.main import parameter_t
+from conf_ini_g.specification.parameter.value import missing_required_value_t
+from conf_ini_g.specification.section.main import section_t
+from conf_ini_g.specification.section.unit import IsUnitSection
 from conf_ini_g.standard.path_extension import (
     ValidateInputPath,
     ValidateOutputPath,
     any_path_h,
     path_t,
 )
-from conf_ini_g.standard.str_extension import EvaluatedValue
+from conf_ini_g.standard.str_extension import AsInterpretedObject
 
 
-INI_VALUE_ASSIGNEMENT = "="
+SECTIONS = "SECTIONS"
 
 
 def DraftSpecificationFromINIDocument(path: any_path_h, /) -> str | None:
     """"""
     ini_config = INIConfigFromINIDocument(path)
     if ini_config is None:
         return None
 
     sections = []
     for section_name, parameters in ini_config.items():
         # possibly_fuzzy=True: in case the raw config is not valid in that respect
-        if unit.IsUnitSection(section_name, possibly_fuzzy=True):
+        if IsUnitSection(section_name, possibly_fuzzy=True):
             continue
 
         parameters_as_lst = []
         for parameter_name, value_as_str in parameters.items():
-            value, _ = EvaluatedValue(value_as_str)
+            value, _ = AsInterpretedObject(value_as_str)
             py_type = type(value)
 
             parameter = (
                 f"{parameter_t.__name__}(\n"
                 f'                name="{parameter_name}",\n'
-                f"                default={missing_required_value_t.__name__}(types={py_type.__name__})\n"
+                f"                types={py_type.__name__},\n"
+                f"                default={missing_required_value_t.__name__}()\n"
                 f"            )"
             )
             parameters_as_lst.append(parameter)
 
         parameters_as_str = ",\n            ".join(parameters_as_lst)
         section = (
             f"    {section_t.__name__}(\n"
@@ -85,48 +84,24 @@
             f"        ]\n"
             f"    )"
         )
         sections.append(section)
 
     imports = (
         f"# To use this specification file:\n"
-        f"#     1. import the object SECTIONS\n"
+        f"#     1. import the object {SECTIONS}\n"
         f"#     2. instantiate a conf_ini_g.specification.config.config_t from it\n"
-        f"from conf_ini_g.specification.default import {missing_required_value_t.__name__}\n"
-        f"from conf_ini_g.specification.parameter import {parameter_t.__name__}\n"
-        f"from conf_ini_g.specification.section import {section_t.__name__}\n"
+        f"from conf_ini_g.specification.parameter.main "
+        f"import {parameter_t.__name__}\n"
+        f"from conf_ini_g.specification.parameter.value "
+        f"import {missing_required_value_t.__name__}\n"
+        f"from conf_ini_g.specification.section.main import {section_t.__name__}\n"
     )
 
-    return imports + "\nSECTIONS = (\n" + ",\n".join(sections) + ",\n)\n"
-
-
-def INIConfigFromINIDocument(path: any_path_h, /) -> ini_config_h | None:
-    """"""
-    ini_config = cfpr.ConfigParser(
-        delimiters=INI_VALUE_ASSIGNEMENT,
-        comment_prefixes=INI_COMMENT_MARKER,
-        empty_lines_in_values=False,
-        interpolation=None,
-    )
-    ini_config.optionxform = lambda option: option
-    try:
-        # Returns DEFAULT <Section: DEFAULT> if path does not exist or is a folder
-        ini_config.read(path, encoding=sstm.getfilesystemencoding())
-    except cfpr.MissingSectionHeaderError:
-        return None
-
-    output = {
-        section: {parameter: value for parameter, value in parameters.items()}
-        for section, parameters in ini_config.items()
-        if section != cfpr.DEFAULTSECT
-    }
-    if output.__len__() == 0:
-        return None
-
-    return output
+    return imports + f"\n{SECTIONS} = (\n" + ",\n".join(sections) + ",\n)\n"
 
 
 def SaveRawConfigToINIDocument(
     config: any_raw_config_h,
     path: any_path_h,
     /,
     *,
@@ -157,55 +132,55 @@
     Run with: python -m conf_ini_g.interface.storage.config
     from package base folder.
     """
     main_encoding = sstm.getfilesystemencoding()
 
     parser = argument_parser_t(
         prog="python -m conf_ini_g.interface.storage.config",
-        description="Display or save a draft config specification based on an INI file.",
+        description="Display or save a draft config specification "
+        "based on an INI file.",
         allow_abbrev=False,
     )
     # type=argparse.FileType() => automatic file opening
     parser.add_argument(
-        dest="ini_document",
+        dest="ini_path",
         help="Input: Path to INI configuration file",
         metavar="INI_config_file",
     )
     # type=argparse.FileType('w', encoding=main_encoding) => automatic creation of file
     parser.add_argument(
         dest="draft_specification",
-        help="Output: Path to draft config specification file. If not passed, specification is displayed in console.",
+        help="Output: Path to draft config specification file. "
+        "If not passed, specification is displayed in console.",
         default=None,
         nargs="?",
         metavar="draft_spec_file",
     )
     parser.add_argument(
         "--overwrite",
         dest="should_overwrite",
         action="store_true",
         help="Allows overwriting of draft config specification file.",
     )
 
     arguments = parser.parse_args()
-    ini_path = path_t(arguments.ini_document)
+    ini_path = path_t(arguments.ini_path)
     draft_path = arguments.draft_specification
     main_should_overwrite = arguments.should_overwrite
 
-    if (main_error := ValidateInputPath(ini_path)) is not None:
-        print(main_error + "\n")
+    if (issue := ValidateInputPath(ini_path)) is not None:
+        print(issue + "\n")
         parser.print_help()
         sstm.exit(-1)
 
     if draft_path is not None:
         draft_path = path_t(draft_path)
-        main_error = ValidateOutputPath(
-            draft_path, should_overwrite=main_should_overwrite
-        )
-        if main_error is not None:
-            print(main_error + "\n")
+        issue = ValidateOutputPath(draft_path, should_overwrite=main_should_overwrite)
+        if issue is not None:
+            print(issue + "\n")
             parser.print_help()
             sstm.exit(-1)
 
     draft = DraftSpecificationFromINIDocument(ini_path)
     if draft is None:
         print(f"{ini_path}: Not a valid INI document")
         sstm.exit(-1)
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/interface/storage/constant.py` & `conf-ini-g-2023.5/conf_ini_g/interface/storage/constant.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.4/conf_ini_g/light/config.py` & `conf-ini-g-2023.5/conf_ini_g/raw/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,114 +25,108 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
+import configparser as cfpr
+import sys as sstm
+from typing import Any
 
-import inspect as nspt
-from typing import Any, Callable, Sequence
+from conf_ini_g.interface.storage.constant import INI_COMMENT_MARKER
+from conf_ini_g.standard.path_extension import any_path_h
+from conf_ini_g.standard.str_extension import Flattened
 
-from conf_ini_g.standard.path_extension import any_path_h, path_t
-from conf_ini_g.standard.str_extension import AlignedNameAndValue
-from conf_ini_g.standard.type_extension import EducatedValue, Unaliased
-
-
-config_as_dict_h = dict[str, dict[str, Any]]
-
-
-class config_t:
-    path: path_t
-    base_for_relative_paths: path_t
-    _annotations: dict[str, Any]
-
-    @classmethod
-    def NewFromDictionary(
-        cls, as_dict: config_as_dict_h, /, *, path: any_path_h = None
-    ) -> config_t:
-        """
-        The dictionary values are already properly typed
-        """
-        instance = cls()
-
-        if (path is not None) and isinstance(path, str):
-            path = path_t(path)
-
-        instance.path = path
-        if path is None:
-            instance.base_for_relative_paths = path_t.home()
-        else:
-            instance.base_for_relative_paths = path.parent
-        instance._annotations = nspt.get_annotations(cls)
-
-        for s_name, section in as_dict.items():
-            for p_name, value in section.items():
-                instance.Set(_FullName(s_name, p_name), value)
-
-        return instance
-
-    def Set(self, name: str, value: Any, /) -> None:
-        """"""
-        expected_type = Unaliased(self._annotations[name])
-        educated = EducatedValue(value, expected_type, self.base_for_relative_paths)
-
-        setattr(self, name, educated)
-
-    def __str__(self) -> str:
-        """"""
-        output = []
-
-        max_name_length = 0
-        AllButCallable = lambda _elm: not isinstance(_elm, Callable)
-        for name, value in nspt.getmembers(self, AllButCallable):
-            if name[0] != "_":
-                if (current_length := name.__len__()) > max_name_length:
-                    max_name_length = current_length
-                output.append(_FormattedNameAndValue(name, value))
-        output = map(
-            lambda _elm: AlignedNameAndValue(_elm, max_name_length + 1), output
-        )
 
-        return "\n".join(output)
+ini_config_h = dict[str, dict[str, str]]  # Without value interpretation
+raw_config_h = dict[str, dict[str, Any]]  # With interpreted values, and possibly units
+any_raw_config_h = ini_config_h | raw_config_h
 
 
-def _FullName(section: str, parameter: str, /) -> str:
-    """"""
-    return f"{section.strip().lower().replace(' ', '_')}_{parameter.strip().lower()}"
+INI_VALUE_ASSIGNMENT = "="
 
 
-def _FormattedNameAndValue(name: str, value: Any, /) -> str:
+def INIConfigFromINIDocument(
+    path: any_path_h,
+    /,
+    *,
+    arguments: raw_config_h = None,
+) -> ini_config_h | None:
     """"""
-    if value is None:
-        as_str = "None"
-    elif isinstance(value, bool):
-        as_str = str(value)
-    elif isinstance(value, str):
-        as_str = f'"{value}"'
-    elif isinstance(value, path_t):
-        as_str = f"💻{value}"
-    else:
-        as_str = _FormattedValue(value)
+    ini_config = cfpr.ConfigParser(
+        delimiters=INI_VALUE_ASSIGNMENT,
+        comment_prefixes=INI_COMMENT_MARKER,
+        empty_lines_in_values=False,
+        interpolation=None,
+    )
+    ini_config.optionxform = lambda option: option
+    try:
+        # Returns DEFAULT <Section: DEFAULT> if path does not exist or is a folder
+        ini_config.read(path, encoding=sstm.getfilesystemencoding())
+    except cfpr.MissingSectionHeaderError:
+        return None
+
+    output = {
+        section: {parameter: value for parameter, value in parameters.items()}
+        for section, parameters in ini_config.items()
+        if section != cfpr.DEFAULTSECT
+    }
+    if arguments is not None:
+        for sct_name, parameters in arguments.items():
+            if sct_name not in output:
+                output[sct_name] = {}
+            for prm_name, value in parameters.items():
+                output[sct_name][prm_name] = value
 
-    return f"{name} = {as_str}"
+    if output.__len__() == 0:
+        return None
+
+    return output
 
 
-def _FormattedValue(value: Any, /, *, level: int = 0) -> str:
+def AsStr(config: any_raw_config_h, /, *, in_html_format: bool = False) -> str:
     """"""
-    if value is None:
-        output = "None"
-    elif isinstance(value, bool):
-        output = str(value)
-    elif isinstance(value, str):
-        output = f'"{value}"'
-    elif isinstance(value, path_t):
-        output = f"💻{value}"
-    elif isinstance(value, Sequence):
-        output = ", ".join(_FormattedValue(_vle, level=level + 1) for _vle in value)
-        if level > 0:
-            output = f"({output})"
+    output = []
+
+    if in_html_format:
+        section_color = '<span style="color:green">'
+        parameter_color = '<span style="color:blue">'
+        color_reset = "</span>"
+        newline = "<br/>"
+        indentation = "&nbsp;"
     else:
-        output = f"{value}:{type(value).__name__}"
+        section_color = "[green]"
+        parameter_color = "[blue]"
+        color_reset = "[/]"
+        newline = "\n"
+        indentation = " "
+
+    longest = 0
+    for section, parameters in config.items():
+        if parameters.__len__() == 0:
+            continue
+
+        inner_output = []
+        lengths = []
+        for name, value in parameters.items():
+            length = name.__len__()
+            lengths.append(length)
+            longest = max(longest, length)
 
-    return output
+            flattened = Flattened(str(value))
+            inner_output.append(f"{parameter_color}{name}{color_reset}@= {flattened}")
+
+        output.append(
+            (f"{section_color}[{section}]{color_reset}", inner_output, lengths)
+        )
+
+    output = (
+        f"{_sct}{newline}"
+        + newline.join(
+            _lne.replace("@", (longest - _lgt + 1) * indentation, 1)
+            for _lne, _lgt in zip(_prm, _lgs)
+        )
+        for _sct, _prm, _lgs in output
+    )
+
+    return f"{newline}{newline}".join(output)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/light/conversion.py` & `conf-ini-g-2023.5/conf_ini_g/light/conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from configparser import ConfigParser as config_parser_t
 
 from openpyxl import Workbook as workbook_t
 
 from conf_ini_g.light.ini import NewConfigFromPath as NewConfigFromINIPath
 from conf_ini_g.light.xlsx import NewConfigFromPath as NewConfigFromXLSXPath
 from conf_ini_g.standard.path_extension import any_path_h, path_t
-from conf_ini_g.standard.type_extension import EducatedString
 
 
 def INItoXLSX(
     ini_path: any_path_h, xlsx_path: any_path_h, /, *, should_overwrite: bool = False
 ) -> None:
     """"""
     ini_path, xlsx_path = _AsPaths(ini_path, xlsx_path)
@@ -52,29 +51,29 @@
     # Remove the (a priori unique) default worksheet
     for worksheet in workbook.sheetnames:
         # The "remove" method is for worksheets, not names. Use this instead:
         del workbook[worksheet]
     for sct_name, content in config.items():
         worksheet = workbook.create_sheet(title=sct_name)
         for prm_name, value in content.items():
-            worksheet.append((prm_name, EducatedString(value)))
+            worksheet.append((prm_name, str(value)))
 
     workbook.save(xlsx_path)
 
 
 def XLSXtoINI(
     xlsx_path: any_path_h, ini_path: any_path_h, /, *, should_overwrite: bool = False
 ) -> None:
     """"""
     ini_path, xlsx_path = _AsPaths(ini_path, xlsx_path)
     _CheckOverwriting(ini_path, should_overwrite)
 
     config_as_dict = NewConfigFromXLSXPath(xlsx_path)
     config_as_dict = {
-        _sct: {_prm: EducatedString(_vle) for _prm, _vle in _ctn.items()}
+        _sct: {_prm: str(_vle) for _prm, _vle in _ctn.items()}
         for _sct, _ctn in config_as_dict.items()
     }
 
     config = config_parser_t()
     config.optionxform = lambda option: option  # To avoid automatic lowercasing
     config.read_dict(config_as_dict)
     with open(ini_path, "w") as accessor:
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/light/ini.py` & `conf-ini-g-2023.5/conf_ini_g/light/ini.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,36 +28,38 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from configparser import ConfigParser as config_t
 from configparser import ExtendedInterpolation
 
-from conf_ini_g.light.config import config_as_dict_h
+from conf_ini_g.raw.config import ini_config_h
 from conf_ini_g.standard.path_extension import any_path_h
-from conf_ini_g.standard.str_extension import ConvertedValue
 
 
 _DEFAULT_OPTIONS = (
     ("delimiters", ("=",)),
     ("comment_prefixes", ("#",)),
     ("inline_comment_prefixes", ("#",)),
     ("interpolation", ExtendedInterpolation()),
 )
 
 
-def NewConfigFromPath(path: any_path_h, /, **kwargs) -> config_as_dict_h:
+def NewConfigFromPath(path: any_path_h, /, **kwargs) -> ini_config_h:
     """"""
     options = kwargs.copy()
     for name, value in _DEFAULT_OPTIONS:
         if name not in options:
             options[name] = value
 
     config = config_t(**options)
     config.optionxform = lambda option: option  # To avoid automatic lowercasing
     config.read(path)
 
     # config.sections(): Does not include the default section named configparser.DEFAULTSECT
-    return {
-        _nme: {_prm: ConvertedValue(_vle) for _prm, _vle in config[_nme].items()}
-        for _nme in config.sections()
-    }
+    return {_nme: dict(config[_nme]) for _nme in config.sections()}
+    # return {
+    #     _nme: {
+    #         _prm: _vle for _prm, _vle in config[_nme].items()
+    #     }
+    #     for _nme in config.sections()
+    # }
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/light/xlsx.py` & `conf-ini-g-2023.5/conf_ini_g/light/xlsx.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,26 +27,25 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from openpyxl import load_workbook as WorkbookFromPath
 
-from conf_ini_g.light.config import config_as_dict_h
+from conf_ini_g.raw.config import ini_config_h
 from conf_ini_g.standard.path_extension import any_path_h
-from conf_ini_g.standard.str_extension import ConvertedValue
 
 
-def NewConfigFromPath(path: any_path_h, /) -> config_as_dict_h:
+def NewConfigFromPath(path: any_path_h, /) -> ini_config_h:
     """"""
     output = {}
 
     workbook = WorkbookFromPath(filename=path)
     for name in workbook.sheetnames:
         sheet = workbook[name]
         contents = {}
         for row in tuple(sheet.rows):
-            contents[row[0].value] = ConvertedValue(row[1].value)
+            contents[row[0].value] = row[1].value
 
         output[name] = contents
 
     return output
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/raw/config.py` & `conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/choices.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,66 +25,44 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Any
+import dataclasses as dtcl
+from typing import Annotated, ClassVar, Sequence
 
-import colorama as clrm
-
-from conf_ini_g.standard.str_extension import Flattened
-
-
-# Straight from the INI document, without value interpretation
-ini_config_h = dict[str, dict[str, str]]
-raw_config_h = dict[str, dict[str, Any]]  # With interpreted values
-any_raw_config_h = ini_config_h | raw_config_h
-
-
-def AsStr(config: any_raw_config_h, /, *, in_html_format: bool = False) -> str:
-    """"""
-    output = []
-
-    if in_html_format:
-        section_color = '<span style="color:green">'
-        parameter_color = '<span style="color:blue">'
-        color_reset = "</span>"
-        newline = "<br/>"
-        indentation = "&nbsp;"
-    else:
-        section_color = clrm.Fore.GREEN
-        parameter_color = clrm.Fore.BLUE
-        color_reset = clrm.Fore.RESET
-        newline = "\n"
-        indentation = " "
-
-    longest = 0
-    for section, parameters in config.items():
-        if parameters.__len__() == 0:
-            continue
-
-        inner_output = []
-        lengths = []
-        for name, value in parameters.items():
-            length = name.__len__()
-            lengths.append(length)
-            longest = max(longest, length)
-
-            flattened = Flattened(str(value))
-            inner_output.append(f"{parameter_color}{name}{color_reset}@= {flattened}")
-
-        output.append(
-            (f"{section_color}[{section}]{color_reset}", inner_output, lengths)
-        )
-
-    output = (
-        f"{_sct}{newline}"
-        + newline.join(
-            _lne.replace("@", (longest - _lgt + 1) * indentation, 1)
-            for _lne, _lgt in zip(_prm, _lgs)
-        )
-        for _sct, _prm, _lgs in output
-    )
-
-    return f"{newline}{newline}".join(output)
+from conf_ini_g.specification.parameter.annotation import (
+    annotation_t,
+    py_type_options_h,
+)
+from conf_ini_g.standard.type_extension import annotated_hint_t
+
+
+@dtcl.dataclass(repr=False, eq=False)
+class choices_t(annotation_t):
+    VALID_PY_TYPES: ClassVar[py_type_options_h] = str
+
+    options: Sequence[str] = None
+
+    @classmethod
+    def NewAnnotatedType(cls, options: Sequence[str], /) -> annotated_hint_t:
+        """"""
+        return Annotated[cls.VALID_PY_TYPES, cls(tuple(options))]
+
+    def Issues(self, py_type: type, /) -> list[str]:
+        """"""
+        output = super().Issues(py_type)
+
+        for option in self.options:
+            if not isinstance(option, str):
+                output.append(
+                    f"{type(option).__name__}: Invalid type of option {option} "
+                    f"in {self}; Expected=str"
+                )
+
+        return output
+
+    def ValueIsCompliant(self, value: str, /) -> bool:
+        """"""
+        return value in self.options
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/specification/constant.py` & `conf-ini-g-2023.5/conf_ini_g/specification/parameter/value.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,26 +25,38 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import string as strg
 
+class missing_required_value_t:
+    TEXT = "MISSING REQUIRED VALUE"
 
-UNIT_SECTION = "UNITS"  # In uppercase
-UNIT_SEPARATOR = "'"
+    def __str__(self) -> str:
+        """"""
+        return self.__class__.TEXT
 
-PARAMETER_WORD_SEPARATOR = "_"
-VALID_CHARACTERS = strg.ascii_letters + strg.digits + PARAMETER_WORD_SEPARATOR
+    def __rich__(self) -> str:
+        """"""
+        return f"[red]{self.__class__.TEXT}[/]"
 
-MOD_ELM_SEPARATOR = ":"
 
-STD_ABBREVIATIONS = {
-    "fct": "function",
-    "mod": "module",
-    "n": "number of",
-    "o": "of",
-    "prm": "parameter",
-    "rng": "range",
-}
+class invalid_value_t:
+    """
+    Do not use invalid_value_t = object, for example, otherwise isinstance returns True for anything.
+    """
+
+    TEXT = "INVALID VALUE"
+
+    def __str__(self) -> str:
+        """"""
+        return self.__class__.TEXT
+
+    def __rich__(self) -> str:
+        """"""
+        return f"[red]{self.__class__.TEXT}[/]"
+
+
+MISSING_REQUIRED_VALUE = missing_required_value_t()
+INVALID_VALUE = invalid_value_t()
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/specification/constrained_type.py` & `conf-ini-g-2023.5/conf_ini_g/specification/parameter/type.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,99 +28,75 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 import dataclasses as dtcl
-from conf_ini_g.standard.path_extension import path_t as pl_path_t
 from typing import Annotated, Any, Sequence
 
-import colorama as clrm
+from rich.text import Text as text_t
 
-from conf_ini_g.specification.constraint import (
-    boolean_t,
-    choices_t,
-    constraint_t,
-    number_t,
-    path_t,
-    sequence_t,
-)
-from conf_ini_g.standard.str_extension import EvaluatedValue
+from conf_ini_g.catalog.specification.parameter.boolean import boolean_t
+from conf_ini_g.catalog.specification.parameter.choices import choices_t
+from conf_ini_g.catalog.specification.parameter.number import number_t
+from conf_ini_g.catalog.specification.parameter.path import path_t
+from conf_ini_g.catalog.specification.parameter.sequence import sequence_t
+from conf_ini_g.specification.parameter.annotation import annotation_t
+from conf_ini_g.specification.parameter.value import INVALID_VALUE
+from conf_ini_g.standard.path_extension import path_t as pl_path_t
+from conf_ini_g.standard.str_extension import AsInterpretedObject
 from conf_ini_g.standard.type_extension import (
     FAKE_TYPE_ANNOTATION,
     AnnotationsOfType,
     PythonTypeOfAnnotated,
-    annotated_type_t,
-    any_type_and_none_h,
+    annotated_hint_t,
+    any_hint_h,
     none_t,
 )
 
 
-any_annotation_h = constraint_t | Any
-
-
-# Do not use _invalid_value_t = object, for example, otherwise isinstance returns True for anything
-class _invalid_value_t:
-    """"""
-
-    def __str__(self) -> str:
-        """"""
-        return f"{clrm.Fore.RED}INVALID VALUE{clrm.Fore.RESET}"
-
-
-INVALID_VALUE = _invalid_value_t()
-
-
 @dtcl.dataclass(repr=False, eq=False)
-class constrained_type_t:
-
+class type_t:
     py_type: type = None
-    annotations: Sequence[any_annotation_h] = None
+    annotations: Sequence[annotation_t] = None
 
     @classmethod
-    def NewFromType(cls, type_: any_type_and_none_h, /) -> constrained_type_t:
-        """"""
+    def NewFromType(cls, type_: any_hint_h | None, /) -> type_t:
+        """
+        type_: Can be None if None is accepted as a value for a parameter.
+        """
         if isinstance(type_, (type, none_t)):
             type_ = Annotated[type_, FAKE_TYPE_ANNOTATION]
-        # else: must be annotated_type_t
 
         return cls.NewFromAnnotatedType(type_)
 
     @classmethod
-    def NewFromAnnotatedType(
-        cls, annotated_type: annotated_type_t, /
-    ) -> constrained_type_t:
+    def NewFromAnnotatedType(cls, annotated_type: annotated_hint_t, /) -> type_t:
         """"""
-        instance = cls()
+        output = cls()
 
-        instance.py_type = PythonTypeOfAnnotated(annotated_type)
-        instance.annotations = AnnotationsOfType(annotated_type)
+        output.py_type = PythonTypeOfAnnotated(annotated_type)
+        output.annotations = AnnotationsOfType(annotated_type)
 
-        return instance
+        return output
 
-    def Issues(self, name: str, section: str, /) -> Sequence[str]:
+    def Issues(self) -> list[str]:
         """"""
         output = []
 
-        # self.annotations.__len__() == 0 is OK. It means that there was only a fake annotation, which has been
-        # discarded by AnnotationsOfType.
         py_type = self.py_type
         for annotation in self.annotations:
-            if hasattr(annotation, "Issues"):
-                output.extend(annotation.Issues(py_type, name, section))
-            # This was once considered an issue, but it probably isn't
-            # else:
-            #     output.append(f'{annotation}: Annotation has no "Issues" method')
+            output.extend(f"[{self}] {_iss}" for _iss in annotation.Issues(py_type))
 
         return output
 
     def ContainsOrMatches(
         self,
-        expected_annotation: any_annotation_h | Sequence[any_annotation_h],
+        expected_annotation: annotation_t | Sequence[annotation_t],
         /,
         *,
         py_type: type = None,
         full: bool = False,
     ) -> bool:
         """"""
         if (py_type is not None) and (self.py_type is not py_type):
@@ -129,15 +105,16 @@
         ref_types = tuple(type(_nnt) for _nnt in self.annotations)
         if isinstance(expected_annotation, Sequence):
             expected_annotations = expected_annotation
         else:
             expected_annotations = (expected_annotation,)
 
         if full:
-            # Comparing the iterators returns False, hence the conversions to lists (through sorted, which is necessary)
+            # Comparing the iterators returns False, hence the conversions to lists
+            # (through sorted, which is necessary).
             type_name = lambda _elm: _elm.__name__
             ref_types = sorted(ref_types, key=type_name)
             expected_types = sorted(
                 (type(_nnt) for _nnt in expected_annotations), key=type_name
             )
 
             return ref_types == expected_types
@@ -145,163 +122,163 @@
             n_founds = 0
             for annotation in expected_annotations:
                 if isinstance(annotation, ref_types):
                     n_founds += 1
 
             return n_founds == expected_annotations.__len__()
 
-    def FirstConstraintWithAttribute(
+    def FirstAnnotationWithAttribute(
         self, attribute: str | Sequence[str], /
-    ) -> any_annotation_h | None:
+    ) -> annotation_t | None:
         """"""
         # Do not test isinstance(attribute, Sequence) since str is a sequence
         if isinstance(attribute, str):
             attributes = (attribute,)
         else:
             attributes = attribute
 
         for annotation in self.annotations:
             if all(hasattr(annotation, _ttr) for _ttr in attributes):
                 return annotation
 
         return None
 
-    def TypedValue(self, value: Any, /) -> tuple[Any | None, bool]:
+    def ValueIsCompliant(self, value: Any, /) -> bool:
         """"""
-        failed_conversion = None, False
+        return isinstance(value, self.py_type) and all(
+            _nnt.ValueIsCompliant(value) for _nnt in self.annotations
+        )
 
+    def TypedValue(self, value: Any, /) -> tuple[Any | None, bool]:
+        """"""
         if isinstance(value, self.py_type):
-            typed_value, success = value, True
-        elif isinstance(value, str):
-            typed_value, success = EvaluatedValue(value, expected_type=self.py_type)
-        else:
-            return failed_conversion
+            return value, True
 
-        if success:
-            for annotation in self.annotations:
-                if hasattr(annotation, "ValueIsValid") and not annotation.ValueIsValid(
-                    typed_value
-                ):
-                    return failed_conversion
-
-            return typed_value, True
+        if isinstance(value, str):
+            typed_value, success = AsInterpretedObject(
+                value, expected_type=self.py_type
+            )
+            if success and self.ValueIsCompliant(typed_value):
+                return typed_value, True
 
-        return failed_conversion
+        return INVALID_VALUE, False
 
     def __str__(self) -> str:
         """"""
+        return text_t.from_markup(self.__rich__()).plain
+
+    def __rich__(self) -> str:
+        """"""
         if self.py_type is none_t:
             type_name = "None"
         else:
             type_name = self.py_type.__name__
-        output = [f"{clrm.Fore.CYAN}{type_name}{clrm.Fore.RESET}"]
+        output = [f"[blue]{type_name}[/]"]
 
         for annotation in self.annotations:
-            output.append(str(annotation))
+            output.append(type(annotation).__name__)
 
-        return " ->\n".join(output)
+        return "&".join(output)
 
 
 @dtcl.dataclass(init=False, repr=False, eq=False)
-class constrained_types_t(list):
+class type_options_t(list[type_t]):
     """"""
 
     @classmethod
-    def NewFromTypes(
-        cls, types: Sequence[any_type_and_none_h], /
-    ) -> constrained_types_t:
+    def NewFromTypes(cls, any_types: Sequence[any_hint_h | None], /) -> type_options_t:
         """"""
-        instance = cls()
+        output = cls()
 
         idx_o_none = 0
-        for t_idx, type_ in enumerate(types):
-            cstd_type = constrained_type_t.NewFromType(type_)
-            instance.append(cstd_type)
-            if cstd_type.py_type is none_t:
+        for t_idx, any_type in enumerate(any_types):
+            type_ = type_t.NewFromType(any_type)
+            output.append(type_)
+            if type_.py_type is none_t:
                 idx_o_none = t_idx
 
         if idx_o_none > 0:
-            keep = instance[idx_o_none]
-            del instance[idx_o_none]
-            instance.insert(0, keep)
+            keep = output[idx_o_none]
+            del output[idx_o_none]
+            output.insert(0, keep)
 
-        return instance
+        return output
 
     @property
     def n_types(self) -> int:
         """"""
         return self.__len__()
 
-    def Issues(self, name: str, section: str, /) -> Sequence[str]:
+    def Issues(self) -> list[str]:
         """"""
         output = []
 
         if self.n_types == 0:
-            output.append(f"{section}/{name}: Empty list of allowed types")
+            output.append(f"{self}: Empty list of allowed types")
         else:
             if (self.n_types == 1) and self.AllowsNone():
-                output.append(
-                    f'{self}: None cannot be the only allowed type of the optional parameter "{section}/{name}"'
-                )
+                output.append(f"{self}: None cannot be the only allowed type")
             n_nones = 0
             for cstd_type in self:
                 if cstd_type.py_type is none_t:
                     n_nones += 1
                 else:
-                    output.extend(cstd_type.Issues(name, section))
+                    output.extend(f"[{self}] {_iss}" for _iss in cstd_type.Issues())
             if n_nones > 1:
-                output.append(
-                    f'{self}: None cannot be mentioned more than once for parameter "{section}/{name}"'
-                )
+                output.append(f"{self}: None cannot be mentioned more than once")
 
         return output
 
     def AllowsNone(self) -> bool:
         """"""
         return self[0].py_type is none_t
 
-    def MatchingTypeOf(self, py_type: type, /) -> constrained_type_t:
+    def MatchingTypeOf(self, value: Any, /) -> type_t:
         """"""
         output = None
 
         for cstd_type in self:
-            if cstd_type.py_type is py_type:
+            if isinstance(value, cstd_type.py_type):
                 output = cstd_type
                 break
 
         return output
 
-    def TypedValue(self, value: str, /) -> tuple[Any, constrained_type_t | None]:
+    def ValueIsCompliant(self, value: Any, /) -> bool:
+        """"""
+        return any(_tpe.ValueIsCompliant(value) for _tpe in self)
+
+    def TypedValueAndType(self, value: str, /) -> tuple[Any, type_t | None]:
         """"""
-        typed_value = None
+        typed_value = INVALID_VALUE
         type_spec = None
 
-        success = False
-        for cstd_type in self:
-            typed_value, success = cstd_type.TypedValue(value)
+        for type_ in self:
+            typed_value, success = type_.TypedValue(value)
             if success:
-                type_spec = cstd_type
+                type_spec = type_
                 break
 
-        if not success:
-            typed_value = INVALID_VALUE
-
         return typed_value, type_spec
 
     def __str__(self) -> str:
         """"""
-        output = (str(_typ) for _typ in self)
+        return text_t.from_markup(self.__rich__()).plain
+
+    def __rich__(self) -> str:
+        """"""
+        output = (_typ.__rich__() for _typ in self)
 
-        return " +\n".join(output)
+        return " + ".join(output)
 
 
-SIMPLE_ATT_TYPES: dict[str, constrained_type_t] = {
-    "boolean": constrained_type_t.NewFromAnnotatedType(Annotated[bool, boolean_t()]),
-    "float": constrained_type_t.NewFromAnnotatedType(Annotated[float, number_t()]),
-    "int": constrained_type_t.NewFromAnnotatedType(Annotated[int, number_t()]),
-    "choices": constrained_type_t.NewFromAnnotatedType(Annotated[str, choices_t()]),
-    "path": constrained_type_t.NewFromAnnotatedType(Annotated[pl_path_t, path_t()]),
-    "sequence": constrained_type_t.NewFromAnnotatedType(Annotated[tuple, sequence_t()]),
-    "None": constrained_type_t.NewFromAnnotatedType(
-        Annotated[None, FAKE_TYPE_ANNOTATION]
+BASIC_TYPES: dict[str, type_t] = {
+    "boolean": type_t.NewFromAnnotatedType(Annotated[bool, boolean_t()]),
+    "float": type_t.NewFromAnnotatedType(Annotated[float, number_t()]),
+    "int": type_t.NewFromAnnotatedType(Annotated[int, number_t()]),
+    "choices": type_t.NewFromAnnotatedType(Annotated[str, choices_t()]),
+    "path": type_t.NewFromAnnotatedType(
+        Annotated[pl_path_t, path_t(target_type=path_t.TARGET_TYPE.any, is_input=True)]
     ),
+    "sequence": type_t.NewFromAnnotatedType(Annotated[tuple, sequence_t()]),
+    "None": type_t.NewFromAnnotatedType(Annotated[None, FAKE_TYPE_ANNOTATION]),
 }
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/specification/generic.py` & `conf-ini-g-2023.5/conf_ini_g/specification/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,57 +26,50 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
-from typing import Any
+import string as strg
 
-import colorama as clrm
+from rich.text import Text as text_t
 
-from conf_ini_g.specification.constant import VALID_CHARACTERS
-from conf_ini_g.standard.dtcl_extension import AsStr
+
+WORD_SEPARATOR = "_"
+VALID_CHARACTERS = strg.ascii_letters + strg.digits + WORD_SEPARATOR
 
 
 @dtcl.dataclass(repr=False, eq=False)
-class generic_t:
+class base_t:
     name: str
     definition: str = "No Definition Provided"
     description: str = "No Description Provided"
     basic: bool = True
 
-    def AsDict(self) -> dict[str, Any]:
-        """"""
-        return dtcl.asdict(self)
-
-    def Issues(self, /, *, context: str = None) -> list[str]:
+    def Issues(self) -> list[str]:
         """"""
         output = []
 
-        if context is None:
-            context = ""
-        else:
-            context = f' in "{context}"'
-
         if any(_chr not in VALID_CHARACTERS for _chr in self.name):
             output.append(
-                f"{self.name}: Name{context} contains invalid characters; "
+                f"{self.name}: Name contains invalid characters; "
                 f"Valid={VALID_CHARACTERS}"
             )
         if not isinstance(self.definition, str):
             output.append(
-                f'{self.definition}: Not a valid string for definition of "{self.name}"{context}'
+                f'{self.definition}: Not a valid string for definition of "{self.name}"'
             )
         if not isinstance(self.description, str):
             output.append(
-                f'{self.description}: Not a valid string for description of "{self.name}"{context}'
+                f'{self.description}: Not a valid string for description of "{self.name}"'
             )
 
         return output
 
     def __str__(self) -> str:
         """"""
-        return AsStr(self)
-
+        return text_t.from_markup(self.__rich__()).plain
 
-clrm.init()
+    def __rich__(self) -> str:
+        """"""
+        return f"[blue]Name[/]@=@{self.name}\n[blue]Basic[/]@=@{self.basic}"
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/specification/section.py` & `conf-ini-g-2023.5/conf_ini_g/specification/section/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,89 +25,124 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+from __future__ import annotations
+
 import dataclasses as dtcl
 import itertools as ittl
 import textwrap as text
 from typing import Any
 from typing import NamedTuple as named_tuple_t
 from typing import Sequence
 
-from conf_ini_g.specification.generic import generic_t
-from conf_ini_g.specification.parameter import parameter_t
+from rich.text import Text as text_t
+
+from conf_ini_g.specification.base import base_t
+from conf_ini_g.specification.parameter.main import parameter_t
+from conf_ini_g.specification.parameter.unit import unit_t
+from conf_ini_g.specification.section.unit import IsUnitSection
+from conf_ini_g.standard.str_extension import AlignedOnSeparator
+from conf_ini_g.standard.type_extension import UNIVERSAL_ANNOTATED_TYPES, TypeAsRichStr
+
+
+PARAMETERS = "parameters"
 
 
-@dtcl.dataclass(init=False, repr=False, eq=False)
+@dtcl.dataclass(init=False, repr=False, eq=False)  # Cannot have __init__ method
 class controller_t(named_tuple_t):
     section: str = None
     parameter: str = None
-    # All controller values are equal in role. However, this one is called primary because it refers to the parameters
-    # of the section, as opposed to the parameters in the alternatives.
+    # All controller values are equal in role. However, this one is called primary
+    # because it refers to the parameters of the section, as opposed to the parameters
+    # in the alternatives.
     primary_value: Any = None
 
+    def __str__(self) -> str:
+        """"""
+        return text_t.from_markup(self.__rich__()).plain
+
+    def __rich__(self) -> str:
+        """"""
+        return (
+            f"[magenta]{type(self).__name__}[/]: "
+            f"[blue]{self.section}.{self.parameter}[/]={self.primary_value}"
+        )
 
-@dtcl.dataclass(init=False, repr=False, eq=False)
-class section_t(generic_t, list[parameter_t]):
 
+@dtcl.dataclass(repr=False, eq=False)
+class section_t(base_t, list[parameter_t]):
     category: str = "Main"
     optional: bool = False
-    accept_unknown_parameters: bool = False
+    is_growable: bool = False
     controller: controller_t = None
-    alternatives: dict[Any, list[parameter_t]] = None
-    # Cannot be None as Python prohibits indexing by None
-    controller_value: Any = None
-
-    def __init__(self, *_, **kwargs) -> None:
-        """"""
-        list.__init__(self, kwargs.get("parameters", []))
-
-        attributes = tuple(_fld.name for _fld in dtcl.fields(section_t))
-        arguments = {_key: _val for _key, _val in kwargs.items() if _key in attributes}
-        for name, value in arguments.items():
-            setattr(self, name, value)
+    alternatives: dict[str, list[parameter_t]] = None
+    parameters: list[parameter_t] | None = None  # Used only during instantiation.
+
+    def __post_init__(self) -> None:
+        """"""
+        if self.parameters is not None:
+            self.extend(self.parameters)
+            self.parameters = None
+
+    def AddUnspecifiedParameter(self, name: str, /) -> parameter_t:
+        """
+        For programmatic use
+        """
+        if IsUnitSection(self.name):
+            parameter = unit_t(
+                name=name,
+                definition="Unit definition",
+                basic=True,
+            )
+        else:
+            parameter = parameter_t(
+                name=name,
+                definition="Programmatic parameter",
+                description="This parameter is not part of the specification. "
+                "It was added programmatically because it was found in the INI document or "
+                "passed as a command-line argument",
+                basic=self.basic,
+                types=UNIVERSAL_ANNOTATED_TYPES,
+                default=None,
+            )
+        self.append(parameter)
+
+        return parameter
 
     @property
     def all_parameters(self) -> Sequence[parameter_t]:
         """"""
         if self.alternatives is None:
             return self
         else:
             return tuple(ittl.chain(self, *self.alternatives.values()))
 
-    @property
-    def active_parameters(self) -> list[parameter_t]:
+    def ActiveParameters(self, controller_value: str, /) -> Sequence[parameter_t]:
         """"""
-        # The test self.controller_value is None avoids querying self.alternatives with None, which is forbidden by
-        # Python. This could happen if the config has not been fully activated, which should be avoided, but do happen
-        # when instantiating a command-line parser for example (other cases?)
-        if (
-            (self.controller is None)
-            or (self.controller_value == self.controller.primary_value)
-            or (self.controller_value is None)
-        ):
+        if controller_value == self.controller.primary_value:
             return self
         else:
-            return self.alternatives[self.controller_value]
+            return self.alternatives[controller_value]
 
     @property
     def controlling_values(self) -> Sequence[Any]:
         """
-        Call only on controlled sections
+        No check of controlled status; Call with care.
         """
         return (self.controller.primary_value,) + tuple(self.alternatives.keys())
 
-    def Issues(self, /, *, context: str = None) -> Sequence[str]:
+    def Issues(self) -> list[str]:
         """"""
         output = super().Issues()
 
-        valid_name_sets = [tuple(_prm.name for _prm in super().__iter__())]
+        valid_name_sets = [tuple(_prm.name for _prm in self)]
         if self.alternatives is not None:
             for parameters in self.alternatives.values():
                 valid_name_sets.append(tuple(_prm.name for _prm in parameters))
         for valid_name_set in valid_name_sets:
             if valid_name_set.__len__() > set(valid_name_set).__len__():
                 output.append(
                     f"{self.name}: Section with repeated parameter names (possibly in alternatives)"
@@ -121,32 +156,32 @@
 
         if (self.controller is None) and (not optional) and (self.__len__() == 0):
             output.append(f"{self.name}: Empty mandatory section")
 
         n_parameters = 0
         n_basic_prms = 0
         for parameter in self.all_parameters:
-            output.extend(parameter.Issues(section=self.name))
+            output.extend(f"[{self.name}] {_iss}" for _iss in parameter.Issues())
 
             n_parameters += 1
             if parameter.basic:
                 n_basic_prms += 1
 
             if parameter.basic and not basic:
                 output.append(
-                    f"{parameter.name}: Basic parameter in advanced section {self.name}"
+                    f'{parameter.name}: Basic parameter in advanced section "{self.name}"'
                 )
             if optional and not parameter.optional:
                 output.append(
-                    f"{parameter.name}: Mandatory parameter in optional section {self.name}"
+                    f'{parameter.name}: Mandatory parameter in optional section "{self.name}"'
                 )
 
-        if (n_parameters == 0) and not self.accept_unknown_parameters:
+        if (n_parameters == 0) and not self.is_growable:
             output.append(
-                f"{self.name}: Section without specified parameters which does not accept unknown parameters"
+                f"{self.name}: Section without specified parameters which does not accept unspecified parameters"
             )
         if basic and (n_parameters > 0) and (n_basic_prms == 0):
             output.append(f"{self.name}: Basic section without any basic parameters")
 
         control = (self.controller, self.alternatives)
         if any(_elm is None for _elm in control) and any(
             _elm is not None for _elm in control
@@ -166,45 +201,54 @@
                 if not parameter.optional:
                     output.append(
                         f'{parameter.name}: Mandatory parameter in controlled section "{self.name}"'
                     )
 
         return output
 
-    def AddParameter(self, parameter: parameter_t) -> None:
-        """
-        For programmatic use
-        """
-        self.active_parameters.append(parameter)
-
-    def _Item(self, key: str | int) -> parameter_t | None:
+    def _Item(self, key: str | int, /) -> parameter_t | None:
         """"""
-        if isinstance(key, str):
-            for parameter in self.active_parameters:
-                if key == parameter.name:
-                    return parameter
-        else:
-            for parameter in self.active_parameters:
-                if ((actual := parameter.actual) is not None) and (key == actual.uid):
-                    return parameter
+        if isinstance(key, int):
+            return list.__getitem__(self, key)
+
+        for parameter in self.all_parameters:
+            if parameter.name == key:
+                return parameter
 
         return None
 
-    def __contains__(self, key: str | int) -> bool:
+    def __contains__(self, key: str, /) -> bool:
         """"""
         return self._Item(key) is not None
 
-    def __getitem__(self, key: str | int) -> parameter_t:
+    def __getitem__(self, key: str | int, /) -> parameter_t:
         """"""
         item = self._Item(key)
         if item is None:
-            raise KeyError(f"{key}: Not a parameter of section {self.name}")
+            raise KeyError(f"{key}: Not a parameter of section {self.name}.")
 
         return item
 
-    def __str__(self) -> str:
+    def __rich__(self) -> str:
         """"""
-        parameters = (str(_prm) for _prm in self)
-        parameters = "\n".join(parameters)
-        parameters = text.indent(parameters, "    ")
+        output = [
+            TypeAsRichStr(self),
+            *text.indent(super().__rich__(), "    ").splitlines(),
+            f"    [blue]Category[/]@=@{self.category}",
+            f"    [blue]Optional[/]@=@{self.optional}",
+            f"    [blue]Growable[/]@=@{self.is_growable}",
+        ]
+
+        if has_controller := (self.controller is not None):
+            output.append(f"    [blue]Controller[/]@=@{self.controller}")
+
+        output.extend(text.indent(_prm.__rich__(), "    ") for _prm in self)
+        if has_controller:
+            output.append("    With alternatives:")
+            for ctl_name, parameters in self.alternatives.items():
+                output.append(f"        {ctl_name}")
+                for parameter in parameters:
+                    output.append(text.indent(parameter.__rich__(), "            "))
+
+        output = AlignedOnSeparator(output, "@=@", " = ")
 
-        return f"{super().__str__()}\n{parameters}"
+        return "\n".join(output)
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/specification/unit.py` & `conf-ini-g-2023.5/conf_ini_g/specification/parameter/unit.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,19 +25,25 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+import dataclasses as dtcl
 from math import pi as PI
+from typing import Annotated
 
-from conf_ini_g.specification.constant import UNIT_SECTION
+from conf_ini_g.catalog.specification.parameter.number import number_in_str_t
+from conf_ini_g.specification.parameter.main import parameter_t
+from conf_ini_g.specification.parameter.type import type_options_t
 
 
+UNIT_SEPARATOR = "'"
+
 _STD_UNIT_CONVERSIONS = (
     # unit, unit name, parent unit (None if none), conversion factor (1.0 if None)
     ("si", "site", None, 1.0),  # Synonym for sample, pixel, voxel...
     #
     ("km", "kilometer", "m", 1000.0),
     ("m", "meter", "si", 1.0),
     ("cm", "centimeter", "m", 1.0e-2),
@@ -57,17 +63,34 @@
     ("h", "hour", "s", 3600.0),
     ("mn", "minute", "s", 60.0),
     ("s", "second", "si", 1.0),
     ("ms", "millisecond", "s", 1.0e-3),
     ("us", "microsecond", "s", 1.0e-6),
     ("ns", "nanosecond", "s", 1.0e-9),
 )
-
 STD_UNIT_CONVERSIONS = {_elm[0]: _elm[-1] for _elm in _STD_UNIT_CONVERSIONS}
 
 
-def IsUnitSection(section: str, /, *, possibly_fuzzy: bool = False) -> bool:
-    """"""
-    if possibly_fuzzy:
-        return section.lower() == UNIT_SECTION.lower()
-    else:
-        return section == UNIT_SECTION
+@dtcl.dataclass(repr=False, eq=False)
+class unit_t(parameter_t):
+    def __post_init__(self) -> None:
+        """
+        Unit parameter are never part of a specification. They can appear in INI
+        documents, and are therefore only instantiated programmatically.
+        """
+        self.types = type_options_t.NewFromTypes(
+            (int, float, Annotated[str, number_in_str_t()])
+        )
+
+    def Issues(self) -> list[str]:
+        """"""
+        if self.name in STD_UNIT_CONVERSIONS.keys():
+            return [
+                f"{self.name}: Redefinition of a standard unit; Please use another unit name."
+            ]
+
+        return []
+
+    @property
+    def optional(self) -> bool:
+        """"""
+        return True
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/standard/dtcl_extension.py` & `conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/boolean.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,35 +26,36 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
+from enum import Enum as enum_t
+from typing import Annotated, ClassVar
 
-import colorama as clrm
+from conf_ini_g.specification.parameter.annotation import (
+    annotation_t,
+    py_type_options_h,
+)
+from conf_ini_g.standard.type_extension import annotated_hint_t
+
+
+@dtcl.dataclass(repr=False, eq=False)
+class boolean_t(annotation_t):
+    VALID_PY_TYPES: ClassVar[py_type_options_h] = bool
+
+    class MODE(enum_t):
+        # Always list true value first
+        true_false = ("True", "False")
+        yes_no = ("Yes", "No")
+        on_off = ("On", "Off")
+
+    mode: enum_t = MODE.true_false
+
+    @classmethod
+    def NewAnnotatedType(cls, mode: enum_t = None) -> annotated_hint_t:
+        """"""
+        if mode is None:
+            mode = cls.MODE.true_false
 
-from conf_ini_g.standard.str_extension import Flattened
-
-
-def AsStr(instance: dtcl.dataclass, /) -> str:
-    """"""
-    output = [f"{clrm.Fore.MAGENTA}{instance.__class__.__name__[:-2].upper()}:"]
-
-    field_names = (_fld.name for _fld in dtcl.fields(instance))
-    for name in field_names:
-        value = getattr(instance, name)
-
-        length = 0  # Only to silence a linter warning
-        if (
-            isinstance(value, (tuple, list))
-            and ((length := value.__len__()) > 0)
-            and not isinstance(value[0], (int, float, str))
-        ):
-            value = f"{length} x {type(value[0]).__name__}"
-        elif isinstance(value, str) and (value.__len__() == 0):
-            value = '""'
-
-        flattened = Flattened(str(value))
-        output.append(f"    {clrm.Fore.CYAN}{name}{clrm.Fore.RESET}={flattened}")
-
-    return "\n".join(output)
+        return Annotated[cls.VALID_PY_TYPES, cls(mode=mode)]
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/standard/str_extension.py` & `conf-ini-g-2023.5/conf_ini_g/standard/str_extension.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,156 +25,200 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+from __future__ import annotations
+
 import ast as asgt
+import dataclasses as dtcl
 import textwrap as text
-from conf_ini_g.standard.path_extension import path_t
-from typing import Any
-
-from conf_ini_g.standard.type_extension import none_t
-
+from types import GenericAlias, UnionType
+from typing import Any, Iterable, Sequence
 
-class _no_default_t:
-    pass
+from conf_ini_g.standard.type_extension import (
+    HintTreeFromTypeHint,
+    hint_node_t,
+    none_t,
+    raw_hint_h,
+)
 
 
 TRUE_VALUES = ("true", "yes", "on")
 FALSE_VALUES = ("false", "no", "off")
 
 
+@dtcl.dataclass(slots=True, repr=False, eq=False)
+class _value_node_t:
+    consolidated: Any
+    type: type | None = None
+    elements: tuple[_value_node_t, ...] | None = None
+
+    def __post_init__(self) -> None:
+        """"""
+        self.type = type(self.consolidated)
+
+
 def Flattened(string: str, /) -> str:
     """"""
-    return text.dedent(string).replace("\n", " ")
+    return text.dedent(string).replace("\n", "; ")
 
 
-def EvaluatedValue(string: str, /, *, expected_type: type = None) -> tuple[Any, bool]:
-    """
-    Evaluated: Means there might be a string evaluation (with ast.literal_eval) to convert the string into a value.
-    But direct conversions might be performed instead.
+def AlignedOnSeparator(
+    string: str | Sequence[str], separator: str, replacement: str, /
+) -> str | tuple[str, ...] | list[str]:
+    """"""
+    if should_return_str := isinstance(string, str):
+        lines = string.splitlines()
+    else:
+        lines = string
+    indices = tuple(_lne.find(separator) for _lne in lines)
+    longest = max(indices)
+
+    output = (
+        _lne.replace(separator, (longest - _lgt) * " " + replacement, 1)
+        if _lgt > 0
+        else _lne
+        for _lne, _lgt in zip(lines, indices)
+    )
+    if should_return_str:
+        return "\n".join(output)
+    elif isinstance(string, tuple):
+        return tuple(output)
+    else:
+        return list(output)
 
-    expected_type: Must not be passed explicitly as None since None is interpreted as "no specific expected type". When
-    expecting None, pass none_t.
+
+def AsInterpretedObject(
+    string: str, /, *, expected_type: type | None = None
+) -> tuple[Any, bool]:
+    """
+    expected_type: Must not be passed explicitly as None since None is interpreted as
+    "no specific expected type". When expecting None, pass none_t.
     """
     if expected_type is None:
-        return _EvaluatedValue(string, default_to_str=True)
+        try:
+            value = asgt.literal_eval(string)
+        except (SyntaxError, ValueError):
+            value = string
+
+        return value, True
+
+    failed_interpretation = None, False
+    lowered = string.lower()
 
-    failed_conversion = None, False
+    if expected_type is none_t:
+        return None, (lowered == "none")
 
     if expected_type is bool:
-        if (lower := string.lower()) in TRUE_VALUES:
+        if lowered in TRUE_VALUES:
             return True, True
-        elif lower in FALSE_VALUES:
+        if lowered in FALSE_VALUES:
             return False, True
-        #
-    elif expected_type in (int, float):
-        value = _ConvertedValue(string, expected_type)
-        if value is None:
-            return failed_conversion
+        return failed_interpretation
 
+    # The expected type might be instantiable from a string, e.g.: float("1.0").
+    # However, a success does not mean that the interpretation is valid, e.g.:
+    # tuple("(1, 2, 3)"). To confirm that a success is indeed a correct interpretation,
+    # the string representation of the interpreted value is compared with the string.
+    # This is not a perfect test, so "literal_eval" might still be called below.
+    try:
+        value = expected_type(string)
+        success = str(value).replace(" ", "") == string.replace(" ", "")
+    except:
+        value, success = failed_interpretation
+    if success:
         return value, True
-        #
-    elif expected_type is path_t:
-        # An empty string becomes "." when converted to a pathlib Path while it should be interpreted as "no path
-        # specified", which is closer to None. To avoid this confusion, an empty string is considered invalid.
-        if string.__len__() > 0:
-            return path_t(string), True
-        #
-    elif expected_type in (tuple, list):
-        value, success = _EvaluatedValue(string)
-        if success and isinstance(value, (tuple, list)):
-            if (expected_type is tuple) and isinstance(value, list):
-                value = tuple(value)
-            elif (expected_type is list) and isinstance(value, tuple):
-                value = list(value)
-
-            return value, True
-        #
-    elif expected_type is none_t:
-        if string.lower() == "none":
-            return None, True
-        #
-    else:
-        value, _ = _EvaluatedValue(string, default_to_str=True)
-        if isinstance(value, expected_type):
-            return value, True
 
-    return failed_conversion
+    try:
+        value = asgt.literal_eval(string)
+        success = type(value) is expected_type
+        if not success:
+            value = None
+    except (SyntaxError, ValueError):
+        value, success = failed_interpretation
+
+    return value, success
 
 
-def _EvaluatedValue(
-    string: str, /, *, default_to_str: bool = False
+def AsComplexInterpretedObject(
+    string: str,
+    /,
+    *,
+    expected_type: raw_hint_h | hint_node_t | None = None,
 ) -> tuple[Any, bool]:
     """"""
-    if (lowered := string.lower()) == "none":
-        return None, True
-    elif lowered in TRUE_VALUES:
-        return True, True
-    elif lowered in FALSE_VALUES:
-        return False, True
-
-    try:
-        value = asgt.literal_eval(string)
-        success = True
-    except (SyntaxError, ValueError):
-        if default_to_str:
-            value = string
-            success = True
+    if isinstance(expected_type, (GenericAlias, UnionType, hint_node_t)):
+        value, _ = AsInterpretedObject(string)
+        value_tree = _ValueTreeOfValue(value)
+        if isinstance(expected_type, hint_node_t):
+            hint_tree = expected_type
         else:
-            value = None
-            success = False
+            hint_tree = HintTreeFromTypeHint(expected_type)
+        if _CastValueTree(value_tree, hint_tree):
+            return _ValueFromValueTree(value_tree), True
+        else:
+            return None, False
 
-    return value, success
+    return AsInterpretedObject(string, expected_type=expected_type)
 
 
-def ConvertedValue(string: str, /) -> Any:
+def _ValueTreeOfValue(value: Any, /) -> _value_node_t:
     """"""
-    if (lowered := string.lower()) == "none":
-        output = None
-    elif lowered in TRUE_VALUES:
-        output = True
-    elif lowered in FALSE_VALUES:
-        output = False
-    elif str.isdigit(string):
-        # Can the conversion to integer fail if isdigit is True? Did not check, so just in case...
-        output = _ConvertedValue(string, int)
-    elif (output := _ConvertedValue(string, float)) is not None:
-        pass
-    elif "," in string:
-        top_level = []
-        pieces = string.split(",")
-        first_idx = 0
-        status = 0
-        for last_idx, piece in enumerate(pieces):
-            if "(" in piece:
-                status += 1
-            elif ")" in piece:
-                status -= 1
-            if status == 0:
-                stripped = ",".join(pieces[first_idx : (last_idx + 1)]).strip(" ()")
-                top_level.append(stripped)
-                first_idx = last_idx + 1
-        output = tuple(ConvertedValue(_vle) for _vle in top_level)
-    else:
-        output = string
+    if isinstance(value, Iterable) and not isinstance(value, str):
+        elements = tuple(_ValueTreeOfValue(_elm) for _elm in value)
+        return _value_node_t(consolidated=value, elements=elements)
 
-    return output
+    return _value_node_t(consolidated=value)
 
 
-def _ConvertedValue(string: str, type_: type, /) -> Any | None:
+def _ValueFromValueTree(value_tree: _value_node_t, /) -> Any:
     """"""
-    try:
-        output = type_(string)
-    except ValueError:
-        output = None
+    if isinstance(value_tree.consolidated, Iterable) and not isinstance(
+        value_tree.consolidated, str
+    ):
+        elements = (_ValueFromValueTree(_elm) for _elm in value_tree.elements)
+        return value_tree.type(elements)
 
-    return output
+    return value_tree.type(value_tree.consolidated)
 
 
-def AlignedNameAndValue(unaligned: str, space: int, /) -> str:
+def _CastValueTree(value_node: _value_node_t, hint_node: hint_node_t, /) -> bool:
     """"""
-    name, value = unaligned.split("=", maxsplit=1)
+    if hint_node.type is None:  # Or
+        if any(_CastValueTree(value_node, _elm) for _elm in hint_node.elements):
+            return True
+        else:
+            return False
+
+    if not isinstance(value_node.consolidated, hint_node.type):
+        try:
+            _ = hint_node.type(value_node.consolidated)
+            success = True
+        except:
+            success = False
+        if not success:
+            return False
+    if hint_node.elements is None:
+        value_node.type = hint_node.type
+        return True
+
+    n_value_children = value_node.elements.__len__()
+    n_hint_elements = hint_node.elements.__len__()
+    has_ellipsis = (n_hint_elements == 2) and (hint_node.elements[1].type is Ellipsis)
+    should_fake_ellipsis = (n_hint_elements == 1) and issubclass(
+        hint_node.type, (list, set)
+    )
+    if has_ellipsis or should_fake_ellipsis or (n_value_children == n_hint_elements):
+        if has_ellipsis or should_fake_ellipsis:
+            hint_elements = n_value_children * (hint_node.elements[0],)
+        else:
+            hint_elements = hint_node.elements
+        for value_elm, hint_elm in zip(value_node.elements, hint_elements):
+            if not _CastValueTree(value_elm, hint_elm):
+                return False
+        value_node.type = hint_node.type
+        return True
 
-    return f"{name:{space}}= {value}"
+    return False
```

### Comparing `conf-ini-g-2023.4/conf_ini_g/version.py` & `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UNS
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,8 +25,14 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.4"
+from PyQt5 import QtWidgets as wdgt
+
+
+class text_wgt_t(wdgt.QLineEdit):
+    def Text(self) -> str:
+        """"""
+        return self.text().strip()
```

### Comparing `conf-ini-g-2023.4/conf_ini_g.egg-info/PKG-INFO` & `conf-ini-g-2023.5/conf_ini_g.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-ini-g
-Version: 2023.4
+Version: 2023.5
 Summary: App Configuration in INI format with Automatic Command-Line Parser and Graphical Interface Generation
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
```

### Comparing `conf-ini-g-2023.4/conf_ini_g.egg-info/SOURCES.txt` & `conf-ini-g-2023.5/conf_ini_g.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,50 +7,59 @@
 conf_ini_g/__init__.py
 conf_ini_g/version.py
 conf_ini_g.egg-info/PKG-INFO
 conf_ini_g.egg-info/SOURCES.txt
 conf_ini_g.egg-info/dependency_links.txt
 conf_ini_g.egg-info/requires.txt
 conf_ini_g.egg-info/top_level.txt
-conf_ini_g/activated/config.py
-conf_ini_g/activated/parameter.py
-conf_ini_g/activated/section.py
-conf_ini_g/activated/unit.py
+conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py
+conf_ini_g/catalog/interface/screen/library/pyqt5/main.py
+conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py
+conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py
+conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py
+conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py
+conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py
+conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py
+conf_ini_g/catalog/interface/screen/parameter/boolean.py
+conf_ini_g/catalog/interface/screen/parameter/choices.py
+conf_ini_g/catalog/interface/screen/parameter/none.py
+conf_ini_g/catalog/interface/screen/parameter/path.py
+conf_ini_g/catalog/interface/screen/parameter/sequence.py
+conf_ini_g/catalog/interface/screen/parameter/text.py
+conf_ini_g/catalog/specification/parameter/boolean.py
+conf_ini_g/catalog/specification/parameter/choices.py
+conf_ini_g/catalog/specification/parameter/number.py
+conf_ini_g/catalog/specification/parameter/path.py
+conf_ini_g/catalog/specification/parameter/sequence.py
+conf_ini_g/instance/config.py
+conf_ini_g/instance/parameter/base.py
+conf_ini_g/instance/parameter/main.py
+conf_ini_g/instance/parameter/unit.py
 conf_ini_g/interface/console/__init__.py
 conf_ini_g/interface/console/config.py
-conf_ini_g/interface/console/generic.py
 conf_ini_g/interface/screen/config.py
 conf_ini_g/interface/screen/generic.py
-conf_ini_g/interface/screen/parameter.py
 conf_ini_g/interface/screen/section.py
-conf_ini_g/interface/screen/component/boolean.py
-conf_ini_g/interface/screen/component/choices.py
-conf_ini_g/interface/screen/component/default_entry.py
-conf_ini_g/interface/screen/component/file_dialogs.py
-conf_ini_g/interface/screen/component/none.py
-conf_ini_g/interface/screen/component/path.py
-conf_ini_g/interface/screen/component/sequence.py
-conf_ini_g/interface/screen/component/type_options.py
-conf_ini_g/interface/screen/library/pyqt5_constant.py
-conf_ini_g/interface/screen/library/pyqt5_generic.py
-conf_ini_g/interface/screen/library/pyqt5_parameter.py
+conf_ini_g/interface/screen/parameter/main.py
+conf_ini_g/interface/screen/parameter/path_chooser.py
+conf_ini_g/interface/screen/parameter/type_selector.py
 conf_ini_g/interface/storage/config.py
 conf_ini_g/interface/storage/constant.py
 conf_ini_g/light/config.py
 conf_ini_g/light/conversion.py
 conf_ini_g/light/ini.py
 conf_ini_g/light/xlsx.py
 conf_ini_g/raw/config.py
+conf_ini_g/specification/base.py
 conf_ini_g/specification/config.py
-conf_ini_g/specification/constant.py
-conf_ini_g/specification/constrained_type.py
-conf_ini_g/specification/constraint.py
-conf_ini_g/specification/default.py
-conf_ini_g/specification/generic.py
-conf_ini_g/specification/parameter.py
-conf_ini_g/specification/section.py
-conf_ini_g/specification/unit.py
-conf_ini_g/standard/dtcl_extension.py
+conf_ini_g/specification/parameter/annotation.py
+conf_ini_g/specification/parameter/main.py
+conf_ini_g/specification/parameter/type.py
+conf_ini_g/specification/parameter/unit.py
+conf_ini_g/specification/parameter/value.py
+conf_ini_g/specification/section/main.py
+conf_ini_g/specification/section/unit.py
 conf_ini_g/standard/path_extension.py
+conf_ini_g/standard/py_extension.py
 conf_ini_g/standard/str_extension.py
 conf_ini_g/standard/type_extension.py
 documentation/wiki/description.asciidoc
```

### Comparing `conf-ini-g-2023.4/documentation/wiki/description.asciidoc` & `conf-ini-g-2023.5/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.4/setup.py` & `conf-ini-g-2023.5/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -68,24 +68,35 @@
 PYPI_TOPIC = "Software Development"
 PYPI_AUDIENCE = "Developers"
 PYPI_STATUS = "4 - Beta"
 
 IMPORT_NAME = "conf_ini_g"
 PACKAGES = [
     IMPORT_NAME,
-    f"{IMPORT_NAME}.activated",
+    f"{IMPORT_NAME}.catalog",
+    f"{IMPORT_NAME}.catalog.interface",
+    f"{IMPORT_NAME}.catalog.interface.screen",
+    f"{IMPORT_NAME}.catalog.interface.screen.library",
+    f"{IMPORT_NAME}.catalog.interface.screen.library.pyqt5",
+    f"{IMPORT_NAME}.catalog.interface.screen.library.pyqt5.widget",
+    f"{IMPORT_NAME}.catalog.interface.screen.parameter",
+    f"{IMPORT_NAME}.catalog.specification",
+    f"{IMPORT_NAME}.catalog.specification.parameter",
+    f"{IMPORT_NAME}.instance",
+    f"{IMPORT_NAME}.instance.parameter",
     f"{IMPORT_NAME}.interface",
     f"{IMPORT_NAME}.interface.console",
     f"{IMPORT_NAME}.interface.screen",
-    f"{IMPORT_NAME}.interface.screen.component",
-    f"{IMPORT_NAME}.interface.screen.library",
+    f"{IMPORT_NAME}.interface.screen.parameter",
     f"{IMPORT_NAME}.interface.storage",
     f"{IMPORT_NAME}.light",
     f"{IMPORT_NAME}.raw",
     f"{IMPORT_NAME}.specification",
+    f"{IMPORT_NAME}.specification.parameter",
+    f"{IMPORT_NAME}.specification.section",
     f"{IMPORT_NAME}.standard",
 ]
 EXCLUDED_FOLDERS = (
     f"{IMPORT_NAME}.documentation",
     f"{IMPORT_NAME}.test",
 )
 ENTRY_POINTS = {}
@@ -115,30 +126,30 @@
                 folders.append(node)
     folders = sorted(folders)
 
     packages = sorted(PACKAGES)
     if packages != folders:
         raise ValueError(
             f"Mismatch between declared and found packages:\n"
-            f"    - Declared=\n      {packages}\n"
-            f"    - Found=\n      {folders}"
+            f"    - Declared=\n      {packages};\n"
+            f"    - Found=\n      {folders}."
         )
 
 
 def Version():
     """"""
     contents = {}
     with open(HERE / IMPORT_NAME / "version.py") as accessor:
         exec(accessor.read(), contents)
 
     output = contents["__version__"]
     if isinstance(output, str) and rgex.fullmatch(r"20[0-9]{2}\.[1-9][0-9]*", output):
         return output
 
-    raise ValueError(f"{output}: Invalid version")
+    raise ValueError(f"{output}: Invalid version.")
 
 
 if __name__ == "__main__":
     #
     CheckCoherenceBetweenDeclarationAndReality()
     # fmt: off
     setup(
@@ -168,11 +179,11 @@
         },
         #
         packages=PACKAGES,
         entry_points=ENTRY_POINTS,
         python_requires=f">={PY_VERSION}",
         install_requires=[
             "PyQt5",
-            "colorama",
+            "rich",
             "openpyxl",
         ],
     )
```

