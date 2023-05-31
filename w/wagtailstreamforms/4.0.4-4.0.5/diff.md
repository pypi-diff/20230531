# Comparing `tmp/wagtailstreamforms-4.0.4.tar.gz` & `tmp/wagtailstreamforms-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailstreamforms-4.0.4.tar", last modified: Fri Apr 21 07:59:07 2023, max compression
+gzip compressed data, was "wagtailstreamforms-4.0.5.tar", last modified: Wed May 31 08:31:46 2023, max compression
```

## Comparing `wagtailstreamforms-4.0.4.tar` & `wagtailstreamforms-4.0.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.699855 wagtailstreamforms-4.0.4/wagtailstreamforms/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.699855 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.699855 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.699855 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.699855 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.699855 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.699855 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.699855 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/wagtailstreamforms/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/wagtailstreamforms/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/management/commands/prunesubmissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/wagtailstreamforms/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    26213 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/migrations/0002_form_site.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/migrations/0003_alter_form_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/wagtailstreamforms/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/models/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/models/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/streamfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.699855 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/advanced_settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/confirm_copy.html
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/form_block.html
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/index_submissions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/list_submissions.html
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/non_existent_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/partials/form_field.html
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.699855 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/wagtailadmin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/wagtailstreamforms/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/templatetags/streamforms_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/wagtailstreamforms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/utils/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/utils/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.703856 wagtailstreamforms-4.0.4/wagtailstreamforms/views/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/views/advanced_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/views/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/views/submission_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/views/submission_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/wagtailstreamforms_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-21 07:59:03.000000 wagtailstreamforms-4.0.4/wagtailstreamforms/wagtailstreamforms_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:59:07.699855 wagtailstreamforms-4.0.4/wagtailstreamforms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-21 07:59:07.000000 wagtailstreamforms-4.0.4/wagtailstreamforms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-21 07:59:07.000000 wagtailstreamforms-4.0.4/wagtailstreamforms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 07:59:07.000000 wagtailstreamforms-4.0.4/wagtailstreamforms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-21 07:59:07.000000 wagtailstreamforms-4.0.4/wagtailstreamforms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 07:59:07.000000 wagtailstreamforms-4.0.4/wagtailstreamforms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.813808 wagtailstreamforms-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 08:31:40.000000 wagtailstreamforms-4.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-31 08:31:40.000000 wagtailstreamforms-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-31 08:31:46.813808 wagtailstreamforms-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-31 08:31:40.000000 wagtailstreamforms-4.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 08:31:40.000000 wagtailstreamforms-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-31 08:31:46.813808 wagtailstreamforms-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-31 08:31:40.000000 wagtailstreamforms-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.809807 wagtailstreamforms-4.0.5/wagtailstreamforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 08:31:40.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-31 08:31:40.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-31 08:31:40.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-31 08:31:40.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-31 08:31:40.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-31 08:31:40.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.805807 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.805807 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.809807 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-31 08:31:40.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.805807 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.809807 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.805807 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.809807 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.809807 wagtailstreamforms-4.0.5/wagtailstreamforms/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.809807 wagtailstreamforms-4.0.5/wagtailstreamforms/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/management/commands/prunesubmissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.809807 wagtailstreamforms-4.0.5/wagtailstreamforms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    26213 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/migrations/0002_form_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/migrations/0003_alter_form_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.809807 wagtailstreamforms-4.0.5/wagtailstreamforms/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/models/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/models/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/streamfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.805807 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.813808 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/advanced_settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/confirm_copy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/form_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/index_submissions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/list_submissions.html
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/non_existent_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.813808 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/partials/form_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.805807 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/wagtailadmin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.813808 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.813808 wagtailstreamforms-4.0.5/wagtailstreamforms/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/templatetags/streamforms_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.813808 wagtailstreamforms-4.0.5/wagtailstreamforms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/utils/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/utils/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.813808 wagtailstreamforms-4.0.5/wagtailstreamforms/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/views/advanced_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/views/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/views/submission_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/views/submission_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/wagtailstreamforms_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 08:31:41.000000 wagtailstreamforms-4.0.5/wagtailstreamforms/wagtailstreamforms_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:46.809807 wagtailstreamforms-4.0.5/wagtailstreamforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-31 08:31:46.000000 wagtailstreamforms-4.0.5/wagtailstreamforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-31 08:31:46.000000 wagtailstreamforms-4.0.5/wagtailstreamforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:31:46.000000 wagtailstreamforms-4.0.5/wagtailstreamforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-31 08:31:46.000000 wagtailstreamforms-4.0.5/wagtailstreamforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 08:31:46.000000 wagtailstreamforms-4.0.5/wagtailstreamforms.egg-info/top_level.txt
```

### Comparing `wagtailstreamforms-4.0.4/LICENSE` & `wagtailstreamforms-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/PKG-INFO` & `wagtailstreamforms-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailstreamforms
-Version: 4.0.4
+Version: 4.0.5
 Summary: Wagtail forms in a streamfield
 Home-page: https://github.com/AccentDesign/wagtailstreamforms/
 Author: Stuart George
 Author-email: stuart@accentdesign.co.uk
 License: MIT
 Download-URL: https://pypi.python.org/pypi/wagtailstreamforms
 Description: Wagtail StreamForms
