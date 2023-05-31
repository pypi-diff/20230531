# Comparing `tmp/imio.restapi-1.0b1.tar.gz` & `tmp/imio.restapi-1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.restapi-1.0b1.tar", last modified: Mon Jan  3 12:46:29 2022, max compression
+gzip compressed data, was "dist/imio.restapi-1.0b2.tar", last modified: Wed May 31 08:58:24 2023, max compression
```

## Comparing `imio.restapi-1.0b1.tar` & `imio.restapi-1.0b2.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      657 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/LICENSE.rst
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio.restapi.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio.restapi.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      137 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio.restapi.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio.restapi.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio.restapi.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12327 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio.restapi.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3360 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio.restapi.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio.restapi.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      269 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio.restapi.egg-info/requires.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/settings/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      787 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/settings/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      612 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/settings/view.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2381 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/settings/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1663 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/settings/dataprovider.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/settings/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/form/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5984 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/form/tools.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7520 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/form/form.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      983 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/form/action.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      606 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/form/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4129 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/form/link.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/form/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      396 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/form/templates/action.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      119 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/form/templates/link.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      966 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/form/importer.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/form/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      589 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/setuphandlers.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/services/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1187 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/services/at.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2097 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/services/request_schema.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9809 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/services/add.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1399 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/services/transition.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4100 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/services/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2770 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/services/rest_link.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1696 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/services/uid.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2284 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/services/search.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2270 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/services/pod.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1115 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/services/update.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4569 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/services/infos.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/services/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1370 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      737 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/locales/imio.history.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2137 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/locales/imio.restapi.pot
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      535 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/locales/update.sh
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2019 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/locales/en/LC_MESSAGES/imio.restapi.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      682 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/locales/en/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      611 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/locales/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1320 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/locales/update.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2819 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/locales/fr/LC_MESSAGES/imio.restapi.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      689 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/locales/fr/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/locales/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/vocabularies/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      781 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/vocabularies/applications.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      368 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/vocabularies/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4973 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/vocabularies/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/vocabularies/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      162 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      182 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/profiles/default/registry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      118 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/profiles/default/rolemap.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/profiles/default/catalog.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      483 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/profiles/default/controlpanel.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/profiles/uninstall/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      122 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2993 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1761 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4035 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/serializer/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      414 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/serializer/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      875 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/serializer/rest_link.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3387 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/serializer/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/serializer/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5923 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/tests/test_service_transition.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3555 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/tests/test_service_infos.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3788 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/tests/test_service_pod.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1088 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/tests/test_service_search.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11979 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/tests/test_service_add.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2967 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/tests/test_service_update.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1917 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/tests/test_setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/upgrades.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      129 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      901 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1380 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/browser/viewlets.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/src/imio/restapi/browser/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      528 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/browser/templates/link-viewlet.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/browser/templates/action-viewlet.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      468 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/restapi/upgrades.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/src/imio/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       59 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/docs/index.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       39 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/requirements.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2253 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12327 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      127 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6685 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/CONTRIBUTORS.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2019 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2022-01-03 12:46:29.000000 imio.restapi-1.0b1/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      297 2022-01-03 12:46:28.000000 imio.restapi-1.0b1/DEVELOP.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      657 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/LICENSE.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio.restapi.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio.restapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      137 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio.restapi.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio.restapi.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio.restapi.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12564 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio.restapi.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3397 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio.restapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio.restapi.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      269 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio.restapi.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/settings/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      787 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/settings/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      612 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/settings/view.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2381 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/settings/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1663 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/settings/dataprovider.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/settings/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/form/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5984 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/form/tools.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7520 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/form/form.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      983 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/form/action.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      606 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/form/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4129 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/form/link.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/form/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      396 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/form/templates/action.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      119 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/form/templates/link.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      966 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/form/importer.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/form/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      589 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/setuphandlers.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1187 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/at.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2097 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/request_schema.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9809 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/add.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1399 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/transition.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4100 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2770 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/rest_link.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1696 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/uid.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2284 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/search.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2270 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/pod.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1115 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/update.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4569 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/infos.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/services/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1370 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      737 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/imio.history.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2137 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/imio.restapi.pot
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      535 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/update.sh
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2019 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/en/LC_MESSAGES/imio.restapi.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      682 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/en/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      611 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1320 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/update.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2819 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/fr/LC_MESSAGES/imio.restapi.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      689 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/fr/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/locales/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/vocabularies/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      781 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/vocabularies/applications.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      368 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/vocabularies/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4973 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/vocabularies/base.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/vocabularies/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      162 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      182 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/profiles/default/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      118 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/profiles/default/rolemap.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/profiles/default/catalog.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      483 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/profiles/default/controlpanel.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/profiles/uninstall/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      122 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2993 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1761 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4724 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/serializer/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      414 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/serializer/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      875 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/serializer/rest_link.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3387 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/serializer/base.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/serializer/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5923 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/tests/test_service_transition.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3555 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/tests/test_service_infos.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      754 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/tests/test_utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3788 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/tests/test_service_pod.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1088 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/tests/test_service_search.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11979 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/tests/test_service_add.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2967 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/tests/test_service_update.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1917 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/tests/test_setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/upgrades.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      129 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/browser/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      901 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/browser/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1380 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/browser/viewlets.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/browser/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      528 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/browser/templates/link-viewlet.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/browser/templates/action-viewlet.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      468 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/restapi/upgrades.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/src/imio/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       59 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/docs/index.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       39 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/requirements.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2253 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12564 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      127 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6866 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/CONTRIBUTORS.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2019 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      297 2023-05-31 08:58:24.000000 imio.restapi-1.0b2/DEVELOP.rst
```

### Comparing `imio.restapi-1.0b1/LICENSE.rst` & `imio.restapi-1.0b2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio.restapi.egg-info/PKG-INFO` & `imio.restapi-1.0b2/src/imio.restapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.restapi
-Version: 1.0b1
+Version: 1.0b2
 Summary: Extended rest api service for IMIO usecases
 Home-page: https://pypi.python.org/pypi/imio.restapi
 Author: Martin Peeters
 Author-email: martin.peeters@affinitic.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -80,14 +80,21 @@
         - Martin Peeters [Affinitic], Original author
         
         
         Changelog
         =========
         
         
