# Comparing `tmp/wedge-lib-3.1.0.tar.gz` & `tmp/wedge-lib-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wedge-lib-3.1.0.tar", last modified: Tue May 30 09:54:25 2023, max compression
+gzip compressed data, was "wedge-lib-3.1.1.tar", last modified: Wed May 31 15:21:43 2023, max compression
```

## Comparing `wedge-lib-3.1.0.tar` & `wedge-lib-3.1.1.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.517428 wedge-lib-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-30 09:54:25.517428 wedge-lib-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-30 09:54:25.517428 wedge-lib-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.501428 wedge-lib-3.1.0/w/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.501428 wedge-lib-3.1.0/w/data_test_factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/data_test_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/data_test_factory/data_test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.501428 wedge-lib-3.1.0/w/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.501428 wedge-lib-3.1.0/w/django/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/commands/abstract_maintenance_mode_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.501428 wedge-lib-3.1.0/w/django/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.501428 wedge-lib-3.1.0/w/django/services/business/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/services/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/services/business/user_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.501428 wedge-lib-3.1.0/w/django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/templatetags/util_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.501428 wedge-lib-3.1.0/w/django/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.501428 wedge-lib-3.1.0/w/django/tests/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/tests/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/tests/builders/user_test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/tests/django_testcase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.501428 wedge-lib-3.1.0/w/django/tests/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/tests/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/tests/factories/auth_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/tests/factories/reference_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/tests/view_testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/django/w_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.501428 wedge-lib-3.1.0/w/drf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.501428 wedge-lib-3.1.0/w/drf/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/decorators/group_required.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/exception_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/drf/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/jwt/jwt_authentication_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/jwt/jwt_viewset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/jwt/login_viewset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/drf/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/middlewares/maintenance_mode_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/drf/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/serializers/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/serializers/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/serializers/serpy_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/drf/sso/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/sso/sso_auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/sso/sso_user_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/drf/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/tests/api_testcase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/drf/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/tests/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/drf/tests/helpers/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/tests/helpers/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/tests/helpers/jwt/jwt_test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/drf/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/validators/drf_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/drf/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/mixins/dataclasses_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/mixins/thread_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/serializers/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/abstract_model_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/abstract_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/services/imports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/imports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.505428 wedge-lib-3.1.0/w/services/imports/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/imports/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/imports/models/import_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.509428 wedge-lib-3.1.0/w/services/technical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/abstract_import_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/boto3_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/cloudinary_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/context_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/csv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/date_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/db_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/dict_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/excel_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/filesystem_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/google_map_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/ip_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/json_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/key_generator_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/list_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/mail_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/maintenance_mode_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.509428 wedge-lib-3.1.0/w/services/technical/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/models/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/models/csv_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/models/request_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/models/request_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/models/sso.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/models/yousign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/pdf_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/sso_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/string_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/template_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/uniqid_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/url_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/yaml_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/services/technical/yousign_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.509428 wedge-lib-3.1.0/w/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.509428 wedge-lib-3.1.0/w/tests/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/builders/abstract_test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/builders/test_test_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.509428 wedge-lib-3.1.0/w/tests/drf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/drf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.509428 wedge-lib-3.1.0/w/tests/drf/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/drf/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/drf/middlewares/test_maintenance_mode_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/drf/test_model_service_viewset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/drf/test_viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.509428 wedge-lib-3.1.0/w/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.509428 wedge-lib-3.1.0/w/tests/fixtures/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.509428 wedge-lib-3.1.0/w/tests/fixtures/datasets/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/builders/builder_with_auto_now.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/builders/builder_with_internal_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/builders/builder_with_related_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/builders/factory_boy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/builders/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/builders/simple_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.513428 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/drf_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/dtf_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/dtf_recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/example_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/factory_boys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/serpy_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/simple_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.513428 wedge-lib-3.1.0/w/tests/fixtures/datasets/sso_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/sso_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/sso_service/create_sso_user_with_success_return_dict.json
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/sso_service/get_or_create_sso_user_with_success_return_dict.json
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/fixtures/datasets/sso_service/get_or_create_user_with_unknown_user_return_user.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.513428 wedge-lib-3.1.0/w/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/helpers/auth_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/helpers/cloudinary_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/helpers/date_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/helpers/google_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/helpers/orm_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/helpers/request_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/helpers/service_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/helpers/sso_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/helpers/yousign_test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.513428 wedge-lib-3.1.0/w/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/mixins/api_viewset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/mixins/boto3test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/mixins/factory_boy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/mixins/faker_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/mixins/serializer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/mixins/testcase_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.513428 wedge-lib-3.1.0/w/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/serializers/serpy_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/serializers/test_serpy_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.513428 wedge-lib-3.1.0/w/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.517428 wedge-lib-3.1.0/w/tests/services/technical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_abstract_import_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_boto3_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_cloudinary_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_context_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_csv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_date_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_dict_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_excel_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_filesystem_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_google_map_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_ip_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_json_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_key_generator_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_list_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_mail_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_maintenance_mode_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_pdf_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_sso_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_string_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_template_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_uniqid_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_url_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_yaml_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/technical/test_yousign_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/tests/services/test_abstract_model_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-30 09:52:15.000000 wedge-lib-3.1.0/w/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:54:25.517428 wedge-lib-3.1.0/wedge_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-30 09:54:25.000000 wedge-lib-3.1.0/wedge_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-30 09:54:25.000000 wedge-lib-3.1.0/wedge_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:54:25.000000 wedge-lib-3.1.0/wedge_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-30 09:54:25.000000 wedge-lib-3.1.0/wedge_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-30 09:54:25.000000 wedge-lib-3.1.0/wedge_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.619619 wedge-lib-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-31 15:21:43.619619 wedge-lib-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-31 15:21:43.619619 wedge-lib-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/data_test_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/data_test_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/data_test_factory/data_test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/django/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/commands/abstract_maintenance_mode_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/django/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/django/services/business/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/services/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/services/business/user_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/templatetags/util_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/django/tests/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/tests/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/tests/builders/user_test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/tests/django_testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/django/tests/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/tests/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/tests/factories/auth_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/tests/factories/reference_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/tests/view_testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/django/w_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/drf/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/decorators/group_required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/exception_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/drf/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/jwt/jwt_authentication_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/jwt/jwt_viewset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/jwt/login_viewset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/drf/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/middlewares/maintenance_mode_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/drf/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/serializers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/serializers/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/serializers/serpy_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/drf/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/sso/sso_auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/sso/sso_user_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/drf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/tests/api_testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.603619 wedge-lib-3.1.1/w/drf/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/tests/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.607619 wedge-lib-3.1.1/w/drf/tests/helpers/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/tests/helpers/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/tests/helpers/jwt/jwt_test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.607619 wedge-lib-3.1.1/w/drf/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/validators/drf_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/drf/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.607619 wedge-lib-3.1.1/w/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/mixins/dataclasses_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/mixins/thread_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.607619 wedge-lib-3.1.1/w/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/serializers/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.607619 wedge-lib-3.1.1/w/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/abstract_model_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/abstract_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.607619 wedge-lib-3.1.1/w/services/imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/imports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.607619 wedge-lib-3.1.1/w/services/imports/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/imports/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/imports/models/import_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.607619 wedge-lib-3.1.1/w/services/technical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/abstract_import_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/boto3_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/cloudinary_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/context_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/csv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/date_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/db_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/dict_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/excel_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/filesystem_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/google_map_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/ip_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/json_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/key_generator_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/list_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/mail_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/maintenance_mode_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.611619 wedge-lib-3.1.1/w/services/technical/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/models/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/models/csv_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/models/request_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/models/request_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/models/sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/models/yousign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/pdf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/sso_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/string_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/template_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/uniqid_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/url_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/yaml_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/services/technical/yousign_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.611619 wedge-lib-3.1.1/w/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.611619 wedge-lib-3.1.1/w/tests/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/builders/abstract_test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/builders/test_test_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.611619 wedge-lib-3.1.1/w/tests/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/drf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.611619 wedge-lib-3.1.1/w/tests/drf/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/drf/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/drf/middlewares/test_maintenance_mode_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/drf/test_model_service_viewset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/drf/test_viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.611619 wedge-lib-3.1.1/w/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.611619 wedge-lib-3.1.1/w/tests/fixtures/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.611619 wedge-lib-3.1.1/w/tests/fixtures/datasets/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/builders/builder_with_auto_now.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/builders/builder_with_internal_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/builders/builder_with_related_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/builders/factory_boy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/builders/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/builders/simple_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.611619 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/drf_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/dtf_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/dtf_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/example_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/factory_boys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/serpy_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/simple_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.611619 wedge-lib-3.1.1/w/tests/fixtures/datasets/sso_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/sso_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/sso_service/create_sso_user_with_success_return_dict.json
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/sso_service/get_or_create_sso_user_with_success_return_dict.json
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/fixtures/datasets/sso_service/get_or_create_user_with_unknown_user_return_user.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.615619 wedge-lib-3.1.1/w/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/helpers/auth_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/helpers/cloudinary_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/helpers/date_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/helpers/google_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/helpers/orm_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/helpers/request_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/helpers/service_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/helpers/sso_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/helpers/yousign_test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.615619 wedge-lib-3.1.1/w/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/mixins/api_viewset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/mixins/boto3test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/mixins/factory_boy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/mixins/faker_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/mixins/serializer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/mixins/testcase_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.615619 wedge-lib-3.1.1/w/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/serializers/serpy_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/serializers/test_serpy_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.615619 wedge-lib-3.1.1/w/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.619619 wedge-lib-3.1.1/w/tests/services/technical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_abstract_import_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_boto3_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_cloudinary_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_context_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_csv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_date_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_dict_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_excel_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_filesystem_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_google_map_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_ip_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_json_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_key_generator_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_list_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_mail_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_maintenance_mode_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_pdf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_sso_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_string_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_template_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_uniqid_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_url_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_yaml_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/technical/test_yousign_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/tests/services/test_abstract_model_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-31 15:19:38.000000 wedge-lib-3.1.1/w/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:21:43.619619 wedge-lib-3.1.1/wedge_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-31 15:21:43.000000 wedge-lib-3.1.1/wedge_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-31 15:21:43.000000 wedge-lib-3.1.1/wedge_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:21:43.000000 wedge-lib-3.1.1/wedge_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-31 15:21:43.000000 wedge-lib-3.1.1/wedge_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-31 15:21:43.000000 wedge-lib-3.1.1/wedge_lib.egg-info/top_level.txt
```

### Comparing `wedge-lib-3.1.0/LICENSE.txt` & `wedge-lib-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/PKG-INFO` & `wedge-lib-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedge-lib
-Version: 3.1.0
+Version: 3.1.1
 Summary: Wedge library for django application
 Home-page: https://github.com/Wedge-Digital/w
 Author-email: francois.schneider@wedge-digital.com
 License: MIT
 Description: # Wedge Library
         
         ## Démarrage rapide
