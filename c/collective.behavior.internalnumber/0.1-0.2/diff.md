# Comparing `tmp/collective.behavior.internalnumber-0.1.tar.gz` & `tmp/collective.behavior.internalnumber-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.behavior.internalnumber-0.1.tar", last modified: Wed May 31 12:02:51 2017, max compression
+gzip compressed data, was "dist/collective.behavior.internalnumber-0.2.tar", last modified: Wed May 31 07:26:45 2023, max compression
```

## Comparing `collective.behavior.internalnumber-0.1.tar` & `collective.behavior.internalnumber-0.2.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/
--rw-rw-r--   0 sge       (1000) sge       (1000)      161 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     3404 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     1831 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1877 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       67 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)       63 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/CONTRIBUTORS.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       90 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/CHANGES.rst
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective.behavior.internalnumber.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective.behavior.internalnumber.egg-info/top_level.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      250 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective.behavior.internalnumber.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective.behavior.internalnumber.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)       31 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective.behavior.internalnumber.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       53 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective.behavior.internalnumber.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective.behavior.internalnumber.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)     2717 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective.behavior.internalnumber.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)     3404 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective.behavior.internalnumber.egg-info/PKG-INFO
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/
--rw-rw-r--   0 sge       (1000) sge       (1000)       80 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/
--rw-rw-r--   0 sge       (1000) sge       (1000)       80 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/
--rw-rw-r--   0 sge       (1000) sge       (1000)      558 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/testing.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2047 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/testing.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      916 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/subscribers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      736 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/setuphandlers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      282 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/interfaces.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1810 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     3500 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/behavior.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1050 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/adapters.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      296 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2506 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/test_subscribers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2468 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/test_setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2078 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/test_settings.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      931 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/test_robot.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     4782 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/test_behavior.py
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/robot/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2067 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/robot/test_example.robot
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/uninstall/
--rw-rw-r--   0 sge       (1000) sge       (1000)      144 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/testing/
--rw-rw-r--   0 sge       (1000) sge       (1000)      227 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/testing/types.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      183 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/testing/metadata.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/testing/types/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1984 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/testing/types/testtype.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/default/
--rw-rw-r--   0 sge       (1000) sge       (1000)      127 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/default/registry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      266 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/default/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      578 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/default/controlpanel.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      226 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/default/catalog.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      227 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/default/browserlayer.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/locales/
--rwxrwxr-x   0 sge       (1000) sge       (1000)      539 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/locales/update.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)     2115 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/locales/collective.behavior.internalnumber.pot
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/locales/fr/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2463 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/locales/fr/LC_MESSAGES/collective.behavior.internalnumber.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/browser/
--rw-rw-r--   0 sge       (1000) sge       (1000)     3360 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/browser/settings.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      708 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/browser/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/browser/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/browser/static/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/browser/static/.gitkeep
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)       97 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/docs/index.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      681 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/docs/LICENSE.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2017-05-31 12:02:51.000000 collective.behavior.internalnumber-0.1/docs/LICENSE.GPL
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1262 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/setuphandlers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1942 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1250 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/adapters.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2115 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/locales/collective.behavior.internalnumber.pot
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      539 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/locales/update.sh
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2463 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/locales/fr/LC_MESSAGES/collective.behavior.internalnumber.po
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/testing/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/testing/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1984 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/testing/types/testtype.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      227 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/testing/types.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      227 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      266 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      127 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/default/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      226 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/default/catalog.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      578 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/default/controlpanel.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/uninstall/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      144 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2047 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3699 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/behavior.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      282 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      560 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/testing.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/robot/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2067 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/robot/test_example.robot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2602 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/test_subscribers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6176 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/test_settings.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4954 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/test_behavior.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      931 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/test_robot.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2997 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/test_setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      286 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/subscribers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      444 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/browser/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/browser/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/browser/static/.gitkeep
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      878 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/browser/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6187 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/browser/settings.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/behavior/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective.behavior.internalnumber.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective.behavior.internalnumber.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective.behavior.internalnumber.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       31 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective.behavior.internalnumber.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective.behavior.internalnumber.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4975 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective.behavior.internalnumber.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2789 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective.behavior.internalnumber.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective.behavior.internalnumber.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      250 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/src/collective.behavior.internalnumber.egg-info/requires.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       85 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/requirements-6.0.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      681 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/docs/LICENSE.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       97 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/docs/index.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2098 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4975 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       91 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/requirements-5.2.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       98 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      588 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       63 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/CONTRIBUTORS.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2448 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3054 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/Makefile
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      140 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       65 2023-05-31 07:26:45.000000 collective.behavior.internalnumber-0.2/requirements-4.3.txt
```

### Comparing `collective.behavior.internalnumber-0.1/setup.py` & `collective.behavior.internalnumber-0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,24 +10,30 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='collective.behavior.internalnumber',
-    version='0.1',
+    version='0.2',
     description="Configurable internal number plone behavior",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
