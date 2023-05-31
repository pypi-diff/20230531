# Comparing `tmp/redturtle.chefcookie-2.0.2.tar.gz` & `tmp/redturtle.chefcookie-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.chefcookie-2.0.2.tar", last modified: Fri Apr 28 11:35:41 2023, max compression
+gzip compressed data, was "redturtle.chefcookie-2.1.0.tar", last modified: Wed May 31 09:13:51 2023, max compression
```

## Comparing `redturtle.chefcookie-2.0.2.tar` & `redturtle.chefcookie-2.1.0.tar`

### file list

```diff
@@ -1,108 +1,110 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2239 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/CHANGES.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       58 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/CONTRIBUTORS.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      586 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/DEVELOP.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/LICENSE.GPL
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      660 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/LICENSE.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      503 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/MANIFEST.in
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4763 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1362 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/README.rst
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.621284 redturtle.chefcookie-2.0.2/docs/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7901 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/docs/conf.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       83 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/docs/index.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      394 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2348 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.617284 redturtle.chefcookie-2.0.2/src/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.621284 redturtle.chefcookie-2.0.2/src/redturtle/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.621284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      137 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.621284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4054 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/chefcookie_consent_registry.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1508 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      888 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/controlpanel.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    18193 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/cookie_config.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.621284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/overrides/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/overrides/.gitkeep
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.621284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/.gitkeep
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.621284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      368 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/.babelrc
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      437 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/.eslintrc.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      202 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/.gitignore
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        8 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/.nvmrc
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      183 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/.prettierrc
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1071 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/LICENSE
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    21073 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/README.md
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/_js/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1912 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/_js/_helper.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    87005 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/_js/script.js
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/_tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5864 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/_tests/index.html
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    11340 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/_tests/script.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)   933160 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/chefcookie.min.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3924 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/package.json
--rw-rw-r--   0 mauro     (1000) mauro     (1000)   810910 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/yarn.lock
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1969 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/cookie-settings.png
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    19718 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/redturtle_chefcookie.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    11501 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/redturtle_chefcookie_tech.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7376 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/styles.css
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/templates/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      309 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/templates/get_chefcookie_js.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2671 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/viewlets.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1526 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    11801 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/defaults.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    10151 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/README.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.617284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/en/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/en/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9001 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.po
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.617284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/it/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/it/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    12413 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      643 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/manual.pot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9060 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/redturtle.chefcookie.pot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1756 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/update.py
--rwxrwxr-x   0 mauro     (1000) mauro     (1000)      516 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/update.sh
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/permissions.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.617284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/profiles/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/profiles/default/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      186 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/profiles/default/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/profiles/default/catalog.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      532 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/profiles/default/controlpanel.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      195 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/profiles/default/metadata.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      218 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/profiles/default/registry.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      118 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/profiles/default/rolemap.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/profiles/uninstall/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      130 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/restapi/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/restapi/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      438 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/restapi/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      494 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/restapi/get.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1024 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/setuphandlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1595 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/testing.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/tests/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/tests/robot/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2011 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/tests/robot/test_example.robot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      955 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/tests/test_robot.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2428 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/tests/test_setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.625284 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/transformers/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      396 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/transformers/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2632 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/transformers/adapters.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      605 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/transformers/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4702 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/transformers/transform.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3037 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/upgrades.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      798 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/upgrades.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-28 11:35:41.621284 redturtle.chefcookie-2.0.2/src/redturtle.chefcookie.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4763 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle.chefcookie.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3846 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle.chefcookie.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle.chefcookie.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       40 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle.chefcookie.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle.chefcookie.egg-info/namespace_packages.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle.chefcookie.egg-info/not-zip-safe
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      218 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle.chefcookie.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-04-28 11:35:41.000000 redturtle.chefcookie-2.0.2/src/redturtle.chefcookie.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.951290 redturtle.chefcookie-2.1.0/
+-rw-r--r--   0 cekk       (501) staff       (20)     2296 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       58 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      660 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      503 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     6215 2023-05-31 09:13:51.951445 redturtle.chefcookie-2.1.0/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     1362 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/README.rst
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.929023 redturtle.chefcookie-2.1.0/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7901 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)       83 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      394 2023-05-31 09:13:51.951939 redturtle.chefcookie-2.1.0/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2348 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.923279 redturtle.chefcookie-2.1.0/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.929334 redturtle.chefcookie-2.1.0/src/redturtle/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.933739 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/
+-rw-r--r--   0 cekk       (501) staff       (20)      137 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.935354 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4054 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/chefcookie_consent_registry.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1508 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      888 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/controlpanel.py
+-rw-r--r--   0 cekk       (501) staff       (20)    18193 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/cookie_config.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.935591 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/overrides/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/overrides/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.936879 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.940576 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/
+-rw-r--r--   0 cekk       (501) staff       (20)      368 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/.babelrc
+-rw-r--r--   0 cekk       (501) staff       (20)      437 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/.eslintrc.js
+-rw-r--r--   0 cekk       (501) staff       (20)      202 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/.gitignore
+-rw-r--r--   0 cekk       (501) staff       (20)        8 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/.nvmrc
+-rw-r--r--   0 cekk       (501) staff       (20)      183 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/.prettierrc
+-rw-r--r--   0 cekk       (501) staff       (20)     1071 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/LICENSE
+-rw-r--r--   0 cekk       (501) staff       (20)    21073 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/README.md
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.942721 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/_js/
+-rw-r--r--   0 cekk       (501) staff       (20)     1912 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/_js/_helper.js
+-rw-r--r--   0 cekk       (501) staff       (20)    87005 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/_js/script.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.943577 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/_tests/
+-rw-r--r--   0 cekk       (501) staff       (20)     5864 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/_tests/index.html
+-rw-r--r--   0 cekk       (501) staff       (20)    11340 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/_tests/script.js
+-rw-r--r--   0 cekk       (501) staff       (20)   933160 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/chefcookie.min.js
+-rw-r--r--   0 cekk       (501) staff       (20)     3924 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/package.json
+-rw-r--r--   0 cekk       (501) staff       (20)   810910 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/yarn.lock
+-rw-r--r--   0 cekk       (501) staff       (20)     1969 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/cookie-settings.png
+-rw-r--r--   0 cekk       (501) staff       (20)    19718 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/redturtle_chefcookie.js
+-rw-r--r--   0 cekk       (501) staff       (20)    15273 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/redturtle_chefcookie_tech.js
+-rw-r--r--   0 cekk       (501) staff       (20)     7376 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/styles.css
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.943890 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/templates/
+-rw-r--r--   0 cekk       (501) staff       (20)      309 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/templates/get_chefcookie_js.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     2671 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/viewlets.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1526 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)    11801 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/defaults.py
+-rw-r--r--   0 cekk       (501) staff       (20)    10151 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.945466 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.924901 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.946005 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      525 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     9001 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.925166 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.946535 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     6459 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.mo
+-rw-r--r--   0 cekk       (501) staff       (20)    12413 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.po
+-rw-r--r--   0 cekk       (501) staff       (20)      643 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/manual.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     9060 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/redturtle.chefcookie.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1756 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      516 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      273 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.925578 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.948130 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      186 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      532 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      195 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      218 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.948387 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      130 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.949083 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      438 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/restapi/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      494 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/restapi/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1024 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1595 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.949770 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/tests/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.950019 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/tests/robot/
+-rw-r--r--   0 cekk       (501) staff       (20)     2011 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/tests/robot/test_example.robot
+-rw-r--r--   0 cekk       (501) staff       (20)      955 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/tests/test_robot.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2428 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/tests/test_setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.951055 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/transformers/
+-rw-r--r--   0 cekk       (501) staff       (20)      396 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/transformers/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2632 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/transformers/adapters.py
+-rw-r--r--   0 cekk       (501) staff       (20)      605 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/transformers/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     4702 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/transformers/transform.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3037 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/upgrades.py
+-rw-r--r--   0 cekk       (501) staff       (20)      798 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/upgrades.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-31 09:13:51.931361 redturtle.chefcookie-2.1.0/src/redturtle.chefcookie.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     6215 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle.chefcookie.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3990 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle.chefcookie.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle.chefcookie.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       53 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle.chefcookie.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       10 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle.chefcookie.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle.chefcookie.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      218 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle.chefcookie.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       10 2023-05-31 09:13:51.000000 redturtle.chefcookie-2.1.0/src/redturtle.chefcookie.egg-info/top_level.txt
```

### Comparing `redturtle.chefcookie-2.0.2/CHANGES.rst` & `redturtle.chefcookie-2.1.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Changelog
 =========
 