```

### Comparing `wedge-lib-3.1.0/README.md` & `wedge-lib-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/setup.cfg` & `wedge-lib-3.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/setup.py` & `wedge-lib-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/data_test_factory/data_test_factory.py` & `wedge-lib-3.1.1/w/data_test_factory/data_test_factory.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/debug.py` & `wedge-lib-3.1.1/w/debug.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/django/commands/abstract_maintenance_mode_command.py` & `wedge-lib-3.1.1/w/django/commands/abstract_maintenance_mode_command.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/django/models.py` & `wedge-lib-3.1.1/w/django/models.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/django/services/business/user_service.py` & `wedge-lib-3.1.1/w/django/services/business/user_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/django/tests/django_testcase.py` & `wedge-lib-3.1.1/w/django/tests/django_testcase.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/django/tests/factories/auth_factories.py` & `wedge-lib-3.1.1/w/django/tests/factories/auth_factories.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/django/tests/view_testcase.py` & `wedge-lib-3.1.1/w/django/tests/view_testcase.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/django/utils.py` & `wedge-lib-3.1.1/w/django/utils.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/django/w_command.py` & `wedge-lib-3.1.1/w/django/w_command.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/decorators/group_required.py` & `wedge-lib-3.1.1/w/drf/decorators/group_required.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/exception_handler.py` & `wedge-lib-3.1.1/w/drf/exception_handler.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/jwt/jwt_authentication_backend.py` & `wedge-lib-3.1.1/w/drf/jwt/jwt_authentication_backend.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/jwt/jwt_viewset.py` & `wedge-lib-3.1.1/w/drf/jwt/jwt_viewset.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/jwt/login_viewset.py` & `wedge-lib-3.1.1/w/drf/jwt/login_viewset.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/middlewares/maintenance_mode_middleware.py` & `wedge-lib-3.1.1/w/drf/middlewares/maintenance_mode_middleware.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/mixins.py` & `wedge-lib-3.1.1/w/drf/mixins.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/serializers/fields.py` & `wedge-lib-3.1.1/w/drf/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/serializers/serpy_serializers.py` & `wedge-lib-3.1.1/w/drf/serializers/serpy_serializers.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/sso/sso_auth_backend.py` & `wedge-lib-3.1.1/w/drf/sso/sso_auth_backend.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/sso/sso_user_mixin.py` & `wedge-lib-3.1.1/w/drf/sso/sso_user_mixin.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/tests/api_testcase.py` & `wedge-lib-3.1.1/w/drf/tests/api_testcase.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/tests/helpers/jwt/jwt_test_helper.py` & `wedge-lib-3.1.1/w/drf/tests/helpers/jwt/jwt_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/drf/viewsets.py` & `wedge-lib-3.1.1/w/drf/viewsets.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/exceptions.py` & `wedge-lib-3.1.1/w/exceptions.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/serializers/serializer.py` & `wedge-lib-3.1.1/w/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/abstract_model_service.py` & `wedge-lib-3.1.1/w/services/abstract_model_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/abstract_service.py` & `wedge-lib-3.1.1/w/services/abstract_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/abstract_import_service.py` & `wedge-lib-3.1.1/w/services/technical/abstract_import_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/auth_service.py` & `wedge-lib-3.1.1/w/services/technical/auth_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/boto3_service.py` & `wedge-lib-3.1.1/w/services/technical/boto3_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,32 +14,31 @@
     _s3_resource: Session.resource = None
     _s3_client: Session.client = None
     _prefix_path = None
 
     @classmethod
     def init(cls):
         for key in [
-            "AWS_S3_ENDPOINT_URL",
             "AWS_ACCESS_KEY_ID",
             "AWS_SECRET_ACCESS_KEY",
             "AWS_STORAGE_BUCKET_NAME",
         ]:
             if not hasattr(settings, key) or not getattr(settings, key):
                 raise RuntimeError(f"Please set {key} in your settings")
 
         credentials = {
-            "endpoint_url": settings.AWS_S3_ENDPOINT_URL,
             "aws_access_key_id": settings.AWS_ACCESS_KEY_ID,
             "aws_secret_access_key": settings.AWS_SECRET_ACCESS_KEY,
             "region_name": settings.AWS_S3_REGION_NAME,
         }
