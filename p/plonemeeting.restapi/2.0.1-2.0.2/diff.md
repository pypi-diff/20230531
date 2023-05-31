# Comparing `tmp/plonemeeting.restapi-2.0.1.tar.gz` & `tmp/plonemeeting.restapi-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plonemeeting.restapi-2.0.1.tar", last modified: Tue Mar  7 15:02:43 2023, max compression
+gzip compressed data, was "dist/plonemeeting.restapi-2.0.2.tar", last modified: Wed May 31 08:59:30 2023, max compression
```

## Comparing `plonemeeting.restapi-2.0.1.tar` & `plonemeeting.restapi-2.0.2.tar`

### file list

```diff
@@ -1,97 +1,100 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      657 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/LICENSE.rst
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      272 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/setuphandlers.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3192 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/get.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      725 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/users.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15679 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/add.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3132 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1667 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/meetingconfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6723 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/search.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1469 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/annex.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1372 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/infos.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1531 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      475 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/imio.history.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      575 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/en/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      609 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/en/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      434 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/plone.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      609 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      667 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/imio.history.po
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      332 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/sync_pos.sh
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/profiles/testing/metadata.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      176 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      240 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/profiles/default/rolemap.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/profiles/default/catalog.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1200 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8563 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9154 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/item.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2060 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5072 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/meetingconfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4971 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/user.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3579 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/dxfields.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    20042 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1636 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/pod_template.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2522 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/atfields.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1847 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/summary.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2916 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/catalog.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3241 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/meeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2157 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/annex.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      741 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/converters.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      524 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      283 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/testing.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/deserializer/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      458 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/deserializer/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      952 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/deserializer/dxfields.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      879 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/deserializer/atfields.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/deserializer/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2354 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/deserializer/atcontent.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2746 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_infos.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1550 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5671 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_annexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24124 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_get.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8682 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13616 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_meetingconfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    43097 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_add.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6953 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_users.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    38238 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_search.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      330 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/overrides.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/src/plonemeeting/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting.restapi.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting.restapi.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      145 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting.restapi.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting.restapi.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting.restapi.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22252 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting.restapi.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3378 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting.restapi.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting.restapi.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/src/plonemeeting.restapi.egg-info/requires.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      125 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/bootstrap.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       61 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/requirements.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1745 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22252 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      167 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16518 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1162 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      469 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/Makefile
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      199 2023-03-07 15:02:42.000000 plonemeeting.restapi-2.0.1/README.md
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2023-03-07 15:02:43.000000 plonemeeting.restapi-2.0.1/setup.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      657 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/LICENSE.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      272 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/setuphandlers.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3192 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/get.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      725 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/users.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15679 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/add.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4315 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1667 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/meetingconfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6723 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/search.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1469 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/annex.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11176 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/attendees.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1372 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/infos.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1531 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      475 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/imio.history.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      575 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/en/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      609 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/en/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      434 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/plone.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      609 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      667 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/imio.history.po
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      332 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/sync_pos.sh
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/testing/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      176 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      240 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/default/rolemap.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/default/catalog.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1200 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8670 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9914 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/item.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2181 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5072 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/meetingconfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5028 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/user.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1366 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/held_position.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3579 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/dxfields.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24015 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/base.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1636 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/pod_template.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2522 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/atfields.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1847 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/summary.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2916 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/catalog.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3517 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/meeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2157 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/annex.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      741 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/converters.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      524 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      283 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/testing.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      458 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      952 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/dxfields.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      879 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/atfields.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2354 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/atcontent.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23607 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_attendees.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2746 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_infos.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1550 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/base.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5671 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_annexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24124 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_get.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8682 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13616 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_meetingconfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    45503 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_add.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6953 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_users.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    38238 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_search.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      330 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/overrides.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      145 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22581 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3536 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/requires.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      125 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/bootstrap.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       61 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/requirements.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1745 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22581 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      167 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16775 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1162 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      469 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/Makefile
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      199 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/README.md
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/setup.cfg
```

### Comparing `plonemeeting.restapi-2.0.1/LICENSE.rst` & `plonemeeting.restapi-2.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/get.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/get.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/users.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/users.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/add.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/add.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/configure.zcml` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/configure.zcml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:plone="http://namespaces.plone.org/plone"
     xmlns:zcml="http://namespaces.zope.org/zcml">
 
-  <!-- get UID -->
+  <!-- GET element from UID -->
   <plone:service
     method="GET"
     for="Products.CMFPlone.interfaces.IPloneSiteRoot"
     factory=".get.UidSearchGet"
     name="@get"
     layer="plonemeeting.restapi.interfaces.IPMRestapiLayer"
     permission="zope2.View" />
 
-  <!-- search -->
+  <!-- GET search -->
   <plone:service
     method="GET"
     for="Products.CMFCore.interfaces.ISiteRoot"
     accept="application/json,application/schema+json"
     name="@search"
     factory=".search.PMSearchGet"
     layer="plonemeeting.restapi.interfaces.IPMRestapiLayer"
@@ -36,15 +36,15 @@
     method="POST"
     name="@annex"
     for="Products.CMFCore.interfaces.ISiteRoot"
     factory=".add.AnnexPost"
     layer="plonemeeting.restapi.interfaces.IPMRestapiLayer"
     permission="zope2.View" />
 
-  <!-- get UID item -->
+  <!-- GET item from UID -->
   <plone:service
     method="GET"
     for="Products.CMFCore.interfaces.IFolderish"
     factory=".get.ItemGet"
     name="@item"
     layer="plonemeeting.restapi.interfaces.IPMRestapiLayer"
     permission="zope2.View" />
@@ -65,47 +65,80 @@
     factory=".add.MeetingPost"
     name="@meeting"
     layer="plonemeeting.restapi.interfaces.IPMRestapiLayer"
     permission="zope2.View" />
 
   <adapter factory=".annex.Annexes" name="annex" />
 
-  <!-- annexes -->
+  <!-- GET annexes -->
   <plone:service
     method="GET"
     for="zope.interface.Interface"
     accept="application/json,application/schema+json"
     name="@annexes"
     factory=".annex.AnnexesGet"
     layer="plonemeeting.restapi.interfaces.IPMRestapiLayer"
     permission="zope2.View" />
 
-  <!-- get config -->
+  <!-- GET config -->
   <plone:service
     method="GET"
     for="zope.interface.Interface"
     accept="application/json,application/schema+json"
     name="@config"
     factory=".meetingconfig.ConfigSearchGet"
     layer="plonemeeting.restapi.interfaces.IPMRestapiLayer"
     permission="zope2.View" />
 
-  <!-- get infos -->
+  <!-- GET infos -->
   <plone:service
     method="GET"
     for="zope.interface.Interface"
     accept="application/json,application/schema+json"
     name="@infos"
     factory=".infos.PMInfosGet"
     layer="plonemeeting.restapi.interfaces.IPMRestapiLayer"
     permission="zope2.View" />
 
-  <!-- get users -->
+  <!-- GET users -->
   <plone:service
       method="GET"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      accept="application/json,application/schema+json"
+      name="@users"
       factory=".users.PMUsersGet"
+      layer="plonemeeting.restapi.interfaces.IPMRestapiLayer"
+      permission="zope2.View" />
+
+  <!-- GET attendees on meeting or item -->
+  <plone:service
+      method="GET"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      accept="application/json,application/schema+json"
+      name="@attendees"
+      factory=".attendees.AttendeesGet"
+      layer="plonemeeting.restapi.interfaces.IPMRestapiLayer"
+      permission="zope2.View" />
+
+  <!-- GET attendee on meeting or item -->
+  <plone:service
+      method="GET"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      accept="application/json,application/schema+json"
+      name="@attendee"
+      factory=".attendees.AttendeeGet"
+      layer="plonemeeting.restapi.interfaces.IPMRestapiLayer"
+      permission="zope2.View" />
+
+  <adapter factory=".attendees.Attendees" name="attendees" />
+
+  <!-- PATCH attendee on meeting or item -->
+  <plone:service
+      method="PATCH"
       for="Products.CMFCore.interfaces.ISiteRoot"
-      permission="zope2.View"
+      accept="application/json,application/schema+json"
+      name="@attendee"
+      factory=".attendees.AttendeePatch"
       layer="plonemeeting.restapi.interfaces.IPMRestapiLayer"
-      name="@users" />
+      permission="zope2.View" />
 
 </configure>
```

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/meetingconfig.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/meetingconfig.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/search.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/search.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/annex.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/annex.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/services/infos.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/infos.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/configure.zcml` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/en/LC_MESSAGES/plone.po` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/en/LC_MESSAGES/imio.history.po` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/plone.po` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/imio.history.po` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/testing.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/testing.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/utils.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,24 @@
                                (api.user.get_current().getId(), cfg_id, in_name_of))
         user = api.user.get(in_name_of)
         if not user:
             raise BadRequest(IN_NAME_OF_USER_NOT_FOUND % in_name_of)
     return in_name_of, access_cfg_ids
 
 
-def get_serializer(obj, extra_include_name=None, serializer=None):
+def get_serializer(obj, extra_include_name=None, serializer=None, interface=ISerializeToJsonSummary):
     """ """
     request = getRequest()
-    interface = ISerializeToJsonSummary
-    prefix = ''
-    if extra_include_name:
-        prefix = "extra_include_{0}_".format(extra_include_name)
-    if use_obj_serializer(request.form, prefix=prefix):
-        interface = ISerializeToJson
+    # check if need to use ISerializeToJson interface
+    if interface != ISerializeToJson:
+        prefix = ''
+        if extra_include_name:
+            prefix = "extra_include_{0}_".format(extra_include_name)
+        if use_obj_serializer(request.form, prefix=prefix):
+            interface = ISerializeToJson
     serializer = queryMultiAdapter((obj, request), interface)
     if extra_include_name:
         serializer._extra_include_name = extra_include_name
     return serializer
 
 
 def get_param(value, default=False, extra_include_name=None, serializer=None):
```

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/item.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # -*- coding: utf-8 -*-
 
 from imio.helpers.content import uuidsToObjects
 from plone import api
 from plone.restapi.interfaces import ISerializeToJson
 from plone.restapi.interfaces import ISerializeToJsonSummary
 from plonemeeting.restapi.serializer.base import BaseATSerializeFolderToJson