+        "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
+        "Framework :: Plone :: Addon",
         "Framework :: Plone :: 4.3",
+        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords='Python Plone',
     author='Stephan Geulette',
     author_email='support@imio.be',
     url='https://pypi.python.org/pypi/collective.behavior.internalnumber',
```

### Comparing `collective.behavior.internalnumber-0.1/README.rst` & `collective.behavior.internalnumber-0.2/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
+.. image:: https://github.com/IMIO/collective.behavior.internalnumber/actions/workflows/main.yml/badge.svg?branch=master
+    :target: https://github.com/IMIO/collective.behavior.internalnumber/actions/workflows/main.yml
+
+.. image:: https://coveralls.io/repos/github/IMIO/collective.behavior.internalnumber/badge.svg
+    :target: https://coveralls.io/github/IMIO/collective.behavior.internalnumber
+
+.. image:: http://img.shields.io/pypi/v/collective.behavior.internalnumber.svg
+   :alt: PyPI badge
+   :target: https://pypi.org/project/collective.behavior.internalnumber
+
+
 ==============================================================================
 collective.behavior.internalnumber
 ==============================================================================
 
 This product adds a plone behavior for dexterity content.
 The behavior adds a text field containing an internal number.
```

### Comparing `collective.behavior.internalnumber-0.1/src/collective.behavior.internalnumber.egg-info/SOURCES.txt` & `collective.behavior.internalnumber-0.2/src/collective.behavior.internalnumber.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 CHANGES.rst
 CONTRIBUTORS.rst
 MANIFEST.in
+Makefile
 README.rst
+requirements-4.3.txt
+requirements-5.2.txt
+requirements-6.0.txt
 setup.cfg
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.rst
 docs/index.rst
 src/collective/__init__.py
 src/collective.behavior.internalnumber.egg-info/PKG-INFO
