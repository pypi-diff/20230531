# Comparing `tmp/collective.auditlog-2.0.0a1.tar.gz` & `tmp/collective.auditlog-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.auditlog-2.0.0a1.tar", last modified: Wed Mar 11 12:28:55 2020, max compression
+gzip compressed data, was "dist/collective.auditlog-2.0.0a2.tar", last modified: Thu Mar 19 14:32:44 2020, max compression
```

## Comparing `collective.auditlog-2.0.0a1.tar` & `collective.auditlog-2.0.0a2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/
--rw-rw-r--   0 ale       (1000) ale       (1000)       63 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/MANIFEST.in
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective.auditlog.egg-info/
--rw-rw-r--   0 ale       (1000) ale       (1000)    13750 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective.auditlog.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)       11 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective.auditlog.egg-info/namespace_packages.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective.auditlog.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1815 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective.auditlog.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      152 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective.auditlog.egg-info/entry_points.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective.auditlog.egg-info/not-zip-safe
--rw-rw-r--   0 ale       (1000) ale       (1000)      160 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective.auditlog.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)       11 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective.auditlog.egg-info/top_level.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)    13750 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     1587 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/setup.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2169 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/CHANGES.rst
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective/
--rw-rw-r--   0 ale       (1000) ale       (1000)       56 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective/auditlog/
--rw-rw-r--   0 ale       (1000) ale       (1000)     3879 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/catalog.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective/auditlog/tests/
--rw-rw-r--   0 ale       (1000) ale       (1000)     5725 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/tests/test_actions.py
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/tests/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2651 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/browser.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3958 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/td.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      855 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/models.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      336 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/tasks.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      326 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/permissions.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     4339 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     1302 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/controlpanel.pt
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective/auditlog/upgrades/
--rw-rw-r--   0 ale       (1000) ale       (1000)      326 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/upgrades/to1001.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1957 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/upgrades/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)       15 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/upgrades/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1126 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3705 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/handlers.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      399 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/profiles.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     1121 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/asyncqueue.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4487 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/utils.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective/auditlog/locales/
--rw-rw-r--   0 ale       (1000) ale       (1000)     1237 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/locales/collective.auditlog.pot
--rw-rw-r--   0 ale       (1000) ale       (1000)     1060 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/action.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     4123 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/logview.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)     2183 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/controlpanel.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1853 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/db.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective/auditlog/static/
--rw-rw-r--   0 ale       (1000) ale       (1000)    37031 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/static/infinitescroll.jquery.js
--rw-rw-r--   0 ale       (1000) ale       (1000)      330 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/permissions.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4978 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/interfaces.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1293 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/testing.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective/auditlog/profiles/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/collective/auditlog/profiles/default/
--rw-rw-r--   0 ale       (1000) ale       (1000)      170 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/profiles/default/metadata.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      355 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/profiles/default/rolemap.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      554 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/profiles/default/controlpanel.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      153 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/profiles/default/toolset.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)     7436 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/profiles/default/contentrules.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      819 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/profiles/default/actions.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      120 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/profiles/default/registry.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)     8580 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/collective/auditlog/action.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/docs/
--rw-rw-r--   0 ale       (1000) ale       (1000)      736 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/docs/LICENSE.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1504 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/docs/INSTALL.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)    17987 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/docs/LICENSE.GPL
--rw-rw-r--   0 ale       (1000) ale       (1000)      435 2020-03-11 12:28:55.000000 collective.auditlog-2.0.0a1/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     8178 2020-03-11 12:28:54.000000 collective.auditlog-2.0.0a1/README.rst
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       63 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/MANIFEST.in
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    13932 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)       11 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/namespace_packages.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1815 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      152 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/entry_points.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/not-zip-safe
+-rw-rw-r--   0 ale       (1000) ale       (1000)      160 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       11 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/top_level.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)    13932 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1576 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/setup.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2295 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/CHANGES.rst
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       56 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3879 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/catalog.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/tests/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5725 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/tests/test_actions.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/tests/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2651 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/browser.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3958 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/td.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      855 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/models.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      336 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/tasks.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      326 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/permissions.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4339 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1302 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/controlpanel.pt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/upgrades/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      326 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/upgrades/to1001.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1957 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/upgrades/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)       15 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/upgrades/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1126 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3705 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/handlers.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      399 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1121 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/asyncqueue.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4501 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/utils.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/locales/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1237 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/locales/collective.auditlog.pot
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1060 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/action.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4123 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/logview.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2183 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/controlpanel.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1853 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/db.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/static/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    37031 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/static/infinitescroll.jquery.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)      330 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/permissions.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4978 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/interfaces.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1293 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/testing.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      170 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/metadata.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      355 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/rolemap.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      554 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/controlpanel.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      153 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/toolset.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7436 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/contentrules.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      819 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/actions.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      120 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/registry.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8638 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/action.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/docs/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      736 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/docs/LICENSE.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1504 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/docs/INSTALL.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17987 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/docs/LICENSE.GPL
+-rw-rw-r--   0 ale       (1000) ale       (1000)      435 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8178 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/README.rst
```

### Comparing `collective.auditlog-2.0.0a1/collective.auditlog.egg-info/PKG-INFO` & `collective.auditlog-2.0.0a2/collective.auditlog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.auditlog
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Provides extra conditions and triggers for all content actions
 Home-page: http://svn.plone.org/svn/collective/
 Author: rain2o
 Author-email: Joel@rain2odesigns.com
 License: GPL
 Description: Introduction
         ============
