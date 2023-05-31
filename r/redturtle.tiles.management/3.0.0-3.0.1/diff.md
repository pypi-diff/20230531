# Comparing `tmp/redturtle.tiles.management-3.0.0.tar.gz` & `tmp/redturtle.tiles.management-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.tiles.management-3.0.0.tar", last modified: Fri Sep 16 15:10:28 2022, max compression
+gzip compressed data, was "redturtle.tiles.management-3.0.1.tar", last modified: Wed May 31 15:02:36 2023, max compression
```

## Comparing `redturtle.tiles.management-3.0.0.tar` & `redturtle.tiles.management-3.0.1.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.782776 redturtle.tiles.management-3.0.0/
--rw-r--r--   0 pieronicolli   (501) staff       (20)       75 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/.coveragerc
--rw-r--r--   0 pieronicolli   (501) staff       (20)      245 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/.editorconfig
--rw-r--r--   0 pieronicolli   (501) staff       (20)       23 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/.gitattributes
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4359 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/CHANGES.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)       51 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/CONTRIBUTORS.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2981 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/Gruntfile.js
--rw-r--r--   0 pieronicolli   (501) staff       (20)      361 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/MANIFEST.in
--rw-r--r--   0 pieronicolli   (501) staff       (20)     9283 2022-09-16 15:10:28.782838 redturtle.tiles.management-3.0.0/PKG-INFO
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4102 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/README.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1945 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/base.cfg
--rw-r--r--   0 pieronicolli   (501) staff       (20)       61 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/bobtemplate.cfg
--rw-r--r--   0 pieronicolli   (501) staff       (20)      162 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/buildout.cfg
--rw-r--r--   0 pieronicolli   (501) staff       (20)       27 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/constraints.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)       39 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/constraints_plone51.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)       39 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/constraints_plone52.txt
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.775602 redturtle.tiles.management-3.0.0/docs/
--rw-r--r--   0 pieronicolli   (501) staff       (20)    18092 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/docs/LICENSE.GPL
--rw-r--r--   0 pieronicolli   (501) staff       (20)      677 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/docs/LICENSE.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)       89 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/docs/index.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)    83959 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/package-lock.json
--rw-r--r--   0 pieronicolli   (501) staff       (20)      702 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/package.json
--rw-r--r--   0 pieronicolli   (501) staff       (20)       50 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/requirements.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      270 2022-09-16 15:10:28.783095 redturtle.tiles.management-3.0.0/setup.cfg
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1934 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/setup.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.771880 redturtle.tiles.management-3.0.0/src/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.775700 redturtle.tiles.management-3.0.0/src/redturtle/
--rw-r--r--   0 pieronicolli   (501) staff       (20)       80 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/__init__.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.776620 redturtle.tiles.management-3.0.0/src/redturtle/tiles/
--rw-r--r--   0 pieronicolli   (501) staff       (20)       80 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/__init__.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.777447 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1237 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/__init__.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.778447 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      378 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/add.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4397 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      685 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/controlpanel.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2805 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/delete.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      842 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/edit.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.778745 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/overrides/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/overrides/.gitkeep
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1107 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/overrides/plone.app.tiles.browser.add.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      282 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/overrides/plone.app.tiles.browser.tileformlayout.pt
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.780075 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/.gitkeep
--rw-r--r--   0 pieronicolli   (501) staff       (20)       77 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/bundle.js
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3386 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/integration.css
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3785 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/integration.css.map
--rw-r--r--   0 pieronicolli   (501) staff       (20)    11783 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/integration.js
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1510 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/loader.svg
--rw-r--r--   0 pieronicolli   (501) staff       (20)   104563 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/polyfill.min.js
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5815 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/redturtle-tiles-management-compiled.js.map
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2682 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/tiles-management-compiled.css
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1285 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/tiles-management-compiled.css.map
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4853 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/tiles-management-compiled.js
--rw-r--r--   0 pieronicolli   (501) staff       (20)    22275 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/tiles-management-compiled.js.map
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.780295 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/templates/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3835 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/templates/tiles_management.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1128 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/templates/tiles_view.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5331 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/tiles_management.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      438 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/tiles_view.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1454 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/traversal.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      661 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/vocabulary.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3032 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1579 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/event_handler.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2153 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/interfaces.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.780624 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/locales/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.772424 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/locales/it/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.780730 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/locales/it/LC_MESSAGES/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3420 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/locales/it/LC_MESSAGES/redturtle.tiles.management.po
--rw-r--r--   0 pieronicolli   (501) staff       (20)      756 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/locales/manual.pot
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2662 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/locales/redturtle.tiles.management.pot
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      535 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/locales/update.sh
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.772724 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.781342 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/default/
--rw-r--r--   0 pieronicolli   (501) staff       (20)      186 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/default/browserlayer.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      607 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/default/controlpanel.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      168 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/default/metadata.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/default/redturtletilesmanagement_default.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1760 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/default/registry.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      453 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/default/rolemap.xml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.781445 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/default/types/
--rw-r--r--   0 pieronicolli   (501) staff       (20)      388 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/default/types/Document.xml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.781545 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/to_1100/
--rw-r--r--   0 pieronicolli   (501) staff       (20)      372 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/to_1100/registry.xml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.781838 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/uninstall/
--rw-r--r--   0 pieronicolli   (501) staff       (20)      118 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/uninstall/redturtletilesmanagement_uninstall.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      755 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/uninstall/registry.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2480 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/setuphandlers.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1449 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/testing.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.782564 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      308 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/helpers.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.782676 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/robot/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2035 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/robot/test_example.robot
--rw-r--r--   0 pieronicolli   (501) staff       (20)      908 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/test_robot.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2261 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/test_setup.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3646 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/test_tiles_creation.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2903 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/test_tiles_show_hide.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5061 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/test_tiles_view.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1639 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/upgrades.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2523 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/vocabularies.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2022-09-16 15:10:28.776523 redturtle.tiles.management-3.0.0/src/redturtle.tiles.management.egg-info/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     9283 2022-09-16 15:10:28.000000 redturtle.tiles.management-3.0.0/src/redturtle.tiles.management.egg-info/PKG-INFO
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4367 2022-09-16 15:10:28.000000 redturtle.tiles.management-3.0.0/src/redturtle.tiles.management.egg-info/SOURCES.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)        1 2022-09-16 15:10:28.000000 redturtle.tiles.management-3.0.0/src/redturtle.tiles.management.egg-info/dependency_links.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)       40 2022-09-16 15:10:28.000000 redturtle.tiles.management-3.0.0/src/redturtle.tiles.management.egg-info/entry_points.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)       26 2022-09-16 15:10:28.000000 redturtle.tiles.management-3.0.0/src/redturtle.tiles.management.egg-info/namespace_packages.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)        1 2022-09-16 15:10:28.000000 redturtle.tiles.management-3.0.0/src/redturtle.tiles.management.egg-info/not-zip-safe
--rw-r--r--   0 pieronicolli   (501) staff       (20)      198 2022-09-16 15:10:28.000000 redturtle.tiles.management-3.0.0/src/redturtle.tiles.management.egg-info/requires.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)       10 2022-09-16 15:10:28.000000 redturtle.tiles.management-3.0.0/src/redturtle.tiles.management.egg-info/top_level.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1157 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/test_plone51.cfg
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1224 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/test_plone52.cfg
--rw-r--r--   0 pieronicolli   (501) staff       (20)      108 2022-09-16 15:10:27.000000 redturtle.tiles.management-3.0.0/versions.cfg
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.471685 redturtle.tiles.management-3.0.1/
+-rw-r--r--   0 cekk       (501) staff       (20)       75 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/.coveragerc
+-rw-r--r--   0 cekk       (501) staff       (20)      245 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/.editorconfig
+-rw-r--r--   0 cekk       (501) staff       (20)       23 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/.gitattributes
+-rw-r--r--   0 cekk       (501) staff       (20)     4481 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       51 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     2981 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/Gruntfile.js
+-rw-r--r--   0 cekk       (501) staff       (20)      361 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)    12284 2023-05-31 15:02:36.471878 redturtle.tiles.management-3.0.1/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     4102 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     1945 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/base.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)       61 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/bobtemplate.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)      162 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/buildout.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       39 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/constraints_plone51.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       39 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/constraints_plone52.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.453845 redturtle.tiles.management-3.0.1/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      677 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/docs/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       89 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    83959 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/package-lock.json
+-rw-r--r--   0 cekk       (501) staff       (20)      702 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/package.json
+-rw-r--r--   0 cekk       (501) staff       (20)       50 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      270 2023-05-31 15:02:36.472342 redturtle.tiles.management-3.0.1/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     1934 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.445268 redturtle.tiles.management-3.0.1/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.454078 redturtle.tiles.management-3.0.1/src/redturtle/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.456223 redturtle.tiles.management-3.0.1/src/redturtle/tiles/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.458139 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/
+-rw-r--r--   0 cekk       (501) staff       (20)     1237 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.460629 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      378 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/add.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4397 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      685 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/controlpanel.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2805 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/delete.py
+-rw-r--r--   0 cekk       (501) staff       (20)      842 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/edit.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.461356 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/overrides/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/overrides/.gitkeep
+-rw-r--r--   0 cekk       (501) staff       (20)     1107 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/overrides/plone.app.tiles.browser.add.pt
+-rw-r--r--   0 cekk       (501) staff       (20)      282 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/overrides/plone.app.tiles.browser.tileformlayout.pt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.464695 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/.gitkeep
+-rw-r--r--   0 cekk       (501) staff       (20)       77 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/bundle.js
+-rw-r--r--   0 cekk       (501) staff       (20)     3386 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/integration.css
+-rw-r--r--   0 cekk       (501) staff       (20)     3785 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/integration.css.map
+-rw-r--r--   0 cekk       (501) staff       (20)    11783 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/integration.js
+-rw-r--r--   0 cekk       (501) staff       (20)     1510 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/loader.svg
+-rw-r--r--   0 cekk       (501) staff       (20)   104563 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/polyfill.min.js
+-rw-r--r--   0 cekk       (501) staff       (20)     5815 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/redturtle-tiles-management-compiled.js.map
+-rw-r--r--   0 cekk       (501) staff       (20)     2682 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/tiles-management-compiled.css
+-rw-r--r--   0 cekk       (501) staff       (20)     1285 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/tiles-management-compiled.css.map
+-rw-r--r--   0 cekk       (501) staff       (20)     4853 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/tiles-management-compiled.js
+-rw-r--r--   0 cekk       (501) staff       (20)    22275 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/tiles-management-compiled.js.map
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.465403 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/templates/
+-rw-r--r--   0 cekk       (501) staff       (20)     3835 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/templates/tiles_management.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     1128 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/templates/tiles_view.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     5331 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/tiles_management.py
+-rw-r--r--   0 cekk       (501) staff       (20)      438 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/tiles_view.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1454 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/traversal.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1900 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/vocabulary.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3032 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1579 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/event_handler.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2153 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.466167 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/locales/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.446524 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.466719 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1643 2023-05-31 15:02:36.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/locales/it/LC_MESSAGES/redturtle.tiles.management.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     3420 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/locales/it/LC_MESSAGES/redturtle.tiles.management.po
+-rw-r--r--   0 cekk       (501) staff       (20)      756 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/locales/manual.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     2662 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/locales/redturtle.tiles.management.pot
+-rwxr-xr-x   0 cekk       (501) staff       (20)      535 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/locales/update.sh
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.447237 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.468229 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      186 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      607 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      168 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/default/redturtletilesmanagement_default.txt
+-rw-r--r--   0 cekk       (501) staff       (20)     1760 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      453 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.468563 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/default/types/
+-rw-r--r--   0 cekk       (501) staff       (20)      388 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/default/types/Document.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.468804 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/to_1100/
+-rw-r--r--   0 cekk       (501) staff       (20)      372 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/to_1100/registry.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.469480 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/uninstall/redturtletilesmanagement_uninstall.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      755 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/uninstall/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     2480 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1449 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.471233 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      308 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/helpers.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.471473 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/robot/
+-rw-r--r--   0 cekk       (501) staff       (20)     2035 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/robot/test_example.robot
+-rw-r--r--   0 cekk       (501) staff       (20)      908 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/test_robot.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2261 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/test_setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3646 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/test_tiles_creation.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2903 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/test_tiles_show_hide.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5061 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/test_tiles_view.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1639 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/upgrades.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2523 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/vocabularies.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 15:02:36.455993 redturtle.tiles.management-3.0.1/src/redturtle.tiles.management.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)    12284 2023-05-31 15:02:36.000000 redturtle.tiles.management-3.0.1/src/redturtle.tiles.management.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     4451 2023-05-31 15:02:36.000000 redturtle.tiles.management-3.0.1/src/redturtle.tiles.management.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-05-31 15:02:36.000000 redturtle.tiles.management-3.0.1/src/redturtle.tiles.management.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       53 2023-05-31 15:02:36.000000 redturtle.tiles.management-3.0.1/src/redturtle.tiles.management.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       26 2023-05-31 15:02:36.000000 redturtle.tiles.management-3.0.1/src/redturtle.tiles.management.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-05-31 15:02:36.000000 redturtle.tiles.management-3.0.1/src/redturtle.tiles.management.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      198 2023-05-31 15:02:36.000000 redturtle.tiles.management-3.0.1/src/redturtle.tiles.management.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       10 2023-05-31 15:02:36.000000 redturtle.tiles.management-3.0.1/src/redturtle.tiles.management.egg-info/top_level.txt
+-rw-r--r--   0 cekk       (501) staff       (20)     1157 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/test_plone51.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     1224 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/test_plone52.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)      108 2023-05-31 15:02:35.000000 redturtle.tiles.management-3.0.1/versions.cfg
```

### Comparing `redturtle.tiles.management-3.0.0/CHANGES.rst` & `redturtle.tiles.management-3.0.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+3.0.1 (2023-05-31)
+------------------
+
+- Fix context where to check permission in vocabulary.py customization.
+  [cekk]
+
+
 3.0.0 (2022-09-16)
 ------------------
 
 - Prepare package for pip.
   [eikichi18]
