# Comparing `tmp/umap-project-1.3.0.tar.gz` & `tmp/umap-project-1.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umap-project-1.3.0.tar", last modified: Wed May 31 08:37:12 2023, max compression
+gzip compressed data, was "umap-project-1.3.0a0.tar", last modified: Wed May 31 07:43:08 2023, max compression
```

## Comparing `umap-project-1.3.0.tar` & `umap-project-1.3.0a0.tar`

### file list

```diff
@@ -1,535 +1,535 @@
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.843614 umap-project-1.3.0/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      482 2016-04-23 07:38:39.000000 umap-project-1.3.0/LICENSE
--rw-r--r--   0 ybon      (1000) ybon      (1000)      196 2018-07-14 08:06:10.000000 umap-project-1.3.0/MANIFEST.in
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2165 2023-05-31 08:37:12.846947 umap-project-1.3.0/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1184 2019-02-22 20:49:23.000000 umap-project-1.3.0/README.md
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1389 2023-05-31 08:37:12.846947 umap-project-1.3.0/setup.cfg
--rw-r--r--   0 ybon      (1000) ybon      (1000)       37 2023-05-23 16:48:43.000000 umap-project-1.3.0/setup.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.740280 umap-project-1.3.0/umap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      178 2023-05-23 16:48:43.000000 umap-project-1.3.0/umap/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      541 2023-05-23 16:48:43.000000 umap-project-1.3.0/umap/admin.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      109 2023-05-23 16:48:43.000000 umap-project-1.3.0/umap/apps.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      535 2023-02-22 09:51:22.000000 umap-project-1.3.0/umap/autocomplete.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.740280 umap-project-1.3.0/umap/bin/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      256 2016-09-17 20:05:31.000000 umap-project-1.3.0/umap/bin/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      448 2023-05-31 07:12:01.000000 umap-project-1.3.0/umap/context_processors.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2021 2023-05-23 16:48:43.000000 umap-project-1.3.0/umap/decorators.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      869 2023-05-23 16:48:43.000000 umap-project-1.3.0/umap/fields.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2740 2023-05-23 17:05:44.000000 umap-project-1.3.0/umap/forms.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.716946 umap-project-1.3.0/umap/locale/am_ET/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.743613 umap-project-1.3.0/umap/locale/am_ET/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6577 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/am_ET/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11035 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/am_ET/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.716946 umap-project-1.3.0/umap/locale/ar/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.743613 umap-project-1.3.0/umap/locale/ar/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4038 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9743 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.716946 umap-project-1.3.0/umap/locale/ast/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.743613 umap-project-1.3.0/umap/locale/ast/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      432 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/locale/ast/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8007 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/locale/ast/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.716946 umap-project-1.3.0/umap/locale/bg/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.743613 umap-project-1.3.0/umap/locale/bg/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7132 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11584 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.716946 umap-project-1.3.0/umap/locale/ca/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.743613 umap-project-1.3.0/umap/locale/ca/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7185 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10694 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.716946 umap-project-1.3.0/umap/locale/cs_CZ/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.743613 umap-project-1.3.0/umap/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7364 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/cs_CZ/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10996 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/cs_CZ/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.716946 umap-project-1.3.0/umap/locale/da/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.746946 umap-project-1.3.0/umap/locale/da/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6995 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10627 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.716946 umap-project-1.3.0/umap/locale/de/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.746946 umap-project-1.3.0/umap/locale/de/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7335 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11063 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.716946 umap-project-1.3.0/umap/locale/el/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.746946 umap-project-1.3.0/umap/locale/el/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10115 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13827 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.716946 umap-project-1.3.0/umap/locale/en/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.746946 umap-project-1.3.0/umap/locale/en/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      337 2023-05-31 07:14:25.000000 umap-project-1.3.0/umap/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7443 2023-05-31 07:12:10.000000 umap-project-1.3.0/umap/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.716946 umap-project-1.3.0/umap/locale/es/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.746946 umap-project-1.3.0/umap/locale/es/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7292 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11100 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/et/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.750280 umap-project-1.3.0/umap/locale/et/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6136 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9983 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/fa_IR/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.750280 umap-project-1.3.0/umap/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8955 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/fa_IR/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12488 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/fa_IR/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/fi/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.750280 umap-project-1.3.0/umap/locale/fi/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5792 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10408 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/fr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.750280 umap-project-1.3.0/umap/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7904 2023-05-31 07:56:55.000000 umap-project-1.3.0/umap/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11039 2023-05-31 07:56:47.000000 umap-project-1.3.0/umap/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/gl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.750280 umap-project-1.3.0/umap/locale/gl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7160 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10751 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/he/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.750280 umap-project-1.3.0/umap/locale/he/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8007 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11518 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/hr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.750280 umap-project-1.3.0/umap/locale/hr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1777 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8477 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/hu/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.750280 umap-project-1.3.0/umap/locale/hu/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7561 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11122 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/id/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.753613 umap-project-1.3.0/umap/locale/id/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      425 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8000 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/is/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.753613 umap-project-1.3.0/umap/locale/is/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7603 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/is/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11110 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/it/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.753613 umap-project-1.3.0/umap/locale/it/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7309 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11188 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/ja/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.753613 umap-project-1.3.0/umap/locale/ja/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7672 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11240 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/ko/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.753613 umap-project-1.3.0/umap/locale/ko/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7625 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11132 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/lt/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.753613 umap-project-1.3.0/umap/locale/lt/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6845 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10659 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/ms/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.753613 umap-project-1.3.0/umap/locale/ms/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7577 2023-05-31 07:14:25.000000 umap-project-1.3.0/umap/locale/ms/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10506 2023-05-31 07:14:01.000000 umap-project-1.3.0/umap/locale/ms/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/nl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.753613 umap-project-1.3.0/umap/locale/nl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6999 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10549 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/no/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.753613 umap-project-1.3.0/umap/locale/no/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      423 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/locale/no/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7998 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/locale/no/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/pl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.756946 umap-project-1.3.0/umap/locale/pl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7298 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11013 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.720280 umap-project-1.3.0/umap/locale/pt/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.756946 umap-project-1.3.0/umap/locale/pt/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7256 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10828 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/pt_BR/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.756946 umap-project-1.3.0/umap/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7282 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10908 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/pt_PT/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.756946 umap-project-1.3.0/umap/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7271 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10843 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/ro/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.756946 umap-project-1.3.0/umap/locale/ro/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1482 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8428 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/ru/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.756946 umap-project-1.3.0/umap/locale/ru/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9228 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12926 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/si_LK/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.756946 umap-project-1.3.0/umap/locale/si_LK/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      447 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/locale/si_LK/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8022 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/locale/si_LK/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/sk_SK/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.756946 umap-project-1.3.0/umap/locale/sk_SK/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6891 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/sk_SK/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10730 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/sk_SK/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/sl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.760280 umap-project-1.3.0/umap/locale/sl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6825 2023-05-31 07:14:25.000000 umap-project-1.3.0/umap/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10538 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/sr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.760280 umap-project-1.3.0/umap/locale/sr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8830 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12352 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/sv/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.760280 umap-project-1.3.0/umap/locale/sv/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6975 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10508 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/th_TH/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.760280 umap-project-1.3.0/umap/locale/th_TH/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10318 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/th_TH/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13772 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/th_TH/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/tr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.760280 umap-project-1.3.0/umap/locale/tr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7375 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10952 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/uk_UA/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.760280 umap-project-1.3.0/umap/locale/uk_UA/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9429 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/uk_UA/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12970 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/uk_UA/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/vi/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.760280 umap-project-1.3.0/umap/locale/vi/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6064 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10544 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/zh/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.760280 umap-project-1.3.0/umap/locale/zh/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4419 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9338 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.723613 umap-project-1.3.0/umap/locale/zh_TW/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.763613 umap-project-1.3.0/umap/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6802 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10562 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.763613 umap-project-1.3.0/umap/management/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.3.0/umap/management/__init__.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.763613 umap-project-1.3.0/umap/management/commands/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.3.0/umap/management/commands/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      839 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/management/commands/anonymous_edit_url.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1298 2019-04-07 14:33:20.000000 umap-project-1.3.0/umap/management/commands/generate_js_locale.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1902 2019-04-07 14:28:38.000000 umap-project-1.3.0/umap/management/commands/import_pictograms.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      207 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/managers.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/middleware.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.763613 umap-project-1.3.0/umap/migrations/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5563 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/migrations/0001_initial.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      373 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/migrations/0002_tilelayer_tms.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      812 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/migrations/0003_add_tilelayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      530 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/migrations/0004_add_licence.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2018-07-14 11:58:47.000000 umap-project-1.3.0/umap/migrations/0005_remove_map_tilelayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      497 2019-04-07 08:09:35.000000 umap-project-1.3.0/umap/migrations/0006_auto_20190407_0719.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/migrations/0007_auto_20190416_1757.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      459 2023-05-23 16:48:43.000000 umap-project-1.3.0/umap/migrations/0008_alter_map_settings.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      886 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/migrations/0009_star.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-11-26 16:02:45.000000 umap-project-1.3.0/umap/migrations/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11456 2023-05-31 07:12:01.000000 umap-project-1.3.0/umap/models.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.763613 umap-project-1.3.0/umap/settings/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1617 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/settings/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7642 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/settings/base.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      386 2018-05-19 15:10:46.000000 umap-project-1.3.0/umap/settings/dev.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.763613 umap-project-1.3.0/umap/static/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.3.0/umap/static/.gitignore
--rw-r--r--   0 ybon      (1000) ybon      (1000)      638 2016-04-23 07:38:39.000000 umap-project-1.3.0/umap/static/favicon.ico
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.766946 umap-project-1.3.0/umap/static/umap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    18104 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/static/umap/base.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9125 2016-04-23 07:38:39.000000 umap-project-1.3.0/umap/static/umap/bitbucket.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5858 2023-05-30 06:46:59.000000 umap-project-1.3.0/umap/static/umap/content.css
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.770280 umap-project-1.3.0/umap/static/umap/font/
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   182984 2018-05-17 09:59:39.000000 umap-project-1.3.0/umap/static/umap/font/FiraSans-Light.woff
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   129180 2018-05-17 09:59:39.000000 umap-project-1.3.0/umap/static/umap/font/FiraSans-Light.woff2
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   191400 2018-05-17 09:59:39.000000 umap-project-1.3.0/umap/static/umap/font/FiraSans-LightItalic.woff
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   135744 2018-05-17 09:59:39.000000 umap-project-1.3.0/umap/static/umap/font/FiraSans-LightItalic.woff2
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   198128 2018-05-17 09:59:39.000000 umap-project-1.3.0/umap/static/umap/font/FiraSans-SemiBold.woff
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   140168 2018-05-17 09:59:39.000000 umap-project-1.3.0/umap/static/umap/font/FiraSans-SemiBold.woff2
--rw-r--r--   0 ybon      (1000) ybon      (1000)      832 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/static/umap/font.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1564 2016-04-23 07:38:39.000000 umap-project-1.3.0/umap/static/umap/github.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.773613 umap-project-1.3.0/umap/static/umap/img/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13636 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/static/umap/img/16-white.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    57263 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/static/umap/img/16-white.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11308 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/static/umap/img/16.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    38140 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/static/umap/img/16.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)    19711 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/static/umap/img/24-white.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    38377 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/static/umap/img/24-white.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)    16878 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/static/umap/img/24.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    36478 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/static/umap/img/24.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)      430 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/static/umap/img/edit-16.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      554 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/static/umap/img/edit.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)      190 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/static/umap/img/icon-bg.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      327 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/static/umap/img/logo.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5537 2016-04-23 07:38:39.000000 umap-project-1.3.0/umap/static/umap/img/logo_filigree.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      375 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/static/umap/img/marker.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      473 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/static/umap/img/opensource.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1997 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/static/umap/img/osm.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1472 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/static/umap/img/search.gif
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.776946 umap-project-1.3.0/umap/static/umap/js/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7937 2023-05-30 19:46:43.000000 umap-project-1.3.0/umap/static/umap/js/umap.autocomplete.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    38965 2023-05-31 08:22:15.000000 umap-project-1.3.0/umap/static/umap/js/umap.controls.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    19966 2023-05-30 19:49:34.000000 umap-project-1.3.0/umap/static/umap/js/umap.core.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31642 2023-05-30 19:46:43.000000 umap-project-1.3.0/umap/static/umap/js/umap.features.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27320 2023-05-30 19:46:43.000000 umap-project-1.3.0/umap/static/umap/js/umap.forms.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5762 2023-05-30 19:46:43.000000 umap-project-1.3.0/umap/static/umap/js/umap.icon.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    68708 2023-05-31 07:12:01.000000 umap-project-1.3.0/umap/static/umap/js/umap.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33580 2023-05-30 19:46:43.000000 umap-project-1.3.0/umap/static/umap/js/umap.layer.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5809 2023-05-30 19:46:43.000000 umap-project-1.3.0/umap/static/umap/js/umap.permissions.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6802 2023-05-30 19:46:43.000000 umap-project-1.3.0/umap/static/umap/js/umap.popup.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4421 2023-05-30 19:46:43.000000 umap-project-1.3.0/umap/static/umap/js/umap.slideshow.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4191 2023-05-30 19:46:43.000000 umap-project-1.3.0/umap/static/umap/js/umap.tableeditor.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6872 2023-05-30 19:46:43.000000 umap-project-1.3.0/umap/static/umap/js/umap.ui.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8711 2023-05-30 19:46:43.000000 umap-project-1.3.0/umap/static/umap/js/umap.xhr.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.803613 umap-project-1.3.0/umap/static/umap/locale/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27485 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/am_ET.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27414 2023-05-31 07:14:01.000000 umap-project-1.3.0/umap/static/umap/locale/am_ET.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23264 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/ar.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23199 2023-05-31 07:14:01.000000 umap-project-1.3.0/umap/static/umap/locale/ar.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22797 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/ast.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:01.000000 umap-project-1.3.0/umap/static/umap/locale/ast.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26550 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/bg.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26485 2023-05-31 07:14:01.000000 umap-project-1.3.0/umap/static/umap/locale/bg.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23646 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/ca.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23581 2023-05-31 07:14:02.000000 umap-project-1.3.0/umap/static/umap/locale/ca.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24628 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/cs_CZ.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24557 2023-05-31 07:14:02.000000 umap-project-1.3.0/umap/static/umap/locale/cs_CZ.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23232 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/da.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23167 2023-05-31 07:14:02.000000 umap-project-1.3.0/umap/static/umap/locale/da.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24743 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/de.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24678 2023-05-31 07:14:03.000000 umap-project-1.3.0/umap/static/umap/locale/de.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33701 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/el.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33636 2023-05-31 07:14:02.000000 umap-project-1.3.0/umap/static/umap/locale/el.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22797 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/en.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22732 2023-05-31 07:12:10.000000 umap-project-1.3.0/umap/static/umap/locale/en.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22442 2023-05-31 07:14:04.000000 umap-project-1.3.0/umap/static/umap/locale/en_US.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24956 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/es.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24891 2023-05-31 07:14:04.000000 umap-project-1.3.0/umap/static/umap/locale/es.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23050 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/et.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22985 2023-05-31 07:14:04.000000 umap-project-1.3.0/umap/static/umap/locale/et.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30194 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/fa_IR.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30123 2023-05-31 07:14:04.000000 umap-project-1.3.0/umap/static/umap/locale/fa_IR.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23862 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/fi.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23797 2023-05-31 07:14:04.000000 umap-project-1.3.0/umap/static/umap/locale/fi.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24960 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/fr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24895 2023-05-31 07:14:05.000000 umap-project-1.3.0/umap/static/umap/locale/fr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24456 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/gl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24391 2023-05-31 07:14:05.000000 umap-project-1.3.0/umap/static/umap/locale/gl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26905 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/he.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26840 2023-05-31 07:14:05.000000 umap-project-1.3.0/umap/static/umap/locale/he.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23005 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/hr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22940 2023-05-31 07:14:05.000000 umap-project-1.3.0/umap/static/umap/locale/hr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25810 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/hu.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25745 2023-05-31 07:14:05.000000 umap-project-1.3.0/umap/static/umap/locale/hu.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22795 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/id.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:06.000000 umap-project-1.3.0/umap/static/umap/locale/id.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24377 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/is.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24312 2023-05-31 07:14:06.000000 umap-project-1.3.0/umap/static/umap/locale/is.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24474 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/it.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24409 2023-05-31 07:14:06.000000 umap-project-1.3.0/umap/static/umap/locale/it.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25895 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/ja.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25830 2023-05-31 07:14:06.000000 umap-project-1.3.0/umap/static/umap/locale/ja.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23023 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/ko.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22958 2023-05-31 07:14:06.000000 umap-project-1.3.0/umap/static/umap/locale/ko.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23762 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/lt.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23697 2023-05-31 07:14:08.000000 umap-project-1.3.0/umap/static/umap/locale/lt.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23906 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/ms.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23841 2023-05-31 07:14:08.000000 umap-project-1.3.0/umap/static/umap/locale/ms.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24414 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/nl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24349 2023-05-31 07:14:08.000000 umap-project-1.3.0/umap/static/umap/locale/nl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23074 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/no.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23009 2023-05-31 07:14:08.000000 umap-project-1.3.0/umap/static/umap/locale/no.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24276 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/pl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24211 2023-05-31 07:14:08.000000 umap-project-1.3.0/umap/static/umap/locale/pl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:09.000000 umap-project-1.3.0/umap/static/umap/locale/pl_PL.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24433 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/pt.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24368 2023-05-31 07:14:09.000000 umap-project-1.3.0/umap/static/umap/locale/pt.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24422 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/pt_BR.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24351 2023-05-31 07:14:09.000000 umap-project-1.3.0/umap/static/umap/locale/pt_BR.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24432 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/pt_PT.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24361 2023-05-31 07:14:09.000000 umap-project-1.3.0/umap/static/umap/locale/pt_PT.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22856 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/ro.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22791 2023-05-31 07:14:09.000000 umap-project-1.3.0/umap/static/umap/locale/ro.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31470 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/ru.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31405 2023-05-31 07:14:10.000000 umap-project-1.3.0/umap/static/umap/locale/ru.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22801 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/si_LK.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:10.000000 umap-project-1.3.0/umap/static/umap/locale/si_LK.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24310 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/sk_SK.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24239 2023-05-31 07:14:10.000000 umap-project-1.3.0/umap/static/umap/locale/sk_SK.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24157 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/sl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24092 2023-05-31 07:14:10.000000 umap-project-1.3.0/umap/static/umap/locale/sl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27557 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/sr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27492 2023-05-31 07:14:10.000000 umap-project-1.3.0/umap/static/umap/locale/sr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24031 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/sv.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23966 2023-05-31 07:14:12.000000 umap-project-1.3.0/umap/static/umap/locale/sv.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22801 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/th_TH.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:12.000000 umap-project-1.3.0/umap/static/umap/locale/th_TH.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24649 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/tr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24584 2023-05-31 07:14:12.000000 umap-project-1.3.0/umap/static/umap/locale/tr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31037 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/uk_UA.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30966 2023-05-31 07:14:12.000000 umap-project-1.3.0/umap/static/umap/locale/uk_UA.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23174 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/vi.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23109 2023-05-31 07:14:12.000000 umap-project-1.3.0/umap/static/umap/locale/vi.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:13.000000 umap-project-1.3.0/umap/static/umap/locale/vi_VN.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22421 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/zh.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22356 2023-05-31 07:14:13.000000 umap-project-1.3.0/umap/static/umap/locale/zh.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:13.000000 umap-project-1.3.0/umap/static/umap/locale/zh_CN.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:13.000000 umap-project-1.3.0/umap/static/umap/locale/zh_TW.Big5.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22410 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap/static/umap/locale/zh_TW.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22339 2023-05-31 07:14:13.000000 umap-project-1.3.0/umap/static/umap/locale/zh_TW.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31816 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/static/umap/map.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1492 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/static/umap/nav.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    19408 2016-04-23 07:38:39.000000 umap-project-1.3.0/umap/static/umap/openstreetmap.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.806947 umap-project-1.3.0/umap/static/umap/test/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      464 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/static/umap/test/.eslintrc
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1665 2023-05-30 15:52:32.000000 umap-project-1.3.0/umap/static/umap/test/Controls.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11544 2023-05-30 15:52:32.000000 umap-project-1.3.0/umap/static/umap/test/DataLayer.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9423 2023-05-30 15:52:32.000000 umap-project-1.3.0/umap/static/umap/test/Feature.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    16802 2023-05-30 15:52:32.000000 umap-project-1.3.0/umap/static/umap/test/Map.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3318 2023-05-30 15:52:32.000000 umap-project-1.3.0/umap/static/umap/test/Marker.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2314 2023-05-30 15:52:32.000000 umap-project-1.3.0/umap/static/umap/test/Permissions.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12614 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/static/umap/test/Polygon.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13986 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/static/umap/test/Polyline.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3216 2023-05-30 15:52:32.000000 umap-project-1.3.0/umap/static/umap/test/TableEditor.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14080 2023-05-30 19:49:34.000000 umap-project-1.3.0/umap/static/umap/test/Util.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9840 2023-05-30 15:52:32.000000 umap-project-1.3.0/umap/static/umap/test/_pre.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5318 2023-05-30 19:49:34.000000 umap-project-1.3.0/umap/static/umap/test/index.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)       49 2018-06-02 13:09:22.000000 umap-project-1.3.0/umap/static/umap/theme.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3225 2016-04-23 07:38:39.000000 umap-project-1.3.0/umap/static/umap/twitter.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.730280 umap-project-1.3.0/umap/static/umap/vendors/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.806947 umap-project-1.3.0/umap/static/umap/vendors/contextmenu/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1231 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    16343 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)      990 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8994 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.806947 umap-project-1.3.0/umap/static/umap/vendors/csv2geojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    15029 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/csv2geojson/csv2geojson.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6994 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/csv2geojson/index.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.806947 umap-project-1.3.0/umap/static/umap/vendors/dompurify/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    62738 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/dompurify/purify.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.810280 umap-project-1.3.0/umap/static/umap/vendors/editable/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    74768 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/editable/Leaflet.Editable.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3898 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/editable/Path.Drag.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.810280 umap-project-1.3.0/umap/static/umap/vendors/editinosm/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1263 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9141 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3340 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/editinosm/edit-in-osm.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.810280 umap-project-1.3.0/umap/static/umap/vendors/formbuilder/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12235 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.810280 umap-project-1.3.0/umap/static/umap/vendors/fullscreen/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5041 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3654 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/fullscreen/fullscreen.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      420 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/fullscreen/fullscreen@2x.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      994 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.810280 umap-project-1.3.0/umap/static/umap/vendors/georsstogeojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3202 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.810280 umap-project-1.3.0/umap/static/umap/vendors/hash/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3462 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/hash/leaflet-hash.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.810280 umap-project-1.3.0/umap/static/umap/vendors/heat/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5158 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/heat/leaflet-heat.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.813614 umap-project-1.3.0/umap/static/umap/vendors/i18n/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1305 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/i18n/Leaflet.i18n.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.816947 umap-project-1.3.0/umap/static/umap/vendors/leaflet/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.820280 umap-project-1.3.0/umap/static/umap/vendors/leaflet/images/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1259 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/leaflet/images/layers-2x.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      696 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/leaflet/images/layers.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2464 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1466 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/leaflet/images/marker-icon.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      618 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/leaflet/images/marker-shadow.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)   398517 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet-src.esm.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   759894 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map
--rw-r--r--   0 ybon      (1000) ybon      (1000)   400242 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet-src.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   759986 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet-src.js.map
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14106 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)   140468 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   191112 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet.js.map
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.820280 umap-project-1.3.0/umap/static/umap/vendors/loading/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3252 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/loading/Control.Loading.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14143 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/loading/Control.Loading.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.820280 umap-project-1.3.0/umap/static/umap/vendors/locatecontrol/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2471 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30907 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.820280 umap-project-1.3.0/umap/static/umap/vendors/markercluster/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1346 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)      886 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/markercluster/MarkerCluster.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/markercluster/WhereAreTheJavascriptFiles.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)    80271 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   157229 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33679 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/markercluster/leaflet.markercluster.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27566 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.823614 umap-project-1.3.0/umap/static/umap/vendors/measurable/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      937 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/measurable/Leaflet.Measurable.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7256 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/measurable/Leaflet.Measurable.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.823614 umap-project-1.3.0/umap/static/umap/vendors/minimap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1998 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/minimap/Control.MiniMap.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12129 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/minimap/Control.MiniMap.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.823614 umap-project-1.3.0/umap/static/umap/vendors/minimap/images/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      219 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/minimap/images/toggle.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8057 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/minimap/images/toggle.svg
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.823614 umap-project-1.3.0/umap/static/umap/vendors/osmtogeojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    35642 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.823614 umap-project-1.3.0/umap/static/umap/vendors/photon/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14433 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/photon/leaflet.photon.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.823614 umap-project-1.3.0/umap/static/umap/vendors/print/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    44559 2021-09-12 08:45:21.000000 umap-project-1.3.0/umap/static/umap/vendors/print/leaflet.browser.print.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23442 2021-09-12 08:45:21.000000 umap-project-1.3.0/umap/static/umap/vendors/print/leaflet.browser.print.min.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.823614 umap-project-1.3.0/umap/static/umap/vendors/togeojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    18098 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/togeojson/togeojson.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.823614 umap-project-1.3.0/umap/static/umap/vendors/togpx/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    17936 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/togpx/togpx.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.823614 umap-project-1.3.0/umap/static/umap/vendors/tokml/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11521 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/tokml/tokml.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.823614 umap-project-1.3.0/umap/static/umap/vendors/toolbar/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2890 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9060 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2244 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/toolbar/leaflet.toolbar.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5326 2023-05-31 08:36:21.000000 umap-project-1.3.0/umap/static/umap/vendors/toolbar/leaflet.toolbar.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.826947 umap-project-1.3.0/umap/templates/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      305 2016-04-23 07:38:39.000000 umap-project-1.3.0/umap/templates/404.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4904 2016-04-23 07:38:39.000000 umap-project-1.3.0/umap/templates/500.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.826947 umap-project-1.3.0/umap/templates/auth/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      467 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/templates/auth/user_detail.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      487 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/templates/auth/user_stars.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      702 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/templates/base.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.826947 umap-project-1.3.0/umap/templates/registration/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1157 2023-03-01 18:10:17.000000 umap-project-1.3.0/umap/templates/registration/login.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.840280 umap-project-1.3.0/umap/templates/umap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      128 2018-05-18 20:43:08.000000 umap-project-1.3.0/umap/templates/umap/about.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1897 2023-05-31 07:12:01.000000 umap-project-1.3.0/umap/templates/umap/about_summary.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2857 2023-05-31 07:12:01.000000 umap-project-1.3.0/umap/templates/umap/content.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      634 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/templates/umap/content_footer.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1309 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/templates/umap/css.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-05-18 20:43:08.000000 umap-project-1.3.0/umap/templates/umap/footer.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      631 2023-05-31 07:12:01.000000 umap-project-1.3.0/umap/templates/umap/home.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3155 2023-05-30 19:49:34.000000 umap-project-1.3.0/umap/templates/umap/js.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      112 2023-05-30 19:46:43.000000 umap-project-1.3.0/umap/templates/umap/locale.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)      629 2023-05-30 06:46:59.000000 umap-project-1.3.0/umap/templates/umap/login_popup_end.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      595 2021-09-12 08:45:40.000000 umap-project-1.3.0/umap/templates/umap/map_detail.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      200 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/templates/umap/map_fragment.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      165 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/templates/umap/map_init.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      597 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/templates/umap/map_list.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/templates/umap/map_messages.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1125 2023-05-31 07:12:01.000000 umap-project-1.3.0/umap/templates/umap/navigation.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      878 2018-05-18 20:43:08.000000 umap-project-1.3.0/umap/templates/umap/password_change.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      258 2018-05-18 20:43:08.000000 umap-project-1.3.0/umap/templates/umap/password_change_done.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      390 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/templates/umap/search.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      448 2018-05-18 20:43:08.000000 umap-project-1.3.0/umap/templates/umap/search_bar.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)        2 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/templates/umap/success.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.840280 umap-project-1.3.0/umap/templatetags/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.3.0/umap/templatetags/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2405 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/templatetags/umap_tags.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.843614 umap-project-1.3.0/umap/tests/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/tests/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2945 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/tests/base.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1466 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/tests/conftest.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      360 2023-05-05 17:42:43.000000 umap-project-1.3.0/umap/tests/settings.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2870 2023-02-27 10:29:01.000000 umap-project-1.3.0/umap/tests/test_datalayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7173 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/tests/test_datalayer_views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      339 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/tests/test_licence.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3149 2018-07-14 13:10:40.000000 umap-project-1.3.0/umap/tests/test_map.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    20902 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/tests/test_map_views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      605 2018-07-14 08:06:10.000000 umap-project-1.3.0/umap/tests/test_tilelayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      407 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/tests/test_utils.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5822 2023-05-31 07:12:01.000000 umap-project-1.3.0/umap/tests/test_views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5304 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/urls.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4381 2023-05-30 13:55:57.000000 umap-project-1.3.0/umap/utils.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    28421 2023-05-31 07:12:01.000000 umap-project-1.3.0/umap/views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1152 2018-05-19 15:10:36.000000 umap-project-1.3.0/umap/wsgi.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 08:37:12.843614 umap-project-1.3.0/umap_project.egg-info/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2165 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap_project.egg-info/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14363 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap_project.egg-info/SOURCES.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)        1 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap_project.egg-info/dependency_links.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)       39 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap_project.egg-info/entry_points.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)      263 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap_project.egg-info/requires.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)        5 2023-05-31 08:37:12.000000 umap-project-1.3.0/umap_project.egg-info/top_level.txt
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.651023 umap-project-1.3.0a0/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      482 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/LICENSE
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      196 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/MANIFEST.in
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2167 2023-05-31 07:43:08.651023 umap-project-1.3.0a0/PKG-INFO
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1184 2019-02-22 20:49:23.000000 umap-project-1.3.0a0/README.md
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1395 2023-05-31 07:43:08.651023 umap-project-1.3.0a0/setup.cfg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       37 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/setup.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.531023 umap-project-1.3.0a0/umap/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      178 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/umap/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      541 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/umap/admin.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      109 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/umap/apps.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      535 2023-02-22 09:51:22.000000 umap-project-1.3.0a0/umap/autocomplete.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.534356 umap-project-1.3.0a0/umap/bin/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      256 2016-09-17 20:05:31.000000 umap-project-1.3.0a0/umap/bin/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      448 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/context_processors.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2021 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/umap/decorators.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      869 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/umap/fields.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2740 2023-05-23 17:05:44.000000 umap-project-1.3.0a0/umap/forms.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.524356 umap-project-1.3.0a0/umap/locale/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/am_ET/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.534356 umap-project-1.3.0a0/umap/locale/am_ET/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6577 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/am_ET/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11035 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/am_ET/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/ar/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.534356 umap-project-1.3.0a0/umap/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4038 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9743 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/ast/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.534356 umap-project-1.3.0a0/umap/locale/ast/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      432 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/ast/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8007 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/ast/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/bg/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.534356 umap-project-1.3.0a0/umap/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7132 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11584 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/ca/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.534356 umap-project-1.3.0a0/umap/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7185 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10694 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/cs_CZ/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.537689 umap-project-1.3.0a0/umap/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7364 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/cs_CZ/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10996 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/cs_CZ/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/da/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.537689 umap-project-1.3.0a0/umap/locale/da/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6995 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10627 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/de/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.537689 umap-project-1.3.0a0/umap/locale/de/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7335 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11063 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/el/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.537689 umap-project-1.3.0a0/umap/locale/el/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10115 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13827 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/en/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.537689 umap-project-1.3.0a0/umap/locale/en/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      337 2023-05-31 07:14:25.000000 umap-project-1.3.0a0/umap/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7443 2023-05-31 07:12:10.000000 umap-project-1.3.0a0/umap/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/es/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.537689 umap-project-1.3.0a0/umap/locale/es/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7292 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11100 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/et/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.541023 umap-project-1.3.0a0/umap/locale/et/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6136 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9983 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/fa_IR/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.541023 umap-project-1.3.0a0/umap/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8955 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/fa_IR/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12488 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/fa_IR/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/fi/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.541023 umap-project-1.3.0a0/umap/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5792 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10408 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/fr/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.541023 umap-project-1.3.0a0/umap/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7399 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11327 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/gl/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.541023 umap-project-1.3.0a0/umap/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7160 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10751 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/he/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.544356 umap-project-1.3.0a0/umap/locale/he/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8007 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11518 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/hr/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.544356 umap-project-1.3.0a0/umap/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1777 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8477 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/hu/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.544356 umap-project-1.3.0a0/umap/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7561 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11122 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/id/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.544356 umap-project-1.3.0a0/umap/locale/id/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      425 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8000 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/is/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.544356 umap-project-1.3.0a0/umap/locale/is/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7603 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/is/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11110 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/it/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.544356 umap-project-1.3.0a0/umap/locale/it/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7309 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11188 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/ja/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.547689 umap-project-1.3.0a0/umap/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7672 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11240 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/ko/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.547689 umap-project-1.3.0a0/umap/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7625 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11132 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/lt/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.547689 umap-project-1.3.0a0/umap/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6845 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10659 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/ms/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.547689 umap-project-1.3.0a0/umap/locale/ms/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7577 2023-05-31 07:14:25.000000 umap-project-1.3.0a0/umap/locale/ms/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10506 2023-05-31 07:14:01.000000 umap-project-1.3.0a0/umap/locale/ms/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/nl/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.547689 umap-project-1.3.0a0/umap/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6999 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10549 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/no/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.551023 umap-project-1.3.0a0/umap/locale/no/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      423 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/no/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7998 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/no/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/pl/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.551023 umap-project-1.3.0a0/umap/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7298 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11013 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/pt/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.551023 umap-project-1.3.0a0/umap/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7256 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10828 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/pt_BR/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.551023 umap-project-1.3.0a0/umap/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7282 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10908 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/pt_PT/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.551023 umap-project-1.3.0a0/umap/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7271 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10843 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/ro/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.551023 umap-project-1.3.0a0/umap/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1482 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8428 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/ru/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.554356 umap-project-1.3.0a0/umap/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9228 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12926 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/si_LK/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.554356 umap-project-1.3.0a0/umap/locale/si_LK/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      447 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/si_LK/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8022 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/si_LK/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/sk_SK/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.554356 umap-project-1.3.0a0/umap/locale/sk_SK/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6891 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sk_SK/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10730 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sk_SK/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/sl/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.554356 umap-project-1.3.0a0/umap/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6825 2023-05-31 07:14:25.000000 umap-project-1.3.0a0/umap/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10538 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/sr/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.554356 umap-project-1.3.0a0/umap/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8830 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12352 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/sv/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.554356 umap-project-1.3.0a0/umap/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6975 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10508 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/th_TH/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.557690 umap-project-1.3.0a0/umap/locale/th_TH/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10318 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/th_TH/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13772 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/th_TH/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.524356 umap-project-1.3.0a0/umap/locale/tr/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.557690 umap-project-1.3.0a0/umap/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7375 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10952 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.524356 umap-project-1.3.0a0/umap/locale/uk_UA/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.557690 umap-project-1.3.0a0/umap/locale/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9429 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/uk_UA/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12970 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/uk_UA/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.524356 umap-project-1.3.0a0/umap/locale/vi/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.557690 umap-project-1.3.0a0/umap/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6064 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10544 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.524356 umap-project-1.3.0a0/umap/locale/zh/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.557690 umap-project-1.3.0a0/umap/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4419 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9338 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.524356 umap-project-1.3.0a0/umap/locale/zh_TW/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.561023 umap-project-1.3.0a0/umap/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6802 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10562 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.561023 umap-project-1.3.0a0/umap/management/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.3.0a0/umap/management/__init__.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.561023 umap-project-1.3.0a0/umap/management/commands/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.3.0a0/umap/management/commands/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      839 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/management/commands/anonymous_edit_url.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1298 2019-04-07 14:33:20.000000 umap-project-1.3.0a0/umap/management/commands/generate_js_locale.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1902 2019-04-07 14:28:38.000000 umap-project-1.3.0a0/umap/management/commands/import_pictograms.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      207 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/managers.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/middleware.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.561023 umap-project-1.3.0a0/umap/migrations/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5563 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/migrations/0001_initial.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      373 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/migrations/0002_tilelayer_tms.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      812 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/migrations/0003_add_tilelayer.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      530 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/migrations/0004_add_licence.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2018-07-14 11:58:47.000000 umap-project-1.3.0a0/umap/migrations/0005_remove_map_tilelayer.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      497 2019-04-07 08:09:35.000000 umap-project-1.3.0a0/umap/migrations/0006_auto_20190407_0719.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/migrations/0007_auto_20190416_1757.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      459 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/umap/migrations/0008_alter_map_settings.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      886 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/migrations/0009_star.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-11-26 16:02:45.000000 umap-project-1.3.0a0/umap/migrations/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11456 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/models.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.564356 umap-project-1.3.0a0/umap/settings/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1617 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/settings/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7642 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/settings/base.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      386 2018-05-19 15:10:46.000000 umap-project-1.3.0a0/umap/settings/dev.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.564356 umap-project-1.3.0a0/umap/static/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/.gitignore
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      638 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/favicon.ico
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.574356 umap-project-1.3.0a0/umap/static/umap/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    18104 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/base.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9125 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/umap/bitbucket.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5858 2023-05-30 06:46:59.000000 umap-project-1.3.0a0/umap/static/umap/content.css
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.577690 umap-project-1.3.0a0/umap/static/umap/font/
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   182984 2018-05-17 09:59:39.000000 umap-project-1.3.0a0/umap/static/umap/font/FiraSans-Light.woff
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   129180 2018-05-17 09:59:39.000000 umap-project-1.3.0a0/umap/static/umap/font/FiraSans-Light.woff2
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   191400 2018-05-17 09:59:39.000000 umap-project-1.3.0a0/umap/static/umap/font/FiraSans-LightItalic.woff
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   135744 2018-05-17 09:59:39.000000 umap-project-1.3.0a0/umap/static/umap/font/FiraSans-LightItalic.woff2
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   198128 2018-05-17 09:59:39.000000 umap-project-1.3.0a0/umap/static/umap/font/FiraSans-SemiBold.woff
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   140168 2018-05-17 09:59:39.000000 umap-project-1.3.0a0/umap/static/umap/font/FiraSans-SemiBold.woff2
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      832 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/font.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1564 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/umap/github.png
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.584356 umap-project-1.3.0a0/umap/static/umap/img/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13636 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/static/umap/img/16-white.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    57263 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/static/umap/img/16-white.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11308 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/img/16.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    38140 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/img/16.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    19711 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/24-white.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    38377 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/24-white.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    16878 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/24.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    36478 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/24.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      430 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/img/edit-16.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      554 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/edit.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      190 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/img/icon-bg.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      327 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/logo.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5537 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/umap/img/logo_filigree.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      375 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/img/marker.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      473 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/opensource.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1997 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/osm.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1472 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/img/search.gif
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.587690 umap-project-1.3.0a0/umap/static/umap/js/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7937 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.autocomplete.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    38967 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.controls.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    19966 2023-05-30 19:49:34.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.core.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    31642 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.features.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27320 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.forms.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5762 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.icon.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    68708 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    33580 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.layer.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5809 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.permissions.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6802 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.popup.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4421 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.slideshow.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4191 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.tableeditor.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6872 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.ui.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8711 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.xhr.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.607690 umap-project-1.3.0a0/umap/static/umap/locale/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27485 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/am_ET.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27414 2023-05-31 07:14:01.000000 umap-project-1.3.0a0/umap/static/umap/locale/am_ET.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23264 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ar.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23199 2023-05-31 07:14:01.000000 umap-project-1.3.0a0/umap/static/umap/locale/ar.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22797 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ast.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:01.000000 umap-project-1.3.0a0/umap/static/umap/locale/ast.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    26550 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/bg.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    26485 2023-05-31 07:14:01.000000 umap-project-1.3.0a0/umap/static/umap/locale/bg.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23646 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ca.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23581 2023-05-31 07:14:02.000000 umap-project-1.3.0a0/umap/static/umap/locale/ca.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24628 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/cs_CZ.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24557 2023-05-31 07:14:02.000000 umap-project-1.3.0a0/umap/static/umap/locale/cs_CZ.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23232 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/da.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23167 2023-05-31 07:14:02.000000 umap-project-1.3.0a0/umap/static/umap/locale/da.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24743 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/de.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24678 2023-05-31 07:14:03.000000 umap-project-1.3.0a0/umap/static/umap/locale/de.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    33701 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/el.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    33636 2023-05-31 07:14:02.000000 umap-project-1.3.0a0/umap/static/umap/locale/el.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22797 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/en.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22732 2023-05-31 07:12:10.000000 umap-project-1.3.0a0/umap/static/umap/locale/en.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22442 2023-05-31 07:14:04.000000 umap-project-1.3.0a0/umap/static/umap/locale/en_US.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24956 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/es.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24891 2023-05-31 07:14:04.000000 umap-project-1.3.0a0/umap/static/umap/locale/es.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23050 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/et.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22985 2023-05-31 07:14:04.000000 umap-project-1.3.0a0/umap/static/umap/locale/et.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    30194 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/fa_IR.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    30123 2023-05-31 07:14:04.000000 umap-project-1.3.0a0/umap/static/umap/locale/fa_IR.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23862 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/fi.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23797 2023-05-31 07:14:04.000000 umap-project-1.3.0a0/umap/static/umap/locale/fi.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24960 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/fr.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24895 2023-05-31 07:14:05.000000 umap-project-1.3.0a0/umap/static/umap/locale/fr.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24456 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/gl.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24391 2023-05-31 07:14:05.000000 umap-project-1.3.0a0/umap/static/umap/locale/gl.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    26905 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/he.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    26840 2023-05-31 07:14:05.000000 umap-project-1.3.0a0/umap/static/umap/locale/he.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23005 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/hr.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22940 2023-05-31 07:14:05.000000 umap-project-1.3.0a0/umap/static/umap/locale/hr.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    25810 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/hu.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    25745 2023-05-31 07:14:05.000000 umap-project-1.3.0a0/umap/static/umap/locale/hu.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22795 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/id.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:06.000000 umap-project-1.3.0a0/umap/static/umap/locale/id.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24377 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/is.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24312 2023-05-31 07:14:06.000000 umap-project-1.3.0a0/umap/static/umap/locale/is.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24474 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/it.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24409 2023-05-31 07:14:06.000000 umap-project-1.3.0a0/umap/static/umap/locale/it.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    25895 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ja.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    25830 2023-05-31 07:14:06.000000 umap-project-1.3.0a0/umap/static/umap/locale/ja.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23023 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ko.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22958 2023-05-31 07:14:06.000000 umap-project-1.3.0a0/umap/static/umap/locale/ko.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23762 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/lt.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23697 2023-05-31 07:14:08.000000 umap-project-1.3.0a0/umap/static/umap/locale/lt.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23906 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ms.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23841 2023-05-31 07:14:08.000000 umap-project-1.3.0a0/umap/static/umap/locale/ms.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24414 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/nl.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24349 2023-05-31 07:14:08.000000 umap-project-1.3.0a0/umap/static/umap/locale/nl.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23074 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/no.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23009 2023-05-31 07:14:08.000000 umap-project-1.3.0a0/umap/static/umap/locale/no.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24276 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/pl.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24211 2023-05-31 07:14:08.000000 umap-project-1.3.0a0/umap/static/umap/locale/pl.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:09.000000 umap-project-1.3.0a0/umap/static/umap/locale/pl_PL.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24433 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/pt.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24368 2023-05-31 07:14:09.000000 umap-project-1.3.0a0/umap/static/umap/locale/pt.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24422 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/pt_BR.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24351 2023-05-31 07:14:09.000000 umap-project-1.3.0a0/umap/static/umap/locale/pt_BR.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24432 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/pt_PT.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24361 2023-05-31 07:14:09.000000 umap-project-1.3.0a0/umap/static/umap/locale/pt_PT.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22856 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ro.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22791 2023-05-31 07:14:09.000000 umap-project-1.3.0a0/umap/static/umap/locale/ro.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    31470 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ru.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    31405 2023-05-31 07:14:10.000000 umap-project-1.3.0a0/umap/static/umap/locale/ru.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22801 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/si_LK.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:10.000000 umap-project-1.3.0a0/umap/static/umap/locale/si_LK.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24310 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/sk_SK.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24239 2023-05-31 07:14:10.000000 umap-project-1.3.0a0/umap/static/umap/locale/sk_SK.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24157 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/sl.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24092 2023-05-31 07:14:10.000000 umap-project-1.3.0a0/umap/static/umap/locale/sl.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27557 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/sr.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27492 2023-05-31 07:14:10.000000 umap-project-1.3.0a0/umap/static/umap/locale/sr.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24031 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/sv.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23966 2023-05-31 07:14:12.000000 umap-project-1.3.0a0/umap/static/umap/locale/sv.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22801 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/th_TH.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:12.000000 umap-project-1.3.0a0/umap/static/umap/locale/th_TH.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24649 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/tr.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24584 2023-05-31 07:14:12.000000 umap-project-1.3.0a0/umap/static/umap/locale/tr.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    31037 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/uk_UA.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    30966 2023-05-31 07:14:12.000000 umap-project-1.3.0a0/umap/static/umap/locale/uk_UA.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23174 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/vi.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23109 2023-05-31 07:14:12.000000 umap-project-1.3.0a0/umap/static/umap/locale/vi.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:13.000000 umap-project-1.3.0a0/umap/static/umap/locale/vi_VN.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22421 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/zh.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22356 2023-05-31 07:14:13.000000 umap-project-1.3.0a0/umap/static/umap/locale/zh.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:13.000000 umap-project-1.3.0a0/umap/static/umap/locale/zh_CN.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:13.000000 umap-project-1.3.0a0/umap/static/umap/locale/zh_TW.Big5.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22410 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/zh_TW.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22339 2023-05-31 07:14:13.000000 umap-project-1.3.0a0/umap/static/umap/locale/zh_TW.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    31816 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/map.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1492 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/nav.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    19408 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/umap/openstreetmap.png
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.617690 umap-project-1.3.0a0/umap/static/umap/test/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      464 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/test/.eslintrc
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1665 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/Controls.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11544 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/DataLayer.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9423 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/Feature.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    16802 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/Map.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3318 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/Marker.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2314 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/Permissions.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12614 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/test/Polygon.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13986 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/test/Polyline.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3216 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/TableEditor.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14080 2023-05-30 19:49:34.000000 umap-project-1.3.0a0/umap/static/umap/test/Util.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9840 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/_pre.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5318 2023-05-30 19:49:34.000000 umap-project-1.3.0a0/umap/static/umap/test/index.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       49 2018-06-02 13:09:22.000000 umap-project-1.3.0a0/umap/static/umap/theme.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3225 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/umap/twitter.png
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.527689 umap-project-1.3.0a0/umap/static/umap/vendors/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.621023 umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1231 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    16343 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      990 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8994 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.621023 umap-project-1.3.0a0/umap/static/umap/vendors/csv2geojson/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    15029 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/csv2geojson/csv2geojson.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6994 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/csv2geojson/index.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.621023 umap-project-1.3.0a0/umap/static/umap/vendors/dompurify/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    62738 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/dompurify/purify.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.621023 umap-project-1.3.0a0/umap/static/umap/vendors/editable/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    74768 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/editable/Leaflet.Editable.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3898 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/editable/Path.Drag.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.621023 umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1263 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9141 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3340 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/edit-in-osm.png
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.624357 umap-project-1.3.0a0/umap/static/umap/vendors/formbuilder/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12235 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.624357 umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5041 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3654 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/fullscreen.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      420 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/fullscreen@2x.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      994 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.624357 umap-project-1.3.0a0/umap/static/umap/vendors/georsstogeojson/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3202 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.624357 umap-project-1.3.0a0/umap/static/umap/vendors/hash/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3462 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/hash/leaflet-hash.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.624357 umap-project-1.3.0a0/umap/static/umap/vendors/heat/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5158 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/heat/leaflet-heat.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.624357 umap-project-1.3.0a0/umap/static/umap/vendors/i18n/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1305 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/i18n/Leaflet.i18n.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.631023 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.631023 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1259 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/layers-2x.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      696 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/layers.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2464 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1466 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/marker-icon.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      618 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/marker-shadow.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   398517 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.esm.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   759894 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   400242 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   759986 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.js.map
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14106 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   140468 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   191112 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet.js.map
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.631023 umap-project-1.3.0a0/umap/static/umap/vendors/loading/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3252 2023-05-31 07:42:57.000000 umap-project-1.3.0a0/umap/static/umap/vendors/loading/Control.Loading.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14143 2023-05-31 07:42:57.000000 umap-project-1.3.0a0/umap/static/umap/vendors/loading/Control.Loading.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.631023 umap-project-1.3.0a0/umap/static/umap/vendors/locatecontrol/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2471 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    30907 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.634357 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1346 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      886 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/MarkerCluster.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/WhereAreTheJavascriptFiles.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    80271 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   157229 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    33679 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27566 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.634357 umap-project-1.3.0a0/umap/static/umap/vendors/measurable/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      937 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/measurable/Leaflet.Measurable.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7256 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/measurable/Leaflet.Measurable.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.634357 umap-project-1.3.0a0/umap/static/umap/vendors/minimap/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1998 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/minimap/Control.MiniMap.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12129 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/minimap/Control.MiniMap.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.634357 umap-project-1.3.0a0/umap/static/umap/vendors/minimap/images/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      219 2023-05-31 07:42:55.000000 umap-project-1.3.0a0/umap/static/umap/vendors/minimap/images/toggle.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8057 2023-05-31 07:42:56.000000 umap-project-1.3.0a0/umap/static/umap/vendors/minimap/images/toggle.svg
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.634357 umap-project-1.3.0a0/umap/static/umap/vendors/osmtogeojson/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    35642 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.637690 umap-project-1.3.0a0/umap/static/umap/vendors/photon/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14433 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/photon/leaflet.photon.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.637690 umap-project-1.3.0a0/umap/static/umap/vendors/print/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    44559 2021-09-12 08:45:21.000000 umap-project-1.3.0a0/umap/static/umap/vendors/print/leaflet.browser.print.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23442 2021-09-12 08:45:21.000000 umap-project-1.3.0a0/umap/static/umap/vendors/print/leaflet.browser.print.min.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.637690 umap-project-1.3.0a0/umap/static/umap/vendors/togeojson/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    18098 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/togeojson/togeojson.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.637690 umap-project-1.3.0a0/umap/static/umap/vendors/togpx/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    17936 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/togpx/togpx.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.637690 umap-project-1.3.0a0/umap/static/umap/vendors/tokml/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11521 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/tokml/tokml.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.641023 umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2890 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9060 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2244 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5326 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.641023 umap-project-1.3.0a0/umap/templates/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      305 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/templates/404.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4904 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/templates/500.html
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.641023 umap-project-1.3.0a0/umap/templates/auth/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      467 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/templates/auth/user_detail.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      487 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/templates/auth/user_stars.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      702 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/templates/base.html
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.641023 umap-project-1.3.0a0/umap/templates/registration/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1157 2023-03-01 18:10:17.000000 umap-project-1.3.0a0/umap/templates/registration/login.html
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.647690 umap-project-1.3.0a0/umap/templates/umap/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      128 2018-05-18 20:43:08.000000 umap-project-1.3.0a0/umap/templates/umap/about.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1897 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/templates/umap/about_summary.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2857 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/templates/umap/content.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      634 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/templates/umap/content_footer.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1309 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/templates/umap/css.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-05-18 20:43:08.000000 umap-project-1.3.0a0/umap/templates/umap/footer.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      631 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/templates/umap/home.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3155 2023-05-30 19:49:34.000000 umap-project-1.3.0a0/umap/templates/umap/js.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      112 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/templates/umap/locale.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      629 2023-05-30 06:46:59.000000 umap-project-1.3.0a0/umap/templates/umap/login_popup_end.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      595 2021-09-12 08:45:40.000000 umap-project-1.3.0a0/umap/templates/umap/map_detail.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      200 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/templates/umap/map_fragment.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      165 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/templates/umap/map_init.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      597 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/templates/umap/map_list.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/templates/umap/map_messages.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1125 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/templates/umap/navigation.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      878 2018-05-18 20:43:08.000000 umap-project-1.3.0a0/umap/templates/umap/password_change.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      258 2018-05-18 20:43:08.000000 umap-project-1.3.0a0/umap/templates/umap/password_change_done.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      390 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/templates/umap/search.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      448 2018-05-18 20:43:08.000000 umap-project-1.3.0a0/umap/templates/umap/search_bar.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        2 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/templates/umap/success.html
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.647690 umap-project-1.3.0a0/umap/templatetags/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/templatetags/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2405 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/templatetags/umap_tags.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.647690 umap-project-1.3.0a0/umap/tests/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/tests/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2945 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/tests/base.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1466 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/tests/conftest.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      360 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/tests/settings.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2870 2023-02-27 10:29:01.000000 umap-project-1.3.0a0/umap/tests/test_datalayer.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7173 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/tests/test_datalayer_views.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      339 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/tests/test_licence.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3149 2018-07-14 13:10:40.000000 umap-project-1.3.0a0/umap/tests/test_map.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    20902 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/tests/test_map_views.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      605 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/tests/test_tilelayer.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      407 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/tests/test_utils.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5822 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/tests/test_views.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5304 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/urls.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4381 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/utils.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    28421 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/views.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1152 2018-05-19 15:10:36.000000 umap-project-1.3.0a0/umap/wsgi.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.651023 umap-project-1.3.0a0/umap_project.egg-info/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2167 2023-05-31 07:43:08.000000 umap-project-1.3.0a0/umap_project.egg-info/PKG-INFO
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14363 2023-05-31 07:43:08.000000 umap-project-1.3.0a0/umap_project.egg-info/SOURCES.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        1 2023-05-31 07:43:08.000000 umap-project-1.3.0a0/umap_project.egg-info/dependency_links.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       39 2023-05-31 07:43:08.000000 umap-project-1.3.0a0/umap_project.egg-info/entry_points.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      263 2023-05-31 07:43:08.000000 umap-project-1.3.0a0/umap_project.egg-info/requires.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        5 2023-05-31 07:43:08.000000 umap-project-1.3.0a0/umap_project.egg-info/top_level.txt
```

### Comparing `umap-project-1.3.0/PKG-INFO` & `umap-project-1.3.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umap-project
-Version: 1.3.0
+Version: 1.3.0a0
 Summary: Create maps with OpenStreetMap layers in a minute and embed them in your site.
 Author: Yohan Boniface
 Keywords: django leaflet geodjango openstreetmap map
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `umap-project-1.3.0/README.md` & `umap-project-1.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/setup.cfg` & `umap-project-1.3.0a0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = umap-project
-version = 1.3.0
+version = 1.3.0.alpha
 description = Create maps with OpenStreetMap layers in a minute and embed them in your site.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Yohan Boniface
 homepage = https://github.com/umap-project/umap
 keywords = django leaflet geodjango openstreetmap map
 classifiers =
```