@@ -223,14 +223,21 @@
         - Alessandro Pisa, bug fixing, testing
         - Enfold Systems, celery integration and audit view
         
         
         Changelog
         =========
         
+        2.0.0a2 (2020-03-19)
+        --------------------
+        
+        - Fix request not having an environment attribute in instance scripts
+          [ale-rt]
+        
+        
         2.0.0a1 (2020-03-11)
         --------------------
         
         - Remove inconsistent passing of ``request`` parameter and use zope.globalrequest instead.
           [thet]
         
         - Remove deprecations.
```

### Comparing `collective.auditlog-2.0.0a1/collective.auditlog.egg-info/SOURCES.txt` & `collective.auditlog-2.0.0a2/collective.auditlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/PKG-INFO` & `collective.auditlog-2.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.auditlog
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Provides extra conditions and triggers for all content actions
 Home-page: http://svn.plone.org/svn/collective/
 Author: rain2o
 Author-email: Joel@rain2odesigns.com
 License: GPL
 Description: Introduction
         ============
@@ -223,14 +223,21 @@
         - Alessandro Pisa, bug fixing, testing
         - Enfold Systems, celery integration and audit view
         
         
         Changelog
         =========
         
+        2.0.0a2 (2020-03-19)
+        --------------------
+        
+        - Fix request not having an environment attribute in instance scripts
+          [ale-rt]
+        
+        
         2.0.0a1 (2020-03-11)
         --------------------
         
         - Remove inconsistent passing of ``request`` parameter and use zope.globalrequest instead.
           [thet]
         
         - Remove deprecations.
```

### Comparing `collective.auditlog-2.0.0a1/setup.py` & `collective.auditlog-2.0.0a2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # coding=utf-8
 from setuptools import find_packages
 from setuptools import setup
 
-import os
 