-2.0.2 (2023-04-28)
+2.1.0 (2023-05-31)
 ------------------
 
-- remove default set cookie
+- Remove default set cookie
   [mamico]
-
+- Add title to close link also for tech cookies.
+  [cekk]
 
 2.0.1 (2022-11-08)
 ------------------
 
 - Remove unused python_requires in setup.py
   [cekk]
```

### Comparing `redturtle.chefcookie-2.0.2/DEVELOP.rst` & `redturtle.chefcookie-2.1.0/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/LICENSE.GPL` & `redturtle.chefcookie-2.1.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/LICENSE.rst` & `redturtle.chefcookie-2.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/README.rst` & `redturtle.chefcookie-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/docs/conf.py` & `redturtle.chefcookie-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/setup.py` & `redturtle.chefcookie-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.chefcookie",
-    version="2.0.2",
+    version="2.1.0",
     description="Cookie policy integration with chefookie",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/chefcookie_consent_registry.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/chefcookie_consent_registry.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/configure.zcml` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/controlpanel.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/cookie_config.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/cookie_config.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/LICENSE` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/LICENSE`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/README.md` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/README.md`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/_js/_helper.js` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/_js/_helper.js`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/_js/script.js` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/_js/script.js`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/_tests/index.html` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/_tests/index.html`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/_tests/script.js` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/_tests/script.js`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/chefcookie.min.js` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/chefcookie.min.js`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/package.json` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/package.json`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/chefcookie/yarn.lock` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/chefcookie/yarn.lock`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/cookie-settings.png` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/cookie-settings.png`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/redturtle_chefcookie.js` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/redturtle_chefcookie.js`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/redturtle_chefcookie_tech.js` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/redturtle_chefcookie_tech.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,170 +1,250 @@
 class redturtlechefcookie extends chefcookie {
     showSettings() {
-        this.logTracking('settings_open');
-        let el = document.querySelector('.chefcookie__settings-container');
-        el.classList.add('chefcookie__settings-container--visible');
-        el.style.minHeight = el.scrollHeight + 'px';
+        this.logTracking("settings_open");
+        let el = document.querySelector(".chefcookie__settings-container");
+        el.classList.add("chefcookie__settings-container--visible");
+        el.style.minHeight = el.scrollHeight + "px";
         setTimeout(() => {
-            if (el.classList.contains('chefcookie__settings-container--visible')) {
-                el.style.height = 'auto';
+            if (el.classList.contains("chefcookie__settings-container--visible")) {
+                el.style.height = "auto";
             }
         }, this.animationSpeed);
         this.fixMaxHeight();
     }
     acceptAllScripts() {
         let providers = [];
-        this.config.settings.forEach(settings__value => {
+        this.config.settings.forEach((settings__value) => {
             if (settings__value.scripts !== undefined) {
-                Object.entries(settings__value.scripts).forEach(([scripts__key, scripts__value]) => {
-                    this.accept(scripts__key, false);
-                });
+                Object.entries(settings__value.scripts).forEach(
+                    ([scripts__key, scripts__value]) => {
+                        this.accept(scripts__key, false);
+                    }
+                );
             }
         });
     }
     switchSettingsLabelsOpen() {
-        document.querySelector('.chefcookie__button--accept').style.display = 'block';
-        document.querySelector('.chefcookie__button--settings').style.display = 'none';
+        document.querySelector(".chefcookie__button--accept").style.display =
+            "block";
+        document.querySelector(".chefcookie__button--settings").style.display =
+            "none";
     }
     buildDom() {
         document.body.insertAdjacentHTML(
-            'afterbegin',
+            "afterbegin",
             `
-            <div id="cc-banner" class="chefcookie chefcookie--${this.config.style.layout} chefcookie--columns-${
-                'columns' in this.config.style ? this.config.style.columns : 'auto'
-            }${
-                'scripts_selection' in this.config && this.config.scripts_selection !== false
-                    ? ` chefcookie--has-scripts`
-                    : ``
-            } chefcookie--hidden">
+            <div id="cc-banner" class="chefcookie chefcookie--${
+              this.config.style.layout
+            } chefcookie--columns-${
+        "columns" in this.config.style ? this.config.style.columns : "auto"
+      }${
+        "scripts_selection" in this.config &&
+        this.config.scripts_selection !== false
+          ? ` chefcookie--has-scripts`
+          : ``
+      } chefcookie--hidden">
                 <div class="chefcookie__inner">
                     <div class="chefcookie__box">
 
-                        <a data-cc-destroy href="#" class="close"></a>
+                        <a data-cc-destroy href="#" class="close" title="${this.getLabel(
+                          "close"
+                        )}"></a>
 
-                        <div class="chefcookie__message">${this.translate(this.config.message)}</div>
+                        <div class="chefcookie__message">${this.translate(
+                          this.config.message
+                        )}</div>
                         <div class="chefcookie__settings-container">
-                            <ul class="chefcookie__groups chefcookie__groups--count-${this.config.settings.length}">
+                            <ul class="chefcookie__groups chefcookie__groups--count-${
+                              this.config.settings.length
+                            }">
                                 ${this.config.settings
-                                    .map(
-                                        (group, i) => `
+                                  .map(
+                                    (group, i) => `
                                     <li class="chefcookie__group${
-                                        group.cannot_be_modified ? ` chefcookie__group--disabled` : ``
+                                      group.cannot_be_modified
+                                        ? ` chefcookie__group--disabled`
+                                        : ``
                                     }">
                                         <label class="chefcookie__group-label" for="chefcookie_group_${i}">
                                             <input${
-                                                group.cannot_be_modified ? ` disabled="disabled"` : ``
+                                              group.cannot_be_modified
+                                                ? ` disabled="disabled"`
+                                                : ``
                                             } class="chefcookie__group-checkbox" data-status="${this.isCheckboxActiveForGroup(
-                                            i
-                                        )}" id="chefcookie_group_${i}" type="checkbox" name="chefcookie_group[]" value="${i}"${
-                                            this.isCheckboxActiveForGroup(i) === 2 ? ` checked="checked"` : ``
-                                        } />
-                                            <span class="chefcookie__group-title">${this.translate(group.title)}</span>
+                                      i
+                                    )}" id="chefcookie_group_${i}" type="checkbox" name="chefcookie_group[]" value="${i}"${
+                                      this.isCheckboxActiveForGroup(i) === 2
+                                        ? ` checked="checked"`
+                                        : ``
+                                    } />
+                                            <span class="chefcookie__group-title">${this.translate(
+                                              group.title
+                                            )}</span>
                                             <span class="chefcookie__group-checkbox-icon"></span>
                                             ${
-                                                'description' in group && group.description != ''
-                                                    ? `
+                                              "description" in group &&
+                                              group.description != ""
+                                                ? `
                                             <span class="chefcookie__group-description">${this.translate(
-                                                group.description
+                                              group.description
                                             )}</span>
                                             `
-                                                    : ``
+                                                : ``
                                             }
                                             ${
-                                                'scripts_selection' in this.config &&
-                                                this.config.scripts_selection === 'collapse' &&
-                                                'scripts' in group &&
-                                                Object.keys(group.scripts).length > 0 &&
-                                                Object.keys(group.scripts)[0].indexOf('dummy_') === -1
-                                                    ? `
+                                              "scripts_selection" in
+                                                this.config &&
+                                              this.config.scripts_selection ===
+                                                "collapse" &&
+                                              "scripts" in group &&
+                                              Object.keys(group.scripts)
+                                                .length > 0 &&
+                                              Object.keys(
+                                                group.scripts
+                                              )[0].indexOf("dummy_") === -1
+                                                ? `
                                                         <a href="#" class="chefcookie__group-collapse">${
-                                                            this.getLabel('group_open') != ''
-                                                                ? this.getLabel('group_open')
-                                                                : this.getLabel('settings_open')
+                                                          this.getLabel(
+                                                            "group_open"
+                                                          ) != ""
+                                                            ? this.getLabel(
+                                                                "group_open"
+                                                              )
+                                                            : this.getLabel(
+                                                                "settings_open"
+                                                              )
                                                         }</a>
                                                     `
-                                                    : ``
+                                                : ``
                                             }
                                         </label>
                                         ${
-                                            'scripts_selection' in this.config &&
-                                            this.config.scripts_selection !== false &&
-                                            'scripts' in group &&
-                                            Object.keys(group.scripts).length > 0 &&
-                                            Object.keys(group.scripts)[0].indexOf('dummy_') === -1
-                                                ? `
+                                          "scripts_selection" in this.config &&
+                                          this.config.scripts_selection !==
+                                            false &&
+                                          "scripts" in group &&
+                                          Object.keys(group.scripts).length >
+                                            0 &&
+                                          Object.keys(group.scripts)[0].indexOf(
+                                            "dummy_"
+                                          ) === -1
+                                            ? `
                                                 <ul class="chefcookie__scripts chefcookie__scripts--count-${
-                                                    Object.keys(group.scripts).length
+                                                  Object.keys(group.scripts)
+                                                    .length
                                                 }${
-                                                      this.config.scripts_selection !== 'collapse'
-                                                          ? ` chefcookie__scripts--visible`
-                                                          : ``
-                                                  }">
+                                                this.config
+                                                  .scripts_selection !==
+                                                "collapse"
+                                                  ? ` chefcookie__scripts--visible`
+                                                  : ``
+                                              }">
                                                     ${Object.keys(group.scripts)
-                                                        .map(
-                                                            j => `
+                                                      .map(
+                                                        (j) => `
                                                         <li class="chefcookie__script${
-                                                            group.cannot_be_modified
-                                                                ? ` chefcookie__script--disabled`
-                                                                : ``
+                                                          group.cannot_be_modified
+                                                            ? ` chefcookie__script--disabled`
+                                                            : ``
                                                         }">
                                                             <label class="chefcookie__script-label" for="chefcookie_script_${i}_${j}">
                                                                 <input${
-                                                                    group.cannot_be_modified
-                                                                        ? ` disabled="disabled"`
-                                                                        : ``
-                                                                } class="chefcookie__script-checkbox" id="chefcookie_script_${i}_${j}" type="checkbox" name="chefcookie_script[]" value="${i}|${j}"${
-                                                                this.isCheckboxActiveForProvider(i, j)
-                                                                    ? ` checked="checked"`
+                                                                  group.cannot_be_modified
+                                                                    ? ` disabled="disabled"`
                                                                     : ``
-                                                            } />
+                                                                } class="chefcookie__script-checkbox" id="chefcookie_script_${i}_${j}" type="checkbox" name="chefcookie_script[]" value="${i}|${j}"${
+                                                          this.isCheckboxActiveForProvider(
+                                                            i,
+                                                            j
+                                                          )
+                                                            ? ` checked="checked"`
+                                                            : ``
+                                                        } />
                                                                 <span class="chefcookie__script-title">${
-                                                                    typeof group.scripts[j] === 'object' &&
-                                                                    group.scripts[j] !== null &&
-                                                                    'title' in group.scripts[j] &&
-                                                                    group.scripts[j].title != ''
-                                                                        ? this.translate(group.scripts[j].title)
-                                                                        : j
+                                                                  typeof group
+                                                                    .scripts[
+                                                                    j
+                                                                  ] ===
+                                                                    "object" &&
+                                                                  group.scripts[
+                                                                    j
+                                                                  ] !== null &&
+                                                                  "title" in
+                                                                    group
+                                                                      .scripts[
+                                                                      j
+                                                                    ] &&
+                                                                  group.scripts[
+                                                                    j
+                                                                  ].title != ""
+                                                                    ? this.translate(
+                                                                        group
+                                                                          .scripts[
+                                                                          j
+                                                                        ].title
+                                                                      )
+                                                                    : j
                                                                 }</span>
                                                                 <span class="chefcookie__script-checkbox-icon"></span>
                                                             </label>
                                                             ${
-                                                                typeof group.scripts[j] === 'object' &&
-                                                                group.scripts[j] !== null &&
-                                                                'description' in group.scripts[j] &&
-                                                                group.scripts[j].description != ''
-                                                                    ? '<div class="chefcookie__script-description">' +
-                                                                      '<a href="#" class="chefcookie__script-description-collapse">' +
-                                                                      this.getLabel('details_open') +
-                                                                      '</a>' +
-                                                                      '<div class="chefcookie__script-description-content">' +
-                                                                      this.translate(group.scripts[j].description) +
-                                                                      '</div>' +
-                                                                      '</div>'
-                                                                    : ''
+                                                              typeof group
+                                                                .scripts[j] ===
+                                                                "object" &&
+                                                              group.scripts[
+                                                                j
+                                                              ] !== null &&
+                                                              "description" in
+                                                                group.scripts[
+                                                                  j
+                                                                ] &&
+                                                              group.scripts[j]
+                                                                .description !=
+                                                                ""
+                                                                ? '<div class="chefcookie__script-description">' +
+                                                                  '<a href="#" class="chefcookie__script-description-collapse">' +
+                                                                  this.getLabel(
+                                                                    "details_open"
+                                                                  ) +
+                                                                  "</a>" +
+                                                                  '<div class="chefcookie__script-description-content">' +
+                                                                  this.translate(
+                                                                    group
+                                                                      .scripts[
+                                                                      j
+                                                                    ]
+                                                                      .description
+                                                                  ) +
+                                                                  "</div>" +
+                                                                  "</div>"
+                                                                : ""
                                                             }
                                                         </li>
                                                     `
-                                                        )
-                                                        .join('')}
+                                                      )
+                                                      .join("")}
                                                 </ul>
                                             `
-                                                : ``
+                                            : ``
                                         }
                                     </li>
                                 `
-                                    )
-                                    .join('')}
+                                  )
+                                  .join("")}
                             </ul>
                         </div>
                         <div class="chefcookie__buttons chefcookie__buttons--count-${