### Comparing `umap-project-1.3.0/umap/admin.py` & `umap-project-1.3.0a0/umap/admin.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/autocomplete.py` & `umap-project-1.3.0a0/umap/autocomplete.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/decorators.py` & `umap-project-1.3.0a0/umap/decorators.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/fields.py` & `umap-project-1.3.0a0/umap/fields.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/forms.py` & `umap-project-1.3.0a0/umap/forms.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/am_ET/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/am_ET/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/am_ET/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/am_ET/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ar/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ar/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ast/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/ast/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/bg/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/bg/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ca/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ca/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/cs_CZ/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/cs_CZ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/cs_CZ/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/cs_CZ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/da/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/da/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/de/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/de/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/el/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/el/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/en/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/es/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/es/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/et/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/et/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/fa_IR/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/fa_IR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/fa_IR/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/fa_IR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/fi/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/fi/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/fr/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/fr/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,29 +1,25 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: uMap\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2013-11-22 14:00+0000\n"
-"Last-Translator: yohanboniface <yohanboniface@free.fr>, "
-"2013-2014,2018-2019,2023\n"
+"Last-Translator: yohanboniface <yohanboniface@free.fr>, 2014,2016\n"
 "Language-Team: French (http://app.transifex.com/openstreetmap/umap/language/"
 "fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid "%(current_user)s has no maps."
 msgstr "%(current_user)s n'a aucune carte."
 