-
+        if getattr(settings, "AWS_S3_ENDPOINT_URL", None):
+            credentials["endpoint_url"] = settings.AWS_S3_ENDPOINT_URL
         cls._s3_resource = Boto3Service._get_ressource(credentials)
         cls._s3_client = Boto3Service._get_client(credentials)
-        cls._prefix_path = settings.SANDBOX_PREFIX
+        cls._prefix_path = settings.BUCKET_PREFIX
 
     @classmethod
     def _get_client(cls, credentials):
         return boto3.client("s3", **credentials)
 
     @classmethod
     def _get_ressource(cls, credentials):
```

### Comparing `wedge-lib-3.1.0/w/services/technical/cloudinary_service.py` & `wedge-lib-3.1.1/w/services/technical/cloudinary_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/context_service.py` & `wedge-lib-3.1.1/w/services/technical/context_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/csv_service.py` & `wedge-lib-3.1.1/w/services/technical/csv_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/date_service.py` & `wedge-lib-3.1.1/w/services/technical/date_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/dict_service.py` & `wedge-lib-3.1.1/w/services/technical/dict_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/excel_service.py` & `wedge-lib-3.1.1/w/services/technical/excel_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/file_service.py` & `wedge-lib-3.1.1/w/services/technical/file_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/filesystem_service.py` & `wedge-lib-3.1.1/w/services/technical/filesystem_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/google_map_service.py` & `wedge-lib-3.1.1/w/services/technical/google_map_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/json_service.py` & `wedge-lib-3.1.1/w/services/technical/json_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/key_generator_service.py` & `wedge-lib-3.1.1/w/services/technical/key_generator_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/list_service.py` & `wedge-lib-3.1.1/w/services/technical/list_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/mail_service.py` & `wedge-lib-3.1.1/w/services/technical/mail_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/maintenance_mode_service.py` & `wedge-lib-3.1.1/w/services/technical/maintenance_mode_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/models/request_response.py` & `wedge-lib-3.1.1/w/services/technical/models/request_response.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/models/request_session.py` & `wedge-lib-3.1.1/w/services/technical/models/request_session.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/models/sso.py` & `wedge-lib-3.1.1/w/services/technical/models/sso.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/models/yousign.py` & `wedge-lib-3.1.1/w/services/technical/models/yousign.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/pdf_service.py` & `wedge-lib-3.1.1/w/services/technical/pdf_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/request_service.py` & `wedge-lib-3.1.1/w/services/technical/request_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/sso_service.py` & `wedge-lib-3.1.1/w/services/technical/sso_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/string_service.py` & `wedge-lib-3.1.1/w/services/technical/string_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/uniqid_service.py` & `wedge-lib-3.1.1/w/services/technical/uniqid_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/url_service.py` & `wedge-lib-3.1.1/w/services/technical/url_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/yaml_service.py` & `wedge-lib-3.1.1/w/services/technical/yaml_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/services/technical/yousign_service.py` & `wedge-lib-3.1.1/w/services/technical/yousign_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/builders/abstract_test_builder.py` & `wedge-lib-3.1.1/w/tests/builders/abstract_test_builder.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/builders/test_test_builder.py` & `wedge-lib-3.1.1/w/tests/builders/test_test_builder.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/drf/middlewares/test_maintenance_mode_middleware.py` & `wedge-lib-3.1.1/w/tests/drf/middlewares/test_maintenance_mode_middleware.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/drf/test_model_service_viewset.py` & `wedge-lib-3.1.1/w/tests/drf/test_model_service_viewset.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/drf/test_viewsets.py` & `wedge-lib-3.1.1/w/tests/drf/test_viewsets.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/fixtures/datasets/builders/builder_with_internal_dependencies.py` & `wedge-lib-3.1.1/w/tests/fixtures/datasets/builders/builder_with_internal_dependencies.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/fixtures/datasets/builders/builder_with_related_dependencies.py` & `wedge-lib-3.1.1/w/tests/fixtures/datasets/builders/builder_with_related_dependencies.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/fixtures/datasets/builders/factory_boy.py` & `wedge-lib-3.1.1/w/tests/fixtures/datasets/builders/factory_boy.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/fixtures/datasets/builders/models.py` & `wedge-lib-3.1.1/w/tests/fixtures/datasets/builders/models.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/drf_serializer.py` & `wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/drf_serializer.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/dtf_models.py` & `wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/dtf_models.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/dtf_recipes.py` & `wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/dtf_recipes.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/models.py` & `wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/models.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/serpy_serializer.py` & `wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/serpy_serializer.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/fixtures/datasets/django_app/viewsets.py` & `wedge-lib-3.1.1/w/tests/fixtures/datasets/django_app/viewsets.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/helpers/cloudinary_test_helper.py` & `wedge-lib-3.1.1/w/tests/helpers/cloudinary_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/helpers/google_test_helper.py` & `wedge-lib-3.1.1/w/tests/helpers/google_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/helpers/request_test_helper.py` & `wedge-lib-3.1.1/w/tests/helpers/request_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/helpers/service_test_helper.py` & `wedge-lib-3.1.1/w/tests/helpers/service_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/helpers/sso_test_helper.py` & `wedge-lib-3.1.1/w/tests/helpers/sso_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/helpers/yousign_test_helper.py` & `wedge-lib-3.1.1/w/tests/helpers/yousign_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/mixins/api_viewset_mixin.py` & `wedge-lib-3.1.1/w/tests/mixins/api_viewset_mixin.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/mixins/boto3test_mixin.py` & `wedge-lib-3.1.1/w/tests/mixins/boto3test_mixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from w.services.technical.boto3_service import Boto3Service
 
 
 class Boto3TestMixin:
     def setup_method(self, method):
         self.s3_mock = mock_s3()
         self.s3_mock.start()
