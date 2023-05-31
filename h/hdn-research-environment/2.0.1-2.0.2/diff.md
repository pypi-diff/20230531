# Comparing `tmp/hdn-research-environment-2.0.1.tar.gz` & `tmp/hdn-research-environment-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-2.0.1.tar", last modified: Mon May 29 12:32:44 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-2.0.2.tar", last modified: Wed May 31 14:41:02 2023, max compression
```

## Comparing `hdn-research-environment-2.0.1.tar` & `hdn-research-environment-2.0.2.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.0.1/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.0.1/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.0.1/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.1/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/api/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/api/v1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/api/v1/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/api/v1/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/api/v1/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/api/v2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/api/v2/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      943 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/api/v2/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.1/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2832 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.0.1/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3562 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      792 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/mailers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.1/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.1/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2317 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    18754 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4342 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.0.1/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.1/environment/static/environment/css/environment-base.css
--rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/static/environment/css/manage_billing_account.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.0.1/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     2637 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     6684 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.1/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1111 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.0.1/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.1/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.0.1/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     5481 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3871 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/templates/environment/research_environments.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.1/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.1/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.1/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3514 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.1/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.0.1/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.1/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    13311 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.1/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     2871 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.1/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-05-29 12:32:44.000000 hdn-research-environment-2.0.1/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.1/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.0.2/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.0.2/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.0.2/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/api/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/api/v1/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/api/v1/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/api/v1/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/api/v1/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/api/v2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/api/v2/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.2/environment/api/v2/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2832 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.0.2/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3562 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      792 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/mailers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.2/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.2/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    19372 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.2/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4342 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.0.2/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.0.2/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2637 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     7049 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.2/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1854 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.2/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.0.2/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.0.2/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5481 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3871 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3514 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.0.2/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    13384 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.2/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2954 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.2/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.2/setup.py
```

### Comparing `hdn-research-environment-2.0.1/LICENSE` & `hdn-research-environment-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/PKG-INFO` & `hdn-research-environment-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.0.1/environment/api/v1/__init__.py` & `hdn-research-environment-2.0.2/environment/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/api/v1/auth.py` & `hdn-research-environment-2.0.2/environment/api/v1/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/api/v1/decorators.py` & `hdn-research-environment-2.0.2/environment/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/api/v2/__init__.py` & `hdn-research-environment-2.0.2/environment/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/api/v2/decorators.py` & `hdn-research-environment-2.0.2/environment/api/v2/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,7 @@
         request.url = f"{api_url}{request.url}"
         prepped = request.prepare()
         _apply_api_credentials(prepped, api_url)
 
         return session.send(prepped)
 
     return wrapper
-
```

### Comparing `hdn-research-environment-2.0.1/environment/constants.py` & `hdn-research-environment-2.0.2/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/decorators.py` & `hdn-research-environment-2.0.2/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/deserializers.py` & `hdn-research-environment-2.0.2/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/entities.py` & `hdn-research-environment-2.0.2/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/exceptions.py` & `hdn-research-environment-2.0.2/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/forms.py` & `hdn-research-environment-2.0.2/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/mailers.py` & `hdn-research-environment-2.0.2/environment/mailers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/migrations/0001_initial.py` & `hdn-research-environment-2.0.2/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.0.2/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.0.2/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-2.0.2/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/models.py` & `hdn-research-environment-2.0.2/environment/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,22 +39,25 @@
     is_revoked = models.BooleanField(default=False)
 
 
 class Workflow(models.Model):
     objects = WorkflowManager()
 
     project = models.ForeignKey(
-        "project.PublishedProject", related_name="workflows", on_delete=models.CASCADE
+        "project.PublishedProject",
+        related_name="workflows",
+        on_delete=models.CASCADE,
+        null=True,
     )
     user = models.ForeignKey(
         "user.User", related_name="workflows", on_delete=models.CASCADE
     )
     execution_resource_name = models.CharField(max_length=256, unique=True)
 