-msgid "%(current_user)s has no starred maps yet."
-msgstr "%(current_user)s n'a aucune carte favorite."
-
 msgid "About"
 msgstr "À propos"
 
 msgid "Add POIs: markers, lines, polygons..."
 msgstr "Ajouter des points d'intérêt : marqueurs, lignes, polygones..."
 
 msgid "And it's <a href=\"%(repo_url)s\">open source</a>!"
@@ -31,17 +27,14 @@
 
 msgid "Batch import geostructured data (geojson, gpx, kml, osm...)"
 msgstr "Import des données géographiques en masse (geojson, gpx, kml, osm...)"
 
 msgid "Browse %(current_user)s's maps"
 msgstr "Consulter les cartes de %(current_user)s"
 
-msgid "Browse %(current_user)s's starred maps"
-msgstr "Consulter les cartes favorites de %(current_user)s"
-
 msgid "Change my password"
 msgstr "Changer de mot de passe"
 
 msgid "Change password"
 msgstr "Changer le mot de passe"
 
 msgid "Choose the layers of your map"
@@ -183,28 +176,18 @@
 
 msgid "Sign in"
 msgstr "Créer un compte"
 
 msgid "Site is readonly for maintenance"
 msgstr "Le site est en lecture seule pour maintenance."
 