-
-version = "2.0.0a1"
+version = "2.0.0a2"
 
 
 long_description = "\n\n".join([open("README.rst").read(), open("CHANGES.rst").read(),])
 
 
 setup(
     name="collective.auditlog",
```

### Comparing `collective.auditlog-2.0.0a1/CHANGES.rst` & `collective.auditlog-2.0.0a2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.0.0a2 (2020-03-19)
+--------------------
+
+- Fix request not having an environment attribute in instance scripts
+  [ale-rt]
+
+
 2.0.0a1 (2020-03-11)
 --------------------
 
 - Remove inconsistent passing of ``request`` parameter and use zope.globalrequest instead.
   [thet]
 
 - Remove deprecations.
```

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/catalog.py` & `collective.auditlog-2.0.0a2/collective/auditlog/catalog.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/tests/test_actions.py` & `collective.auditlog-2.0.0a2/collective/auditlog/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/browser.py` & `collective.auditlog-2.0.0a2/collective/auditlog/browser.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/td.py` & `collective.auditlog-2.0.0a2/collective/auditlog/td.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/models.py` & `collective.auditlog-2.0.0a2/collective/auditlog/models.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/configure.zcml` & `collective.auditlog-2.0.0a2/collective/auditlog/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/controlpanel.pt` & `collective.auditlog-2.0.0a2/collective/auditlog/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/upgrades/configure.zcml` & `collective.auditlog-2.0.0a2/collective/auditlog/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/__init__.py` & `collective.auditlog-2.0.0a2/collective/auditlog/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/handlers.py` & `collective.auditlog-2.0.0a2/collective/auditlog/handlers.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/asyncqueue.py` & `collective.auditlog-2.0.0a2/collective/auditlog/asyncqueue.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/utils.py` & `collective.auditlog-2.0.0a2/collective/auditlog/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,20 +54,21 @@
 
 
 def getHostname():
     """
     stolen from the developer manual
     """
     request = getRequest()
-    if "HTTP_X_FORWARDED_HOST" in request.environ:
+    environ = getattr(request, "environ", {})
+    if "HTTP_X_FORWARDED_HOST" in environ:
         # Virtual host
-        host = request.environ["HTTP_X_FORWARDED_HOST"]
-    elif "HTTP_HOST" in request.environ:
+        host = environ["HTTP_X_FORWARDED_HOST"]
+    elif "HTTP_HOST" in environ:
         # Direct client request
-        host = request.environ["HTTP_HOST"]
+        host = environ["HTTP_HOST"]
     else:
         return None
 
     # separate to domain name and port sections
     host = host.split(":")[0].lower()
 
     return host
```

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/locales/collective.auditlog.pot` & `collective.auditlog-2.0.0a2/collective/auditlog/locales/collective.auditlog.pot`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/action.zcml` & `collective.auditlog-2.0.0a2/collective/auditlog/action.zcml`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/logview.pt` & `collective.auditlog-2.0.0a2/collective/auditlog/logview.pt`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/controlpanel.py` & `collective.auditlog-2.0.0a2/collective/auditlog/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/db.py` & `collective.auditlog-2.0.0a2/collective/auditlog/db.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/static/infinitescroll.jquery.js` & `collective.auditlog-2.0.0a2/collective/auditlog/static/infinitescroll.jquery.js`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/interfaces.py` & `collective.auditlog-2.0.0a2/collective/auditlog/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/testing.py` & `collective.auditlog-2.0.0a2/collective/auditlog/testing.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/profiles/default/controlpanel.xml` & `collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/profiles/default/contentrules.xml` & `collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/contentrules.xml`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/profiles/default/actions.xml` & `collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/collective/auditlog/action.py` & `collective.auditlog-2.0.0a2/collective/auditlog/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,16 @@
             if isinstance(rule, RuleExecutable):
                 return rule
             frame = frame.f_back
         return None
 
     @property
     def can_execute(self):
-        if self.request.environ.get("disable.auditlog", False):
+        environ = getattr(self.request, "environ", {})
+        if environ.get("disable.auditlog", False):
             return False
 
         event = self.event
         event_iface = next(event.__implemented__.interfaces())
 
         rule = self.rule
         if rule and event_iface != rule.rule.event:
@@ -122,14 +123,15 @@
     @memoize
     def getLogEntry(self):
         """ Get's a log entry for your action
         """
         event = self.event
         obj = event.object
         data = {"info": ""}
+        environ = getattr(self.request, "environ", {})
 
         # the order of those interface checks matters since some interfaces
         # inherit from others
         if IObjectRemovedEvent.providedBy(event):
             # need to keep track of removed events so it doesn't get called
             # more than once for each object
             action = "removed"
@@ -165,23 +167,23 @@
             action = "workflow"
         elif IObjectClonedEvent.providedBy(event):
             action = "copied"
         elif ICheckinEvent.providedBy(event):
             info = {"message": event.message}
             data["info"] = json.dumps(info)
             action = "checked in"
-            self.request.environ["disable.auditlog"] = True
+            environ["disable.auditlog"] = True
             data["working_copy"] = "/".join(obj.getPhysicalPath())
             obj = event.baseline
         elif IBeforeCheckoutEvent.providedBy(event):
             action = "checked out"
-            self.request.environ["disable.auditlog"] = True
+            environ["disable.auditlog"] = True
         elif ICancelCheckoutEvent.providedBy(event):
             action = "cancel check out"
-            self.request.environ["disable.auditlog"] = True
+            environ["disable.auditlog"] = True
             data["working_copy"] = "/".join(obj.getPhysicalPath())
             obj = event.baseline
         elif IUserLoggedInEvent.providedBy(event):
             action = "logged in"
             info = {"user": event.object.getUserName()}
             data["info"] = json.dumps(info)
         elif IUserLoggedOutEvent.providedBy(event):
```

### Comparing `collective.auditlog-2.0.0a1/docs/LICENSE.txt` & `collective.auditlog-2.0.0a2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/docs/INSTALL.txt` & `collective.auditlog-2.0.0a2/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/docs/LICENSE.GPL` & `collective.auditlog-2.0.0a2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a1/README.rst` & `collective.auditlog-2.0.0a2/README.rst`

 * *Files identical despite different names*