+        1.0b2 (2023-05-31)
+        ------------------
+        
+        - Added helper `utils.serialize_term` that will serialize a vocabulary term
+          the same way it is done by the `FieldSerializer`.
+          [gbastien]
+        
         1.0b1 (2022-01-03)
         ------------------
         
         - In `FolderPost.do_reply` if an error occurs, do not continue,
           stop and return the result with the error immediately.
           [gbastien]
```

### Comparing `imio.restapi-1.0b1/src/imio.restapi.egg-info/SOURCES.txt` & `imio.restapi-1.0b2/src/imio.restapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -82,11 +82,12 @@
 src/imio/restapi/tests/test_service_add.py
 src/imio/restapi/tests/test_service_infos.py
 src/imio/restapi/tests/test_service_pod.py
 src/imio/restapi/tests/test_service_search.py
 src/imio/restapi/tests/test_service_transition.py
 src/imio/restapi/tests/test_service_update.py
 src/imio/restapi/tests/test_setup.py
+src/imio/restapi/tests/test_utils.py
 src/imio/restapi/vocabularies/__init__.py
 src/imio/restapi/vocabularies/applications.py
 src/imio/restapi/vocabularies/base.py
 src/imio/restapi/vocabularies/configure.zcml
```

### Comparing `imio.restapi-1.0b1/src/imio/restapi/settings/configure.zcml` & `imio.restapi-1.0b2/src/imio/restapi/settings/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/settings/view.py` & `imio.restapi-1.0b2/src/imio/restapi/settings/view.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/settings/interfaces.py` & `imio.restapi-1.0b2/src/imio/restapi/settings/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/settings/dataprovider.py` & `imio.restapi-1.0b2/src/imio/restapi/settings/dataprovider.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/form/tools.py` & `imio.restapi-1.0b2/src/imio/restapi/form/tools.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/form/form.py` & `imio.restapi-1.0b2/src/imio/restapi/form/form.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/form/action.py` & `imio.restapi-1.0b2/src/imio/restapi/form/action.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/form/configure.zcml` & `imio.restapi-1.0b2/src/imio/restapi/form/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/form/link.py` & `imio.restapi-1.0b2/src/imio/restapi/form/link.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/form/importer.py` & `imio.restapi-1.0b2/src/imio/restapi/form/importer.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/setuphandlers.py` & `imio.restapi-1.0b2/src/imio/restapi/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/services/at.py` & `imio.restapi-1.0b2/src/imio/restapi/services/at.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/services/request_schema.py` & `imio.restapi-1.0b2/src/imio/restapi/services/request_schema.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/services/add.py` & `imio.restapi-1.0b2/src/imio/restapi/services/add.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/services/transition.py` & `imio.restapi-1.0b2/src/imio/restapi/services/transition.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/services/configure.zcml` & `imio.restapi-1.0b2/src/imio/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/services/rest_link.py` & `imio.restapi-1.0b2/src/imio/restapi/services/rest_link.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/services/uid.py` & `imio.restapi-1.0b2/src/imio/restapi/services/uid.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/services/search.py` & `imio.restapi-1.0b2/src/imio/restapi/services/search.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/services/pod.py` & `imio.restapi-1.0b2/src/imio/restapi/services/pod.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/services/update.py` & `imio.restapi-1.0b2/src/imio/restapi/services/update.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/services/infos.py` & `imio.restapi-1.0b2/src/imio/restapi/services/infos.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/configure.zcml` & `imio.restapi-1.0b2/src/imio/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/locales/imio.history.pot` & `imio.restapi-1.0b2/src/imio/restapi/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/locales/imio.restapi.pot` & `imio.restapi-1.0b2/src/imio/restapi/locales/imio.restapi.pot`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/locales/update.sh` & `imio.restapi-1.0b2/src/imio/restapi/locales/update.sh`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/locales/en/LC_MESSAGES/imio.restapi.po` & `imio.restapi-1.0b2/src/imio/restapi/locales/en/LC_MESSAGES/imio.restapi.po`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/locales/en/LC_MESSAGES/imio.history.po` & `imio.restapi-1.0b2/src/imio/restapi/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/locales/README.rst` & `imio.restapi-1.0b2/src/imio/restapi/locales/README.rst`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/locales/update.py` & `imio.restapi-1.0b2/src/imio/restapi/locales/update.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/locales/fr/LC_MESSAGES/imio.restapi.po` & `imio.restapi-1.0b2/src/imio/restapi/locales/fr/LC_MESSAGES/imio.restapi.po`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/locales/fr/LC_MESSAGES/imio.history.po` & `imio.restapi-1.0b2/src/imio/restapi/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/vocabularies/applications.py` & `imio.restapi-1.0b2/src/imio/restapi/vocabularies/applications.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/vocabularies/base.py` & `imio.restapi-1.0b2/src/imio/restapi/vocabularies/base.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/testing.py` & `imio.restapi-1.0b2/src/imio/restapi/testing.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/interfaces.py` & `imio.restapi-1.0b2/src/imio/restapi/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/utils.py` & `imio.restapi-1.0b2/src/imio/restapi/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -128,7 +128,25 @@
 
 
 def listify(value):
     """Make sure value is a list."""
     if not hasattr(value, "__iter__"):
         value = [value]
     return value
+
+
+def serialize_term(tokens, vocab):
+    """Given a term p_values and a p_vocab, generate a serialized version
+       with {'token': p_token[0], 'value': term_value}.
+       This is useful when it is not a real field and we can not use a FieldSerializer."""
+    res = []
+    only_one = False
+    if isinstance(tokens, basestring):
+        only_one = True
+        tokens = [tokens]
+    for token in tokens:
+        res.append({'token': token, 'title': vocab.getTerm(token).title})
+    # if we receive one token, we return a dict, if we receive a list of tokens
+    # even if only one token in the list, we return a list of dicts
+    if res and only_one:
+        res = res[0]
+    return res
```