```

### Comparing `wagtailstreamforms-4.0.4/README.rst` & `wagtailstreamforms-4.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/setup.py` & `wagtailstreamforms-4.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/blocks.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/conf.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/conf.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/fields.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/forms.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/forms.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/hooks.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo` & `wagtailstreamforms-4.0.5/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/locale/es/LC_MESSAGES/django.po` & `wagtailstreamforms-4.0.5/wagtailstreamforms/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo` & `wagtailstreamforms-4.0.5/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po` & `wagtailstreamforms-4.0.5/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po` & `wagtailstreamforms-4.0.5/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/management/commands/prunesubmissions.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/management/commands/prunesubmissions.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/migrations/0001_initial.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/migrations/0002_form_site.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/migrations/0002_form_site.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/migrations/0003_alter_form_fields.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/migrations/0003_alter_form_fields.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/models/__init__.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/models/file.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/models/file.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/models/form.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/models/form.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/models/submission.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/models/submission.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/streamfield.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/streamfield.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/advanced_settings.html` & `wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/advanced_settings.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/confirm_copy.html` & `wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/confirm_copy.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/confirm_delete.html` & `wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/index_submissions.html` & `wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/index_submissions.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/list_submissions.html` & `wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/list_submissions.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html` & `wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html` & `wagtailstreamforms-4.0.5/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/templatetags/streamforms_tags.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/templatetags/streamforms_tags.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/urls.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/utils/apps.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/utils/apps.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/utils/loading.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/utils/loading.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/views/advanced_settings.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/views/advanced_settings.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/views/copy.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/views/copy.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/views/submission_delete.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/views/submission_delete.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/views/submission_list.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/views/submission_list.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/wagtail_hooks.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/wagtailstreamforms_fields.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/wagtailstreamforms_fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,17 +208,35 @@
                 ("required", blocks.BooleanBlock(required=False)),
             ],
             icon=self.icon,
             label=self.label,
         )
 
 
+class MultipleFileInput(forms.ClearableFileInput):
+    allow_multiple_selected = True
+
+
+class MultipleFileField(forms.FileField):
+    def __init__(self, *args, **kwargs):
+        kwargs.setdefault("widget", MultipleFileInput())
+        super().__init__(*args, **kwargs)
+
+    def clean(self, data, initial=None):
+        single_file_clean = super().clean
+        if data and isinstance(data, (list, tuple)):
+            result = [single_file_clean(d, initial) for d in data]
+        else:
+            result = single_file_clean(data, initial)
+        return result
+
+
 class MultiFileField(BaseField):
-    field_class = forms.FileField
-    widget = forms.widgets.FileInput(attrs={"multiple": True})
+    field_class = MultipleFileField
+    widget = MultipleFileInput(attrs={"multiple": True})
     icon = "doc-full-inverse"
     label = _("Files field")
 
     def get_form_block(self):
         return blocks.StructBlock(
             [
                 ("label", blocks.CharBlock()),
```

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms/wagtailstreamforms_hooks.py` & `wagtailstreamforms-4.0.5/wagtailstreamforms/wagtailstreamforms_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms.egg-info/PKG-INFO` & `wagtailstreamforms-4.0.5/wagtailstreamforms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailstreamforms
-Version: 4.0.4
+Version: 4.0.5
 Summary: Wagtail forms in a streamfield
 Home-page: https://github.com/AccentDesign/wagtailstreamforms/
 Author: Stuart George
 Author-email: stuart@accentdesign.co.uk
 License: MIT
 Download-URL: https://pypi.python.org/pypi/wagtailstreamforms
 Description: Wagtail StreamForms
```

### Comparing `wagtailstreamforms-4.0.4/wagtailstreamforms.egg-info/SOURCES.txt` & `wagtailstreamforms-4.0.5/wagtailstreamforms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