-msgid "Starred maps"
-msgstr "Favoris"
-
 msgid "Take me to the home page"
 msgstr "Retour à la page d'accueil"
 
 msgid ""
-"This instance of uMap is currently in read only mode, no creation/edit is "
-"allowed."
-msgstr ""
-"uMap est actuelle en mode lecture seule, aucune création ou modification "
-"n'est possible."
-
-msgid ""
 "This is a demo instance, used for tests and pre-rolling releases. If you "
 "need a stable instance, please use <a "
 "href=\"%(stable_url)s\">%(stable_url)s</a>. You can also host your own "
 "instance, it's <a href=\"%(repo_url)s\">open source</a>!"
 msgstr ""
 "Il s'agit d'un site de démonstration, utilisé pour les tests et validation "
 "avant diffusion. Si vous avez besoin d'une version stable, utilisez plutôt "
```

### Comparing `umap-project-1.3.0/umap/locale/fr/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/fr/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -18,384 +18,374 @@
 # yohanboniface <yohanboniface@free.fr>, 2013-2014,2018-2019,2023
 # YOHAN BONIFACE <yb@enix.org>, 2012
 # yohanboniface <yohanboniface@free.fr>, 2014,2016
 msgid ""
 msgstr ""
 "Project-Id-Version: uMap\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-05-31 07:12+0000\n"