### Comparing `imio.restapi-1.0b1/src/imio/restapi/serializer/rest_link.py` & `imio.restapi-1.0b2/src/imio/restapi/serializer/rest_link.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/serializer/base.py` & `imio.restapi-1.0b2/src/imio/restapi/serializer/base.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/tests/test_service_transition.py` & `imio.restapi-1.0b2/src/imio/restapi/tests/test_service_transition.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/tests/test_service_infos.py` & `imio.restapi-1.0b2/src/imio/restapi/tests/test_service_infos.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/tests/test_service_pod.py` & `imio.restapi-1.0b2/src/imio/restapi/tests/test_service_pod.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/tests/test_service_search.py` & `imio.restapi-1.0b2/src/imio/restapi/tests/test_service_search.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/tests/test_service_add.py` & `imio.restapi-1.0b2/src/imio/restapi/tests/test_service_add.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/tests/test_service_update.py` & `imio.restapi-1.0b2/src/imio/restapi/tests/test_service_update.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/tests/test_setup.py` & `imio.restapi-1.0b2/src/imio/restapi/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/browser/configure.zcml` & `imio.restapi-1.0b2/src/imio/restapi/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/browser/viewlets.py` & `imio.restapi-1.0b2/src/imio/restapi/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/src/imio/restapi/browser/templates/link-viewlet.pt` & `imio.restapi-1.0b2/src/imio/restapi/browser/templates/link-viewlet.pt`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/setup.py` & `imio.restapi-1.0b2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.restapi",
-    version="1.0b1",
+    version="1.0b2",
     description="Extended rest api service for IMIO usecases",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 6 - Mature",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.restapi-1.0b1/PKG-INFO` & `imio.restapi-1.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.restapi