-    workspace_name = models.CharField(max_length=256)
+    workspace_name = models.CharField(max_length=256, null=True)
 
     INPROGRESS = 0
     SUCCESS = 1
     FAILED = 2
     STATUS_CHOICES = [
         (INPROGRESS, "In Progress"),
         (SUCCESS, "Succeeded"),
@@ -63,15 +66,19 @@
     status = models.PositiveSmallIntegerField(choices=STATUS_CHOICES)
 
     CREATE = 0
     DESTROY = 1
     START = 2
     PAUSE = 3
     CHANGE = 4
+    WORKSPACE_CREATE = 5
+    WORKSPACE_DESTROY = 6
     TYPE_CHOICES = [
         (CREATE, "Creating"),
         (DESTROY, "Destroying"),
         (START, "Starting"),
         (PAUSE, "Pausing"),
         (CHANGE, "Changing"),
+        (WORKSPACE_CREATE, "Creating Workspace"),
+        (WORKSPACE_DESTROY, "Destroying Workspace"),
     ]
     type = models.PositiveSmallIntegerField(choices=TYPE_CHOICES)
```

### Comparing `hdn-research-environment-2.0.1/environment/services.py` & `hdn-research-environment-2.0.2/environment/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Iterable, Optional
+from typing import Tuple, Iterable, Optional, Dict
 from collections import defaultdict
 
 from django.db.models import Model
 from django.core.mail import send_mail
 from django.template import loader
 from django.conf import settings
 from django.apps import apps
@@ -176,14 +176,20 @@
         email=user.cloud_identity.email,
         billing_account_id=billing_account_id,
         region=region,
     )
     if not response.ok:
         error_message = response.json()["error"]
         raise CreateWorkspaceFailed(error_message)
