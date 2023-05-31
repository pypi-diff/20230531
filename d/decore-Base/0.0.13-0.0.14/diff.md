# Comparing `tmp/decore_Base-0.0.13.tar.gz` & `tmp/decore_Base-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decore_Base-0.0.13.tar", last modified: Fri May 26 20:03:48 2023, max compression
+gzip compressed data, was "decore_Base-0.0.14.tar", last modified: Wed May 31 12:31:49 2023, max compression
```

## Comparing `decore_Base-0.0.13.tar` & `decore_Base-0.0.14.tar`

### file list

```diff
@@ -1,156 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.512316 decore_Base-0.0.13/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.492315 decore_Base-0.0.13/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-26 20:03:39.000000 decore_Base-0.0.13/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.492315 decore_Base-0.0.13/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-26 20:03:39.000000 decore_Base-0.0.13/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-26 20:03:39.000000 decore_Base-0.0.13/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.496315 decore_Base-0.0.13/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-26 20:03:39.000000 decore_Base-0.0.13/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 20:03:39.000000 decore_Base-0.0.13/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-26 20:03:39.000000 decore_Base-0.0.13/KOFI.md
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-26 20:03:39.000000 decore_Base-0.0.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-26 20:03:48.516316 decore_Base-0.0.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-26 20:03:39.000000 decore_Base-0.0.13/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-26 20:03:39.000000 decore_Base-0.0.13/README_DE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.496315 decore_Base-0.0.13/decore_Base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-26 20:03:48.000000 decore_Base-0.0.13/decore_Base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-05-26 20:03:48.000000 decore_Base-0.0.13/decore_Base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:03:48.000000 decore_Base-0.0.13/decore_Base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 20:03:48.000000 decore_Base-0.0.13/decore_Base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 20:03:48.000000 decore_Base-0.0.13/decore_Base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.496315 decore_Base-0.0.13/decore_base/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.496315 decore_Base-0.0.13/decore_base/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/classes/decore_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/decore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.496315 decore_Base-0.0.13/decore_base/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/docs/social_header.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.496315 decore_Base-0.0.13/decore_base/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/extensions/conform_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.500316 decore_Base-0.0.13/decore_base/extensions/depricated/
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/extensions/depricated/askform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/extensions/depricated/buyform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/extensions/depricated/conform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/extensions/depricated/deform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/extensions/perform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/extensions/reform_client_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/extensions/reform_server_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.500316 decore_Base-0.0.13/decore_base/library/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.500316 decore_Base-0.0.13/decore_base/library/particl_market/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/library/particl_market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/library/particl_market/particl_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/library/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/library/powershell2.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/library/return_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.500316 decore_Base-0.0.13/decore_base/library/roaster/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/library/roaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/library/roaster/roaster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/library/roaster/roaster_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/library/roaster/roaster_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.500316 decore_Base-0.0.13/decore_base/prepare/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.500316 decore_Base-0.0.13/decore_base/prepare/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/.vscode/launch.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.492315 decore_Base-0.0.13/decore_base/prepare/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.500316 decore_Base-0.0.13/decore_base/prepare/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.500316 decore_Base-0.0.13/decore_base/prepare/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/css/912.77e6bcbe.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    64483 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.504315 decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.504315 decore_Base-0.0.13/decore_base/prepare/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.504315 decore_Base-0.0.13/decore_base/prepare/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    29630 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/js/912.e7a2b7ea.js
--rw-r--r--   0 runner    (1001) docker     (123)    17942 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/js/app.7ef3a1f6.js
--rw-r--r--   0 runner    (1001) docker     (123)   380277 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/static/js/vendor.03c46c80.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.504315 decore_Base-0.0.13/decore_base/prepare/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/prepare/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.504315 decore_Base-0.0.13/decore_base/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.504315 decore_Base-0.0.13/decore_base/sample/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.508316 decore_Base-0.0.13/decore_base/sample/bases/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/bases/account_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/bases/company_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/bases/global_management_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/bases/information_stytem_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/bases/person_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/language.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.508316 decore_Base-0.0.13/decore_base/sample/models/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/models/account_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/models/company_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/models/person_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.492315 decore_Base-0.0.13/decore_base/sample/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.508316 decore_Base-0.0.13/decore_base/sample/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.508316 decore_Base-0.0.13/decore_base/sample/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/css/912.77e6bcbe.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    64483 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.512316 decore_Base-0.0.13/decore_base/sample/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.512316 decore_Base-0.0.13/decore_base/sample/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.512316 decore_Base-0.0.13/decore_base/sample/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    29630 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/js/912.e7a2b7ea.js
--rw-r--r--   0 runner    (1001) docker     (123)    17942 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/js/app.7ef3a1f6.js
--rw-r--r--   0 runner    (1001) docker     (123)   380277 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/static/js/vendor.03c46c80.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.512316 decore_Base-0.0.13/decore_base/sample/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:03:48.512316 decore_Base-0.0.13/decore_base/sample/state/
--rw-r--r--   0 runner    (1001) docker     (123)  1290240 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/state/database.db
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/state/keybase.kdbx
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-05-26 20:03:39.000000 decore_Base-0.0.13/decore_base/sample/state/querybase.db
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 20:03:39.000000 decore_Base-0.0.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 20:03:39.000000 decore_Base-0.0.13/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-26 20:03:48.516316 decore_Base-0.0.13/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.295996 decore_Base-0.0.14/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.251995 decore_Base-0.0.14/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-31 12:31:41.000000 decore_Base-0.0.14/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.251995 decore_Base-0.0.14/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-31 12:31:41.000000 decore_Base-0.0.14/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-31 12:31:41.000000 decore_Base-0.0.14/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.251995 decore_Base-0.0.14/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-31 12:31:41.000000 decore_Base-0.0.14/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 12:31:41.000000 decore_Base-0.0.14/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-31 12:31:41.000000 decore_Base-0.0.14/KOFI.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-31 12:31:41.000000 decore_Base-0.0.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-31 12:31:49.295996 decore_Base-0.0.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-31 12:31:41.000000 decore_Base-0.0.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-31 12:31:41.000000 decore_Base-0.0.14/README_DE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.255995 decore_Base-0.0.14/decore_Base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-31 12:31:49.000000 decore_Base-0.0.14/decore_Base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-31 12:31:49.000000 decore_Base-0.0.14/decore_Base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:31:49.000000 decore_Base-0.0.14/decore_Base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-31 12:31:49.000000 decore_Base-0.0.14/decore_Base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 12:31:49.000000 decore_Base-0.0.14/decore_Base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.255995 decore_Base-0.0.14/decore_base/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.259995 decore_Base-0.0.14/decore_base/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/decore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.259995 decore_Base-0.0.14/decore_base/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/docs/social_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.263995 decore_Base-0.0.14/decore_base/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.263995 decore_Base-0.0.14/decore_base/library/particl_market/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/particl_market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/particl_market/particl_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/powershell2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/return_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.263995 decore_Base-0.0.14/decore_base/library/roaster/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/roaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/roaster/roaster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/roaster/roaster_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/roaster/roaster_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.263995 decore_Base-0.0.14/decore_base/prepare/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.263995 decore_Base-0.0.14/decore_base/prepare/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/.vscode/launch.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.243995 decore_Base-0.0.14/decore_base/prepare/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.263995 decore_Base-0.0.14/decore_base/prepare/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.267995 decore_Base-0.0.14/decore_base/prepare/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/css/912.77e6bcbe.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    64483 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.271995 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.271995 decore_Base-0.0.14/decore_base/prepare/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.275995 decore_Base-0.0.14/decore_base/prepare/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29907 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/js/912.f638ed14.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/js/app.465385a3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   380277 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/js/vendor.03c46c80.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.275995 decore_Base-0.0.14/decore_base/prepare/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.275995 decore_Base-0.0.14/decore_base/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.275995 decore_Base-0.0.14/decore_base/sample/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.279996 decore_Base-0.0.14/decore_base/sample/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/account_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/company_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/global_management_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/information_stytem_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/person_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/language.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.279996 decore_Base-0.0.14/decore_base/sample/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/models/account_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/models/company_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/models/person_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/models/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.247995 decore_Base-0.0.14/decore_base/sample/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.279996 decore_Base-0.0.14/decore_base/sample/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.279996 decore_Base-0.0.14/decore_base/sample/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/css/912.77e6bcbe.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    64483 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.287996 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.287996 decore_Base-0.0.14/decore_base/sample/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.287996 decore_Base-0.0.14/decore_base/sample/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29907 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/js/912.f638ed14.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/js/app.465385a3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   380277 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/js/vendor.03c46c80.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.291996 decore_Base-0.0.14/decore_base/sample/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.291996 decore_Base-0.0.14/decore_base/sample/state/
+-rw-r--r--   0 runner    (1001) docker     (123)  1306624 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/state/database.db
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/state/keybase.kdbx
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/state/querybase.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.295996 decore_Base-0.0.14/decore_base/uniform/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/conform_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.295996 decore_Base-0.0.14/decore_base/uniform/depricated/
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/depricated/askform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/depricated/buyform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/depricated/conform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/depricated/deform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/perform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/reform_client_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/reform_server_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-31 12:31:41.000000 decore_Base-0.0.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-31 12:31:41.000000 decore_Base-0.0.14/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-31 12:31:49.295996 decore_Base-0.0.14/setup.cfg
```

### Comparing `decore_Base-0.0.13/.github/FUNDING.yml` & `decore_Base-0.0.14/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/.gitignore` & `decore_Base-0.0.14/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/.vscode/launch.json` & `decore_Base-0.0.14/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/KOFI.md` & `decore_Base-0.0.14/KOFI.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# decore Base | crafting UI simply
+
 # decore Base | open source on github
 
 decore Base is now available on github. 
 
 Still very incomplete but to better visualize the running process I decided to publish the code on github.
 
 The documentation is not yet complete and will be expanded over time.
```

### Comparing `decore_Base-0.0.13/LICENSE` & `decore_Base-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/PKG-INFO` & `decore_Base-0.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decore_Base
-Version: 0.0.13
+Version: 0.0.14
 Summary: decore Base is a "Python to Vue.js" open source package that helps you go from idea to view in a few simple steps. It is targeted to those who want to focus on the results of their algorithms, do scientific work, perform promotional teaching or learning functions.
 Home-page: https://github.com/KemoPanzah/decore_Base
 Author: Kemo Panzah
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
```

### Comparing `decore_Base-0.0.13/README.md` & `decore_Base-0.0.14/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Documentation
-decore Base is a "Python to Vue.js" open source package that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms , do scientific work, or perform teaching or learning functions.
+decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms , do scientific work, or perform teaching or learning functions.
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/P5P2JCC5B)
 
-**decore Base is still under development, only available for Windows and not yet ready for production.**
+**decore Base is currently a work in progress, only locally deployable, only available for Windows and not yet ready for production.**
 
 The recommended IDE is Visual Studio Code and all my comments and documentation here will also refer to vscode only.
 
 [Insight into the current progress of the decore project](https://github.com/users/KemoPanzah/projects/1/views/1)
 
 ## Contribution
 The biggest help I can get right now is if you take a look at the project and tell me what you think. I am grateful for any criticism.
@@ -102,25 +102,34 @@
 ## Api reference
 To create a GUI with decore Base, you decorate functions in the source code according to the default of the execution process.
 
 The decore module contains those functions that are needed to create the metadata for the decore front application.
 
 To understand the general approach, synchronize the sample application with the command `python app.py --sample` in your project root directory.
 
-### @decore.app()
-### @decore.base()
-### @decore.view()
-### @decore.dialog()
-### @decore.widget()
-### @decore.action()
+#### @decore.app()
+#### @decore.base()
+#### @decore.view()
+#### @decore.dialog()
+#### @decore.widget()
+#### @decore.action()
 
 ## Model reference
-To make working with the original Peewee model even easier, some functions have been added to the model.
+To simplify the work with the original Peewee model even more, the model was extended by some functions.
 
-!DESCRIPTION FOLLOWS!
+### Fields
+The following fields are currently usable in decore Base and are evaluated by the frontend.
+
+#### BackRefMetaField
+#### CharField
+#### ForeignKeyField
+#### IntegerField
+#### ManyToManyField
+#### PasswordField
+#### TextField
 
 ## Component processing
 ```mermaid
 graph
 A[Base] --> B[View]
 B --> Z[Action]
 B --> C[Dialog]
```

### Comparing `decore_Base-0.0.13/README_DE.md` & `decore_Base-0.0.14/README_DE.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Documentation
-decore Base ist ein "Python to Vue.js"-Open-Source-Paket, das Ihnen hilft, in wenigen einfachen Schritten von der Idee zur Ansicht zu gelangen. Es richtet sich an diejenigen, die sich auf die Ergebnisse ihrer Algorithmen konzentrieren , wissenschaftlich arbeiten wollen, oder Lehr- bzw. Lernfunktionen ausüben.
+decore Base ist ein Out-Of-The-Box "Python to Vue.js" Daten-Anwendungs-Dashboard, das Ihnen hilft, in wenigen einfachen Schritten von der Idee zur Ansicht zu gelangen. Es richtet sich an diejenigen, die sich auf die Ergebnisse ihrer Algorithmen konzentrieren , wissenschaftlich arbeiten wollen, oder Lehr- bzw. Lernfunktionen ausüben.
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/P5P2JCC5B)
 
