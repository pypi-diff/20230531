# Comparing `tmp/ftw.referencewidget-4.0.0b1.tar.gz` & `tmp/ftw.referencewidget-4.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftw.referencewidget-4.0.0b1.tar", last modified: Fri Aug 12 01:25:10 2022, max compression
+gzip compressed data, was "ftw.referencewidget-4.0.0b2.tar", last modified: Mon May 22 14:27:40 2023, max compression
```

## Comparing `ftw.referencewidget-4.0.0b1.tar` & `ftw.referencewidget-4.0.0b2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.498009 ftw.referencewidget-4.0.0b1/
--rw-r--r--   0 maethu     (501) staff       (20)      137 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/MANIFEST.in
--rw-r--r--   0 maethu     (501) staff       (20)    19114 2022-08-12 01:25:10.497759 ftw.referencewidget-4.0.0b1/PKG-INFO
--rw-r--r--   0 maethu     (501) staff       (20)     7085 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/README.rst
--rw-r--r--   0 maethu     (501) staff       (20)       73 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/constraints.txt
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.479752 ftw.referencewidget-4.0.0b1/docs/
--rw-r--r--   0 maethu     (501) staff       (20)     7248 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/docs/HISTORY.txt
--rw-r--r--   0 maethu     (501) staff       (20)    18092 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/docs/LICENSE.GPL
--rw-r--r--   0 maethu     (501) staff       (20)      721 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/docs/LICENSE.txt
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.480990 ftw.referencewidget-4.0.0b1/docs/static/
--rw-r--r--   0 maethu     (501) staff       (20)   164752 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/docs/static/list.png
--rw-r--r--   0 maethu     (501) staff       (20)   329017 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/docs/static/search.png
--rw-r--r--   0 maethu     (501) staff       (20)   136044 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/docs/static/selected.png
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.481380 ftw.referencewidget-4.0.0b1/ftw/
--rw-r--r--   0 maethu     (501) staff       (20)      244 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/__init__.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.485890 ftw.referencewidget-4.0.0b1/ftw/referencewidget/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.486121 ftw.referencewidget-4.0.0b1/ftw/referencewidget/Extensions/
--rw-r--r--   0 maethu     (501) staff       (20)      253 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/Extensions/install.py
--rw-r--r--   0 maethu     (501) staff       (20)      177 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)     2850 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/behaviors.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.487222 ftw.referencewidget-4.0.0b1/ftw/referencewidget/browser/
--rw-r--r--   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/browser/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      513 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/browser/configure.zcml
--rw-r--r--   0 maethu     (501) staff       (20)      162 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/browser/fake_edit.py
--rw-r--r--   0 maethu     (501) staff       (20)     4694 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/browser/utils.py
--rw-r--r--   0 maethu     (501) staff       (20)     3935 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/configure.zcml
--rw-r--r--   0 maethu     (501) staff       (20)     3699 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/converter.py
--rw-r--r--   0 maethu     (501) staff       (20)     3205 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/datagridfield.py
--rw-r--r--   0 maethu     (501) staff       (20)     1152 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/interfaces.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.487499 ftw.referencewidget-4.0.0b1/ftw/referencewidget/locales/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.475753 ftw.referencewidget-4.0.0b1/ftw/referencewidget/locales/de/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.487731 ftw.referencewidget-4.0.0b1/ftw/referencewidget/locales/de/LC_MESSAGES/
--rw-r--r--   0 maethu     (501) staff       (20)     3748 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/locales/de/LC_MESSAGES/ftw.referencewidget.po
--rw-r--r--   0 maethu     (501) staff       (20)     3564 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/locales/ftw.referencewidget.pot
--rw-r--r--   0 maethu     (501) staff       (20)      311 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/overrides.zcml
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.476100 ftw.referencewidget-4.0.0b1/ftw/referencewidget/profiles/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.488202 ftw.referencewidget-4.0.0b1/ftw/referencewidget/profiles/default/
--rw-r--r--   0 maethu     (501) staff       (20)      145 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/profiles/default/metadata.xml
--rw-r--r--   0 maethu     (501) staff       (20)      123 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/profiles/default/registry.xml
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.488477 ftw.referencewidget-4.0.0b1/ftw/referencewidget/profiles/uninstall/
--rw-r--r--   0 maethu     (501) staff       (20)      303 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/profiles/uninstall/registry.xml
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.476439 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.489236 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/dist/
--rw-r--r--   0 maethu     (501) staff       (20)   279211 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/dist/referencewidget.es.js
--rw-r--r--   0 maethu     (501) staff       (20)   122169 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/dist/referencewidget.umd.js
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.489607 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/
--rw-r--r--   0 maethu     (501) staff       (20)     1035 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/main.js
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.490068 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/
--rw-r--r--   0 maethu     (501) staff       (20)     6763 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/App.vue
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.491305 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/components/
--rw-r--r--   0 maethu     (501) staff       (20)     1374 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/components/Breadcrumbs.vue
--rw-r--r--   0 maethu     (501) staff       (20)     3193 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/components/ListItems.vue
--rw-r--r--   0 maethu     (501) staff       (20)      876 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/components/Pagination.vue
--rw-r--r--   0 maethu     (501) staff       (20)      830 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/components/ResolveIcon.vue
--rw-r--r--   0 maethu     (501) staff       (20)     2586 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/components/searchForm.vue
--rw-r--r--   0 maethu     (501) staff       (20)      213 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/i18n.js
--rw-r--r--   0 maethu     (501) staff       (20)     1141 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/selectable.py
--rw-r--r--   0 maethu     (501) staff       (20)     3138 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/sources.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.491771 ftw.referencewidget-4.0.0b1/ftw/referencewidget/templates/
--rw-r--r--   0 maethu     (501) staff       (20)      610 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/templates/referencewidget_display.pt
--rw-r--r--   0 maethu     (501) staff       (20)     2023 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/templates/referencewidget_input.pt
--rw-r--r--   0 maethu     (501) staff       (20)     1907 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/testing.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.494490 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/
--rw-r--r--   0 maethu     (501) staff       (20)     1755 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      386 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/builders.py
--rw-r--r--   0 maethu     (501) staff       (20)     1717 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_change_widget_config.py
--rw-r--r--   0 maethu     (501) staff       (20)     1738 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_converter.py
--rw-r--r--   0 maethu     (501) staff       (20)     1357 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_datagrid_field.py
--rw-r--r--   0 maethu     (501) staff       (20)     1335 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_override.py
--rw-r--r--   0 maethu     (501) staff       (20)     4369 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_related_items_behavior.py
--rw-r--r--   0 maethu     (501) staff       (20)     4937 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_relation_choice.py
--rw-r--r--   0 maethu     (501) staff       (20)     3956 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_source.py
--rw-r--r--   0 maethu     (501) staff       (20)      293 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_uninstall.py
--rw-r--r--   0 maethu     (501) staff       (20)     2565 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_utils.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.495128 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/views/
--rw-r--r--   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/views/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      319 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/views/configure.zcml
--rw-r--r--   0 maethu     (501) staff       (20)     1275 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/views/form.py
--rw-r--r--   0 maethu     (501) staff       (20)     1472 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/widgets.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.495397 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.495988 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/
--rw-r--r--   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      122 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/registry.xml
--rw-r--r--   0 maethu     (501) staff       (20)      200 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/upgrade.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.496664 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/
--rw-r--r--   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      286 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/jsregistry.xml
--rw-r--r--   0 maethu     (501) staff       (20)      354 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/upgrade.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.497313 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/
--rw-r--r--   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      350 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/registry.xml
--rw-r--r--   0 maethu     (501) staff       (20)      314 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/upgrade.py
--rw-r--r--   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/upgrades/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      485 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/utils.py
--rw-r--r--   0 maethu     (501) staff       (20)     7584 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/ftw/referencewidget/widget.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2022-08-12 01:25:10.483264 ftw.referencewidget-4.0.0b1/ftw.referencewidget.egg-info/
--rw-r--r--   0 maethu     (501) staff       (20)    19114 2022-08-12 01:25:10.000000 ftw.referencewidget-4.0.0b1/ftw.referencewidget.egg-info/PKG-INFO
--rw-r--r--   0 maethu     (501) staff       (20)     3673 2022-08-12 01:25:10.000000 ftw.referencewidget-4.0.0b1/ftw.referencewidget.egg-info/SOURCES.txt
--rw-r--r--   0 maethu     (501) staff       (20)        1 2022-08-12 01:25:10.000000 ftw.referencewidget-4.0.0b1/ftw.referencewidget.egg-info/dependency_links.txt
--rw-r--r--   0 maethu     (501) staff       (20)       91 2022-08-12 01:25:10.000000 ftw.referencewidget-4.0.0b1/ftw.referencewidget.egg-info/entry_points.txt
--rw-r--r--   0 maethu     (501) staff       (20)        4 2022-08-12 01:25:10.000000 ftw.referencewidget-4.0.0b1/ftw.referencewidget.egg-info/namespace_packages.txt
--rw-r--r--   0 maethu     (501) staff       (20)        1 2022-08-12 01:25:10.000000 ftw.referencewidget-4.0.0b1/ftw.referencewidget.egg-info/not-zip-safe
--rw-r--r--   0 maethu     (501) staff       (20)      361 2022-08-12 01:25:10.000000 ftw.referencewidget-4.0.0b1/ftw.referencewidget.egg-info/requires.txt
--rw-r--r--   0 maethu     (501) staff       (20)        4 2022-08-12 01:25:10.000000 ftw.referencewidget-4.0.0b1/ftw.referencewidget.egg-info/top_level.txt
--rw-r--r--   0 maethu     (501) staff       (20)       41 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/requirements.txt
--rw-r--r--   0 maethu     (501) staff       (20)      191 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/requirements_barebone.txt
--rw-r--r--   0 maethu     (501) staff       (20)       38 2022-08-12 01:25:10.498077 ftw.referencewidget-4.0.0b1/setup.cfg
--rw-r--r--   0 maethu     (501) staff       (20)     1797 2022-08-12 01:25:09.000000 ftw.referencewidget-4.0.0b1/setup.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.896274 ftw.referencewidget-4.0.0b2/
+-rw-r--r--   0 maethu     (501) staff       (20)      137 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/MANIFEST.in
+-rw-r--r--   0 maethu     (501) staff       (20)    15519 2023-05-22 14:27:40.896121 ftw.referencewidget-4.0.0b2/PKG-INFO
+-rw-r--r--   0 maethu     (501) staff       (20)     7085 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/README.rst
+-rw-r--r--   0 maethu     (501) staff       (20)       71 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/constraints.txt
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.886435 ftw.referencewidget-4.0.0b2/docs/
+-rw-r--r--   0 maethu     (501) staff       (20)     7674 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/docs/HISTORY.txt
+-rw-r--r--   0 maethu     (501) staff       (20)    18092 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/docs/LICENSE.GPL
+-rw-r--r--   0 maethu     (501) staff       (20)      721 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/docs/LICENSE.txt
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.887113 ftw.referencewidget-4.0.0b2/docs/static/
+-rw-r--r--   0 maethu     (501) staff       (20)   164752 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/docs/static/list.png
+-rw-r--r--   0 maethu     (501) staff       (20)   329017 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/docs/static/search.png
+-rw-r--r--   0 maethu     (501) staff       (20)   136044 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/docs/static/selected.png
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.887299 ftw.referencewidget-4.0.0b2/ftw/
+-rw-r--r--   0 maethu     (501) staff       (20)      244 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/__init__.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.889678 ftw.referencewidget-4.0.0b2/ftw/referencewidget/
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.889800 ftw.referencewidget-4.0.0b2/ftw/referencewidget/Extensions/
+-rw-r--r--   0 maethu     (501) staff       (20)      253 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/Extensions/install.py
+-rw-r--r--   0 maethu     (501) staff       (20)      177 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)     2881 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/behaviors.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.890261 ftw.referencewidget-4.0.0b2/ftw/referencewidget/browser/
+-rw-r--r--   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/browser/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      513 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/browser/configure.zcml
+-rw-r--r--   0 maethu     (501) staff       (20)      162 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/browser/fake_edit.py
+-rw-r--r--   0 maethu     (501) staff       (20)     4694 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/browser/utils.py
+-rw-r--r--   0 maethu     (501) staff       (20)     3959 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/configure.zcml
+-rw-r--r--   0 maethu     (501) staff       (20)     3699 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/converter.py
+-rw-r--r--   0 maethu     (501) staff       (20)     3205 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/datagridfield.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1152 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/interfaces.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.890366 ftw.referencewidget-4.0.0b2/ftw/referencewidget/locales/
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.884393 ftw.referencewidget-4.0.0b2/ftw/referencewidget/locales/de/
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.890485 ftw.referencewidget-4.0.0b2/ftw/referencewidget/locales/de/LC_MESSAGES/
+-rw-r--r--   0 maethu     (501) staff       (20)     3853 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/locales/de/LC_MESSAGES/ftw.referencewidget.po
+-rw-r--r--   0 maethu     (501) staff       (20)     3653 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/locales/ftw.referencewidget.pot
+-rw-r--r--   0 maethu     (501) staff       (20)      311 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/overrides.zcml
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.884552 ftw.referencewidget-4.0.0b2/ftw/referencewidget/profiles/
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.890729 ftw.referencewidget-4.0.0b2/ftw/referencewidget/profiles/default/
+-rw-r--r--   0 maethu     (501) staff       (20)      145 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/profiles/default/metadata.xml
+-rw-r--r--   0 maethu     (501) staff       (20)      123 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/profiles/default/registry.xml
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.890832 ftw.referencewidget-4.0.0b2/ftw/referencewidget/profiles/uninstall/
+-rw-r--r--   0 maethu     (501) staff       (20)      303 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/profiles/uninstall/registry.xml
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.884708 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.891402 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/dist/
+-rw-r--r--   0 maethu     (501) staff       (20)   532815 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/dist/referencewidget.es.js
+-rw-r--r--   0 maethu     (501) staff       (20)   228318 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/dist/referencewidget.umd.js
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.891671 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/
+-rw-r--r--   0 maethu     (501) staff       (20)     1154 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/main.js
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.891893 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/
+-rw-r--r--   0 maethu     (501) staff       (20)     6881 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/App.vue
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.892590 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/components/
+-rw-r--r--   0 maethu     (501) staff       (20)     1374 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/components/Breadcrumbs.vue
+-rw-r--r--   0 maethu     (501) staff       (20)     3738 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/components/ListItems.vue
+-rw-r--r--   0 maethu     (501) staff       (20)      876 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/components/Pagination.vue
+-rw-r--r--   0 maethu     (501) staff       (20)      813 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/components/ResolveIcon.vue
+-rw-r--r--   0 maethu     (501) staff       (20)     2586 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/components/searchForm.vue
+-rw-r--r--   0 maethu     (501) staff       (20)      213 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/i18n.js
+-rw-r--r--   0 maethu     (501) staff       (20)     1141 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/selectable.py
+-rw-r--r--   0 maethu     (501) staff       (20)     3196 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/sources.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.893212 ftw.referencewidget-4.0.0b2/ftw/referencewidget/templates/
+-rw-r--r--   0 maethu     (501) staff       (20)      610 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/templates/referencewidget_display.pt
+-rw-r--r--   0 maethu     (501) staff       (20)     2110 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/templates/referencewidget_input.pt
+-rw-r--r--   0 maethu     (501) staff       (20)     1907 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/testing.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.894629 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/
+-rw-r--r--   0 maethu     (501) staff       (20)     1755 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      386 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/builders.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1717 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_change_widget_config.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1738 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_converter.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1357 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_datagrid_field.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1335 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_override.py
+-rw-r--r--   0 maethu     (501) staff       (20)     4369 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_related_items_behavior.py
+-rw-r--r--   0 maethu     (501) staff       (20)     4937 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_relation_choice.py
+-rw-r--r--   0 maethu     (501) staff       (20)     3956 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_source.py
+-rw-r--r--   0 maethu     (501) staff       (20)      293 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_uninstall.py
+-rw-r--r--   0 maethu     (501) staff       (20)     2565 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_utils.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.894965 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/views/
+-rw-r--r--   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/views/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      319 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/views/configure.zcml
+-rw-r--r--   0 maethu     (501) staff       (20)     1275 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/views/form.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1472 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/widgets.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.895059 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.895350 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/
+-rw-r--r--   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      122 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/registry.xml
+-rw-r--r--   0 maethu     (501) staff       (20)      200 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/upgrade.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.895682 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/
+-rw-r--r--   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      286 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/jsregistry.xml
+-rw-r--r--   0 maethu     (501) staff       (20)      354 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/upgrade.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.895970 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/
+-rw-r--r--   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      350 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/registry.xml
+-rw-r--r--   0 maethu     (501) staff       (20)      314 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/upgrade.py
+-rw-r--r--   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/upgrades/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      485 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/utils.py
+-rw-r--r--   0 maethu     (501) staff       (20)     8585 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw/referencewidget/widget.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-05-22 14:27:40.888127 ftw.referencewidget-4.0.0b2/ftw.referencewidget.egg-info/
+-rw-r--r--   0 maethu     (501) staff       (20)    15519 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw.referencewidget.egg-info/PKG-INFO
+-rw-r--r--   0 maethu     (501) staff       (20)     3673 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw.referencewidget.egg-info/SOURCES.txt
+-rw-r--r--   0 maethu     (501) staff       (20)        1 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw.referencewidget.egg-info/dependency_links.txt
+-rw-r--r--   0 maethu     (501) staff       (20)       42 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw.referencewidget.egg-info/entry_points.txt
+-rw-r--r--   0 maethu     (501) staff       (20)        4 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw.referencewidget.egg-info/namespace_packages.txt
+-rw-r--r--   0 maethu     (501) staff       (20)        1 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw.referencewidget.egg-info/not-zip-safe
+-rw-r--r--   0 maethu     (501) staff       (20)      361 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw.referencewidget.egg-info/requires.txt
+-rw-r--r--   0 maethu     (501) staff       (20)        4 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/ftw.referencewidget.egg-info/top_level.txt
+-rw-r--r--   0 maethu     (501) staff       (20)       41 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/requirements.txt
+-rw-r--r--   0 maethu     (501) staff       (20)      191 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/requirements_barebone.txt
+-rw-r--r--   0 maethu     (501) staff       (20)       38 2023-05-22 14:27:40.896306 ftw.referencewidget-4.0.0b2/setup.cfg
+-rw-r--r--   0 maethu     (501) staff       (20)     1897 2023-05-22 14:27:40.000000 ftw.referencewidget-4.0.0b2/setup.py
```

### Comparing `ftw.referencewidget-4.0.0b1/README.rst` & `ftw.referencewidget-4.0.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/docs/HISTORY.txt` & `ftw.referencewidget-4.0.0b2/docs/HISTORY.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 Changelog
 =========
 
 