+from plonemeeting.restapi.serializer.base import serialize_attendees
 from plonemeeting.restapi.serializer.base import serialize_extra_include_annexes
 from plonemeeting.restapi.serializer.base import serialize_pod_templates
 from plonemeeting.restapi.serializer.summary import PMBrainJSONSummarySerializer
 from plonemeeting.restapi.utils import build_catalog_query
 from Products.PloneMeeting.interfaces import IMeetingItem
+from Products.PloneMeeting.utils import get_internal_number
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
 
 
 class BaseSerializeItemToJson(object):
     """ """
 
     def _available_extra_includes(self, result):
         """ """
         result["@extra_includes"] = [
             "annexes",
+            "attendees",
             "proposing_group",
             "category",
             "classifier",
             "groups_in_charge",
             "associated_groups",
             "pod_templates",
             "meeting",
@@ -123,14 +126,17 @@
         if "config" in extra_include:
             tool = api.portal.get_tool('portal_plonemeeting')
             cfg = tool.getMeetingConfig(self.context)
             result["extra_include_config"] = {}
             if cfg:
                 serializer = self._get_serializer(cfg, "config")
                 result["extra_include_config"] = serializer()
+        if "attendees" in extra_include:
+            result["extra_include_attendees"] = serialize_attendees(
+                self.context, extra_include_name="attendees", base_serializer=self)
 
         # various type of deliberation may be included
         # if we find a key containing "deliberation", we use it
         # add pass it to documentgenerator helper.deliberation_for_restapi
         delib_extra_includes = [ei for ei in extra_include
                                 if "deliberation" in ei]
         if delib_extra_includes:
@@ -176,12 +182,20 @@
 
 
 @implementer(ISerializeToJson)
 @adapter(IMeetingItem, Interface)
 class SerializeToJson(BaseSerializeItemToJson, BaseATSerializeFolderToJson):
     """ """
 
+    def _include_fields(self, obj):
+        """Manage internal_numbe manually as it is not a field for now but
+           a stored attribute, will be a field when item will be DX."""
+        result = super(SerializeToJson, self)._include_fields(obj)
+        if self.fullobjects or "internal_number" in self.metadata_fields:
+            result["internal_number"] = get_internal_number(obj)
+        return result
+
 
 @implementer(ISerializeToJsonSummary)
 @adapter(IMeetingItem, Interface)
 class SerializeToJsonSummary(BaseSerializeItemToJson, PMBrainJSONSummarySerializer):
     """ """
```

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/configure.zcml` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/configure.zcml`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
     <!-- Custom serializers -->
     <adapter factory=".annex.SerializeToJson" />
     <adapter factory=".annex.SerializeToJsonSummary" />
     <adapter factory=".catalog.PMLazyCatalogResultSerializer" />
     <adapter factory=".item.SerializeToJson" />
     <adapter factory=".item.SerializeToJsonSummary" />
+    <adapter factory=".held_position.SerializeToJson" />
+    <adapter factory=".held_position.SerializeToJsonSummary" />
     <adapter factory=".meeting.SerializeToJson" />
     <adapter factory=".meeting.SerializeToJsonSummary" />
     <adapter factory=".meetingconfig.SerializeToJson" />
     <adapter factory=".meetingconfig.SerializeToJsonSummary" />
     <adapter factory=".summary.PMJSONSummarySerializer" />
     <adapter factory=".pod_template.SerializeToJson" />
     <adapter factory=".pod_template.SerializeToJsonSummary" />
```

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/meetingconfig.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/meetingconfig.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/user.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 
+from imio.helpers.cache import get_plone_groups_for_user
 from plone import api
 from plone.restapi.interfaces import ISerializeToJson
 from plone.restapi.interfaces import ISerializeToJsonSummary
 from plone.restapi.serializer.user import BaseSerializer as BaseUserSerializer
 from plonemeeting.restapi.interfaces import IPMRestapiLayer
 from plonemeeting.restapi.serializer.base import BaseSerializeToJson
 from Products.CMFCore.interfaces._tools import IMemberData
```

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/dxfields.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/dxfields.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/base.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from collective.documentgenerator.interfaces import IGenerablePODTemplates
 from collective.iconifiedcategory.utils import _categorized_elements
 from collective.iconifiedcategory.utils import get_categorized_elements
 from imio.helpers.content import base_hasattr
 from imio.helpers.content import get_vocab
 from imio.restapi.serializer.base import SerializeFolderToJson as IMIODXSerializeFolderToJson
 from imio.restapi.serializer.base import SerializeToJson as IMIODXSerializeToJson
+from imio.restapi.utils import serialize_term
 from plone import api
 from plone.autoform.interfaces import READ_PERMISSIONS_KEY
 from plone.dexterity.interfaces import IDexterityContainer
 from plone.dexterity.interfaces import IDexterityContent
 from plone.dexterity.utils import iterSchemata
 from plone.restapi.batching import HypermediaBatch
 from plone.restapi.deserializer import boolean_value
@@ -26,20 +27,20 @@
 from plone.restapi.serializer.nextprev import NextPrevious
 from plone.supermodel.utils import mergedTaggedValueDict
 from plonemeeting.restapi import logger
 from plonemeeting.restapi.config import ANNEXES_FILTER_VALUES
 from plonemeeting.restapi.interfaces import IPMRestapiLayer
 from plonemeeting.restapi.utils import get_param
 from plonemeeting.restapi.utils import get_serializer
-from Products.CMFCore.utils import getToolByName
 from zope.component import adapter
 from zope.component import ComponentLookupError
 from zope.component import getAdapter
 from zope.component import getMultiAdapter
 from zope.component import queryMultiAdapter
+from zope.i18n import translate
 from zope.interface import implementer
 from zope.interface import Interface
 from zope.schema import getFields
 
 
 NO_VOCAB_ERROR = "Trying to get vocabulary for field %s but it is None"
 SUFFIXED_CHOICES_PATTERN = "%s__choices"
@@ -87,16 +88,93 @@
     # uids must contains something or passing an empty list means do not filter on uids
     uids = uids or ["dummy_uid"]
     annexes = get_categorized_elements(
         context, result_type="objects", uids=uids)  # , filters=filters)
     for annex in annexes:
         serializer = get_serializer(
             annex, extra_include_name=extra_include_name, serializer=base_serializer)
-        serialized_annex = serializer()
-        result.append(serialized_annex)
+        result.append(serializer())
+    return result
+
+
+def serialize_attendees(context, attendee=None, extra_include_name=None, base_serializer=None):
+    """ """
+    result = []
+    tool = api.portal.get_tool("portal_plonemeeting")
+    cfg = tool.getMeetingConfig(context)
+    attendee_types = {}
+    is_meeting = context.__class__.__name__ == "Meeting"
+    meeting = context if is_meeting else context.getMeeting()
+    # return empty result when called on item out of meeting
+    if meeting is None:
+        return result
+    if is_meeting:
+        attendee_types.update({attendee_uid: 'present' for attendee_uid in context.get_attendees()})
+        attendee_types.update({absent_uid: 'absent' for absent_uid in context.get_absents()})
+        attendee_types.update({excused_uid: 'excused' for excused_uid in context.get_excused()})
+    else:
+        # MeetingItem
+        attendee_types.update({attendee_uid: 'present' for attendee_uid in context.get_attendees()})
+        attendee_types.update({absent_uid: 'absent' for absent_uid in
+                               meeting.get_absents() + context.get_item_absents()})
+        attendee_types.update({excused_uid: 'excused' for excused_uid in
+                               meeting.get_excused() + context.get_item_excused()})
+
+    # initialize voter
+    voters = meeting.get_voters()
+    signatories = context.get_signatories(include_position_type=True) \
+        if is_meeting else context.get_item_signatories(include_position_type=True)
+    non_attendees = context.get_item_non_attendees()
+    attendees = [attendee] if attendee is not None else context.get_all_attendees(the_objects=True)
+    for attendee in attendees:
+        serializer = get_serializer(
+            attendee,
+            extra_include_name=extra_include_name,
+            serializer=base_serializer,
+            interface=ISerializeToJson)
+        # for is_meeting position_type, let the serializer manage it
+        serializer._init()
+        serializer.fullobjects = False
+        if is_meeting:
+            serializer.metadata_fields = ['position_type']
+        serialized = serializer()
+        serialized_uid = serialized['UID']
+        # for not is_meeting position_type, manage it manually as it may be redefined
+        # attendee (context) is used to return correct value depending on gender/number
+        position_type_vocab = None
+        if not is_meeting:
+            position_type_vocab = get_vocab(attendee, "PMPositionTypes")
+            serialized['position_type'] = serialize_term(
+                meeting.get_attendee_position_for(context.UID(), serialized_uid),
+                position_type_vocab)
+        # manage "attendee_type"
+        attendee_type = "non_attendee" if \
+            serialized_uid in non_attendees else attendee_types[serialized_uid]
+        serialized["attendee_type"] = {
+            'token': attendee_type,
+            'title': translate(attendee_type, domain="PloneMeeting", context=context.REQUEST)}
+        # manage "signatory"
+        serialized["signatory"] = None
+        serialized["signatory_position_type"] = None
+        signatory_infos = signatories.get(serialized_uid, {})
+        if signatory_infos:
+            position_type_vocab = position_type_vocab if position_type_vocab is not None \
+                else get_vocab(attendee, "PMPositionTypes")
+            serialized["signatory"] = signatory_infos['signature_number']
+            serialized["signatory_position_type"] = serialize_term(
+                signatory_infos['position_type'],
+                position_type_vocab)
+        # manage "voter"
+        serialized["voter"] = serialized_uid in voters
+        result.append(serialized)
+        # manage hp title that could change on item
+        item = None
+        if not is_meeting:
+            item = context
+        serialized["title"] = meeting.get_attendee_short_title(attendee, cfg, item=item)
     return result
 
 
 def serialize_extra_include_annexes(result, serializer):
     """ """
     # compute filters to get annexes
     filters = {}
@@ -113,14 +191,17 @@
 
 
 class BaseSerializeToJson(object):
     """__call__ must be redefined by class heritating from BaseSerializeToJson."""
 
     def _init(self):
         """ """
+        # if already _init, pass, could have been changed manually
+        if base_hasattr(self, 'metadata_fields'):
+            return
         self.metadata_fields = self.get_param('metadata_fields', [])
         self.asked_extra_include = self._get_asked_extra_include()
         self.asked_additional_values = self._get_asked_additional_values()
         self.asked_includes = self._get_asked_includes()
         # fullobjects is True:
         # if actually asked in request
         # or if nothing else asked
@@ -294,15 +375,15 @@
     def _include_items(self, obj, include_items):
         """ """
         result = {}
         include_items = self.get_param("include_items", include_items)
         if include_items:
             query = self._build_query()
 
-            catalog = getToolByName(self.context, "portal_catalog")
+            catalog = api.portal.get_tool("portal_catalog")
             brains = catalog(query)
 
             batch = HypermediaBatch(self.request, brains)
 
             result["items_total"] = batch.items_total
             if batch.links:
                 result["batching"] = batch.links
```

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/pod_template.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/pod_template.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/atfields.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/atfields.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/summary.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/summary.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/catalog.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/catalog.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/meeting.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/meeting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from plone import api
 from plone.restapi.interfaces import IFieldSerializer
 from plone.restapi.interfaces import ISerializeToJson
 from plone.restapi.interfaces import ISerializeToJsonSummary
 from plonemeeting.restapi.serializer.base import BaseDXSerializeFolderToJson
+from plonemeeting.restapi.serializer.base import serialize_attendees
 from plonemeeting.restapi.serializer.base import serialize_extra_include_annexes
 from plonemeeting.restapi.serializer.base import serialize_pod_templates
 from plonemeeting.restapi.serializer.summary import PMBrainJSONSummarySerializer
 from Products.PloneMeeting.content.meeting import IMeeting
 from Products.PloneMeeting.utils import get_dx_field
 from zope.component import adapter
 from zope.component import queryMultiAdapter
@@ -17,25 +18,28 @@
 
 
 class BaseSerializeMeetingToJson(object):
     """ """
 
     def _available_extra_includes(self, result):
         """ """
-        result["@extra_includes"] = ["annexes", "pod_templates"]
+        result["@extra_includes"] = ["annexes", "attendees", "pod_templates"]
         return result
 
     def _extra_include(self, result):
         """ """
         extra_include = self._get_asked_extra_include()
         if "pod_templates" in extra_include:
             result["extra_include_pod_templates"] = serialize_pod_templates(
                 self.context, self)
         if "annexes" in extra_include:
             result = serialize_extra_include_annexes(result, self)
+        if "attendees" in extra_include:
+            result["extra_include_attendees"] = serialize_attendees(
+                self.context, extra_include_name="attendees", base_serializer=self)
         return result
 
     def _include_custom(self, obj, result):
         """Include "date" by default."""
         if self.fullobjects or \
            "date" in self.metadata_fields or \
            self.get_param('include_base_data', True):
```

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/annex.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/annex.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/serializer/converters.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/converters.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/config.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/config.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/deserializer/dxfields.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/dxfields.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/deserializer/atfields.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/atfields.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/deserializer/atcontent.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/atcontent.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_infos.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_infos.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/base.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/base.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_annexes.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_annexes.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_get.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_get.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/config.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/config.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_meetingconfig.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_meetingconfig.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_add.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 
+from collective.behavior.internalnumber.browser.settings import set_settings
 from collective.iconifiedcategory.utils import calculate_category_id
 from datetime import datetime
 from datetime import timedelta
 from imio.helpers.content import object_values
 from plonemeeting.restapi.config import CONFIG_ID_ERROR
 from plonemeeting.restapi.config import CONFIG_ID_NOT_FOUND_ERROR
 from plonemeeting.restapi.services.add import ANNEX_CONTENT_CATEGORY_ERROR
@@ -217,42 +218,49 @@
         self._enableField("associatedGroups")
         self.changeUser("pmManager")
         transaction.commit()
         endpoint_url = "{0}/@item".format(self.portal_url)
         json = {
             "config_id": cfg.getId(),
             "proposingGroup": self.developers.getId(),
+            "preferredMeeting": "unknown_uid",
             "optionalAdvisers": [self.vendors.getId(), self.orgOutside1_uid],
             "groupsInCharge": [self.vendors.getId(), self.orgOutside1_uid],
             "title": "My item",
         }
         response = self.api_session.post(endpoint_url, json=json)
         self.assertEqual(response.status_code, 400, response.content)
         self.assertEqual(
             response.json(),
-            {u'message': u'[{\'field\': \'groupsInCharge\', \'message\': u"Values [\'%s\'] '
-             u'are not allowed for vocabulary of element Groups in charge.", \'error\': \'ValidationError\'}, '
-             u'{\'field\': \'optionalAdvisers\', \'message\': u"Values [\'%s\'] are not allowed for '
-             u'vocabulary of element Optional advisers.", \'error\': \'ValidationError\'}]' % (
-                 self.orgOutside1_uid, self.orgOutside1_uid),
+            {u'message': u'[{\'field\': \'groupsInCharge\', \'message\': '
+             u'u"Values [\'%s\'] are not allowed for vocabulary of element Groups in charge.", '
+             u'\'error\': \'ValidationError\'}, {\'field\': \'optionalAdvisers\', '
+             u'\'message\': u"Values [\'%s\'] are not allowed for vocabulary of element Optional advisers.", '
+             u'\'error\': \'ValidationError\'}, {\'field\': \'preferredMeeting\', \'message\': '
+             u'u"Values [\'unknown_uid\'] are not allowed for vocabulary of element Preferred meeting.", '
+             u'\'error\': \'ValidationError\'}]' % (self.orgOutside1_uid, self.orgOutside1_uid),
              u'type': u'BadRequest'})
+        # if preferredMeeting set to None, then created item will use ITEM_NO_PREFERRED_MEETING_VALUE
+        json["preferredMeeting"] = None
         # check for groupsInCharge
         json["optionalAdvisers"] = [self.vendors.getId()]
         response = self.api_session.post(endpoint_url, json=json)
         self.assertEqual(response.status_code, 400, response.content)
         self.assertEqual(
             response.json(),
             {u'message': u'[{\'field\': \'groupsInCharge\', \'message\': u"Values [\'%s\'] '
              u'are not allowed for vocabulary of element Groups in charge.", '
              u'\'error\': \'ValidationError\'}]' % self.orgOutside1_uid,
              u'type': u'BadRequest'})
         # fix everything
         json["groupsInCharge"] = [self.vendors.getId()]
         response = self.api_session.post(endpoint_url, json=json)
         self.assertEqual(response.status_code, 201, response.content)
+        self.assertEqual(response.json()["preferredMeeting"],
+                         {u'token': u'whatever', u'title': u'No preference'})
 
     def test_restapi_add_item_wf_transitions_present(self):
         """When creating an item, we may define "wf_transitions"
            until "present", in this case, item is "presented" in next meeting."""
         cfg = self.meetingConfig
         self.changeUser("pmManager")
         # meeting in the future
@@ -428,30 +436,32 @@
             {
                 u"message": IGNORE_VALIDATION_FOR_VALUED_ERROR % "category",
                 u"type": u"BadRequest",
             }
         )
         # use "ignore_validation_for" correctly
         # bypass category validation and classifier validation
-        # remove category from data and pass an empty classifier
+        # pass empty classifier/category
+        # define a ignore_validation_for a field that it not in json data
         # check also that such an item may be set to WF state "validated"
-        json["ignore_validation_for"] = ["category", "classifier"]
-        json.pop("category")
+        json["ignore_validation_for"] = ["category", "classifier", "groupsInCharge"]
+        json["category"] = None
         json["classifier"] = None
         json["wf_transitions"] = ["propose", "validate"]
         response = self.api_session.post(endpoint_url, json=json)
         transaction.begin()
         self.assertEqual(response.status_code, 201, response.content)
         pmFolder = self.getMeetingFolder()
         item = pmFolder.objectValues()[-1]
         self.assertEqual(item.getCategory(), "")
         self.assertEqual(item.getClassifier(), "")
         # a warning was added nevertheless
         self.assertEqual(response.json()['@warnings'],
-                         [IGNORE_VALIDATION_FOR_WARNING % "category, classifier"])
+                         [IGNORE_VALIDATION_FOR_WARNING %
+                          "category, classifier, groupsInCharge"])
         self.assertEqual(item.query_state(), "validated")
 
     def test_restapi_add_item_wf_transitions(self):
         """When creating an item, we may define "wf_transitions"."""
         cfg = self.meetingConfig
         self.changeUser("pmManager")
         endpoint_url = "{0}/@item".format(self.portal_url)
@@ -876,14 +886,47 @@
         self.assertEqual(annex1.file.contentType, "text/plain")
         self.assertEqual(
             annex2.file.filename, json["__children__"][1]["file"]["filename"]
         )
         self.assertEqual(annex2.file.size, 6475)
         self.assertEqual(annex2.file.contentType, "application/pdf")
 
+    def test_restapi_add_item_with_internal_number(self):
+        """When creating an item and using internal_number, it is correctly incremented."""
+        cfg = self.meetingConfig
+        set_settings({cfg.getItemTypeName(): {'u': False, 'nb': 5, 'expr': u'number'}})
+        transaction.commit()
+        self.changeUser("pmManager")
+        endpoint_url = "{0}/@item".format(self.portal_url)
+        json = {
+            "config_id": cfg.getId(),
+            "proposingGroup": self.developers.getId(),
+            "title": "My item",
+        }
+        self.api_session.post(endpoint_url, json=json)
+        transaction.begin()
+        pmFolder = self.getMeetingFolder()
+        item = pmFolder.objectValues()[-1]
+        self.assertEqual(item.internal_number, 5)
+        self.assertEqual(self.catalog(internal_number=5)[0].UID, item.UID())
+        # returned when using metadata_fields even if not a real field
+        # internal_number, not a real field, managed manually
+        endpoint_url = "{0}/@get?uid={1}" \
+            "&metadata_fields=internal_number".format(self.portal_url, item.UID())
+        response = self.api_session.get(endpoint_url)
+        self.assertEqual(response.status_code, 200, response.content)
+        resp_json = response.json()
+        self.assertEqual(resp_json["internal_number"], 5)
+        # also returned when using fullobjects
+        endpoint_url = endpoint_url.replace("&metadata_fields=internal_number", "&fullobjects")
+        response = self.api_session.get(endpoint_url)
+        self.assertEqual(response.status_code, 200, response.content)
+        resp_json = response.json()
+        self.assertEqual(resp_json["internal_number"], 5)
+
     def test_restapi_add_a_meeting_with_annexes(self):
         """When creating a meeting, we may add annexes as __children__,
            we may add several annexes at once."""
         cfg = self.meetingConfig
         self.changeUser("pmManager")
         endpoint_url = "{0}/@item".format(self.portal_url)
         json = {
```

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_users.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_users.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting/restapi/tests/test_services_search.py` & `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_search.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting.restapi.egg-info/PKG-INFO` & `plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plonemeeting.restapi
-Version: 2.0.1
+Version: 2.0.2
 Summary: Extended rest api service for Products.PloneMeeting usecases
 Home-page: https://pypi.python.org/pypi/plonemeeting.restapi
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -56,14 +56,23 @@
         
         Changelog
         =========
         
         Version 1.x is for PloneMeeting 4.1.x, version 2.x is for PloneMeeting 4.2.x+
         
         
+        2.0.2 (2023-05-31)
+        ------------------
+        
+        - Added `@attendees GET` on meeting and item and `@attendee GET/PATCH`
+          on meeting and item. Added `extra_include=attendees` on meeting and item.
+          [gbastien]
+        - Manage `metadata_fields=internal_number`.
+          [gbastien]
+        
         2.0.1 (2023-03-07)
         ------------------
         
         - Fixed test isolation problem when tests executed together with `imio.pm.ws` tests.
           [gbastien]
         
         2.0 (2023-03-06)
@@ -114,15 +123,15 @@
           Parameter `include_choices_for=field_name` may be given, in this case,
           a key `field_name__choices` is added to the result with `token/title` of
           the selectable values.
           [gbastien]
         - Refactored `@item extra_include=linked_items` to filter results using a
           catalog query so parameters and functionnality is similar to other endpoints.
           Removed `utils.filter_data` that could be dangerous and build a catalog query.
-          Formalized convienence catalog index names substitution (passing parameter `type`
+          Formalized convenience catalog index names substitution (passing parameter `type`
           corresponds to index `portal_type` or `state` corresponds to `review_state`).
           [gbastien]
         - Parameter `config_id` is no more required when using `in_name_of`
           in `@get` or `@search`.
           Added `bbb.py` to backport methods `get_filtered_plone_groups_for_user` and
           `getActiveConfigs` from `ToolPloneMeeting` so it is avaible when using
           `PloneMeeting 4.1.x`.
```

### Comparing `plonemeeting.restapi-2.0.1/src/plonemeeting.restapi.egg-info/SOURCES.txt` & `plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -48,32 +48,35 @@
 src/plonemeeting/restapi/serializer/annex.py
 src/plonemeeting/restapi/serializer/atfields.py
 src/plonemeeting/restapi/serializer/base.py
 src/plonemeeting/restapi/serializer/catalog.py
 src/plonemeeting/restapi/serializer/configure.zcml
 src/plonemeeting/restapi/serializer/converters.py
 src/plonemeeting/restapi/serializer/dxfields.py
+src/plonemeeting/restapi/serializer/held_position.py
 src/plonemeeting/restapi/serializer/item.py
 src/plonemeeting/restapi/serializer/meeting.py
 src/plonemeeting/restapi/serializer/meetingconfig.py
 src/plonemeeting/restapi/serializer/pod_template.py
 src/plonemeeting/restapi/serializer/summary.py
 src/plonemeeting/restapi/serializer/user.py
 src/plonemeeting/restapi/services/__init__.py
 src/plonemeeting/restapi/services/add.py
 src/plonemeeting/restapi/services/annex.py
+src/plonemeeting/restapi/services/attendees.py
 src/plonemeeting/restapi/services/configure.zcml
 src/plonemeeting/restapi/services/get.py
 src/plonemeeting/restapi/services/infos.py
 src/plonemeeting/restapi/services/meetingconfig.py
 src/plonemeeting/restapi/services/search.py
 src/plonemeeting/restapi/services/users.py
 src/plonemeeting/restapi/tests/__init__.py
 src/plonemeeting/restapi/tests/base.py
 src/plonemeeting/restapi/tests/config.py
 src/plonemeeting/restapi/tests/test_services_add.py
 src/plonemeeting/restapi/tests/test_services_annexes.py
+src/plonemeeting/restapi/tests/test_services_attendees.py
 src/plonemeeting/restapi/tests/test_services_get.py
 src/plonemeeting/restapi/tests/test_services_infos.py
 src/plonemeeting/restapi/tests/test_services_meetingconfig.py
 src/plonemeeting/restapi/tests/test_services_search.py
 src/plonemeeting/restapi/tests/test_services_users.py
```

### Comparing `plonemeeting.restapi-2.0.1/setup.py` & `plonemeeting.restapi-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 long_description = "\n\n".join(
     [open("README.rst").read(), open("CHANGES.rst").read(), ])
 
 
 setup(
     name="plonemeeting.restapi",
-    version="2.0.1",
+    version="2.0.2",
     description="Extended rest api service for Products.PloneMeeting usecases",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `plonemeeting.restapi-2.0.1/PKG-INFO` & `plonemeeting.restapi-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plonemeeting.restapi
-Version: 2.0.1
+Version: 2.0.2
 Summary: Extended rest api service for Products.PloneMeeting usecases
 Home-page: https://pypi.python.org/pypi/plonemeeting.restapi
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -56,14 +56,23 @@
         
         Changelog
         =========
         
         Version 1.x is for PloneMeeting 4.1.x, version 2.x is for PloneMeeting 4.2.x+
         
         
+        2.0.2 (2023-05-31)
+        ------------------
+        
+        - Added `@attendees GET` on meeting and item and `@attendee GET/PATCH`
+          on meeting and item. Added `extra_include=attendees` on meeting and item.
+          [gbastien]
+        - Manage `metadata_fields=internal_number`.
+          [gbastien]
+        
         2.0.1 (2023-03-07)
         ------------------
         
         - Fixed test isolation problem when tests executed together with `imio.pm.ws` tests.
           [gbastien]
         
         2.0 (2023-03-06)
@@ -114,15 +123,15 @@
           Parameter `include_choices_for=field_name` may be given, in this case,
           a key `field_name__choices` is added to the result with `token/title` of
           the selectable values.
           [gbastien]
         - Refactored `@item extra_include=linked_items` to filter results using a
           catalog query so parameters and functionnality is similar to other endpoints.
           Removed `utils.filter_data` that could be dangerous and build a catalog query.
-          Formalized convienence catalog index names substitution (passing parameter `type`
+          Formalized convenience catalog index names substitution (passing parameter `type`
           corresponds to index `portal_type` or `state` corresponds to `review_state`).
           [gbastien]
         - Parameter `config_id` is no more required when using `in_name_of`
           in `@get` or `@search`.
           Added `bbb.py` to backport methods `get_filtered_plone_groups_for_user` and
           `getActiveConfigs` from `ToolPloneMeeting` so it is avaible when using
           `PloneMeeting 4.1.x`.
```

### Comparing `plonemeeting.restapi-2.0.1/CHANGES.rst` & `plonemeeting.restapi-2.0.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 Changelog
 =========
 
 Version 1.x is for PloneMeeting 4.1.x, version 2.x is for PloneMeeting 4.2.x+
 
 
+2.0.2 (2023-05-31)
+------------------
+
+- Added `@attendees GET` on meeting and item and `@attendee GET/PATCH`
+  on meeting and item. Added `extra_include=attendees` on meeting and item.
+  [gbastien]
+- Manage `metadata_fields=internal_number`.
+  [gbastien]
+
 2.0.1 (2023-03-07)
 ------------------
 
 - Fixed test isolation problem when tests executed together with `imio.pm.ws` tests.
   [gbastien]
 
 2.0 (2023-03-06)
@@ -58,15 +67,15 @@
   Parameter `include_choices_for=field_name` may be given, in this case,
   a key `field_name__choices` is added to the result with `token/title` of
   the selectable values.
   [gbastien]
 - Refactored `@item extra_include=linked_items` to filter results using a
   catalog query so parameters and functionnality is similar to other endpoints.
   Removed `utils.filter_data` that could be dangerous and build a catalog query.
-  Formalized convienence catalog index names substitution (passing parameter `type`
+  Formalized convenience catalog index names substitution (passing parameter `type`
   corresponds to index `portal_type` or `state` corresponds to `review_state`).
   [gbastien]
 - Parameter `config_id` is no more required when using `in_name_of`
   in `@get` or `@search`.
   Added `bbb.py` to backport methods `get_filtered_plone_groups_for_user` and
   `getActiveConfigs` from `ToolPloneMeeting` so it is avaible when using
   `PloneMeeting 4.1.x`.
```

### Comparing `plonemeeting.restapi-2.0.1/README.rst` & `plonemeeting.restapi-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.1/LICENSE.GPL` & `plonemeeting.restapi-2.0.2/LICENSE.GPL`

 * *Files identical despite different names*

