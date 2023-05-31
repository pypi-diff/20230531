# Comparing `tmp/cubicweb-eac-1.5.3.tar.gz` & `tmp/cubicweb-eac-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-eac-1.5.3.tar", last modified: Wed May 31 14:56:51 2023, max compression
+gzip compressed data, was "cubicweb-eac-2.0.0.tar", last modified: Wed Dec 21 22:21:53 2022, max compression
```

## Comparing `cubicweb-eac-1.5.3.tar` & `cubicweb-eac-2.0.0.tar`

### file list

```diff
@@ -1,79 +1,77 @@
-drwxr-xr-x   0 ethieblin  (1000) ethieblin  (1001)        0 2023-05-31 14:56:51.396636 cubicweb-eac-1.5.3/
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      505 2021-09-12 15:52:26.000000 cubicweb-eac-1.5.3/MANIFEST.in
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      634 2023-05-31 14:56:51.396636 cubicweb-eac-1.5.3/PKG-INFO
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)       72 2021-08-26 09:49:38.000000 cubicweb-eac-1.5.3/README.rst
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      497 2022-04-21 15:02:41.000000 cubicweb-eac-1.5.3/a.txt
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      497 2022-04-21 15:02:56.000000 cubicweb-eac-1.5.3/b.txt
-drwxr-xr-x   0 ethieblin  (1000) ethieblin  (1001)        0 2023-05-31 14:56:51.384636 cubicweb-eac-1.5.3/cubicweb_eac/
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      618 2022-07-13 14:52:43.000000 cubicweb-eac-1.5.3/cubicweb_eac/__init__.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      972 2023-05-31 12:51:19.000000 cubicweb-eac-1.5.3/cubicweb_eac/__pkginfo__.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     4450 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/cubicweb_eac/ccplugin.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    51928 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/cubicweb_eac/dataimport.py
-drwxr-xr-x   0 ethieblin  (1000) ethieblin  (1001)        0 2023-05-31 14:56:51.388636 cubicweb-eac-1.5.3/cubicweb_eac/entities/
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    30532 2023-05-31 12:51:19.000000 cubicweb-eac-1.5.3/cubicweb_eac/entities/__init__.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    32747 2023-05-31 12:51:19.000000 cubicweb-eac-1.5.3/cubicweb_eac/entities/rdf.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     4602 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/cubicweb_eac/hooks.py
-drwxr-xr-x   0 ethieblin  (1000) ethieblin  (1001)        0 2023-05-31 14:56:51.388636 cubicweb-eac-1.5.3/cubicweb_eac/i18n/
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    27634 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/cubicweb_eac/i18n/en.po
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    32064 2021-08-26 09:49:38.000000 cubicweb-eac-1.5.3/cubicweb_eac/i18n/fr.po
-drwxr-xr-x   0 ethieblin  (1000) ethieblin  (1001)        0 2023-05-31 14:56:51.388636 cubicweb-eac-1.5.3/cubicweb_eac/migration/
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      107 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/cubicweb_eac/migration/0.2.0_Any.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      784 2022-02-10 10:42:47.000000 cubicweb-eac-1.5.3/cubicweb_eac/migration/0.3.0_Any.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)       40 2021-08-26 09:49:38.000000 cubicweb-eac-1.5.3/cubicweb_eac/migration/0.3.1_Any.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      483 2021-08-26 09:49:38.000000 cubicweb-eac-1.5.3/cubicweb_eac/migration/0.5.0_Any.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)       37 2021-08-26 09:49:38.000000 cubicweb-eac-1.5.3/cubicweb_eac/migration/0.5.1_Any.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)       41 2021-08-26 09:49:38.000000 cubicweb-eac-1.5.3/cubicweb_eac/migration/0.6.0_Any.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)       40 2021-08-26 09:49:38.000000 cubicweb-eac-1.5.3/cubicweb_eac/migration/0.8.0_Any.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      216 2021-08-26 09:49:38.000000 cubicweb-eac-1.5.3/cubicweb_eac/migration/0.8.1_Any.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     2534 2023-05-31 09:50:10.000000 cubicweb-eac-1.5.3/cubicweb_eac/migration/0.9.0_Any.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     1082 2022-01-07 13:42:46.000000 cubicweb-eac-1.5.3/cubicweb_eac/migration/postcreate.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    18155 2022-01-07 13:42:46.000000 cubicweb-eac-1.5.3/cubicweb_eac/schema.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     5055 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/cubicweb_eac/sobjects.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     2783 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/cubicweb_eac/testutils.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    13338 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/cubicweb_eac/views.py
-drwxr-xr-x   0 ethieblin  (1000) ethieblin  (1001)        0 2023-05-31 14:56:51.388636 cubicweb-eac-1.5.3/cubicweb_eac.egg-info/
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      634 2023-05-31 14:56:51.000000 cubicweb-eac-1.5.3/cubicweb_eac.egg-info/PKG-INFO
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     1881 2023-05-31 14:56:51.000000 cubicweb-eac-1.5.3/cubicweb_eac.egg-info/SOURCES.txt
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)        1 2023-05-31 14:56:51.000000 cubicweb-eac-1.5.3/cubicweb_eac.egg-info/dependency_links.txt
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)       37 2023-05-31 14:56:51.000000 cubicweb-eac-1.5.3/cubicweb_eac.egg-info/entry_points.txt
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)        1 2020-08-26 07:48:47.000000 cubicweb-eac-1.5.3/cubicweb_eac.egg-info/not-zip-safe
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      136 2023-05-31 14:56:51.000000 cubicweb-eac-1.5.3/cubicweb_eac.egg-info/requires.txt
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)       13 2023-05-31 14:56:51.000000 cubicweb-eac-1.5.3/cubicweb_eac.egg-info/top_level.txt
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)       21 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/dev-requirements.txt
-drwxr-xr-x   0 ethieblin  (1000) ethieblin  (1001)        0 2023-05-31 14:56:51.388636 cubicweb-eac-1.5.3/doc/
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     4685 2020-08-26 07:37:21.000000 cubicweb-eac-1.5.3/doc/supported.rst
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)       38 2023-05-31 14:56:51.396636 cubicweb-eac-1.5.3/setup.cfg
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     2590 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/setup.py
-drwxr-xr-x   0 ethieblin  (1000) ethieblin  (1001)        0 2023-05-31 14:56:51.392636 cubicweb-eac-1.5.3/test/
-drwxr-xr-x   0 ethieblin  (1000) ethieblin  (1001)        0 2023-05-31 14:56:51.396636 cubicweb-eac-1.5.3/test/data/
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    33823 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/test/data/FRAD033_EAC_00001.xml
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    16116 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/test/data/FRAD033_EAC_00001_simplified.xml
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     6755 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/test/data/FRAD033_EAC_00001_simplified_export.xml
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    35699 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/test/data/FRAD033_EAC_00003.xml
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     8814 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/test/data/FRAD033_EAC_00071.xml
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    15266 2022-04-19 08:52:54.000000 cubicweb-eac-1.5.3/test/data/FRAN_NP_050553.xml
--rw-rw-r--   0 ethieblin  (1000) ethieblin  (1001)    15383 2021-06-29 11:36:12.000000 cubicweb-eac-1.5.3/test/data/FRAN_NP_050805.xml
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     9771 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/test/data/Service de l'administration generale et des assemblees.xml
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)        4 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/test/data/bootstrap_cubes
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    41510 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/test/data/cpf.xsd
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      813 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/test/data/custom_kind.xml
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     1880 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/test/data/family_rico.ttl
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)       22 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/test/data/invalid_xml.xml
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     3923 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/test/data/missing_tag.xml
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      625 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/test/data/no_name_entry.xml
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      645 2020-08-25 14:19:18.000000 cubicweb-eac-1.5.3/test/data/no_name_entry_part.xml
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      321 2023-05-31 09:47:59.000000 cubicweb-eac-1.5.3/test/data/organization_rdf.ttl
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     2176 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/test/data/organization_rico.ttl
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)      375 2023-05-31 09:47:29.000000 cubicweb-eac-1.5.3/test/data/person_rdf.ttl
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     3282 2023-05-31 09:45:53.000000 cubicweb-eac-1.5.3/test/data/person_rico.ttl
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     7619 2021-08-26 09:49:38.000000 cubicweb-eac-1.5.3/test/export-roundtrip.rst
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     4177 2021-08-26 09:49:38.000000 cubicweb-eac-1.5.3/test/export-simple.rst
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    61016 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/test/test_dataimport.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     6784 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/test/test_entities.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     1081 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/test/test_export.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     3260 2022-02-10 10:42:47.000000 cubicweb-eac-1.5.3/test/test_hooks.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     9854 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/test/test_rdf.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)    11392 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/test/test_schema.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     7285 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/test/test_views.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     1081 2022-05-05 10:13:56.000000 cubicweb-eac-1.5.3/test/utils.py
--rw-r--r--   0 ethieblin  (1000) ethieblin  (1001)     1198 2023-05-31 09:44:50.000000 cubicweb-eac-1.5.3/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 22:21:53.238659 cubicweb-eac-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      505 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      599 2022-12-21 22:21:53.238659 cubicweb-eac-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       72 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 22:21:53.214658 cubicweb-eac-2.0.0/cubicweb_eac/
+-rw-rw-rw-   0 root         (0) root         (0)      618 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      972 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4458 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/ccplugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    50675 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/dataimport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 22:21:53.214658 cubicweb-eac-2.0.0/cubicweb_eac/entities/
+-rw-rw-rw-   0 root         (0) root         (0)    30509 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/entities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32724 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/entities/rdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4592 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 22:21:53.214658 cubicweb-eac-2.0.0/cubicweb_eac/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    27634 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)    32064 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 22:21:53.222658 cubicweb-eac-2.0.0/cubicweb_eac/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/migration/0.2.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      784 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/migration/0.3.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/migration/0.3.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      483 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/migration/0.5.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/migration/0.5.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/migration/0.6.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/migration/0.8.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/migration/0.8.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/migration/0.9.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    18155 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     5048 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/sobjects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/testutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    13334 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/cubicweb_eac/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 22:21:53.214658 cubicweb-eac-2.0.0/cubicweb_eac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      599 2022-12-21 22:21:52.000000 cubicweb-eac-2.0.0/cubicweb_eac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1849 2022-12-21 22:21:53.000000 cubicweb-eac-2.0.0/cubicweb_eac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-21 22:21:52.000000 cubicweb-eac-2.0.0/cubicweb_eac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2022-12-21 22:21:52.000000 cubicweb-eac-2.0.0/cubicweb_eac.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-21 22:21:52.000000 cubicweb-eac-2.0.0/cubicweb_eac.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      136 2022-12-21 22:21:53.000000 cubicweb-eac-2.0.0/cubicweb_eac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-12-21 22:21:53.000000 cubicweb-eac-2.0.0/cubicweb_eac.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/dev-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 22:21:53.222658 cubicweb-eac-2.0.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     4685 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/doc/supported.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2022-12-21 22:21:53.238659 cubicweb-eac-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 22:21:53.226659 cubicweb-eac-2.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 22:21:53.238659 cubicweb-eac-2.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)    33823 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/FRAD033_EAC_00001.xml
+-rw-rw-rw-   0 root         (0) root         (0)    16116 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/FRAD033_EAC_00001_simplified.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6755 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/FRAD033_EAC_00001_simplified_export.xml
+-rw-rw-rw-   0 root         (0) root         (0)    35699 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/FRAD033_EAC_00003.xml
+-rw-rw-rw-   0 root         (0) root         (0)     8814 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/FRAD033_EAC_00071.xml
+-rw-rw-rw-   0 root         (0) root         (0)     9771 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/Service de l'administration generale et des assemblees.xml
+-rw-rw-rw-   0 root         (0) root         (0)        4 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)    41449 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/cpf.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      813 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/custom_kind.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1568 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/family_rico.ttl
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/invalid_xml.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3923 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/missing_tag.xml
+-rw-rw-rw-   0 root         (0) root         (0)      625 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/no_name_entry.xml
+-rw-rw-rw-   0 root         (0) root         (0)      645 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/no_name_entry_part.xml
+-rw-rw-rw-   0 root         (0) root         (0)      296 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/organization_rdf.ttl
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/organization_rico.ttl
+-rw-rw-rw-   0 root         (0) root         (0)      350 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/person_rdf.ttl
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/person_rico.ttl
+-rw-rw-rw-   0 root         (0) root         (0)     3180 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/xlink.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     5695 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/data/xml.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     7619 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/export-roundtrip.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4177 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/export-simple.rst
+-rw-rw-rw-   0 root         (0) root         (0)    55582 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/test_dataimport.py
+-rw-rw-rw-   0 root         (0) root         (0)     6669 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/test_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/test_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     3260 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/test_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)    11834 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/test_rdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    10936 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7240 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/test/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2022-12-21 22:21:09.000000 cubicweb-eac-2.0.0/tox.ini
```

### Comparing `cubicweb-eac-1.5.3/PKG-INFO` & `cubicweb-eac-2.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cubicweb-eac
-Version: 1.5.3
+Version: 2.0.0
 Summary: Implementation of Encoded Archival Context for CubicWeb
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-eac
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Description: Summary
-        -------
-        Implementation of Encoded Archival Context for CubicWeb
-        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: JavaScript
+
+Summary
+-------
+Implementation of Encoded Archival Context for CubicWeb
+
+
```

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/__init__.py` & `cubicweb-eac-2.0.0/cubicweb_eac/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/__pkginfo__.py` & `cubicweb-eac-2.0.0/cubicweb_eac/__pkginfo__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pylint: disable=W0622
 """cubicweb-eac application packaging information"""
 
 distname = "cubicweb-eac"
 modname = "cubicweb_eac"  # required by apycot
 
-numversion = (1, 5, 3)
+numversion = (2, 0, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "Implementation of Encoded Archival Context for CubicWeb"
 web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
 
 __depends__ = {
-    "cubicweb": ">= 3.26.0, < 3.38.0",
+    "cubicweb": ">= 3.38.0, < 3.39.0",
     "cubicweb-prov": ">= 0.4.0",
     "cubicweb-skos": ">= 1.3.0",
     "cubicweb-addressbook": ">=1.6.0",  # first release with python3 support
     "cubicweb-compound": ">= 0.6.0",
     "python-dateutil": None,
 }
 __recommends__ = {}
```

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/ccplugin.py` & `cubicweb-eac-2.0.0/cubicweb_eac/ccplugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from os.path import basename
 from time import time
 
 from cubicweb.toolsutils import Command, underline_title
 from cubicweb.cwctl import CWCTL
 from cubicweb.utils import admincnx
 from cubicweb.dataimport.importer import SimpleImportLog
-from cubicweb.web.views.cwsources import REVERSE_SEVERITIES
+from cubicweb_web.views.cwsources import REVERSE_SEVERITIES
 
 from cubicweb_eac.sobjects import init_extid2eid_index
 
 
 class ImportEacData(Command):
     """Import some EAC files.
 
@@ -120,16 +120,17 @@
 
 
 def _store(cnx):
     if cnx.repo.system_source.dbdriver == "postgres":
         from cubicweb.dataimport.stores import MetadataGenerator
         from cubicweb.dataimport.massive_store import MassiveObjectStore
 
-        MetadataGenerator.META_RELATIONS = MetadataGenerator.META_RELATIONS - set(
-            ["owned_by", "created_by"]
-        )
+        MetadataGenerator.META_RELATIONS = MetadataGenerator.META_RELATIONS - {
+            "owned_by",
+            "created_by",
+        }
         metagen = MetadataGenerator(cnx)
         return MassiveObjectStore(cnx, metagen=metagen, eids_seq_range=1000)
     else:
         from cubicweb.dataimport.stores import NoHookRQLObjectStore
 
         return NoHookRQLObjectStore(cnx)
```

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/dataimport.py` & `cubicweb-eac-2.0.0/cubicweb_eac/dataimport.py`

 * *Files 11% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     """EAC input has an invalid XML format"""
 
 
 class MissingTag(RuntimeError):
     """Mandatory tag is missing in EAC input"""
 
     def __init__(self, tag, tag_parent=None):
-        super(MissingTag, self).__init__()
+        super().__init__()
         self.tag = tag
         self.tag_parent = tag_parent
 
 
 def external_uri(uri):
     values = [str(uri)]
     return ExtEntity("ExternalUri", uri, {"uri": set(values), "cwuri": set(values)})
@@ -122,16 +122,15 @@
     of `elem` being None.
     """
     if inspect.isgeneratorfunction(func):
 
         def wrapped(self, elem, *args, **kwargs):
             if elem is None:
                 return
-            for extentity in func(self, elem, *args, **kwargs):
-                yield extentity
+            yield from func(self, elem, *args, **kwargs)
 
     else:
 
         def wrapped(self, elem, *args, **kwargs):
             if elem is None:
                 return None
             else:
@@ -157,15 +156,15 @@
                     )
                     self.import_log.record_warning(msg, line=objectXMLWrap.sourceline)
             attribute_added = False
             for extentity in func(self, elem):
                 if xmlwrap is not None and extentity.etype in etypes:
                     # prevent association of xmlwrap to several extentities.
                     assert not attribute_added, "xml_wrap attribute already added"