+4.0.0b2 (2023-05-22)
+--------------------
+
+- Load and register widget via patternslib. [mathias.leimgruber]
+
+- Fix selected state in widget for selected items and add title to selected items. [mathias.leimgruber]
+
+- Use switch instead of checkboxes for better readability. [mathias.leimgruber]
+
+- Fix mimetype icons for files and images. [mathias.leimgruber]
+
+- Support supermodel RelationChoice fields [mathias.leimgruber]
+
+
 4.0.0b1 (2022-08-11)
 --------------------
 
 - Improve styling [mathias.leimgruber]
 
 - Add options to translate the js widget and add translations (german) [mathias.leimgruber]
```

### Comparing `ftw.referencewidget-4.0.0b1/docs/LICENSE.GPL` & `ftw.referencewidget-4.0.0b2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/docs/LICENSE.txt` & `ftw.referencewidget-4.0.0b2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/docs/static/list.png` & `ftw.referencewidget-4.0.0b2/docs/static/list.png`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/docs/static/search.png` & `ftw.referencewidget-4.0.0b2/docs/static/search.png`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/docs/static/selected.png` & `ftw.referencewidget-4.0.0b2/docs/static/selected.png`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/behaviors.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/behaviors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 from ftw.referencewidget.selectable import DefaultSelectable
 from ftw.referencewidget.sources import ReferenceObjSourceBinder
 from ftw.referencewidget.widget import ReferenceWidgetFactory
 from plone.autoform import directives
 from plone.autoform.interfaces import IFormFieldProvider
 from plone.supermodel import model
 from plone.supermodel.model import fieldset
-from Products.CMFPlone import PloneMessageFactory as _
+from Products.CMFPlone import PloneMessageFactory as pmf
+from ftw.referencewidget import _
 from z3c.relationfield.schema import RelationChoice, RelationList
 from zope.interface import provider
 
 
 @provider(IFormFieldProvider)
 class IRelatedItems(model.Schema):
     """Behavior, which provides the same functionality as the
     plone.app.relationfield IRelatedItems behavior, BUT it uses a different
     widget.
 
     """
 
     fieldset('categorization',
-             label=_(u'Categorization'),
+             label=pmf('Categorization'),
              fields=['relatedItems'])
 
     directives.widget(relatedItems=ReferenceWidgetFactory)
     relatedItems = RelationList(
-        title=_(u'label_related_items', default=u'Related Items'),
+        title=_('label_related_items', default='Related Items'),
         default=[],
         value_type=RelationChoice(title=u"Related",
                                   source=ReferenceObjSourceBinder()),
         required=False,
     )
 
 
 @provider(IFormFieldProvider)
 class IRelationChoiceExample(model.Schema):
     """Demo behavior containing a RelationChoice (single value).
 
     """
     directives.widget(realtionchoice=ReferenceWidgetFactory)
     realtionchoice = RelationChoice(
-        title=_(u'Related Choice'),
+        title=_('Related Choice'),
         source=ReferenceObjSourceBinder(),
         default=None,
         required=False,
     )
 
 
 class CustomSelectableClass(DefaultSelectable):
@@ -56,31 +57,31 @@
 class IRelationChoiceRestricted(model.Schema):
     """Demo behavior containing a RelationChoice (single value).
     But it's not allowd to reference a folder.
 
     """
     directives.widget(realtionchoice_restricted=ReferenceWidgetFactory)
     realtionchoice_restricted = RelationChoice(
-        title=_(u'Related Choice Restricted'),
+        title=_('Related Choice Restricted'),
         source=ReferenceObjSourceBinder(
             nonselectable=['Folder']),
         default=None,
         required=False,
     )
 
     directives.widget(realtionchoice_restricted_title=ReferenceWidgetFactory)
     realtionchoice_restricted_title = RelationChoice(
-        title=_(u'Related Choice Restricted Title'),
+        title=_('Related Choice Restricted Title'),
         source=ReferenceObjSourceBinder(
             selectable_class=CustomSelectableClass),
         default=None,
         required=False,
     )
 
     directives.widget(realtionchoice_restricted_path=ReferenceWidgetFactory)
     realtionchoice_restricted_path = RelationChoice(
-        title=_(u'Related Choice Restricted Title'),
+        title=_('Related Choice Restricted Title'),
         source=ReferenceObjSourceBinder(
             root_path='/testfolder'),
         default=None,
         required=False,
     )
```

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/browser/configure.zcml` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/browser/utils.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/browser/utils.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/configure.zcml` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         factory=".widget.ReferenceWidgetFactory"
         provides="z3c.form.interfaces.IFieldWidget"
         for="z3c.relationfield.interfaces.IRelation" />
 
 
     <plone:behavior
         title="Related items"