+    execution_resource_name = response.json()["execution-name"]
+    persist_workflow(
+        user=user,
+        execution_resource_name=execution_resource_name,
+        type=Workflow.WORKSPACE_CREATE,
+    )
 
 
 def _create_workbench_kwargs(
     user: User,
     project: PublishedProject,
     workspace_name: str,
     instance_type: str,
@@ -351,14 +357,24 @@
     return [
         (environment, project, workflows)
         for project, environment, workflows in project_environment_workflow_triplets
         if environment is None and workflows.exists()
     ]
 
 
+def get_workspaces_being_created(user: User) -> Dict[str, Tuple[None, None, Workflow]]:
+    workspace_creation_workflows = Workflow.objects.filter(
+        user=user, type=Workflow.WORKSPACE_CREATE, status=Workflow.INPROGRESS
+    )
+    return {
+        workflow.get_type_display(): (None, None, workflow)
+        for workflow in workspace_creation_workflows
+    }
+
+
 def get_environment_project_pairs_with_expired_access(
     user: User,
 ) -> Iterable[Tuple[ResearchEnvironment, PublishedProject]]:
     all_environment_project_pairs = get_environments_with_projects(user)
     return [
         (environment, project)
         for environment, project in all_environment_project_pairs
@@ -367,15 +383,15 @@
 
 
 def sort_environments_per_workspace(
     environment_project_workflow_triplets: Iterable[
         Tuple[ResearchEnvironment, PublishedProject, Iterable[Workflow]]
     ],
     workspaces: Iterable[ResearchWorkspace],
-):
+) -> Dict[str, Tuple[ResearchEnvironment, PublishedProject, Iterable[Workflow]]]:
     sorted_environments_project_workflow_triplets = defaultdict(
         list, {workspace.gcp_project_id: [] for workspace in workspaces}
     )
     for environment, project, workflows in environment_project_workflow_triplets:
         if environment:
             sorted_environments_project_workflow_triplets[
                 environment.workspace_name
@@ -545,15 +561,14 @@
     return execution.state
 
 
 def mark_workflow_as_finished(
     execution_resource_name: str, execution_state: executions.Execution.State
 ):
     workflow = Workflow.objects.get(execution_resource_name=execution_resource_name)
-    # workflow.status = Workflow.SUCCESS
     if execution_state == executions.Execution.State.SUCCEEDED:
         workflow.status = Workflow.SUCCESS
     else:
         workflow.status = Workflow.FAILED
 
     workflow.save()
```

### Comparing `hdn-research-environment-2.0.1/environment/signals.py` & `hdn-research-environment-2.0.2/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.0.2/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.0.2/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.0.2/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.0.2/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/tasks.py` & `hdn-research-environment-2.0.2/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-2.0.2/environment/templates/environment/_available_environments_list.html`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,20 @@
     {% elif recent_workflow_succeeded %}
         <div class="alert alert-success" role="alert">
             {{ recent_workflow.get_type_display }} {{ recent_workflow.project }} finished!
         </div>
     {% endif %}
 {% endif %}
 
-<div class="d-flex justify-content-between mb-3 px-4 container">
-    <h6 class="text-center"><strong>Workspace Name</strong></h6>
+<div class="d-flex flex-column align-items-end px-4 mb-3">
     <a class="btn btn-primary btn-sm" href="{% url 'create_workspace' %}">
       + Workspace
     </a>
 </div>
 
-<hr>
-
 <div id="accordion">
     {% for workspace_name, environments_project_workflow_triplets in workspace_project_environment_workflow_triplets_dict.items %}
         {% with collapse="collapse-"|add:workspace_name heading="heading-"|add:workspace_name %}
             <div class="card">
                 <div class="card-header" id="{{ heading }}">
                     <button class="btn btn-link" data-toggle="collapse" data-target="#{{ collapse }}" aria-expanded="true" aria-controls="{{ collapse }}">
                         <h6 class="mb-0">
@@ -34,53 +31,57 @@
                 </div>
 
                 <div id="{{ collapse }}" class="collapse show" aria-labelledby="{{ heading }}" data-parent="#accordion">
                     <div class="card-body">
                         {% if environments_project_workflow_triplets|length %}
                             <ul class="list-group list-group-flush">
                                 {% for environment, project, workflows in environments_project_workflow_triplets %}
-                                    <li class="list-group-item">
-                                        <div class="row">
-                                            <div class="col-md-3">
-                                                <a href="{% url 'published_project' project.slug project.version %}" target="_blank">
-                                                    {{ project }}
-                                                </a>
-                                            </div>
-                                            <div class="col-md-3">
-                                                <small>
-                                                    <i>Environment type:</i> {{ environment.type.value|capfirst }}<br>
-                                                    <i>Instance type:</i> {{ environment.instance_type.value }}<br>
-                                                    <i>Region:</i> {{ environment.region.value }}
-                                                </small>
-                                            </div>
-                                            <div class="col-md-2">
-                                                {% if workflows.exists %}
-                                                    {{ workflows.first.get_type_display }}
-                                                {% else %}
-                                                    {{ environment.status.value|capfirst }}
-                                                {% endif %}
-                                            </div>
-                                            <div class="col-md-4">
-                                                <div class="d-flex flex-wrap">
+                                    {% if not environment and not project %}
+                                        <div class="loader" style="margin: 18px; font-size: 5px">Loading...</div>
+                                    {% else %}
+                                        <li class="list-group-item">
+                                            <div class="row">
+                                                <div class="col-md-3">
+                                                    <a href="{% url 'published_project' project.slug project.version %}" target="_blank">
+                                                        {{ project }}
+                                                    </a>
+                                                </div>
+                                                <div class="col-md-3">
+                                                    <small>
+                                                        <i>Environment type:</i> {{ environment.type.value|capfirst }}<br>
+                                                        <i>Instance type:</i> {{ environment.instance_type.value }}<br>
+                                                        <i>Region:</i> {{ environment.region.value }}
+                                                    </small>
+                                                </div>
+                                                <div class="col-md-2">
                                                     {% if workflows.exists %}
-                                                        <div class="loader" style="margin: 18px; font-size: 5px">Loading...</div>
-                                                    {% elif environment.is_running or environment.is_paused %}
-                                                        {% if environment.is_running %}
-                                                            <a href="{{ environment.url }}" target="_blank" class="btn btn-sm btn-success m-1">Open</a>
-                                                            {% environment_modal_button environment=environment project=project button_type="modal_pause" %}
-                                                        {% else %}
-                                                            {% environment_modal_button environment=environment project=project button_type="modal_start" %}
-                                                        {% endif %}
-                                                        {% environment_modal_button environment=environment project=project button_type="modal_instance" %}
-                                                        {% environment_modal_button environment=environment project=project button_type="modal_destroy" %}
+                                                        {{ workflows.first.get_type_display }}
+                                                    {% else %}
+                                                        {{ environment.status.value|capfirst }}
                                                     {% endif %}
                                                 </div>
+                                                <div class="col-md-4">
+                                                    <div class="d-flex flex-wrap">
+                                                        {% if workflows.exists %}
+                                                            <div class="loader" style="margin: 18px; font-size: 5px">Loading...</div>
+                                                        {% elif environment.is_running or environment.is_paused %}
+                                                            {% if environment.is_running %}
+                                                                <a href="{{ environment.url }}" target="_blank" class="btn btn-sm btn-success m-1">Open</a>
+                                                                {% environment_modal_button environment=environment project=project button_type="modal_pause" %}
+                                                            {% else %}
+                                                                {% environment_modal_button environment=environment project=project button_type="modal_start" %}
+                                                            {% endif %}
+                                                            {% environment_modal_button environment=environment project=project button_type="modal_instance" %}
+                                                            {% environment_modal_button environment=environment project=project button_type="modal_destroy" %}
+                                                        {% endif %}
+                                                    </div>
+                                                </div>
                                             </div>
-                                        </div>
-                                    </li>
+                                        </li>
+                                    {% endif %}
                                 {% endfor %}
                             </ul>
                         {% else %}
                             <div class="text-center">
                                 You don't have any worbenches in this workspace.<br>
                                 Create one in the "Projects" tab.
                             </div>
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
 {% load action_buttons %} {% if recent_workflow %} {% if recent_workflow_failed
 %}
 {{ recent_workflow.get_type_display }} {{ recent_workflow.project }} failed!
 Try again later.
 {% elif recent_workflow_succeeded %}
 {{ recent_workflow.get_type_display }} {{ recent_workflow.project }} finished!
 {% endif %} {% endif %}
-* Workspace Name *
 +_Workspace
-===============================================================================
 {% for workspace_name, environments_project_workflow_triplets in
 workspace_project_environment_workflow_triplets_dict.items %} {% with
 collapse="collapse-"|add:workspace_name heading="heading-"|add:workspace_name
 %}
 * {{ workspace_name }} *
 {% if environments_project_workflow_triplets|length %}
     * {% for environment, project, workflows in
-      environments_project_workflow_triplets %}
+      environments_project_workflow_triplets %} {% if not environment and not
+      project %}
+      Loading...
+    * {% else %}
     * {{_project_}}
       Environment type: {{ environment.type.value|capfirst }}
       Instance type: {{ environment.instance_type.value }}
       Region: {{ environment.region.value }}
       {% if workflows.exists %} {{ workflows.first.get_type_display }} {% else
       %} {{ environment.status.value|capfirst }} {% endif %}
       {% if workflows.exists %}
@@ -29,14 +30,14 @@
       environment=environment project=project button_type="modal_pause" %} {%
       else %} {% environment_modal_button environment=environment
       project=project button_type="modal_start" %} {% endif %} {%
       environment_modal_button environment=environment project=project
       button_type="modal_instance" %} {% environment_modal_button
       environment=environment project=project button_type="modal_destroy" %} {%
       endif %}
-    * {% endfor %}
+    * {% endif %} {% endfor %}
 {% else %}
 You don't have any worbenches in this workspace.
 Create one in the "Projects" tab.
 {% endif %}
 {% endwith %} {% endfor %}
```

### Comparing `hdn-research-environment-2.0.1/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-2.0.2/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.0.2/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.0.2/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/templates/environment/create_workspace.html` & `hdn-research-environment-2.0.2/environment/templates/environment/create_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.0.2/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-2.0.2/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/templates/environment/research_environments.html` & `hdn-research-environment-2.0.2/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.0.2/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.0.2/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/tests/helpers.py` & `hdn-research-environment-2.0.2/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/tests/mocks.py` & `hdn-research-environment-2.0.2/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/tests/test_decorators.py` & `hdn-research-environment-2.0.2/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/tests/test_services.py` & `hdn-research-environment-2.0.2/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/tests/test_signals.py` & `hdn-research-environment-2.0.2/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/tests/test_utilities.py` & `hdn-research-environment-2.0.2/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/tests/test_validators.py` & `hdn-research-environment-2.0.2/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/tests/test_views.py` & `hdn-research-environment-2.0.2/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/urls.py` & `hdn-research-environment-2.0.2/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/utilities.py` & `hdn-research-environment-2.0.2/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.1/environment/views.py` & `hdn-research-environment-2.0.2/environment/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,28 +80,35 @@
         )
     )
     projects_with_environments_being_created = (
         services.get_projects_with_environment_being_created(
             available_project_environment_workflow_triplets
         )
     )