-                            'show_decline_button' in this.config && this.config.show_decline_button === true ? '3' : '2'
+                          "show_decline_button" in this.config &&
+                          this.config.show_decline_button === true
+                            ? "3"
+                            : "2"
                         }">
                             <a href="#chefcookie__decline" class="chefcookie__button chefcookie__button--decline">${this.getLabel(
-                                'decline'
+                              "decline"
                             )}</a>
                         </div>
                     </div>
                 </div>
             </div>
         `
         );
```

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/static/styles.css` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/static/styles.css`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/browser/viewlets.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/configure.zcml` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/defaults.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/defaults.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/interfaces.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/README.rst` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.po` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.po`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.po` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.po`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/manual.pot` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/redturtle.chefcookie.pot` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/redturtle.chefcookie.pot`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/update.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/locales/update.sh` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/locales/update.sh`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/profiles/default/controlpanel.xml` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/setuphandlers.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/testing.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/tests/robot/test_example.robot` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/tests/test_robot.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/tests/test_setup.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/transformers/adapters.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/transformers/adapters.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/transformers/configure.zcml` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/transformers/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/transformers/transform.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/transformers/transform.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/upgrades.py` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/upgrades.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle/chefcookie/upgrades.zcml` & `redturtle.chefcookie-2.1.0/src/redturtle/chefcookie/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.2/src/redturtle.chefcookie.egg-info/SOURCES.txt` & `redturtle.chefcookie-2.1.0/src/redturtle.chefcookie.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 src/redturtle/chefcookie/browser/templates/get_chefcookie_js.pt
 src/redturtle/chefcookie/locales/README.rst
 src/redturtle/chefcookie/locales/__init__.py
 src/redturtle/chefcookie/locales/manual.pot
 src/redturtle/chefcookie/locales/redturtle.chefcookie.pot
 src/redturtle/chefcookie/locales/update.py
 src/redturtle/chefcookie/locales/update.sh
+src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.mo
 src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.po
+src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.mo
 src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.po
 src/redturtle/chefcookie/profiles/default/browserlayer.xml
 src/redturtle/chefcookie/profiles/default/catalog.xml
 src/redturtle/chefcookie/profiles/default/controlpanel.xml
 src/redturtle/chefcookie/profiles/default/metadata.xml
 src/redturtle/chefcookie/profiles/default/registry.xml
 src/redturtle/chefcookie/profiles/default/rolemap.xml
```