-        description="Adds the ability to assign related items"
+        description="Adds the ability to assign related items via ftw.referencewidget"
         provides=".behaviors.IRelatedItems"
         />
 
     <!-- Some behaviors to demonstrate several use-cases -->
     <plone:behavior
         title="Relation choice demo behavior"
         description="Adds the ability to assign one related item"
```

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/converter.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/converter.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/datagridfield.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/datagridfield.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/interfaces.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/interfaces.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/locales/de/LC_MESSAGES/ftw.referencewidget.po` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/locales/de/LC_MESSAGES/ftw.referencewidget.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-08-12 00:19+0000\n"
+"POT-Creation-Date: 2022-08-12 14:49+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -109,15 +109,15 @@
 #: ./ftw/referencewidget/widget.py:90
 msgid "label_reset"
 msgstr "Zurücksetzen"
 
 #. Default: "Search text"
 #: ./ftw/referencewidget/widget.py:94
 msgid "label_searchtext"
-msgstr "Suchtext"
+msgstr "Suche im aktuellen"
 
 #. Default: "Ascending"
 #: ./ftw/referencewidget/widget.py:88
 msgid "label_sort_ascending"
 msgstr "Aufwärts"
 
 #. Default: "Sort by"
@@ -156,7 +156,12 @@
 msgstr "Reihenfolge"
 
 #. Default: "Startpage"
 #: ./ftw/referencewidget/widget.py:91
 msgid "label_startpage"
 msgstr "Startseite"
 