+    workspaces_being_created_dict = services.get_workspaces_being_created(request.user)
     environment_projects_pairs_with_creating = (
-        projects_with_environments_being_created + environment_project_workflow_triplets
+        projects_with_environments_being_created
+        + environment_project_workflow_triplets
+        + workspaces_being_created_dict.values()
     )
 
     sorted_environments_project_workflow_triplets_dict = (
         services.sort_environments_per_workspace(
             environment_projects_pairs_with_creating, workspaces_list
         )
     )
 
+    sorted_environments_project_workflow_triplets_with_creating_dict = {
+        **sorted_environments_project_workflow_triplets_dict,
+        **workspaces_being_created_dict,
+    }
+
     context = {
         "environment_project_workflow_triplets": environment_projects_pairs_with_creating,
-        "available_project_environment_workflow_triplets": available_project_environment_workflow_triplets,
-        "workspace_project_environment_workflow_triplets_dict": sorted_environments_project_workflow_triplets_dict,
+        "workspace_project_environment_workflow_triplets_dict": sorted_environments_project_workflow_triplets_with_creating_dict,
         "billing_accounts_list": billing_accounts_list,
     }
 
     return render(
         request,
         "environment/research_environments.html",
         context,
@@ -367,13 +374,8 @@
     )
     finished = execution_state != Execution.State.ACTIVE
     if finished:
         services.mark_workflow_as_finished(
             execution_resource_name=execution_resource_name,
             execution_state=execution_state,
         )
-    # finished=True
-    # services.mark_workflow_as_finished(
-    #     execution_resource_name=execution_resource_name,
-    #     execution_state=None,
-    # )
     return JsonResponse({"finished": finished})
```

### Comparing `hdn-research-environment-2.0.1/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.0.2/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.0.1/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.0.2/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 environment/migrations/0003_cloudidentity_is_workspace_done.py
 environment/migrations/0004_auto_20220309_0330.py
 environment/migrations/0005_workflow.py
 environment/migrations/0006_delete_billingsetup.py
 environment/migrations/0007_billingaccountsharinginvite.py
 environment/migrations/0008_workflow_workspace_name.py
 environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
 environment/migrations/__init__.py
 environment/static/environment/css/create_research_environment.css
 environment/static/environment/css/environment-base.css
 environment/static/environment/css/manage_billing_account.css
 environment/static/environment/js/cookie.js
 environment/static/environment/js/gpu_disabling.js
 environment/static/environment/js/pricing_change.js
```

### Comparing `hdn-research-environment-2.0.1/setup.cfg` & `hdn-research-environment-2.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 2.0.1
+version = 2.0.2
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