-                    extentity.values.setdefault("xml_wrap", set([])).add(
+                    extentity.values.setdefault("xml_wrap", set()).add(
                         etree.tostring(xmlwrap, encoding="utf-8")
                     )
                     attribute_added = True
                 yield extentity
 
         return wraps(func)(wrapped)
 
@@ -178,16 +177,16 @@
     def decorator(func):
         @wraps(func)
         def wrapper(self, elem):
             for extentity in func(self, elem):
                 if extentity.etype == etype:
                     items = self.parse_items(elem)
                     if items:
-                        extentity.values["items"] = set([items])
-                        extentity.values["items_format"] = set(["text/html"])
+                        extentity.values["items"] = {items}
+                        extentity.values["items_format"] = {"text/html"}
                 yield extentity
 
         return wrapper
 
     return decorator
 
 
@@ -268,16 +267,15 @@
         # pylint: disable=protected-access
         if inspect.isgeneratorfunction(func):
 
             def wrapped(self, elem, *args, **kwargs):
                 if self._elem_find(elem, tagname) is None:
                     warn(self, elem)
                     return
-                for extentity in func(self, elem, *args, **kwargs):
-                    yield extentity
+                yield from func(self, elem, *args, **kwargs)
 
         else:
 
             def wrapped(self, elem, *args, **kwargs):
                 if self._elem_find(elem, tagname) is None:
                     warn(self, elem)
                     return None
@@ -329,15 +327,15 @@
                 if extid:
                     yield external_uri(extid)
             else:
                 extid = None
 
             def update_extentity(extentity):
                 if extid is not None and extentity.etype == etype:
-                    extentity.values["equivalent_concept"] = set([extid])
+                    extentity.values["equivalent_concept"] = {extid}
 
             if inspect.isgeneratorfunction(func):
                 for extentity in func(self, elem, *args, **kwargs):
                     update_extentity(extentity)
                     yield extentity
             else:
                 extentity = func(self, elem, *args, **kwargs)
@@ -345,15 +343,15 @@
                 yield extentity
 
         return wrapped
 
     return decorator
 
 
-class EACCPFImporter(object):
+class EACCPFImporter:
     """Importer for EAC-CPF data.
 
     The importer will generate `extid`s using the `extid_generator` function
     if specified or use `uuid.uuid4` to generate unique `extid`s.
 
     During import the `record` attribute is set to the external entity of the
     imported AuthorityRecord.
@@ -381,33 +379,33 @@
 
         self._gen_extid = extid_generator
         self.record = ExtEntity("AuthorityRecord", None, {})
         # Store a mapping of XML elements to produced ExtEntities
         self._visited = {}
 
     def __getattribute__(self, name):
-        attr = super(EACCPFImporter, self).__getattribute__(name)
+        attr = super().__getattribute__(name)
         if name.startswith("build_"):
             return trace_extentity(self)(attr)
         return attr
 
     def values_from_attrib(self, elem, name_attrib_tuples):
         values = {}
         for var_name, attrib_name in name_attrib_tuples:
             attrib_value = elem.attrib.get(attrib_name)
             if attrib_value:
-                values[var_name] = set([str(attrib_value)])
+                values[var_name] = {str(attrib_value)}
         return values
 
     def values_from_xpaths(self, elem, name_path_tuples):
         values = {}
         for var_name, var_path in name_path_tuples:
             var = self._elem_find(elem, var_path)
             if var is not None and var.text:
-                values[var_name] = set([str(var.text)])
+                values[var_name] = {str(var.text)}
         return values
 
     def parse_items(self, elem):
         values = []
         new_elem = copy.deepcopy(elem)
         for list_elem in self._elem_findall(new_elem, "eac:list"):
             list_elem.tag = "ul"
@@ -418,15 +416,15 @@
         filtered = [
             e for e in re.split(r"xmlns\S*\"", result) if not e.startswith("xmlns")
         ]
         return "".join(filtered)
 
     def record_visited(self, elem, extentity):
         assert extentity.extid, extentity
-        self._visited.setdefault(elem, set([])).add(extentity.extid)
+        self._visited.setdefault(elem, set()).add(extentity.extid)
 
     def not_visited(self):
         """Yield (tagname, sourceline) items corresponding to XML elements not
         used to build any ExtEntity.
         """
         visited = self._visited
         ns = self.namespaces["eac"]
@@ -441,15 +439,15 @@
             "description",
             "mandates",
             "places",
             "legalStatuses",
             "occupations",
             "relations",
         ]
-        containers = ["{{{0}}}{1}".format(ns, tag) for tag in container_tags]
+        containers = [f"{{{ns}}}{tag}" for tag in container_tags]
         while queue:
             elem = queue.popleft()
             if not isinstance(elem, etree._Element) or isinstance(elem, etree._Comment):
                 continue
             if elem in visited:
                 continue
             if elem.tag not in containers:
@@ -482,65 +480,59 @@
     @filter_empty
     def external_entities(self):
         """Parse a EAC XML file to and yield external entities."""
         # control element.
         control = self._elem_find(self._root, "eac:control")
         if control is None:
             raise MissingTag("control")
-        for extentity in self.parse_control(control):
-            yield extentity
+        yield from self.parse_control(control)
         # Records (identity tags) are within cpfDescription tag.
         cpf_desc = self._elem_find(self._root, "eac:cpfDescription")
         if cpf_desc is None:
             raise MissingTag("cpfDescription")
         # identity element.
         identity = self._elem_find(cpf_desc, "eac:identity")
         if identity is None:
             raise MissingTag("identity", "cpfDescription")
-        for extentity in self.parse_identity(identity):
-            yield extentity
+        yield from self.parse_identity(identity)
         # description element.
         description = self._elem_find(cpf_desc, "eac:description")
         if description is not None:
-            for extentity in self.parse_description(description):
-                yield extentity
+            yield from self.parse_description(description)
         # relations element.
-        for extentity in self.parse_relations(cpf_desc):
-            yield extentity
+        yield from self.parse_relations(cpf_desc)
         # Record is complete.
         self.record_visited(self._root, self.record)
         yield self.record
 
     def parse_identity(self, identity):
         """Parse the `identity` tag and yield external entities, possibly
         updating record's `values` dict.
         """
         # entityId
         isni = self._elem_find(identity, "eac:entityId")
         if isni is not None and isni.text:
             self.record_visited(isni, self.record)
-            self.record.values["isni"] = set([str(isni.text)])
+            self.record.values["isni"] = {str(isni.text)}
         # entityType
         akind = self._elem_find(identity, "eac:entityType")
         if akind is None:
             raise MissingTag("entityType", "identity")
         agent_kind = self.build_agent_kind(akind)
         yield agent_kind
-        self.record.values["agent_kind"] = set([agent_kind.extid])
+        self.record.values["agent_kind"] = {agent_kind.extid}
         name_entry = None
         name_entries = self._elem_findall(identity, "eac:nameEntry")
         if not name_entries:
             raise MissingTag("nameEntry", "identity")
         for name_entry in name_entries:
-            for extentity in self.build_name_entry(name_entry):
-                yield extentity
+            yield from self.build_name_entry(name_entry)
         parallel_name_entries = self._elem_findall(identity, "eac:nameEntryParallel")
         for parallel_name_entry in parallel_name_entries:
-            for extentity in self.build_parallel(parallel_name_entry):
-                yield extentity
+            yield from self.build_parallel(parallel_name_entry)
 
     @relate_to_record_through("ParallelNames", "parallel_names_of")
     @add_names_for("ParallelNames")
     @add_dates_for("ParallelNames")
     def build_parallel(self, elem):
         """For each nameEntryParallel build a new object linked to the
         EAC-CPF document and get relations for all childrens"""
@@ -556,36 +548,33 @@
     @filter_empty
     def extract_dates_from(self, elem, tag):
         for date in self.find_nested(elem, "eac:date", tag):
             yield ExtEntity(
                 "DateEntity",
                 self._gen_extid(),
                 {
-                    "start_date": set([self.parse_date(date)]),
-                    "end_date": set([self.parse_date(date)]),
+                    "start_date": {self.parse_date(date)},
+                    "end_date": {self.parse_date(date)},
                 },
             )
         for date_range in self.find_nested(elem, "eac:dateRange", tag):
             yield ExtEntity(
                 "DateEntity", self._gen_extid(), self.parse_daterange(date_range)
             )
 
     @filter_empty
     @elem_maybe_none
     def build_date_entry(self, elem):
         """Build DateEntitys linked to a parent entity"""
         for usedates in self._elem_findall(elem, "eac:useDates"):
-            for extentity in self.build_date_entry(usedates):
-                yield extentity
+            yield from self.build_date_entry(usedates)
         if self._elem_find(elem, "eac:dateSet"):
             for date_set in self._elem_findall(elem, "eac:dateSet"):
-                for extentity in self.extract_dates_from(date_set, "eac:dateSet"):
-                    yield extentity
-        for entity in self.extract_dates_from(elem, "eac:test"):
-            yield entity
+                yield from self.extract_dates_from(date_set, "eac:dateSet")
+        yield from self.extract_dates_from(elem, "eac:test")
 
     @filter_empty
     @filter_none
     @elem_maybe_none
     def build_name_child(self, elem):
         """Build NameEntry external entity"""
         for elem in self._elem_findall(elem, "eac:nameEntry"):
@@ -612,15 +601,15 @@
         """Add a `languages` on AuthorityRecord"""
         languages = []
         for elem in elems:
             language = self._elem_find(elem, "eac:language")
             if language is not None and language.text.strip():
                 languages.append(language.text.strip())
         if languages:
-            self.record.values["languages"] = set([", ".join(languages)])
+            self.record.values["languages"] = {", ".join(languages)}
 
     @filter_none
     def parse_description(self, description):
         """Parse the `description` tag and yield external entities, possibly
         updating record's `values` dict.
         """
         # dates.
@@ -632,54 +621,46 @@
             self.record_visited(elem, self.record)
             self.record_visited(elem.getparent(), self.record)
             dates = self.parse_daterange(elem)
             if dates:
                 self.record.values.update(dates)
         # address.
         for place in self.find_nested(description, "eac:place", "eac:places"):
-            for extentity in self.build_place(place):
-                yield extentity
+            yield from self.build_place(place)
         # additional EAC-CPF information.
         for legal_status in self.find_nested(
             description, "eac:legalStatus", "eac:legalStatuses"
         ):
-            for extentity in self.build_legal_status(legal_status):
-                yield extentity
+            yield from self.build_legal_status(legal_status)
         # mandate
         for mandate in self.find_nested(description, "eac:mandate", "eac:mandates"):
-            for extentity in self.build_mandate(mandate):
-                yield extentity
+            yield from self.build_mandate(mandate)
         # languagesUsed
         languages = self.find_nested(
             description, "eac:languageUsed", "eac:languagesUsed"
         )
         if languages:
             self.parse_languages(languages)
         # history
         for history in self._elem_findall(description, "eac:biogHist"):
-            for extentity in self.build_history(history):
-                yield extentity
+            yield from self.build_history(history)
         # structure
         for structure in self._elem_findall(description, "eac:structureOrGenealogy"):
-            for extentity in self.build_structure(structure):
-                yield extentity
+            yield from self.build_structure(structure)
         # function
         for function in self.find_nested(description, "eac:function", "eac:functions"):
-            for extentity in self.build_function(function):
-                yield extentity
+            yield from self.build_function(function)
         # occupation
         for occupation in self.find_nested(
             description, "eac:occupation", "eac:occupations"
         ):
-            for extentity in self.build_occupation(occupation):
-                yield extentity
+            yield from self.build_occupation(occupation)
         # general context
         for context in self._elem_findall(description, "eac:generalContext"):
-            for extentity in self.build_generalcontext(context):
-                yield extentity
+            yield from self.build_generalcontext(context)
 
     def find_nested(self, elem, tagname, innertag):
         """Return a list of element with `tagname` within `element` possibly
         nested within `innertag`.
         """
         all_elems = self._elem_findall(elem, tagname)
         wrapper = self._elem_find(elem, innertag)
@@ -702,17 +683,15 @@
                 % (tagname, elem.tag),
                 line=elem.sourceline,
             )
         elem = elems[0] if elems else None
         values = {}
         if elem is not None:
             parsed = self.parse_tag_content(elem)
-            values.update(
-                zip((attrname, attrname + "_format"), (set([p]) for p in parsed))
-            )
+            values.update(zip((attrname, attrname + "_format"), ({p} for p in parsed)))
         return values
 
     def parse_tag_content(self, elem):
         """Parse the content of an element be it plain text or HTML and return
         the content along with MIME type.
         """
         assert elem is not None, "unexpected empty element"
@@ -744,34 +723,34 @@
     def build_name_entry(self, element):
         """Build a NameEntry external entity."""
         self.record_visited(element, self.record)
         parts = self._elem_findall(element, "eac:part")
         if not parts:
             raise MissingTag("part", "nameEntry")
         # Join all "part" tags into a single "parts" attribute.
-        values = {"parts": set([", ".join(str(p.text) for p in parts)])}
+        values = {"parts": {", ".join(str(p.text) for p in parts)}}
         # Consider first authorizedForm and then alternativeForm, missing
         # possible combinations which cannot be handled until the model is
         # complete.
         if self._elem_find(element, "eac:authorizedForm") is not None:
-            values["form_variant"] = set(["authorized"])
+            values["form_variant"] = {"authorized"}
         elif self._elem_find(element, "eac:alternativeForm") is not None:
-            values["form_variant"] = set(["alternative"])
+            values["form_variant"] = {"alternative"}
         yield ExtEntity("NameEntry", self._gen_extid(), values)
 
     @elem_maybe_none
     def build_agent_kind(self, elem):
         """Build a AgentKind external entity"""
         # Map EAC entity types to our terminolgy.
         kind = TYPE_MAPPING.get(elem.text, "unknown-agent-kind")
         if kind == "unknown-agent-kind":
             msg = self._("unexpected entity type {}").format(elem.text)
             self.import_log.record_warning(msg, line=elem.sourceline)
         agentkind_id = "agentkind/" + kind
-        return ExtEntity("AgentKind", agentkind_id, {"name": set([str(kind)])})
+        return ExtEntity("AgentKind", agentkind_id, {"name": {str(kind)}})
 
     @elem_maybe_none
     @relate_to_record_through("LegalStatus", "legal_status_agent")
     @filter_empty
     @add_citations_for("LegalStatus")
     @add_place_entries_for("LegalStatus")
     @add_items_for("LegalStatus")
@@ -781,15 +760,15 @@
         """Build a `LegalStatus` external entity.
 
         Extra `kwargs` are passed to `parse_tag_description`.
         """
         values = self.parse_tag_description(elem, **kwargs)
         term = self._elem_find(elem, "eac:term")
         if term is not None and term.text:
-            values["term"] = set([str(term.text)])
+            values["term"] = {str(term.text)}
         yield ExtEntity("LegalStatus", self._gen_extid(), values)
 
     @elem_maybe_none
     @relate_to_record_through("Mandate", "mandate_agent")
     @filter_empty
     @add_citations_for("Mandate")
     @add_place_entries_for("Mandate")
@@ -800,15 +779,15 @@
         """Build a `Mandate` external entity.
 
         Extra `kwargs` are passed to `parse_tag_description`.
         """
         values = self.parse_tag_description(elem, **kwargs)
         term = self._elem_find(elem, "eac:term")
         if term is not None and term.text:
-            values["term"] = set([str(term.text)])
+            values["term"] = {str(term.text)}
         yield ExtEntity("Mandate", self._gen_extid(), values)
 
     @elem_maybe_none
     def build_citation(self, elem):
         """Build a `Citation` external entity."""
         for citation_elem in self._elem_findall(elem, "eac:citation"):
             note = citation_elem.text.strip() if citation_elem.text else ""
@@ -817,101 +796,100 @@
                 msg = self._("element {0} has no text nor (valid) link").format(
                     etree.tostring(citation_elem)
                 )
                 self.import_log.record_warning(msg, line=citation_elem.sourceline)
                 return
             values = {}
             if uri:
-                values["uri"] = set([str(uri)])
+                values["uri"] = {str(uri)}
             if note:
-                values["note"] = set([str(note)])
+                values["note"] = {str(note)}
                 if "<span>" in note:
-                    values["note_format"] = set(["text/html"])
+                    values["note_format"] = {"text/html"}
             yield ExtEntity("Citation", self._gen_extid(), values)
 
     @relate_to_record_through("History", "history_agent")
     @add_citations_for("History")
     @add_items_for("History")
     @elem_maybe_none
     def build_history(self, elem):
         """Build a `History` external entity."""
         abstract = self._elem_find(elem, "eac:abstract")
         desc, desc_format = self.parse_tag_content(elem)
         if desc:
-            values = {"text": set([desc]), "text_format": set([desc_format])}
+            values = {"text": {desc}, "text_format": {desc_format}}
             if abstract is not None and abstract.text:
-                values["abstract"] = set([str(abstract.text)])
+                values["abstract"] = {str(abstract.text)}
             history = ExtEntity("History", self._gen_extid(), values)
             for child in self.parse_history_chronitems(elem):
                 if child.etype == "HistoricalEvent":
                     history.values.setdefault("has_event", set()).add(child.extid)
                 yield child
             yield history
 
     def parse_history_chronitems(self, elem):
         """Build en `Event` external entity."""
         for citem in self._elem_findall(elem, ".//eac:chronItem"):
-            for extentity in self.build_event(citem):
-                yield extentity
+            yield from self.build_event(citem)
 
     @add_dates_for("HistoricalEvent")
     @add_place_entries_for("HistoricalEvent")
     @filter_none
     @filter_empty
     @elem_maybe_none
     def build_event(self, elem):
         """Build a `HistoricalEvent` external entity."""
         values = {}
         event = self._elem_find(elem, "eac:event")
         if event is not None and event.text:
-            values["event"] = set([str(event.text)])
+            values["event"] = {str(event.text)}
         yield ExtEntity("HistoricalEvent", self._gen_extid(), values)
 
     @elem_maybe_none
     @relate_to_record_through("Structure", "structure_agent")
     @add_citations_for("Structure")
     @add_items_for("Structure")
     def build_structure(self, elem):
         """Build a `Structure` external entity."""
         desc, desc_format = self.parse_tag_content(elem)
         if desc:
             values = {
-                "description": set([desc]),
-                "description_format": set([desc_format]),
+                "description": {desc},
+                "description_format": {desc_format},
             }
             yield ExtEntity("Structure", self._gen_extid(), values)
 
     @relate_to_record_through("AgentPlace", "place_agent")
     @filter_empty
     @add_citations_for("AgentPlace")
     @add_dates_for("AgentPlace")
     @add_items_for("AgentPlace")
     def build_place(self, elem):
         """Build a AgentPlace external entity"""
         values = {}
         role = self._elem_find(elem, "eac:placeRole")
         if role is not None:
-            values["role"] = set([str(role.text)])
+            values["role"] = {str(role.text)}
         for address in self._elem_findall(elem, "eac:address"):
             for extentity in self.build_address(address):
                 if extentity.values:
-                    values["place_address"] = set([extentity.extid])
+                    values["place_address"] = {extentity.extid}
                     yield extentity
         place = ExtEntity("AgentPlace", self._gen_extid(), values)
         for child in self.build_place_entry(elem):
             if child.etype == "PlaceEntry":
                 place.values.setdefault("place_entry_relation", set()).add(child.extid)
             yield child
         yield place
 
     @filter_empty
     @equivalent_concept("eac:placeEntry", "PlaceEntry")
     def build_place_entry(self, elem):
         for entry in self._elem_findall(elem, "eac:placeEntry"):
-            values = {"name": set([str(entry.text)])}
+            values = {"name": {str(entry.text)}}
             values.update(
                 self.values_from_attrib(
                     entry,
                     (
                         ("local_type", "localType"),
                         ("longitude", "longitude"),
                         ("latitude", "latitude"),
@@ -927,72 +905,72 @@
         for line in self._elem_findall(elem, "eac:addressLine"):
             address_lines.append(str(line.text))
             if "localType" in line.attrib:
                 attr = dict(ADDRESS_MAPPING).get(line.attrib["localType"])
                 if attr:
                     address_entity.setdefault(attr, set()).add(str(line.text))
         if address_lines:
-            address_entity["raw_address"] = set(["\n".join(address_lines)])
+            address_entity["raw_address"] = {"\n".join(address_lines)}
         yield ExtEntity("PostalAddress", self._gen_extid(), address_entity)
 
     @relate_to_record_through("AgentFunction", "function_agent")
     @filter_empty
     @add_citations_for("AgentFunction")
     @add_place_entries_for("AgentFunction")
     @add_dates_for("AgentFunction")
     @add_items_for("AgentFunction")
     @equivalent_concept("eac:term", "AgentFunction")
     def build_function(self, elem):
         """Build a `AgentFunction`s external entities"""
         values = self.parse_tag_description(elem)
         term = self._elem_find(elem, "eac:term")
         if term is not None:
-            values["name"] = set([str(term.text)])
+            values["name"] = {str(term.text)}
         yield ExtEntity("AgentFunction", self._gen_extid(), values)
 
     @relate_to_record_through("Occupation", "occupation_agent")
     @filter_empty
     @add_citations_for("Occupation")
     @add_place_entries_for("Occupation")
     @add_items_for("Occupation")
     @add_dates_for("Occupation")
     @equivalent_concept("eac:term", "Occupation")
     def build_occupation(self, elem):
         """Build a `Occupation`s external entities"""
         values = self.parse_tag_description(elem)
         term = self._elem_find(elem, "eac:term")
         if term is not None:
-            values["term"] = set([str(term.text)])
+            values["term"] = {str(term.text)}
         yield ExtEntity("Occupation", self._gen_extid(), values)
 
     @relate_to_record_through("GeneralContext", "general_context_of")
     @add_citations_for("GeneralContext")
     @add_items_for("GeneralContext")
     def build_generalcontext(self, elem):
         """Build a `GeneralContext` external entity"""
         content, content_format = self.parse_tag_content(elem)
         if content:
             values = {
-                "content": set([content]),
-                "content_format": set([content_format]),
+                "content": {content},
+                "content_format": {content_format},
             }
             yield ExtEntity("GeneralContext", self._gen_extid(), values)
 
     @elem_maybe_none
     def parse_daterange(self, elem):
         """Parse a `dateRange` tag and return a dict mapping `start_date` and
         `end_date` to parsed date range.
         """
         values = {}
         for eactag, attrname in zip(
             ("eac:fromDate", "eac:toDate"), ("start_date", "end_date")
         ):
             date = self.parse_date(self._elem_find(elem, eactag))
             if date:
-                values[attrname] = set([date])
+                values[attrname] = {date}
         return values
 
     @elem_maybe_none
     def parse_date(self, elem):
         """Parse a date-like element"""
 
         def record_warning(msg):
@@ -1051,16 +1029,15 @@
         builders = (
             ("eac:cpfRelation", self.build_relation),
             ("eac:resourceRelation", self.build_resource_relation),
             ("eac:functionRelation", self.build_function_relation),
         )
         for xpath, builder in builders:
             for elem in self._elem_findall(relations, xpath):
-                for extentity in builder(elem):
-                    yield extentity
+                yield from builder(elem)
 
     @add_xml_wrap_for(
         "AssociationRelation",
         "ChronologicalRelation",
         "HierarchicalRelation",
         "IdentityRelation",
         "FamilyRelation",
@@ -1147,18 +1124,18 @@
                     "found a cpfRelation without any object (no "
                     "xlink:href attribute), skipping"
                 ),
                 line=elem.sourceline,
             )
             return
         yield external_uri(obj_uri)
-        values = {agent_role: set([self.record.extid]), other_role: set([obj_uri])}
+        values = {agent_role: {self.record.extid}, other_role: {obj_uri}}
         rentry = self._elem_find(elem, "eac:relationEntry")
         if rentry is not None and rentry.text.strip():
-            values["entry"] = set([str(rentry.text)])
+            values["entry"] = {str(rentry.text)}
         values.update(self.parse_tag_description(elem))
         yield ExtEntity(etype, self._gen_extid(), values)
 
     @add_place_entries_for("EACFunctionRelation")
     @add_dates_for("EACFunctionRelation")
     @add_xml_wrap_for("EACFunctionRelation")
     def build_function_relation(self, elem):
@@ -1169,20 +1146,20 @@
         the AuthorityRecord object"""
         values = self.parse_tag_description(elem)
         relationship = elem.attrib.pop("functionRelationType", None)
         obj_uri = elem.attrib.pop("{%(xlink)s}href" % self.namespaces, None)
         # Yield the ExternalUri object
         if obj_uri:
             yield external_uri(obj_uri)
-            values.update({"function_relation_function": set([str(obj_uri)])})
+            values.update({"function_relation_function": {str(obj_uri)}})
         if relationship:
-            values.update({"r_type": set([str(relationship)])})
+            values.update({"r_type": {str(relationship)}})
         values.update(
             {
-                "function_relation_agent": set([str(self.record.extid)]),
+                "function_relation_agent": {str(self.record.extid)},
             }
         )
         values.update(
             self.values_from_xpaths(
                 elem,
                 (
                     ("place_entry", "eac:placeEntry"),
@@ -1190,15 +1167,15 @@
                 ),
             )
         )
         if elem.attrib:
             attributes = json.dumps(dict(elem.attrib), sort_keys=True)
         else:
             attributes = json.dumps({})
-        values.update({"xml_attributes": set([str(attributes)])})
+        values.update({"xml_attributes": {str(attributes)}})
         yield ExtEntity("EACFunctionRelation", self._gen_extid(), values)
 
     @add_place_entries_for("EACResourceRelation")
     @add_dates_for("EACResourceRelation")
     @add_xml_wrap_for("EACResourceRelation")
     def build_resource_relation(self, elem):
         """Build a `EACResourceRelation` external entity (along with
@@ -1212,56 +1189,54 @@
                     "attribute), skipping"
                 ),
                 line=elem.sourceline,
             )
             return
         yield external_uri(obj_uri)
         values = {
-            "resource_relation_resource": set([obj_uri]),
-            "resource_relation_agent": set([self.record.extid]),
+            "resource_relation_resource": {obj_uri},
+            "resource_relation_agent": {self.record.extid},
         }
         relation_entry = self._elem_find(elem, "eac:relationEntry")
         if relation_entry is not None:
-            values["relation_entry"] = set([str(relation_entry.text)])
+            values["relation_entry"] = {str(relation_entry.text)}
         resource_role = elem.attrib.pop("{%(xlink)s}role" % self.namespaces, None)
         if resource_role:
-            values["resource_role"] = set([str(resource_role)])
+            values["resource_role"] = {str(resource_role)}
         agent_role = elem.attrib.pop("resourceRelationType", None)
         if agent_role:
-            values["agent_role"] = set([str(agent_role)])
+            values["agent_role"] = {str(agent_role)}
         if elem.attrib:
             attributes = json.dumps(dict(elem.attrib), sort_keys=True)
         else:
             attributes = json.dumps({})
-        values.update({"xml_attributes": set([str(attributes)])})
+        values.update({"xml_attributes": {str(attributes)}})
         values.update(self.parse_tag_description(elem))
         yield ExtEntity("EACResourceRelation", self._gen_extid(), values)
 
     @filter_none
     def parse_control(self, control):
         """Parse the `control` tag."""
         record_id = self._elem_find(control, "eac:recordId")
         if record_id is not None and record_id.text and record_id.text.strip():
             record_id = record_id.text.strip()
-            self.record.extid = "authorityrecord-{}".format(record_id)
-            self.record.values["record_id"] = set([to_unicode(record_id)])
+            self.record.extid = f"authorityrecord-{record_id}"
+            self.record.values["record_id"] = {to_unicode(record_id)}
             self.record_visited(record_id, self.record)
         else:
             raise InvalidEAC("recordId element in control tag is mandatory")
         for other_record_id in self._elem_findall(control, "eac:otherRecordId"):
             other_id = other_record_id.text.strip()
             if other_id:
                 values = {
-                    "eac_other_record_id_of": set([self.record.extid]),
-                    "value": set([str(other_id)]),
+                    "eac_other_record_id_of": {self.record.extid},
+                    "value": {str(other_id)},
                 }
                 if other_record_id.attrib.get("localType"):
-                    values["local_type"] = set(
-                        [str(other_record_id.attrib["localType"])]
-                    )
+                    values["local_type"] = {str(other_record_id.attrib["localType"])}
                 extentity = ExtEntity("EACOtherRecordId", self._gen_extid(), values)
                 self.record_visited(other_record_id, extentity)
                 yield extentity
         builders = (
             ("eac:sources/eac:source", self.build_source),
             (
                 "eac:maintenanceHistory/eac:maintenanceEvent",
@@ -1274,51 +1249,51 @@
                 for extentity in builder(elem):
                     yield extentity
 
     def build_maintenance_event(self, elem):
         """Parse a `maintenanceEvent` tag, yielding a prov:Activity external
         entity along with necessary Records.
         """
-        values = {"generated": set([self.record.extid])}
+        values = {"generated": {self.record.extid}}
         event_type = self.parse_event_type(self._elem_find(elem, "eac:eventType"))
         if event_type is not None:
-            values["type"] = set([event_type])
+            values["type"] = {event_type}
         date = self._elem_find(elem, "eac:eventDateTime")
         if date is not None:
             dtattr = date.attrib.get("standardDateTime")
             if dtattr:
                 try:
                     event_date = parse_date(dtattr)
                 except ValueError:
                     self.import_log.record_warning(
                         self._("could not parse date from %s") % etree.tostring(date),
                         line=date.sourceline,
                     )
                 else:
-                    values["start"] = set([event_date])
-                    values["end"] = set([event_date])
+                    values["start"] = {event_date}
+                    values["end"] = {event_date}
         values.update(self.parse_tag_description(elem, "eac:eventDescription"))
         values.update(self.values_from_xpaths(elem, (("agent", "eac:agent"),)))
         agent_type = self._elem_find(elem, "eac:agentType")
         values["agent_type"] = "unknown"
         if agent_type.text in {"human", "machine"}:
-            values["agent_type"] = set([str(agent_type.text)])
+            values["agent_type"] = {str(agent_type.text)}
         yield ExtEntity("Activity", self._gen_extid(), values)
 
     @relate_to_record_through("Convention", "convention_of")
     @add_citations_for("Convention")
     @filter_none
     @filter_empty
     @elem_maybe_none
     def build_convention(self, elem):
         """Build a `Convention` external entity"""
         values = self.parse_tag_description(elem)
         abbrev = self._elem_find(elem, "eac:abbreviation")
         if abbrev is not None and abbrev.text:
-            values["abbrev"] = set([str(abbrev.text)])
+            values["abbrev"] = {str(abbrev.text)}
         yield ExtEntity("Convention", self._gen_extid(), values)
 
     @elem_maybe_none
     def parse_event_type(self, elem):
         """Parse an `eventType` element and try to match a prov:type to build a
         prov:Activity.
         """
@@ -1345,12 +1320,12 @@
     @filter_empty
     @add_xml_wrap_for("EACSource")
     def build_source(self, elem):
         """Parse a `source` tag, yielding EACSource external entities."""
         values = self.parse_tag_description(elem)
         url = elem.attrib.get("{%(xlink)s}href" % self.namespaces)
         if url is not None:
-            values["url"] = set([str(url)])
+            values["url"] = {str(url)}
         entry = self._elem_find(elem, "eac:sourceEntry")
         if entry is not None and entry.text:
-            values["title"] = set([str(entry.text)])
+            values["title"] = {str(entry.text)}
         yield ExtEntity("EACSource", self._gen_extid(), values)
```

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/entities/__init__.py` & `cubicweb-eac-2.0.0/cubicweb_eac/entities/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding: utf-8
 # copyright 2016-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -19,23 +18,24 @@
 import json
 
 from functools import wraps
 
 from lxml import etree
 
 from logilab.common.date import ustrftime
+from logilab.common.decorators import cachedproperty
 
 from cubicweb.predicates import is_instance
 from cubicweb.entities import AnyEntity, fetch_config
 from cubicweb.entity import EntityAdapter
 
 from cubicweb_eac import TYPE_MAPPING, ADDRESS_MAPPING, MAINTENANCETYPE_MAPPING
 
 
-class DateRelationMixin(object):
+class DateRelationMixin:
     @property
     def start_date(self):
         if self.date_relation:
             return self.date_relation[0].start_date
 
     @property
     def end_date(self):
@@ -71,25 +71,25 @@
     @property
     def other_record_ids(self):
         return sorted(
             [(r.local_type, r.value) for r in self.reverse_eac_other_record_id_of],
             key=lambda x: (x[0] or "", x[1] or ""),
         )
 
-    @property
+    @cachedproperty
     def activities(self):
         return self._cw.execute(
             "Any A, TYPE, START, END, AGENTTYPE, AGENT, DESCR WHERE"
             "A is Activity, A generated X, X is AuthorityRecord, X eid %(eid)s,"
             "A type TYPE, A start START, A end END, A agent_type AGENTTYPE,"
             "A agent AGENT, A description DESCR",
             {"eid": self.eid},
         ).entities()
 
-    @property
+    @cachedproperty
     def sources(self):
         return self._cw.execute(
             "Any S, TITLE, URL WHERE"
             "S is EACSource, S source_agent X, X is AuthorityRecord, X eid %(eid)s,"
             "S title TITLE, S url URL",
             {"eid": self.eid},
         ).entities()
@@ -169,15 +169,15 @@
 
 
 class GeneralContext(AnyEntity):
     __regid__ = "GeneralContext"
     fetch_attrs, cw_fetch_order = fetch_config(("content",))
 
 
-class JsonAttrsMixin(object):
+class JsonAttrsMixin:
     @property
     def json_attrs(self):
         return json.loads(self.xml_attributes)
 
 
 class EACResourceRelation(DateRelationMixin, AnyEntity, JsonAttrsMixin):
     __regid__ = "EACResourceRelation"
@@ -229,15 +229,15 @@
 
 
 class DateEntity(AnyEntity):
     __regid__ = "DateEntity"
     fetch_attrs, cw_fetch_order = fetch_config(("start_date", "end_date"))
 
 
-class SameAsMixIn(object):
+class SameAsMixIn:
     """Mix-in class for entity types supporting vocabulary_source and
     equivalent_concept relations.
     """
 
     @property
     def scheme(self):
         return self.vocabulary_source and self.vocabulary_source[0] or None
@@ -342,16 +342,16 @@
         '{http://www.w3.org/1999/xlink}href'
 
     """
     try:
         prefix, name = prefix_name.split(":", 1)
     except ValueError:
         return prefix_name
-    assert prefix in namespaces, "Unknown namespace prefix: {0}".format(prefix)
-    return "{{{0}}}".format(namespaces[prefix]) + name
+    assert prefix in namespaces, f"Unknown namespace prefix: {prefix}"
+    return f"{{{namespaces[prefix]}}}" + name
 
 
 class AbstractXmlAdapter(EntityAdapter):
     """Abstract adapter to produce XML documents."""
 
     content_type = "text/xml"
     encoding = "utf-8"
@@ -455,15 +455,15 @@
     @property
     def file_name(self):
         """Return a file name for the dump."""
         if self.entity.isni:
             name = self.entity.isni.replace("/", "_")
         else:
             name = str(self.entity.eid)
-        return "EAC_{0}.xml".format(name)
+        return f"EAC_{name}.xml"
 
     def dump(self):
         """Return an XML string representing the given agent using the EAC-CPF schema."""
         # Keep related activities since they are used multiple times
         self.activities = sorted(
             self.entity.reverse_generated, key=lambda x: x.start, reverse=True
         )
@@ -557,15 +557,15 @@
             sources_elt.append(self.source_element(eac_source))
         if len(sources_elt):
             control_elt.append(sources_elt)
 
     def identity_element(self, cpfdescription_elt):
         identity_elt = self.element("identity", parent=cpfdescription_elt)
         self._elt_text_from_attr("entityId", self.entity, "isni", parent=identity_elt)
-        type_mapping = dict((v, k) for k, v in TYPE_MAPPING.items())
+        type_mapping = {v: k for k, v in TYPE_MAPPING.items()}
         eac_type = type_mapping.get(self.entity.kind)
         self.element("entityType", parent=identity_elt, text=eac_type)
         for name_entry in self.entity.reverse_name_entry_for:
             elem = self.element("nameEntry", parent=identity_elt)
             for part in name_entry.parts.split(", "):
                 self.element("part", parent=elem, text=part)
             if name_entry.form_variant == "authorized":
@@ -635,15 +635,15 @@
         for resource_relation in self.entity.reverse_resource_relation_agent:
             relations_elt.append(self.resource_relation_element(resource_relation))
         if len(relations_elt):
             cpfdescription_elt.append(relations_elt)
 
     def maintenance_event_element(self, activity, history_elt):
         event_elt = self.element("maintenanceEvent", parent=history_elt)
-        type_mapping = dict((v, k) for k, v in MAINTENANCETYPE_MAPPING.items())
+        type_mapping = {v: k for k, v in MAINTENANCETYPE_MAPPING.items()}
         activity_type = type_mapping.get(activity.type, "created")
         self.element("eventType", parent=event_elt, text=activity_type)
         self.element(
             "eventDateTime",
             parent=event_elt,
             attributes={
                 "standardDateTime": ustrftime(activity.start, fmt=self.datetime_fmt)
@@ -874,8 +874,8 @@
             if not value:
                 return []
             return [self.element("p", text=line) for line in value.splitlines()]
         else:
             value = entity.printable_value(attr_name)
             if not value:
                 return []
-            return list(etree.fromstring("<root>{0}</root>".format(value)))
+            return list(etree.fromstring(f"<root>{value}</root>"))
```

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/entities/rdf.py` & `cubicweb-eac-2.0.0/cubicweb_eac/entities/rdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding: utf-8
 # copyright 2021-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -14,14 +13,16 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from rdflib import BNode, Literal, URIRef
 from rdflib.term import _is_valid_uri
 
+from logilab.common.decorators import cachedproperty
+
 from cubicweb.predicates import is_instance
 from cubicweb.entities.adapters import EntityRDFAdapter
 from cubicweb.uilib import remove_html_tags
 
 
 class AuthorityRecordRDFAdapter(EntityRDFAdapter):
     __regid__ = "rdf.schemaorg"
@@ -131,19 +132,19 @@
     )
 
 
 class AuthorityRecordRICORDFAdapter(EntityRDFAdapter):
     __regid__ = "rdf.rico"
     __select__ = EntityRDFAdapter.__select__ & is_instance("AuthorityRecord")
 
-    @property
+    @cachedproperty
     def agent_uri(self):
         return URIRef(f"{self.uri}#agent")
 
-    @property
+    @cachedproperty
     def inst_uri(self):
         return URIRef(f"{self.uri}#inst")
 
     def relation_triples(
         self,
         class_uri,
         relation_uri,
@@ -576,15 +577,14 @@
                     None,
                     start,
                     end,
                 )
                 yield (occupation_uri, RDF.type, RICO.Activity)
                 yield (occupation_uri, RICO.hasActivityType, occupation_type_uri)
                 yield (occupation_type_uri, RDF.type, RICO.OccupationType)
-                yield (occupation_type_uri, RDF.type, RICO.ActivityType)
                 yield (occupation_type_uri, RDFS.label, Literal(occ_name))
 
                 yield (
                     self.agent_uri,
                     RICO.hasOrHadOccupationOfType,
                     occupation_type_uri,
                 )
```

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/hooks.py` & `cubicweb-eac-2.0.0/cubicweb_eac/hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                     self.info(
                         'deleting "%s" as %s-object is being deleted',
                         relation.dc_title(),
                         rtype,
                     )
                     relation.cw_delete()
                 else:
-                    argname = "{}-subject-{}".format(rtype, relation.eid)
+                    argname = f"{rtype}-subject-{relation.eid}"
                     errors[rtype] = _(
                         '"%({})s" would need to be deleted alongside '
                         "the AuthorityRecord but this is disallowed"
                     ).format(argname)
                     msgargs[argname] = relation.dc_title()
         if errors:
             raise ValidationError(self.entity.eid, errors, msgargs)
```

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/i18n/en.po` & `cubicweb-eac-2.0.0/cubicweb_eac/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/i18n/fr.po` & `cubicweb-eac-2.0.0/cubicweb_eac/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/migration/0.3.0_Any.py` & `cubicweb-eac-2.0.0/cubicweb_eac/migration/0.3.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/migration/0.9.0_Any.py` & `cubicweb-eac-2.0.0/cubicweb_eac/migration/0.9.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/migration/postcreate.py` & `cubicweb-eac-2.0.0/cubicweb_eac/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/schema.py` & `cubicweb-eac-2.0.0/cubicweb_eac/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/sobjects.py` & `cubicweb-eac-2.0.0/cubicweb_eac/sobjects.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             extid2eid = init_extid2eid_index(self._cw, source)
         importer = ExtEntitiesImporter(
             self._cw.vreg.schema,
             store,
             import_log=import_log,
             extid2eid=extid2eid,
             etypes_order_hint=dataimport.ETYPES_ORDER_HINT,
-            **kwargs
+            **kwargs,
         )
         generator = self.external_entities_generator(stream, import_log)
         extentities = self.external_entities_stream(
             generator.external_entities(), extid2eid
         )
         importer.import_entities(extentities)
         if generator.record is not None:
@@ -112,13 +112,13 @@
             """Create agent kind when necessary and remove them from the entity stream, allowing to
             set cwuri properly without attempt to update.
             """
             for extentity in extentities:
                 if extentity.etype == "AgentKind":
                     assert (
                         extentity.extid in extid2eid
-                    ), "unexpected agent kind {}".format(extentity)
+                    ), f"unexpected agent kind {extentity}"
                 else:
                     yield extentity
 
         extentities = handle_agent_kind(extentities)
         return extentities
```

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/testutils.py` & `cubicweb-eac-2.0.0/cubicweb_eac/testutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     import_log = SimpleImportLog(basename(fpath))
     created, updated, _ = cnx.call_service(
         "eac.import", stream=fpath, import_log=import_log, raise_on_error=True
     )
     return created, updated
 
 
-class XmlTestMixin(object):
+class XmlTestMixin:
     """Mixin class provinding additional assertion methods for checking XML data."""
 
     def assertXmlEqual(self, actual, expected):
         """Check that both XML strings represent the same XML tree."""
         checker = LXMLOutputChecker()
         if not checker.check_output(expected, actual, 0):
             message = checker.output_difference(Example("", expected), actual, 0)
```

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac/views.py` & `cubicweb-eac-2.0.0/cubicweb_eac/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 .. _`saem_ref`: https://www.cubicweb.org/project/cubicweb-saem_ref
 """
 
 from functools import partial
 import os.path
 
 from cubicweb import tags, _
-from cubicweb.view import View
+from cubicweb_web.view import View
 from cubicweb.predicates import (
     is_instance,
     match_user_groups,
     one_line_rset,
     score_entity,
 )
 from cubicweb.dataimport.importer import HTMLImportLog
-from cubicweb.web import (
+from cubicweb_web import (
     action,
     component,
     formfields as ff,
     formwidgets as fw,
     httpcache,
 )
-from cubicweb.web.views import actions, calendar, cwsources, forms, idownloadable, uicfg
+from cubicweb_web.views import actions, calendar, cwsources, forms, idownloadable, uicfg
 
 from cubicweb_skos import to_unicode
 
 from cubicweb_eac import dataimport
 
 
 abaa = uicfg.actionbox_appearsin_addmenu
@@ -258,15 +258,15 @@
     def stop(self):
         return self.entity.end_date
 
 
 # Import
 
 
-class EACImportMixin(object):
+class EACImportMixin:
     __regid__ = "eac.import"
     __select__ = match_user_groups("managers", "users")
 
 
 class EACImportForm(EACImportMixin, forms.FieldsForm):
     """File import form for EAC-CPF"""
```

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac.egg-info/PKG-INFO` & `cubicweb-eac-2.0.0/cubicweb_eac.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cubicweb-eac
-Version: 1.5.3
+Version: 2.0.0
 Summary: Implementation of Encoded Archival Context for CubicWeb
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-eac
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Description: Summary
-        -------
-        Implementation of Encoded Archival Context for CubicWeb
-        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: JavaScript
+
+Summary
+-------
+Implementation of Encoded Archival Context for CubicWeb
+
+
```

### Comparing `cubicweb-eac-1.5.3/cubicweb_eac.egg-info/SOURCES.txt` & `cubicweb-eac-2.0.0/cubicweb_eac.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 MANIFEST.in
 README.rst
-a.txt
-b.txt
 dev-requirements.txt
 setup.py
 tox.ini
 cubicweb_eac/__init__.py
 cubicweb_eac/__pkginfo__.py
 cubicweb_eac/ccplugin.py
 cubicweb_eac/dataimport.py
@@ -47,22 +45,22 @@
 test/test_views.py
 test/utils.py
 test/data/FRAD033_EAC_00001.xml
 test/data/FRAD033_EAC_00001_simplified.xml
 test/data/FRAD033_EAC_00001_simplified_export.xml
 test/data/FRAD033_EAC_00003.xml
 test/data/FRAD033_EAC_00071.xml
-test/data/FRAN_NP_050553.xml
-test/data/FRAN_NP_050805.xml
 test/data/Service de l'administration generale et des assemblees.xml
 test/data/bootstrap_cubes
 test/data/cpf.xsd
 test/data/custom_kind.xml
 test/data/family_rico.ttl
 test/data/invalid_xml.xml
 test/data/missing_tag.xml
 test/data/no_name_entry.xml
 test/data/no_name_entry_part.xml
 test/data/organization_rdf.ttl
 test/data/organization_rico.ttl
 test/data/person_rdf.ttl
-test/data/person_rico.ttl
+test/data/person_rico.ttl
+test/data/xlink.xsd
+test/data/xml.xsd
```

### Comparing `cubicweb-eac-1.5.3/doc/supported.rst` & `cubicweb-eac-2.0.0/doc/supported.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/setup.py` & `cubicweb-eac-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
 install_requires = [
-    "{0} {1}".format(d, v and v or "").strip() for d, v in requires.items()
+    "{} {}".format(d, v and v or "").strip() for d, v in requires.items()
 ]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
```

### Comparing `cubicweb-eac-1.5.3/test/data/FRAD033_EAC_00001.xml` & `cubicweb-eac-2.0.0/test/data/FRAD033_EAC_00001.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/data/FRAD033_EAC_00001_simplified.xml` & `cubicweb-eac-2.0.0/test/data/FRAD033_EAC_00001_simplified.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/data/FRAD033_EAC_00001_simplified_export.xml` & `cubicweb-eac-2.0.0/test/data/FRAD033_EAC_00001_simplified_export.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/data/FRAD033_EAC_00003.xml` & `cubicweb-eac-2.0.0/test/data/FRAD033_EAC_00003.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/data/FRAD033_EAC_00071.xml` & `cubicweb-eac-2.0.0/test/data/FRAD033_EAC_00071.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/data/Service de l'administration generale et des assemblees.xml` & `cubicweb-eac-2.0.0/test/data/Service de l'administration generale et des assemblees.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/data/cpf.xsd` & `cubicweb-eac-2.0.0/test/data/cpf.xsd`

 * *Files 1% similar despite different names*

#### Comparing `cubicweb-eac-1.5.3/test/data/cpf.xsd` & `cubicweb-eac-2.0.0/test/data/cpf.xsd`

```diff
@@ -53,16 +53,16 @@
   
   The work of the EACWG has been supported by the Society of American Archivists, Staatsbibliothek 
   zu Berlin, Archivio di Stato di Bologna, Istituto per i Beni Artistici, Culturali e Naturali 
   della Regione Emilia-Romagna, and by generous funding from the Delmas Foundation.
   
 -->
 <xs:schema xmlns="urn:isbn:1-931666-33-4" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:xs="http://www.w3.org/2001/XMLSchema" elementFormDefault="qualified" targetNamespace="urn:isbn:1-931666-33-4">
-  <xs:import namespace="http://www.w3.org/1999/xlink" schemaLocation="http://www.loc.gov/standards/xlink/xlink.xsd"/>
-  <xs:import namespace="http://www.w3.org/XML/1998/namespace" schemaLocation="http://www.w3.org/2007/08/xml.xsd"/>
+  <xs:import namespace="http://www.w3.org/1999/xlink" schemaLocation="xlink.xsd"/>
+  <xs:import namespace="http://www.w3.org/XML/1998/namespace" schemaLocation="xml.xsd"/>
   <xs:element name="eac-cpf">
     <xs:complexType>
       <xs:sequence>
         <xs:element ref="control"/>
         <xs:choice>
           <xs:element ref="cpfDescription"/>
           <xs:element ref="multipleIdentities"/>
```

### Comparing `cubicweb-eac-1.5.3/test/data/custom_kind.xml` & `cubicweb-eac-2.0.0/test/data/custom_kind.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/data/missing_tag.xml` & `cubicweb-eac-2.0.0/test/data/missing_tag.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/data/no_name_entry.xml` & `cubicweb-eac-2.0.0/test/data/no_name_entry.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/data/no_name_entry_part.xml` & `cubicweb-eac-2.0.0/test/data/no_name_entry_part.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/data/person_rico.ttl` & `cubicweb-eac-2.0.0/test/data/person_rico.ttl`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix rico: <https://www.ica.org/standards/RiC/ontology#> .
 @prefix ricoform: <https://www.ica.org/standards/RiC/vocabularies/documentaryFormTypes#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 
-<{{BASE_URL}}{{name}}> a rico:AgentName ;
-    rico:isOrWasAgentNameOf <{{BASE_URL}}{{eid}}#agent> ;
+<{{name_uri}}> a rico:AgentName ;
+    rico:isOrWasAgentNameOf <{{uri}}#agent> ;
     rico:textualValue "Jean Jacques" ;
     rico:type "authorized" .
 
-<{{BASE_URL}}{{eid}}#inst> a rico:Instantiation ;
+<{{uri}}#inst> a rico:Instantiation ;
     rico:identifier "A123" ;
-    rico:isInstantiationOf <{{BASE_URL}}{{eid}}> .
+    rico:isInstantiationOf <{{uri}}> .
 
-<{{BASE_URL}}{{fam1}}#agent> rico:hasFamilyAssociationWith <{{BASE_URL}}{{eid}}#agent> ;
-    rico:personHasFamilyRelation <{{BASE_URL}}{{eid}}#family_to_B123> .
+<{{fam1_uri}}#agent> rico:hasFamilyAssociationWith <{{uri}}#agent> ;
+    rico:personHasFamilyRelation <{{uri}}#family_to_B123> .
 
-<{{BASE_URL}}{{fam2}}#agent> rico:hasFamilyAssociationWith <{{BASE_URL}}{{eid}}#agent> ;
-    rico:personHasFamilyRelation <{{BASE_URL}}{{eid}}#family_to_B234> .
+<{{fam2_uri}}#agent> rico:hasFamilyAssociationWith <{{uri}}#agent> ;
+    rico:personHasFamilyRelation <{{uri}}#family_to_B234> .
 
-<{{BASE_URL}}{{occupation}}> a rico:OccupationType, rico:ActivityType ;
+<{{occupation_uri}}> a rico:OccupationType ;
     rdfs:label "fan de poules" ;
-    rico:isOrWasOccupationTypeOf <{{BASE_URL}}{{eid}}#agent> .
+    rico:isOrWasOccupationTypeOf <{{uri}}#agent> .
 
-<{{BASE_URL}}{{eid}}#family_to_B123> a rico:FamilyRelation ;
-    rico:familyRelationConnects <{{BASE_URL}}{{fam1}}#agent>,
-        <{{BASE_URL}}{{eid}}#agent> .
-
-<{{BASE_URL}}{{eid}}#family_to_B234> a rico:FamilyRelation ;
-    rico:familyRelationConnects <{{BASE_URL}}{{fam2}}#agent>,
-        <{{BASE_URL}}{{eid}}#agent> .
+<{{uri}}#family_to_B123> a rico:FamilyRelation ;
+    rico:familyRelationConnects <{{fam1_uri}}#agent>,
+        <{{uri}}#agent> .
+
+<{{uri}}#family_to_B234> a rico:FamilyRelation ;
+    rico:familyRelationConnects <{{fam2_uri}}#agent>,
+        <{{uri}}#agent> .
 
-<{{BASE_URL}}{{eid}}> a rico:Record ;
-    rico:describesOrDescribed <{{BASE_URL}}{{eid}}#agent> ;
+<{{uri}}> a rico:Record ;
+    rico:describesOrDescribed <{{uri}}#agent> ;
     rico:hasDocumentaryForm ricoform:AuthorityRecord ;
-    rico:hasInstantiation <{{BASE_URL}}{{eid}}#inst> .
+    rico:hasInstantiation <{{uri}}#inst> .
 
-<{{BASE_URL}}{{family}}#agent> rico:groupIsSourceOfMembershipRelation <{{BASE_URL}}{{eid}}#family_to_F123> ;
-    rico:hasOrHadMember <{{BASE_URL}}{{eid}}#agent> .
+<{{family_uri}}#agent> rico:groupIsSourceOfMembershipRelation <{{uri}}#family_to_F123> ;
+    rico:hasOrHadMember <{{uri}}#agent> .
 
-<{{BASE_URL}}{{eid}}#family_to_F123> a rico:MembershipRelation ;
-    rico:membershipRelationHasSource <{{BASE_URL}}{{family}}#agent> ;
-    rico:membershipRelationHasTarget <{{BASE_URL}}{{eid}}#agent> .
+<{{uri}}#family_to_F123> a rico:MembershipRelation ;
+    rico:membershipRelationHasSource <{{family_uri}}#agent> ;
+    rico:membershipRelationHasTarget <{{uri}}#agent> .
 
-<{{BASE_URL}}{{eid}}#agent> a rico:Agent,
+<{{uri}}#agent> a rico:Agent,
         rico:Person ;
     rico:agentIsTargetOfPerformanceRelation _:N99fdb5f2c68c49ca964757cf2f695b1e ;
     rico:birthDate "2010-01-01"^^xsd:date ;
     rico:deathDate "2050-05-02"^^xsd:date ;
-    rico:isOrWasDescribedBy <{{BASE_URL}}{{eid}}> ;
-    rico:hasFamilyAssociationWith <{{BASE_URL}}{{fam1}}#agent>,
-        <{{BASE_URL}}{{fam2}}#agent> ;
-    rico:hasOrHadAgentName <{{BASE_URL}}{{name}}> ;
-    rico:hasOrHadOccupationOfType <{{BASE_URL}}{{occupation}}> ;
-    rico:isOrWasMemberOf <{{BASE_URL}}{{family}}#agent> ;
+    rico:isOrWasDescribedBy <{{uri}}> ;
+    rico:hasFamilyAssociationWith <{{fam1_uri}}#agent>,
+        <{{fam2_uri}}#agent> ;
+    rico:hasOrHadAgentName <{{name_uri}}> ;
+    rico:hasOrHadOccupationOfType <{{occupation_uri}}> ;
+    rico:isOrWasMemberOf <{{family_uri}}#agent> ;
     rico:name "Jean Jacques" ;
     rico:performsOrPerformed _:N5264360765f4419fa567c3dff26adc17 ;
-    rico:personHasFamilyRelation <{{BASE_URL}}{{eid}}#family_to_B123>,
-        <{{BASE_URL}}{{eid}}#family_to_B234> ;
-    rico:personIsTargetOfMembershipRelation <{{BASE_URL}}{{eid}}#family_to_F123> .
+    rico:personHasFamilyRelation <{{uri}}#family_to_B123>,
+        <{{uri}}#family_to_B234> ;
+    rico:personIsTargetOfMembershipRelation <{{uri}}#family_to_F123> .
 
 _:N5264360765f4419fa567c3dff26adc17 a rico:Activity ;
     rico:activityIsSourceOfPerformanceRelation _:N99fdb5f2c68c49ca964757cf2f695b1e ;
-    rico:hasActivityType <{{BASE_URL}}{{occupation}}> ;
-    rico:isOrWasPerformedBy <{{BASE_URL}}{{eid}}#agent> .
+    rico:hasActivityType <{{occupation_uri}}> ;
+    rico:isOrWasPerformedBy <{{uri}}#agent> .
 
 _:N99fdb5f2c68c49ca964757cf2f695b1e a rico:PerformanceRelation ;
     rico:performanceRelationHasSource _:N5264360765f4419fa567c3dff26adc17 ;
-    rico:performanceRelationHasTarget <{{BASE_URL}}{{eid}}#agent> .
+    rico:performanceRelationHasTarget <{{uri}}#agent> .
```

### Comparing `cubicweb-eac-1.5.3/test/export-roundtrip.rst` & `cubicweb-eac-2.0.0/test/export-roundtrip.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/export-simple.rst` & `cubicweb-eac-2.0.0/test/export-simple.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/test_dataimport.py` & `cubicweb-eac-2.0.0/test/test_dataimport.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding: utf-8
 # copyright 2015-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -41,31 +40,24 @@
 """
 
 
 def mock_(string):
     return string
 
 
-def tolist(dic):
-    """Transform sets in `dic` values as lists for easier comparison."""
-    for k, v in dic.items():
-        if isinstance(v, set):
-            v = list(v)
-        dic[k] = v
-    return dic
-
-
 def extentities2dict(entities):
     edict = {}
     for extentity in entities:
         edict.setdefault(extentity.etype, {})[extentity.extid] = extentity.values
     return edict
 
 
 class EACXMLParserTC(unittest.TestCase):
+    maxDiff = None
+
     @classmethod
     def datapath(cls, *fname):
         """joins the object's datadir and `fname`"""
         return join(dirname(__file__), "data", *fname)
 
     def file_extentities(self, fname):
         fpath = self.datapath(fname)
@@ -80,1000 +72,930 @@
     def test_parse_FRAD033_EAC_00001(self):
         _gen_extid = map(str, (x for x in count() if x not in (2, 38))).__next__
         expected = [
             (
                 "EACOtherRecordId",
                 _gen_extid(),
                 {
-                    "eac_other_record_id_of": set(
-                        ["authorityrecord-FRAD033_EAC_00001"]
-                    ),
-                    "value": set(["1234"]),
+                    "eac_other_record_id_of": {"authorityrecord-FRAD033_EAC_00001"},
+                    "value": {"1234"},
                 },
             ),
             (
                 "EACOtherRecordId",
                 _gen_extid(),
                 {
-                    "eac_other_record_id_of": set(
-                        ["authorityrecord-FRAD033_EAC_00001"]
-                    ),
-                    "value": set(["ABCD"]),
-                    "local_type": set(["letters"]),
+                    "eac_other_record_id_of": {"authorityrecord-FRAD033_EAC_00001"},
+                    "value": {"ABCD"},
+                    "local_type": {"letters"},
                 },
             ),
             (
                 "EACSource",
                 _gen_extid(),
                 {
-                    "source_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "title": set(["1. Ouvrages imprimés..."]),
-                    "description": set(["des bouquins"]),
-                    "description_format": set(["text/plain"]),
+                    "source_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "title": {"1. Ouvrages imprimés..."},
+                    "description": {"des bouquins"},
+                    "description_format": {"text/plain"},
                 },
             ),
             (
                 "EACSource",
                 _gen_extid(),
                 {
-                    "source_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "url": set(["http://archives.gironde.fr"]),
-                    "title": set(["Site des Archives départementales de la Gironde"]),
+                    "source_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "url": {"http://archives.gironde.fr"},
+                    "title": {"Site des Archives départementales de la Gironde"},
                 },
             ),
             (
                 "Activity",
                 _gen_extid(),
                 {
-                    "type": set(["create"]),
-                    "agent_type": ["human"],
-                    "generated": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "start": set([datetime.datetime(2013, 4, 24, 5, 34, 41)]),
-                    "end": set([datetime.datetime(2013, 4, 24, 5, 34, 41)]),
-                    "description": set(["bla bla"]),
-                    "description_format": set(["text/plain"]),
+                    "type": {"create"},
+                    "agent_type": {"human"},
+                    "generated": {"authorityrecord-FRAD033_EAC_00001"},
+                    "start": {datetime.datetime(2013, 4, 24, 5, 34, 41)},
+                    "end": {datetime.datetime(2013, 4, 24, 5, 34, 41)},
+                    "description": {"bla bla"},
+                    "description_format": {"text/plain"},
                 },
             ),
             (
                 "Activity",
                 _gen_extid(),
                 {
-                    "generated": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "type": set(["modify"]),
-                    "agent_type": ["human"],
-                    "start": set([datetime.datetime(2015, 1, 15, 7, 16, 33)]),
-                    "end": set([datetime.datetime(2015, 1, 15, 7, 16, 33)]),
-                    "agent": set(["Delphine Jamet"]),
+                    "generated": {"authorityrecord-FRAD033_EAC_00001"},
+                    "type": {"modify"},
+                    "agent_type": {"human"},
+                    "start": {datetime.datetime(2015, 1, 15, 7, 16, 33)},
+                    "end": {datetime.datetime(2015, 1, 15, 7, 16, 33)},
+                    "agent": {"Delphine Jamet"},
                 },
             ),
             (
                 "Convention",
                 _gen_extid(),
                 {
-                    "convention_of": ["authorityrecord-FRAD033_EAC_00001"],
-                    "abbrev": set(["ISAAR(CPF)"]),
-                    "has_citation": ["8"],
-                    "description_format": set(["text/html"]),
-                    "description": set(
-                        [
-                            '<p xmlns="urn:isbn:1-931666-33-4" '
-                            'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
-                            'xmlns:xlink="http://www.w3.org/1999/xlink">Norme '
-                            "ISAAR(CPF) du Conseil international des archives, "
-                            "2e \xe9dition, 1996.</p>"
-                        ]
-                    ),
+                    "convention_of": {"authorityrecord-FRAD033_EAC_00001"},
+                    "abbrev": {"ISAAR(CPF)"},
+                    "has_citation": {"8"},
+                    "description_format": {"text/html"},
+                    "description": {
+                        '<p xmlns="urn:isbn:1-931666-33-4" '
+                        'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+                        'xmlns:xlink="http://www.w3.org/1999/xlink">Norme '
+                        "ISAAR(CPF) du Conseil international des archives, "
+                        "2e \xe9dition, 1996.</p>"
+                    },
                 },
             ),
             (
                 "Citation",
                 _gen_extid(),
                 {
-                    "uri": set(["http://www.ica.org"]),
+                    "uri": {"http://www.ica.org"},
                 },
             ),
             (
                 "Convention",
                 _gen_extid(),
                 {
-                    "convention_of": ["authorityrecord-FRAD033_EAC_00001"],
-                    "description_format": set(["text/html"]),
-                    "description": set(
-                        [
-                            '<p xmlns="urn:isbn:1-931666-33-4" '
-                            'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
-                            'xmlns:xlink="http://www.w3.org/1999/xlink">AFNOR '
-                            "NF Z 44-060, octobre 1983, Catalogue "
-                            "d\u2019auteurs et d\u2019anonymes : forme et\n          "
-                            "structure des vedettes des collectivit\xe9s auteurs.</p>"
-                        ]
-                    ),
+                    "convention_of": {"authorityrecord-FRAD033_EAC_00001"},
+                    "description_format": {"text/html"},
+                    "description": {
+                        '<p xmlns="urn:isbn:1-931666-33-4" '
+                        'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+                        'xmlns:xlink="http://www.w3.org/1999/xlink">AFNOR '
+                        "NF Z 44-060, octobre 1983, Catalogue "
+                        "d\u2019auteurs et d\u2019anonymes : forme et\n          "
+                        "structure des vedettes des collectivit\xe9s auteurs.</p>"
+                    },
                 },
             ),
             (
                 "Convention",
                 _gen_extid(),
                 {
-                    "convention_of": ["authorityrecord-FRAD033_EAC_00001"],
-                    "description_format": set(["text/html"]),
-                    "description": set(
-                        [
-                            '<p xmlns="urn:isbn:1-931666-33-4" '
-                            'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
-                            'xmlns:xlink="http://www.w3.org/1999/xlink">Norme ISO 8601 '
-                            ":2004 \xc9l\xe9ments de donn\xe9es et formats "
-                            "d\u2019\xe9change -- \xc9change\n          "
-                            "d\u2019information -- Repr\xe9sentation de la date et "
-                            "de l\u2019heure.</p>"
-                        ]
-                    ),
+                    "convention_of": {"authorityrecord-FRAD033_EAC_00001"},
+                    "description_format": {"text/html"},
+                    "description": {
+                        '<p xmlns="urn:isbn:1-931666-33-4" '
+                        'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+                        'xmlns:xlink="http://www.w3.org/1999/xlink">Norme ISO 8601 '
+                        ":2004 \xc9l\xe9ments de donn\xe9es et formats "
+                        "d\u2019\xe9change -- \xc9change\n          "
+                        "d\u2019information -- Repr\xe9sentation de la date et "
+                        "de l\u2019heure.</p>"
+                    },
                 },
             ),
             (
                 "AgentKind",
                 "agentkind/authority",
-                {"name": set(["authority"])},
+                {"name": {"authority"}},
             ),
             (
                 "NameEntry",
                 _gen_extid(),
                 {
-                    "parts": set(["Gironde, Conseil général"]),
-                    "form_variant": set(["authorized"]),
-                    "name_entry_for": set(["authorityrecord-FRAD033_EAC_00001"]),
+                    "parts": {"Gironde, Conseil général"},
+                    "form_variant": {"authorized"},
+                    "name_entry_for": {"authorityrecord-FRAD033_EAC_00001"},
                 },
             ),
             (
                 "NameEntry",
                 _gen_extid(),
                 {
-                    "parts": set(["CG33"]),
-                    "form_variant": set(["alternative"]),
-                    "name_entry_for": set(["authorityrecord-FRAD033_EAC_00001"]),
+                    "parts": {"CG33"},
+                    "form_variant": {"alternative"},
+                    "name_entry_for": {"authorityrecord-FRAD033_EAC_00001"},
                 },
             ),
             (
                 "ParallelNames",
                 _gen_extid(),
                 {
-                    "parallel_names_of": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "simple_name_relation": set(["15", "14"]),
-                    "authorized_form": set(["AFNOR_Z44-060\n\t"]),
+                    "parallel_names_of": {"authorityrecord-FRAD033_EAC_00001"},
+                    "simple_name_relation": {"15", "14"},
+                    "authorized_form": {"AFNOR_Z44-060\n\t"},
                 },
             ),
             (
                 "NameEntry",
                 _gen_extid(),
                 {
-                    "script_code": set(["Latn"]),
-                    "preferred_form": ["AFNOR_Z44-060\n\t  "],
-                    "parts": set(
-                        ["Institut international des droits de\n\t  l'homme\n\t  "]
-                    ),
-                    "language": set(["fr"]),
+                    "script_code": {"Latn"},
+                    "preferred_form": {"AFNOR_Z44-060\n\t  "},
+                    "parts": {
+                        "Institut international des droits de\n\t  l'homme\n\t  "
+                    },
+                    "language": {"fr"},
                 },
             ),
             (
                 "NameEntry",
                 _gen_extid(),
                 {
-                    "script_code": set(["Latn"]),
-                    "parts": set(
-                        ["International institute of human\n\t  rights\n\t  "]
-                    ),
-                    "language": set(["en"]),
+                    "script_code": {"Latn"},
+                    "parts": {"International institute of human\n\t  rights\n\t  "},
+                    "language": {"en"},
                 },
             ),
             (
                 "ParallelNames",
                 _gen_extid(),
                 {
-                    "parallel_names_of": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "date_relation": set(["17", "18", "19"]),
-                    "simple_name_relation": set(["20", "21", "22"]),
+                    "parallel_names_of": {"authorityrecord-FRAD033_EAC_00001"},
+                    "date_relation": {"17", "18", "19"},
+                    "simple_name_relation": {"20", "21", "22"},
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
-                {"start_date": set([datetime.date(1949, 1, 1)])},
+                {"start_date": {datetime.date(1949, 1, 1)}},
             ),
             (
                 "DateEntity",
                 _gen_extid(),
-                {"start_date": set([datetime.date(1950, 1, 1)])},
+                {"start_date": {datetime.date(1950, 1, 1)}},
             ),
             (
                 "DateEntity",
                 _gen_extid(),
-                {"start_date": set([datetime.date(1950, 1, 1)])},
+                {"start_date": {datetime.date(1950, 1, 1)}},
             ),
             (
                 "NameEntry",
                 _gen_extid(),
-                {"parts": ["Federal Chancellery\n\t  of Germany\n\t  "]},
+                {"parts": {"Federal Chancellery\n\t  of Germany\n\t  "}},
             ),
             (
                 "NameEntry",
                 _gen_extid(),
-                {"parts": ["Chancellerie f\xe9d\xe9rale\n\t  d'Allemagne\n\t  "]},
+                {"parts": {"Chancellerie f\xe9d\xe9rale\n\t  d'Allemagne\n\t  "}},
             ),
             (
                 "NameEntry",
                 _gen_extid(),
-                {"parts": set(["BK\n\t  "])},
+                {"parts": {"BK\n\t  "}},
             ),
             (
                 "PostalAddress",
                 _gen_extid(),
                 {
-                    "street": set(["1 Esplanade Charles de Gaulle"]),
-                    "postalcode": set(["33074"]),
-                    "raw_address": set(
-                        ["1 Esplanade Charles de Gaulle\n33074\n Bordeaux Cedex"]
-                    ),
-                    "city": set([" Bordeaux Cedex"]),
+                    "street": {"1 Esplanade Charles de Gaulle"},
+                    "postalcode": {"33074"},
+                    "raw_address": {
+                        "1 Esplanade Charles de Gaulle\n33074\n Bordeaux Cedex"
+                    },
+                    "city": {" Bordeaux Cedex"},
                 },
             ),
             (
                 "AgentPlace",
                 _gen_extid(),
                 {
-                    "role": set(["siege"]),
-                    "place_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "place_entry_relation": set(["25"]),
-                    "place_address": set(["23"]),
+                    "role": {"siege"},
+                    "place_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "place_entry_relation": {"25"},
+                    "place_address": {"23"},
                 },
             ),
             (
                 "PlaceEntry",
                 _gen_extid(),
                 {
-                    "name": set(["Bordeaux (Gironde, France)"]),
-                    "equivalent_concept": set(
-                        ["http://catalogue.bnf.fr/ark:/12148/cb152418385"]
-                    ),
+                    "name": {"Bordeaux (Gironde, France)"},
+                    "equivalent_concept": {
+                        "http://catalogue.bnf.fr/ark:/12148/cb152418385"
+                    },
                 },
             ),
             (
                 "AgentPlace",
                 _gen_extid(),
                 {
-                    "place_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "place_entry_relation": set(["27"]),
-                    "role": set(["domicile"]),
+                    "place_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "place_entry_relation": {"27"},
+                    "role": {"domicile"},
                 },
             ),
             (
                 "PlaceEntry",
                 _gen_extid(),
                 {
-                    "latitude": set(["43.60426"]),
-                    "local_type": set(["other"]),
-                    "longitude": set(["1.44367"]),
-                    "name": set(["Toulouse (France)"]),
+                    "latitude": {"43.60426"},
+                    "local_type": {"other"},
+                    "longitude": {"1.44367"},
+                    "name": {"Toulouse (France)"},
                 },
             ),
             (
                 "AgentPlace",
                 _gen_extid(),
                 {
-                    "place_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "role": set(["dodo"]),
-                    "place_entry_relation": set(["29"]),
+                    "place_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "role": {"dodo"},
+                    "place_entry_relation": {"29"},
                 },
             ),
             (
                 "PlaceEntry",
                 _gen_extid(),
                 {
-                    "name": set(["Lit"]),
+                    "name": {"Lit"},
                 },
             ),
             (
                 "LegalStatus",
                 _gen_extid(),
                 {
-                    "term": set(["Collectivité territoriale"]),
-                    "date_relation": set(["31"]),
-                    "description": set(["Description du statut"]),
-                    "description_format": set(["text/plain"]),
-                    "legal_status_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
+                    "term": {"Collectivité territoriale"},
+                    "date_relation": {"31"},
+                    "description": {"Description du statut"},
+                    "description_format": {"text/plain"},
+                    "legal_status_agent": {"authorityrecord-FRAD033_EAC_00001"},
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
                 {
-                    "start_date": set([datetime.date(1234, 1, 1)]),
-                    "end_date": set([datetime.date(3000, 1, 1)]),
+                    "start_date": {datetime.date(1234, 1, 1)},
+                    "end_date": {datetime.date(3000, 1, 1)},
                 },
             ),
             (
                 "Mandate",
                 _gen_extid(),
                 {
-                    "term": set(["1. Constitutions françaises"]),
-                    "description": set(["Description du mandat"]),
-                    "description_format": set(["text/plain"]),
-                    "mandate_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
+                    "term": {"1. Constitutions françaises"},
+                    "description": {"Description du mandat"},
+                    "description_format": {"text/plain"},
+                    "mandate_agent": {"authorityrecord-FRAD033_EAC_00001"},
                 },
             ),
             (
                 "History",
                 _gen_extid(),
                 {
-                    "abstract": set(["Test of an abstract element"]),
-                    "has_citation": set(["39", "40"]),
-                    "has_event": set(["36", "34"]),
-                    "text": set(
-                        [
-                            "\n".join(
-                                (
-                                    '<p xmlns="urn:isbn:1-931666-33-4" '
-                                    'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
-                                    'xmlns:xlink="http://www.w3.org/1999/xlink">{0}</p>'
-                                ).format(text)
-                                for text in [
-                                    "La loi du 22 décembre 1789, en divisant ...",
-                                    "L'inspecteur Canardo",
-                                ]
-                            )
-                        ]
-                    ),
-                    "text_format": set(["text/html"]),
-                    "items": set(
-                        [
-                            '<ul  >\n\t    <li>\n\t      <span style="font-'
-                            '       style:italic">1450-1950\n\t      </span>\n\t'
-                            "      (1929)\n\t    </li>\n\t    <li>\n\t      "
-                            '<span style="font-style:italic">Globe\n\t      '
-                            "Gliding\n\t      </span>\n\t      (1930)\n\t    </l"
-                            'i>\n\t    <li>\n\t      <span style="font-     '
-                            '  style:italic">Gems\n\t      </span>\n\t      '
-                            "(1931)\n\t    </li>\n\t  </ul>\n      "
-                        ]
-                    ),
-                    "items_format": set(["text/html"]),
-                    "history_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
+                    "abstract": {"Test of an abstract element"},
+                    "has_citation": {"39", "40"},
+                    "has_event": {"36", "34"},
+                    "text": {
+                        "\n".join(
+                            (
+                                '<p xmlns="urn:isbn:1-931666-33-4" '
+                                'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+                                'xmlns:xlink="http://www.w3.org/1999/xlink">{}</p>'
+                            ).format(text)
+                            for text in [
+                                "La loi du 22 décembre 1789, en divisant ...",
+                                "L'inspecteur Canardo",
+                            ]
+                        )
+                    },
+                    "text_format": {"text/html"},
+                    "items": {
+                        '<ul  >\n\t    <li>\n\t      <span style="font-'
+                        '       style:italic">1450-1950\n\t      </span>\n\t'
+                        "      (1929)\n\t    </li>\n\t    <li>\n\t      "
+                        '<span style="font-style:italic">Globe\n\t      '
+                        "Gliding\n\t      </span>\n\t      (1930)\n\t    </l"
+                        'i>\n\t    <li>\n\t      <span style="font-     '
+                        '  style:italic">Gems\n\t      </span>\n\t      '
+                        "(1931)\n\t    </li>\n\t  </ul>\n      "
+                    },
+                    "items_format": {"text/html"},
+                    "history_agent": {"authorityrecord-FRAD033_EAC_00001"},
                 },
             ),
             (
                 "HistoricalEvent",
                 _gen_extid(),
                 {
-                    "date_relation": set(["35"]),
-                    "event": [
+                    "date_relation": {"35"},
+                    "event": {
                         "Left Mer and moved to the mainland.\n\t      "
                         "Worked at various jobs including canecutter\n\t      "
                         "and railway labourer.\n\t      "
-                    ],
+                    },
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
                 {
-                    "end_date": [datetime.date(1957, 1, 1)],
-                    "start_date": [datetime.date(1957, 1, 1)],
+                    "end_date": {datetime.date(1957, 1, 1)},
+                    "start_date": {datetime.date(1957, 1, 1)},
                 },
             ),
             (
                 "HistoricalEvent",
                 _gen_extid(),
                 {
-                    "date_relation": set(["37"]),
-                    "event": set(
-                        [
-                            "Union representative, Townsville-\n\t      "
-                            "Mount Isa rail construction project.\n\t      "
-                        ]
-                    ),
+                    "date_relation": {"37"},
+                    "event": {
+                        "Union representative, Townsville-\n\t      "
+                        "Mount Isa rail construction project.\n\t      "
+                    },
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
                 {
-                    "end_date": [datetime.date(1961, 1, 1)],
-                    "start_date": [datetime.date(1960, 1, 1)],
+                    "end_date": {datetime.date(1961, 1, 1)},
+                    "start_date": {datetime.date(1960, 1, 1)},
                 },
             ),
             (
                 "Citation",
                 _gen_extid(),
                 {
-                    "uri": set(
-                        [
-                            "http://www.assemblee-nationale.fr/histoire/images-decentralisation/"
-                            "decentralisation/loi-du-22-decembre-1789-.pdf"
-                        ]
-                    )
+                    "uri": {
+                        "http://www.assemblee-nationale.fr/histoire/images-decentralisation/"
+                        "decentralisation/loi-du-22-decembre-1789-.pdf"
+                    }
                 },
             ),
             (
                 "Citation",
                 _gen_extid(),
                 {
-                    "uri": set(["http://pifgadget"]),
-                    "note": set(["Voir aussi pifgadget"]),
+                    "uri": {"http://pifgadget"},
+                    "note": {"Voir aussi pifgadget"},
                 },
             ),
             (
                 "Structure",
                 _gen_extid(),
                 {
-                    "description": set(
-                        [
-                            '<p xmlns="urn:isbn:1-931666-33-4" '
-                            'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
-                            'xmlns:xlink="http://www.w3.org/1999/xlink">Pour accomplir '
-                            "ses missions ...</p>"
-                        ]
-                    ),
-                    "description_format": set(["text/html"]),
-                    "has_citation": set(["42"]),
-                    "structure_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
+                    "description": {
+                        '<p xmlns="urn:isbn:1-931666-33-4" '
+                        'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+                        'xmlns:xlink="http://www.w3.org/1999/xlink">Pour accomplir '
+                        "ses missions ...</p>"
+                    },
+                    "description_format": {"text/html"},
+                    "has_citation": {"42"},
+                    "structure_agent": {"authorityrecord-FRAD033_EAC_00001"},
                 },
             ),
             (
                 "Citation",
                 _gen_extid(),
                 {
-                    "note": set(
-                        [
-                            "L'\xe9l\xe9ment Citation \xe0 fournir un lien vers un document "
-                            "externe comme un\n               organigramme ou un arbre "
-                            "g\xe9n\xe9alogique. Pour une pr\xe9sentation plus simple, "
-                            "sous forme\n               de texte, on peut utiliser un "
-                            "ou plusieurs \xe9l\xe9m."
-                        ]
-                    )
+                    "note": {
+                        "L'\xe9l\xe9ment Citation \xe0 fournir un lien vers un document "
+                        "externe comme un\n               organigramme ou un arbre "
+                        "g\xe9n\xe9alogique. Pour une pr\xe9sentation plus simple, "
+                        "sous forme\n               de texte, on peut utiliser un "
+                        "ou plusieurs \xe9l\xe9m."
+                    }
                 },
             ),
             (
                 "AgentFunction",
                 _gen_extid(),
                 {
-                    "description": set(
-                        [
-                            '<p xmlns="urn:isbn:1-931666-33-4" '
-                            'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
-                            'xmlns:xlink="http://www.w3.org/1999/xlink">Quatre grands '
-                            "domaines de compétence...</p>"
-                        ]
-                    ),
-                    "description_format": set(["text/html"]),
-                    "function_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
+                    "description": {
+                        '<p xmlns="urn:isbn:1-931666-33-4" '
+                        'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+                        'xmlns:xlink="http://www.w3.org/1999/xlink">Quatre grands '
+                        "domaines de compétence...</p>"
+                    },
+                    "description_format": {"text/html"},
+                    "function_agent": {"authorityrecord-FRAD033_EAC_00001"},
                 },
             ),
             (
                 "AgentFunction",
                 _gen_extid(),
                 {
-                    "name": set(["action sociale"]),
-                    "function_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "description": set(
-                        [
-                            '<p xmlns="urn:isbn:1-931666-33-4" '
-                            'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
-                            'xmlns:xlink="http://www.w3.org/1999/xlink">1. Solidarité\n'
-                            "            blablabla.</p>"
-                        ]
-                    ),
-                    "description_format": set(["text/html"]),
-                    "equivalent_concept": set(
-                        ["http://data.culture.fr/thesaurus/page/ark:/67717/T1-200"]
-                    ),
+                    "name": {"action sociale"},
+                    "function_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "description": {
+                        '<p xmlns="urn:isbn:1-931666-33-4" '
+                        'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+                        'xmlns:xlink="http://www.w3.org/1999/xlink">1. Solidarité\n'
+                        "            blablabla.</p>"
+                    },
+                    "description_format": {"text/html"},
+                    "equivalent_concept": {
+                        "http://data.culture.fr/thesaurus/page/ark:/67717/T1-200"
+                    },
                 },
             ),
             (
                 "AgentFunction",
                 _gen_extid(),
                 {
-                    "name": set(["environnement"]),
-                    "function_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "equivalent_concept": set(
-                        ["http://data.culture.fr/thesaurus/page/ark:/67717/T1-1074"]
-                    ),
+                    "name": {"environnement"},
+                    "function_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "equivalent_concept": {
+                        "http://data.culture.fr/thesaurus/page/ark:/67717/T1-1074"
+                    },
                 },
             ),
             (
                 "Occupation",
                 _gen_extid(),
                 {
-                    "term": set(["Réunioniste"]),
-                    "date_relation": set(["47"]),
-                    "description": set(["Organisation des réunions ..."]),
-                    "description_format": set(["text/plain"]),
-                    "occupation_agent": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "has_citation": set(["48"]),
-                    "equivalent_concept": set(["http://pifgadget.com"]),
+                    "term": {"Réunioniste"},
+                    "date_relation": {"47"},
+                    "description": {"Organisation des réunions ..."},
+                    "description_format": {"text/plain"},
+                    "occupation_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "has_citation": {"48"},
+                    "equivalent_concept": {"http://pifgadget.com"},
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
                 {
-                    "start_date": set([datetime.date(1987, 1, 1)]),
-                    "end_date": set([datetime.date(2099, 1, 1)]),
+                    "start_date": {datetime.date(1987, 1, 1)},
+                    "end_date": {datetime.date(2099, 1, 1)},
                 },
             ),
             (
                 "Citation",
                 _gen_extid(),
                 {
-                    "note": set(["la bible"]),
+                    "note": {"la bible"},
                 },
             ),
             (
                 "GeneralContext",
                 _gen_extid(),
                 {
-                    "content": set(
-                        [
-                            '<p xmlns="urn:isbn:1-931666-33-4" '
-                            'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
-                            'xmlns:xlink="http://www.w3.org/1999/xlink">very famous</p>'
-                        ]
-                    ),
-                    "content_format": set(["text/html"]),
-                    "has_citation": set(["50"]),
-                    "general_context_of": set(["authorityrecord-FRAD033_EAC_00001"]),
+                    "content": {
+                        '<p xmlns="urn:isbn:1-931666-33-4" '
+                        'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+                        'xmlns:xlink="http://www.w3.org/1999/xlink">very famous</p>'
+                    },
+                    "content_format": {"text/html"},
+                    "has_citation": {"50"},
+                    "general_context_of": {"authorityrecord-FRAD033_EAC_00001"},
                 },
             ),
             (
                 "Citation",
                 _gen_extid(),
                 {
-                    "note": set(["it's well known"]),
+                    "note": {"it's well known"},
                 },
             ),
             (
                 "ExternalUri",
                 "CG33-DIRADSJ",
                 {
-                    "uri": set(["CG33-DIRADSJ"]),
-                    "cwuri": set(["CG33-DIRADSJ"]),
+                    "uri": {"CG33-DIRADSJ"},
+                    "cwuri": {"CG33-DIRADSJ"},
                 },
             ),
             (
                 "HierarchicalRelation",
                 _gen_extid(),
                 {
-                    "entry": set(
-                        [
-                            "Gironde. Conseil général. Direction de l'administration et de "
-                            "la sécurité juridique"
-                        ]
-                    ),
-                    "date_relation": set(["52"]),
-                    "description": set(["Coucou"]),
-                    "description_format": set(["text/plain"]),
-                    "hierarchical_parent": set(["CG33-DIRADSJ"]),
-                    "hierarchical_child": set(["authorityrecord-FRAD033_EAC_00001"]),
+                    "entry": {
+                        "Gironde. Conseil général. Direction de l'administration et de "
+                        "la sécurité juridique"
+                    },
+                    "date_relation": {"52"},
+                    "description": {"Coucou"},
+                    "description_format": {"text/plain"},
+                    "hierarchical_parent": {"CG33-DIRADSJ"},
+                    "hierarchical_child": {"authorityrecord-FRAD033_EAC_00001"},
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
                 {
-                    "start_date": set([datetime.date(2008, 1, 1)]),
-                    "end_date": set([datetime.date(2099, 1, 1)]),
+                    "start_date": {datetime.date(2008, 1, 1)},
+                    "end_date": {datetime.date(2099, 1, 1)},
                 },
             ),
             (
                 "ExternalUri",
                 "whatever",
                 {
-                    "uri": set(["whatever"]),
-                    "cwuri": set(["whatever"]),
+                    "uri": {"whatever"},
+                    "cwuri": {"whatever"},
                 },
             ),
             (
                 "ExternalUri",
                 "/dev/null",
                 {
-                    "uri": set(["/dev/null"]),
-                    "cwuri": set(["/dev/null"]),
+                    "uri": {"/dev/null"},
+                    "cwuri": {"/dev/null"},
                 },
             ),
             (
                 "ChronologicalRelation",
                 _gen_extid(),
                 {
-                    "chronological_predecessor": set(["whatever"]),
-                    "chronological_successor": set(
-                        ["authorityrecord-FRAD033_EAC_00001"]
-                    ),
-                    "date_relation": set(["54"]),
-                    "entry": set(["CG32"]),
+                    "chronological_predecessor": {"whatever"},
+                    "chronological_successor": {"authorityrecord-FRAD033_EAC_00001"},
+                    "date_relation": {"54"},
+                    "entry": {"CG32"},
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
                 {
-                    "start_date": set([datetime.date(1917, 1, 1)]),
-                    "end_date": set([datetime.date(2009, 1, 1)]),
+                    "start_date": {datetime.date(1917, 1, 1)},
+                    "end_date": {datetime.date(2009, 1, 1)},
                 },
             ),
             (
                 "ChronologicalRelation",
                 _gen_extid(),
                 {
-                    "chronological_predecessor": set(
-                        ["authorityrecord-FRAD033_EAC_00001"]
-                    ),
-                    "chronological_successor": set(["/dev/null"]),
-                    "date_relation": set(["56"]),
-                    "xml_wrap": set(
-                        [
-                            b'<gloups xmlns="urn:isbn:1-931666-33-4"'
-                            b' xmlns:xsi="http://www.w3.org/2001/XML'
-                            b'Schema-instance" xmlns:xlink="http://'
-                            b'www.w3.org/1999/xlink">hips</gloups>'
-                        ]
-                    ),
-                    "entry": set(["Trash"]),
+                    "chronological_predecessor": {"authorityrecord-FRAD033_EAC_00001"},
+                    "chronological_successor": {"/dev/null"},
+                    "date_relation": {"56"},
+                    "xml_wrap": {
+                        b'<gloups xmlns="urn:isbn:1-931666-33-4"'
+                        b' xmlns:xsi="http://www.w3.org/2001/XML'
+                        b'Schema-instance" xmlns:xlink="http://'
+                        b'www.w3.org/1999/xlink">hips</gloups>'
+                    },
+                    "entry": {"Trash"},
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
-                {"start_date": set([datetime.date(2042, 1, 1)])},
+                {"start_date": {datetime.date(2042, 1, 1)}},
             ),
             (
                 "IdentityRelation",
                 _gen_extid(),
                 {
-                    "date_relation": ["58"],
-                    "entry": ["Trash"],
-                    "identity_from": ["authorityrecord-FRAD033_EAC_00001"],
-                    "identity_to": ["/dev/null"],
-                    "xml_wrap": set(
-                        [
-                            b'<gloups xmlns="urn:isbn:1-931666-33-4" '
-                            b'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
-                            b'xmlns:xlink="http://www.w3.org/1999/xlink">hips</gloups>'
-                        ]
-                    ),
+                    "date_relation": {"58"},
+                    "entry": {"Trash"},
+                    "identity_from": {"authorityrecord-FRAD033_EAC_00001"},
+                    "identity_to": {"/dev/null"},
+                    "xml_wrap": {
+                        b'<gloups xmlns="urn:isbn:1-931666-33-4" '
+                        b'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+                        b'xmlns:xlink="http://www.w3.org/1999/xlink">hips</gloups>'
+                    },
                 },
             ),
-            ("DateEntity", _gen_extid(), {"start_date": [datetime.date(2042, 1, 1)]}),
+            ("DateEntity", _gen_extid(), {"start_date": {datetime.date(2042, 1, 1)}}),
             (
                 "FamilyRelation",
                 _gen_extid(),
                 {
-                    "date_relation": ["60"],
-                    "entry": ["CG32"],
-                    "family_from": ["authorityrecord-FRAD033_EAC_00001"],
-                    "family_to": ["whatever"],
+                    "date_relation": {"60"},
+                    "entry": {"CG32"},
+                    "family_from": {"authorityrecord-FRAD033_EAC_00001"},
+                    "family_to": {"whatever"},
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
                 {
-                    "end_date": [datetime.date(2009, 1, 1)],
-                    "start_date": [datetime.date(1917, 1, 1)],
+                    "end_date": {datetime.date(2009, 1, 1)},
+                    "start_date": {datetime.date(1917, 1, 1)},
                 },
             ),
             (
                 "AssociationRelation",
                 _gen_extid(),
                 {
-                    "association_from": set(["authorityrecord-FRAD033_EAC_00001"]),
-                    "association_to": set(["agent-x"]),
+                    "association_from": {"authorityrecord-FRAD033_EAC_00001"},
+                    "association_to": {"agent-x"},
                 },
             ),
             (
                 "EACResourceRelation",
                 _gen_extid(),
                 {
-                    "agent_role": set(["creatorOf"]),
-                    "date_relation": set(["63"]),
-                    "xml_attributes": set(
-                        [
-                            '{"{http://www.w3.org/1999/xlink}actuate": "onRequest", '
-                            '"{http://www.w3.org/1999/xlink}show": "new", '
-                            '"{http://www.w3.org/1999/xlink}type": "simple"}'
-                        ]
-                    ),
-                    "relation_entry": set(
-                        [
-                            "Gironde. Conseil g\xe9n\xe9ral. Direction de"
-                            " l'administration et de la s\xe9curit\xe9 juridique"
-                        ]
-                    ),
-                    "resource_role": set(["Fonds d'archives"]),
-                    "resource_relation_resource": set(
-                        ["http://gael.gironde.fr/ead.html?id=FRAD033_IR_N"]
-                    ),
-                    "resource_relation_agent": set(
-                        ["authorityrecord-FRAD033_EAC_00001"]
-                    ),
-                    "xml_wrap": set(
-                        [
-                            b'<he xmlns="urn:isbn:1-931666-33-4" '
-                            b'xmlns:xlink="http://www.w3.org/1999'
-                            b'/xlink" xmlns:xsi="http://www.w3.org'
-                            b'/2001/XMLSchema-instance">joe</he>'
-                        ]
-                    ),
+                    "agent_role": {"creatorOf"},
+                    "date_relation": {"63"},
+                    "xml_attributes": {
+                        '{"{http://www.w3.org/1999/xlink}actuate": "onRequest", '
+                        '"{http://www.w3.org/1999/xlink}show": "new", '
+                        '"{http://www.w3.org/1999/xlink}type": "simple"}'
+                    },
+                    "relation_entry": {
+                        "Gironde. Conseil g\xe9n\xe9ral. Direction de"
+                        " l'administration et de la s\xe9curit\xe9 juridique"
+                    },
+                    "resource_role": {"Fonds d'archives"},
+                    "resource_relation_resource": {
+                        "http://gael.gironde.fr/ead.html?id=FRAD033_IR_N"
+                    },
+                    "resource_relation_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "xml_wrap": {
+                        b'<he xmlns="urn:isbn:1-931666-33-4" '
+                        b'xmlns:xlink="http://www.w3.org/1999'
+                        b'/xlink" xmlns:xsi="http://www.w3.org'
+                        b'/2001/XMLSchema-instance">joe</he>'
+                    },
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
                 {
-                    "start_date": set([datetime.date(1673, 1, 1)]),
-                    "end_date": set([datetime.date(1963, 1, 1)]),
+                    "start_date": {datetime.date(1673, 1, 1)},
+                    "end_date": {datetime.date(1963, 1, 1)},
                 },
             ),
             (
                 "EACFunctionRelation",
                 _gen_extid(),
                 {
-                    "description": set(
-                        [
-                            '<p xmlns="urn:isbn:1-931666-33-4" xmlns:xsi="http:/'
-                            '/www.w3.org/2001/XMLSchema-instance" xmlns:xlink="http:'
-                            '//www.w3.org/1999/xlink">The management of the University'
-                            "'s\n\t  communication with its alumni.\n\t  </p>"
-                        ]
-                    ),
-                    "r_type": set(["performs"]),
-                    "description_format": set(["text/html"]),
-                    "function_relation_agent": set(
-                        ["authorityrecord-FRAD033_EAC_00001"]
-                    ),
-                    "function_relation_function": set(
-                        ["http://gael.gironde.fr/ead.html?" "id=FRAD033_IR_N"]
-                    ),
-                    "relation_entry": set(
-                        [
-                            "Alumni communication\n\tmanagement, "
-                            "University of\n\tGlasgow\n\t"
-                        ]
-                    ),
-                    "xml_wrap": set(
-                        [
-                            b'<mods xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"'
-                            b' xmlns="urn:isbn:1-931666-33-4" xmlns:xlink="http://www.w3'
-                            b'.org/1999/xlink" xsi:schemaLocation="http://www.loc.gov'
-                            b"/mods/v3 http:         //www.loc.gov/mods/v3/mods-3-3.xsd"
-                            b'">\n\t    <titleInfo>\n\t      <title>Artisti trentini'
-                            b" tra le due\n\t      guerre\n\t      </title>\n\t    </titleInfo"
-                            b'>\n\t    <name>\n\t      <namePart type="given">Nicoletta'
-                            b'\n\t      </namePart>\n\t      <namePart type="family'
-                            b'">Boschiero\n\t      </namePart>\n\t      <role>\n\t\t<roleTerm'
-                            b' type="text">autore\n\t\t</roleTerm>\n\t      </role>\n\t'
-                            b"    </name>\n\t  </mods>\n\t"
-                        ]
-                    ),
-                    "xml_attributes": set(
-                        [
-                            '{"{http://www.w3.org/1999/xlink}actuate": '
-                            '"onLoad", "{http://www.w3.org/1999/xlink}arcrole": '
-                            '"http://test_arcrole.lol.com", '
-                            '"{http://www.w3.org/1999/xlink}role": '
-                            '"http://test_role.lmao.com"}'
-                        ]
-                    ),
+                    "description": {
+                        '<p xmlns="urn:isbn:1-931666-33-4" xmlns:xsi="http:/'
+                        '/www.w3.org/2001/XMLSchema-instance" xmlns:xlink="http:'
+                        '//www.w3.org/1999/xlink">The management of the University'
+                        "'s\n\t  communication with its alumni.\n\t  </p>"
+                    },
+                    "r_type": {"performs"},
+                    "description_format": {"text/html"},
+                    "function_relation_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "function_relation_function": {
+                        "http://gael.gironde.fr/ead.html?" "id=FRAD033_IR_N"
+                    },
+                    "relation_entry": {
+                        "Alumni communication\n\tmanagement, "
+                        "University of\n\tGlasgow\n\t"
+                    },
+                    "xml_wrap": {
+                        b'<mods xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"'
+                        b' xmlns="urn:isbn:1-931666-33-4" xmlns:xlink="http://www.w3'
+                        b'.org/1999/xlink" xsi:schemaLocation="http://www.loc.gov'
+                        b"/mods/v3 http:         //www.loc.gov/mods/v3/mods-3-3.xsd"
+                        b'">\n\t    <titleInfo>\n\t      <title>Artisti trentini'
+                        b" tra le due\n\t      guerre\n\t      </title>\n\t    </titleInfo"
+                        b'>\n\t    <name>\n\t      <namePart type="given">Nicoletta'
+                        b'\n\t      </namePart>\n\t      <namePart type="family'
+                        b'">Boschiero\n\t      </namePart>\n\t      <role>\n\t\t<roleTerm'
+                        b' type="text">autore\n\t\t</roleTerm>\n\t      </role>\n\t'
+                        b"    </name>\n\t  </mods>\n\t"
+                    },
+                    "xml_attributes": {
+                        '{"{http://www.w3.org/1999/xlink}actuate": '
+                        '"onLoad", "{http://www.w3.org/1999/xlink}arcrole": '
+                        '"http://test_arcrole.lol.com", '
+                        '"{http://www.w3.org/1999/xlink}role": '
+                        '"http://test_role.lmao.com"}'
+                    },
                 },
             ),
             (
                 "EACFunctionRelation",
                 _gen_extid(),
                 {
-                    "function_relation_function": set(["FRAD033_IR_N"]),
-                    "function_relation_agent": set(
-                        ["authorityrecord-FRAD033_EAC_00001"]
-                    ),
-                    "description": set(
-                        [
-                            '<p xmlns="urn:isbn:1-931666-33-4" '
-                            'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
-                            'xmlns:xlink="http://www.w3.org/1999/xlink">'
-                            "The second responsibility of the\n\t  "
-                            "Department is to control the establishment\n\t  "
-                            "and abolishment of schools.\n\t  </p>"
-                        ]
-                    ),
-                    "r_type": set(["controls"]),
-                    "description_format": set(["text/html"]),
-                    "date_relation": set(["66"]),
-                    "relation_entry": set(
-                        ["Establishment and abolishment\n\tof schools\n\t"]
-                    ),
-                    "xml_attributes": set(["{}"]),
+                    "function_relation_function": {"FRAD033_IR_N"},
+                    "function_relation_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "description": {
+                        '<p xmlns="urn:isbn:1-931666-33-4" '
+                        'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+                        'xmlns:xlink="http://www.w3.org/1999/xlink">'
+                        "The second responsibility of the\n\t  "
+                        "Department is to control the establishment\n\t  "
+                        "and abolishment of schools.\n\t  </p>"
+                    },
+                    "r_type": {"controls"},
+                    "description_format": {"text/html"},
+                    "date_relation": {"66"},
+                    "relation_entry": {
+                        "Establishment and abolishment\n\tof schools\n\t"
+                    },
+                    "xml_attributes": {"{}"},
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
                 {
-                    "start_date": set([datetime.date(1922, 1, 1)]),
-                    "end_date": set([datetime.date(2001, 1, 1)]),
+                    "start_date": {datetime.date(1922, 1, 1)},
+                    "end_date": {datetime.date(2001, 1, 1)},
                 },
             ),
             (
                 "EACFunctionRelation",
                 _gen_extid(),
                 {
-                    "function_relation_agent": set(
-                        ["authorityrecord-FRAD033_EAC_00001"]
-                    ),
-                    "description": set(
-                        [
-                            '<p xmlns="urn:isbn:1-931666-33-4" '
-                            'xmlns:xsi="http://www.w3.org/2001/X'
-                            'MLSchema-instance" xmlns:xlink="http://ww'
-                            'w.w3.org/1999/xlink">Some description'
-                            "\n            </p>"
-                        ]
-                    ),
-                    "function_relation_function": set(["ONLY_XLINK"]),
-                    "description_format": set(["text/html"]),
-                    "relation_entry": set(["Some relation entry\n          "]),
-                    "xml_attributes": set(["{}"]),
-                    "date_relation": ["68"],
+                    "function_relation_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "description": {
+                        '<p xmlns="urn:isbn:1-931666-33-4" '
+                        'xmlns:xsi="http://www.w3.org/2001/X'
+                        'MLSchema-instance" xmlns:xlink="http://ww'
+                        'w.w3.org/1999/xlink">Some description'
+                        "\n            </p>"
+                    },
+                    "function_relation_function": {"ONLY_XLINK"},
+                    "description_format": {"text/html"},
+                    "relation_entry": {"Some relation entry\n          "},
+                    "xml_attributes": {"{}"},
+                    "date_relation": {"68"},
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
                 {
-                    "start_date": set([datetime.date(1922, 1, 1)]),
-                    "end_date": set([datetime.date(2001, 1, 1)]),
+                    "start_date": {datetime.date(1922, 1, 1)},
+                    "end_date": {datetime.date(2001, 1, 1)},
                 },
             ),
             (
                 "EACFunctionRelation",
                 _gen_extid(),
                 {
-                    "function_relation_agent": set(
-                        ["authorityrecord-FRAD033_EAC_00001"]
-                    ),
-                    "description": set(
-                        [
-                            '<p xmlns="urn:isbn:1-931666-33-4" '
-                            'xmlns:xsi="http://www.w3.org/2001/X'
-                            'MLSchema-instance" xmlns:xlink="http://ww'
-                            'w.w3.org/1999/xlink">Some description'
-                            "\n            </p>"
-                        ]
-                    ),
-                    "r_type": set(["ONLY_RELATION_TYPE"]),
-                    "description_format": set(["text/html"]),
-                    "relation_entry": set(["Some relation entry\n          "]),
-                    "xml_attributes": set(["{}"]),
-                    "date_relation": ["70"],
+                    "function_relation_agent": {"authorityrecord-FRAD033_EAC_00001"},
+                    "description": {
+                        '<p xmlns="urn:isbn:1-931666-33-4" '
+                        'xmlns:xsi="http://www.w3.org/2001/X'
+                        'MLSchema-instance" xmlns:xlink="http://ww'
+                        'w.w3.org/1999/xlink">Some description'
+                        "\n            </p>"
+                    },
+                    "r_type": {"ONLY_RELATION_TYPE"},
+                    "description_format": {"text/html"},
+                    "relation_entry": {"Some relation entry\n          "},
+                    "xml_attributes": {"{}"},
+                    "date_relation": {"70"},
                 },
             ),
             (
                 "DateEntity",
                 _gen_extid(),
                 {
-                    "start_date": set([datetime.date(1922, 1, 1)]),
-                    "end_date": set([datetime.date(2001, 1, 1)]),
+                    "start_date": {datetime.date(1922, 1, 1)},
+                    "end_date": {datetime.date(2001, 1, 1)},
                 },
             ),
             (
                 "ExternalUri",
                 "ONLY_XLINK",
-                {"uri": set(["ONLY_XLINK"]), "cwuri": set(["ONLY_XLINK"])},
+                {"uri": {"ONLY_XLINK"}, "cwuri": {"ONLY_XLINK"}},
             ),
             (
                 "ExternalUri",
                 "FRAD033_IR_N",
-                {"uri": set(["FRAD033_IR_N"]), "cwuri": set(["FRAD033_IR_N"])},
+                {"uri": {"FRAD033_IR_N"}, "cwuri": {"FRAD033_IR_N"}},
             ),
             (
                 "ExternalUri",
                 "http://gael.gironde.fr/ead.html?id=FRAD033_IR_N",
                 {
-                    "uri": set(["http://gael.gironde.fr/ead.html?id=FRAD033_IR_N"]),
-                    "cwuri": set(["http://gael.gironde.fr/ead.html?id=FRAD033_IR_N"]),
+                    "uri": {"http://gael.gironde.fr/ead.html?id=FRAD033_IR_N"},
+                    "cwuri": {"http://gael.gironde.fr/ead.html?id=FRAD033_IR_N"},
                 },
             ),
             (
                 "ExternalUri",
                 "agent-x",
-                {"uri": set(["agent-x"]), "cwuri": set(["agent-x"])},
+                {"uri": {"agent-x"}, "cwuri": {"agent-x"}},
             ),
             (
                 "ExternalUri",
                 "http://data.culture.fr/thesaurus/page/ark:/67717/T1-200",
                 {
-                    "uri": set(
-                        ["http://data.culture.fr/thesaurus/page/ark:/67717/T1-200"]
-                    ),
-                    "cwuri": set(
-                        ["http://data.culture.fr/thesaurus/page/ark:/67717/T1-200"]
-                    ),
+                    "uri": {"http://data.culture.fr/thesaurus/page/ark:/67717/T1-200"},
+                    "cwuri": {
+                        "http://data.culture.fr/thesaurus/page/ark:/67717/T1-200"
+                    },
                 },
             ),
             (
                 "ExternalUri",
                 "http://data.culture.fr/thesaurus/page/ark:/67717/T1-1074",
                 {
-                    "uri": set(
-                        ["http://data.culture.fr/thesaurus/page/ark:/67717/T1-1074"]
-                    ),
-                    "cwuri": set(
-                        ["http://data.culture.fr/thesaurus/page/ark:/67717/T1-1074"]
-                    ),
+                    "uri": {"http://data.culture.fr/thesaurus/page/ark:/67717/T1-1074"},
+                    "cwuri": {
+                        "http://data.culture.fr/thesaurus/page/ark:/67717/T1-1074"
+                    },
                 },
             ),
             (
                 "ExternalUri",
                 "http://catalogue.bnf.fr/ark:/12148/cb152418385",
                 {
-                    "uri": set(["http://catalogue.bnf.fr/ark:/12148/cb152418385"]),
-                    "cwuri": set(["http://catalogue.bnf.fr/ark:/12148/cb152418385"]),
+                    "uri": {"http://catalogue.bnf.fr/ark:/12148/cb152418385"},
+                    "cwuri": {"http://catalogue.bnf.fr/ark:/12148/cb152418385"},
                 },
             ),
             (
                 "ExternalUri",
                 "http://pifgadget.com",
                 {
-                    "uri": set(["http://pifgadget.com"]),
-                    "cwuri": set(["http://pifgadget.com"]),
+                    "uri": {"http://pifgadget.com"},
+                    "cwuri": {"http://pifgadget.com"},
                 },
             ),
             (
                 "AuthorityRecord",
                 "authorityrecord-FRAD033_EAC_00001",
                 {
-                    "isni": set(["22330001300016"]),
-                    "languages": ["English, Spanish"],
-                    "start_date": set([datetime.date(1800, 1, 1)]),
-                    "end_date": set([datetime.date(2099, 1, 1)]),
-                    "agent_kind": set(["agentkind/authority"]),
-                    "record_id": set(["FRAD033_EAC_00001"]),
+                    "isni": {"22330001300016"},
+                    "languages": {"English, Spanish"},
+                    "start_date": {datetime.date(1800, 1, 1)},
+                    "end_date": {datetime.date(2099, 1, 1)},
+                    "agent_kind": {"agentkind/authority"},
+                    "record_id": {"FRAD033_EAC_00001"},
                 },
             ),
         ]
+
         expected = [ExtEntity(*vals) for vals in expected]
         fpath = self.datapath("FRAD033_EAC_00001_simplified.xml")
         import_log = SimpleImportLog(fpath)
         # Use a predictable extid_generator.
         extid_generator = map(str, count()).__next__
         importer = dataimport.EACCPFImporter(
             fpath, import_log, mock_, extid_generator=extid_generator
         )
         entities = list(importer.external_entities())
+
         # Used for an easier handling of the order error while generating the 2 lists
         self.check_order_entities(entities, expected)
-        self.check_external_entities(entities, expected)
-        visited = set([])
+
+        assert extentities2dict(entities) == extentities2dict(expected)
+
+        visited = set()
         for x in importer._visited.values():
             visited.update(x)
+
         self.assertCountEqual(visited, [x.extid for x in expected])
+
         # Gather not-visited tag by name and group source lines.
         not_visited = {}
         for tagname, sourceline in importer.not_visited():
-            not_visited.setdefault(tagname, set([])).add(sourceline)
-        self.assertEqual(
-            not_visited,
-            {
-                "maintenanceStatus": set([12]),
-                "publicationStatus": set([14]),
-                "recordId": set([8]),
-                "maintenanceAgency": set([16]),
-                "languageDeclaration": set([21]),
-                "languageUsed": set([188, 195]),
-                "localControl": set([54]),
-                "source": set([76]),  # empty.
-                "structureOrGenealogy": set([268]),  # empty.
-                "biogHist": set([328, 331]),  # empty.
-            },
-        )
+            not_visited.setdefault(tagname, set()).add(sourceline)
+
+        assert not_visited == {
+            "maintenanceStatus": {12},
+            "publicationStatus": {14},
+            "recordId": {8},
+            "maintenanceAgency": {16},
+            "languageDeclaration": {21},
+            "languageUsed": {188, 195},
+            "localControl": {54},
+            "source": {76},  # empty.
+            "structureOrGenealogy": {268},  # empty.
+            "biogHist": {328, 331},  # empty.
+        }
 
     def check_order_entities(self, entities, expected):
         """Usefull test for comparing sorted lists of actual and
         expected entities. Make it easier to check where to add a
         new entity or swap 2 of them.
         """
 
@@ -1081,15 +1003,15 @@
             return sorted(
                 ((e.etype, e.extid) for e in elems if e.etype != "ExternalUri"),
                 key=lambda e: e[1],
             )
 
         a_lst = get_sorted(entities)
         e_lst = get_sorted(expected)
-        self.assertEquals(a_lst, e_lst)
+        assert a_lst == e_lst
 
     def test_values_from_functions(self):
         fname = "FRAD033_EAC_00001_simplified.xml"
         fpath = self.datapath(fname)
         self.root = etree.fromstring(XML_TEST)
         import_log = SimpleImportLog(fpath)
         importer = dataimport.EACCPFImporter(fpath, import_log)
@@ -1102,28 +1024,28 @@
                 ("body_value", "body"),
                 ("empty_value", "empty"),
             ),
         )
         self.assertEqual(
             values,
             {
-                "to_value": set(["Tove"]),
-                "from_value": set(["Jani"]),
-                "heading_value": set(["Reminder"]),
-                "body_value": set(["Hey!"]),
+                "to_value": {"Tove"},
+                "from_value": {"Jani"},
+                "heading_value": {"Reminder"},
+                "body_value": {"Hey!"},
             },
         )
         attrib = importer.values_from_attrib(
             self.root, (("test_varname", "test"), ("test_varname_2", "test2"))
         )
         self.assertEqual(
             attrib,
             {
-                "test_varname": set(["test_value"]),
-                "test_varname_2": set(["test2_value"]),
+                "test_varname": {"test_value"},
+                "test_varname_2": {"test2_value"},
             },
         )
 
     def test_mandate_under_mandates(self):
         """In FRAD033_EAC_00003.xml, <mandate> element are within <mandates>."""
         entities = list(self.file_extentities("FRAD033_EAC_00003.xml"))
         expected_terms = [
@@ -1152,15 +1074,15 @@
         extid = next(iter(mandate_with_link.values["has_citation"]))
         url = (
             "http://www.legifrance.gouv.fr/affichCode.do?idArticle=LEGIARTI000019202816"
         )
         citation = next(
             x for x in entities if x.etype == "Citation" and url in x.values["uri"]
         )
-        self.assertEqual(extid, citation.extid)
+        assert extid == citation.extid
 
     def test_agentfunction_within_functions_tag(self):
         """In FRAD033_EAC_00003.xml, <function> element are within <functions>
         not <description>.
         """
         entities = self.file_extentities("FRAD033_EAC_00003.xml")
         self.assertCountEqual(
@@ -1191,48 +1113,14 @@
             getattr(self, method)(actual, expected, msg=msg)
         except AssertionError as exc:
             msg = str(exc)
             if ctx:
                 msg = ("[%s] " % ctx) + msg
             raise AssertionError(msg)
 
-    def check_external_entities(self, entities, expected):
-        entities = extentities2dict(entities)
-        expected = extentities2dict(expected)
-        etypes, expected_etypes = list(entities), list(expected)
-        self.ctx_assert("assertCountEqual", etypes, expected_etypes, ctx="etypes")
-
-        def safe_int(value):
-            try:
-                return int(value)
-            except ValueError:
-                return 9999
-
-        ordered_etypes = [
-            x[1]
-            for x in sorted(
-                (min(safe_int(extid) for extid in edict), etype)
-                for etype, edict in expected.items()
-            )
-        ]
-        for etype in ordered_etypes:
-            edict = expected[etype]
-            entities_etype = entities[etype]
-            extids, expected_extids = list(entities_etype), list(edict)
-            self.ctx_assert(
-                "assertCountEqual", extids, expected_extids, ctx="%s/extids" % etype
-            )
-            for extid, values in edict.items():
-                self.ctx_assert(
-                    "assertEqual",
-                    tolist(entities_etype[extid]),
-                    tolist(values),
-                    ctx="%s/%s/values" % (etype, extid),
-                )
-
     def test_errors(self):
         log = SimpleImportLog("<dummy>")
         with self.assertRaises(dataimport.InvalidXML):
             importer = dataimport.EACCPFImporter(BytesIO(b"no xml"), log, mock_)
             list(importer.external_entities())
         with self.assertRaises(dataimport.MissingTag):
             importer = dataimport.EACCPFImporter(BytesIO(b"<xml/>"), log, mock_)
@@ -1248,29 +1136,29 @@
             scheme = cnx.create_entity("ConceptScheme")
             scheme.add_concept(
                 "environnement",
                 cwuri="http://data.culture.fr/thesaurus/page/ark:/67717/T1-1074",
             )
             cnx.commit()
             created, updated = testutils.eac_import(cnx, fpath)
-            self.assertEqual(len(created), 80)
-            self.assertEqual(updated, set())
+            assert len(created) == 80
+            assert updated == set()
             rset = cnx.find("AuthorityRecord", isni="22330001300016")
-            self.assertEqual(len(rset), 1)
+            assert len(rset) == 1
             record = rset.one()
-            self.assertEqual(record.kind, "authority")
-            self.assertEqual(record.start_date, datetime.date(1800, 1, 1))
-            self.assertEqual(record.end_date, datetime.date(2099, 1, 1))
+            assert record.kind == "authority"
+            assert record.start_date, datetime.date(1800, 1 == 1)
+            assert record.end_date, datetime.date(2099, 1 == 1)
             self.assertEqual(
                 record.other_record_ids, [(None, "1234"), ("letters", "ABCD")]
             )
             address = record.postal_address[0]
-            self.assertEqual(address.street, "1 Esplanade Charles de Gaulle")
-            self.assertEqual(address.postalcode, "33074")
-            self.assertEqual(address.city, " Bordeaux Cedex")
+            assert address.street == "1 Esplanade Charles de Gaulle"
+            assert address.postalcode == "33074"
+            assert address.city == " Bordeaux Cedex"
             self.assertEqual(
                 address.raw_address,
                 "1 Esplanade Charles de Gaulle\n33074\n Bordeaux Cedex",
             )
             rset = cnx.execute(
                 """
                  Any R,N WHERE P place_agent A, A eid %(eid)s,
@@ -1281,15 +1169,15 @@
                 rset.rows,
                 [
                     ["siege", "Bordeaux (Gironde, France)"],
                     ["domicile", "Toulouse (France)"],
                     ["dodo", "Lit"],
                 ],
             )
-            self.assertEqual(len(record.reverse_function_agent), 3)
+            assert len(record.reverse_function_agent) == 3
             for related in (
                 "structure",
                 "history",
                 "mandate",
                 "occupation",
                 "generalcontext",
                 "legal_status",
@@ -1301,72 +1189,72 @@
             ):
                 with self.subTest(related=related):
                     checker = getattr(self, "_check_" + related)
                     checker(cnx, record)
 
     def _check_structure(self, cnx, record):
         rset = cnx.find("Structure", structure_agent=record)
-        self.assertEqual(len(rset), 1)
+        assert len(rset) == 1
         self.assertEqual(
             rset.one().printable_value("description", format="text/plain").strip(),
             "Pour accomplir ses missions ...",
         )
 
     def _check_convention(self, cnx, record):
         rset = cnx.find("Convention", convention_of=record).sorted_rset(lambda x: x.eid)
-        self.assertEqual(len(rset), 3)
+        assert len(rset) == 3
         self.assertEqual(
             rset.get_entity(0, 0)
             .printable_value("description", format="text/plain")
             .strip(),
             "Norme ISAAR(CPF) du Conseil international des archives, "
             "2e \xe9dition, 1996.",
         )
 
     def _check_history(self, cnx, record):
         rset = cnx.find("History", history_agent=record)
-        self.assertEqual(len(rset), 1)
+        assert len(rset) == 1
         entity = rset.one()
         self.assertEqual(
             entity.printable_value("abstract", format="text/plain").strip(),
             "Test of an abstract element",
         )
         self.assertEqual(
             entity.printable_value("text", format="text/plain").strip(),
             "La loi du 22 décembre 1789, en divisant ...\n\nL'inspecteur Canardo",
         )
         events = rset.one().has_event
-        self.assertEqual(len(events), 2)
+        assert len(events) == 2
 
     def _check_mandate(self, cnx, record):
         rset = cnx.find("Mandate", mandate_agent=record)
-        self.assertEqual(len(rset), 1)
+        assert len(rset) == 1
         self.assertEqual(
             rset.one().printable_value("description", format="text/plain").strip(),
             "Description du mandat",
         )
 
     def _check_occupation(self, cnx, record):
         occupation = cnx.find("Occupation", occupation_agent=record).one()
-        self.assertEqual(occupation.term, "Réunioniste")
+        assert occupation.term == "Réunioniste"
         citation = occupation.has_citation[0]
-        self.assertEqual(citation.note, "la bible")
+        assert citation.note == "la bible"
         voc = occupation.equivalent_concept[0]
-        self.assertEqual(voc.uri, "http://pifgadget.com")
+        assert voc.uri == "http://pifgadget.com"
 
     def _check_generalcontext(self, cnx, record):
         occupation = cnx.find("GeneralContext", general_context_of=record).one()
         self.assertIn("very famous", occupation.content)
-        self.assertEqual(occupation.content_format, "text/html")
+        assert occupation.content_format == "text/html"
         citation = occupation.has_citation[0]
-        self.assertEqual(citation.note, "it's well known")
+        assert citation.note == "it's well known"
 
     def _check_legal_status(self, cnx, record):
         rset = cnx.find("LegalStatus", legal_status_agent=record)
-        self.assertEqual(len(rset), 1)
+        assert len(rset) == 1
         self.assertEqual(
             rset.one().printable_value("description", format="text/plain").strip(),
             "Description du statut",
         )
 
     def _check_eac_relations(self, cnx, record):
         relation = cnx.find("HierarchicalRelation").one()
@@ -1375,26 +1263,26 @@
             "Gironde. Conseil général. Direction de "
             "l'administration et de la sécurité juridique",
         )
         self.assertEqual(
             relation.printable_value("description", format="text/plain"), "Coucou"
         )
         other_record = cnx.find("ExternalUri", uri="CG33-DIRADSJ").one()
-        self.assertEqual(relation.hierarchical_parent[0], other_record)
+        assert relation.hierarchical_parent[0] == other_record
         relation = cnx.find("AssociationRelation").one()
-        self.assertEqual(relation.association_from[0], record)
+        assert relation.association_from[0] == record
         other_record = cnx.find("ExternalUri", uri="agent-x").one()
-        self.assertEqual(other_record.cwuri, "agent-x")
-        self.assertEqual(relation.association_to[0], other_record)
+        assert other_record.cwuri == "agent-x"
+        assert relation.association_to[0] == other_record
         rset = cnx.find("EACResourceRelation", agent_role="creatorOf")
-        self.assertEqual(len(rset), 1)
+        assert len(rset) == 1
         rrelation = rset.one()
-        self.assertEqual(rrelation.resource_relation_agent[0], record)
+        assert rrelation.resource_relation_agent[0] == record
         exturi = rrelation.resource_relation_resource[0]
-        self.assertEqual(exturi.uri, "http://gael.gironde.fr/ead.html?id=FRAD033_IR_N")
+        assert exturi.uri == "http://gael.gironde.fr/ead.html?id=FRAD033_IR_N"
         self.assertEqual(
             rrelation.xml_wrap.getvalue().decode(),
             '<he xmlns="urn:isbn:1-931666-33-4" xmlns:xlink="http'
             '://www.w3.org/1999/xlink" xmlns:xsi="http://www.w3.org'
             '/2001/XMLSchema-instance">joe</he>',
         )
         self.assertEqual(
@@ -1429,42 +1317,42 @@
             " le due\n\t      guerre\n\t      </title>\n\t    </titleInfo>\n"
             '\t    <name>\n\t      <namePart type="given">Nicoletta\n\t'
             '      </namePart>\n\t      <namePart type="family">Boschiero\n'
             '\t      </namePart>\n\t      <role>\n\t\t<roleTerm type="text'
             '">autore\n\t\t</roleTerm>\n\t      </role>\n\t    </name>\n\t'
             "  </mods>\n\t",
         )
-        self.assertEqual(func_relation.function_relation_agent[0], record)
+        assert func_relation.function_relation_agent[0] == record
         self.assertEqual(
             func_relation.function_relation_function[0].uri,
             "http://gael.gironde.fr/ead.html?id=FRAD033_IR_N",
         )
         rset = cnx.find("EACFunctionRelation", r_type="controls")
         func_relation = rset.one()
-        self.assertEqual(func_relation.function_relation_agent[0], record)
+        assert func_relation.function_relation_agent[0] == record
         self.assertEqual(
             func_relation.function_relation_function[0].uri, "FRAD033_IR_N"
         )
 
     def _check_parallel_relations(self, cnx, record):
         rset = cnx.find("ParallelNames", parallel_names_of=record).sorted_rset(
             lambda x: x.eid
         )
-        self.assertEqual(len(rset), 2)
+        assert len(rset) == 2
         p_entity = rset.get_entity(0, 0)
-        self.assertEqual(p_entity.parallel_names_of[0], record)
-        self.assertEqual(len(p_entity.simple_name_relation), 2)
-        self.assertEqual(len(p_entity.date_relation), 0)
+        assert p_entity.parallel_names_of[0] == record
+        assert len(p_entity.simple_name_relation) == 2
+        assert len(p_entity.date_relation) == 0
         p_entity = rset.get_entity(1, 0)
-        self.assertEqual(p_entity.parallel_names_of[0], record)
-        self.assertEqual(len(p_entity.simple_name_relation), 3)
-        self.assertEqual(len(p_entity.date_relation), 3)
+        assert p_entity.parallel_names_of[0] == record
+        assert len(p_entity.simple_name_relation) == 3
+        assert len(p_entity.date_relation) == 3
 
     def _check_equivalent_concept(self, cnx, record):
-        functions = dict((f.name, f) for f in record.reverse_function_agent)
+        functions = {f.name: f for f in record.reverse_function_agent}
         self.assertEqual(
             functions["action sociale"].equivalent_concept[0].cwuri,
             "http://data.culture.fr/thesaurus/page/ark:/67717/T1-200",
         )
         self.assertEqual(
             functions["action sociale"].equivalent_concept[0].cw_etype, "ExternalUri"
         )
@@ -1483,19 +1371,19 @@
         self.assertEqual(
             place.equivalent_concept[0].cwuri,
             "http://catalogue.bnf.fr/ark:/12148/cb152418385",
         )
 
     def _check_control(self, cnx, record):
         rset = cnx.find("EACSource")
-        self.assertEqual(len(rset), 2)
+        assert len(rset) == 2
         rset = cnx.execute("Any A WHERE A generated X, X eid %(x)s", {"x": record.eid})
-        self.assertEqual(len(rset), 2)
+        assert len(rset) == 2
         rset = cnx.execute('Any A WHERE A agent "Delphine Jamet"')
-        self.assertEqual(len(rset), 1)
+        assert len(rset) == 1
 
     def test_multiple_imports(self):
         def count_entity(cnx, etype):
             return cnx.execute("Any COUNT(X) WHERE X is %s" % etype)[0][0]
 
         with self.admin_access.repo_cnx() as cnx:
             nb_records_before = count_entity(cnx, "AuthorityRecord")
@@ -1503,15 +1391,15 @@
                 "FRAD033_EAC_00001.xml",
                 "FRAD033_EAC_00003.xml",
                 "FRAD033_EAC_00071.xml",
             ):
                 fpath = self.datapath(fname)
                 created, updated = testutils.eac_import(cnx, fpath)
             nb_records_after = count_entity(cnx, "AuthorityRecord")
-            self.assertEqual(nb_records_after - nb_records_before, 3)
+            assert nb_records_after - nb_records_before == 3
 
     def test_unknown_kind(self):
         with self.admin_access.repo_cnx() as cnx:
             testutils.eac_import(cnx, self.datapath("custom_kind.xml"))
             self.assertRaises(
                 NoResultError, cnx.find("AgentKind", name="a custom kind").one
             )
@@ -1520,20 +1408,20 @@
                 "unknown-agent-kind",
             )
 
     def test_no_name_entry(self):
         with self.admin_access.repo_cnx() as cnx:
             with self.assertRaises(dataimport.MissingTag) as cm:
                 testutils.eac_import(cnx, self.datapath("no_name_entry.xml"))
-            self.assertEqual(cm.exception.tag, "nameEntry")
-            self.assertEqual(cm.exception.tag_parent, "identity")
+            assert cm.exception.tag == "nameEntry"
+            assert cm.exception.tag_parent == "identity"
 
     def test_no_name_entry_part(self):
         with self.admin_access.repo_cnx() as cnx:
             with self.assertRaises(dataimport.MissingTag) as cm:
                 testutils.eac_import(cnx, self.datapath("no_name_entry_part.xml"))
-            self.assertEqual(cm.exception.tag, "part")
-            self.assertEqual(cm.exception.tag_parent, "nameEntry")
+            assert cm.exception.tag == "part"
+            assert cm.exception.tag_parent == "nameEntry"
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `cubicweb-eac-1.5.3/test/test_entities.py` & `cubicweb-eac-2.0.0/test/test_entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding: utf-8
 # copyright 2016-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -39,18 +38,18 @@
                 mandate_agent=alice,
             )
             cnx.commit()
             serializer = alice.cw_adapt_to("EAC-CPF")
             line1, line2 = serializer._eac_richstring_paragraph_elements(
                 mandate, "description"
             )
-        self.assertEqual(line1.tag, "p")
-        self.assertEqual(line1.text, "ding")
-        self.assertEqual(line2.tag, "p")
-        self.assertEqual(line2.text, "likes rabbits")
+        assert line1.tag == "p"
+        assert line1.text == "ding"
+        assert line2.tag == "p"
+        assert line2.text == "likes rabbits"
 
     def test_richstring_html_simple(self):
         with self.admin_access.cnx() as cnx:
             alice = testutils.authority_record(cnx, "T-01", "Alice")
             desc = "<span>ding</span>"
             mandate = cnx.create_entity(
                 "Mandate",
@@ -60,15 +59,15 @@
                 mandate_agent=alice,
             )
             cnx.commit()
             serializer = alice.cw_adapt_to("EAC-CPF")
             (tag,) = serializer._eac_richstring_paragraph_elements(
                 mandate, "description"
             )
-        self.assertEqual(tag.tag, "span")
+        assert tag.tag == "span"
         self.assertIn(desc, etree.tostring(tag, encoding="unicode"))
 
     def test_richstring_html_multiple_elements(self):
         with self.admin_access.cnx() as cnx:
             alice = testutils.authority_record(cnx, "T-01", "Alice")
             desc = ["<h1>she <i>rules!</i></h1>", '<a href="1">pif</a>']
             mandate = cnx.create_entity(
@@ -79,16 +78,16 @@
                 mandate_agent=alice,
             )
             cnx.commit()
             serializer = alice.cw_adapt_to("EAC-CPF")
             h1, a = serializer._eac_richstring_paragraph_elements(
                 mandate, "description"
             )
-        self.assertEqual(h1.tag, "h1")
-        self.assertEqual(a.tag, "a")
+        assert h1.tag == "h1"
+        assert a.tag == "a"
         self.assertIn(etree.tostring(h1, encoding="unicode"), desc[0])
         self.assertIn(etree.tostring(a, encoding="unicode"), desc[1])
 
     def test_richstring_markdown(self):
         with self.admin_access.cnx() as cnx:
             alice = testutils.authority_record(cnx, "T-01", "Alice")
             desc = "[pif](http://gadget.com) is *red*"
@@ -101,15 +100,15 @@
                 mandate_agent=alice,
             )
             cnx.commit()
             serializer = alice.cw_adapt_to("EAC-CPF")
             (tag,) = serializer._eac_richstring_paragraph_elements(
                 mandate, "description"
             )
-        self.assertEqual(tag.tag, "p")
+        assert tag.tag == "p"
         self.assertIn(desc_html, etree.tostring(tag, encoding="unicode"))
 
     def test_richstring_rest(self):
         with self.admin_access.cnx() as cnx:
             alice = testutils.authority_record(cnx, "T-01", "Alice")
             desc = "`pif <http://gadget.com>`_ is *red*"
             desc_html = (
@@ -124,22 +123,22 @@
                 mandate_agent=alice,
             )
             cnx.commit()
             serializer = alice.cw_adapt_to("EAC-CPF")
             (ptag,) = serializer._eac_richstring_paragraph_elements(
                 mandate, "description"
             )
-        self.assertEqual(ptag.tag, "p")
+        assert ptag.tag == "p"
         self.assertIn(desc_html, etree.tostring(ptag, encoding="unicode"))
 
     def test_richstring_empty(self):
         def check(authority_record):
             serializer = authority_record.cw_adapt_to("EAC-CPF")
             res = serializer._eac_richstring_paragraph_elements(mandate, "description")
-            self.assertEqual(res, [])
+            assert res == []
 
         with self.admin_access.cnx() as cnx:
             alice = testutils.authority_record(cnx, "T-01", "Alice")
             mandate = cnx.create_entity(
                 "Mandate", term="w", description=None, mandate_agent=alice
             )
             cnx.commit()
@@ -161,14 +160,14 @@
                 description=" ",
                 description_format="text/markdown",
                 mandate_agent=arecord,
             )
             cnx.commit()
             serializer = arecord.cw_adapt_to("EAC-CPF")
             element = serializer.mandate_element(mandate)
-            self.assertEqual(["term"], [child.tag for child in element])
+            assert ["term"] == [child.tag for child in element]
 
 
 if __name__ == "__main__":
     import unittest
 
     unittest.main()
```

### Comparing `cubicweb-eac-1.5.3/test/test_export.py` & `cubicweb-eac-2.0.0/test/test_export.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 FLAGS = doctest.REPORT_UDIFF
 
 
 class EACExportFunctionalTests(CubicWebTC, testutils.XmlTestMixin):
     """Functional tests for EAC-CPF export."""
 
     def setUp(self):
-        super(EACExportFunctionalTests, self).setUp()
+        super().setUp()
         self.globs = globals().copy()
         self.globs["self"] = self
 
     def _test(self, filename):
         with self.admin_access.cnx() as cnx:
             self.globs["cnx"] = cnx
             failure_count, test_count = doctest.testfile(
```

### Comparing `cubicweb-eac-1.5.3/test/test_hooks.py` & `cubicweb-eac-2.0.0/test/test_hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/test/test_rdf.py` & `cubicweb-eac-2.0.0/test/test_rdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -101,41 +101,53 @@
                 family_from=person,
                 family_to=fam1,
                 entry="Famille Poulet",
             )
             cnx.commit()
 
     def compare_graphs(self, graph, eid_dict, target_ttl_file_name):
-        with open(self.datapath(target_ttl_file_name), "r") as f:
+        with open(self.datapath(target_ttl_file_name)) as f:
             data = f.read()
             data = data.replace("{{BASE_URL}}", BASE_URL)
             for key, value in eid_dict.items():
                 data = data.replace("{{%s}}" % key, str(value))
 
+            print("Formatting data:\n================\n")
+            print(eid_dict)
             target_graph = Graph().parse(data=data, format="ttl")
+            print(
+                "Graph generated by the test code:\n=================================\n"
+            )
             print(graph.serialize(format="ttl"))
             common, tested_only, target_only = graph_diff(graph, target_graph)
+            print("*Diffing graphs...*\n")
+            print("Expected graph:\n===============\n")
             print(target_only.serialize(format="ttl"))
+            print("Graph from test code:\n=====================\n")
             print(tested_only.serialize(format="ttl"))
-            self.assertEqual(len(tested_only), 0)
-            self.assertEqual(len(target_only), 0)
+
+            # check that the diffs are empty
+            assert len(tested_only) == 0
+            assert len(target_only) == 0
 
     def test_person_authority_schemaorg(self):
         with self.admin_access.repo_cnx() as cnx:
             entity = cnx.find("AuthorityRecord", record_id="A123").one()
             graph = ConjunctiveGraph()
             add_entity_to_graph(graph, entity, "rdf.schemaorg")
-            self.compare_graphs(graph, {"eid": entity.eid}, "person_rdf.ttl")
+            self.compare_graphs(graph, {"uri": entity.absolute_url()}, "person_rdf.ttl")
 
     def test_organization_authority_schemaorg(self):
         with self.admin_access.repo_cnx() as cnx:
             entity = cnx.find("AuthorityRecord", record_id="C123").one()
             graph = ConjunctiveGraph()
             add_entity_to_graph(graph, entity, "rdf.schemaorg")
-            self.compare_graphs(graph, {"eid": entity.eid}, "organization_rdf.ttl")
+            self.compare_graphs(
+                graph, {"uri": entity.absolute_url()}, "organization_rdf.ttl"
+            )
 
     def test_family_rico(self):
         with self.admin_access.repo_cnx() as cnx:
             rset = cnx.execute(
                 "Any X, N, A WHERE X is AuthorityRecord, X record_id %(id)s,"
                 "R is FamilyRelation, R family_from X,"
                 "R family_to A, A agent_kind K, K name 'person',"
@@ -154,17 +166,21 @@
             family_eid = rset[0][0]
             graph = ConjunctiveGraph()
             add_entity_to_graph(graph, record, "rdf.rico")
             self.compare_graphs(
                 graph,
                 {
                     "eid": record.eid,
+                    "uri": record.absolute_url(),
                     "p_eid": agent_person,
+                    "p_uri": cnx.entity_from_eid(agent_person).absolute_url(),
                     "name_eid": name,
+                    "name_uri": cnx.entity_from_eid(name).absolute_url(),
                     "ar_eid": family_eid,
+                    "ar_uri": cnx.entity_from_eid(family_eid).absolute_url(),
                 },
                 "family_rico.ttl",
             )
 
     def test_person_rico(self):
         with self.admin_access.repo_cnx() as cnx:
             rset = cnx.execute(
@@ -195,22 +211,31 @@
 
             graph = ConjunctiveGraph()
             add_entity_to_graph(graph, record, "rdf.rico")
             self.compare_graphs(
                 graph,
                 {
                     "eid": eid,
+                    "uri": record.absolute_url(),
                     "occupation": occupation,
+                    "occupation_uri": cnx.entity_from_eid(occupation).absolute_url(),
                     "name": name,
+                    "name_uri": cnx.entity_from_eid(name).absolute_url(),
                     "fam1": fam1,
+                    "fam1_uri": cnx.entity_from_eid(fam1).absolute_url(),
                     "fam2": fam2,
+                    "fam2_uri": cnx.entity_from_eid(fam2).absolute_url(),
                     "famrel1": famrel1,
+                    "famrel1_uri": cnx.entity_from_eid(famrel1).absolute_url(),
                     "famrel2": famrel2,
+                    "famrel2_uri": cnx.entity_from_eid(famrel2).absolute_url(),
                     "familyrel": rel_family,
+                    "familyrel_uri": cnx.entity_from_eid(rel_family).absolute_url(),
                     "family": family_eid,
+                    "family_uri": cnx.entity_from_eid(family_eid).absolute_url(),
                 },
                 "person_rico.ttl",
             )
 
     def test_organization_rico(self):
         with self.admin_access.repo_cnx() as cnx:
             rset = cnx.execute(
@@ -239,19 +264,29 @@
 
             graph = ConjunctiveGraph()
             add_entity_to_graph(graph, record, "rdf.rico")
             self.compare_graphs(
                 graph,
                 {
                     "eid": eid,
+                    "uri": record.absolute_url(),
                     "name": name,
+                    "name_uri": cnx.entity_from_eid(name).absolute_url(),
                     "parent_of": parent_of,
+                    "parent_of_uri": cnx.entity_from_eid(parent_of).absolute_url(),
                     "parent_of_rel": parent_of_rel,
+                    "parent_of_rel_uri": cnx.entity_from_eid(
+                        parent_of_rel
+                    ).absolute_url(),
                     "child_of": child_of,
+                    "child_of_uri": cnx.entity_from_eid(child_of).absolute_url(),
                     "child_of_rel": child_of_rel,
+                    "child_of_rel_uri": cnx.entity_from_eid(
+                        child_of_rel
+                    ).absolute_url(),
                 },
                 "organization_rico.ttl",
             )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `cubicweb-eac-1.5.3/test/test_schema.py` & `cubicweb-eac-2.0.0/test/test_schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -104,114 +104,103 @@
             self.assertIn("must be less than", str(cm.exception))
 
 
 class AuthorityRecordGraphTC(CubicWebTC):
     def test_graph_structure(self):
         graph = AuthorityRecordGraph(self.schema)
         expected = {
-            "AgentFunction": {("function_agent", "subject"): set(["AuthorityRecord"])},
-            "AgentPlace": {("place_agent", "subject"): set(["AuthorityRecord"])},
+            "AgentFunction": {("function_agent", "subject"): {"AuthorityRecord"}},
+            "AgentPlace": {("place_agent", "subject"): {"AuthorityRecord"}},
             "Citation": {
-                ("has_citation", "object"): set(
-                    [
-                        "GeneralContext",
-                        "Mandate",
-                        "Occupation",
-                        "AgentFunction",
-                        "AgentPlace",
-                        "History",
-                        "LegalStatus",
-                        "Convention",
-                        "Structure",
-                    ]
-                )
+                ("has_citation", "object"): {
+                    "GeneralContext",
+                    "Mandate",
+                    "Occupation",
+                    "AgentFunction",
+                    "AgentPlace",
+                    "History",
+                    "LegalStatus",
+                    "Convention",
+                    "Structure",
+                }
             },
             "DateEntity": {
-                ("date_relation", "object"): set(
-                    [
-                        "HistoricalEvent",
-                        "AgentFunction",
-                        "EACFunctionRelation",
-                        "LegalStatus",
-                        "Mandate",
-                        "NameEntry",
-                        "Occupation",
-                        "AgentPlace",
-                        "EACResourceRelation",
-                        "ParallelNames",
-                    ]
-                )
+                ("date_relation", "object"): {
+                    "HistoricalEvent",
+                    "AgentFunction",
+                    "EACFunctionRelation",
+                    "LegalStatus",
+                    "Mandate",
+                    "NameEntry",
+                    "Occupation",
+                    "AgentPlace",
+                    "EACResourceRelation",
+                    "ParallelNames",
+                }
             },
             "PlaceEntry": {
-                ("place_entry_relation", "object"): set(
-                    [
-                        "HistoricalEvent",
-                        "AgentFunction",
-                        "EACFunctionRelation",
-                        "LegalStatus",
-                        "Mandate",
-                        "Occupation",
-                        "AgentPlace",
-                        "EACResourceRelation",
-                    ]
-                )
+                ("place_entry_relation", "object"): {
+                    "HistoricalEvent",
+                    "AgentFunction",
+                    "EACFunctionRelation",
+                    "LegalStatus",
+                    "Mandate",
+                    "Occupation",
+                    "AgentPlace",
+                    "EACResourceRelation",
+                }
             },
             "EACFunctionRelation": {
-                ("function_relation_agent", "subject"): set(["AuthorityRecord"])
+                ("function_relation_agent", "subject"): {"AuthorityRecord"}
             },
             "EACOtherRecordId": {
-                ("eac_other_record_id_of", "subject"): set(["AuthorityRecord"])
+                ("eac_other_record_id_of", "subject"): {"AuthorityRecord"}
             },
             "EACResourceRelation": {
-                ("resource_relation_agent", "subject"): set(["AuthorityRecord"])
+                ("resource_relation_agent", "subject"): {"AuthorityRecord"}
             },
-            "Convention": {("convention_of", "subject"): set(["AuthorityRecord"])},
-            "EACSource": {("source_agent", "subject"): set(["AuthorityRecord"])},
-            "HistoricalEvent": {("has_event", "object"): set(["History"])},
-            "GeneralContext": {
-                ("general_context_of", "subject"): set(["AuthorityRecord"])
-            },
-            "History": {("history_agent", "subject"): set(["AuthorityRecord"])},
-            "LegalStatus": {
-                ("legal_status_agent", "subject"): set(["AuthorityRecord"])
-            },
-            "Mandate": {("mandate_agent", "subject"): set(["AuthorityRecord"])},
+            "Convention": {("convention_of", "subject"): {"AuthorityRecord"}},
+            "EACSource": {("source_agent", "subject"): {"AuthorityRecord"}},
+            "HistoricalEvent": {("has_event", "object"): {"History"}},
+            "GeneralContext": {("general_context_of", "subject"): {"AuthorityRecord"}},
+            "History": {("history_agent", "subject"): {"AuthorityRecord"}},
+            "LegalStatus": {("legal_status_agent", "subject"): {"AuthorityRecord"}},
+            "Mandate": {("mandate_agent", "subject"): {"AuthorityRecord"}},
             "NameEntry": {
-                ("name_entry_for", "subject"): set(["AuthorityRecord"]),
-                ("simple_name_relation", "object"): set(["ParallelNames"]),
-            },
-            "Occupation": {("occupation_agent", "subject"): set(["AuthorityRecord"])},
-            "ParallelNames": {
-                ("parallel_names_of", "subject"): set(["AuthorityRecord"])
+                ("name_entry_for", "subject"): {"AuthorityRecord"},
+                ("simple_name_relation", "object"): {"ParallelNames"},
             },
-            "PostalAddress": {("place_address", "object"): set(["AgentPlace"])},
-            "Structure": {("structure_agent", "subject"): set(["AuthorityRecord"])},
+            "Occupation": {("occupation_agent", "subject"): {"AuthorityRecord"}},
+            "ParallelNames": {("parallel_names_of", "subject"): {"AuthorityRecord"}},
+            "PostalAddress": {("place_address", "object"): {"AgentPlace"}},
+            "Structure": {("structure_agent", "subject"): {"AuthorityRecord"}},
         }
-        struct = dict(
-            (k, dict((rel, set(targets)) for rel, targets in v.items()))
+        struct = {
+            k: {rel: set(targets) for rel, targets in v.items()}
             for k, v in graph.parent_structure("AuthorityRecord").items()
-        )
-        self.assertEqual(struct, expected)
+        }
+        assert struct == expected
 
     def test_optional_relations(self):
         graph = AuthorityRecordGraph(self.schema)
         structure = graph.parent_structure("AuthorityRecord")
         opts = optional_relations(self.schema, structure)
         expected = {
-            "NameEntry": set(
-                [("name_entry_for", "subject"), ("simple_name_relation", "object")]
-            )
+            "NameEntry": {
+                ("name_entry_for", "subject"),
+                ("simple_name_relation", "object"),
+            }
         }
-        self.assertEqual(opts, expected)
+        assert opts == expected
 
     def test_relations_consistency(self):
         graph = AuthorityRecordGraph(self.schema)
         structure = graph.parent_structure("AuthorityRecord")
         structurals, optionals, mandatories = graph_relations(self.schema, structure)
-        self.assertEqual(structurals - optionals, mandatories)
+        assert structurals - optionals == mandatories
 
 
 class SecurityTC(CubicWebTC):
     """Test case for permissions set in the schema"""
 
     @contextmanager
     def assertUnauthorized(self, cnx):
```

### Comparing `cubicweb-eac-1.5.3/test/test_views.py` & `cubicweb-eac-2.0.0/test/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 """cubicweb-eac test for views."""
 
 import unittest
 
 from cubicweb import Binary
 from cubicweb.devtools.testlib import CubicWebTC
-from cubicweb.web.views.actions import CopyAction
+from cubicweb_web.views.actions import CopyAction
 
 from cubicweb_eac import testutils
 
 
 class FuncViewsTC(CubicWebTC):
     def test_import_ok(self):
         regid = "eac.import"
@@ -51,15 +51,15 @@
             fields = {"file": (fname, open(self.datapath(fname), "rb"))}
             req.form = self.fake_form(regid, fields)
             # now actually test the import
             html = req.view(regid)
             self.assertIn("EAC import failed", html)
             # Still only one AuthorityRecord.
             rset = req.find("AuthorityRecord")
-            self.assertEqual(len(rset), 1)
+            assert len(rset) == 1
 
     def test_import_invalid_xml(self):
         regid = "eac.import"
         fname = "invalid_xml.xml"
         with self.admin_access.web_request() as req:
             fields = {"file": (fname, open(self.datapath(fname), "rb"))}
             req.form = self.fake_form(regid, fields)
@@ -78,23 +78,23 @@
             self.assertIn("Missing tag cpfDescription in XML file", html)
 
     def test_export_filename(self):
         with self.admin_access.web_request() as req:
             cnx = req.cnx
             record = testutils.authority_record(cnx, "T-07", "jim")
             for isni, expected_filename in (
-                ("", "EAC_{0}.xml".format(record.eid)),
+                ("", f"EAC_{record.eid}.xml"),
                 ("ZZZ/4242", "EAC_ZZZ_4242.xml"),
             ):
                 record.cw_set(isni=isni)
                 view = self.vreg["views"].select("eac.export", req, record.as_rset())
                 view.set_request_content_type()
                 self.assertEqual(
                     view._cw.headers_out.getRawHeaders("content-disposition"),
-                    ['attachment;filename="{0}"'.format(expected_filename)],
+                    [f'attachment;filename="{expected_filename}"'],
                 )
 
     def test_xmlwrap_component(self):
         with self.admin_access.cnx() as cnx:
             bob = testutils.authority_record(cnx, "T-02", "bob")
             uri = cnx.create_entity("ExternalUri", uri="http://logilab.fr")
             cnx.create_entity(
@@ -108,15 +108,15 @@
             rset = req.find("EACResourceRelation")
             component = self.vreg["ctxcomponents"].select(
                 "eac.xml_wrap", req, rset=rset
             )
             content = []
             component.render_body(content.append)
         self.assertIn("plop", content[0])
-        self.assertEqual(content[0].count("plip"), 2)
+        assert content[0].count("plip") == 2
 
 
 class AuthorityRecordFormsTC(CubicWebTC):
     def test_no_copy_action(self):
         with self.admin_access.cnx() as cnx:
             testutils.authority_record(cnx, "T-06", "toto")
             cnx.commit()
@@ -138,15 +138,15 @@
             cls = self.vreg["etypes"].etype_class("HierarchicalRelation")(req)
             form = self.vreg["forms"].select("edition", req, entity=cls)
             field = form.field_by_name("hierarchical_parent", "subject")
             choices = unrelated_authorityrecord("hierarchical_parent", form, field)
             expected = [("1", str(ar1)), ("2", str(ar2))]
             self.assertCountEqual(choices, expected)
         # Now with a __linkto.
-        linkto = "hierarchical_parent:{0}:subject".format(ar2)
+        linkto = f"hierarchical_parent:{ar2}:subject"
         with self.admin_access.web_request(__linkto=linkto) as req:
             cls = self.vreg["etypes"].etype_class("HierarchicalRelation")(req)
             form = self.vreg["forms"].select("edition", req, entity=cls)
             field = form.field_by_name("hierarchical_parent", "subject")
             choices = unrelated_authorityrecord("hierarchical_parent", form, field)
             expected = [("2", str(ar2))]
             self.assertCountEqual(choices, expected)
```

### Comparing `cubicweb-eac-1.5.3/test/utils.py` & `cubicweb-eac-2.0.0/test/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-eac-1.5.3/tox.ini` & `cubicweb-eac-2.0.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tox]
 envlist = py3,flake8,check-manifest,yamllint,black
 
 [testenv]
 deps =
   -rdev-requirements.txt
 commands =
-  {envpython} -m pytest {posargs:test}
+  {envpython} -m pytest -vv {posargs:test}
 
 [testenv:check-manifest]
 skip_install = true
 deps =
   check-manifest
 commands =
   {envpython} -m check_manifest {toxinidir}
```