+#. Default: "Total"
+#: ./ftw/referencewidget/widget.py:97
+msgid "label_total"
+msgstr "Total:"
+
```

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/locales/ftw.referencewidget.pot` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/locales/ftw.referencewidget.pot`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #--- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 #SOME DESCRIPTIVE TITLE.
 #FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-08-12 00:19+0000\n"
+"POT-Creation-Date: 2022-08-12 14:49+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -156,7 +156,12 @@
 msgstr ""
 
 #. Default: "Startpage"
 #: ./ftw/referencewidget/widget.py:91
 msgid "label_startpage"
 msgstr ""
 
+#. Default: "Total"
+#: ./ftw/referencewidget/widget.py:97
+msgid "label_total"
+msgstr ""
+
```

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/main.js` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/main.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -2,14 +2,15 @@
 import {
     createApp
 } from "vue";
 import VueAxios from "vue-axios";
 import axios from "axios";
 import qs from "qs";
 import i18n from "./widget/i18n.js";
+import Base from "@patternslib/patternslib/src/core/base";
 
 function axiosInstance() {
     const instance = axios.create({
         paramsSerializer: (params) =>
             qs.stringify(params, {
                 arrayFormat: "repeat"
             }),
@@ -18,27 +19,33 @@
             "Content-Type": "application/json",
             Prefer: "return=representation",
         },
     });
     return instance;
 }
 
-function initReferenceWidget() {
-    document.querySelectorAll(".reference-widget-app").forEach((element) => {
-        if (element.classList.contains("initialized")) {
-            return;
-        }
-
-        const app = createApp(App);
-        app.use(VueAxios, {
-            axios: axiosInstance(),
-        });
-
-        const messages = JSON.parse(element.getAttribute("data-translations"));
-        app.use(i18n, messages);
-        app.mount(element);
-        element.classList.add("initialized");
+function initReferenceWidget(element) {
+    if (element.classList.contains("initialized")) {
+        return;
+    }
+
+    const app = createApp(App);
+    app.use(VueAxios, {
+        axios: axiosInstance(),
     });
+
+    const messages = JSON.parse(element.getAttribute("data-translations"));
+    app.use(i18n, messages);
+    app.mount(element);
+    element.classList.add("initialized");
 }
 
-initReferenceWidget();
-window.initReferenceWidget = initReferenceWidget;
+window.initReferenceWidget = initReferenceWidget;
+
+export default Base.extend({
+    name: "reference-browser-widget",
+    trigger: ".reference-widget-app",
+    parser: "mockup",
+    init() {
+        initReferenceWidget(this.$el[0]);
+    },
+});
```

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/App.vue` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/App.vue`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
           />
           <Pagination
             v-if="data.batching"
             @next="fetchData"
             @previous="fetchData"
             :batching="data.batching"
           />