```

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/testing.zcml` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/testing.zcml`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
-    i18n_domain="collective.behavior.talcondition">
+    i18n_domain="collective.behavior.internalnumber">
 
   <include file="configure.zcml" />
   <include package="plone.app.dexterity" />
 
   <genericsetup:registerProfile
       name="testing"
       title="collective.behavior.internalnumber tests"
```

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/testing.py` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/testing.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/configure.zcml` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/configure.zcml`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,17 @@
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:i18n="http://namespaces.zope.org/i18n"
     xmlns:plone="http://namespaces.plone.org/plone"
     i18n_domain="collective.behavior.internalnumber">
 
   <i18n:registerTranslations directory="locales" />
 
-  <includeDependencies package="." />
+  <include package="collective.behavior.talcondition" />
+  <include package="collective.dexteritytextindexer" />
+  <include package="collective.z3cform.datagridfield" />
 
   <include package="plone.behavior" file="meta.zcml" />
 
   <include package=".browser" />
 
   <plone:behavior
       title="Internal number field"
```

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/behavior.py` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/behavior.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 
-from zope import component
-from zope import schema
-from zope.interface import alsoProvides, Invalid
-from z3c.form import validator, widget
-
+from collective.behavior.internalnumber import _
+from collective.behavior.internalnumber.browser.settings import get_pt_settings
+from collective.behavior.talcondition.utils import _evaluateExpression
 from plone import api
 from plone.autoform.interfaces import IFormFieldProvider
 from plone.supermodel import model
-
 from Products.CMFPlone.utils import safe_unicode
-from collective.behavior.talcondition.utils import _evaluateExpression
-
-from . import _
-from browser.settings import get_pt_settings
+from z3c.form import validator
+from z3c.form import widget
+from zope import component
+from zope import schema
+from zope.interface import alsoProvides
+from zope.interface import Invalid
 
 
 class IInternalNumberBehavior(model.Schema):
 
     internal_number = schema.TextLine(
         title=_(u"Internal number"),
         required=False,)
 
+
 alsoProvides(IInternalNumberBehavior, IFormFieldProvider)
 
 
 def validateIndexValueUniqueness(context, portal_type, index_name, value):
     """
         check at 'portal_type' 'context' creation if 'index' 'value' is uniqueness
     """
@@ -66,16 +66,19 @@
 component.provideAdapter(InternalNumberValidator)
 
 
 # To avoid grokking the package required by plone.directives.form.default_value decorator
 
 def internal_number_default(data):
     """ Default value of internal_number """
+    if data.view is None or not hasattr(data.view, 'portal_type'):
+        return u''
     settings = get_pt_settings(data.view.portal_type)
     ret = _evaluateExpression(data.context, settings.get('expr', ''), extra_expr_ctx={'number': settings.get('nb', 0)},
                               empty_expr_is_true='')
     return ret
 
+
 DefaultinternalNumber = widget.ComputedWidgetAttribute(internal_number_default,
                                                        field=IInternalNumberBehavior['internal_number'])
 
 component.provideAdapter(DefaultinternalNumber, name='default')
```

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/adapters.py` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/adapters.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # -*- coding: utf-8 -*-
 
-from zope.component import adapts
-from zope.interface import implements
-
+from collective.behavior.internalnumber.behavior import IInternalNumberBehavior
+from collective.dexteritytextindexer.interfaces import IDynamicTextIndexExtender
 from plone.indexer import indexer
 from Products.CMFCore.interfaces import IContentish
-from Products.CMFPlone.utils import base_hasattr, safe_unicode
-from Products.PluginIndexes.common.UnIndex import _marker as common_marker
+from Products.CMFPlone.utils import base_hasattr
+from Products.CMFPlone.utils import safe_unicode
+from zope.component import adapts
+from zope.interface import implementer
 
-from collective import dexteritytextindexer
 
-from .behavior import IInternalNumberBehavior
+try:
+    from Products.PluginIndexes.common.UnIndex import _marker as common_marker  # noqa
+except ImportError:
+    from Products.PluginIndexes.unindex import _marker as common_marker  # noqa
 
 
 @indexer(IContentish)
 def internal_number_index(obj):
     """ Index method escaping acquisition and ready for ZCatalog 3 """
     if base_hasattr(obj, 'internal_number') and obj.internal_number:
         return obj.internal_number
     return common_marker
 
 
+@implementer(IDynamicTextIndexExtender)
 class InternalNumberSearchableExtender(object):
     """
         Extends SearchableText of IInternalNumberBehavior objects.
     """
     adapts(IInternalNumberBehavior)
-    implements(dexteritytextindexer.IDynamicTextIndexExtender)
 
     def __init__(self, context):
         self.context = context
 
     def __call__(self):
         return safe_unicode(self.context.internal_number)
```

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/test_subscribers.py` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/test_subscribers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # -*- coding: utf-8 -*-
 
-import unittest
-
-from plone import api
-
+from collective.behavior.internalnumber import TYPE_CONFIG
+from collective.behavior.internalnumber.browser.settings import get_pt_settings
+from collective.behavior.internalnumber.subscribers import object_added
 from collective.behavior.internalnumber.testing import COLLECTIVE_BEHAVIOR_INTERNALNUMBER_INTEGRATION_TESTING  # noqa
+from plone import api
 
-from .. import TYPE_CONFIG
-from ..browser.settings import get_pt_settings
-from ..subscribers import object_added
+import unittest
 
 
 class TestSubscribers(unittest.TestCase):
     """Test settings."""
 
     layer = COLLECTIVE_BEHAVIOR_INTERNALNUMBER_INTEGRATION_TESTING
```

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/test_setup.py` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/test_setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,70 @@
 # -*- coding: utf-8 -*-
 """Setup tests for this package."""
+from collective.behavior.internalnumber import PLONE_VERSION
+from collective.behavior.internalnumber import TYPE_CONFIG
+from collective.behavior.internalnumber.testing import COLLECTIVE_BEHAVIOR_INTERNALNUMBER_INTEGRATION_TESTING
+from plone import api
+from zope.schema._bootstrapinterfaces import WrongType
+
 import unittest
 
-from zope.schema._bootstrapinterfaces import WrongType
 
-from collective.behavior.internalnumber.testing import COLLECTIVE_BEHAVIOR_INTERNALNUMBER_INTEGRATION_TESTING  # noqa
-from plone import api
+class CommonSetup():  # noqa
 
-from .. import TYPE_CONFIG
+    def set_installer(self):
+        if PLONE_VERSION >= '5.1':
+            from Products.CMFPlone.utils import get_installer  # noqa
+            self.installer = get_installer(self.portal, self.layer["request"])
+            self.ipi = self.installer.is_product_installed
+        else:
+            self.installer = api.portal.get_tool('portal_quickinstaller')  # noqa
+            self.ipi = self.installer.isProductInstalled
 
 
-class TestSetup(unittest.TestCase):
+class TestSetup(unittest.TestCase, CommonSetup):
     """Test that collective.behavior.internalnumber is properly installed."""
 
     layer = COLLECTIVE_BEHAVIOR_INTERNALNUMBER_INTEGRATION_TESTING
 
     def setUp(self):
         """Custom shared utility setup for tests."""
         self.portal = self.layer['portal']
-        self.installer = api.portal.get_tool('portal_quickinstaller')
+        self.set_installer()
 
     def test_product_installed(self):
         """Test if collective.behavior.internalnumber is installed."""
-        self.assertTrue(self.installer.isProductInstalled(
-            'collective.behavior.internalnumber'))
+        self.assertTrue(self.ipi('collective.behavior.internalnumber'))
 
     def test_browserlayer(self):
         """Test that ICollectiveBehaviorInternalnumberLayer is registered."""
-        from collective.behavior.internalnumber.interfaces import (
-            ICollectiveBehaviorInternalnumberLayer)
+        from collective.behavior.internalnumber.interfaces import ICollectiveBehaviorInternalnumberLayer
         from plone.browserlayer import utils
         self.assertIn(ICollectiveBehaviorInternalnumberLayer, utils.registered_layers())
 
     def test_registry(self):
         self.assertRaises(api.exc.InvalidParameterError, api.portal.set_registry_record, 'Unexistent key', True)
         self.assertRaises(WrongType, api.portal.set_registry_record, TYPE_CONFIG, 'string')
         api.portal.set_registry_record(TYPE_CONFIG, [])
 
 
-class TestUninstall(unittest.TestCase):
+class TestUninstall(unittest.TestCase, CommonSetup):
 
     layer = COLLECTIVE_BEHAVIOR_INTERNALNUMBER_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer['portal']
-        self.installer = api.portal.get_tool('portal_quickinstaller')
-        self.installer.uninstallProducts(['collective.behavior.internalnumber'])
+        self.set_installer()
+        if PLONE_VERSION >= '5.1':
+            self.installer.uninstall_product('collective.behavior.internalnumber')
+        else:
+            self.installer.uninstallProducts(['collective.behavior.internalnumber'])
 
     def test_product_uninstalled(self):
         """Test if collective.behavior.internalnumber is cleanly uninstalled."""
-        self.assertFalse(self.installer.isProductInstalled(
-            'collective.behavior.internalnumber'))
+        self.assertFalse(self.ipi('collective.behavior.internalnumber'))
 
     def test_browserlayer_removed(self):
         """Test that ICollectiveBehaviorInternalnumberLayer is removed."""
         from collective.behavior.internalnumber.interfaces import ICollectiveBehaviorInternalnumberLayer
         from plone.browserlayer import utils
         self.assertNotIn(ICollectiveBehaviorInternalnumberLayer, utils.registered_layers())
```

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/test_robot.py` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/test_behavior.py` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/test_behavior.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
 