-Version: 1.0b1
+Version: 1.0b2
 Summary: Extended rest api service for IMIO usecases
 Home-page: https://pypi.python.org/pypi/imio.restapi
 Author: Martin Peeters
 Author-email: martin.peeters@affinitic.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -80,14 +80,21 @@
         - Martin Peeters [Affinitic], Original author
         
         
         Changelog
         =========
         
         
+        1.0b2 (2023-05-31)
+        ------------------
+        
+        - Added helper `utils.serialize_term` that will serialize a vocabulary term
+          the same way it is done by the `FieldSerializer`.
+          [gbastien]
+        
         1.0b1 (2022-01-03)
         ------------------
         
         - In `FolderPost.do_reply` if an error occurs, do not continue,
           stop and return the result with the error immediately.
           [gbastien]
```

### Comparing `imio.restapi-1.0b1/CHANGES.rst` & `imio.restapi-1.0b2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.0b2 (2023-05-31)
+------------------
+
+- Added helper `utils.serialize_term` that will serialize a vocabulary term
+  the same way it is done by the `FieldSerializer`.
+  [gbastien]
+
 1.0b1 (2022-01-03)
 ------------------
 
 - In `FolderPost.do_reply` if an error occurs, do not continue,
   stop and return the result with the error immediately.
   [gbastien]
```

### Comparing `imio.restapi-1.0b1/README.rst` & `imio.restapi-1.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0b1/LICENSE.GPL` & `imio.restapi-1.0b2/LICENSE.GPL`

 * *Files identical despite different names*

