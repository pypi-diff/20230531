# Comparing `tmp/hyperthought-transfer-0.2.2.tar.gz` & `tmp/hyperthought-transfer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jason\Documents\repos\hyperthought-transfer\dist\tmpsfgw0z5u\hyperthought-transfer-0.2.2.tar", last modified: Wed May 31 09:36:38 2023, max compression
+gzip compressed data, was "C:\Users\Jason\Documents\repos\hyperthought-transfer\dist\tmpbh_esrx_\hyperthought-transfer-0.2.3.tar", last modified: Wed May 31 15:21:59 2023, max compression
```

## Comparing `hyperthought-transfer-0.2.2.tar` & `hyperthought-transfer-0.2.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/
--rw-rw-rw-   0        0        0      632 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/.coveragerc
--rw-rw-rw-   0        0        0      661 2023-01-03 12:02:08.000000 hyperthought-transfer-0.2.2/.gitignore
--rw-rw-rw-   0        0        0      514 2023-01-03 12:02:08.000000 hyperthought-transfer-0.2.2/.readthedocs.yml
--rw-rw-rw-   0        0        0       84 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/AUTHORS.rst
--rw-rw-rw-   0        0        0      141 2022-05-17 15:55:48.000000 hyperthought-transfer-0.2.2/CHANGELOG.rst
--rw-rw-rw-   0        0        0    14388 2022-12-27 15:26:41.000000 hyperthought-transfer-0.2.2/CONTRIBUTING.rst
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/docs/
--rw-rw-rw-   0        0        0       43 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/docs/authors.rst
--rw-rw-rw-   0        0        0       45 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/docs/changelog.rst
--rw-rw-rw-   0        0        0    10090 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/docs/contributing.rst
--rw-rw-rw-   0        0        0     2430 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/docs/index.rst
--rw-rw-rw-   0        0        0       74 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/docs/license.rst
--rw-rw-rw-   0        0        0     1183 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/docs/Makefile
--rw-rw-rw-   0        0        0       41 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/docs/readme.rst
--rw-rw-rw-   0        0        0      238 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/docs/_static/
--rw-rw-rw-   0        0        0       19 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/docs/_static/.gitignore
--rw-rw-rw-   0        0        0     1100 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0      150 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2766 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2022-05-17 15:55:48.000000 hyperthought-transfer-0.2.2/README.rst
--rw-rw-rw-   0        0        0     1335 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-05-31 09:35:56.000000 hyperthought-transfer-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/antivirus/
--rw-rw-rw-   0        0        0     2513 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/antivirus/base.py
--rw-rw-rw-   0        0        0     2928 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/antivirus/_mcafee.py
--rw-rw-rw-   0        0        0     2992 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/antivirus/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/
--rw-rw-rw-   0        0        0      798 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/data.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/database/
--rw-rw-rw-   0        0        0     1224 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/database/connect.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/database/template/
--rw-rw-rw-   0        0        0     1419 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/database/template/create.py
--rw-rw-rw-   0        0        0    40960 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/database/template/template.db
--rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/database/template/__init__.py
--rw-rw-rw-   0        0        0     4130 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/database/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/process/
--rw-rw-rw-   0        0        0     6642 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/process/filebinner.py
--rw-rw-rw-   0        0        0       40 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/process/__init__.py
--rw-rw-rw-   0        0        0       47 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/database/
--rw-rw-rw-   0        0        0     3273 2023-05-31 09:22:05.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/database/connect.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/database/template/
--rw-rw-rw-   0        0        0     1596 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/database/template/create.py
--rw-rw-rw-   0        0        0   147456 2023-05-30 11:50:42.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/database/template/template.db
--rw-rw-rw-   0        0        0       36 2023-02-01 16:27:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/database/template/__init__.py
--rw-rw-rw-   0        0        0    71738 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/database/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/processes/
--rw-rw-rw-   0        0        0     6857 2023-05-31 09:04:03.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/processes/rules.py
--rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/processes/__init__.py
--rw-rw-rw-   0        0        0     2046 2023-01-03 12:02:08.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/utils.py
--rw-rw-rw-   0        0        0    49016 2023-05-31 08:46:11.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/__init__.py
--rw-rw-rw-   0        0        0      713 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-05-16 11:27:09.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2766 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1840 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       22 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/src/hyperthought_transfer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 09:36:38.000000 hyperthought-transfer-0.2.2/tests/
--rw-rw-rw-   0        0        0      299 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/tests/conftest.py
--rw-rw-rw-   0        0        0     2659 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.2/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:59.000000 hyperthought-transfer-0.2.3/
+-rw-rw-rw-   0        0        0      632 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/.coveragerc
+-rw-rw-rw-   0        0        0      661 2023-01-03 12:02:08.000000 hyperthought-transfer-0.2.3/.gitignore
+-rw-rw-rw-   0        0        0      514 2023-01-03 12:02:08.000000 hyperthought-transfer-0.2.3/.readthedocs.yml
+-rw-rw-rw-   0        0        0       84 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0      141 2022-05-17 15:55:48.000000 hyperthought-transfer-0.2.3/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    14388 2022-12-27 15:26:41.000000 hyperthought-transfer-0.2.3/CONTRIBUTING.rst
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/docs/
+-rw-rw-rw-   0        0        0       43 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/docs/authors.rst
+-rw-rw-rw-   0        0        0       45 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/docs/changelog.rst
+-rw-rw-rw-   0        0        0    10090 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/docs/contributing.rst
+-rw-rw-rw-   0        0        0     2430 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/docs/index.rst
+-rw-rw-rw-   0        0        0       74 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/docs/license.rst
+-rw-rw-rw-   0        0        0     1183 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/docs/Makefile
+-rw-rw-rw-   0        0        0       41 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/docs/readme.rst
+-rw-rw-rw-   0        0        0      238 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/docs/_static/
+-rw-rw-rw-   0        0        0       19 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/docs/_static/.gitignore
+-rw-rw-rw-   0        0        0     1100 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      150 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2766 2023-05-31 15:21:59.000000 hyperthought-transfer-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2022-05-17 15:55:48.000000 hyperthought-transfer-0.2.3/README.rst
+-rw-rw-rw-   0        0        0     1335 2023-05-31 15:21:59.000000 hyperthought-transfer-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-05-31 13:17:13.000000 hyperthought-transfer-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/antivirus/
+-rw-rw-rw-   0        0        0     2513 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/antivirus/base.py
+-rw-rw-rw-   0        0        0     2928 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/antivirus/_mcafee.py
+-rw-rw-rw-   0        0        0     2992 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/antivirus/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/
+-rw-rw-rw-   0        0        0      798 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/data.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/database/
+-rw-rw-rw-   0        0        0     1224 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/database/connect.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/database/template/
+-rw-rw-rw-   0        0        0     1419 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/database/template/create.py
+-rw-rw-rw-   0        0        0    40960 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/database/template/template.db
+-rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/database/template/__init__.py
+-rw-rw-rw-   0        0        0     4130 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/database/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/process/
+-rw-rw-rw-   0        0        0     6642 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/process/filebinner.py
+-rw-rw-rw-   0        0        0       40 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/process/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:59.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/database/
+-rw-rw-rw-   0        0        0     3273 2023-05-31 09:22:05.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/database/connect.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:59.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/database/template/
+-rw-rw-rw-   0        0        0     1596 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/database/template/create.py
+-rw-rw-rw-   0        0        0   147456 2023-05-30 11:50:42.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/database/template/template.db
+-rw-rw-rw-   0        0        0       36 2023-02-01 16:27:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/database/template/__init__.py
+-rw-rw-rw-   0        0        0    72906 2023-05-31 15:21:47.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/database/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:59.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/processes/
+-rw-rw-rw-   0        0        0     6857 2023-05-31 09:04:03.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/processes/rules.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/processes/__init__.py
+-rw-rw-rw-   0        0        0     2046 2023-01-03 12:02:08.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/utils.py
+-rw-rw-rw-   0        0        0    49016 2023-05-31 08:46:11.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-05-16 11:27:09.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2766 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1840 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       22 2023-05-31 15:21:58.000000 hyperthought-transfer-0.2.3/src/hyperthought_transfer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 15:21:59.000000 hyperthought-transfer-0.2.3/tests/
+-rw-rw-rw-   0        0        0      299 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/tests/conftest.py
+-rw-rw-rw-   0        0        0     2659 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.3/tox.ini
```

### Comparing `hyperthought-transfer-0.2.2/.coveragerc` & `hyperthought-transfer-0.2.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/.gitignore` & `hyperthought-transfer-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/.readthedocs.yml` & `hyperthought-transfer-0.2.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/CONTRIBUTING.rst` & `hyperthought-transfer-0.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/docs/conf.py` & `hyperthought-transfer-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/docs/index.rst` & `hyperthought-transfer-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/docs/Makefile` & `hyperthought-transfer-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/LICENSE.txt` & `hyperthought-transfer-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/PKG-INFO` & `hyperthought-transfer-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperthought-transfer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Package used to upload files to and download files from the HyperThought® content management system.
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Jason Thiese
 Author-email: jthiese@ues.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `hyperthought-transfer-0.2.2/README.rst` & `hyperthought-transfer-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/setup.cfg` & `hyperthought-transfer-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/setup.py` & `hyperthought-transfer-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 from setuptools import setup, find_packages
 
 
 if __name__ == "__main__":
     try:
         setup(
-            version="0.2.2",
+            version="0.2.3",
             use_scm_version={
                 "version_scheme": "no-guess-dev",
                 "local-scheme": "no-local-version",
             },
             packages=find_packages(where="src"),
             package_dir={"": "src"},
             include_package_data=True,
```

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/antivirus/base.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/antivirus/base.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/antivirus/_mcafee.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/antivirus/_mcafee.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/antivirus/__init__.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/antivirus/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/data.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/data.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/database/connect.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/database/connect.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/database/template/create.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/database/template/create.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/database/template/template.db` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/database/template/template.db`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/database/__init__.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/database/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/filebinner/process/filebinner.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/filebinner/process/filebinner.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/database/connect.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/database/connect.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/database/template/create.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/database/template/create.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/database/template/template.db` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/database/template/template.db`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/database/__init__.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/database/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -778,14 +778,56 @@
 
         for row in cursor.fetchall():
             yield {
                 key: row[key]
                 for key in row.keys()
             }
 