+"POT-Creation-Date: 2023-04-21 20:50+0000\n"
 "PO-Revision-Date: 2013-11-22 14:00+0000\n"
-"Last-Translator: yohanboniface <yohanboniface@free.fr>, 2013-2014,2018-2019,2023\n"
+"Last-Translator: yohanboniface <yohanboniface@free.fr>, 2014,2016\n"
 "Language-Team: French (http://app.transifex.com/openstreetmap/umap/language/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
-#: forms.py:40
+#: tmp/framacarte/templates/umap/home.html:8 umap/templates/umap/home.html:9
+#, python-format
+msgid ""
+"This is a demo instance, used for tests and pre-rolling releases. If you "
+"need a stable instance, please use <a "
+"href=\"%(stable_url)s\">%(stable_url)s</a>. You can also host your own "
+"instance, it's <a href=\"%(repo_url)s\">open source</a>!"
+msgstr "Il s'agit d'un site de démonstration, utilisé pour les tests et validation avant diffusion. Si vous avez besoin d'une version stable, utilisez plutôt <a href=\"%(stable_url)s\">%(stable_url)s</a>. Vous pouvez aussi mettre en place votre propre version, c'est <a href=\"%(repo_url)s\">open source</a>!"
+
+#: tmp/framacarte/templates/umap/home.html:83
+#: tmp/framacarte/templates/umap/navigation.html:14
+#: umap/templates/umap/about_summary.html:33
+#: umap/templates/umap/navigation.html:26
+msgid "Create a map"
+msgstr "Créer une carte"
+
+#: tmp/framacarte/templates/umap/navigation.html:7
+#: umap/templates/umap/navigation.html:10
+msgid "My maps"
+msgstr "Mes cartes"
+
+#: tmp/framacarte/templates/umap/navigation.html:9
+#: umap/templates/umap/navigation.html:12
+msgid "Log in"
+msgstr "Connexion"
+
+#: tmp/framacarte/templates/umap/navigation.html:9
+#: umap/templates/umap/navigation.html:12
+msgid "Sign in"
+msgstr "Créer un compte"
+
+#: tmp/framacarte/templates/umap/navigation.html:12
+#: umap/templates/umap/navigation.html:20
+msgid "Log out"
+msgstr "Déconnexion"
+
+#: tmp/framacarte/templates/umap/search_bar.html:6
+#: umap/templates/umap/search_bar.html:6
+msgid "Search maps"
+msgstr "Chercher des cartes"
+
+#: tmp/framacarte/templates/umap/search_bar.html:10
+#: tmp/framacarte/templates/umap/search_bar.html:13
+#: umap/templates/umap/search_bar.html:9
+msgid "Search"
+msgstr "Chercher"
+
+#: umap/forms.py:40
 #, python-format
 msgid "Secret edit link is %s"
 msgstr "Lien de modification secret : %s"
 