```

### Comparing `redturtle.tiles.management-3.0.0/Gruntfile.js` & `redturtle.tiles.management-3.0.1/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/README.rst` & `redturtle.tiles.management-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/base.cfg` & `redturtle.tiles.management-3.0.1/base.cfg`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/docs/LICENSE.GPL` & `redturtle.tiles.management-3.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/docs/LICENSE.rst` & `redturtle.tiles.management-3.0.1/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/package-lock.json` & `redturtle.tiles.management-3.0.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/package.json` & `redturtle.tiles.management-3.0.1/package.json`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/setup.py` & `redturtle.tiles.management-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     + open("CHANGES.rst").read()
     + "\n"
 )
 
 
 setup(
     name="redturtle.tiles.management",
-    version="3.0.0",
+    version="3.0.1",
     description="An alternative method for handling and showing tiles",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
```

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/__init__.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/configure.zcml` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/controlpanel.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/delete.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/delete.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/edit.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/edit.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/overrides/plone.app.tiles.browser.add.pt` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/overrides/plone.app.tiles.browser.add.pt`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/integration.css` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/integration.css`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/integration.css.map` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/integration.css.map`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/integration.js` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/integration.js`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/loader.svg` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/loader.svg`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/polyfill.min.js` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/polyfill.min.js`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/redturtle-tiles-management-compiled.js.map` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/redturtle-tiles-management-compiled.js.map`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/tiles-management-compiled.css` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/tiles-management-compiled.css`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/tiles-management-compiled.css.map` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/tiles-management-compiled.css.map`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/tiles-management-compiled.js` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/tiles-management-compiled.js`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/static/tiles-management-compiled.js.map` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/static/tiles-management-compiled.js.map`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/templates/tiles_management.pt` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/templates/tiles_management.pt`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/templates/tiles_view.pt` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/templates/tiles_view.pt`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/tiles_management.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/tiles_management.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/browser/traversal.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/browser/traversal.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/configure.zcml` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/event_handler.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/event_handler.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/interfaces.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/locales/it/LC_MESSAGES/redturtle.tiles.management.po` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/locales/it/LC_MESSAGES/redturtle.tiles.management.po`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/locales/manual.pot` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/locales/redturtle.tiles.management.pot` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/locales/redturtle.tiles.management.pot`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/locales/update.sh` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/locales/update.sh`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/default/controlpanel.xml` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/default/registry.xml` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/profiles/uninstall/registry.xml` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/profiles/uninstall/registry.xml`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/setuphandlers.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/testing.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/robot/test_example.robot` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/test_robot.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/test_setup.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/test_tiles_creation.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/test_tiles_creation.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/test_tiles_show_hide.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/test_tiles_show_hide.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/tests/test_tiles_view.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/tests/test_tiles_view.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/upgrades.zcml` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle/tiles/management/vocabularies.py` & `redturtle.tiles.management-3.0.1/src/redturtle/tiles/management/vocabularies.py`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/src/redturtle.tiles.management.egg-info/SOURCES.txt` & `redturtle.tiles.management-3.0.1/src/redturtle.tiles.management.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 src/redturtle/tiles/management/browser/static/tiles-management-compiled.js
 src/redturtle/tiles/management/browser/static/tiles-management-compiled.js.map
 src/redturtle/tiles/management/browser/templates/tiles_management.pt
 src/redturtle/tiles/management/browser/templates/tiles_view.pt
 src/redturtle/tiles/management/locales/manual.pot
 src/redturtle/tiles/management/locales/redturtle.tiles.management.pot
 src/redturtle/tiles/management/locales/update.sh
+src/redturtle/tiles/management/locales/it/LC_MESSAGES/redturtle.tiles.management.mo
 src/redturtle/tiles/management/locales/it/LC_MESSAGES/redturtle.tiles.management.po
 src/redturtle/tiles/management/profiles/default/browserlayer.xml
 src/redturtle/tiles/management/profiles/default/controlpanel.xml
 src/redturtle/tiles/management/profiles/default/metadata.xml
 src/redturtle/tiles/management/profiles/default/redturtletilesmanagement_default.txt
 src/redturtle/tiles/management/profiles/default/registry.xml
 src/redturtle/tiles/management/profiles/default/rolemap.xml
```

### Comparing `redturtle.tiles.management-3.0.0/test_plone51.cfg` & `redturtle.tiles.management-3.0.1/test_plone51.cfg`

 * *Files identical despite different names*

### Comparing `redturtle.tiles.management-3.0.0/test_plone52.cfg` & `redturtle.tiles.management-3.0.1/test_plone52.cfg`

 * *Files identical despite different names*