-**decore Base ist im Moment noch in Arbeit, nur für Windows verfügbar und noch nicht bereit für die Produktion.**
+**decore Base ist im Moment noch in Arbeit, nur lokal einsetzbar, nur für Windows verfügbar und noch nicht bereit für die Produktion.**
 
 Die empfohlene IDE ist Visual Studio Code und alle meine Ausführungen und Dokumentationen werden sich hier auch nur auf vscode beziehen.
 
 [Einsicht in den derzeitigen Vortschritt des decore Projektes](https://github.com/users/KemoPanzah/projects/1/views/1)
 
 ## Contribution
 Die größte Hilfe die ich derzeit bekommen kann ist, wenn ihr Euch das Projekt anschaut und mir eure Meinung dazu mitteilt. Ich bin für jede Kritik dankbar. 
@@ -103,25 +103,34 @@
 ## Api reference
 Um eine GUI mit decore Base zu erstellen, dekoriert man Funktionen im Quellcode nach der Vorgabe des Abarbeitungsprozesses.
 
 Das decore Modul enthält jene Funktionen die bei der Erstellung der Metadaten für die decore Front Applikation benötigt werden.
 
 Um die allgemeine Herangehensweise zu verstehen synchronisieren Sie sich die Sample Applikation mit dem Befehl `python app.py --sample` in Ihrem Projektstammverzeichnis.
 
-### @decore.app()
-### @decore.base()
-### @decore.view()
-### @decore.dialog()
-### @decore.widget()
-### @decore.action()
+#### @decore.app()
+#### @decore.base()
+#### @decore.view()
+#### @decore.dialog()
+#### @decore.widget()
+#### @decore.action()
 
 ## Model reference
 Um die Arbeit mit dem originalen Peewee-Model noch weiter zu vereinfachen, wurde das Model um einige funktionen erweitert.
 
-!BESCHREIBUNG FOLGT!
+### Fields
+Folgende Felder sind derzeit in decore Base nutzbar und werden vom Frontend ausgewertet.
+
+#### BackRefMetaField
+#### CharField
+#### ForeignKeyField
+#### IntegerField
+#### ManyToManyField
+#### PasswordField
+#### TextField
 
 ## Component processing
 ```mermaid
 graph
 A[Base] --> B[View]
 B --> Z[Action]
 B --> C[Dialog]
```

### Comparing `decore_Base-0.0.13/decore_Base.egg-info/PKG-INFO` & `decore_Base-0.0.14/decore_Base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decore-Base
-Version: 0.0.13
+Version: 0.0.14
 Summary: decore Base is a "Python to Vue.js" open source package that helps you go from idea to view in a few simple steps. It is targeted to those who want to focus on the results of their algorithms, do scientific work, perform promotional teaching or learning functions.
 Home-page: https://github.com/KemoPanzah/decore_Base
 Author: Kemo Panzah
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
```

### Comparing `decore_Base-0.0.13/decore_Base.egg-info/SOURCES.txt` & `decore_Base-0.0.14/decore_Base.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,22 +31,14 @@
 decore_base/classes/decore_prompt.py
 decore_base/classes/decore_query.py
 decore_base/classes/decore_return.py
 decore_base/classes/decore_translate.py
 decore_base/classes/decore_view.py
 decore_base/classes/decore_widget.py
 decore_base/docs/social_header.txt
-decore_base/extensions/conform_model.py
-decore_base/extensions/perform_model.py
-decore_base/extensions/reform_client_model.py
-decore_base/extensions/reform_server_model.py
-decore_base/extensions/depricated/askform_base.py
-decore_base/extensions/depricated/buyform_base.py
-decore_base/extensions/depricated/conform_base.py
-decore_base/extensions/depricated/deform_base.py
 decore_base/library/__init__.py
 decore_base/library/powershell.py
 decore_base/library/powershell2.py
 decore_base/library/return_value.py
 decore_base/library/particl_market/__init__.py
 decore_base/library/particl_market/particl_market.py
 decore_base/library/roaster/__init__.py
@@ -70,33 +62,35 @@
 decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
 decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
 decore_base/prepare/spa/static/icons/favicon-128x128.png
 decore_base/prepare/spa/static/icons/favicon-16x16.png
 decore_base/prepare/spa/static/icons/favicon-32x32.png
 decore_base/prepare/spa/static/icons/favicon-96x96.png
 decore_base/prepare/spa/static/js/65.940d9b80.js
-decore_base/prepare/spa/static/js/912.e7a2b7ea.js
-decore_base/prepare/spa/static/js/app.7ef3a1f6.js
+decore_base/prepare/spa/static/js/912.f638ed14.js
+decore_base/prepare/spa/static/js/app.465385a3.js
 decore_base/prepare/spa/static/js/vendor.03c46c80.js
 decore_base/prepare/spa/templates/index.html
 decore_base/sample/.gitignore
 decore_base/sample/app.py
 decore_base/sample/config.json
 decore_base/sample/language.json
 decore_base/sample/.vscode/launch.json
 decore_base/sample/.vscode/settings.json
 decore_base/sample/bases/__init__.py
 decore_base/sample/bases/account_base.py
 decore_base/sample/bases/company_base.py
 decore_base/sample/bases/global_management_base.py
 decore_base/sample/bases/information_stytem_base.py
 decore_base/sample/bases/person_base.py
+decore_base/sample/bases/test_base.py
 decore_base/sample/models/account_model.py
 decore_base/sample/models/company_model.py
 decore_base/sample/models/person_model.py
+decore_base/sample/models/test_model.py
 decore_base/sample/spa/static/favicon.ico
 decore_base/sample/spa/static/css/912.77e6bcbe.css
 decore_base/sample/spa/static/css/app.d398f07d.css
 decore_base/sample/spa/static/css/vendor.14c9ac7a.css
 decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
@@ -108,14 +102,23 @@
 decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
 decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
 decore_base/sample/spa/static/icons/favicon-128x128.png
 decore_base/sample/spa/static/icons/favicon-16x16.png
 decore_base/sample/spa/static/icons/favicon-32x32.png
 decore_base/sample/spa/static/icons/favicon-96x96.png
 decore_base/sample/spa/static/js/65.940d9b80.js
-decore_base/sample/spa/static/js/912.e7a2b7ea.js
-decore_base/sample/spa/static/js/app.7ef3a1f6.js
+decore_base/sample/spa/static/js/912.f638ed14.js
+decore_base/sample/spa/static/js/app.465385a3.js
 decore_base/sample/spa/static/js/vendor.03c46c80.js
 decore_base/sample/spa/templates/index.html
 decore_base/sample/state/database.db
 decore_base/sample/state/keybase.kdbx
-decore_base/sample/state/querybase.db
+decore_base/sample/state/querybase.db
+decore_base/uniform/__init__.py
+decore_base/uniform/conform_model.py
+decore_base/uniform/perform_model.py
+decore_base/uniform/reform_client_model.py
+decore_base/uniform/reform_server_model.py
+decore_base/uniform/depricated/askform_base.py
+decore_base/uniform/depricated/buyform_base.py
+decore_base/uniform/depricated/conform_base.py
+decore_base/uniform/depricated/deform_base.py
```

### Comparing `decore_Base-0.0.13/decore_Base.egg-info/requires.txt` & `decore_Base-0.0.14/decore_Base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/classes/decore_base.py` & `decore_Base-0.0.14/decore_base/classes/decore_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from threading import Thread
 
 
 class Decore_base(Decore_object):
     def __init__(self):
         Decore_object.__init__(self, p_id=None, p_parent_id='app', p_source_id=None, p_icon=None, p_title=None, p_desc=None, p_doc=None)
         self.model = None
-        # self.through_model = None
         self.field_s = None
         self.rel_field_s = None
         self.schema = None
         self.function_s = []
 
     def start_inits(self):
         for i_function in self.function_s:
```

### Comparing `decore_Base-0.0.13/decore_base/classes/decore_list.py` & `decore_Base-0.0.14/decore_base/classes/decore_list.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/classes/decore_model.py` & `decore_Base-0.0.14/decore_base/classes/decore_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from ..globals import globals
-from .decore_translate import Decore_translate as t
+import inspect
+import logging
+import operator
+from functools import reduce
+from pathlib import Path, PosixPath, WindowsPath
+from shutil import move
+from uuid import uuid1
 
 from cerberus import Validator
-from functools import reduce
-from pathlib import Path, WindowsPath, PosixPath
 from peewee import *
-from peewee import MetaField, FieldAccessor
+from peewee import FieldAccessor, MetaField
 from playhouse.migrate import *
 from playhouse.reflection import Introspector
 from playhouse.shortcuts import model_to_dict
 from pykeepass.entry import Entry
-from shutil import move
-from uuid import uuid1
-import inspect
-import logging
-import operator
+
+from ..globals import globals
+from .decore_translate import Decore_translate as t
+
 
 class PasswordFieldAccessor(object):
     def __init__(self, model, field, name):
         self.model = model
         self.field = field
         self.name = name
     #TODO - alles nochmal durch debuggen SET und GET
@@ -98,38 +100,23 @@
 class ManyToManyField(ManyToManyField):
     def __init__(self, model, backref=None, on_delete=None, on_update=None, _is_backref=False, verbose_name=None, help_text=None, filter_fields=None):
         super().__init__(model, backref, on_delete, on_update, _is_backref)
         self.verbose_name = verbose_name
         self.help_text = help_text
         self.filter_fields = filter_fields
     
-    def bind(self, model, name, set_attribute=True):
-        super().bind(model, name, set_attribute)
-        self.ref_name = name
-
 class BackRefMetaField(MetaField):
-    def __init__(self, ref_name=None ,verbose_name=None, help_text=None, filter_fields=None):
+    def __init__(self,verbose_name=None, help_text=None, filter_fields=None):
         super().__init__(False, False, False, None, None, False, None, None, None, False, None, help_text, verbose_name, None, None, False)
-        if ref_name:
-            self.ref_name = ref_name
-            self.filter_fields = filter_fields
-        else:
-            raise Exception('ref_name must be set to same name as backref from ManyToManyField or ForeignKeyField in ralated model')
-
-    def bind(self, model, name, set_attribute=True):
-        if name.startswith('br_'):
-            super().bind(model, name, set_attribute)
-        else:
-            raise Exception('Attribute name for BackRefMetaField must start with br_ e.g. br_users')
-
-    def db_value(self, value):
-        return None
+        self.filter_fields = filter_fields
     
-    def python_value(self, value):
-        return None
+    def bind(self, model, name, set_attribute):
+        super().bind(model, name, set_attribute)
+        setattr(model,'br_'+name, getattr(model, name)) 
+        delattr(model, name)
 
 class Decore_model(Model):
     id = CharField(primary_key=True, unique=True, verbose_name="ID")
     title = CharField(verbose_name=t('Title'))
     desc = CharField(verbose_name=t('Description'), null=True)
     item_type = CharField(verbose_name=t('Item type'), default='object')
     parent_path = CharField(verbose_name=t('Parent path'), null=True)
@@ -137,15 +124,15 @@
     class Meta:
         # tbase = SqliteDatabase('state/database.db', pragmas=(('cache_size', -1024 * 64),('journal_mode', 'wal')))
         tbase = SqliteDatabase('state/database.db')
 
     def __init__(self, p_known_id=None, *args, **kwargs):
         Model.__init__(self, *args, **kwargs)
         self.kdb_group = self.get_kdb_group()
-
+        
         # TODO - den Weg über get_or_create testen
         if p_known_id:
             if self.get_or_none(self.__class__.id == p_known_id):
                 self.__data__.update(self.get_by_id(p_known_id).__data__)
 
     @classmethod
     def register(cls):
@@ -180,15 +167,15 @@
                 if not b_db_field_found:
                     migrate(cls._meta.migrator.drop_column(cls._meta.table_name, db_field.column_name, cascade=False))
 
     @classmethod
     @property
     def field_s(cls):
         return list(cls._meta.fields.values())
-    
+
     @classmethod
     @property
     def rel_field_s(cls):
         r_value = []
         for field in cls._meta.backrefs:
             if not 'Through' in field.model.__name__:
                 r_value.append(field)
```

### Comparing `decore_Base-0.0.13/decore_base/classes/decore_pool.py` & `decore_Base-0.0.14/decore_base/classes/decore_pool.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 from .decore_widget import Decore_widget
 from .decore_action import Decore_action
 from .decore_element import Decore_element
 from .decore_function import Decore_function
 from .decore_list import Decore_list
 
 
-
 import inspect
-from peewee import Field
+from peewee import Field, BackrefAccessor, ManyToManyField
 
 
 class Decore_pool(object):
     def __init__(self):
         self.__data__ = dict()
         self.base_s = []
         self.view_s = []
         self.dialog_s = []
         self.widget_s = []
         self.action_s = []
         self.element_s = []
 
+    @property
+    def app(self):
+        return self.__data__['app']
+
     def register(self, p_instance):
         if not p_instance.id in self.__data__:
             self.__data__[p_instance.id] = p_instance
         else:
             raise Exception('instance with the same id already in pool')
     
     def extend(self):
@@ -67,18 +70,28 @@
         if type(p_value) is dict:
             for key, value in p_value.items():
                 t_return[key] = self.serialize(value)
         elif Decore_object in inspect.getmro(p_value.__class__):
             setattr(p_value,'class', p_value.__class__.__name__)
             for key, value in p_value.__dict__.items():
                 t_return[key] = self.serialize(value)
+        elif BackrefAccessor in inspect.getmro(p_value.__class__):
+            p_value = getattr(p_value.model, 'br_'+p_value.field.backref) 
+            setattr(p_value,'class', p_value.__class__.__name__)
+            for key, value in p_value.__dict__.items():
+                t_return[key] = self.serialize(value)
+        elif ManyToManyField in inspect.getmro(p_value.__class__):
+            if p_value._is_backref:
+                p_value.__dict__.update(getattr(p_value.model, 'br_'+p_value.name).__dict__) 
+            setattr(p_value,'class', p_value.__class__.__name__)
+            for key, value in p_value.__dict__.items():
+                t_return[key] = self.serialize(value)
         elif Field in inspect.getmro(p_value.__class__):
             setattr(p_value,'class', p_value.__class__.__name__)
             for key, value in p_value.__dict__.items():
-                # t_return['class'] = str(p_value)
                 t_return[key] = self.serialize(value)
         # TODO - depricated - Decore_list wird nicht mehr benötigt - entferne aus dem gesamten Framework
         elif Decore_list in inspect.getmro(p_value.__class__):
             t_list = []
             for value in p_value:
                 t_list.append(self.serialize(value))
             return t_list
```

### Comparing `decore_Base-0.0.13/decore_base/classes/decore_prompt.py` & `decore_Base-0.0.14/decore_base/classes/decore_prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,18 @@
             elif self.args.sample:
                 if not globals.config.app_id == '364871e4-6727-4e1f-80a2-acc9c83ace92':
                     self.sync_sample()
                     exit()
                 else:
                     raise Exception('You can not use the "sample" command in sample project context')
             elif self.args.dev:
-                self.sync_spa()
                 globals.flags.purge_unused_database_cols = False
+                globals.flags.dev_mode = True
+                self.sync_spa()
+                
             elif self.args.build:
                 PyInstaller.__main__.run([
                     '--paths="."',
                     '--add-data=spa;spa',
                     '--collect-data=pykeepass',
                     'app.py'
                 ])
```

### Comparing `decore_Base-0.0.13/decore_base/classes/decore_query.py` & `decore_Base-0.0.14/decore_base/classes/decore_query.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/classes/decore_return.py` & `decore_Base-0.0.14/decore_base/classes/decore_return.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/classes/decore_translate.py` & `decore_Base-0.0.14/decore_base/classes/decore_translate.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/classes/decore_view.py` & `decore_Base-0.0.14/decore_base/classes/decore_view.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/decore.py` & `decore_Base-0.0.14/decore_base/decore.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,31 +26,35 @@
 from str2type import str2type
 from pathlib import Path
 from collections import OrderedDict
 
 
 class Decore(object):
     def __init__(self):
-        self.prompt = Decore_prompt()
+        if not globals.flags.build_mode:
+            self.prompt = Decore_prompt()
         self.pool = Decore_pool()
         self.api = self.get_api()
         Decore_query.create_table(safe=True)
         
     def get_api(self):
         t_static_folder = Path('spa/static')
         t_template_folder = Path('spa/templates')
         api = Flask(__name__, static_folder=t_static_folder.absolute(), template_folder=t_template_folder.absolute())
-        CORS(api, expose_headers=["Content-Disposition"])
-        # Make the WSGI interface available at the top level so wfastcgi can get it.
-        wsgi_app = api.wsgi_app
-        api.config['SECRET_KEY'] = '325245hkhf486axcv5719bf9397cbn69xv'
-        api.config['WTF_CSRF_ENABLED'] = False  # TODO - csrf enebled when not cors
-        print('APP_ROOT_FOLDER >> ' + str(api.root_path))
-        print('STATIC_FOLDER >> ' + str(api.static_folder))
-        print('TEMPLATE_FOLDER >> ' + str(api.template_folder))
+        
+        if globals.flags.dev_mode:
+            CORS(api, expose_headers=["Content-Disposition"])
+            
+        elif not globals.flags.dev_mode: 
+            api.config['SECRET_KEY'] = '325245hkhf486axcv5719bf9397cbn69xv'
+            api.config['WTF_CSRF_ENABLED'] = False  # TODO - csrf enable when not cors
+        
+        # print('APP_ROOT_FOLDER >> ' + str(api.root_path))
+        # print('STATIC_FOLDER >> ' + str(api.static_folder))
+        # print('TEMPLATE_FOLDER >> ' + str(api.template_folder))
         api.add_url_rule('/', 'index', self.index, defaults={'p_path': ''})
         api.add_url_rule('/<path:p_path>', 'index', self.index)
         api.add_url_rule('/get_meta', 'get_meta', self.get_meta)
         api.add_url_rule('/get_default/<p_source_id>', 'get_default', self.get_default)
         api.add_url_rule('/get_last/<p_source_id>', 'get_last', self.get_last)
         api.add_url_rule('/post_item_s/<p_source_id>', 'post_item_s', self.post_item_s, methods=['POST'])
         api.add_url_rule('/post_option_s/<p_source_id>', 'post_option_s', self.post_option_s, methods=['POST'])
@@ -65,16 +69,21 @@
         from waitress import serve
         HOST = os.environ.get('SERVER_HOST', 'localhost')
         try:
             PORT = int(os.environ.get('SERVER_PORT', str(globals.config.app_port)))
         except ValueError:
             PORT = globals.config.app_port
         
-        if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
+        if not globals.flags.dev_mode:
+            logger = logging.getLogger('waitress')
+            logger.info(self.pool.app.title + ' now running on: http://' + str(HOST) + ':' + str(PORT))
+            logger.info('Press CTRL+C to quit.')
+            logger.setLevel(logging.WARNING)
             serve(self.api, host=HOST, port=PORT)
+            
         else:
             self.api.run(HOST, PORT)
 
     def app(self, p_title):
         def wrapper(func):
             self.pool.register(Decore_app('app', None, None, None, p_title, None, func.__doc__))
             self.pool.extend()
@@ -155,16 +164,16 @@
                 t_parent_id = t_parent_s[-2]
             else:
                 t_parent_id = p_parent_id
             t_source_id = t_parent_s[0]
             self.pool.register(Decore_element(func.__name__, t_parent_id, t_source_id, p_icon, p_title, p_desc, p_type, p_default, p_disable, p_schema, func))
         return wrapper
 
-    l_action_type = Literal['standard', 'check', 'response', 'file'] #TODO - check, response > activators
-    l_action_activator = Literal['none', 'default-menu', 'item-submit', 'item-menu', 'item-click']
+    l_action_type = Literal['standard', 'submit', 'check', 'response', 'file', 'download'] #TODO - check, response > activators
+    l_action_activator = Literal['none', 'default-menu', 'item-menu', 'item-click']
 
     def action(self, p_parent_id=None, p_icon=None, p_title=None, p_desc=None, p_type: l_action_type = 'standard', p_activator: l_action_activator = 'none'):
         def wrapper(func):
             t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
             if not p_parent_id:
                 t_parent_id = t_parent_s[-2]
             else:
@@ -212,16 +221,19 @@
     def get_default(self, p_source_id):
         t_source = self.pool.__data__[p_source_id]
         t_item = t_source.model().__data__
         return jsonify(t_item), 200
     
     def get_last(self, p_source_id):
         t_source = self.pool.__data__[p_source_id]
-        t_item = t_source.model.select()[0].__data__
-        return jsonify(t_item), 200
+        if not len(t_source.model.select()) == 0:
+            t_item = t_source.model.select()[-1].__data__
+            return jsonify(t_item), 200
+        else:
+            return self.get_default(p_source_id)
 
     def post_item_s(self, p_source_id):
         t_start = perf_counter()
         t_query = json.loads(request.data)
         t_source = self.pool.__data__[p_source_id]
         t_item_s = t_source.model.get_dict_s(t_query)
         t_end = perf_counter()
@@ -256,14 +268,17 @@
                 value.save(t_path)
                 t_data['item'][key] = t_path
 
         t_return = t_action.func(self.pool.__data__[t_action.source_id], t_data)
 
         if t_action.type == 'standard':
             return {'success': t_return[0], 'result': str(t_return[1])}, 200
+        
+        if t_action.type == 'submit':
+            return {'success': t_return[0], 'result': str(t_return[1])}, 200
 
         elif t_action.type == 'check':
             return {'success': t_return}, 200
 
         elif t_action.type == 'file':
             t_path = Path(t_return)
             return send_file(t_path, download_name=t_path.name)
```

### Comparing `decore_Base-0.0.13/decore_base/docs/social_header.txt` & `decore_Base-0.0.14/decore_base/docs/social_header.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/extensions/conform_model.py` & `decore_Base-0.0.14/decore_base/uniform/conform_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/extensions/depricated/askform_base.py` & `decore_Base-0.0.14/decore_base/uniform/depricated/askform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/extensions/depricated/buyform_base.py` & `decore_Base-0.0.14/decore_base/uniform/depricated/buyform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/extensions/depricated/conform_base.py` & `decore_Base-0.0.14/decore_base/uniform/depricated/conform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/extensions/depricated/deform_base.py` & `decore_Base-0.0.14/decore_base/uniform/depricated/deform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/extensions/perform_model.py` & `decore_Base-0.0.14/decore_base/uniform/perform_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/extensions/reform_client_model.py` & `decore_Base-0.0.14/decore_base/uniform/reform_client_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/extensions/reform_server_model.py` & `decore_Base-0.0.14/decore_base/uniform/reform_server_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/globals.py` & `decore_Base-0.0.14/decore_base/globals.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from pathlib import Path
 from pykeepass import create_database, PyKeePass
 from uuid import uuid4
-import json,logging
+import json,logging,sys
 
 logging.basicConfig(format='[%(levelname)s] | %(message)s', level=logging.INFO)
 
 class Global_flags(object):
     def __init__(self):
+        self.build_mode = self.set_build_mode()
+        self.dev_mode = False
         self.purge_unused_database_cols = False
+    
+    def set_build_mode(self):
+        if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
+            return True
+        else:
+            return False
 
 class Global_config(object):
     def __init__(self):
         self.__data__ = {   
                         'default': {'app_id': str(uuid4()), 'app_port': 5555, 'state_path': 'state'}, 
                         'remote': {'server_addr': '0.0.0.0', 'server_port': 51515}
                         }
```

### Comparing `decore_Base-0.0.13/decore_base/library/particl_market/particl_market.py` & `decore_Base-0.0.14/decore_base/library/particl_market/particl_market.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/library/powershell.py` & `decore_Base-0.0.14/decore_base/library/powershell.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/library/powershell2.py` & `decore_Base-0.0.14/decore_base/library/powershell2.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/library/return_value.py` & `decore_Base-0.0.14/decore_base/library/return_value.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/library/roaster/roaster_client.py` & `decore_Base-0.0.14/decore_base/library/roaster/roaster_client.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/library/roaster/roaster_functions.py` & `decore_Base-0.0.14/decore_base/library/roaster/roaster_functions.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/library/roaster/roaster_server.py` & `decore_Base-0.0.14/decore_base/library/roaster/roaster_server.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/.gitignore` & `decore_Base-0.0.14/decore_base/prepare/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/.vscode/launch.json` & `decore_Base-0.0.14/decore_base/prepare/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/css/912.77e6bcbe.css` & `decore_Base-0.0.14/decore_base/prepare/spa/static/css/912.77e6bcbe.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/css/app.d398f07d.css` & `decore_Base-0.0.14/decore_base/prepare/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css` & `decore_Base-0.0.14/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/favicon.ico` & `decore_Base-0.0.14/decore_base/prepare/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/icons/favicon-128x128.png` & `decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/icons/favicon-16x16.png` & `decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/icons/favicon-32x32.png` & `decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/icons/favicon-96x96.png` & `decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/js/65.940d9b80.js` & `decore_Base-0.0.14/decore_base/prepare/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/js/912.e7a2b7ea.js` & `decore_Base-0.0.14/decore_base/prepare/spa/static/js/912.f638ed14.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkuniform_front"] = globalThis["webpackChunkuniform_front"] || []).push([
     [912], {
         5912: (e, t, l) => {
             l.r(t), l.d(t, {
-                default: () => Lt
+                default: () => Nt
             });
             var s = l(9835),
                 a = l(499),
                 i = (l(9665), l(5360)),
                 o = l(8339);
             class n extends i.y {
                 constructor(e) {
@@ -32,15 +32,15 @@
                 constructor(e) {
                     super(e), this.ql = {}, this.action_store = (0, u.j)(), this.context = "none", this.show = !1, this.has_submit_btn = !1, this.has_close_btn = !1
                 }
                 setSubmitBtn() {
                     let e = !1;
                     this.widget_s.forEach((t => {
                         t.action_s.forEach((t => {
-                            "item-submit" == t.activator && (e = !0)
+                            "submit" == t.type && (e = !0)
                         }))
                     })), this.has_submit_btn = e
                 }
                 setCloseBtn() {
                     let e = !1;
                     "last" != this.context && (e = !0), this.has_close_btn = e
                 }
@@ -224,30 +224,30 @@
                 });
             var D = l(3655);
             const Q = j,
                 Z = Q;
             U()(j, "components", {
                 QDrawer: D.Z
             });
-            class F {
+            class V {
                 constructor(e, t) {
                     this.source = e, this.query = t, this.search = "", this.item = {}, this.item_s = [], this.select_s = [], this.count = 0
                 }
                 setItems() {
                     this.source.getItems(this.query).then((e => {
                         this.item_s = e.data.item_s, this.count = e.data.count
                     })).catch((e => {
                         console.log(e)
                     }))
                 }
             }
-            var V = l(1809);
+            var F = l(1809);
 
             function C(e) {
-                const t = (0, V.Q_)(e, {
+                const t = (0, F.Q_)(e, {
                         state: () => ({
                             el: {}
                         }),
                         getters: {},
                         actions: {
                             sendElement(e, t, l, s) {
                                 let a = {
@@ -264,15 +264,15 @@
                         }
                     }),
                     l = t();
                 return l
             }
             class x extends i.y {
                 constructor(e) {
-                    super(e), this.data = (0, a.qj)(new F(this.uniform.source[this.source_id], {})), this.compose_store = C(this.id), this.action_store = (0, u.j)(), this.form_ref = void 0, this.composer_ref = void 0, this.valid = !0, this.item_s_mode = !1
+                    super(e), this.data = (0, a.qj)(new V(this.uniform.source[this.source_id], {})), this.compose_store = C(this.id), this.action_store = (0, u.j)(), this.form_ref = void 0, this.composer_ref = void 0, this.valid = !0, this.item_s_mode = !1
                 }
                 regComposerElement(e) {
                     e.id in this.item || (this.item[e.id] = e.default), e.schema && (this.source.schema[e.id] = e.schema), this.compose_store.el[e.id] = e
                 }
                 refForm(e) {
                     this.form_ref = e
                 }
@@ -305,48 +305,48 @@
                     this.form_ref && await this.form_ref.validate().then((e => {
                         e || (this.valid = !1)
                     })), this.composer_ref && await this.composer_ref.validate().then((e => {
                         e || (this.valid = !1)
                     }))
                 }
                 reset() {
-                    this.form_ref && this.form_ref.reset(), this.composer_ref && this.form_ref.reset()
+                    this.form_ref && this.form_ref.reset(), this.composer_ref && this.composer_ref.reset()
                 }
                 async submit() {
-                    await this.validateWidget(), this.valid && this.action_s.forEach((e => {
-                        "item-submit" == e.activator && this.action_store.sendAction(e, this.data.item, this.data.source.select_s)
+                    this.valid = !0, await this.validateWidget(), this.valid && this.action_s.forEach((e => {
+                        "submit" == e.type && this.action_store.sendAction(e, this.data.item, this.data.source.select_s)
                     }))
                 }
                 getRules(e) {
                     let t = [];
                     if (e in this.data.source.schema) {
                         const l = this.data.source.schema[e];
-                        "string" == l.type && t.push((e => e && e.length > 0 || "Not valid")), "allowed" in l && l.allowed.forEach((e => {
+                        "string" == l.type && t.push((e => e && e.length > 0 || "Not valid")), "integer" == l.type && t.push((e => null !== e && "" !== e && NaN != parseInt(e) || "Not valid")), "allowed" in l && l.allowed.forEach((e => {
                             t.push((t => t && t == e || "Not valid"))
                         }))
                     }
                     return t
                 }
             }
             const E = {
                     key: 0
                 },
-                K = {
+                z = {
                     key: 1
                 },
                 H = {
                     key: 2
                 },
-                z = {
+                K = {
                     key: 3
                 },
-                O = {
+                I = {
                     key: 4
                 },
-                I = {
+                O = {
                     key: 5
                 },
                 A = {
                     inheritAttrs: !1
                 },
                 Y = Object.assign(A, {
                     __name: "uf-widget-composer",
@@ -360,15 +360,15 @@
                                 greedy: "",
                                 ref: e => {
                                     (0, a.SU)(t).refComposer(e)
                                 }
                             }, {
                                 default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)((0, a.SU)(t).compose_store.el, (e => ((0, s.wg)(), (0, s.iD)("span", {
                                     key: e.id
-                                }, ["p" == e.type ? ((0, s.wg)(), (0, s.iD)("p", E, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h1" == e.type ? ((0, s.wg)(), (0, s.iD)("h1", K, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h2" == e.type ? ((0, s.wg)(), (0, s.iD)("h2", H, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h3" == e.type ? ((0, s.wg)(), (0, s.iD)("h3", z, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h4" == e.type ? ((0, s.wg)(), (0, s.iD)("h4", O, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h5" == e.type ? ((0, s.wg)(), (0, s.iD)("h5", I, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "checkbox" == e.type ? ((0, s.wg)(), (0, s.j4)(o, {
+                                }, ["p" == e.type ? ((0, s.wg)(), (0, s.iD)("p", E, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h1" == e.type ? ((0, s.wg)(), (0, s.iD)("h1", z, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h2" == e.type ? ((0, s.wg)(), (0, s.iD)("h2", H, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h3" == e.type ? ((0, s.wg)(), (0, s.iD)("h3", K, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h4" == e.type ? ((0, s.wg)(), (0, s.iD)("h4", I, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h5" == e.type ? ((0, s.wg)(), (0, s.iD)("h5", O, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "checkbox" == e.type ? ((0, s.wg)(), (0, s.j4)(o, {
                                     key: 6,
                                     "hide-bottom-space": "",
                                     dense: "",
                                     borderless: "",
                                     modelValue: (0, a.SU)(t).item[e.id],
                                     "onUpdate:modelValue": l => (0, a.SU)(t).item[e.id] = l,
                                     rules: (0, a.SU)(t).getRules(e.id),
@@ -393,21 +393,21 @@
             const M = Y,
                 R = M;
             U()(Y, "components", {
                 QForm: P.Z,
                 QField: T.Z,
                 QCheckbox: B.Z
             });
-            const L = {
+            const N = {
                     key: 0
                 },
-                $ = {
+                L = {
                     key: 1
                 },
-                N = {
+                $ = {
                     key: 2
                 },
                 G = {
                     inheritAttrs: !1
                 },
                 J = Object.assign(G, {
                     __name: "uf-widget-layout",
@@ -431,27 +431,27 @@
                                 }, {
                                     default: (0, s.w5)((() => [(0, s._)("h5", null, (0, d.zw)((0, a.SU)(t).title), 1), (0, s.Wm)(i), (0, s.Wm)(o, {
                                         name: (0, a.SU)(t).icon
                                     }, null, 8, ["name"])])),
                                     _: 1
                                 }), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)((0, a.SU)(t).layout, (l => ((0, s.wg)(), (0, s.iD)("span", {
                                     key: l
-                                }, ["c" == l ? ((0, s.wg)(), (0, s.iD)("span", L, [(0, s.Wm)(u, {
+                                }, ["c" == l ? ((0, s.wg)(), (0, s.iD)("span", N, [(0, s.Wm)(u, {
                                     class: "widget-card-section"
                                 }, {
                                     default: (0, s.w5)((() => [(0, s.WI)(e.$slots, "widget-content")])),
                                     _: 3
-                                })])) : (0, s.kq)("", !0), "e" == l && (0, a.SU)(t).element_s.length >= 1 ? ((0, s.wg)(), (0, s.iD)("span", $, [(0, s.Wm)(u, {
+                                })])) : (0, s.kq)("", !0), "e" == l && (0, a.SU)(t).element_s.length >= 1 ? ((0, s.wg)(), (0, s.iD)("span", L, [(0, s.Wm)(u, {
                                     class: "widget-card-section"
                                 }, {
                                     default: (0, s.w5)((() => [(0, s.Wm)(R, {
                                         use: (0, a.SU)(t)
                                     }, null, 8, ["use"])])),
                                     _: 1
-                                })])) : (0, s.kq)("", !0), "a" == l ? ((0, s.wg)(), (0, s.iD)("span", N, [(0, s.Wm)(c, null, {
+                                })])) : (0, s.kq)("", !0), "a" == l ? ((0, s.wg)(), (0, s.iD)("span", $, [(0, s.Wm)(c, null, {
                                     default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)((0, a.SU)(t).dialog_s, (l => ((0, s.wg)(), (0, s.iD)("span", {
                                         key: l.id
                                     }, ["default-menu" == l.activator ? ((0, s.wg)(), (0, s.j4)(r, {
                                         key: 0,
                                         onClick: s => e.uniform.dialog[l.id].showDialog(void 0, "default", (0, a.SU)(t).source),
                                         icon: l.icon,
                                         dense: "",
@@ -530,19 +530,30 @@
                                     dense: "",
                                     outlined: "",
                                     modelValue: (0, a.SU)(t).data.item[e.name],
                                     "onUpdate:modelValue": l => (0, a.SU)(t).data.item[e.name] = l,
                                     label: e.verbose_name,
                                     rules: (0, a.SU)(t).getRules(e.name),
                                     "lazy-rules": "ondemand"
-                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])) : (0, s.kq)("", !0), e.class.includes("IntegerField") ? ((0, s.wg)(), (0, s.j4)(i, {
+                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])) : (0, s.kq)("", !0), e.class.includes("TextField") ? ((0, s.wg)(), (0, s.j4)(i, {
                                     key: 1,
                                     class: "q-pb-sm",
                                     dense: "",
                                     outlined: "",
+                                    modelValue: (0, a.SU)(t).data.item[e.name],
+                                    "onUpdate:modelValue": l => (0, a.SU)(t).data.item[e.name] = l,
+                                    label: e.verbose_name,
+                                    rules: (0, a.SU)(t).getRules(e.name),
+                                    "lazy-rules": "ondemand",
+                                    autogrow: ""
+                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])) : (0, s.kq)("", !0), e.class.includes("IntegerField") ? ((0, s.wg)(), (0, s.j4)(i, {
+                                    key: 2,
+                                    class: "q-pb-sm",
+                                    dense: "",
+                                    outlined: "",
                                     type: "number",
                                     modelValue: (0, a.SU)(t).data.item[e.name],
                                     "onUpdate:modelValue": l => (0, a.SU)(t).data.item[e.name] = l,
                                     label: e.verbose_name,
                                     rules: (0, a.SU)(t).getRules(e.name),
                                     "lazy-rules": "ondemand"
                                 }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])) : (0, s.kq)("", !0)])))), 128))])),
@@ -687,36 +698,36 @@
                                 use: l
                             }, null, 8, ["use"])) : (0, s.kq)("", !0)])),
                             _: 1
                         }, 8, ["use"]))
                     }
                 },
                 Ze = Qe,
-                Fe = Ze,
-                Ve = {
+                Ve = Ze,
+                Fe = {
                     inheritAttrs: !1
                 },
-                Ce = Object.assign(Ve, {
+                Ce = Object.assign(Fe, {
                     __name: "uf-dialog-standard",
                     setup(e) {
                         const t = (0, s.l1)().use;
                         return (e, l) => ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)((0, a.SU)(t).widget_s, (e => ((0, s.wg)(), (0, s.iD)("span", {
                             key: e.id
-                        }, [(0, s.Wm)(Fe, {
+                        }, [(0, s.Wm)(Ve, {
                             id: e.id
                         }, null, 8, ["id"]), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.widget_s, (e => ((0, s.wg)(), (0, s.iD)("span", {
                             key: e.id
-                        }, [(0, s.Wm)(Fe, {
+                        }, [(0, s.Wm)(Ve, {
                             id: e.id
                         }, null, 8, ["id"])])))), 128))])))), 128))
                     }
                 }),
                 xe = Ce,
                 Ee = xe,
-                Ke = {
+                ze = {
                     __name: "uf-dialog",
                     props: {
                         id: {}
                     },
                     setup(e) {
                         const t = e,
                             l = (0, a.qj)(new r(t.id));
@@ -727,27 +738,27 @@
                                 key: 0,
                                 use: l
                             }, null, 8, ["use"])) : (0, s.kq)("", !0)])),
                             _: 1
                         }, 8, ["use"]))
                     }
                 },
-                He = Ke,
-                ze = He;
-            class Oe {
+                He = ze,
+                Ke = He;
+            class Ie {
                 constructor(e) {
                     this.rowsPerPageOptions = [4, 8, 16, 32, 64, 128, 265, 512, 1024], this.rowsPerPage = e, this.page = 1
                 }
             }
-            class Ie extends i.y {
+            class Oe extends i.y {
                 constructor(e) {
-                    super(e), this.ql = {}, this.route = (0, o.yj)(), this.data = (0, a.qj)(new F(this.uniform.source[this.source_id], {
+                    super(e), this.ql = {}, this.route = (0, o.yj)(), this.data = (0, a.qj)(new V(this.uniform.source[this.source_id], {
                         ...this.query,
                         ...this.route.query
-                    })), this.pagination = (0, a.qj)(new Oe(this.pag_recs)), this.item_menu_target = !1, this.item_menu_model = !1, this.item_menu_row = {}
+                    })), this.pagination = (0, a.qj)(new Ie(this.pag_recs)), this.item_menu_target = !1, this.item_menu_model = !1, this.item_menu_row = {}
                 }
                 get column_s() {
                     let e = [];
                     return e.push({
                         name: "gotos",
                         label: "",
                         field: "gotos"
@@ -874,26 +885,26 @@
                     }
                 });
             var Pe = l(6362),
                 Te = l(3246),
                 Be = l(490),
                 Me = l(1233);
             const Re = Ye,
-                Le = Re;
+                Ne = Re;
             U()(Ye, "components", {
                 QMenu: Pe.Z,
                 QList: Te.Z,
                 QItem: Be.Z,
                 QItemSection: Me.Z,
                 QIcon: ee.Z
             });
-            const $e = {
+            const Le = {
                     class: "row full-width items-center"
                 },
-                Ne = {
+                $e = {
                     class: "col-auto"
                 },
                 Ge = {
                     class: "col-auto"
                 },
                 Je = {
                     key: 0,
@@ -949,15 +960,15 @@
                                     })), s || e.push(l)
                                 })), e
                             })),
                             h = (0, s.Fl)((() => {
                                 let e, l = [];
                                 if ("ForeignKeyField" == n.value.class) e = n.value.rel_model;
                                 else {
-                                    let l = t.data.source.rel_field_s.filter((e => "ForeignKeyField" == e.class && e.backref == n.value.ref_name || "ManyToManyField" == e.class && e.name == n.value.ref_name))[0];
+                                    let l = t.data.source.rel_field_s.filter((e => "ForeignKeyField" == e.class && e.backref == n.value.name || "ManyToManyField" == e.class && e.name == n.value.name))[0];
                                     e = "ForeignKeyField" == l.class ? l.model : l.rel_model
                                 }
                                 let s = t.uniform.getSourceByModel(e);
                                 return s.field_s.forEach((e => {
                                     let s = !1;
                                     Object.entries(t.data.query).forEach((([t]) => {
                                         t.includes(e.name) && (s = !0)
@@ -977,35 +988,33 @@
                             })),
                             g = (0, a.iH)(null);
 
                         function w() {
                             let e = i.query;
                             n.value && !m.value ? t.data.source.getOptions(e, n.value.name, null).then((e => {
                                 g.value = e.data
-                            })) : u.value && m.value && ("ForeignKeyField" == n.value.class ? t.data.source.getOptions(e, n.value.name, u.value.name).then((e => {
-                                g.value = e.data
-                            })) : t.data.source.getOptions(e, n.value.ref_name, u.value.name).then((e => {
+                            })) : u.value && m.value && (n.value.class, t.data.source.getOptions(e, n.value.name, u.value.name).then((e => {
                                 g.value = e.data
                             })))
                         }
 
                         function f() {
                             let e = {
                                     ...i.query
                                 },
                                 t = "";
-                            m.value ? m.value && (t = "ForeignKeyField" == n.value.class ? t + n.value.name + "__" + u.value.name : t + n.value.ref_name + "__" + u.value.name) : t = n.value.name, t = t + "__" + r.value, e[t] = d.value, l.push({
+                            m.value ? m.value && (t = (n.value.class, t + n.value.name + "__" + u.value.name)) : t = n.value.name, t = t + "__" + r.value, e[t] = d.value, l.push({
                                 path: i.path,
                                 query: e
                             })
                         }
                         return (e, l) => {
                             const o = (0, s.up)("q-btn"),
                                 v = (0, s.up)("q-select");
-                            return (0, s.wg)(), (0, s.iD)("div", $e, [(0, s._)("div", Ne, [(0, s.Wm)(o, {
+                            return (0, s.wg)(), (0, s.iD)("div", Le, [(0, s._)("div", $e, [(0, s.Wm)(o, {
                                 class: "float-right text-black",
                                 dense: "",
                                 round: "",
                                 flat: "",
                                 icon: "mdi-content-save",
                                 onClick: l[0] || (l[0] = e => (0, a.SU)(t).uniform.queries.saveQuery((0, a.SU)(i)))
                             })]), (0, s._)("div", Ge, [(0, s.Wm)(o, {
@@ -1217,37 +1226,37 @@
                                 _: 1
                             })
                         }
                     }
                 });
             var Qt = l(996);
             const Zt = Dt,
-                Ft = Zt;
+                Vt = Zt;
             U()(Dt, "components", {
                 QToolbar: w.Z,
                 QSpace: v.Z,
                 QPagination: Qt.Z,
                 QSelect: nt.Z
             });
-            const Vt = {
+            const Ft = {
                     inheritAttrs: !1
                 },
-                Ct = Object.assign(Vt, {
+                Ct = Object.assign(Ft, {
                     __name: "uf-view-layout",
                     setup(e) {
                         const t = (0, s.l1)().use,
                             l = (0, s.Fl)((() => {
                                 let e = "0 px";
                                 return t.ql.hasOwnProperty("header") && (e = t.ql.header.size + "px"), e
                             }));
                         return (e, i) => {
                             const o = (0, s.up)("q-header"),
                                 n = (0, s.up)("q-footer"),
                                 u = (0, s.up)("q-layout");
-                            return (0, s.wg)(), (0, s.iD)(s.HY, null, [(0, s.Wm)(Le, {
+                            return (0, s.wg)(), (0, s.iD)(s.HY, null, [(0, s.Wm)(Ne, {
                                 use: (0, a.SU)(t)
                             }, null, 8, ["use"]), (0, s.Wm)(u, {
                                 container: "",
                                 style: {
                                     height: "calc(100vh - 102px)"
                                 }
                             }, {
@@ -1265,15 +1274,15 @@
                                     class: "view-content",
                                     style: (0, d.j5)({
                                         "padding-top": (0, a.SU)(l)
                                     })
                                 }, [(0, s.WI)(e.$slots, "view-content")], 4), (0, s.Wm)(n, {
                                     reveal: ""
                                 }, {
-                                    default: (0, s.w5)((() => [(0, s.Wm)(Ft, {
+                                    default: (0, s.w5)((() => [(0, s.Wm)(Vt, {
                                         use: (0, a.SU)(t)
                                     }, null, 8, ["use"])])),
                                     _: 1
                                 })])),
                                 _: 3
                             })], 64)
                         }
@@ -1282,18 +1291,18 @@
                 xt = Ct,
                 Et = xt;
             U()(Ct, "components", {
                 QLayout: _.Z,
                 QHeader: g.Z,
                 QFooter: y.Z
             });
-            const Kt = {
+            const zt = {
                     inheritAttrs: !1
                 },
-                Ht = Object.assign(Kt, {
+                Ht = Object.assign(zt, {
                     __name: "uf-view-table",
                     setup(e) {
                         const t = (0, s.l1)().use;
                         t.data.setItems();
                         const l = (0, s.Fl)((() => {
                             let e = 16,
                                 l = "0 px";
@@ -1379,44 +1388,44 @@
                                     _: 2
                                 }, 1032, ["props"])])),
                                 _: 1
                             }, 8, ["columns", "filter", "rows", "style", "pagination", "selected"])
                         }
                     }
                 });
-            var zt = l(7220);
-            const Ot = Ht,
-                It = Ot;
+            var Kt = l(7220);
+            const It = Ht,
+                Ot = It;
             U()(Ht, "components", {
                 QTable: We.Z,
-                QTd: zt.Z,
+                QTd: Kt.Z,
                 QBtn: b.Z,
                 QMenu: Pe.Z,
                 QList: Te.Z,
                 QItem: Be.Z,
                 QItemSection: Me.Z
             });
             const At = {
                     __name: "uf-view",
                     props: {
                         id: {}
                     },
                     setup(e) {
                         const t = e,
-                            l = (0, a.qj)(new Ie(t.id));
+                            l = (0, a.qj)(new Oe(t.id));
                         return (0, s.bv)((() => {
                             for (const e of l.dialog_s)
                                 if ("none" == e.activator) {
                                     l.ref[e.id].showDialog({}, "last", l.data.source);
                                     break
                                 }
                         })), (e, t) => ((0, s.wg)(), (0, s.j4)(Et, {
                             use: l
                         }, {
-                            "view-content": (0, s.w5)((() => ["table" == l.type ? ((0, s.wg)(), (0, s.j4)(It, {
+                            "view-content": (0, s.w5)((() => ["table" == l.type ? ((0, s.wg)(), (0, s.j4)(Ot, {
                                 key: 0,
                                 use: l
                             }, null, 8, ["use"])) : (0, s.kq)("", !0)])),
                             _: 1
                         }, 8, ["use"]))
                     }
                 },
@@ -1428,28 +1437,28 @@
                 Bt = {
                     __name: "uf-base",
                     setup(e) {
                         const t = (0, o.yj)(),
                             l = (0, a.qj)(new n(t.params.base_id));
                         return (e, t) => {
                             const a = (0, s.up)("q-page");
-                            return (0, s.wg)(), (0, s.iD)(s.HY, null, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(l.route_dialog_s, (e => ((0, s.wg)(), (0, s.j4)(ze, {
+                            return (0, s.wg)(), (0, s.iD)(s.HY, null, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(l.route_dialog_s, (e => ((0, s.wg)(), (0, s.j4)(Ke, {
                                 key: e.id,
                                 id: e.id
                             }, null, 8, ["id"])))), 128)), (0, s.Wm)(a, null, {
                                 default: (0, s.w5)((() => [l.getView().id ? ((0, s.wg)(), (0, s.iD)("span", Tt, [(0, s.Wm)(Pt, {
                                     id: l.getView().id
                                 }, null, 8, ["id"])])) : (0, s.kq)("", !0)])),
                                 _: 1
                             })], 64)
                         }
                     }
                 };
             var Mt = l(9885);
             const Rt = Bt,
-                Lt = Rt;
+                Nt = Rt;
             U()(Bt, "components", {
                 QPage: Mt.Z
             })
         }
     }
 ]);
```

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/js/app.7ef3a1f6.js` & `decore_Base-0.0.14/decore_base/prepare/spa/static/js/app.465385a3.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -81,15 +81,15 @@
                                     _ = (0, s.up)("q-item"),
                                     y = (0, s.up)("q-chip"),
                                     b = (0, s.up)("q-tree"),
                                     k = (0, s.up)("q-drawer");
                                 return (0, s.wg)(), (0, s.j4)(k, {
                                     "show-if-above": "",
                                     model: !0,
-                                    width: 375,
+                                    width: 300,
                                     side: "left",
                                     breakpoint: 0,
                                     bordered: "",
                                     mini: (0, i.SU)(t).drawer_mini
                                 }, {
                                     default: (0, s.w5)((() => [(0, s.Wm)(w, {
                                         class: "bg-grey-2"
@@ -246,26 +246,26 @@
                     b = n(490),
                     k = n(1233),
                     q = n(2857),
                     j = n(7691),
                     C = n(9984),
                     S = n.n(C);
                 const x = w,
-                    E = x;
+                    W = x;
                 S()(w, "components", {
                     QDrawer: v.Z,
                     QToolbar: g.Z,
                     QBtn: _.Z,
                     QTree: y.Z,
                     QItem: b.Z,
                     QItemSection: k.Z,
                     QIcon: q.Z,
                     QChip: j.Z
                 });
-                const W = {
+                const E = {
                         class: "text-weight-bold"
                     },
                     Q = {
                         class: "text-grey"
                     };
 
                 function Z(e, t, n, o, r, i) {
@@ -283,15 +283,15 @@
                                 width: "500px"
                             }
                         }, {
                             default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(o.action_store.active_s, (e => ((0, s.wg)(), (0, s.j4)(a, {
                                 key: e.id,
                                 class: "row items-center no-wrap"
                             }, {
-                                default: (0, s.w5)((() => [(0, s._)("div", null, [(0, s._)("div", W, (0, d.zw)(e.title), 1), (0, s._)("div", Q, (0, d.zw)(e.result), 1)])])),
+                                default: (0, s.w5)((() => [(0, s._)("div", null, [(0, s._)("div", E, (0, d.zw)(e.title), 1), (0, s._)("div", Q, (0, d.zw)(e.result), 1)])])),
                                 _: 2
                             }, 1024)))), 128))])),
                             _: 1
                         })])),
                         _: 1
                     }, 8, ["modelValue"])
                 }
@@ -331,17 +331,18 @@
                                     r = (0, s.up)("q-input"),
                                     a = (0, s.up)("q-tooltip"),
                                     l = (0, s.up)("q-btn"),
                                     c = (0, s.up)("q-toolbar"),
                                     h = (0, s.up)("q-header"),
                                     p = (0, s.up)("router-view"),
                                     m = (0, s.up)("q-page-container"),
-                                    f = (0, s.up)("q-footer"),
-                                    w = (0, s.up)("q-layout");
-                                return (0, s.wg)(), (0, s.j4)(w, null, {
+                                    f = (0, s.up)("q-space"),
+                                    w = (0, s.up)("q-footer"),
+                                    v = (0, s.up)("q-layout");
+                                return (0, s.wg)(), (0, s.j4)(v, null, {
                                     default: (0, s.w5)((() => [(0, s.Wm)(u.Z, {
                                         use: (0, i.SU)(t)
                                     }, null, 8, ["use"]), (0, s.Wm)(h, {
                                         bordered: "",
                                         class: "bg-black text-white"
                                     }, {
                                         default: (0, s.w5)((() => [(0, s.Wm)(c, null, {
@@ -370,146 +371,155 @@
                                                     _: 1
                                                 })])),
                                                 _: 1
                                             })) : (0, s.kq)("", !0)])),
                                             _: 1
                                         })])),
                                         _: 1
-                                    }), (0, s.Wm)(E, {
+                                    }), (0, s.Wm)(W, {
                                         use: (0, i.SU)(t)
                                     }, null, 8, ["use"]), (0, s.Wm)(m, null, {
                                         default: (0, s.w5)((() => [((0, s.wg)(), (0, s.j4)(p, {
                                             key: e.$route.fullPath
                                         }))])),
                                         _: 1
-                                    }), (0, s.Wm)(B), (0, s.Wm)(f, {
+                                    }), (0, s.Wm)(B), (0, s.Wm)(w, {
                                         bordered: "",
                                         class: "bg-grey-8 text-white"
                                     }, {
                                         default: (0, s.w5)((() => [(0, s.Wm)(c, {
                                             dense: ""
+                                        }, {
+                                            default: (0, s.w5)((() => [(0, s.Wm)(f), (0, s.Wm)(l, {
+                                                flat: "",
+                                                icon: "mdi-coffee",
+                                                href: "https://ko-fi.com/decore_base"
+                                            })])),
+                                            _: 1
                                         })])),
                                         _: 1
                                     })])),
                                     _: 1
                                 })
                             }
                         }
                     });
                 var F = n(7605),
                     I = n(6602),
                     V = n(1973),
                     z = n(6858),
                     H = n(6611),
                     R = n(2133),
-                    K = n(1378);
-                const X = N,
-                    J = X;
+                    K = n(1378),
+                    X = n(136);
+                const J = N,
+                    Y = J;
                 S()(N, "components", {
                     QLayout: F.Z,
                     QHeader: I.Z,
                     QToolbar: g.Z,
                     QToolbarTitle: V.Z,
                     QBtn: _.Z,
                     QTooltip: z.Z,
                     QInput: H.Z,
                     QPageContainer: R.Z,
-                    QFooter: K.Z
+                    QFooter: K.Z,
+                    QSpace: X.Z
                 });
-                var Y = n(5360);
-                class $ extends Y.y {
+                var $ = n(5360);
+                class G extends $.y {
                     constructor(e) {
                         super(e), this.ql = {}, this.drawer_icon = "mdi-backburger", this.drawer_mini = !1, this.expanded_nodes = []
                     }
                     toogleLayoutDrawer() {
                         this.drawer_mini = !this.drawer_mini, this.drawer_mini ? this.drawer_icon = "mdi-forwardburger" : this.drawer_icon = "mdi-backburger"
                     }
                 }
-                const G = (0, s.aZ)({
+                const ee = (0, s.aZ)({
                         name: "App",
                         components: {
-                            "uf-app-layout": J
+                            "uf-app-layout": Y
                         },
                         setup() {
-                            const e = (0, i.qj)(new $("app"));
+                            const e = (0, i.qj)(new G("app"));
                             return (0, l.Z)((() => ({
                                 title: e.title
                             }))), {
                                 use: e
                             }
                         }
                     }),
-                    ee = (0, T.Z)(G, [
+                    te = (0, T.Z)(ee, [
                         ["render", a]
                     ]),
-                    te = ee;
-                var ne = n(3340),
-                    oe = n(1809);
-                const re = (0, ne.h)((() => {
-                    const e = (0, oe.WB)();
+                    ne = te;
+                var oe = n(3340),
+                    re = n(1809);
+                const ie = (0, oe.h)((() => {
+                    const e = (0, re.WB)();
                     return e
                 }));
-                var ie = n(8339);
-                const se = [{
+                var se = n(8339);
+                const ae = [{
                         path: "/:base_id/:view_id",
                         component: () => Promise.all([n.e(736), n.e(912)]).then(n.bind(n, 5912))
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => n.e(65).then(n.bind(n, 7065))
                     }],
-                    ae = se;
-                var le = n(5047);
-                const de = (0, ne.BC)((function() {
-                    const e = ie.PO,
-                        t = (0, ie.p7)({
+                    le = ae;
+                var de = n(5047);
+                const ue = (0, oe.BC)((function() {
+                    const e = se.PO,
+                        t = (0, se.p7)({
                             scrollBehavior: () => ({
                                 left: 0,
                                 top: 0
                             }),
-                            routes: ae,
+                            routes: le,
                             history: e("/")
                         });
                     return t.beforeEach(((e, t) => {
-                        const n = (0, le.I)();
+                        const n = (0, de.I)();
                         return n.use.app.expanded_nodes.push(e.params.base_id), !0
                     })), t
                 }));
-                async function ue(e, t) {
-                    const n = e(te);
+                async function ce(e, t) {
+                    const n = e(ne);
                     n.use(r.Z, t);
-                    const o = "function" === typeof re ? await re({}) : re;
+                    const o = "function" === typeof ie ? await ie({}) : ie;
                     n.use(o);
-                    const s = (0, i.Xl)("function" === typeof de ? await de({
+                    const s = (0, i.Xl)("function" === typeof ue ? await ue({
                         store: o
-                    }) : de);
+                    }) : ue);
                     return o.use((({
                         store: e
                     }) => {
                         e.router = s
                     })), {
                         app: n,
                         store: o,
                         router: s
                     }
                 }
-                const ce = {
+                const he = {
                         config: {}
                     },
-                    he = "/static/",
-                    pe = /\/\//,
-                    me = e => (he + e).replace(pe, "/");
-                async function fe({
+                    pe = "/static/",
+                    me = /\/\//,
+                    fe = e => (pe + e).replace(me, "/");
+                async function we({
                     app: e,
                     router: t,
                     store: n
                 }, o) {
                     let r = !1;
                     const i = e => {
                             try {
-                                return me(t.resolve(e).href)
+                                return fe(t.resolve(e).href)
                             } catch (n) {}
                             return Object(e) === e ? null : e
                         },
                         s = e => {
                             if (r = !0, "string" === typeof e && /^https?:\/\//.test(e)) return void(window.location.href = e);
                             const t = i(e);
                             null !== t && (window.location.href = t)
@@ -519,28 +529,28 @@
                         await o[d]({
                             app: e,
                             router: t,
                             store: n,
                             ssrContext: null,
                             redirect: s,
                             urlPath: a,
-                            publicPath: he
+                            publicPath: pe
                         })
                     } catch (l) {
                         return l && l.url ? void s(l.url) : void console.error("[Quasar] boot error:", l)
                     }!0 !== r && (e.use(t), e.mount("#q-app"))
                 }
-                ue(o.ri, ce).then((e => {
+                ce(o.ri, he).then((e => {
                     const [t, o] = void 0 !== Promise.allSettled ? ["allSettled", e => e.map((e => {
                         if ("rejected" !== e.status) return e.value.default;
                         console.error("[Quasar] boot error:", e.reason)
                     }))] : ["all", e => e.map((e => e.default))];
                     return Promise[t]([Promise.resolve().then(n.bind(n, 6898))]).then((t => {
                         const n = o(t).filter((e => "function" === typeof e));
-                        fe(e, n)
+                        we(e, n)
                     }))
                 }))
             },
             6898: (e, t, n) => {
                 n.r(t), n.d(t, {
                     default: () => u
                 });
@@ -808,15 +818,15 @@
             })
         }
     })(), (() => {
         n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, o) => (n.f[o](e, t), t)), []))
     })(), (() => {
         n.u = e => "js/" + e + "." + {
             65: "940d9b80",
-            912: "e7a2b7ea"
+            912: "f638ed14"
         } [e] + ".js"
     })(), (() => {
         n.miniCssF = e => "css/" + e + ".77e6bcbe.css"
     })(), (() => {
         n.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
```

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/static/js/vendor.03c46c80.js` & `decore_Base-0.0.14/decore_base/prepare/spa/static/js/vendor.03c46c80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/prepare/spa/templates/index.html` & `decore_Base-0.0.14/decore_base/prepare/spa/templates/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><base href=/static/ ><title>Uniform Front</title><meta charset=utf-8><meta name=description content="A part of Unform Famework"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><meta name=api_prod_port content={{port}}><meta name=api_dev_port content=5566><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=/static/js/vendor.03c46c80.js></script><script defer src=/static/js/app.7ef3a1f6.js></script><link href=/static/css/vendor.14c9ac7a.css rel=stylesheet><link href=/static/css/app.d398f07d.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><base href=/static/ ><title>Uniform Front</title><meta charset=utf-8><meta name=description content="A part of Unform Famework"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><meta name=api_prod_port content={{port}}><meta name=api_dev_port content=5566><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=/static/js/vendor.03c46c80.js></script><script defer src=/static/js/app.465385a3.js></script><link href=/static/css/vendor.14c9ac7a.css rel=stylesheet><link href=/static/css/app.d398f07d.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `decore_Base-0.0.13/decore_base/sample/.gitignore` & `decore_Base-0.0.14/decore_base/sample/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/.vscode/launch.json` & `decore_Base-0.0.14/decore_base/sample/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/bases/account_base.py` & `decore_Base-0.0.14/decore_base/sample/bases/account_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/bases/company_base.py` & `decore_Base-0.0.14/decore_base/sample/bases/company_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/bases/global_management_base.py` & `decore_Base-0.0.14/decore_base/sample/bases/global_management_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,27 +6,18 @@
 
 from mimesis import Person, Finance
 from random import randrange
 
 @decore.base(p_title='Global Management', p_icon='mdi-account-supervisor-circle-outline')
 class Global_management_base(object):
     
-    # @decore.function(p_type='init')
-    # def query_tester(self):
-    #     from peewee import DQ
-    #     t_person_s = list(Person_model.select())
-    #     t_companie_s = list(Company_model.select())
-    #     t_account_s = list(Account_model.select())
-    #     t_item_s = Person_model.query({'last_name':'Glover', 'companies__title__eq':'CNA', 'accounts__title__eq':'upper2074@example.com'})
-    #     t_or_chain = None
-    #     t_or_key = 'academic_degree'
-    #     t_or_chain |= DQ(**{t_or_key: 'Master'})
-    #     # t_or_chain |= DQ(**{t_or_key: 'Master'})
-    #     t_or_test = Person_model.filter(t_or_chain)
-    #     pass
+    @decore.function(p_type='init')
+    def query_tester(self):
+        t_item_s = Person_model.query({'companies__title__eq':'NetApp'})
+        pass
 
     @decore.function(p_type='init')
     def create_company_s(self):
         while len(Company_model.select()) < 32:
             t_finance = Finance()
             t_item = Company_model()
             t_item.id = t_item.create_uuid()
```

### Comparing `decore_Base-0.0.13/decore_base/sample/bases/person_base.py` & `decore_Base-0.0.14/decore_base/sample/bases/person_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,29 @@
 @decore.base(p_title='Person', p_model=Model)
 class Person_base(Base):
     
     @decore.widget(p_parent_id='com_vi1_di1', p_title='Persons', p_type='table', p_active_s=Model.field_s)
     def com_vi1_di1_wi1():
         pass
 
-    @decore.view(p_parent_id='Global_management_base', p_title='Persons', p_icon='mdi-account-group-outline', p_type='table', p_active_s=Model.field_s, p_filter_s=[Model.academic_degree, Model.br_companies, Model.br_accounts])
+    @decore.view(p_parent_id='Global_management_base', p_title='Persons', p_icon='mdi-account-group-outline', p_type='table', p_active_s=Model.field_s, p_filter_s=[Model.academic_degree, Model.companies, Model.accounts])
     def per_vi1():
+        
         @decore.dialog(p_title='Person', p_type='standard', p_display='drawer', p_activator='item-click')
         def per_vi1_di1():
             @decore.widget(p_title='Informations', p_type='info', p_active_s=Model.field_s)
             def per_vi1_di1_wi1():
                 @decore.dialog(p_title='Edit Person', p_icon='mdi-pencil', p_type='standard', p_display='drawer', p_activator='item-menu')
                 def per_vi1_wi1_di1():
-                    @decore.widget(p_type='form', p_active_s=[Model.last_name])
+                    @decore.widget(p_type='form', p_active_s=[Model.first_name, Model.last_name])
                     def per_vi1_di1_wi1_di1_wi1():
-                        @decore.action(p_activator='item-submit')
+                        @decore.action(p_type='submit')
                         def per_vie_di1_wi1_di1_wi1_ac1(self, p_data):
-                            return True, 'Hier ist alles Super!'
+                            return True, 'Success!'
+        
+        @decore.dialog(p_title='Edit Person', p_icon='mdi-pencil', p_type='standard', p_display='drawer', p_activator='item-menu')
+        def per_vi1_di2():
+            @decore.widget(p_type='form', p_active_s=[Model.first_name, Model.last_name, Model.companies, Model.accounts])
+            def per_vi1_di2_wi1():
+                @decore.action(p_type='submit')
+                def per_vie_di2_wi1_ac1(self, p_data):
+                    return True, 'Success!'
```

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/css/912.77e6bcbe.css` & `decore_Base-0.0.14/decore_base/sample/spa/static/css/912.77e6bcbe.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/css/app.d398f07d.css` & `decore_Base-0.0.14/decore_base/sample/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/css/vendor.14c9ac7a.css` & `decore_Base-0.0.14/decore_base/sample/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/favicon.ico` & `decore_Base-0.0.14/decore_base/sample/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/icons/favicon-128x128.png` & `decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/icons/favicon-16x16.png` & `decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/icons/favicon-32x32.png` & `decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/icons/favicon-96x96.png` & `decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/js/65.940d9b80.js` & `decore_Base-0.0.14/decore_base/sample/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/js/912.e7a2b7ea.js` & `decore_Base-0.0.14/decore_base/sample/spa/static/js/912.f638ed14.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkuniform_front"] = globalThis["webpackChunkuniform_front"] || []).push([
     [912], {
         5912: (e, t, l) => {
             l.r(t), l.d(t, {
-                default: () => Lt
+                default: () => Nt
             });
             var s = l(9835),
                 a = l(499),
                 i = (l(9665), l(5360)),
                 o = l(8339);
             class n extends i.y {
                 constructor(e) {
@@ -32,15 +32,15 @@
                 constructor(e) {
                     super(e), this.ql = {}, this.action_store = (0, u.j)(), this.context = "none", this.show = !1, this.has_submit_btn = !1, this.has_close_btn = !1
                 }
                 setSubmitBtn() {
                     let e = !1;
                     this.widget_s.forEach((t => {
                         t.action_s.forEach((t => {
-                            "item-submit" == t.activator && (e = !0)
+                            "submit" == t.type && (e = !0)
                         }))
                     })), this.has_submit_btn = e
                 }
                 setCloseBtn() {
                     let e = !1;
                     "last" != this.context && (e = !0), this.has_close_btn = e
                 }
@@ -224,30 +224,30 @@
                 });
             var D = l(3655);
             const Q = j,
                 Z = Q;
             U()(j, "components", {
                 QDrawer: D.Z
             });
-            class F {
+            class V {
                 constructor(e, t) {
                     this.source = e, this.query = t, this.search = "", this.item = {}, this.item_s = [], this.select_s = [], this.count = 0
                 }
                 setItems() {
                     this.source.getItems(this.query).then((e => {
                         this.item_s = e.data.item_s, this.count = e.data.count
                     })).catch((e => {
                         console.log(e)
                     }))
                 }
             }
-            var V = l(1809);
+            var F = l(1809);
 
             function C(e) {
-                const t = (0, V.Q_)(e, {
+                const t = (0, F.Q_)(e, {
                         state: () => ({
                             el: {}
                         }),
                         getters: {},
                         actions: {
                             sendElement(e, t, l, s) {
                                 let a = {
@@ -264,15 +264,15 @@
                         }
                     }),
                     l = t();
                 return l
             }
             class x extends i.y {
                 constructor(e) {
-                    super(e), this.data = (0, a.qj)(new F(this.uniform.source[this.source_id], {})), this.compose_store = C(this.id), this.action_store = (0, u.j)(), this.form_ref = void 0, this.composer_ref = void 0, this.valid = !0, this.item_s_mode = !1
+                    super(e), this.data = (0, a.qj)(new V(this.uniform.source[this.source_id], {})), this.compose_store = C(this.id), this.action_store = (0, u.j)(), this.form_ref = void 0, this.composer_ref = void 0, this.valid = !0, this.item_s_mode = !1
                 }
                 regComposerElement(e) {
                     e.id in this.item || (this.item[e.id] = e.default), e.schema && (this.source.schema[e.id] = e.schema), this.compose_store.el[e.id] = e
                 }
                 refForm(e) {
                     this.form_ref = e
                 }
@@ -305,48 +305,48 @@
                     this.form_ref && await this.form_ref.validate().then((e => {
                         e || (this.valid = !1)
                     })), this.composer_ref && await this.composer_ref.validate().then((e => {
                         e || (this.valid = !1)
                     }))
                 }
                 reset() {
-                    this.form_ref && this.form_ref.reset(), this.composer_ref && this.form_ref.reset()
+                    this.form_ref && this.form_ref.reset(), this.composer_ref && this.composer_ref.reset()
                 }
                 async submit() {
-                    await this.validateWidget(), this.valid && this.action_s.forEach((e => {
-                        "item-submit" == e.activator && this.action_store.sendAction(e, this.data.item, this.data.source.select_s)
+                    this.valid = !0, await this.validateWidget(), this.valid && this.action_s.forEach((e => {
+                        "submit" == e.type && this.action_store.sendAction(e, this.data.item, this.data.source.select_s)
                     }))
                 }
                 getRules(e) {
                     let t = [];
                     if (e in this.data.source.schema) {
                         const l = this.data.source.schema[e];
-                        "string" == l.type && t.push((e => e && e.length > 0 || "Not valid")), "allowed" in l && l.allowed.forEach((e => {
+                        "string" == l.type && t.push((e => e && e.length > 0 || "Not valid")), "integer" == l.type && t.push((e => null !== e && "" !== e && NaN != parseInt(e) || "Not valid")), "allowed" in l && l.allowed.forEach((e => {
                             t.push((t => t && t == e || "Not valid"))
                         }))
                     }
                     return t
                 }
             }
             const E = {
                     key: 0
                 },
-                K = {
+                z = {
                     key: 1
                 },
                 H = {
                     key: 2
                 },
-                z = {
+                K = {
                     key: 3
                 },
-                O = {
+                I = {
                     key: 4
                 },
-                I = {
+                O = {
                     key: 5
                 },
                 A = {
                     inheritAttrs: !1
                 },
                 Y = Object.assign(A, {
                     __name: "uf-widget-composer",
@@ -360,15 +360,15 @@
                                 greedy: "",
                                 ref: e => {
                                     (0, a.SU)(t).refComposer(e)
                                 }
                             }, {
                                 default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)((0, a.SU)(t).compose_store.el, (e => ((0, s.wg)(), (0, s.iD)("span", {
                                     key: e.id
-                                }, ["p" == e.type ? ((0, s.wg)(), (0, s.iD)("p", E, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h1" == e.type ? ((0, s.wg)(), (0, s.iD)("h1", K, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h2" == e.type ? ((0, s.wg)(), (0, s.iD)("h2", H, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h3" == e.type ? ((0, s.wg)(), (0, s.iD)("h3", z, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h4" == e.type ? ((0, s.wg)(), (0, s.iD)("h4", O, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h5" == e.type ? ((0, s.wg)(), (0, s.iD)("h5", I, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "checkbox" == e.type ? ((0, s.wg)(), (0, s.j4)(o, {
+                                }, ["p" == e.type ? ((0, s.wg)(), (0, s.iD)("p", E, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h1" == e.type ? ((0, s.wg)(), (0, s.iD)("h1", z, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h2" == e.type ? ((0, s.wg)(), (0, s.iD)("h2", H, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h3" == e.type ? ((0, s.wg)(), (0, s.iD)("h3", K, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h4" == e.type ? ((0, s.wg)(), (0, s.iD)("h4", I, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "h5" == e.type ? ((0, s.wg)(), (0, s.iD)("h5", O, (0, d.zw)((0, a.SU)(t).item[e.id]), 1)) : (0, s.kq)("", !0), "checkbox" == e.type ? ((0, s.wg)(), (0, s.j4)(o, {
                                     key: 6,
                                     "hide-bottom-space": "",
                                     dense: "",
                                     borderless: "",
                                     modelValue: (0, a.SU)(t).item[e.id],
                                     "onUpdate:modelValue": l => (0, a.SU)(t).item[e.id] = l,
                                     rules: (0, a.SU)(t).getRules(e.id),
@@ -393,21 +393,21 @@
             const M = Y,
                 R = M;
             U()(Y, "components", {
                 QForm: P.Z,
                 QField: T.Z,
                 QCheckbox: B.Z
             });
-            const L = {
+            const N = {
                     key: 0
                 },
-                $ = {
+                L = {
                     key: 1
                 },
-                N = {
+                $ = {
                     key: 2
                 },
                 G = {
                     inheritAttrs: !1
                 },
                 J = Object.assign(G, {
                     __name: "uf-widget-layout",
@@ -431,27 +431,27 @@
                                 }, {
                                     default: (0, s.w5)((() => [(0, s._)("h5", null, (0, d.zw)((0, a.SU)(t).title), 1), (0, s.Wm)(i), (0, s.Wm)(o, {
                                         name: (0, a.SU)(t).icon
                                     }, null, 8, ["name"])])),
                                     _: 1
                                 }), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)((0, a.SU)(t).layout, (l => ((0, s.wg)(), (0, s.iD)("span", {
                                     key: l
-                                }, ["c" == l ? ((0, s.wg)(), (0, s.iD)("span", L, [(0, s.Wm)(u, {
+                                }, ["c" == l ? ((0, s.wg)(), (0, s.iD)("span", N, [(0, s.Wm)(u, {
                                     class: "widget-card-section"
                                 }, {
                                     default: (0, s.w5)((() => [(0, s.WI)(e.$slots, "widget-content")])),
                                     _: 3
-                                })])) : (0, s.kq)("", !0), "e" == l && (0, a.SU)(t).element_s.length >= 1 ? ((0, s.wg)(), (0, s.iD)("span", $, [(0, s.Wm)(u, {
+                                })])) : (0, s.kq)("", !0), "e" == l && (0, a.SU)(t).element_s.length >= 1 ? ((0, s.wg)(), (0, s.iD)("span", L, [(0, s.Wm)(u, {
                                     class: "widget-card-section"
                                 }, {
                                     default: (0, s.w5)((() => [(0, s.Wm)(R, {
                                         use: (0, a.SU)(t)
                                     }, null, 8, ["use"])])),
                                     _: 1
-                                })])) : (0, s.kq)("", !0), "a" == l ? ((0, s.wg)(), (0, s.iD)("span", N, [(0, s.Wm)(c, null, {
+                                })])) : (0, s.kq)("", !0), "a" == l ? ((0, s.wg)(), (0, s.iD)("span", $, [(0, s.Wm)(c, null, {
                                     default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)((0, a.SU)(t).dialog_s, (l => ((0, s.wg)(), (0, s.iD)("span", {
                                         key: l.id
                                     }, ["default-menu" == l.activator ? ((0, s.wg)(), (0, s.j4)(r, {
                                         key: 0,
                                         onClick: s => e.uniform.dialog[l.id].showDialog(void 0, "default", (0, a.SU)(t).source),
                                         icon: l.icon,
                                         dense: "",
@@ -530,19 +530,30 @@
                                     dense: "",
                                     outlined: "",
                                     modelValue: (0, a.SU)(t).data.item[e.name],
                                     "onUpdate:modelValue": l => (0, a.SU)(t).data.item[e.name] = l,
                                     label: e.verbose_name,
                                     rules: (0, a.SU)(t).getRules(e.name),
                                     "lazy-rules": "ondemand"
-                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])) : (0, s.kq)("", !0), e.class.includes("IntegerField") ? ((0, s.wg)(), (0, s.j4)(i, {
+                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])) : (0, s.kq)("", !0), e.class.includes("TextField") ? ((0, s.wg)(), (0, s.j4)(i, {
                                     key: 1,
                                     class: "q-pb-sm",
                                     dense: "",
                                     outlined: "",
+                                    modelValue: (0, a.SU)(t).data.item[e.name],
+                                    "onUpdate:modelValue": l => (0, a.SU)(t).data.item[e.name] = l,
+                                    label: e.verbose_name,
+                                    rules: (0, a.SU)(t).getRules(e.name),
+                                    "lazy-rules": "ondemand",
+                                    autogrow: ""
+                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])) : (0, s.kq)("", !0), e.class.includes("IntegerField") ? ((0, s.wg)(), (0, s.j4)(i, {
+                                    key: 2,
+                                    class: "q-pb-sm",
+                                    dense: "",
+                                    outlined: "",
                                     type: "number",
                                     modelValue: (0, a.SU)(t).data.item[e.name],
                                     "onUpdate:modelValue": l => (0, a.SU)(t).data.item[e.name] = l,
                                     label: e.verbose_name,
                                     rules: (0, a.SU)(t).getRules(e.name),
                                     "lazy-rules": "ondemand"
                                 }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])) : (0, s.kq)("", !0)])))), 128))])),
@@ -687,36 +698,36 @@
                                 use: l
                             }, null, 8, ["use"])) : (0, s.kq)("", !0)])),
                             _: 1
                         }, 8, ["use"]))
                     }
                 },
                 Ze = Qe,
-                Fe = Ze,
-                Ve = {
+                Ve = Ze,
+                Fe = {
                     inheritAttrs: !1
                 },
-                Ce = Object.assign(Ve, {
+                Ce = Object.assign(Fe, {
                     __name: "uf-dialog-standard",
                     setup(e) {
                         const t = (0, s.l1)().use;
                         return (e, l) => ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)((0, a.SU)(t).widget_s, (e => ((0, s.wg)(), (0, s.iD)("span", {
                             key: e.id
-                        }, [(0, s.Wm)(Fe, {
+                        }, [(0, s.Wm)(Ve, {
                             id: e.id
                         }, null, 8, ["id"]), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.widget_s, (e => ((0, s.wg)(), (0, s.iD)("span", {
                             key: e.id
-                        }, [(0, s.Wm)(Fe, {
+                        }, [(0, s.Wm)(Ve, {
                             id: e.id
                         }, null, 8, ["id"])])))), 128))])))), 128))
                     }
                 }),
                 xe = Ce,
                 Ee = xe,
-                Ke = {
+                ze = {
                     __name: "uf-dialog",
                     props: {
                         id: {}
                     },
                     setup(e) {
                         const t = e,
                             l = (0, a.qj)(new r(t.id));
@@ -727,27 +738,27 @@
                                 key: 0,
                                 use: l
                             }, null, 8, ["use"])) : (0, s.kq)("", !0)])),
                             _: 1
                         }, 8, ["use"]))
                     }
                 },
-                He = Ke,
-                ze = He;
-            class Oe {
+                He = ze,
+                Ke = He;
+            class Ie {
                 constructor(e) {
                     this.rowsPerPageOptions = [4, 8, 16, 32, 64, 128, 265, 512, 1024], this.rowsPerPage = e, this.page = 1
                 }
             }
-            class Ie extends i.y {
+            class Oe extends i.y {
                 constructor(e) {
-                    super(e), this.ql = {}, this.route = (0, o.yj)(), this.data = (0, a.qj)(new F(this.uniform.source[this.source_id], {
+                    super(e), this.ql = {}, this.route = (0, o.yj)(), this.data = (0, a.qj)(new V(this.uniform.source[this.source_id], {
                         ...this.query,
                         ...this.route.query
-                    })), this.pagination = (0, a.qj)(new Oe(this.pag_recs)), this.item_menu_target = !1, this.item_menu_model = !1, this.item_menu_row = {}
+                    })), this.pagination = (0, a.qj)(new Ie(this.pag_recs)), this.item_menu_target = !1, this.item_menu_model = !1, this.item_menu_row = {}
                 }
                 get column_s() {
                     let e = [];
                     return e.push({
                         name: "gotos",
                         label: "",
                         field: "gotos"
@@ -874,26 +885,26 @@
                     }
                 });
             var Pe = l(6362),
                 Te = l(3246),
                 Be = l(490),
                 Me = l(1233);
             const Re = Ye,
-                Le = Re;
+                Ne = Re;
             U()(Ye, "components", {
                 QMenu: Pe.Z,
                 QList: Te.Z,
                 QItem: Be.Z,
                 QItemSection: Me.Z,
                 QIcon: ee.Z
             });
-            const $e = {
+            const Le = {
                     class: "row full-width items-center"
                 },
-                Ne = {
+                $e = {
                     class: "col-auto"
                 },
                 Ge = {
                     class: "col-auto"
                 },
                 Je = {
                     key: 0,
@@ -949,15 +960,15 @@
                                     })), s || e.push(l)
                                 })), e
                             })),
                             h = (0, s.Fl)((() => {
                                 let e, l = [];
                                 if ("ForeignKeyField" == n.value.class) e = n.value.rel_model;
                                 else {
-                                    let l = t.data.source.rel_field_s.filter((e => "ForeignKeyField" == e.class && e.backref == n.value.ref_name || "ManyToManyField" == e.class && e.name == n.value.ref_name))[0];
+                                    let l = t.data.source.rel_field_s.filter((e => "ForeignKeyField" == e.class && e.backref == n.value.name || "ManyToManyField" == e.class && e.name == n.value.name))[0];
                                     e = "ForeignKeyField" == l.class ? l.model : l.rel_model
                                 }
                                 let s = t.uniform.getSourceByModel(e);
                                 return s.field_s.forEach((e => {
                                     let s = !1;
                                     Object.entries(t.data.query).forEach((([t]) => {
                                         t.includes(e.name) && (s = !0)
@@ -977,35 +988,33 @@
                             })),
                             g = (0, a.iH)(null);
 
                         function w() {
                             let e = i.query;
                             n.value && !m.value ? t.data.source.getOptions(e, n.value.name, null).then((e => {
                                 g.value = e.data
-                            })) : u.value && m.value && ("ForeignKeyField" == n.value.class ? t.data.source.getOptions(e, n.value.name, u.value.name).then((e => {
-                                g.value = e.data
-                            })) : t.data.source.getOptions(e, n.value.ref_name, u.value.name).then((e => {
+                            })) : u.value && m.value && (n.value.class, t.data.source.getOptions(e, n.value.name, u.value.name).then((e => {
                                 g.value = e.data
                             })))
                         }
 
                         function f() {
                             let e = {
                                     ...i.query
                                 },
                                 t = "";
-                            m.value ? m.value && (t = "ForeignKeyField" == n.value.class ? t + n.value.name + "__" + u.value.name : t + n.value.ref_name + "__" + u.value.name) : t = n.value.name, t = t + "__" + r.value, e[t] = d.value, l.push({
+                            m.value ? m.value && (t = (n.value.class, t + n.value.name + "__" + u.value.name)) : t = n.value.name, t = t + "__" + r.value, e[t] = d.value, l.push({
                                 path: i.path,
                                 query: e
                             })
                         }
                         return (e, l) => {
                             const o = (0, s.up)("q-btn"),
                                 v = (0, s.up)("q-select");
-                            return (0, s.wg)(), (0, s.iD)("div", $e, [(0, s._)("div", Ne, [(0, s.Wm)(o, {
+                            return (0, s.wg)(), (0, s.iD)("div", Le, [(0, s._)("div", $e, [(0, s.Wm)(o, {
                                 class: "float-right text-black",
                                 dense: "",
                                 round: "",
                                 flat: "",
                                 icon: "mdi-content-save",
                                 onClick: l[0] || (l[0] = e => (0, a.SU)(t).uniform.queries.saveQuery((0, a.SU)(i)))
                             })]), (0, s._)("div", Ge, [(0, s.Wm)(o, {
@@ -1217,37 +1226,37 @@
                                 _: 1
                             })
                         }
                     }
                 });
             var Qt = l(996);
             const Zt = Dt,
-                Ft = Zt;
+                Vt = Zt;
             U()(Dt, "components", {
                 QToolbar: w.Z,
                 QSpace: v.Z,
                 QPagination: Qt.Z,
                 QSelect: nt.Z
             });
-            const Vt = {
+            const Ft = {
                     inheritAttrs: !1
                 },
-                Ct = Object.assign(Vt, {
+                Ct = Object.assign(Ft, {
                     __name: "uf-view-layout",
                     setup(e) {
                         const t = (0, s.l1)().use,
                             l = (0, s.Fl)((() => {
                                 let e = "0 px";
                                 return t.ql.hasOwnProperty("header") && (e = t.ql.header.size + "px"), e
                             }));
                         return (e, i) => {
                             const o = (0, s.up)("q-header"),
                                 n = (0, s.up)("q-footer"),
                                 u = (0, s.up)("q-layout");
-                            return (0, s.wg)(), (0, s.iD)(s.HY, null, [(0, s.Wm)(Le, {
+                            return (0, s.wg)(), (0, s.iD)(s.HY, null, [(0, s.Wm)(Ne, {
                                 use: (0, a.SU)(t)
                             }, null, 8, ["use"]), (0, s.Wm)(u, {
                                 container: "",
                                 style: {
                                     height: "calc(100vh - 102px)"
                                 }
                             }, {
@@ -1265,15 +1274,15 @@
                                     class: "view-content",
                                     style: (0, d.j5)({
                                         "padding-top": (0, a.SU)(l)
                                     })
                                 }, [(0, s.WI)(e.$slots, "view-content")], 4), (0, s.Wm)(n, {
                                     reveal: ""
                                 }, {
-                                    default: (0, s.w5)((() => [(0, s.Wm)(Ft, {
+                                    default: (0, s.w5)((() => [(0, s.Wm)(Vt, {
                                         use: (0, a.SU)(t)
                                     }, null, 8, ["use"])])),
                                     _: 1
                                 })])),
                                 _: 3
                             })], 64)
                         }
@@ -1282,18 +1291,18 @@
                 xt = Ct,
                 Et = xt;
             U()(Ct, "components", {
                 QLayout: _.Z,
                 QHeader: g.Z,
                 QFooter: y.Z
             });
-            const Kt = {
+            const zt = {
                     inheritAttrs: !1
                 },
-                Ht = Object.assign(Kt, {
+                Ht = Object.assign(zt, {
                     __name: "uf-view-table",
                     setup(e) {
                         const t = (0, s.l1)().use;
                         t.data.setItems();
                         const l = (0, s.Fl)((() => {
                             let e = 16,
                                 l = "0 px";
@@ -1379,44 +1388,44 @@
                                     _: 2
                                 }, 1032, ["props"])])),
                                 _: 1
                             }, 8, ["columns", "filter", "rows", "style", "pagination", "selected"])
                         }
                     }
                 });
-            var zt = l(7220);
-            const Ot = Ht,
-                It = Ot;
+            var Kt = l(7220);
+            const It = Ht,
+                Ot = It;
             U()(Ht, "components", {
                 QTable: We.Z,
-                QTd: zt.Z,
+                QTd: Kt.Z,
                 QBtn: b.Z,
                 QMenu: Pe.Z,
                 QList: Te.Z,
                 QItem: Be.Z,
                 QItemSection: Me.Z
             });
             const At = {
                     __name: "uf-view",
                     props: {
                         id: {}
                     },
                     setup(e) {
                         const t = e,
-                            l = (0, a.qj)(new Ie(t.id));
+                            l = (0, a.qj)(new Oe(t.id));
                         return (0, s.bv)((() => {
                             for (const e of l.dialog_s)
                                 if ("none" == e.activator) {
                                     l.ref[e.id].showDialog({}, "last", l.data.source);
                                     break
                                 }
                         })), (e, t) => ((0, s.wg)(), (0, s.j4)(Et, {
                             use: l
                         }, {
-                            "view-content": (0, s.w5)((() => ["table" == l.type ? ((0, s.wg)(), (0, s.j4)(It, {
+                            "view-content": (0, s.w5)((() => ["table" == l.type ? ((0, s.wg)(), (0, s.j4)(Ot, {
                                 key: 0,
                                 use: l
                             }, null, 8, ["use"])) : (0, s.kq)("", !0)])),
                             _: 1
                         }, 8, ["use"]))
                     }
                 },
@@ -1428,28 +1437,28 @@
                 Bt = {
                     __name: "uf-base",
                     setup(e) {
                         const t = (0, o.yj)(),
                             l = (0, a.qj)(new n(t.params.base_id));
                         return (e, t) => {
                             const a = (0, s.up)("q-page");
-                            return (0, s.wg)(), (0, s.iD)(s.HY, null, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(l.route_dialog_s, (e => ((0, s.wg)(), (0, s.j4)(ze, {
+                            return (0, s.wg)(), (0, s.iD)(s.HY, null, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(l.route_dialog_s, (e => ((0, s.wg)(), (0, s.j4)(Ke, {
                                 key: e.id,
                                 id: e.id
                             }, null, 8, ["id"])))), 128)), (0, s.Wm)(a, null, {
                                 default: (0, s.w5)((() => [l.getView().id ? ((0, s.wg)(), (0, s.iD)("span", Tt, [(0, s.Wm)(Pt, {
                                     id: l.getView().id
                                 }, null, 8, ["id"])])) : (0, s.kq)("", !0)])),
                                 _: 1
                             })], 64)
                         }
                     }
                 };
             var Mt = l(9885);
             const Rt = Bt,
-                Lt = Rt;
+                Nt = Rt;
             U()(Bt, "components", {
                 QPage: Mt.Z
             })
         }
     }
 ]);
```

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/js/app.7ef3a1f6.js` & `decore_Base-0.0.14/decore_base/sample/spa/static/js/app.465385a3.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -81,15 +81,15 @@
                                     _ = (0, s.up)("q-item"),
                                     y = (0, s.up)("q-chip"),
                                     b = (0, s.up)("q-tree"),
                                     k = (0, s.up)("q-drawer");
                                 return (0, s.wg)(), (0, s.j4)(k, {
                                     "show-if-above": "",
                                     model: !0,
-                                    width: 375,
+                                    width: 300,
                                     side: "left",
                                     breakpoint: 0,
                                     bordered: "",
                                     mini: (0, i.SU)(t).drawer_mini
                                 }, {
                                     default: (0, s.w5)((() => [(0, s.Wm)(w, {
                                         class: "bg-grey-2"
@@ -246,26 +246,26 @@
                     b = n(490),
                     k = n(1233),
                     q = n(2857),
                     j = n(7691),
                     C = n(9984),
                     S = n.n(C);
                 const x = w,
-                    E = x;
+                    W = x;
                 S()(w, "components", {
                     QDrawer: v.Z,
                     QToolbar: g.Z,
                     QBtn: _.Z,
                     QTree: y.Z,
                     QItem: b.Z,
                     QItemSection: k.Z,
                     QIcon: q.Z,
                     QChip: j.Z
                 });
-                const W = {
+                const E = {
                         class: "text-weight-bold"
                     },
                     Q = {
                         class: "text-grey"
                     };
 
                 function Z(e, t, n, o, r, i) {
@@ -283,15 +283,15 @@
                                 width: "500px"
                             }
                         }, {
                             default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(o.action_store.active_s, (e => ((0, s.wg)(), (0, s.j4)(a, {
                                 key: e.id,
                                 class: "row items-center no-wrap"
                             }, {
-                                default: (0, s.w5)((() => [(0, s._)("div", null, [(0, s._)("div", W, (0, d.zw)(e.title), 1), (0, s._)("div", Q, (0, d.zw)(e.result), 1)])])),
+                                default: (0, s.w5)((() => [(0, s._)("div", null, [(0, s._)("div", E, (0, d.zw)(e.title), 1), (0, s._)("div", Q, (0, d.zw)(e.result), 1)])])),
                                 _: 2
                             }, 1024)))), 128))])),
                             _: 1
                         })])),
                         _: 1
                     }, 8, ["modelValue"])
                 }
@@ -331,17 +331,18 @@
                                     r = (0, s.up)("q-input"),
                                     a = (0, s.up)("q-tooltip"),
                                     l = (0, s.up)("q-btn"),
                                     c = (0, s.up)("q-toolbar"),
                                     h = (0, s.up)("q-header"),
                                     p = (0, s.up)("router-view"),
                                     m = (0, s.up)("q-page-container"),
-                                    f = (0, s.up)("q-footer"),
-                                    w = (0, s.up)("q-layout");
-                                return (0, s.wg)(), (0, s.j4)(w, null, {
+                                    f = (0, s.up)("q-space"),
+                                    w = (0, s.up)("q-footer"),
+                                    v = (0, s.up)("q-layout");
+                                return (0, s.wg)(), (0, s.j4)(v, null, {
                                     default: (0, s.w5)((() => [(0, s.Wm)(u.Z, {
                                         use: (0, i.SU)(t)
                                     }, null, 8, ["use"]), (0, s.Wm)(h, {
                                         bordered: "",
                                         class: "bg-black text-white"
                                     }, {
                                         default: (0, s.w5)((() => [(0, s.Wm)(c, null, {
@@ -370,146 +371,155 @@
                                                     _: 1
                                                 })])),
                                                 _: 1
                                             })) : (0, s.kq)("", !0)])),
                                             _: 1
                                         })])),
                                         _: 1
-                                    }), (0, s.Wm)(E, {
+                                    }), (0, s.Wm)(W, {
                                         use: (0, i.SU)(t)
                                     }, null, 8, ["use"]), (0, s.Wm)(m, null, {
                                         default: (0, s.w5)((() => [((0, s.wg)(), (0, s.j4)(p, {
                                             key: e.$route.fullPath
                                         }))])),
                                         _: 1
-                                    }), (0, s.Wm)(B), (0, s.Wm)(f, {
+                                    }), (0, s.Wm)(B), (0, s.Wm)(w, {
                                         bordered: "",
                                         class: "bg-grey-8 text-white"
                                     }, {
                                         default: (0, s.w5)((() => [(0, s.Wm)(c, {
                                             dense: ""
+                                        }, {
+                                            default: (0, s.w5)((() => [(0, s.Wm)(f), (0, s.Wm)(l, {
+                                                flat: "",
+                                                icon: "mdi-coffee",
+                                                href: "https://ko-fi.com/decore_base"
+                                            })])),
+                                            _: 1
                                         })])),
                                         _: 1
                                     })])),
                                     _: 1
                                 })
                             }
                         }
                     });
                 var F = n(7605),
                     I = n(6602),
                     V = n(1973),
                     z = n(6858),
                     H = n(6611),
                     R = n(2133),
-                    K = n(1378);
-                const X = N,
-                    J = X;
+                    K = n(1378),
+                    X = n(136);
+                const J = N,
+                    Y = J;
                 S()(N, "components", {
                     QLayout: F.Z,
                     QHeader: I.Z,
                     QToolbar: g.Z,
                     QToolbarTitle: V.Z,
                     QBtn: _.Z,
                     QTooltip: z.Z,
                     QInput: H.Z,
                     QPageContainer: R.Z,
-                    QFooter: K.Z
+                    QFooter: K.Z,
+                    QSpace: X.Z
                 });
-                var Y = n(5360);
-                class $ extends Y.y {
+                var $ = n(5360);
+                class G extends $.y {
                     constructor(e) {
                         super(e), this.ql = {}, this.drawer_icon = "mdi-backburger", this.drawer_mini = !1, this.expanded_nodes = []
                     }
                     toogleLayoutDrawer() {
                         this.drawer_mini = !this.drawer_mini, this.drawer_mini ? this.drawer_icon = "mdi-forwardburger" : this.drawer_icon = "mdi-backburger"
                     }
                 }
-                const G = (0, s.aZ)({
+                const ee = (0, s.aZ)({
                         name: "App",
                         components: {
-                            "uf-app-layout": J
+                            "uf-app-layout": Y
                         },
                         setup() {
-                            const e = (0, i.qj)(new $("app"));
+                            const e = (0, i.qj)(new G("app"));
                             return (0, l.Z)((() => ({
                                 title: e.title
                             }))), {
                                 use: e
                             }
                         }
                     }),
-                    ee = (0, T.Z)(G, [
+                    te = (0, T.Z)(ee, [
                         ["render", a]
                     ]),
-                    te = ee;
-                var ne = n(3340),
-                    oe = n(1809);
-                const re = (0, ne.h)((() => {
-                    const e = (0, oe.WB)();
+                    ne = te;
+                var oe = n(3340),
+                    re = n(1809);
+                const ie = (0, oe.h)((() => {
+                    const e = (0, re.WB)();
                     return e
                 }));
-                var ie = n(8339);
-                const se = [{
+                var se = n(8339);
+                const ae = [{
                         path: "/:base_id/:view_id",
                         component: () => Promise.all([n.e(736), n.e(912)]).then(n.bind(n, 5912))
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => n.e(65).then(n.bind(n, 7065))
                     }],
-                    ae = se;
-                var le = n(5047);
-                const de = (0, ne.BC)((function() {
-                    const e = ie.PO,
-                        t = (0, ie.p7)({
+                    le = ae;
+                var de = n(5047);
+                const ue = (0, oe.BC)((function() {
+                    const e = se.PO,
+                        t = (0, se.p7)({
                             scrollBehavior: () => ({
                                 left: 0,
                                 top: 0
                             }),
-                            routes: ae,
+                            routes: le,
                             history: e("/")
                         });
                     return t.beforeEach(((e, t) => {
-                        const n = (0, le.I)();
+                        const n = (0, de.I)();
                         return n.use.app.expanded_nodes.push(e.params.base_id), !0
                     })), t
                 }));
-                async function ue(e, t) {
-                    const n = e(te);
+                async function ce(e, t) {
+                    const n = e(ne);
                     n.use(r.Z, t);
-                    const o = "function" === typeof re ? await re({}) : re;
+                    const o = "function" === typeof ie ? await ie({}) : ie;
                     n.use(o);
-                    const s = (0, i.Xl)("function" === typeof de ? await de({
+                    const s = (0, i.Xl)("function" === typeof ue ? await ue({
                         store: o
-                    }) : de);
+                    }) : ue);
                     return o.use((({
                         store: e
                     }) => {
                         e.router = s
                     })), {
                         app: n,
                         store: o,
                         router: s
                     }
                 }
-                const ce = {
+                const he = {
                         config: {}
                     },
-                    he = "/static/",
-                    pe = /\/\//,
-                    me = e => (he + e).replace(pe, "/");
-                async function fe({
+                    pe = "/static/",
+                    me = /\/\//,
+                    fe = e => (pe + e).replace(me, "/");
+                async function we({
                     app: e,
                     router: t,
                     store: n
                 }, o) {
                     let r = !1;
                     const i = e => {
                             try {
-                                return me(t.resolve(e).href)
+                                return fe(t.resolve(e).href)
                             } catch (n) {}
                             return Object(e) === e ? null : e
                         },
                         s = e => {
                             if (r = !0, "string" === typeof e && /^https?:\/\//.test(e)) return void(window.location.href = e);
                             const t = i(e);
                             null !== t && (window.location.href = t)
@@ -519,28 +529,28 @@
                         await o[d]({
                             app: e,
                             router: t,
                             store: n,
                             ssrContext: null,
                             redirect: s,
                             urlPath: a,
-                            publicPath: he
+                            publicPath: pe
                         })
                     } catch (l) {
                         return l && l.url ? void s(l.url) : void console.error("[Quasar] boot error:", l)
                     }!0 !== r && (e.use(t), e.mount("#q-app"))
                 }
-                ue(o.ri, ce).then((e => {
+                ce(o.ri, he).then((e => {
                     const [t, o] = void 0 !== Promise.allSettled ? ["allSettled", e => e.map((e => {
                         if ("rejected" !== e.status) return e.value.default;
                         console.error("[Quasar] boot error:", e.reason)
                     }))] : ["all", e => e.map((e => e.default))];
                     return Promise[t]([Promise.resolve().then(n.bind(n, 6898))]).then((t => {
                         const n = o(t).filter((e => "function" === typeof e));
-                        fe(e, n)
+                        we(e, n)
                     }))
                 }))
             },
             6898: (e, t, n) => {
                 n.r(t), n.d(t, {
                     default: () => u
                 });
@@ -808,15 +818,15 @@
             })
         }
     })(), (() => {
         n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, o) => (n.f[o](e, t), t)), []))
     })(), (() => {
         n.u = e => "js/" + e + "." + {
             65: "940d9b80",
-            912: "e7a2b7ea"
+            912: "f638ed14"
         } [e] + ".js"
     })(), (() => {
         n.miniCssF = e => "css/" + e + ".77e6bcbe.css"
     })(), (() => {
         n.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
```

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/static/js/vendor.03c46c80.js` & `decore_Base-0.0.14/decore_base/sample/spa/static/js/vendor.03c46c80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/decore_base/sample/spa/templates/index.html` & `decore_Base-0.0.14/decore_base/sample/spa/templates/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><base href=/static/ ><title>Uniform Front</title><meta charset=utf-8><meta name=description content="A part of Unform Famework"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><meta name=api_prod_port content={{port}}><meta name=api_dev_port content=5566><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=/static/js/vendor.03c46c80.js></script><script defer src=/static/js/app.7ef3a1f6.js></script><link href=/static/css/vendor.14c9ac7a.css rel=stylesheet><link href=/static/css/app.d398f07d.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><base href=/static/ ><title>Uniform Front</title><meta charset=utf-8><meta name=description content="A part of Unform Famework"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><meta name=api_prod_port content={{port}}><meta name=api_dev_port content=5566><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=/static/js/vendor.03c46c80.js></script><script defer src=/static/js/app.465385a3.js></script><link href=/static/css/vendor.14c9ac7a.css rel=stylesheet><link href=/static/css/app.d398f07d.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `decore_Base-0.0.13/decore_base/sample/state/database.db` & `decore_Base-0.0.14/decore_base/sample/state/database.db`

 * *Files 1% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -6557,12 +6557,13 @@
 INSERT INTO company_model VALUES('ebf5376d-f3e9-11ed-9f45-309c23812330','Greyvoid',NULL,'object',NULL,88);
 INSERT INTO company_model VALUES('ebf73338-f3e9-11ed-925a-309c23812330','Sistemos',NULL,'object',NULL,118);
 INSERT INTO company_model VALUES('ebf92f02-f3e9-11ed-95b4-309c23812330','Shirokiya',NULL,'object',NULL,108);
 INSERT INTO company_model VALUES('ebfb532e-f3e9-11ed-a65d-309c23812330','Verizon Wireless',NULL,'object',NULL,37);
 INSERT INTO company_model VALUES('ebfd27c0-f3e9-11ed-98b5-309c23812330','Frontier Airlines',NULL,'object',NULL,42);
 INSERT INTO company_model VALUES('ebff225f-f3e9-11ed-948c-309c23812330','Dollar Tree',NULL,'object',NULL,79);
 CREATE TABLE IF NOT EXISTS "account_model" ("id" VARCHAR(255) NOT NULL PRIMARY KEY, "title" VARCHAR(255) NOT NULL, "desc" VARCHAR(255), "item_type" VARCHAR(255) NOT NULL, "parent_path" VARCHAR(255), "person_id" VARCHAR(255) NOT NULL, "email" VARCHAR(255) NOT NULL, "password" VARCHAR NOT NULL, FOREIGN KEY ("person_id") REFERENCES "person_model" ("id"));
+CREATE TABLE IF NOT EXISTS "test_model" ("id" VARCHAR(255) NOT NULL PRIMARY KEY, "title" VARCHAR(255) NOT NULL, "desc" VARCHAR(255), "item_type" VARCHAR(255) NOT NULL, "parent_path" VARCHAR(255), "text_field" TEXT NOT NULL, "charfield" VARCHAR(255) NOT NULL, "intfield" INTEGER NOT NULL, "textfield" TEXT NOT NULL);
 CREATE INDEX "company_modelperson_modelthrough_company_model_id" ON "company_model_person_model_through" ("company_model_id");
 CREATE INDEX "company_modelperson_modelthrough_person_model_id" ON "company_model_person_model_through" ("person_model_id");
 CREATE UNIQUE INDEX "company_modelperson_modelthrough_company_model_id_person_396c24e" ON "company_model_person_model_through" ("company_model_id", "person_model_id");
 CREATE INDEX "account_model_person_id" ON "account_model" ("person_id");
 COMMIT;
```

### Comparing `decore_Base-0.0.13/decore_base/sample/state/querybase.db` & `decore_Base-0.0.14/decore_base/sample/state/querybase.db`

 * *Files 17% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -1,5 +1,6 @@
 PRAGMA foreign_keys=OFF;
 BEGIN TRANSACTION;
 CREATE TABLE IF NOT EXISTS "decore_query" ("id" VARCHAR(255) NOT NULL PRIMARY KEY, "parent_id" VARCHAR(255), "base_id" VARCHAR(255) NOT NULL, "view_id" VARCHAR(255) NOT NULL, "type" VARCHAR(255) NOT NULL, "title" VARCHAR(255) NOT NULL, "key" VARCHAR(255) NOT NULL, "value" VARCHAR(255) NOT NULL, "to" VARCHAR(255) NOT NULL, "depth" INTEGER NOT NULL, FOREIGN KEY ("parent_id") REFERENCES "decore_query" ("id"));
+INSERT INTO decore_query VALUES('01f53118-ff64-11ed-8709-309c23812330',NULL,'Global_management_base','per_vi1','user','companies__title__eq:[''Royal Gas'']','companies__title__eq','["Royal Gas"]','{"path": "/Global_management_base/per_vi1", "query": {"companies__title__eq": ["Royal Gas"]}}',0);
 CREATE INDEX "decore_query_parent_id" ON "decore_query" ("parent_id");
 COMMIT;
```

### Comparing `decore_Base-0.0.13/requirements.txt` & `decore_Base-0.0.14/requirements.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.13/setup.cfg` & `decore_Base-0.0.14/setup.cfg`

 * *Files identical despite different names*