-#: forms.py:44 models.py:110
+#: umap/forms.py:44 umap/models.py:114
 msgid "Everyone can edit"
 msgstr "Tout le monde peut modifier"
 
-#: forms.py:45
+#: umap/forms.py:45
 msgid "Only editable with secret edit link"
 msgstr "Modifiable seulement avec le lien de modification secret"
 
-#: middleware.py:14
+#: umap/middleware.py:14
 msgid "Site is readonly for maintenance"
 msgstr "Le site est en lecture seule pour maintenance."
 
-#: models.py:16
+#: umap/models.py:16
 msgid "name"
 msgstr "nom"
 
-#: models.py:47
+#: umap/models.py:47
 msgid "details"
 msgstr "détails"
 
-#: models.py:48
+#: umap/models.py:48
 msgid "Link to a page where the licence is detailed."
 msgstr "Lien vers une page détaillant la licence."
 
-#: models.py:58
+#: umap/models.py:62
 msgid "URL template using OSM tile format"
 msgstr "Modèle d'URL au format des tuiles OSM"
 
-#: models.py:64
+#: umap/models.py:70
 msgid "Order of the tilelayers in the edit box"
 msgstr "Ordre des calques de tuiles dans le panneau de modification"
 
-#: models.py:111
+#: umap/models.py:115
 msgid "Only editors can edit"
 msgstr "Seuls les éditeurs peuvent modifier"
 
-#: models.py:112
+#: umap/models.py:116
 msgid "Only owner can edit"
 msgstr "Seul le créateur peut modifier"
 
-#: models.py:115
+#: umap/models.py:119
 msgid "everyone (public)"
 msgstr "tout le monde (public)"
 
-#: models.py:116
+#: umap/models.py:120
 msgid "anyone with link"
 msgstr "quiconque a le lien"
 
-#: models.py:117
+#: umap/models.py:121
 msgid "editors only"
 msgstr "seulement les modificateurs"
 
-#: models.py:118
+#: umap/models.py:122
 msgid "blocked"
 msgstr "Bloquée"
 
-#: models.py:121 models.py:270
+#: umap/models.py:125 umap/models.py:255
 msgid "description"
 msgstr "description"
 
-#: models.py:122
+#: umap/models.py:126
 msgid "center"
 msgstr "centre"
 
-#: models.py:123
+#: umap/models.py:127
 msgid "zoom"
 msgstr "zoom"
 
-#: models.py:125
+#: umap/models.py:128
 msgid "locate"
 msgstr "géolocaliser"
 
-#: models.py:125
+#: umap/models.py:128
 msgid "Locate user on load?"
 msgstr "Géolocaliser l'utilisateur au chargement ?"
 
-#: models.py:129
+#: umap/models.py:131
 msgid "Choose the map licence."
 msgstr "Choisir une licence pour la carte"
 
-#: models.py:130
+#: umap/models.py:132
 msgid "licence"
 msgstr "licence"
 
-#: models.py:140
+#: umap/models.py:137
 msgid "owner"
 msgstr "créateur"
 
-#: models.py:144
+#: umap/models.py:138
 msgid "editors"
 msgstr "éditeurs"
 
-#: models.py:147
+#: umap/models.py:139
 msgid "edit status"
 msgstr "statut de modification"
 
-#: models.py:150
+#: umap/models.py:140
 msgid "share status"
 msgstr "qui a accès"
 
-#: models.py:153
+#: umap/models.py:141
 msgid "settings"
 msgstr "réglages"
 
-#: models.py:225
+#: umap/models.py:209
 msgid "Clone of"
 msgstr "Clone de"
 
-#: models.py:274
+#: umap/models.py:260
 msgid "display on load"
 msgstr "afficher au chargement."
 
-#: models.py:275
+#: umap/models.py:261
 msgid "Display this layer on load."
 msgstr "Afficher ce calque au chargement."
 
-#: templates/404.html:7
+#: umap/templates/404.html:7
 msgid "Take me to the home page"
 msgstr "Retour à la page d'accueil"
 
-#: templates/auth/user_detail.html:7
+#: umap/templates/auth/user_detail.html:7
 #, python-format
 msgid "Browse %(current_user)s's maps"
 msgstr "Consulter les cartes de %(current_user)s"
 
-#: templates/auth/user_detail.html:15
+#: umap/templates/auth/user_detail.html:15
 #, python-format
 msgid "%(current_user)s has no maps."
 msgstr "%(current_user)s n'a aucune carte."
 
-#: templates/auth/user_stars.html:7
-#, python-format
-msgid "Browse %(current_user)s's starred maps"
-msgstr "Consulter les cartes favorites de %(current_user)s"
-
-#: templates/auth/user_stars.html:15
-#, python-format
-msgid "%(current_user)s has no starred maps yet."
-msgstr "%(current_user)s n'a aucune carte favorite."
-
-#: templates/registration/login.html:4
+#: umap/templates/registration/login.html:4
 msgid "Please log in with your account"
 msgstr "Identifiez-vous"
 
-#: templates/registration/login.html:18
+#: umap/templates/registration/login.html:18
 msgid "Username"
 msgstr "Nom d'utilisateur"
 
-#: templates/registration/login.html:20
+#: umap/templates/registration/login.html:20
 msgid "Password"
 msgstr "Mot de passe"
 
-#: templates/registration/login.html:21
+#: umap/templates/registration/login.html:21
 msgid "Login"
 msgstr "Connexion"
 
-#: templates/registration/login.html:27
+#: umap/templates/registration/login.html:27
 msgid "Please choose a provider"
 msgstr "Merci de choisir un fournisseur"
 
-#: templates/umap/about_summary.html:6
+#: umap/templates/umap/about_summary.html:6
 #, python-format
 msgid ""
 "uMap lets you create maps with <a href=\"%(osm_url)s\" />OpenStreetMap</a> "
 "layers in a minute and embed them in your site."
 msgstr "uMap permet de créer des cartes personnalisées sur des fonds <a href=\"%(osm_url)s\" />OpenStreetMap</a> en un instant et les afficher dans votre site."
 
-#: templates/umap/about_summary.html:11
+#: umap/templates/umap/about_summary.html:11
 msgid "Choose the layers of your map"
 msgstr "Choisir les fonds pour votre carte"
 
-#: templates/umap/about_summary.html:12
+#: umap/templates/umap/about_summary.html:12
 msgid "Add POIs: markers, lines, polygons..."
 msgstr "Ajouter des points d'intérêt : marqueurs, lignes, polygones..."
 
-#: templates/umap/about_summary.html:13
+#: umap/templates/umap/about_summary.html:13
 msgid "Manage POIs colours and icons"
 msgstr "Choisir la couleur et les icônes"
 
-#: templates/umap/about_summary.html:14
+#: umap/templates/umap/about_summary.html:14
 msgid "Manage map options: display a minimap, locate user on load…"
 msgstr "Gérer les options de la carte : afficher une minicarte, géolocaliser l'utilisateur..."
 
-#: templates/umap/about_summary.html:15
+#: umap/templates/umap/about_summary.html:15
 msgid "Batch import geostructured data (geojson, gpx, kml, osm...)"
 msgstr "Import des données géographiques en masse (geojson, gpx, kml, osm...)"
 
-#: templates/umap/about_summary.html:16
+#: umap/templates/umap/about_summary.html:16
 msgid "Choose the license for your data"
 msgstr "Choisir la licence de vos données"
 
-#: templates/umap/about_summary.html:17
+#: umap/templates/umap/about_summary.html:17
 msgid "Embed and share your map"
 msgstr "Exporter et partager votre carte"
 
-#: templates/umap/about_summary.html:23
+#: umap/templates/umap/about_summary.html:23
 #, python-format
 msgid "And it's <a href=\"%(repo_url)s\">open source</a>!"
 msgstr "Et c'est <a href=\"%(repo_url)s\">open source</a>!"
 
-#: templates/umap/about_summary.html:34 templates/umap/navigation.html:28
-msgid "Create a map"
-msgstr "Créer une carte"
-
-#: templates/umap/about_summary.html:37
+#: umap/templates/umap/about_summary.html:35
 msgid "Play with the demo"
 msgstr "Tester la démo"
 
-#: templates/umap/content.html:25
-msgid ""
-"This instance of uMap is currently in read only mode, no creation/edit is "
-"allowed."
-msgstr "uMap est actuelle en mode lecture seule, aucune création ou modification n'est possible."
-
-#: templates/umap/content.html:33
-#, python-format
-msgid ""
-"This is a demo instance, used for tests and pre-rolling releases. If you "
-"need a stable instance, please use <a "
-"href=\"%(stable_url)s\">%(stable_url)s</a>. You can also host your own "
-"instance, it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "Il s'agit d'un site de démonstration, utilisé pour les tests et validation avant diffusion. Si vous avez besoin d'une version stable, utilisez plutôt <a href=\"%(stable_url)s\">%(stable_url)s</a>. Vous pouvez aussi mettre en place votre propre version, c'est <a href=\"%(repo_url)s\">open source</a>!"
-
-#: templates/umap/home.html:10
+#: umap/templates/umap/home.html:17
 msgid "Map of the uMaps"
 msgstr "La carte des uMaps"
 
-#: templates/umap/home.html:17
+#: umap/templates/umap/home.html:24
 msgid "Get inspired, browse maps"
 msgstr "Naviguer dans les cartes"
 
-#: templates/umap/login_popup_end.html:2
+#: umap/templates/umap/login_popup_end.html:2
 msgid "You are logged in. Continuing..."
 msgstr "Vous êtes maintenant identifié. Merci de patienter..."
 
-#: templates/umap/map_list.html:7 views.py:245
+#: umap/templates/umap/map_list.html:7 umap/views.py:226
 msgid "by"
 msgstr "par"
 
-#: templates/umap/map_list.html:11
+#: umap/templates/umap/map_list.html:11
 msgid "More"
 msgstr "Plus"
 
-#: templates/umap/navigation.html:10
-msgid "My maps"
-msgstr "Mes cartes"
-
-#: templates/umap/navigation.html:11
-msgid "Starred maps"
-msgstr "Favoris"
-
-#: templates/umap/navigation.html:13
-msgid "Log in"
-msgstr "Connexion"
-
-#: templates/umap/navigation.html:13
-msgid "Sign in"
-msgstr "Créer un compte"
-
-#: templates/umap/navigation.html:15
+#: umap/templates/umap/navigation.html:14
 msgid "About"
 msgstr "À propos"
 
-#: templates/umap/navigation.html:16
+#: umap/templates/umap/navigation.html:15
 msgid "Help"
 msgstr "Aide"
 
-#: templates/umap/navigation.html:19
+#: umap/templates/umap/navigation.html:18
 msgid "Change password"
 msgstr "Changer le mot de passe"
 
-#: templates/umap/navigation.html:21
-msgid "Log out"
-msgstr "Déconnexion"
-
-#: templates/umap/password_change.html:6
+#: umap/templates/umap/password_change.html:6
 msgid "Password change"
 msgstr "Changer le mot de passe"
 