+    def get_parser_counts_for_files(
+        self,
+        file_ids: List[int],
+    ) -> Dict[int, int]:
+        """
+        Get parser counts for given files.
+
+        Parameters
+        ----------
+        file_id : list of int
+            File ids of interest.
+
+        Returns
+        -------
+        A dict mapping each file id to the number of parsers associated with
+        the file.
+        """
+        for file_id in file_ids:
+            if not isinstance(file_id, int):
+                raise ValueError(f"{file_id} is not an int")
+
+        file_list = ", ".join(str(file_id) for file_id in file_ids)
+        sql = f"""
+        SELECT
+            File.id AS file_id,
+            COUNT(*) AS parser_count
+        FROM
+            File INNER JOIN Parser ON File.id = Parser.file_id
+        WHERE
+            File.id IN ({file_list})
+        GROUP BY
+            File.id
+        """
+        cursor = self.connection.cursor()
+        cursor.execute(sql)
+        results = {
+            row["file_id"]: row["parser_count"]
+            for row in cursor.fetchall()
+        }
+        cursor.close()
+        return results
+
     def get_all_metadata(
         self,
         file_specific: bool = True
     ) -> Generator[Dict, Optional[None], Optional[None]]:
         """
         Get all Metadata records.
```

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/processes/rules.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/processes/rules.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/utils.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/utils.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/manifest/__init__.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer/__init__.py` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer.egg-info/PKG-INFO` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperthought-transfer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Package used to upload files to and download files from the HyperThought® content management system.
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Jason Thiese
 Author-email: jthiese@ues.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `hyperthought-transfer-0.2.2/src/hyperthought_transfer.egg-info/SOURCES.txt` & `hyperthought-transfer-0.2.3/src/hyperthought_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2.2/tox.ini` & `hyperthought-transfer-0.2.3/tox.ini`

 * *Files identical despite different names*