-          total {{ data.items_total }}
+          {{ $i18n("Total") }} {{ data.items_total }}
 
           <ListItems
             :fetchData="fetchData"
             :items="data.items"
             :selectedItems="selected"
             :inputType="inputType"
             :selectableTypes="selectableTypes"
@@ -45,17 +45,17 @@
     <div class="widget-selected-items">
       <ul class="list-group">
         <li class="list-group-item" v-for="item in selected" :key="item">
           <input
             type="checkbox"
             checked
             :name="fieldName"
-            :value="item.replace(portalURL, portalPath)"
+            :value="item.url.replace(portalURL, portalPath)"
           />
-          {{ item }}
+          {{ item.title }} ({{ item.url }})
         </li>
       </ul>
     </div>
     <button
       type="button"
       class="btn btn-primary"
       data-bs-toggle="collapse"
@@ -134,15 +134,15 @@
     this.$refs.browser.addEventListener("hidden.bs.collapse", () => {
       this.open = false;
     });
   },
   methods: {
     async fetchData(url, options) {
       let params = {
-        metadata_fields: ["UID", "is_folderish", "portal_type"],
+        metadata_fields: ["UID", "is_folderish", "portal_type", "mime_type"],
         sort_on: this.formData.sortOn,
         sort_order: this.formData.sortOrder,
       };
 
       if (!url) {
         url = this.data["@id"];
       }
@@ -206,17 +206,18 @@
         ).hide();
       }
     },
     loadSelectedItems(wrapperElement) {
       wrapperElement.parentElement
         .querySelectorAll(".selected_items input")
         .forEach((element) => {
-          this.selected.push(
-            this.portalURL + element.value.replace(this.portalPath, "")
-          );
+          this.selected.push({
+            title: element.getAttribute("data-title"),
+            url: this.portalURL + element.value.replace(this.portalPath, ""),
+          });
         });
       wrapperElement.parentElement.querySelector(".selected_items").remove();
     },
   },
   computed: {
     browserName() {
       return `reference-widget-browser-${this.fieldName.replace(/\./g, "_")}`;
```

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/components/Breadcrumbs.vue` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/components/Breadcrumbs.vue`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/components/Pagination.vue` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/components/Pagination.vue`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/components/ResolveIcon.vue` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/components/ResolveIcon.vue`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <template>
   <div class="d-inline-block me-1">
     <template v-if="item['@type'] == 'File'">
       <img
-        :src="`${item['@id']}/@@iconresolver/mimetype-${item.file['content-type']}`"
+        :src="`${item['@id']}/@@iconresolver/mimetype-${item['mime_type']}`"
       />
     </template>
     <template v-else-if="item['@type'] == 'Image'">
       <img
-        :src="`${item['@id']}/@@iconresolver/mimetype-${item.image['content-type']}`"
+        :src="`${item['@id']}/@@iconresolver/mimetype-${item['mime_type']}`"
       />
     </template>
     <template v-else>
       <img
         :src="`${item['@id']}/@@iconresolver/${iconMapping[item['@type']]}`"
       />
     </template>
```

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/resources/src/widget/components/searchForm.vue` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/resources/src/widget/components/searchForm.vue`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/selectable.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/selectable.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/sources.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
                  root_path=None):
         self.selectable_class = selectable_class or DefaultSelectable
         self.selectable = selectable or []
         self.nonselectable = nonselectable or []
         self.override = override or False
         self.allow_nonsearched_types = allow_nonsearched_types or False
         self.root_path = root_path
+        self.query = {}  # plone.supermodel compatibility
 
     def __call__(self, context):
 
         if not IContentish.providedBy(context):
             request = getSite().REQUEST
             nb = len(getSite().getPhysicalPath())
             if len(request.PARENTS) >= nb:
```

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/templates/referencewidget_display.pt` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/templates/referencewidget_display.pt`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/templates/referencewidget_input.pt` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/templates/referencewidget_input.pt`

 * *Files 9% similar despite different names*

```diff
@@ -15,28 +15,30 @@
                              data-starturl view/get_start_url;
                              data-portalpath view/portal_path;
                              data-fieldname view/name;
                              data-inputtype view/input_type;
                              data-selectabletypes view/selectable_types;
                              data-traversabletypes view/traversable_types;
                              data-icon-mapping view/icon_mapping;
-                             data-translations view/translations"/>
+                             data-translations view/translations;
+                             data-script-source view/script_resource_url"/>
 
         <script>
                 var body = document.getElementsByTagName('body')[0];
                 var head = document.getElementsByTagName('head')[0];
+                var url = document.querySelector('.reference-widget-app').getAttribute('data-script-source');
                 var loadScript = function(url) {    
                     var script = document.createElement('script');
                     script.type = 'module';
                     script.id = 'referencewidget-js';
-                    script.src = body.getAttribute('data-portal-url') + url;
+                    script.src = url;
                     head.appendChild(script);
                 };
                 if (!document.getElementById('referencewidget-js')) {
-                    loadScript('/++resource++ftw.referencewidget/dist/referencewidget.es.js');
+                    loadScript(url);
                 }
         </script>
 
         <!-- non js hidden field for testing -->
         <input type="hidden" tal:attributes="name view/name" />
     </div>
```

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/testing.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/testing.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/__init__.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_change_widget_config.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_change_widget_config.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_converter.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_datagrid_field.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_datagrid_field.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_override.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_override.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_related_items_behavior.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_related_items_behavior.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_relation_choice.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_relation_choice.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_source.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/test_utils.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/views/form.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/views/form.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/tests/widgets.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/tests/widgets.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/ftw/referencewidget/widget.py` & `ftw.referencewidget-4.0.0b2/ftw/referencewidget/widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 from Acquisition import aq_parent
 from ftw.referencewidget import _
 from ftw.referencewidget.browser.utils import get_path_from_widget_start
 from ftw.referencewidget.browser.utils import get_selectable_types
 from ftw.referencewidget.browser.utils import get_traversal_types
 from ftw.referencewidget.browser.utils import is_traversable
 from ftw.referencewidget.interfaces import IReferenceWidget
+from ftw.referencewidget.sources import ReferenceObjSourceBinder
 from plone import api
 from plone.app.redirector.interfaces import IRedirectionStorage
 from Products.CMFCore.Expression import createExprContext
+from Products.CMFPlone.resources.webresource import PloneScriptResource
 from Products.CMFPlone.utils import safe_unicode
 from z3c.form.browser import widget
 from z3c.form.interfaces import IFieldWidget
 from z3c.form.interfaces import IFormLayer
 from z3c.form.widget import FieldWidget
 from z3c.form.widget import Widget
+from z3c.relationfield.schema import RelationChoice
 from zope.component import adapter
 from zope.component import queryUtility
 from zope.i18n import translate
 from zope.interface import implementer
 from zope.interface import implementer_only
+from zope.schema.interfaces import IContextSourceBinder
 from zope.schema.interfaces import IList
 import json
 
 
 @implementer_only(IReferenceWidget)
 class ReferenceBrowserWidget(widget.HTMLTextInputWidget, Widget):
     """ Datepicker widget. """
@@ -60,14 +64,19 @@
         self.traversal_query = traversal_query
 
     def update(self):
         super(ReferenceBrowserWidget, self).update()
         # if isinstance(self.form, DataGridFieldObjectSubForm):
         #     self.context = self.form.__parent__.__parent__.context
 
+        # Make supermodel with keywordwidget (single select) work
+        if isinstance(self.field, RelationChoice):
+            if not IContextSourceBinder.providedBy(self.field.vocabulary):
+                self.field.vocabulary = ReferenceObjSourceBinder()
+
         widget.addFieldClass(self)
 
     def input_type(self):
         if IList.providedBy(self.field):
             return 'checkbox'
         else:
             return 'radio'
@@ -90,14 +99,15 @@
             'Reset': self._translate(_(u"label_reset", default="Reset")),
             'Startpage': self._translate(_(u"label_startpage", default="Startpage")),
             'Previous': self._translate(_(u"label_previous", default="Previous")),
             'Next': self._translate(_(u"label_next", default="Next")),
             'Search text': self._translate(_(u"label_searchtext", default="Search text")),
             'Close': self._translate(_(u"label_close", default="Close")),
             'Browse': self._translate(_(u"label_browse", default="Browse")),
+            'Total': self._translate(_(u"label_total", default="Total")),
         }
         return json.dumps(messages)
 
     def get_object_by_path(self, path):
         storage = queryUtility(IRedirectionStorage)
 
         if isinstance(path, bytes):
@@ -168,14 +178,26 @@
         for fti in api.portal.get_tool('portal_types').objectValues():
             icon = fti.getIconExprObject()
             if icon:
                 icon = icon(expr_context)
             mapping[fti.getId()] = icon
         return json.dumps(mapping)
 
+    def script_resource_url(self):
+        resource = PloneScriptResource(
+            context=self.context,
+            name="reference-browser-widget",
+            depends="",
+            resource='/++resource++ftw.referencewidget/dist/referencewidget.es.js',
+            include=True,
+            unique=True,
+            integrity=True,
+        )
+        return resource.resource_url(api.portal.get().absolute_url())
+
 
 @adapter(IReferenceWidget, IFormLayer)
 @implementer(IFieldWidget)
 def ReferenceWidgetFactory(field,
                            request,
                            block_traversal=[],
                            allow_traversal=[],
```

### Comparing `ftw.referencewidget-4.0.0b1/ftw.referencewidget.egg-info/SOURCES.txt` & `ftw.referencewidget-4.0.0b2/ftw.referencewidget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.0b1/setup.py` & `ftw.referencewidget-4.0.0b2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-version = '4.0.0b1'
+version = '4.0.0b2'
 maintainer = 'Mathias Leimgruber'
 
 tests_require = [
     'collective.z3cform.datagridfield',
     'plone.app.testing',
     'ftw.builder',
     'ftw.testing',
@@ -22,21 +22,23 @@
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Framework :: Plone',
           'Framework :: Plone :: 6.0',
           'Intended Audience :: Developers',
           'Programming Language :: Python',
           'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
       ],
 
-      keywords='ftw 4teamwork widget reference browser',
-      author='%s, 4teamwork AG' % maintainer,
-      author_email='mailto:info@4teamwork.ch',
+      keywords='webcloud7 widget reference browser',
+      author='%s, webcloud7 ag' % maintainer,
+      author_email='mailto:info@webcloud7.ch',
       maintainer=maintainer,
-      url='https://github.com/4teamwork/ftw.referencewidget',
+      url='https://github.com/webcloud7/ftw.referencewidget',
 
       license='GPL2',
       packages=find_packages(exclude=['ez_setup']),
       namespace_packages=['ftw'],
       include_package_data=True,
       zip_safe=False,
```