-#: templates/umap/password_change.html:7
+#: umap/templates/umap/password_change.html:7
 msgid ""
 "Please enter your old password, for security's sake, and then enter your new"
 " password twice so we can verify you typed it in correctly."
 msgstr "Merci de renseigner votre mot de passe actuel, puis deux fois le nouveau."
 
-#: templates/umap/password_change.html:12
+#: umap/templates/umap/password_change.html:12
 msgid "Old password"
 msgstr "Ancien mot de passe"
 
-#: templates/umap/password_change.html:14
+#: umap/templates/umap/password_change.html:14
 msgid "New password"
 msgstr "Nouveau mot de passe"
 
-#: templates/umap/password_change.html:16
+#: umap/templates/umap/password_change.html:16
 msgid "New password confirmation"
 msgstr "Confirmation du nouveau mot de passe"
 
-#: templates/umap/password_change.html:18
+#: umap/templates/umap/password_change.html:18
 msgid "Change my password"
 msgstr "Changer de mot de passe"
 
-#: templates/umap/password_change_done.html:6
+#: umap/templates/umap/password_change_done.html:6
 msgid "Password change successful"
 msgstr "Le mot de passe a été modifié"
 
-#: templates/umap/password_change_done.html:7
+#: umap/templates/umap/password_change_done.html:7
 msgid "Your password was changed."
 msgstr "Votre mot de passe a été modifié"
 
-#: templates/umap/search.html:13
+#: umap/templates/umap/search.html:13
 msgid "Not map found."
 msgstr "Aucune carte trouvée."
 
-#: templates/umap/search_bar.html:6
-msgid "Search maps"
-msgstr "Chercher des cartes"
-
-#: templates/umap/search_bar.html:9
-msgid "Search"
-msgstr "Chercher"
-
-#: views.py:250
+#: umap/views.py:231
 msgid "View the map"
 msgstr "Voir la carte"
 
-#: views.py:547
+#: umap/views.py:519
 #, python-format
 msgid ""
 "Your map has been created! If you want to edit this map from another "
 "computer, please use this link: %(anonymous_url)s"
 msgstr "Votre carte a été créée ! Si vous souhaitez la modifier depuis un autre ordinateur, veuillez utiliser ce lien : %(anonymous_url)s"
 
-#: views.py:552
+#: umap/views.py:524
 msgid "Congratulations, your map has been created!"
 msgstr "Félicitations, votre carte a bien été créée !"
 
-#: views.py:582
+#: umap/views.py:554
 msgid "Map has been updated!"
 msgstr "La carte a été mise à jour !"
 
-#: views.py:607
+#: umap/views.py:579
 msgid "Map editors updated with success!"
 msgstr "Éditeurs de la carte mis à jour !"
 
-#: views.py:632
+#: umap/views.py:604
 msgid "Only its owner can delete the map."
 msgstr "Seul le créateur de la carte peut la supprimer."
 
-#: views.py:655
+#: umap/views.py:627
 #, python-format
 msgid ""
 "Your map has been cloned! If you want to edit this map from another "
 "computer, please use this link: %(anonymous_url)s"
 msgstr "Votre carte a été dupliquée ! Si vous souhaitez la modifier depuis un autre ordinateur, veuillez utiliser ce lien : %(anonymous_url)s"
 
-#: views.py:660
+#: umap/views.py:632
 msgid "Congratulations, your map has been cloned!"
 msgstr "Votre carte a été dupliquée !"
 
-#: views.py:826
+#: umap/views.py:787
 msgid "Layer successfully deleted."
 msgstr "Calque supprimé."