-import unittest
-
-from zope.component import getUtility
-from zope.interface import Invalid
-
+from collective.behavior.internalnumber import TYPE_CONFIG
+from collective.behavior.internalnumber.behavior import internal_number_default
+from collective.behavior.internalnumber.behavior import InternalNumberValidator
+from collective.behavior.internalnumber.behavior import validateIndexValueUniqueness
+from collective.behavior.internalnumber.testing import COLLECTIVE_BEHAVIOR_INTERNALNUMBER_INTEGRATION_TESTING  # noqa
 from plone import api
 from plone.dexterity.interfaces import IDexterityFTI
+from zope.component import getUtility
+from zope.interface import Invalid
 
-from collective.behavior.internalnumber.testing import COLLECTIVE_BEHAVIOR_INTERNALNUMBER_INTEGRATION_TESTING  # noqa
-
-from .. import TYPE_CONFIG
-from ..behavior import validateIndexValueUniqueness, InternalNumberValidator, internal_number_default
+import unittest
 
 
 class TestBehavior(unittest.TestCase):
     """Test behavior."""
 
     layer = COLLECTIVE_BEHAVIOR_INTERNALNUMBER_INTEGRATION_TESTING
```

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/tests/robot/test_example.robot` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/testing/types/testtype.xml` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/testing/types/testtype.xml`

 * *Files identical despite different names*

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/profiles/default/controlpanel.xml` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/locales/update.sh` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/locales/collective.behavior.internalnumber.pot` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/locales/collective.behavior.internalnumber.pot`

 * *Files identical despite different names*

### Comparing `collective.behavior.internalnumber-0.1/src/collective/behavior/internalnumber/locales/fr/LC_MESSAGES/collective.behavior.internalnumber.po` & `collective.behavior.internalnumber-0.2/src/collective/behavior/internalnumber/locales/fr/LC_MESSAGES/collective.behavior.internalnumber.po`

 * *Files identical despite different names*

### Comparing `collective.behavior.internalnumber-0.1/docs/LICENSE.rst` & `collective.behavior.internalnumber-0.2/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.behavior.internalnumber-0.1/docs/LICENSE.GPL` & `collective.behavior.internalnumber-0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