-        Boto3Service._get_client = lambda x: boto3.client("s3")
-        Boto3Service._get_ressource = lambda x: boto3.resource("s3")
+        Boto3Service._get_client = lambda x: boto3.client("s3", region_name="us-east-1")
+        Boto3Service._get_ressource = lambda x: boto3.resource(
+            "s3",
+        )
         Boto3Service.init()
         self.mock_generate_signed_url = {
             "service": Boto3Service,
             "method_name": "generate_signed_url",
             "return_value": "https://bucket-name.s3.amazonaws.com/media/"
             "customers/2/2023/2023_01_recapitulatif_mensuel_2.pdf"
             "?AWSAccessKeyId=foobar_key"
```

### Comparing `wedge-lib-3.1.0/w/tests/mixins/factory_boy_mixin.py` & `wedge-lib-3.1.1/w/tests/mixins/factory_boy_mixin.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/mixins/testcase_mixin.py` & `wedge-lib-3.1.1/w/tests/mixins/testcase_mixin.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/serializers/serpy_serializers.py` & `wedge-lib-3.1.1/w/tests/serializers/serpy_serializers.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/serializers/test_serpy_serializer.py` & `wedge-lib-3.1.1/w/tests/serializers/test_serpy_serializer.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_abstract_import_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_abstract_import_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_auth_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_auth_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_boto3_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_boto3_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
     """
     init
     """
 
     def test_init_service_with_invalid_credentials_return_runtime_error(self):
         for key in [
-            "AWS_S3_ENDPOINT_URL",
             "AWS_ACCESS_KEY_ID",
             "AWS_SECRET_ACCESS_KEY",
+            "AWS_STORAGE_BUCKET_NAME",
         ]:
             new_setting = {key: None}
             with override_settings(**new_setting):
                 with pytest.raises(
                     RuntimeError, match=f"Please set {key} in your settings"
                 ):
                     Boto3Service.init()
```

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_cloudinary_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_cloudinary_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_context_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_context_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_csv_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_csv_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_date_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_date_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_dict_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_dict_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_excel_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_excel_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_file_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_file_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_filesystem_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_filesystem_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_google_map_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_google_map_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_ip_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_ip_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_json_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_json_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_key_generator_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_key_generator_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_list_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_list_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_mail_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_mail_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_maintenance_mode_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_maintenance_mode_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_pdf_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_pdf_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_request_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_request_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_sso_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_sso_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_string_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_string_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_template_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_template_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_uniqid_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_uniqid_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_url_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_url_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_yaml_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_yaml_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/technical/test_yousign_service.py` & `wedge-lib-3.1.1/w/tests/services/technical/test_yousign_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/tests/services/test_abstract_model_service.py` & `wedge-lib-3.1.1/w/tests/services/test_abstract_model_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/w/utils.py` & `wedge-lib-3.1.1/w/utils.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.0/wedge_lib.egg-info/PKG-INFO` & `wedge-lib-3.1.1/wedge_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedge-lib
-Version: 3.1.0
+Version: 3.1.1
 Summary: Wedge library for django application
 Home-page: https://github.com/Wedge-Digital/w
 Author-email: francois.schneider@wedge-digital.com
 License: MIT
 Description: # Wedge Library
         
         ## Démarrage rapide
```

### Comparing `wedge-lib-3.1.0/wedge_lib.egg-info/SOURCES.txt` & `wedge-lib-3.1.1/wedge_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