```

### Comparing `umap-project-1.3.0/umap/locale/gl/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/gl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/gl/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/he/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/he/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/hr/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/hr/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/hu/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/hu/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/id/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/is/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/is/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/is/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/it/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/it/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ja/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ja/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ko/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ko/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/lt/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/lt/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ms/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/ms/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ms/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/ms/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/nl/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/nl/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/no/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/no/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/pl/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/pl/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/pt/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/pt/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/pt_BR/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/pt_BR/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/pt_PT/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/pt_PT/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ro/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ro/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ru/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/ru/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/si_LK/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/si_LK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/sk_SK/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/sk_SK/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/sk_SK/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/sk_SK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/sl/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/sl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/sl/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/sr/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/sr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/sr/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/sv/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/sv/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/th_TH/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/th_TH/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/th_TH/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/th_TH/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/tr/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/tr/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/uk_UA/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/uk_UA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/uk_UA/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/uk_UA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/vi/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/vi/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/zh/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/zh/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/zh_TW/LC_MESSAGES/django.mo` & `umap-project-1.3.0a0/umap/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/locale/zh_TW/LC_MESSAGES/django.po` & `umap-project-1.3.0a0/umap/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/management/commands/anonymous_edit_url.py` & `umap-project-1.3.0a0/umap/management/commands/anonymous_edit_url.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/management/commands/generate_js_locale.py` & `umap-project-1.3.0a0/umap/management/commands/generate_js_locale.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/management/commands/import_pictograms.py` & `umap-project-1.3.0a0/umap/management/commands/import_pictograms.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/middleware.py` & `umap-project-1.3.0a0/umap/middleware.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/migrations/0001_initial.py` & `umap-project-1.3.0a0/umap/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/migrations/0003_add_tilelayer.py` & `umap-project-1.3.0a0/umap/migrations/0003_add_tilelayer.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/migrations/0004_add_licence.py` & `umap-project-1.3.0a0/umap/migrations/0004_add_licence.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/migrations/0007_auto_20190416_1757.py` & `umap-project-1.3.0a0/umap/migrations/0007_auto_20190416_1757.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/migrations/0009_star.py` & `umap-project-1.3.0a0/umap/migrations/0009_star.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/models.py` & `umap-project-1.3.0a0/umap/models.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/settings/__init__.py` & `umap-project-1.3.0a0/umap/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/settings/base.py` & `umap-project-1.3.0a0/umap/settings/base.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/favicon.ico` & `umap-project-1.3.0a0/umap/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/base.css` & `umap-project-1.3.0a0/umap/static/umap/base.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/bitbucket.png` & `umap-project-1.3.0a0/umap/static/umap/bitbucket.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/content.css` & `umap-project-1.3.0a0/umap/static/umap/content.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/font/FiraSans-Light.woff` & `umap-project-1.3.0a0/umap/static/umap/font/FiraSans-Light.woff`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/font/FiraSans-Light.woff2` & `umap-project-1.3.0a0/umap/static/umap/font/FiraSans-Light.woff2`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/font/FiraSans-LightItalic.woff` & `umap-project-1.3.0a0/umap/static/umap/font/FiraSans-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/font/FiraSans-LightItalic.woff2` & `umap-project-1.3.0a0/umap/static/umap/font/FiraSans-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/font/FiraSans-SemiBold.woff` & `umap-project-1.3.0a0/umap/static/umap/font/FiraSans-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/font/FiraSans-SemiBold.woff2` & `umap-project-1.3.0a0/umap/static/umap/font/FiraSans-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/font.css` & `umap-project-1.3.0a0/umap/static/umap/font.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/github.png` & `umap-project-1.3.0a0/umap/static/umap/github.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/img/16-white.png` & `umap-project-1.3.0a0/umap/static/umap/img/16-white.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/img/16-white.svg` & `umap-project-1.3.0a0/umap/static/umap/img/16-white.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/img/16.png` & `umap-project-1.3.0a0/umap/static/umap/img/16.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/img/16.svg` & `umap-project-1.3.0a0/umap/static/umap/img/16.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/img/24-white.png` & `umap-project-1.3.0a0/umap/static/umap/img/24-white.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/img/24-white.svg` & `umap-project-1.3.0a0/umap/static/umap/img/24-white.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/img/24.png` & `umap-project-1.3.0a0/umap/static/umap/img/24.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/img/24.svg` & `umap-project-1.3.0a0/umap/static/umap/img/24.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/img/edit.svg` & `umap-project-1.3.0a0/umap/static/umap/img/edit.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/img/logo_filigree.png` & `umap-project-1.3.0a0/umap/static/umap/img/logo_filigree.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/img/osm.svg` & `umap-project-1.3.0a0/umap/static/umap/img/osm.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/img/search.gif` & `umap-project-1.3.0a0/umap/static/umap/img/search.gif`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.autocomplete.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.autocomplete.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.controls.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.controls.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1283,15 +1283,15 @@
         }
         const currentView = this.options.currentView ? window.location.hash : ''
         return `${this.baseUrl}?${L.Util.buildQueryString(this.queryString)}${currentView}`
     },
 
     build: function() {
         const iframeUrl = this.buildUrl()
-        let code = `<iframe width="${this.dimensions.width}" height="${this.dimensions.height}" frameborder="0" allowfullscreen allow="geolocation" src="${iframeUrl}"></iframe>`
+        const code = `<iframe width="${this.dimensions.width}" height="${this.dimensions.height}" frameborder="0" allowfullscreen allow="geolocation" src="${iframeUrl}"></iframe>`
         if (this.options.includeFullScreenLink) {
             code += `<p><a href="${this.baseUrl}">${L._('See full screen')}</a></p>`
         }
         return code
     },
 })
```

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.core.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.core.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.features.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.features.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.forms.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.forms.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.icon.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.icon.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.layer.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.layer.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.permissions.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.permissions.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.popup.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.popup.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.slideshow.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.slideshow.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.tableeditor.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.tableeditor.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.ui.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.ui.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/js/umap.xhr.js` & `umap-project-1.3.0a0/umap/static/umap/js/umap.xhr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/am_ET.js` & `umap-project-1.3.0a0/umap/static/umap/locale/am_ET.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/am_ET.json` & `umap-project-1.3.0a0/umap/static/umap/locale/am_ET.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ar.js` & `umap-project-1.3.0a0/umap/static/umap/locale/ar.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ar.json` & `umap-project-1.3.0a0/umap/static/umap/locale/ar.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ast.js` & `umap-project-1.3.0a0/umap/static/umap/locale/ast.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ast.json` & `umap-project-1.3.0a0/umap/static/umap/locale/ast.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/bg.js` & `umap-project-1.3.0a0/umap/static/umap/locale/bg.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/bg.json` & `umap-project-1.3.0a0/umap/static/umap/locale/bg.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ca.js` & `umap-project-1.3.0a0/umap/static/umap/locale/ca.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ca.json` & `umap-project-1.3.0a0/umap/static/umap/locale/ca.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/cs_CZ.js` & `umap-project-1.3.0a0/umap/static/umap/locale/cs_CZ.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/cs_CZ.json` & `umap-project-1.3.0a0/umap/static/umap/locale/cs_CZ.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/da.js` & `umap-project-1.3.0a0/umap/static/umap/locale/da.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/da.json` & `umap-project-1.3.0a0/umap/static/umap/locale/da.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/de.js` & `umap-project-1.3.0a0/umap/static/umap/locale/de.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/de.json` & `umap-project-1.3.0a0/umap/static/umap/locale/de.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/el.js` & `umap-project-1.3.0a0/umap/static/umap/locale/el.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/el.json` & `umap-project-1.3.0a0/umap/static/umap/locale/el.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/en.js` & `umap-project-1.3.0a0/umap/static/umap/locale/en.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/en.json` & `umap-project-1.3.0a0/umap/static/umap/locale/en.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/en_US.json` & `umap-project-1.3.0a0/umap/static/umap/locale/en_US.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/es.js` & `umap-project-1.3.0a0/umap/static/umap/locale/es.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/es.json` & `umap-project-1.3.0a0/umap/static/umap/locale/es.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/et.js` & `umap-project-1.3.0a0/umap/static/umap/locale/et.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/et.json` & `umap-project-1.3.0a0/umap/static/umap/locale/et.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/fa_IR.js` & `umap-project-1.3.0a0/umap/static/umap/locale/fa_IR.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/fa_IR.json` & `umap-project-1.3.0a0/umap/static/umap/locale/fa_IR.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/fi.js` & `umap-project-1.3.0a0/umap/static/umap/locale/fi.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/fi.json` & `umap-project-1.3.0a0/umap/static/umap/locale/fi.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/fr.js` & `umap-project-1.3.0a0/umap/static/umap/locale/fr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/fr.json` & `umap-project-1.3.0a0/umap/static/umap/locale/fr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/gl.js` & `umap-project-1.3.0a0/umap/static/umap/locale/gl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/gl.json` & `umap-project-1.3.0a0/umap/static/umap/locale/gl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/he.js` & `umap-project-1.3.0a0/umap/static/umap/locale/he.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/he.json` & `umap-project-1.3.0a0/umap/static/umap/locale/he.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/hr.js` & `umap-project-1.3.0a0/umap/static/umap/locale/hr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/hr.json` & `umap-project-1.3.0a0/umap/static/umap/locale/hr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/hu.js` & `umap-project-1.3.0a0/umap/static/umap/locale/hu.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/hu.json` & `umap-project-1.3.0a0/umap/static/umap/locale/hu.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/id.js` & `umap-project-1.3.0a0/umap/static/umap/locale/id.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/id.json` & `umap-project-1.3.0a0/umap/static/umap/locale/id.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/is.js` & `umap-project-1.3.0a0/umap/static/umap/locale/is.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/is.json` & `umap-project-1.3.0a0/umap/static/umap/locale/is.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/it.js` & `umap-project-1.3.0a0/umap/static/umap/locale/it.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/it.json` & `umap-project-1.3.0a0/umap/static/umap/locale/it.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ja.js` & `umap-project-1.3.0a0/umap/static/umap/locale/ja.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ja.json` & `umap-project-1.3.0a0/umap/static/umap/locale/ja.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ko.js` & `umap-project-1.3.0a0/umap/static/umap/locale/ko.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ko.json` & `umap-project-1.3.0a0/umap/static/umap/locale/ko.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/lt.js` & `umap-project-1.3.0a0/umap/static/umap/locale/lt.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/lt.json` & `umap-project-1.3.0a0/umap/static/umap/locale/lt.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ms.js` & `umap-project-1.3.0a0/umap/static/umap/locale/ms.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ms.json` & `umap-project-1.3.0a0/umap/static/umap/locale/ms.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/nl.js` & `umap-project-1.3.0a0/umap/static/umap/locale/nl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/nl.json` & `umap-project-1.3.0a0/umap/static/umap/locale/nl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/no.js` & `umap-project-1.3.0a0/umap/static/umap/locale/no.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/no.json` & `umap-project-1.3.0a0/umap/static/umap/locale/no.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/pl.js` & `umap-project-1.3.0a0/umap/static/umap/locale/pl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/pl.json` & `umap-project-1.3.0a0/umap/static/umap/locale/pl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/pl_PL.json` & `umap-project-1.3.0a0/umap/static/umap/locale/pl_PL.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/pt.js` & `umap-project-1.3.0a0/umap/static/umap/locale/pt.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/pt.json` & `umap-project-1.3.0a0/umap/static/umap/locale/pt.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/pt_BR.js` & `umap-project-1.3.0a0/umap/static/umap/locale/pt_BR.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/pt_BR.json` & `umap-project-1.3.0a0/umap/static/umap/locale/pt_BR.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/pt_PT.js` & `umap-project-1.3.0a0/umap/static/umap/locale/pt_PT.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/pt_PT.json` & `umap-project-1.3.0a0/umap/static/umap/locale/pt_PT.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ro.js` & `umap-project-1.3.0a0/umap/static/umap/locale/ro.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ro.json` & `umap-project-1.3.0a0/umap/static/umap/locale/ro.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ru.js` & `umap-project-1.3.0a0/umap/static/umap/locale/ru.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/ru.json` & `umap-project-1.3.0a0/umap/static/umap/locale/ru.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/si_LK.js` & `umap-project-1.3.0a0/umap/static/umap/locale/si_LK.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/si_LK.json` & `umap-project-1.3.0a0/umap/static/umap/locale/si_LK.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/sk_SK.js` & `umap-project-1.3.0a0/umap/static/umap/locale/sk_SK.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/sk_SK.json` & `umap-project-1.3.0a0/umap/static/umap/locale/sk_SK.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/sl.js` & `umap-project-1.3.0a0/umap/static/umap/locale/sl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/sl.json` & `umap-project-1.3.0a0/umap/static/umap/locale/sl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/sr.js` & `umap-project-1.3.0a0/umap/static/umap/locale/sr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/sr.json` & `umap-project-1.3.0a0/umap/static/umap/locale/sr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/sv.js` & `umap-project-1.3.0a0/umap/static/umap/locale/sv.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/sv.json` & `umap-project-1.3.0a0/umap/static/umap/locale/sv.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/th_TH.js` & `umap-project-1.3.0a0/umap/static/umap/locale/th_TH.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/th_TH.json` & `umap-project-1.3.0a0/umap/static/umap/locale/th_TH.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/tr.js` & `umap-project-1.3.0a0/umap/static/umap/locale/tr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/tr.json` & `umap-project-1.3.0a0/umap/static/umap/locale/tr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/uk_UA.js` & `umap-project-1.3.0a0/umap/static/umap/locale/uk_UA.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/uk_UA.json` & `umap-project-1.3.0a0/umap/static/umap/locale/uk_UA.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/vi.js` & `umap-project-1.3.0a0/umap/static/umap/locale/vi.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/vi.json` & `umap-project-1.3.0a0/umap/static/umap/locale/vi.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/vi_VN.json` & `umap-project-1.3.0a0/umap/static/umap/locale/vi_VN.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/zh.js` & `umap-project-1.3.0a0/umap/static/umap/locale/zh.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/zh.json` & `umap-project-1.3.0a0/umap/static/umap/locale/zh.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/zh_CN.json` & `umap-project-1.3.0a0/umap/static/umap/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/zh_TW.Big5.json` & `umap-project-1.3.0a0/umap/static/umap/locale/zh_TW.Big5.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/zh_TW.js` & `umap-project-1.3.0a0/umap/static/umap/locale/zh_TW.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/locale/zh_TW.json` & `umap-project-1.3.0a0/umap/static/umap/locale/zh_TW.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/map.css` & `umap-project-1.3.0a0/umap/static/umap/map.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/nav.css` & `umap-project-1.3.0a0/umap/static/umap/nav.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/openstreetmap.png` & `umap-project-1.3.0a0/umap/static/umap/openstreetmap.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/test/Controls.js` & `umap-project-1.3.0a0/umap/static/umap/test/Controls.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/test/DataLayer.js` & `umap-project-1.3.0a0/umap/static/umap/test/DataLayer.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/test/Feature.js` & `umap-project-1.3.0a0/umap/static/umap/test/Feature.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/test/Map.js` & `umap-project-1.3.0a0/umap/static/umap/test/Map.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/test/Marker.js` & `umap-project-1.3.0a0/umap/static/umap/test/Marker.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/test/Permissions.js` & `umap-project-1.3.0a0/umap/static/umap/test/Permissions.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/test/Polygon.js` & `umap-project-1.3.0a0/umap/static/umap/test/Polygon.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/test/Polyline.js` & `umap-project-1.3.0a0/umap/static/umap/test/Polyline.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/test/TableEditor.js` & `umap-project-1.3.0a0/umap/static/umap/test/TableEditor.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/test/Util.js` & `umap-project-1.3.0a0/umap/static/umap/test/Util.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/test/_pre.js` & `umap-project-1.3.0a0/umap/static/umap/test/_pre.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/test/index.html` & `umap-project-1.3.0a0/umap/static/umap/test/index.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/twitter.png` & `umap-project-1.3.0a0/umap/static/umap/twitter.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/csv2geojson/csv2geojson.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/csv2geojson/csv2geojson.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/csv2geojson/index.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/csv2geojson/index.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/dompurify/purify.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/dompurify/purify.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/editable/Leaflet.Editable.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/editable/Leaflet.Editable.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/editable/Path.Drag.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/editable/Path.Drag.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/editinosm/edit-in-osm.png` & `umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/edit-in-osm.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/hash/leaflet-hash.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/hash/leaflet-hash.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/heat/leaflet-heat.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/heat/leaflet-heat.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/i18n/Leaflet.i18n.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/i18n/Leaflet.i18n.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/leaflet/images/layers-2x.png` & `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/leaflet/images/layers.png` & `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png` & `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/leaflet/images/marker-icon.png` & `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/leaflet/images/marker-shadow.png` & `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet-src.esm.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.esm.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map` & `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet-src.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet-src.js.map` & `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/leaflet/leaflet.js.map` & `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/loading/Control.Loading.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/loading/Control.Loading.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/loading/Control.Loading.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/loading/Control.Loading.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/markercluster/MarkerCluster.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/MarkerCluster.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map` & `umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/markercluster/leaflet.markercluster.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map` & `umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/measurable/Leaflet.Measurable.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/measurable/Leaflet.Measurable.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/measurable/Leaflet.Measurable.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/measurable/Leaflet.Measurable.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/minimap/Control.MiniMap.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/minimap/Control.MiniMap.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/minimap/Control.MiniMap.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/minimap/Control.MiniMap.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/minimap/images/toggle.svg` & `umap-project-1.3.0a0/umap/static/umap/vendors/minimap/images/toggle.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/photon/leaflet.photon.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/photon/leaflet.photon.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/print/leaflet.browser.print.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/print/leaflet.browser.print.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/print/leaflet.browser.print.min.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/print/leaflet.browser.print.min.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/togeojson/togeojson.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/togeojson/togeojson.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/togpx/togpx.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/togpx/togpx.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/tokml/tokml.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/tokml/tokml.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/toolbar/leaflet.toolbar.css` & `umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/static/umap/vendors/toolbar/leaflet.toolbar.js` & `umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/500.html` & `umap-project-1.3.0a0/umap/templates/500.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/base.html` & `umap-project-1.3.0a0/umap/templates/base.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/registration/login.html` & `umap-project-1.3.0a0/umap/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/umap/about_summary.html` & `umap-project-1.3.0a0/umap/templates/umap/about_summary.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/umap/content.html` & `umap-project-1.3.0a0/umap/templates/umap/content.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/umap/content_footer.html` & `umap-project-1.3.0a0/umap/templates/umap/content_footer.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/umap/css.html` & `umap-project-1.3.0a0/umap/templates/umap/css.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/umap/home.html` & `umap-project-1.3.0a0/umap/templates/umap/home.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/umap/js.html` & `umap-project-1.3.0a0/umap/templates/umap/js.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/umap/login_popup_end.html` & `umap-project-1.3.0a0/umap/templates/umap/login_popup_end.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/umap/map_detail.html` & `umap-project-1.3.0a0/umap/templates/umap/map_detail.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/umap/map_list.html` & `umap-project-1.3.0a0/umap/templates/umap/map_list.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/umap/navigation.html` & `umap-project-1.3.0a0/umap/templates/umap/navigation.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templates/umap/password_change.html` & `umap-project-1.3.0a0/umap/templates/umap/password_change.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/templatetags/umap_tags.py` & `umap-project-1.3.0a0/umap/templatetags/umap_tags.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/tests/base.py` & `umap-project-1.3.0a0/umap/tests/base.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/tests/conftest.py` & `umap-project-1.3.0a0/umap/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/tests/test_datalayer.py` & `umap-project-1.3.0a0/umap/tests/test_datalayer.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/tests/test_datalayer_views.py` & `umap-project-1.3.0a0/umap/tests/test_datalayer_views.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/tests/test_map.py` & `umap-project-1.3.0a0/umap/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/tests/test_map_views.py` & `umap-project-1.3.0a0/umap/tests/test_map_views.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/tests/test_tilelayer.py` & `umap-project-1.3.0a0/umap/tests/test_tilelayer.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/tests/test_views.py` & `umap-project-1.3.0a0/umap/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/urls.py` & `umap-project-1.3.0a0/umap/urls.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/utils.py` & `umap-project-1.3.0a0/umap/utils.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/views.py` & `umap-project-1.3.0a0/umap/views.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap/wsgi.py` & `umap-project-1.3.0a0/umap/wsgi.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0/umap_project.egg-info/PKG-INFO` & `umap-project-1.3.0a0/umap_project.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umap-project
-Version: 1.3.0
+Version: 1.3.0a0
 Summary: Create maps with OpenStreetMap layers in a minute and embed them in your site.
 Author: Yohan Boniface
 Keywords: django leaflet geodjango openstreetmap map
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `umap-project-1.3.0/umap_project.egg-info/SOURCES.txt` & `umap-project-1.3.0a0/umap_project.egg-info/SOURCES.txt`

 * *Files identical despite different names*

