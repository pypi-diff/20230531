# Comparing `tmp/weni_rp_apps-2.4.2a5.tar.gz` & `tmp/weni_rp_apps-2.4.2a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weni_rp_apps-2.4.2a5.tar", max compression
+gzip compressed data, was "weni_rp_apps-2.4.2a6.tar", max compression
```

## Comparing `weni_rp_apps-2.4.2a5.tar` & `weni_rp_apps-2.4.2a6.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0      646 2023-05-26 20:31:01.301231 weni_rp_apps-2.4.2a5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/activities/__init__.py
--rw-r--r--   0        0        0      231 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/activities/apps.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/activities/migrations/__init__.py
--rw-r--r--   0        0        0     1960 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/activities/signals.py
--rw-r--r--   0        0        0      366 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/activities/tasks.py
--rw-r--r--   0        0        0      325 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/analytics_api/README.md
--rw-r--r--   0        0        0       66 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/analytics_api/__init__.py
--rw-r--r--   0        0        0      264 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/analytics_api/apps.py
--rw-r--r--   0        0        0    13526 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/analytics_api/tests.py
--rw-r--r--   0        0        0      475 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/analytics_api/urls.py
--rw-r--r--   0        0        0     8909 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/analytics_api/views.py
--rw-r--r--   0        0        0       49 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/auth/__init__.py
--rw-r--r--   0        0        0      285 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/auth/apps.py
--rw-r--r--   0        0        0     1321 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/auth/backends.py
--rw-r--r--   0        0        0      430 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/auth/decorators.py
--rw-r--r--   0        0        0      733 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/auth/urls.py
--rw-r--r--   0        0        0     2645 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/auth/views.py
--rw-r--r--   0        0        0      309 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/channel_stats/README.md
--rw-r--r--   0        0        0       66 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/channel_stats/__init__.py
--rw-r--r--   0        0        0      264 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/channel_stats/apps.py
--rw-r--r--   0        0        0     6157 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/channel_stats/serializers.py
--rw-r--r--   0        0        0      317 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/channel_stats/urls.py
--rw-r--r--   0        0        0     3575 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/channel_stats/views.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/grpc/billing/__init__.py
--rw-r--r--   0        0        0      102 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/grpc/billing/apps.py
--rw-r--r--   0        0        0     3508 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/grpc/billing/queries.py
--rw-r--r--   0        0        0     3194 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/grpc/billing/serializers.py
--rw-r--r--   0        0        0     2072 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/grpc/billing/services.py
--rw-r--r--   0        0        0    11471 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/grpc/billing/tests.py
--rw-r--r--   0        0        0      231 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/grpc/billing/urls.py
--rw-r--r--   0        0        0       64 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/grpc/channel/__init__.py
--rw-r--r--   0        0        0      103 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/grpc/channel/apps.py
--rw-r--r--   0        0        0      352 2023-05-26 20:30:43.125041 weni_rp_apps-2.4.2a5/weni/grpc/channel/fields.py
--rw-r--r--   0        0        0     4110 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/channel/serializers.py
--rw-r--r--   0        0        0     4023 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/channel/services.py
--rw-r--r--   0        0        0     7747 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/channel/tests.py
--rw-r--r--   0        0        0      341 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/channel/urls.py
--rw-r--r--   0        0        0       70 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/classifier/__init__.py
--rw-r--r--   0        0        0      109 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/classifier/apps.py
--rw-r--r--   0        0        0     1262 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/classifier/serializers.py
--rw-r--r--   0        0        0     1175 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/classifier/services.py
--rw-r--r--   0        0        0     6460 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/classifier/tests.py
--rw-r--r--   0        0        0      249 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/classifier/urls.py
--rw-r--r--   0        0        0       61 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/core/__init__.py
--rw-r--r--   0        0        0      100 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/core/apps.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/core/management/commands/__init__.py
--rw-r--r--   0        0        0     1573 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/core/management/commands/grpc.py
--rw-r--r--   0        0        0     1213 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/core/serializers.py
--rw-r--r--   0        0        0      965 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/core/services.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/core/tests.py
--rw-r--r--   0        0        0      700 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/core/urls.py
--rw-r--r--   0        0        0       58 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/flow/__init__.py
--rw-r--r--   0        0        0       97 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/flow/apps.py
--rw-r--r--   0        0        0      307 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/flow/serializers.py
--rw-r--r--   0        0        0      658 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/flow/services.py
--rw-r--r--   0        0        0     2766 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/flow/tests.py
--rw-r--r--   0        0        0      213 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/flow/urls.py
--rw-r--r--   0        0        0       56 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/org/__init__.py
--rw-r--r--   0        0        0       95 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/org/apps.py
--rw-r--r--   0        0        0     2770 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/org/serializers.py
--rw-r--r--   0        0        0     3957 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/org/services.py
--rw-r--r--   0        0        0     9824 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/org/tests.py
--rw-r--r--   0        0        0      207 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/org/urls.py
--rw-r--r--   0        0        0       68 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/statistic/__init__.py
--rw-r--r--   0        0        0      107 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/statistic/apps.py
--rw-r--r--   0        0        0      672 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/statistic/services.py
--rw-r--r--   0        0        0     3134 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/statistic/tests.py
--rw-r--r--   0        0        0      252 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/statistic/urls.py
--rw-r--r--   0        0        0       58 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/user/__init__.py
--rw-r--r--   0        0        0       97 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/user/apps.py
--rw-r--r--   0        0        0      843 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/user/serializers.py
--rw-r--r--   0        0        0     3906 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/user/services.py
--rw-r--r--   0        0        0    10078 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/user/tests.py
--rw-r--r--   0        0        0      347 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/grpc/user/urls.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/__init__.py
--rw-r--r--   0        0        0      328 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/apps.py
--rw-r--r--   0        0        0      300 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/authenticators.py
--rw-r--r--   0        0        0     1374 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/backends.py
--rw-r--r--   0        0        0     5562 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/channel/serializers.py
--rw-r--r--   0        0        0    16222 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/channel/tests.py
--rw-r--r--   0        0        0      427 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/channel/urls.py
--rw-r--r--   0        0        0     7611 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/channel/views.py
--rw-r--r--   0        0        0     1433 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/classifier/serializers.py
--rw-r--r--   0        0        0     8525 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/classifier/tests.py
--rw-r--r--   0        0        0      351 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/classifier/urls.py
--rw-r--r--   0        0        0     3169 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/classifier/views.py
--rw-r--r--   0        0        0      107 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/clients/__init__.py
--rw-r--r--   0        0        0      696 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/clients/authenticators.py
--rw-r--r--   0        0        0      486 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/clients/base.py
--rw-r--r--   0        0        0      580 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/clients/connect.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/externals/__init__.py
--rw-r--r--   0        0        0     1308 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/externals/serializers.py
--rw-r--r--   0        0        0      294 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/externals/urls.py
--rw-r--r--   0        0        0     1501 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/externals/views.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/flows/__init__.py
--rw-r--r--   0        0        0     1278 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/flows/serializers.py
--rw-r--r--   0        0        0     4283 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/flows/tests.py
--rw-r--r--   0        0        0      308 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/flows/urls.py
--rw-r--r--   0        0        0      974 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/flows/views.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/globals/__init__.py
--rw-r--r--   0        0        0     2286 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/globals/serializers.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/globals/tests/__init__.py
--rw-r--r--   0        0        0     2183 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/globals/tests/test_serializers.py
--rw-r--r--   0        0        0      220 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/globals/urls.py
--rw-r--r--   0        0        0     1485 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/globals/views.py
--rw-r--r--   0        0        0      868 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/migrations/0001_initial.py
--rw-r--r--   0        0        0     1032 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/migrations/0002_project.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/migrations/__init__.py
--rw-r--r--   0        0        0      916 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/models.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/orgs/__init__.py
--rw-r--r--   0        0        0     3816 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/orgs/serializers.py
--rw-r--r--   0        0        0    14533 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/orgs/tests.py
--rw-r--r--   0        0        0      300 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/orgs/urls.py
--rw-r--r--   0        0        0     4579 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/orgs/views.py
--rw-r--r--   0        0        0      246 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/permissions.py
--rw-r--r--   0        0        0     1993 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/statistic/tests.py
--rw-r--r--   0        0        0      205 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/statistic/urls.py
--rw-r--r--   0        0        0      944 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/statistic/views.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/tests/__init__.py
--rw-r--r--   0        0        0     1249 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/tests/test_models.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/tickets/__init__.py
--rw-r--r--   0        0        0     1152 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/tickets/serializers.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/tickets/tests/__init__.py
--rw-r--r--   0        0        0     3398 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/tickets/tests/test_views.py
--rw-r--r--   0        0        0      443 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/tickets/urls.py
--rw-r--r--   0        0        0     1844 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/tickets/views.py
--rw-r--r--   0        0        0     1315 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/urls.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/users/__init__.py
--rw-r--r--   0        0        0      845 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/users/serializers.py
--rw-r--r--   0        0        0    11864 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/users/tests.py
--rw-r--r--   0        0        0      711 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/users/urls.py
--rw-r--r--   0        0        0     5758 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/users/views.py
--rw-r--r--   0        0        0      555 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/internal/views.py
--rw-r--r--   0        0        0       55 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/orgs_api/__init__.py
--rw-r--r--   0        0        0      253 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/orgs_api/apps.py
--rw-r--r--   0        0        0      906 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/orgs_api/serializers.py
--rw-r--r--   0        0        0     4030 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/orgs_api/tests.py
--rw-r--r--   0        0        0      178 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/orgs_api/urls.py
--rw-r--r--   0        0        0     1444 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/orgs_api/views.py
--rw-r--r--   0        0        0       45 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/s3/__init__.py
--rw-r--r--   0        0        0      243 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/s3/apps.py
--rw-r--r--   0        0        0      250 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/s3/urls.py
--rw-r--r--   0        0        0      550 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/s3/views.py
--rw-r--r--   0        0        0       79 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/serializers/__init__.py
--rw-r--r--   0        0        0      725 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/serializers/fields.py
--rw-r--r--   0        0        0      281 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/success_orgs/apps.py
--rw-r--r--   0        0        0     2403 2023-05-26 20:30:43.129041 weni_rp_apps-2.4.2a5/weni/success_orgs/business.py
--rw-r--r--   0        0        0      563 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/success_orgs/serializers.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/success_orgs/tests/__init__.py
--rw-r--r--   0        0        0     2980 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/success_orgs/tests/test_business.py
--rw-r--r--   0        0        0      494 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/success_orgs/urls.py
--rw-r--r--   0        0        0     2774 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/success_orgs/views.py
--rw-r--r--   0        0        0      318 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/template_message/README.md
--rw-r--r--   0        0        0       72 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/template_message/__init__.py
--rw-r--r--   0        0        0      294 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/template_message/apps.py
--rw-r--r--   0        0        0     2041 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/template_message/serializers.py
--rw-r--r--   0        0        0     5295 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/template_message/tests.py
--rw-r--r--   0        0        0      344 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/template_message/urls.py
--rw-r--r--   0        0        0     1651 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/template_message/views.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/templates/__init__.py
--rw-r--r--   0        0        0      559 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/templates/context_processors.py
--rw-r--r--   0        0        0      315 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/ticketer_queues/README.md
--rw-r--r--   0        0        0       70 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/ticketer_queues/__init__.py
--rw-r--r--   0        0        0      291 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/ticketer_queues/apps.py
--rw-r--r--   0        0        0      242 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/ticketer_queues/serializers.py
--rw-r--r--   0        0        0     1584 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/ticketer_queues/tests.py
--rw-r--r--   0        0        0      378 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/ticketer_queues/urls.py
--rw-r--r--   0        0        0      849 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/ticketer_queues/views.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/utils/__init__.py
--rw-r--r--   0        0        0     1091 2023-05-26 20:30:43.133041 weni_rp_apps-2.4.2a5/weni/utils/app_config.py
--rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.4.2a5/PKG-INFO
+-rw-r--r--   0        0        0      646 2023-05-30 15:39:35.012397 weni_rp_apps-2.4.2a6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/activities/__init__.py
+-rw-r--r--   0        0        0      245 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/activities/apps.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/activities/migrations/__init__.py
+-rw-r--r--   0        0        0     2096 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/activities/signals.py
+-rw-r--r--   0        0        0      366 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/activities/tasks.py
+-rw-r--r--   0        0        0      325 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/analytics_api/README.md
+-rw-r--r--   0        0        0       66 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/analytics_api/__init__.py
+-rw-r--r--   0        0        0      264 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/analytics_api/apps.py
+-rw-r--r--   0        0        0    13526 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/analytics_api/tests.py
+-rw-r--r--   0        0        0      535 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/analytics_api/urls.py
+-rw-r--r--   0        0        0     9016 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/analytics_api/views.py
+-rw-r--r--   0        0        0       49 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/auth/__init__.py
+-rw-r--r--   0        0        0      285 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/auth/apps.py
+-rw-r--r--   0        0        0     1321 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/auth/backends.py
+-rw-r--r--   0        0        0      430 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/auth/decorators.py
+-rw-r--r--   0        0        0      810 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/auth/urls.py
+-rw-r--r--   0        0        0     2645 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/auth/views.py
+-rw-r--r--   0        0        0      309 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/channel_stats/README.md
+-rw-r--r--   0        0        0       66 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/channel_stats/__init__.py
+-rw-r--r--   0        0        0      264 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/channel_stats/apps.py
+-rw-r--r--   0        0        0     6157 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/channel_stats/serializers.py
+-rw-r--r--   0        0        0      347 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/channel_stats/urls.py
+-rw-r--r--   0        0        0     3575 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/channel_stats/views.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/grpc/billing/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/grpc/billing/apps.py
+-rw-r--r--   0        0        0     3508 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/grpc/billing/queries.py
+-rw-r--r--   0        0        0     3194 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/grpc/billing/serializers.py
+-rw-r--r--   0        0        0     2063 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/grpc/billing/services.py
+-rw-r--r--   0        0        0    11364 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/grpc/billing/tests.py
+-rw-r--r--   0        0        0      231 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/grpc/billing/urls.py
+-rw-r--r--   0        0        0       64 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/grpc/channel/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/grpc/channel/apps.py
+-rw-r--r--   0        0        0      352 2023-05-30 15:39:17.288251 weni_rp_apps-2.4.2a6/weni/grpc/channel/fields.py
+-rw-r--r--   0        0        0     4070 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/channel/serializers.py
+-rw-r--r--   0        0        0     4081 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/channel/services.py
+-rw-r--r--   0        0        0     7987 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/channel/tests.py
+-rw-r--r--   0        0        0      341 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/channel/urls.py
+-rw-r--r--   0        0        0       70 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/classifier/__init__.py
+-rw-r--r--   0        0        0      109 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/classifier/apps.py
+-rw-r--r--   0        0        0     1356 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/classifier/serializers.py
+-rw-r--r--   0        0        0     1174 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/classifier/services.py
+-rw-r--r--   0        0        0     6493 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/classifier/tests.py
+-rw-r--r--   0        0        0      249 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/classifier/urls.py
+-rw-r--r--   0        0        0       61 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/core/__init__.py
+-rw-r--r--   0        0        0      100 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/core/apps.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     1588 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/core/management/commands/grpc.py
+-rw-r--r--   0        0        0     1213 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/core/serializers.py
+-rw-r--r--   0        0        0      965 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/core/services.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/core/tests.py
+-rw-r--r--   0        0        0      700 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/core/urls.py
+-rw-r--r--   0        0        0       58 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/flow/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/flow/apps.py
+-rw-r--r--   0        0        0      307 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/flow/serializers.py
+-rw-r--r--   0        0        0      680 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/flow/services.py
+-rw-r--r--   0        0        0     2764 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/flow/tests.py
+-rw-r--r--   0        0        0      213 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/flow/urls.py
+-rw-r--r--   0        0        0       56 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/org/__init__.py
+-rw-r--r--   0        0        0       95 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/org/apps.py
+-rw-r--r--   0        0        0     2836 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/org/serializers.py
+-rw-r--r--   0        0        0     4020 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/org/services.py
+-rw-r--r--   0        0        0     9821 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/org/tests.py
+-rw-r--r--   0        0        0      207 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/org/urls.py
+-rw-r--r--   0        0        0       68 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/statistic/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/statistic/apps.py
+-rw-r--r--   0        0        0      672 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/statistic/services.py
+-rw-r--r--   0        0        0     3132 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/statistic/tests.py
+-rw-r--r--   0        0        0      252 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/statistic/urls.py
+-rw-r--r--   0        0        0       58 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/user/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/user/apps.py
+-rw-r--r--   0        0        0      843 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/user/serializers.py
+-rw-r--r--   0        0        0     3916 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/user/services.py
+-rw-r--r--   0        0        0    10076 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/user/tests.py
+-rw-r--r--   0        0        0      347 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/grpc/user/urls.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/apps.py
+-rw-r--r--   0        0        0      300 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/authenticators.py
+-rw-r--r--   0        0        0     1374 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/backends.py
+-rw-r--r--   0        0        0     5484 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/channel/serializers.py
+-rw-r--r--   0        0        0    16305 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/channel/tests.py
+-rw-r--r--   0        0        0      394 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/channel/urls.py
+-rw-r--r--   0        0        0     7611 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/channel/views.py
+-rw-r--r--   0        0        0     1527 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/classifier/serializers.py
+-rw-r--r--   0        0        0     8626 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/classifier/tests.py
+-rw-r--r--   0        0        0      318 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/classifier/urls.py
+-rw-r--r--   0        0        0     2803 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/classifier/views.py
+-rw-r--r--   0        0        0      113 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/clients/__init__.py
+-rw-r--r--   0        0        0      692 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/clients/authenticators.py
+-rw-r--r--   0        0        0      486 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/clients/base.py
+-rw-r--r--   0        0        0      681 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/clients/connect.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/externals/__init__.py
+-rw-r--r--   0        0        0     1388 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/externals/serializers.py
+-rw-r--r--   0        0        0      294 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/externals/urls.py
+-rw-r--r--   0        0        0     1501 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/externals/views.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/flows/__init__.py
+-rw-r--r--   0        0        0     1278 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/flows/serializers.py
+-rw-r--r--   0        0        0     4318 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/flows/tests.py
+-rw-r--r--   0        0        0      308 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/flows/urls.py
+-rw-r--r--   0        0        0      974 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/flows/views.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/globals/__init__.py
+-rw-r--r--   0        0        0     2286 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/globals/serializers.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/globals/tests/__init__.py
+-rw-r--r--   0        0        0     2183 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/globals/tests/test_serializers.py
+-rw-r--r--   0        0        0      220 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/globals/urls.py
+-rw-r--r--   0        0        0     1484 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/globals/views.py
+-rw-r--r--   0        0        0     1247 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1032 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/migrations/0002_project.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/migrations/__init__.py
+-rw-r--r--   0        0        0      916 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/models.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/orgs/__init__.py
+-rw-r--r--   0        0        0     3976 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/orgs/serializers.py
+-rw-r--r--   0        0        0    14533 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/orgs/tests.py
+-rw-r--r--   0        0        0      300 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/orgs/urls.py
+-rw-r--r--   0        0        0     4592 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/orgs/views.py
+-rw-r--r--   0        0        0      246 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/permissions.py
+-rw-r--r--   0        0        0     1993 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/statistic/tests.py
+-rw-r--r--   0        0        0      205 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/statistic/urls.py
+-rw-r--r--   0        0        0      944 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/statistic/views.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/tests/__init__.py
+-rw-r--r--   0        0        0     1249 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/tests/test_models.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/tickets/__init__.py
+-rw-r--r--   0        0        0     1150 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/tickets/serializers.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/tickets/tests/__init__.py
+-rw-r--r--   0        0        0     3360 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/tickets/tests/test_views.py
+-rw-r--r--   0        0        0      443 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/tickets/urls.py
+-rw-r--r--   0        0        0     1844 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/tickets/views.py
+-rw-r--r--   0        0        0     1315 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/urls.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/users/__init__.py
+-rw-r--r--   0        0        0      845 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/users/serializers.py
+-rw-r--r--   0        0        0    12563 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/users/tests.py
+-rw-r--r--   0        0        0      711 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/users/urls.py
+-rw-r--r--   0        0        0     5849 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/users/views.py
+-rw-r--r--   0        0        0      555 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/internal/views.py
+-rw-r--r--   0        0        0       55 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/orgs_api/__init__.py
+-rw-r--r--   0        0        0      253 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/orgs_api/apps.py
+-rw-r--r--   0        0        0      906 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/orgs_api/serializers.py
+-rw-r--r--   0        0        0     4030 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/orgs_api/tests.py
+-rw-r--r--   0        0        0      178 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/orgs_api/urls.py
+-rw-r--r--   0        0        0     1444 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/orgs_api/views.py
+-rw-r--r--   0        0        0       45 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/s3/__init__.py
+-rw-r--r--   0        0        0      243 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/s3/apps.py
+-rw-r--r--   0        0        0      219 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/s3/urls.py
+-rw-r--r--   0        0        0      550 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/s3/views.py
+-rw-r--r--   0        0        0       93 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/serializers/__init__.py
+-rw-r--r--   0        0        0      725 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/serializers/fields.py
+-rw-r--r--   0        0        0      281 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/success_orgs/apps.py
+-rw-r--r--   0        0        0     2719 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/success_orgs/business.py
+-rw-r--r--   0        0        0      619 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/success_orgs/serializers.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/success_orgs/tests/__init__.py
+-rw-r--r--   0        0        0     3354 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/success_orgs/tests/test_business.py
+-rw-r--r--   0        0        0      494 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/success_orgs/urls.py
+-rw-r--r--   0        0        0     2770 2023-05-30 15:39:17.292251 weni_rp_apps-2.4.2a6/weni/success_orgs/views.py
+-rw-r--r--   0        0        0      318 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/template_message/README.md
+-rw-r--r--   0        0        0       72 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/template_message/__init__.py
+-rw-r--r--   0        0        0      294 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/template_message/apps.py
+-rw-r--r--   0        0        0     2040 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/template_message/serializers.py
+-rw-r--r--   0        0        0     5292 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/template_message/tests.py
+-rw-r--r--   0        0        0      344 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/template_message/urls.py
+-rw-r--r--   0        0        0     1651 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/template_message/views.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/templates/__init__.py
+-rw-r--r--   0        0        0      545 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/templates/context_processors.py
+-rw-r--r--   0        0        0      315 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/ticketer_queues/README.md
+-rw-r--r--   0        0        0       70 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/ticketer_queues/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/ticketer_queues/apps.py
+-rw-r--r--   0        0        0      242 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/ticketer_queues/serializers.py
+-rw-r--r--   0        0        0     1584 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/ticketer_queues/tests.py
+-rw-r--r--   0        0        0      378 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/ticketer_queues/urls.py
+-rw-r--r--   0        0        0      849 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/ticketer_queues/views.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/utils/__init__.py
+-rw-r--r--   0        0        0     1091 2023-05-30 15:39:17.296251 weni_rp_apps-2.4.2a6/weni/utils/app_config.py
+-rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.4.2a6/PKG-INFO
```

### Comparing `weni_rp_apps-2.4.2a5/pyproject.toml` & `weni_rp_apps-2.4.2a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weni-rp-apps"
-version = "2.4.2a5"
+version = "2.4.2a6"
 description = "Weni apps for Rapidpro Platform"
 authors = ["jcbalmeida"]
 license = "AGPL-3.0"
 packages = [
     { include = "weni" }
 ]
```

### Comparing `weni_rp_apps-2.4.2a5/weni/activities/signals.py` & `weni_rp_apps-2.4.2a6/weni/activities/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,44 +9,52 @@
 from temba.campaigns.models import Campaign
 
 
 def create_recent_activity(instance: models.Model, created: bool):
     if instance.is_active:
         action = "CREATE" if created else "UPDATE"
 
-        celery.execute.send_task("create_recent_activity", kwargs=dict(
-            action=action,
-            entity=instance.__class__.__name__.upper(),
-            entity_name=getattr(instance, "name", None),
-            user=instance.modified_by.email,
-            flow_organization=str(instance.org.uuid),
-        ))
+        celery.execute.send_task(
+            "create_recent_activity",
+            kwargs=dict(
+                action=action,
+                entity=instance.__class__.__name__.upper(),
+                entity_name=getattr(instance, "name", None),
+                user=instance.modified_by.email,
+                flow_organization=str(instance.org.uuid),
+            ),
+        )
 
 
 @receiver(post_save, sender=Channel)
 def channel_recent_activity_signal(sender, instance: Channel, created: bool, **kwargs):
     update_fields = kwargs.get("update_fields")
-    if instance.channel_type not in ['WA', 'WAC'] \
-        or update_fields != frozenset({'config',}):
+    if instance.channel_type not in ["WA", "WAC"] or update_fields != frozenset(
+        {
+            "config",
+        }
+    ):
         create_recent_activity(instance, created)
 
 
 @receiver(post_save, sender=Flow)
 def flow_recent_activity_signal(sender, instance: Flow, created: bool, **kwargs):
     update_fields = kwargs.get("update_fields")
-    if update_fields != frozenset({
-        'version_number',
-        'modified_on',
-        'saved_on',
-        'modified_by',
-        'metadata',
-        'saved_by',
-        'base_language',
-        'has_issues'
-    }):
+    if update_fields != frozenset(
+        {
+            "version_number",
+            "modified_on",
+            "saved_on",
+            "modified_by",
+            "metadata",
+            "saved_by",
+            "base_language",
+            "has_issues",
+        }
+    ):
         # This condition prevents two events from being sent when creating a flow
         create_recent_activity(instance, created)
 
 
 @receiver(post_save, sender=Trigger)
 def trigger_recent_activity_signal(sender, instance: Trigger, created: bool, **kwargs):
     create_recent_activity(instance, created)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/analytics_api/tests.py` & `weni_rp_apps-2.4.2a6/weni/analytics_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/analytics_api/views.py` & `weni_rp_apps-2.4.2a6/weni/analytics_api/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from django.db.models import Count, Prefetch, Q
 from django.urls import reverse
-from rest_framework.renderers import JSONRenderer
 from rest_framework.response import Response
 
 from temba.api.v2.views_base import BaseAPIView, ListAPIMixin
 from temba.contacts.models import Contact, ContactGroup
 from temba.flows.models import FlowRun
 from temba.utils import str_to_bool
 
@@ -107,16 +106,24 @@
     def get_read_explorer(cls):
         return {
             "method": "GET",
             "title": "List Contacts Analytics",
             "url": reverse("api.v2.analytics.contacts"),
             "slug": "contacts-analytics",
             "params": [
-                {"name": "group", "required": False, "help": "A group name or UUID to filter by. ex: Customers"},
-                {"name": "deleted", "required": False, "help": "Whether to return only deleted contacts. ex: false"},
+                {
+                    "name": "group",
+                    "required": False,
+                    "help": "A group name or UUID to filter by. ex: Customers",
+                },
+                {
+                    "name": "deleted",
+                    "required": False,
+                    "help": "Whether to return only deleted contacts. ex: false",
+                },
                 {
                     "name": "before",
                     "required": False,
                     "help": "Only return events created before this date, ex: 2015-01-28T18:00:00.000",
                 },
                 {
                     "name": "after",
@@ -129,15 +136,15 @@
 
 class FlowRunAnalyticsEndpoint(BaseAPIView, ListAPIMixin):
     """
     This endpoint shows the analytical data of the flow runs over a period of time.
 
     ## List Analytics Flow Runs data
 
-    A **GET** returns analytical data related to flows, containing information about the type 
+    A **GET** returns analytical data related to flows, containing information about the type
                 of runs and being able to segment by date
 
     * **flow_uuid** - A flow UUID to filter by, ex: f5901b62-ba76-4003-9c62-72fdacc1b7b7.
     * **before** - Only return events created before this date, ex: 2015-01-28T18:00:00.000
     * **after** - Only return events created after this date, ex: 2015-01-28T18:00:00.000
 
     Example:
```

### Comparing `weni_rp_apps-2.4.2a5/weni/auth/backends.py` & `weni_rp_apps-2.4.2a6/weni/auth/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/auth/urls.py` & `weni_rp_apps-2.4.2a6/weni/auth/urls.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,13 +7,23 @@
     OrgHomeRedirectView,
     FlowEditorRedirectView,
 )
 
 urlpatterns = [
     url(r"^oidc/", include("mozilla_django_oidc.urls")),
     path("check-user-legacy/<str:email>/", check_user_legacy, name="check-user-legacy"),
-    path("weni/<uuid:organization>/authenticate", WeniAuthenticationRequestView.as_view(), name="weni-authenticate",),
     path(
-        "weni/<uuid:organization>/flow/<uuid:uuid>/editor", FlowEditorRedirectView.as_view(), name="weni-flow-editor",
+        "weni/<uuid:organization>/authenticate",
+        WeniAuthenticationRequestView.as_view(),
+        name="weni-authenticate",
+    ),
+    path(
+        "weni/<uuid:organization>/flow/<uuid:uuid>/editor",
+        FlowEditorRedirectView.as_view(),
+        name="weni-flow-editor",
+    ),
+    path(
+        "weni/<uuid:organization>/config",
+        OrgHomeRedirectView.as_view(),
+        name="weni-org-home",
     ),
-    path("weni/<uuid:organization>/config", OrgHomeRedirectView.as_view(), name="weni-org-home"),
 ]
```

### Comparing `weni_rp_apps-2.4.2a5/weni/auth/views.py` & `weni_rp_apps-2.4.2a6/weni/auth/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/channel_stats/serializers.py` & `weni_rp_apps-2.4.2a6/weni/channel_stats/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/channel_stats/views.py` & `weni_rp_apps-2.4.2a6/weni/channel_stats/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/billing/queries.py` & `weni_rp_apps-2.4.2a6/weni/grpc/billing/queries.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/billing/serializers.py` & `weni_rp_apps-2.4.2a6/weni/grpc/billing/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/billing/services.py` & `weni_rp_apps-2.4.2a6/weni/grpc/billing/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     ActiveContactDetailSerializer,
     MsgDetailSerializer,
     MessageDetailRequestSerializer,
 )
 
 from google.protobuf import empty_pb2
 
-class BillingService(generics.GenericService):
 
+class BillingService(generics.GenericService):
     serializer_class = BillingRequestSerializer
 
     def Total(self, request, context):
         serializer = self.get_serializer(message=request)
         serializer.is_valid(raise_exception=True)
 
         org = serializer.validated_data["org"]
@@ -51,8 +51,7 @@
         msg = MessageDetailQuery.incoming_message(org_uuid, contact_uuid, before, after)
 
         if not msg:
             return empty_pb2.Empty()
 
         msg_serializer = MsgDetailSerializer(msg)
         return msg_serializer.message
-
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/billing/tests.py` & `weni_rp_apps-2.4.2a6/weni/grpc/billing/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 from django.conf import settings
 from django.test.testcases import TestCase
 from django.utils import timezone as tz
 from google.protobuf.timestamp_pb2 import Timestamp as TimestampMessage
 from rest_framework.exceptions import ErrorDetail
 from temba.orgs.models import Org
-from temba.msgs.models import Msg
 from django.contrib.auth.models import User
-from temba.contacts.models import Contact
 from temba.tests import TembaTest
 from weni.protobuf.flows import billing_pb2 as pb2, billing_pb2_grpc as stubs
 from weni.grpc.billing.queries import ActiveContactsQuery
-from weni.grpc.billing.serializers import BillingRequestSerializer, ActiveContactDetailSerializer
-from django_grpc_framework.test import FakeRpcError, RPCTransactionTestCase
+from weni.grpc.billing.serializers import (
+    BillingRequestSerializer,
+    ActiveContactDetailSerializer,
+)
+from django_grpc_framework.test import RPCTransactionTestCase
 from google.protobuf import empty_pb2
 
 
 class ActiveContactsQueryTest(TembaTest):
     def setUp(self):
         super().setUp()
         self.query = ActiveContactsQuery
@@ -228,52 +229,57 @@
     def test_detailed(self):
         ...
 
     def test_message_detail(self):
         user = User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
         org = Org.objects.create(name="Temba", timezone="Africa/Kigali", created_by=user, modified_by=user)
 
-        contact = self.create_contact(f"Contact 1", phone=f"+553124826922")
+        contact = self.create_contact(f'{"Contact 1"}', phone=f'{"+553124826922"}')
         contact.org = org
         contact.save(update_fields=["org"])
 
         channel = self.create_channel(channel_type="WA", name="channel_test", address="address_test", org=org)
 
         msg = self.create_incoming_msg(contact=contact, text="incoming message test", channel=channel)
-        msg1 = self.create_outgoing_msg(contact=contact, text="incoming message test", channel=channel)
 
         before = tz.now()
         after = tz.now() - tz.timedelta(minutes=1)
 
         result = self.billing_detail_msg(
-            org_uuid=str(org.uuid), contact_uuid=str(contact.uuid), before=str(before), after=str(after)
+            org_uuid=str(org.uuid),
+            contact_uuid=str(contact.uuid),
+            before=str(before),
+            after=str(after),
         )
 
         self.assertEqual(str(msg.uuid), result.uuid)
         self.assertEqual(msg.text, result.text)
         self.assertEqual(msg.direction, result.direction)
         self.assertEqual(channel.id, result.channel_id)
         self.assertEqual(channel.channel_type, result.channel_type)
 
     def test_message_detail_fail(self):
         user = User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
         org = Org.objects.create(name="Temba", timezone="Africa/Kigali", created_by=user, modified_by=user)
 
-        contact = self.create_contact(f"Contact 1", phone=f"+553124826922")
+        contact = self.create_contact("Contact 1", phone="+553124826922")
         contact.org = org
         contact.save(update_fields=["org"])
 
         channel = self.create_channel(channel_type="WA", name="channel_test", address="address_test", org=org)
 
-        msg = self.create_outgoing_msg(contact=contact, text="incoming message test", channel=channel, status="F")
+        self.create_outgoing_msg(contact=contact, text="incoming message test", channel=channel, status="F")
 
         before = tz.now()
         after = tz.now() - tz.timedelta(minutes=1)
 
         result = self.billing_detail_msg(
-            org_uuid=str(org.uuid), contact_uuid=str(contact.uuid), before=str(before), after=str(after)
+            org_uuid=str(org.uuid),
+            contact_uuid=str(contact.uuid),
+            before=str(before),
+            after=str(after),
         )
 
         self.assertEqual(type(result), empty_pb2.Empty)
 
     def billing_detail_msg(self, **kwargs):
         return self.stub.MessageDetail(pb2.MessageDetailRequest(**kwargs))
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/channel/serializers.py` & `weni_rp_apps-2.4.2a6/weni/grpc/channel/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,21 @@
 from temba.utils import analytics
 from weni.grpc.core import serializers as weni_serializers
 from weni.protobuf.flows import channel_pb2
 from weni.grpc.channel import fields
 
 
 class WeniWebChatProtoSerializer(proto_serializers.ProtoSerializer):
-
     org = weni_serializers.OrgUUIDRelatedField(write_only=True)
     user = weni_serializers.UserEmailRelatedField(write_only=True)
     name = serializers.CharField()
     base_url = serializers.URLField(validators=[URLValidator(), validate_external_url], write_only=True)
     uuid = serializers.UUIDField(read_only=True)
 
     def create(self, validated_data):
-        user = validated_data["user"]
         name = validated_data["name"]
 
         config = {CONFIG_BASE_URL: validated_data["base_url"]}
 
         return Channel.create(
             validated_data["org"],
             validated_data["user"],
@@ -42,15 +40,14 @@
 
     class Meta:
         proto_class = channel_pb2.WeniWebChat
         fields = ["user", "name", "base_url", "uuid"]
 
 
 class ChannelProtoSerializer(proto_serializers.ModelProtoSerializer):
-
     user = weni_serializers.UserEmailRelatedField(write_only=True, required=True)
     config = serializers.SerializerMethodField()
     org = serializers.SerializerMethodField()
 
     def get_config(self, instance):
         return json.dumps(instance.config)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/channel/services.py` & `weni_rp_apps-2.4.2a6/weni/grpc/channel/services.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import json
 import re
 
-from django.http import Http404, HttpResponseBadRequest
+from django.http import Http404
 from django.http.response import HttpResponseRedirect
 from django.shortcuts import get_object_or_404
 from django.contrib.sessions.middleware import SessionMiddleware
 from django.contrib.messages.middleware import MessageMiddleware
 from django.contrib.auth.models import User
 from django_grpc_framework import generics, mixins
 from django.test import RequestFactory
 import grpc
 
 from temba.channels.types.weniwebchat.type import WeniWebChatType
 from temba.channels.models import Channel
 from temba.orgs.models import Org
 from temba.channels.types import TYPES
 
-from weni.grpc.channel.serializers import WeniWebChatProtoSerializer, ChannelProtoSerializer, ChannelWACSerializer
+from weni.grpc.channel.serializers import (
+    WeniWebChatProtoSerializer,
+    ChannelProtoSerializer,
+    ChannelWACSerializer,
+)
 from weni.protobuf.flows import channel_pb2
 
 
 # this class will be deprecated
 class WeniWebChatService(mixins.CreateModelMixin, mixins.DestroyModelMixin, generics.GenericService):
-
     channel_type = WeniWebChatType
     serializer_class = WeniWebChatProtoSerializer
 
 
 class ChannelService(
-    mixins.RetrieveModelMixin, mixins.ListModelMixin, mixins.DestroyModelMixin, generics.GenericService
+    mixins.RetrieveModelMixin,
+    mixins.ListModelMixin,
+    mixins.DestroyModelMixin,
+    generics.GenericService,
 ):
-
     queryset = Channel.objects
     lookup_field = "uuid"
     serializer_class = ChannelProtoSerializer
 
     def filter_queryset(self, queryset):
         request = self.request
 
@@ -82,23 +87,27 @@
         url = self.create_channel(user, org, data, channel_type)
 
         if url is None:
             self.context.abort(grpc.StatusCode.INVALID_ARGUMENT, "Bad Request")
 
         if "/users/login/?next=" in url:
             self.context.abort(
-                grpc.StatusCode.INVALID_ARGUMENT, f"User: {user.email} do not have permission in Org: {org.uuid}"
+                grpc.StatusCode.INVALID_ARGUMENT,
+                f"User: {user.email} do not have permission in Org: {org.uuid}",
             )
 
         regex = "[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}"
         channe_uuid = re.findall(regex, url)[0]
         channel = Channel.objects.get(uuid=channe_uuid)
 
         return channel_pb2.Channel(
-            uuid=channe_uuid, name=channel.name, address=channel.address, config=json.dumps(channel.config)
+            uuid=channe_uuid,
+            name=channel.name,
+            address=channel.address,
+            config=json.dumps(channel.config),
         )
 
     def create_channel(self, user: User, org: Org, data: dict, channel_type) -> str:
         factory = RequestFactory()
         url = f"channels/types/{channel_type.slug}/claim"
 
         request = factory.post(url, data)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/channel/tests.py` & `weni_rp_apps-2.4.2a6/weni/grpc/channel/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from django.contrib.auth import get_user_model
 from django_grpc_framework.test import RPCTransactionTestCase
 from rest_framework import serializers
 
 from temba.channels.models import Channel
 from temba.orgs.models import Org, OrgRole
-from temba.channels.types.weniwebchat.type import CONFIG_BASE_URL
 from weni.protobuf.flows import channel_pb2, channel_pb2_grpc
 
 
 User = get_user_model()
 
 
 class gRPCClient:
@@ -36,15 +35,18 @@
         return stub.List(channel_pb2.ChannelListRequest(**kwargs))
 
 
 class ReleaseChannelServiceTest(gRPCClient, RPCTransactionTestCase):
     def setUp(self):
         self.user = User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
         self.org = Org.objects.create(
-            name="Weni", timezone="Africa/Kigali", created_by=self.user, modified_by=self.user
+            name="Weni",
+            timezone="Africa/Kigali",
+            created_by=self.user,
+            modified_by=self.user,
         )
 
         super().setUp()
 
         self.channel_obj = Channel.create(self.org, self.user, None, "WWC", "Test WWC")
 
     def test_released_channel_is_active_equal_to_false(self):
@@ -52,15 +54,18 @@
         self.assertFalse(Channel.objects.get(id=self.channel_obj.id).is_active)
 
 
 class CreateWACServiceTest(gRPCClient, RPCTransactionTestCase):
     def setUp(self):
         self.user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
         self.org = Org.objects.create(
-            name="Weni", timezone="America/Sao_Paulo", created_by=self.user, modified_by=self.user
+            name="Weni",
+            timezone="America/Sao_Paulo",
+            created_by=self.user,
+            modified_by=self.user,
         )
         self.org.add_user(self.user, OrgRole.ADMINISTRATOR)
 
         self.config = {
             "wa_number": "5561995743921",
             "wa_verified_name": "Weni Test",
             "wa_waba_id": "2433443436435435",
@@ -111,26 +116,31 @@
             )
 
 
 class CreateChannelServiceTest(gRPCClient, RPCTransactionTestCase):
     def setUp(self):
         self.user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
         self.org = Org.objects.create(
-            name="Weni", timezone="America/Sao_Paulo", created_by=self.user, modified_by=self.user
+            name="Weni",
+            timezone="America/Sao_Paulo",
+            created_by=self.user,
+            modified_by=self.user,
         )
         self.org.add_user(self.user, OrgRole.ADMINISTRATOR)
 
         super().setUp()
 
     def test_create_weni_web_chat_channel(self):
-
         data = json.dumps({"name": "test", "base_url": "https://weni.ai"})
 
         response = self.channel_create_request(
-            user=self.user.email, org=str(self.org.uuid), data=data, channeltype_code="WWC"
+            user=self.user.email,
+            org=str(self.org.uuid),
+            data=data,
+            channeltype_code="WWC",
         )
         channel = Channel.objects.get(uuid=response.uuid)
         self.assertEqual(channel.address, response.address)
         self.assertEqual(channel.name, response.name)
         self.assertEqual(channel.config.get("base_url"), "https://weni.ai")
         self.assertEqual(channel.org, self.org)
         self.assertEqual(channel.created_by, self.user)
@@ -138,36 +148,48 @@
         self.assertEqual(channel.channel_type, "WWC")
 
 
 class RetrieveChannelServiceTest(gRPCClient, RPCTransactionTestCase):
     def setUp(self):
         self.user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
         self.org = Org.objects.create(
-            name="Weni", timezone="America/Sao_Paulo", created_by=self.user, modified_by=self.user
+            name="Weni",
+            timezone="America/Sao_Paulo",
+            created_by=self.user,
+            modified_by=self.user,
         )
 
         super().setUp()
 
         self.channel_obj = Channel.create(
-            self.org, self.user, None, "WWC", "Test WWC", "test", {"fake_key": "fake_value"}
+            self.org,
+            self.user,
+            None,
+            "WWC",
+            "Test WWC",
+            "test",
+            {"fake_key": "fake_value"},
         )
 
     def test_channel_retrieve_returned_fields(self):
         response = self.channel_retrieve_request(uuid=str(self.channel_obj.uuid))
         self.assertEqual(response.name, self.channel_obj.name)
         self.assertEqual(response.address, self.channel_obj.address)
         self.assertEqual(json.loads(response.config), self.channel_obj.config)
 
 
 class ListChannelServiceTest(gRPCClient, RPCTransactionTestCase):
     def setUp(self):
         self.user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
         self.orgs = [
             Org.objects.create(
-                name=f"Org {org}", timezone="America/Sao_Paulo", created_by=self.user, modified_by=self.user
+                name=f"Org {org}",
+                timezone="America/Sao_Paulo",
+                created_by=self.user,
+                modified_by=self.user,
             )
             for org in range(2)
         ]
 
         for channel in range(6):
             Channel.create(
                 self.orgs[0] if channel % 2 == 0 else self.orgs[1],
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/classifier/serializers.py` & `weni_rp_apps-2.4.2a6/weni/grpc/classifier/serializers.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from temba.classifiers.models import Classifier
 from weni.protobuf.flows import classifier_pb2
 from weni.grpc.core import serializers as weni_serializers
 
 
 class ClassifierProtoSerializer(proto_serializers.ModelProtoSerializer):
-
     uuid = serializers.UUIDField(read_only=True)
     is_active = serializers.BooleanField(read_only=True)
     classifier_type = serializers.CharField(required=True)
     name = serializers.CharField(required=True)
     access_token = weni_serializers.SerializerMethodCharField(required=True)
     user = weni_serializers.UserEmailRelatedField(write_only=True)
     org = weni_serializers.OrgUUIDRelatedField(write_only=True)
@@ -24,8 +23,16 @@
         validated_data.pop("access_token")
 
         return Classifier.create(config=config, **validated_data)
 
     class Meta:
         model = Classifier
         proto_class = classifier_pb2.Classifier
-        fields = ["uuid", "is_active", "classifier_type", "name", "access_token", "org", "user"]
+        fields = [
+            "uuid",
+            "is_active",
+            "classifier_type",
+            "name",
+            "access_token",
+            "org",
+            "user",
+        ]
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/classifier/services.py` & `weni_rp_apps-2.4.2a6/weni/grpc/classifier/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 class ClassifierService(
     mixins.CreateModelMixin,
     mixins.RetrieveModelMixin,
     mixins.DestroyModelMixin,
     generics.GenericService,
     AbstractService,
 ):
-
     serializer_class = ClassifierProtoSerializer
     queryset = Classifier.objects.all()
     lookup_field = "uuid"
 
     def List(self, request, context):
         org = self.get_org_object(request.org_uuid, "uuid")
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/classifier/tests.py` & `weni_rp_apps-2.4.2a6/weni/grpc/classifier/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,38 +10,42 @@
 
 
 def get_test_classifier(test: grpc_test.RPCTransactionTestCase) -> Classifier:
     """
     creates a new classifier object containing an intention and returns it.
     """
     response = test.classifier_create_request(
-            classifier_type="Test Type",
-            user=test.admin.email,
-            org=str(test.org.uuid),
-            name="Test Name",
-            access_token=test.config["access_token"]
-        )
+        classifier_type="Test Type",
+        user=test.admin.email,
+        org=str(test.org.uuid),
+        name="Test Name",
+        access_token=test.config["access_token"],
+    )
 
     classifier = Classifier.objects.get(uuid=response.uuid)
 
     Intent.objects.create(classifier=classifier, name="Test Intent", external_id="FakeExternal")
 
     return classifier
 
 
 class BaseClassifierServiceTest(grpc_test.RPCTransactionTestCase):
-
     def setUp(self):
         self.config = {"access_token": "hbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9"}
 
         self.admin = User.objects.create_user(
             username="testuser", password="123", email="test@weni.ai", is_superuser=True
         )
 
-        self.org = Org.objects.create(name="Weni", timezone="America/Maceio", created_by=self.admin, modified_by=self.admin)
+        self.org = Org.objects.create(
+            name="Weni",
+            timezone="America/Maceio",
+            created_by=self.admin,
+            modified_by=self.admin,
+        )
 
         super().setUp()
 
         self.stub = classifier_pb2_grpc.ClassifierControllerStub(self.channel)
 
     def classifier_list_request(self, **kwargs):
         return self.stub.List(classifier_pb2.ClassifierListRequest(**kwargs))
@@ -53,15 +57,14 @@
         return self.stub.Retrieve(classifier_pb2.ClassifierRetrieveRequest(**kwargs))
 
     def classifier_destroy_request(self, **kwargs):
         return self.stub.Destroy(classifier_pb2.ClassifierDestroyRequest(**kwargs))
 
 
 class ClassifierServiceTest(BaseClassifierServiceTest):
-
     def test_list_classifier(self):
         org = Org.objects.first()
         org_uuid = str(org.uuid)
 
         classifier = Classifier.create(org, self.admin, WitType.slug, "Booker", self.config, sync=False)
 
         response = self.classifier_list_request(org_uuid=org_uuid, is_active=True)
@@ -123,24 +126,23 @@
         classifier_type = "Test Type"
 
         response = self.classifier_create_request(
             classifier_type=classifier_type,
             user=user.email,
             org=str(org.uuid),
             name=name,
-            access_token=access_token
+            access_token=access_token,
         )
 
         self.assertEqual(response.name, name)
         self.assertEqual(response.classifier_type, classifier_type)
         self.assertEqual(response.access_token, access_token)
 
 
 class ClassifierServiceRetrieveTest(BaseClassifierServiceTest):
-
     def test_retrieve_classifier_by_valid_uuid(self):
         classifier = get_test_classifier(self)
         response = self.classifier_retrieve_request(uuid=str(classifier.uuid))
 
         self.assertEqual(classifier.classifier_type, response.classifier_type)
         self.assertEqual(classifier.name, response.name)
         self.assertEqual(classifier.config["access_token"], response.access_token)
@@ -150,15 +152,14 @@
         invalid_uuid = "wrong-wrong-wrong-wrong"
 
         with self.assertRaises(grpc_test.FakeRpcError):
             self.classifier_retrieve_request(uuid=invalid_uuid)
 
 
 class ClassifierServiceDestroyTest(BaseClassifierServiceTest):
-
     def test_destroy_classifier_by_valid_uuid(self):
         classifier = get_test_classifier(self)
         self.assertEqual(classifier.intents.count(), 1)
 
         self.classifier_destroy_request(uuid=str(classifier.uuid), user_email=self.admin.email)
 
         classifier = Classifier.objects.get(uuid=classifier.uuid)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/core/management/commands/grpc.py` & `weni_rp_apps-2.4.2a6/weni/grpc/core/management/commands/grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from concurrent import futures
 
 import grpc
-from django_grpc_framework.management.commands.grpcrunserver import \
-    Command as BaseCommand
+from django_grpc_framework.management.commands.grpcrunserver import (
+    Command as BaseCommand,
+)
 from django_grpc_framework.settings import grpc_settings
 
 
 class Command(BaseCommand):
     help = "Start a grpc server with optional credentials."
 
     def add_arguments(self, parser):
@@ -17,15 +18,16 @@
     def handle(self, *args, **options):
         self.server_key = options["server_key"]
         self.server_crt = options["server_crt"]
         super().handle(*args, **options)
 
     def _serve(self):
         server = grpc.server(
-            futures.ThreadPoolExecutor(max_workers=self.max_workers), interceptors=grpc_settings.SERVER_INTERCEPTORS,
+            futures.ThreadPoolExecutor(max_workers=self.max_workers),
+            interceptors=grpc_settings.SERVER_INTERCEPTORS,
         )
         grpc_settings.ROOT_HANDLERS_HOOK(server)
 
         if self.server_crt and self.server_key:
             # read in key and certificate
             private_key = open(self.server_key, "rb").read()
             certificate_chain = open(self.server_crt, "rb").read()
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/core/serializers.py` & `weni_rp_apps-2.4.2a6/weni/grpc/core/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,14 @@
     def __init__(self, method_name=None, **kwargs):
         self.method_name = method_name
         super().__init__(**kwargs)
 
     def bind(self, field_name, parent):
         # The method name defaults to `get_{field_name}`.
         if self.method_name is None:
-            self.method_name = 'get_{field_name}'.format(field_name=field_name)
+            self.method_name = "get_{field_name}".format(field_name=field_name)
 
         super().bind(field_name, parent)
 
     def get_attribute(self, instance):
         method = getattr(self.parent, self.method_name)
         return method(instance)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/core/services.py` & `weni_rp_apps-2.4.2a6/weni/grpc/core/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,21 +10,20 @@
     def get_user_object(self, value, query_parameter: str = "pk"):
         return self._get_object(User, value, query_parameter)
 
     def get_org_object(self, value, query_parameter: str = "pk") -> Org:
         return self._get_object(Org, value, query_parameter)
 
     def _get_object(self, model, value, query_parameter: str):
-
         query = {query_parameter: value}
 
         try:
             return model.objects.get(**query)
         except model.DoesNotExist:
             self.raises_not_fount(model.__name__, value)
         except exceptions.ValidationError:
             self.raises_not_fount(model.__name__, value)
 
     def raises_not_fount(self, model_name, value):
         if not value:
             value = "None"
-        self.context.abort(grpc.StatusCode.NOT_FOUND, f"{model_name}: {value} not found!")
+        self.context.abort(grpc.StatusCode.NOT_FOUND, f"{model_name}: {value} not found!")
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/core/urls.py` & `weni_rp_apps-2.4.2a6/weni/grpc/core/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/flow/services.py` & `weni_rp_apps-2.4.2a6/weni/grpc/flow/services.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,12 +8,14 @@
 class FlowService(generics.GenericService, AbstractService):
     def List(self, request, _):
         org = self.get_org_object(request.org_uuid, "uuid")
         queryset = Flow.objects.filter(
             name__icontains=request.flow_name,
             org=org.id,
             is_active=True,
-        ).exclude(is_archived=True)[:20]
+        ).exclude(
+            is_archived=True
+        )[:20]
 
         serializer = FlowProtoSerializer(queryset, many=True)
         for message in serializer.message:
             yield message
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/flow/tests.py` & `weni_rp_apps-2.4.2a6/weni/grpc/flow/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from temba.flows.models import Flow
 
 from weni.protobuf.flows import flow_pb2, flow_pb2_grpc
 
 
 class FlowServiceTest(RPCTransactionTestCase):
     def setUp(self):
-
         User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
 
         user = User.objects.first()
 
         temba = Org.objects.create(name="Temba", timezone="America/Maceio", created_by=user, modified_by=user)
         weni = Org.objects.create(name="Weni", timezone="America/Maceio", created_by=user, modified_by=user)
 
@@ -23,15 +22,14 @@
         Flow.create(name="Test Weni flow name", user=user, org=weni)
 
         super().setUp()
 
         self.stub = flow_pb2_grpc.FlowControllerStub(self.channel)
 
     def test_list_flow(self):
-
         temba = Org.objects.get(name="Temba")
         weni = Org.objects.get(name="Weni")
 
         with self.assertRaisesMessage(FakeRpcError, "Org: 123 not found!"):
             for flow in self.flow_list_request(flow_name="test", org_uuid="123"):
                 ...
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/org/serializers.py` & `weni_rp_apps-2.4.2a6/weni/grpc/org/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
         try:
             return model.objects.get(pk=pk)
         except model.DoesNotExist:
             raise proto_serializers.ValidationError(f"{model.__name__}: {pk} not found!")
 
 
 class OrgProtoSerializer(proto_serializers.ModelProtoSerializer):
-
     users = serializers.SerializerMethodField()
     timezone = serializers.CharField()
 
     def set_user_permission(self, user: dict, permission: str) -> dict:
         user["permission_type"] = permission
         return user
 
@@ -28,15 +27,20 @@
         values = ["id", "email", "username", "first_name", "last_name"]
 
         administrators = list(org.administrators.all().values(*values))
         viewers = list(org.viewers.all().values(*values))
         editors = list(org.editors.all().values(*values))
         surveyors = list(org.surveyors.all().values(*values))
 
-        administrators = list(map(lambda user: self.set_user_permission(user, "administrator"), administrators))
+        administrators = list(
+            map(
+                lambda user: self.set_user_permission(user, "administrator"),
+                administrators,
+            )
+        )
         viewers = list(map(lambda user: self.set_user_permission(user, "viewer"), viewers))
         editors = list(map(lambda user: self.set_user_permission(user, "editor"), editors))
         surveyors = list(map(lambda user: self.set_user_permission(user, "surveyor"), surveyors))
 
         users = administrators + viewers + editors + surveyors
 
         return users
@@ -44,25 +48,23 @@
     class Meta:
         model = Org
         proto_class = org_pb2.Org
         fields = ["id", "name", "uuid", "timezone", "date_format", "users"]
 
 
 class OrgCreateProtoSerializer(proto_serializers.ModelProtoSerializer):
-
     user_email = serializers.EmailField()
 
     class Meta:
         model = Org
         proto_class = org_pb2.Org
         fields = ["name", "timezone", "user_email"]
 
 
 class OrgUpdateProtoSerializer(proto_serializers.ModelProtoSerializer):
-
     uuid = serializers.CharField()
     modified_by = weni_serializers.UserEmailRelatedField(required=False, write_only=True)
     timezone = serializers.CharField(required=False)
     name = serializers.CharField(required=False)
     plan_end = serializers.DateTimeField(required=False)
 
     class Meta:
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/org/services.py` & `weni_rp_apps-2.4.2a6/weni/grpc/org/services.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 import grpc
 from django.contrib.auth.models import User
 from django.conf import settings
 from django_grpc_framework import generics, mixins
 from google.protobuf import empty_pb2
 
 from temba.orgs.models import Org
-from weni.grpc.org.serializers import OrgCreateProtoSerializer, OrgProtoSerializer, OrgUpdateProtoSerializer
+from weni.grpc.org.serializers import (
+    OrgCreateProtoSerializer,
+    OrgProtoSerializer,
+    OrgUpdateProtoSerializer,
+)
 from weni.grpc.core.services import AbstractService
 
 
 class OrgService(AbstractService, generics.GenericService, mixins.ListModelMixin):
-
     queryset = Org.objects
     lookup_field = "uuid"
 
     def List(self, request, context):
-
         user = self.get_user(request)
         orgs = self.get_orgs(user)
 
         serializer = OrgProtoSerializer(orgs, many=True)
 
         for msg in serializer.message:
             yield msg
 
     def Create(self, request, context):
-
         serializer = OrgCreateProtoSerializer(message=request)
         serializer.is_valid(raise_exception=True)
 
         user, created = User.objects.get_or_create(email=request.user_email, defaults={"username": request.user_email})
 
         org = Org.objects.create(
-            name=request.name, timezone=request.timezone, created_by=user, modified_by=user, plan="infinity"
+            name=request.name,
+            timezone=request.timezone,
+            created_by=user,
+            modified_by=user,
+            plan="infinity",
         )
 
         org.administrators.add(user)
         org.initialize()
 
         org_serializer = OrgProtoSerializer(org)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/org/tests.py` & `weni_rp_apps-2.4.2a6/weni/grpc/org/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 
 from temba.orgs.models import Org
 from weni.protobuf.flows import org_pb2, org_pb2_grpc
 from weni.grpc.org.serializers import SerializerUtils
 
 
 class OrgServiceTest(RPCTransactionTestCase):
-
     WRONG_ID = -1
     WRONG_UUID = "31313-dasda-dasdasd-23123"
     WRONG_EMAIL = "wrong@email.com"
 
     def setUp(self):
-
         User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
         User.objects.create_user(username="weniuser", password="123", email="wene@user.com")
 
         user = User.objects.get(username="testuser")
 
         Org.objects.create(name="Temba", timezone="Africa/Kigali", created_by=user, modified_by=user)
         Org.objects.create(name="Weni", timezone="Africa/Kigali", created_by=user, modified_by=user)
@@ -37,15 +35,14 @@
 
         with self.assertRaisesMessage(ValidationError, (f"User: {self.WRONG_ID} not found!")):
             SerializerUtils.get_object(User, self.WRONG_ID)
 
         self.assertEquals(user, SerializerUtils.get_object(User, user.pk))
 
     def test_list_orgs(self):
-
         with self.assertRaises(FakeRpcError):
             for org in self.stub_org_list_request():
                 ...
 
         with self.assertRaises(FakeRpcError):
             for org in self.stub_org_list_request(user_email="wrong@email.com"):
                 ...
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/statistic/services.py` & `weni_rp_apps-2.4.2a6/weni/grpc/statistic/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/statistic/tests.py` & `weni_rp_apps-2.4.2a6/weni/grpc/statistic/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from temba.utils.management.commands.test_db import DisableTriggersOn
 
 from weni.protobuf.flows import statistic_pb2, statistic_pb2_grpc
 
 
 class OrgStatisticServiceTest(test_grpc.RPCTransactionTestCase):
     def setUp(self):
-
         User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
         user = User.objects.get(username="testuser")
 
         weni = Org.objects.create(name="Weni", timezone="America/Maceio", created_by=user, modified_by=user)
 
         Flow.create(name="Test Temba", user=user, org=weni, is_active=False)
         Flow.create(name="Test flow name", user=user, org=weni)
@@ -37,15 +36,14 @@
         org = Org.objects.first()
         org_uuid = str(org.uuid)
 
         with self.assertRaisesMessage(test_grpc.FakeRpcError, "Org: 123 not found!"):
             self.org_statistic_list_request(org_uuid="123")
 
         with DisableTriggersOn(Contact):
-
             test_contact = Contact.objects.create(name="Test Contact", org=org)
             Contact.objects.create(name="Weni Contact", org=org)
 
             self.set_obj_active(test_contact, False)
 
             response = self.org_statistic_list_request(org_uuid=org_uuid)
             self.assertEqual(response.active_contacts, 1)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/user/serializers.py` & `weni_rp_apps-2.4.2a6/weni/grpc/user/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/user/services.py` & `weni_rp_apps-2.4.2a6/weni/grpc/user/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,18 @@
     # TODO: Remove this method, it is just a palliative solution
 
     user, created = User.objects.get_or_create(email=user_email, defaults={"username": user_email})
     return user
 
 
 class UserPermissionService(
-    AbstractService, generics.GenericService, mixins.RetrieveModelMixin, mixins.UpdateModelMixin
+    AbstractService,
+    generics.GenericService,
+    mixins.RetrieveModelMixin,
+    mixins.UpdateModelMixin,
 ):
     def Retrieve(self, request, context):
         org = self.get_org_object(request.org_uuid, "uuid")
         user = get_user(request.user_email)
 
         permissions = self.get_user_permissions(org, user)
 
@@ -94,21 +97,19 @@
             if org_field.filter(pk=user.id).exists():
                 permissions[perm_name] = True
 
         return permissions
 
 
 class UserService(generics.GenericService, AbstractService, mixins.RetrieveModelMixin):
-
     serializer_class = UserProtoSerializer
 
     def Update(self, request, context):
-
         if request.language not in [language[0] for language in settings.LANGUAGES]:
-            self.context.abort(grpc.StatusCode.INVALID_ARGUMENT, f"Invalid argument: language")
+            self.context.abort(grpc.StatusCode.INVALID_ARGUMENT, "Invalid argument: language")
 
         user = get_user(request.email)
         user_settings = user.get_settings()
         user_settings.language = request.language
         user_settings.save()
 
         serializer = UserProtoSerializer(user)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/grpc/user/tests.py` & `weni_rp_apps-2.4.2a6/weni/grpc/user/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from weni.protobuf.flows import user_pb2
 from weni.protobuf.flows import user_pb2_grpc
 
 from temba.orgs.models import Org
 
 
 class UserServiceTest(RPCTransactionTestCase):
-
     WRONG_EMAIL = "wrong@wrong.wrong"
     WRONG_UUID = "wrong-wrong-wrong-wrong-wrong."
 
     def setUp(self):
         User.objects.create_user(
             username="testuser",
             password="123",
@@ -210,15 +209,14 @@
             "agent": response.agent,
         }
         false_valeues = [key for key, value in permissions.items() if not value]
 
         return len(false_valeues) == len(permissions.items()) - 1 and permission not in false_valeues
 
     def validate_response_user(self, response, user: User):
-
         self.assertEquals(response.id, user.id)
         self.assertEquals(response.username, user.username)
         self.assertEquals(response.email, user.email)
         self.assertEquals(response.first_name, user.first_name)
         self.assertEquals(response.last_name, user.last_name)
         self.assertEquals(response.date_joined, user.date_joined.strftime("%Y-%m-%dT%H:%M:%S.%fZ"))
         self.assertEquals(response.is_active, user.is_active)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/backends.py` & `weni_rp_apps-2.4.2a6/weni/internal/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/channel/serializers.py` & `weni_rp_apps-2.4.2a6/weni/internal/channel/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 from rest_framework import serializers
 from rest_framework import exceptions
 
 from weni.serializers import fields as weni_serializers
 
 from temba.channels.models import Channel
-from temba.orgs.models import Org
 from temba.utils import analytics
 from weni.internal.models import Project
 
 
 class ChannelWACSerializer(serializers.Serializer):
     user = weni_serializers.UserEmailRelatedField(required=True, write_only=True)
     org = weni_serializers.ProjectUUIDRelatedField(required=True, write_only=True)
@@ -48,15 +47,14 @@
         return value
 
     def create(self, validated_data):
         channel_type = Channel.get_type_from_code("WAC")
         schemes = channel_type.schemes
 
         org = validated_data["org"].org
-        name = validated_data.get("name")
         phone_number_id = validated_data.get("phone_number_id")
         config = validated_data.get("config", {})
         user = validated_data.get("user")
 
         channel = Channel.objects.create(
             org=org,
             country=None,
@@ -97,15 +95,15 @@
         if channel_type is None:
             channel_type_code = validated_data.get("channeltype_code")
             raise exceptions.ValidationError(f"No channels found with '{channel_type_code}' code")
 
         url = self.create_channel(user, org.org, data, channel_type)
 
         if url is None:
-            raise exceptions.ValidationError(f"Url not created")
+            raise exceptions.ValidationError("Url not created")
 
         if "/users/login/?next=" in url:
             raise exceptions.ValidationError(f"User: {user.email} do not have permission in Org: {org.org.uuid}")
 
         regex = "[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}"
         channe_uuid = re.findall(regex, url)[0]
         channel = Channel.objects.get(uuid=channe_uuid)
@@ -130,25 +128,25 @@
 
 
 class ChannelSerializer(serializers.ModelSerializer):
     config = serializers.JSONField()
 
     class Meta:
         extra_kwargs = {
-            'org': {'read_only': True},
-            'is_active': {'read_only': True},
+            "org": {"read_only": True},
+            "is_active": {"read_only": True},
         }
         model = Channel
         fields = (
             "uuid",
             "name",
             "config",
             "address",
             "org",
             "is_active",
-        ) 
+        )
 
     def to_representation(self, instance):
         ret = super().to_representation(instance)
         ret["org"] = instance.org.project.project_uuid if hasattr(instance.org, "project") else None
 
         return ret
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/channel/tests.py` & `weni_rp_apps-2.4.2a6/weni/internal/channel/tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 import json
 from abc import ABC, abstractmethod
-from uuid import uuid1
 from unittest.mock import patch
-from unittest import mock
-from unittest import TestCase
 from rest_framework.test import APIRequestFactory, force_authenticate
 from rest_framework import status
 
 from django.contrib.auth.models import Group
 from django.urls import reverse
-from django.utils import timezone as tz
 from django.utils.http import urlencode
 from django.contrib.auth.models import User
 from django.contrib.contenttypes.models import ContentType
 
 from temba.api.models import APIToken
-from temba.flows.models import Flow
-from temba.orgs.models import Org, OrgRole
-from temba.contacts.models import Contact
+from temba.orgs.models import OrgRole
 from temba.channels.models import Channel
 from temba.channels.types import TYPES
-from temba.tests import TembaTest, mock_mailroom
+from temba.tests import TembaTest
 from weni.internal.models import Project
 
-from .views import AvailableChannels, ChannelEndpoint, extract_form_info, extract_type_info
+from .views import AvailableChannels, ChannelEndpoint
 
 view_class = ChannelEndpoint
 view_class.permission_classes = []
 
 
 class TembaRequestMixin(ABC):
     def reverse(self, viewname, kwargs=None, query_params=None):
@@ -51,15 +45,18 @@
         return self.client.get(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
 
     def request_post(self, data):
         url = reverse(self.get_url_namespace())
         token = APIToken.get_or_create(self.project, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.post(
-            url, HTTP_AUTHORIZATION=f"Token {token.key}", data=json.dumps(data), content_type="application/json"
+            url,
+            HTTP_AUTHORIZATION=f"Token {token.key}",
+            data=json.dumps(data),
+            content_type="application/json",
         )
 
     def request_delete(self, uuid, **query_params):
         url = self.reverse(self.get_url_namespace(), kwargs={"uuid": uuid}, query_params=query_params)
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.delete(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
@@ -69,15 +66,18 @@
         ...
 
 
 class CreateWACServiceTest(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
         self.project = Project.objects.create(
-            name="Weni", timezone="America/Sao_Paulo", created_by=self.user, modified_by=self.user
+            name="Weni",
+            timezone="America/Sao_Paulo",
+            created_by=self.user,
+            modified_by=self.user,
         )
         self.project.add_user(self.user, OrgRole.ADMINISTRATOR)
 
         self.config = {
             "wa_number": "5561995743921",
             "wa_verified_name": "Weni Test",
             "wa_waba_id": "2433443436435435",
@@ -123,26 +123,30 @@
 
         self.request_post(data=payload)
 
         channel = self.request_post(data=payload)
 
         self.assertEqual(channel.status_code, 400)
         self.assertEqual(
-            channel.json().get("phone_number_id").get("error_type"), "WhatsApp.config.error.channel_already_exists"
+            channel.json().get("phone_number_id").get("error_type"),
+            "WhatsApp.config.error.channel_already_exists",
         )
 
     def get_url_namespace(self):
         return "channel-create-wac"
 
 
 class ReleaseChannelTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.org_user = User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
         self.my_org = Project.objects.create(
-            name="Weni", timezone="Africa/Kigali", created_by=self.org_user, modified_by=self.org_user
+            name="Weni",
+            timezone="Africa/Kigali",
+            created_by=self.org_user,
+            modified_by=self.org_user,
         )
 
         super().setUp()
         self.channel_obj = Channel.create(self.my_org.org, self.org_user, None, "WWC", "Test WWC")
 
     def test_released_channel_is_active_equal_to_false(self):
         response = self.request_delete(uuid=str(self.channel_obj.uuid), user=self.org_user.email)
@@ -153,15 +157,18 @@
         return "channel-detail"
 
 
 class CreateChannelTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.org_user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
         self.project = Project.objects.create(
-            name="Weni", timezone="America/Sao_Paulo", created_by=self.org_user, modified_by=self.org_user
+            name="Weni",
+            timezone="America/Sao_Paulo",
+            created_by=self.org_user,
+            modified_by=self.org_user,
         )
         self.project.add_user(self.org_user, OrgRole.ADMINISTRATOR)
 
         super().setUp()
 
     def test_create_weni_web_chat_channel(self):
         payload = {
@@ -186,21 +193,30 @@
         return "channel-list"
 
 
 class RetrieveChannelTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
         self.project = Project.objects.create(
-            name="Weni", timezone="America/Sao_Paulo", created_by=self.user, modified_by=self.user
+            name="Weni",
+            timezone="America/Sao_Paulo",
+            created_by=self.user,
+            modified_by=self.user,
         )
 
         super().setUp()
 
         self.channel_obj = Channel.create(
-            self.project.org, self.user, None, "WWC", "Test WWC", "test", {"fake_key": "fake_value"}
+            self.project.org,
+            self.user,
+            None,
+            "WWC",
+            "Test WWC",
+            "test",
+            {"fake_key": "fake_value"},
         )
 
     def test_channel_retrieve_returned_fields(self):
         response = self.request_detail(uuid=str(self.channel_obj.uuid)).json()
 
         self.assertEqual(response.get("name"), self.channel_obj.name)
         self.assertEqual(response.get("address"), self.channel_obj.address)
@@ -209,20 +225,26 @@
     def get_url_namespace(self):
         return "channel-detail"
 
 
 class ListChannelTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.admin = User.objects.create_user(
-            username="testuseradmin", password="123", email="test@weni.ai", is_superuser=True
+            username="testuseradmin",
+            password="123",
+            email="test@weni.ai",
+            is_superuser=True,
         )
         self.user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
         self.projects = [
             Project.objects.create(
-                name=f"Org {project}", timezone="America/Sao_Paulo", created_by=self.user, modified_by=self.user
+                name=f"Org {project}",
+                timezone="America/Sao_Paulo",
+                created_by=self.user,
+                modified_by=self.user,
             )
             for project in range(2)
         ]
 
         for channel in range(6):
             Channel.create(
                 self.projects[0] if channel % 2 == 0 else self.projects[1],
@@ -396,15 +418,15 @@
         test_form = {
             'widget': to_object(**{'input_type': 'text'}),
             'help_text': 'test field',
             'label': 'test_label'
         }
         result = extract_form_info(to_object(**test_form),'')
         self.assertEqual(result, None)
-        
+
     def test_form_without_type_value(self):
         """ check response without #widget attribute """
         test_form = {
             'help_text': 'test field',
             'label': 'test_label'
         }
         result = extract_form_info(to_object(**test_form),'test_form03')
@@ -414,22 +436,22 @@
         """ make sure that all results have code and name """
         have_code_name = True
         for value in self.types:
             type_in = self.types[value]
             result = extract_type_info(type_in)
             if not (result.get('code')) or not (result.get('name')):
                 have_code_name = False
-        
+
         self.assertEqual(have_code_name, True)
-    
+
     def test_all_types_response_contains_dict(self):
         """ make sure that all results have been processed and converted to dictionaries """
         for value in self.types:
             type_in = self.types[value]
             result = extract_type_info(type_in)
             self.assertEqual(type(result), dict)
 
 
 class to_object:
     def __init__(self, **entries):
         return self.__dict__.update(entries)
-'''
+'''
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/channel/views.py` & `weni_rp_apps-2.4.2a6/weni/internal/channel/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/classifier/serializers.py` & `weni_rp_apps-2.4.2a6/weni/internal/classifier/serializers.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from temba.classifiers.models import Classifier
 from weni.protobuf.flows import classifier_pb2
 from weni.grpc.core import serializers as weni_serializers
 
 
 class ClassifierSerializer(serializers.Serializer):
-
     uuid = serializers.UUIDField(read_only=True)
     is_active = serializers.BooleanField(read_only=True)
     classifier_type = serializers.CharField(required=True)
     name = serializers.CharField(required=True)
     access_token = weni_serializers.SerializerMethodCharField(required=True)
     user = weni_serializers.UserEmailRelatedField(write_only=True)
     org = weni_serializers.OrgUUIDRelatedField(write_only=True)
@@ -26,13 +25,21 @@
         classifier.sync()
 
         return classifier
 
     class Meta:
         model = Classifier
         proto_class = classifier_pb2.Classifier
-        fields = ["uuid", "is_active", "classifier_type", "name", "access_token", "org", "user"]
+        fields = [
+            "uuid",
+            "is_active",
+            "classifier_type",
+            "name",
+            "access_token",
+            "org",
+            "user",
+        ]
 
 
 class ClassifierDeleteSerializer(serializers.Serializer):
     uuid = serializers.UUIDField(required=True)
     user = weni_serializers.UserEmailRelatedField(required=True)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/classifier/tests.py` & `weni_rp_apps-2.4.2a6/weni/internal/classifier/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 from abc import ABC, abstractmethod
 from unittest.mock import patch
 from django.contrib.auth.models import User
 
 from django.contrib.auth.models import Group
 from django.urls import reverse
 from django.utils.http import urlencode
-from django.contrib.auth.models import User
 
 from temba.api.models import APIToken
 
-from temba.tests import TembaTest, mock_mailroom
+from temba.tests import TembaTest
 from temba.orgs.models import Org
 from temba.classifiers.models import Classifier, Intent
 from temba.classifiers.types.wit import WitType
 from temba.classifiers.types.luis import LuisType
-from weni.protobuf.flows import classifier_pb2, classifier_pb2_grpc
 
 
 class TembaRequestMixin(ABC):
     def reverse(self, viewname, kwargs=None, query_params=None):
         url = reverse(viewname, kwargs=kwargs)
 
         if query_params:
@@ -40,19 +38,26 @@
         return self.client.get(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
 
     def request_post(self, data):
         url = reverse(self.get_url_namespace())
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.post(
-            url, HTTP_AUTHORIZATION=f"Token {token.key}", data=json.dumps(data), content_type="application/json"
+            url,
+            HTTP_AUTHORIZATION=f"Token {token.key}",
+            data=json.dumps(data),
+            content_type="application/json",
         )
 
     def request_delete(self, uuid, user_email):
-        url = self.reverse(self.get_url_namespace(), query_params={"user_email": user_email}, kwargs={"uuid": uuid})
+        url = self.reverse(
+            self.get_url_namespace(),
+            query_params={"user_email": user_email},
+            kwargs={"uuid": uuid},
+        )
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.delete(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
 
     @abstractmethod
     def get_url_namespace(self):
         ...
@@ -65,15 +70,18 @@
         self.admin = User.objects.create_user(
             username="testuser", password="123", email="test@weni.ai", is_superuser=True
         )
 
         print(self.admin.is_authenticated)
 
         self.org = Org.objects.create(
-            name="Weni", timezone="America/Maceio", created_by=self.admin, modified_by=self.admin
+            name="Weni",
+            timezone="America/Maceio",
+            created_by=self.admin,
+            modified_by=self.admin,
         )
 
         super().setUp()
 
     def test_list_classifier(self):
         org = Org.objects.first()
         org_uuid = str(org.uuid)
@@ -135,15 +143,18 @@
         self.config = {"access_token": "hbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9"}
 
         self.admin = User.objects.create_user(
             username="testuser", password="123", email="test@weni.ai", is_superuser=True
         )
 
         self.org = Org.objects.create(
-            name="Weni", timezone="America/Maceio", created_by=self.admin, modified_by=self.admin
+            name="Weni",
+            timezone="America/Maceio",
+            created_by=self.admin,
+            modified_by=self.admin,
         )
 
         super().setUp()
 
     @patch("temba.classifiers.tasks.sync_classifier_intents")
     def test_create_classifier(self, mock):
         mock.return_value = None
@@ -178,15 +189,18 @@
         self.config = {"access_token": "hbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9"}
 
         self.admin = User.objects.create_user(
             username="testuser", password="123", email="test@weni.ai", is_superuser=True
         )
 
         self.org = Org.objects.create(
-            name="Weni", timezone="America/Maceio", created_by=self.admin, modified_by=self.admin
+            name="Weni",
+            timezone="America/Maceio",
+            created_by=self.admin,
+            modified_by=self.admin,
         )
 
         super().setUp()
 
     def test_retrieve_classifier_by_valid_uuid(self):
         classifier = Classifier.create(self.org, self.admin, LuisType.slug, "Test2", self.config, sync=False)
         response = self.request_detail(uuid=str(classifier.uuid)).json()
@@ -205,26 +219,29 @@
         self.config = {"access_token": "hbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9"}
 
         self.admin = User.objects.create_user(
             username="testuser", password="123", email="test@weni.ai", is_superuser=True
         )
 
         self.org = Org.objects.create(
-            name="Weni", timezone="America/Maceio", created_by=self.admin, modified_by=self.admin
+            name="Weni",
+            timezone="America/Maceio",
+            created_by=self.admin,
+            modified_by=self.admin,
         )
 
         super().setUp()
 
     def test_destroy_classifier_by_valid_uuid(self):
         classifier = Classifier.create(self.org, self.admin, LuisType.slug, "Test2", self.config, sync=False)
         Intent.objects.create(classifier=classifier, name="Test Intent", external_id="FakeExternal")
 
         self.assertEqual(classifier.intents.count(), 1)
 
-        t = self.request_delete(uuid=str(classifier.uuid), user_email=self.admin.email)
+        self.request_delete(uuid=str(classifier.uuid), user_email=self.admin.email)
 
         classifier = Classifier.objects.get(uuid=classifier.uuid)
         self.assertEqual(classifier.intents.count(), 0)
         self.assertFalse(classifier.is_active)
 
     def get_url_namespace(self):
         return "classifier-detail"
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/classifier/views.py` & `weni_rp_apps-2.4.2a6/weni/internal/classifier/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 from rest_framework import viewsets
-from rest_framework import generics
-from rest_framework import mixins
-from rest_framework.renderers import JSONRenderer
 from rest_framework.response import Response
 from rest_framework import status
 from rest_framework.exceptions import ValidationError
 
-from django.contrib.auth.models import User
-from django.db.models import Count, Prefetch, Q
-from django.urls import reverse
 from django.http import JsonResponse
 
-from temba.api.v2.views_base import BaseAPIView, ListAPIMixin
-from temba.contacts.models import Contact, ContactGroup
 from temba.classifiers.models import Classifier
 from temba.orgs.models import Org
 
 from .serializers import ClassifierSerializer, ClassifierDeleteSerializer
 from weni.internal.views import InternalGenericViewSet
 
 
 class ClassifierEndpoint(viewsets.ModelViewSet, InternalGenericViewSet):
-
     serializer_class = ClassifierSerializer
     lookup_field = "uuid"
 
     def get_queryset(self):
-
         is_active_possibilities = {
             "True": True,
             "False": False,
             "true": True,
             "false": False,
         }
 
@@ -67,24 +57,22 @@
             return JsonResponse(data=serializer.errors, status=status.HTTP_400_BAD_REQUEST)
 
         serializer.save()
 
         return JsonResponse(data=serializer.data, status=status.HTTP_200_OK)
 
     def retrieve(self, request, uuid=None):
-
         try:
             classifier = Classifier.objects.get(uuid=uuid)
         except Classifier.DoesNotExist:
             return Response(status=status.HTTP_404_NOT_FOUND)
 
         return JsonResponse(data=self.get_serializer(classifier).data, status=status.HTTP_200_OK)
 
     def destroy(self, request, uuid=None):
-
         data = {
             "uuid": uuid,
             "user": request.query_params.get("user_email"),
         }
 
         serializer = ClassifierDeleteSerializer(data=data)
         if not serializer.is_valid():
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/clients/authenticators.py` & `weni_rp_apps-2.4.2a6/weni/internal/clients/authenticators.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,14 @@
                 "client_secret": settings.OIDC_RP_CLIENT_SECRET,
                 "grant_type": "client_credentials",
             },
         )
 
         token = response.json().get("access_token")
         return f"Bearer {token}"
-    
+
     @property
     def headers(self):
         return {
             "Content-Type": "application/json; charset: utf-8",
             "Authorization": self._get_module_token(),
         }
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/externals/serializers.py` & `weni_rp_apps-2.4.2a6/weni/internal/externals/serializers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from rest_framework import serializers
 
 
-from weni.serializers import OrgUUIDRelatedField, UserEmailRelatedField
+from weni.serializers import UserEmailRelatedField
 from temba.externals.models import ExternalService
+from weni.serializers.fields import ProjectUUIDRelatedField
 
 
 class ExternalServicesSerializer(serializers.Serializer):
-
     uuid = serializers.UUIDField(read_only=True)
     type_code = serializers.CharField(write_only=True)
     type_fields = serializers.JSONField(write_only=True)
-    org = OrgUUIDRelatedField(write_only=True)
+    project = ProjectUUIDRelatedField(write_only=True)
     user = UserEmailRelatedField(write_only=True)
 
     external_service_type = serializers.CharField(read_only=True)
     name = serializers.CharField(read_only=True)
     config = serializers.JSONField(read_only=True)
 
     def create(self, validated_data: dict):
         validated_data = validated_data
 
         type_code = validated_data.get("type_code")
         type_fields = validated_data.get("type_fields")
         user = validated_data.get("user")
-        org = validated_data.get("org")
+        project = validated_data.get("project")
 
         try:
             type_ = ExternalService.get_type_from_code(type_code)
         except KeyError as error:
             raise serializers.ValidationError(error)
 
         type_serializer = type_.serializer_class(data=type_fields)
         type_serializer.is_valid(raise_exception=True)
-        return type_serializer.save(type=type_, created_by=user, modified_by=user, org=org)
+        return type_serializer.save(
+            type=type_, created_by=user, modified_by=user, org=project
+        )
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/externals/views.py` & `weni_rp_apps-2.4.2a6/weni/internal/externals/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/flows/serializers.py` & `weni_rp_apps-2.4.2a6/weni/internal/flows/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/flows/tests.py` & `weni_rp_apps-2.4.2a6/weni/internal/flows/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,18 @@
         return self.client.get(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
 
     def request_post(self, data):
         url = reverse(self.get_url_namespace())
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.post(
-            url, HTTP_AUTHORIZATION=f"Token {token.key}", data=json.dumps(data), content_type="application/json"
+            url,
+            HTTP_AUTHORIZATION=f"Token {token.key}",
+            data=json.dumps(data),
+            content_type="application/json",
         )
 
     def request_delete(self, uuid):
         url = self.reverse(self.get_url_namespace(), kwargs={"uuid": uuid})
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.delete(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
@@ -52,15 +55,14 @@
     @abstractmethod
     def get_url_namespace(self):
         ...
 
 
 class ListFlowTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
-
         User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
 
         user = User.objects.first()
 
         # print(Org.objects.all())
 
         temba = Org.objects.create(name="Temba", timezone="America/Maceio", created_by=user, modified_by=user)
@@ -69,15 +71,14 @@
         Flow.create(name="Test Temba", user=user, org=temba)
         Flow.create(name="Test flow name", user=user, org=weni)
         Flow.create(name="Test Weni flow name", user=user, org=weni)
 
         super().setUp()
 
     def test_list_flow(self):
-
         temba = Org.objects.filter(name="Temba").first()
         weni = Org.objects.get(name="Weni")
 
         response = self.request_get(flow_name="test", org_uuid="123")  # {'org_uuid': ['“123” is not a valid UUID.']}
         self.assertEquals(response.status_code, 400)
 
         response = self.request_get(flow_name="test", org_uuid="")  # {'org_id': ['This field may not be blank.']}
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/flows/views.py` & `weni_rp_apps-2.4.2a6/weni/internal/flows/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/globals/serializers.py` & `weni_rp_apps-2.4.2a6/weni/internal/globals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/globals/tests/test_serializers.py` & `weni_rp_apps-2.4.2a6/weni/internal/globals/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/globals/views.py` & `weni_rp_apps-2.4.2a6/weni/internal/globals/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
             org_object = Org.objects.get(uuid=org)
             queryset = queryset.filter(org=org_object)
             return queryset
 
         except Org.DoesNotExist as error:
             raise ValidationError(detail={"message": str(error)})
 
-
     def create(self, request, *args, **kwargs):
         serializer = self.get_serializer(data=request.data, many=True)
         serializer.is_valid(raise_exception=True)
 
         self.perform_create(serializer.validated_data)
 
         headers = self.get_success_headers(serializer.data)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/migrations/0002_project.py` & `weni_rp_apps-2.4.2a6/weni/internal/migrations/0002_project.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/models.py` & `weni_rp_apps-2.4.2a6/weni/internal/models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/orgs/serializers.py` & `weni_rp_apps-2.4.2a6/weni/internal/orgs/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         user, _ = User.objects.get_or_create(email=user_email, defaults={"username": user_email})
         attrs["created_by"] = user
         attrs["modified_by"] = user
 
         attrs.pop("user_email")
 
         return super().validate(attrs)
-    
+
     def to_representation(self, instance):
         ret = super().to_representation(instance)
         ret["uuid"] = instance.project_uuid
 
         return ret
 
     def create(self, validated_data):
@@ -62,26 +62,39 @@
         values = ["id", "email", "username", "first_name", "last_name"]
 
         administrators = list(project.administrators.all().values(*values))
         viewers = list(project.viewers.all().values(*values))
         editors = list(project.editors.all().values(*values))
         surveyors = list(project.surveyors.all().values(*values))
 
-        administrators = list(map(lambda user: self.set_user_permission(user, "administrator"), administrators))
+        administrators = list(
+            map(
+                lambda user: self.set_user_permission(user, "administrator"),
+                administrators,
+            )
+        )
         viewers = list(map(lambda user: self.set_user_permission(user, "viewer"), viewers))
         editors = list(map(lambda user: self.set_user_permission(user, "editor"), editors))
         surveyors = list(map(lambda user: self.set_user_permission(user, "surveyor"), surveyors))
 
         users = administrators + viewers + editors + surveyors
 
         return users
 
     class Meta:
         model = Project
-        fields = ["id", "name", "uuid", "timezone", "date_format", "users", "flow_organization"]
+        fields = [
+            "id",
+            "name",
+            "uuid",
+            "timezone",
+            "date_format",
+            "users",
+            "flow_organization",
+        ]
 
 
 class OrgCreateSerializer(serializers.ModelSerializer):
     user_email = serializers.EmailField()
 
     class Meta:
         model = Project
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/orgs/tests.py` & `weni_rp_apps-2.4.2a6/weni/internal/orgs/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/orgs/views.py` & `weni_rp_apps-2.4.2a6/weni/internal/orgs/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,25 +36,25 @@
         return Response(serializer.data)
 
     def create(self, request):
         serializer = OrgCreateSerializer(data=request.data)
         serializer.is_valid(raise_exception=True)
 
         user, created = User.objects.get_or_create(
-            email=request.data.get("user_email"), defaults={"username": request.data.get("user_email")}
+            email=request.data.get("user_email"),
+            defaults={"username": request.data.get("user_email")},
         )
 
         project = Project.objects.create(
             name=request.data.get("name"),
             timezone=request.data.get("timezone"),
             created_by=user,
             modified_by=user,
             plan="infinity",
-            project_uuid=request.data.get("uuid")
-
+            project_uuid=request.data.get("uuid"),
         )
 
         project.administrators.add(user)
         project.initialize()
 
         org_serializer = OrgSerializer(project)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/statistic/tests.py` & `weni_rp_apps-2.4.2a6/weni/internal/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/statistic/views.py` & `weni_rp_apps-2.4.2a6/weni/internal/statistic/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/tests/test_models.py` & `weni_rp_apps-2.4.2a6/weni/internal/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/tickets/serializers.py` & `weni_rp_apps-2.4.2a6/weni/internal/tickets/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 class TicketerConfigSerializer(serializers.Serializer):
     project_auth = serializers.CharField(required=True)
     sector_uuid = serializers.CharField(required=True)
 
 
 class TicketerSerializer(serializers.ModelSerializer):
-
     org = weni_serializers.OrgUUIDRelatedField(required=True)
     config = TicketerConfigSerializer(required=True)
 
     class Meta:
         model = Ticketer
         fields = ("uuid", "org", "ticketer_type", "name", "config")
         read_only_fields = ("uuid",)
@@ -30,13 +29,12 @@
         validated_data["created_by"] = user
         validated_data["modified_by"] = user
 
         return super().create(validated_data)
 
 
 class TicketerQueueSerializer(serializers.ModelSerializer):
-
     uuid = serializers.UUIDField(required=True)
 
     class Meta:
         model = TicketerQueue
         fields = ("uuid", "name")
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/tickets/tests/test_views.py` & `weni_rp_apps-2.4.2a6/weni/internal/tickets/tests/test_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import json
 from uuid import uuid4
 
 from django.urls import reverse
-from django.db import transaction
 from rest_framework.test import APIRequestFactory, force_authenticate
 from rest_framework.permissions import AllowAny
 from rest_framework import status
 
 from temba.tests import TembaTest
 from temba.tickets.models import Ticketer
 from temba.tickets.types.rocketchat import RocketChatType
 from weni.internal.tickets import views
 from weni.internal.models import TicketerQueue
 
 
 class TicketerQueueViewTestMixin(object):
-
     action: dict
 
     def setUp(self):
         self.fake_chats_uuid = uuid4()
         self.factory = APIRequestFactory()
         self.view = views.TicketerQueueViewSet
         self.view.permission_classes = [AllowAny]
@@ -45,28 +43,26 @@
         request = getattr(self.factory, method)(*args, data=data)
         force_authenticate(request, self.user)
 
         return self._get_response(request, **kwargs)
 
 
 class CreateTicketerQueueViewTestCase(TicketerQueueViewTestMixin, TembaTest):
-
     action = dict(post="create")
 
     def test_create_queue(self):
         uuid = str(uuid4())
         kwargs = dict(ticketer_uuid=str(self.ticketer.uuid))
 
         url = reverse("ticketer-queues-list", kwargs=kwargs)
         self.request("post", url, data={"uuid": uuid, "name": "123"}, **kwargs)
         self.assertTrue(self.ticketer.queues.filter(uuid=uuid).exists())
 
 
 class UpdateTicketerQueueViewTestCase(TicketerQueueViewTestMixin, TembaTest):
-
     action = dict(patch="partial_update")
 
     def test_update_queue(self):
         kwargs = dict(ticketer_uuid=str(self.ticketer.uuid), uuid=str(self.queue.uuid))
         url = reverse("ticketer-queues-detail", kwargs=kwargs)
 
         old_name = self.queue.name
@@ -76,15 +72,14 @@
         self.queue.refresh_from_db()
 
         self.assertEqual(self.queue.name, new_name)
         self.assertNotEqual(self.queue.name, old_name)
 
 
 class DestroyTicketerQueueViewTestCase(TicketerQueueViewTestMixin, TembaTest):
-
     action = dict(delete="destroy")
 
     def test_destroy_queue(self):
         kwargs = dict(ticketer_uuid=str(self.ticketer.uuid), uuid=str(self.queue.uuid))
 
         url = reverse("ticketer-queues-detail", kwargs=kwargs)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/tickets/views.py` & `weni_rp_apps-2.4.2a6/weni/internal/tickets/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/urls.py` & `weni_rp_apps-2.4.2a6/weni/internal/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/users/serializers.py` & `weni_rp_apps-2.4.2a6/weni/internal/users/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/users/tests.py` & `weni_rp_apps-2.4.2a6/weni/internal/users/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from django.contrib.auth.models import Group
 from django.urls import reverse
 from django.utils.http import urlencode
 
 from temba.api.models import APIToken
 
 from temba.tests import TembaTest
-from temba.orgs.models import Org
 from weni.internal.models import Project
 from weni.internal.users.views import UserEndpoint, UserPermissionEndpoint, UserViewSet
 
 view_set = UserViewSet
 view_set.permission_classes = []
 
 view_permissions = UserPermissionEndpoint
@@ -46,104 +45,152 @@
         return self.client.get(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
 
     def request_patch(self, data, **kwargs):
         url = self.reverse(self.get_url_namespace(), query_params=kwargs)
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.patch(
-            f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}", data=json.dumps(data), content_type="application/json"
+            f"{url}",
+            HTTP_AUTHORIZATION=f"Token {token.key}",
+            data=json.dumps(data),
+            content_type="application/json",
         )
 
     def request_post(self, data):
         url = reverse(self.get_url_namespace())
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.post(
-            url, HTTP_AUTHORIZATION=f"Token {token.key}", data=json.dumps(data), content_type="application/json"
+            url,
+            HTTP_AUTHORIZATION=f"Token {token.key}",
+            data=json.dumps(data),
+            content_type="application/json",
         )
 
     def request_delete(self, data, **kwargs):
         url = self.reverse(self.get_url_namespace(), query_params=kwargs)
         token = APIToken.get_or_create(self.project, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.delete(
-            f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}", data=json.dumps(data), content_type="application/json"
+            f"{url}",
+            HTTP_AUTHORIZATION=f"Token {token.key}",
+            data=json.dumps(data),
+            content_type="application/json",
         )
 
     @abstractmethod
     def get_url_namespace(self):
         ...
 
 
 class UserPermissionUpdateDestroyTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.admin = User.objects.create_user(
             username="testuser", password="123", email="test@weni.ai", is_superuser=True
         )
 
         self.project = Project.objects.create(
-            name="Test", timezone="Africa/Kigali", created_by=self.admin, modified_by=self.admin
+            name="Test",
+            timezone="Africa/Kigali",
+            created_by=self.admin,
+            modified_by=self.admin,
         )
         super().setUp()
 
     def test_user_permission_destroy(self):
         project = Project.objects.first()
         user = User.objects.first()
 
         destroy_wrong_permission = self.request_delete(
-            data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="adm")
+            data=dict(
+                org_uuid=str(project.project_uuid),
+                user_email=user.email,
+                permission="adm",
+            )
         )
         self.assertEqual(destroy_wrong_permission.status_code, 400)
         self.assertEqual(destroy_wrong_permission.json()[0], "adm is not a valid permission!")
 
-        self.request_patch(data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="viewer"))
+        self.request_patch(
+            data=dict(
+                org_uuid=str(project.project_uuid),
+                user_email=user.email,
+                permission="viewer",
+            )
+        )
         user_permissions = self._get_user_permissions(project=project, user=user)
 
-        self.request_delete(data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="viewer"))
+        self.request_delete(
+            data=dict(
+                org_uuid=str(project.project_uuid),
+                user_email=user.email,
+                permission="viewer",
+            )
+        )
         user_permissions_removed = self._get_user_permissions(project=project, user=user)
 
         self.assertFalse(user_permissions_removed.get("viewer", False))
         self.assertNotEquals(user_permissions, user_permissions_removed)
 
     def test_user_permission_update(self):
         project = Project.objects.first()
         user = User.objects.first()
 
         update_wrong_permission_response = self.request_patch(
-            data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="adm")
+            data=dict(
+                org_uuid=str(project.project_uuid),
+                user_email=user.email,
+                permission="adm",
+            )
         )
         self.assertEqual(update_wrong_permission_response.status_code, 400)
         self.assertEqual(update_wrong_permission_response.json()[0], "adm is not a valid permission!")
 
         update_response = self.request_patch(
-            data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="administrator")
+            data=dict(
+                org_uuid=str(project.project_uuid),
+                user_email=user.email,
+                permission="administrator",
+            )
         ).json()
         user_permissions = self._get_user_permissions(project, user)
 
         self.assertTrue(user_permissions.get("administrator"))
         self.assertTrue(self._permission_is_unique_true(update_response, "administrator"))
 
         update_response = self.request_patch(
-            data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="viewer")
+            data=dict(
+                org_uuid=str(project.project_uuid),
+                user_email=user.email,
+                permission="viewer",
+            )
         ).json()
         user_permissions = self._get_user_permissions(project, user)
 
         self.assertTrue(user_permissions.get("viewer"))
         self.assertTrue(self._permission_is_unique_true(update_response, "viewer"))
 
         update_response = self.request_patch(
-            data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="editor")
+            data=dict(
+                org_uuid=str(project.project_uuid),
+                user_email=user.email,
+                permission="editor",
+            )
         ).json()
         user_permissions = self._get_user_permissions(project, user)
 
         self.assertTrue(user_permissions.get("editor"))
         self.assertTrue(self._permission_is_unique_true(update_response, "editor"))
 
         update_response = self.request_patch(
-            data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="surveyor")
+            data=dict(
+                org_uuid=str(project.project_uuid),
+                user_email=user.email,
+                permission="surveyor",
+            )
         ).json()
         user_permissions = self._get_user_permissions(project, user)
 
         self.assertTrue(user_permissions.get("surveyor"))
         self.assertTrue(self._permission_is_unique_true(update_response, "surveyor"))
 
     def _get_permissions(self, project: Project) -> dict:
@@ -181,15 +228,18 @@
 
 class UserPermissionRetrieveTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.admin = User.objects.create_user(
             username="testuser", password="123", email="test@weni.ai", is_superuser=True
         )
         self.project = Project.objects.create(
-            name="Test", timezone="Africa/Kigali", created_by=self.admin, modified_by=self.admin
+            name="Test",
+            timezone="Africa/Kigali",
+            created_by=self.admin,
+            modified_by=self.admin,
         )
         super().setUp()
 
     def test_user_permission_retrieve(self):
         project = Project.objects.first()
         user = User.objects.first()
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/users/urls.py` & `weni_rp_apps-2.4.2a6/weni/internal/users/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/users/views.py` & `weni_rp_apps-2.4.2a6/weni/internal/users/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,41 +8,53 @@
 from rest_framework.decorators import action
 from rest_framework.response import Response
 from rest_framework import exceptions
 from rest_framework import mixins
 from rest_framework.exceptions import ValidationError
 
 from weni.internal.views import InternalGenericViewSet
-from weni.internal.users.serializers import UserAPITokenSerializer, UserSerializer, UserPermissionSerializer
+from weni.internal.users.serializers import (
+    UserAPITokenSerializer,
+    UserSerializer,
+    UserPermissionSerializer,
+)
 from temba.api.models import APIToken
 from temba.orgs.models import Org
-from weni.internal.models import Project
 
 
 if TYPE_CHECKING:
     from rest_framework.request import Request
 
 User = get_user_model()
 
 
 class UserViewSet(InternalGenericViewSet):
-    @action(detail=False, methods=["GET"], url_path="api-token", serializer_class=UserAPITokenSerializer)
+    @action(
+        detail=False,
+        methods=["GET"],
+        url_path="api-token",
+        serializer_class=UserAPITokenSerializer,
+    )
     def api_token(self, request: "Request", **kwargs):
         serializer = self.get_serializer(data=request.query_params)
         serializer.is_valid(raise_exception=True)
         user = serializer.validated_data.get("user")
         project = serializer.validated_data.get("project")
 
         try:
             api_token = APIToken.objects.get(user=user, org=project.org)
         except APIToken.DoesNotExist:
             raise exceptions.PermissionDenied()
 
         return Response(
-            dict(user=api_token.user.email, project=project.project_uuid, api_token=api_token.key)
+            dict(
+                user=api_token.user.email,
+                project=project.project_uuid,
+                api_token=api_token.key,
+            )
         )
 
 
 class UserPermissionEndpoint(InternalGenericViewSet):
     serializer_class = UserPermissionSerializer
 
     def retrieve(self, request):
@@ -146,12 +158,13 @@
         return Response(status=status.HTTP_200_OK)
 
     def retrieve(self, request):
         if not request.query_params.get("email"):
             raise ValidationError(detail="empty email")
 
         user = User.objects.get_or_create(
-            email=request.query_params.get("email"), defaults={"username": request.query_params.get("email")}
+            email=request.query_params.get("email"),
+            defaults={"username": request.query_params.get("email")},
         )
 
         serializer = self.get_serializer(user[0])
         return Response(serializer.data)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/internal/views.py` & `weni_rp_apps-2.4.2a6/weni/internal/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/orgs_api/serializers.py` & `weni_rp_apps-2.4.2a6/weni/orgs_api/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/orgs_api/tests.py` & `weni_rp_apps-2.4.2a6/weni/orgs_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/orgs_api/views.py` & `weni_rp_apps-2.4.2a6/weni/orgs_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/s3/views.py` & `weni_rp_apps-2.4.2a6/weni/s3/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/serializers/fields.py` & `weni_rp_apps-2.4.2a6/weni/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/success_orgs/business.py` & `weni_rp_apps-2.4.2a6/weni/success_orgs/business.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 
 
 SUCCESS_ORG_QUERIES = dict(
     has_ia=Exists(Classifier.objects.filter(org=OuterRef("pk"), classifier_type="bothub", is_active=True)),
     has_flows=Exists(Flow.objects.filter(org=OuterRef("pk"), is_active=True)),
     has_channel=Exists(Channel.objects.filter(org=OuterRef("pk"), is_active=True)),
     has_msg=Exists(Msg.objects.filter(org=OuterRef("pk"))),
+    has_channel_production=Exists(
+        Channel.objects.filter(org=OuterRef("pk"), is_active=True).exclude(name="WhatsApp: +558231420933")
+    ),
 )
 
 
 class UserDoesNotExist(User.DoesNotExist):
     pass
 
 
@@ -54,15 +57,22 @@
 
 def get_success_orgs() -> "QuerySet[Org]":
     return (
         Org.objects.annotate(user_last_login=F("created_by__last_login"))
         .annotate(**SUCCESS_ORG_QUERIES)
         .annotate(
             is_success_project=Case(
-                When(has_ia=True, has_flows=True, has_channel=True, has_msg=True, then=Value(True)),
+                When(
+                    has_ia=True,
+                    has_flows=True,
+                    has_channel=True,
+                    has_msg=True,
+                    has_channel_production=True,
+                    then=Value(True),
+                ),
                 output_field=BooleanField(),
                 default=Value(False),
             )
         )
     )
 
 
@@ -73,12 +83,11 @@
 def get_user_success_orgs_by_email(email: str) -> dict:
     user = get_user_by_email(email)
 
     return dict(email=user.email, last_login=user.last_login, orgs=get_user_success_orgs(user))
 
 
 def retrieve_success_org(org_uuid: str) -> Org:
-
     try:
         return get_success_orgs().get(uuid=org_uuid)
     except Org.DoesNotExist as error:
         raise OrgDoesNotExist(error)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/success_orgs/serializers.py` & `weni_rp_apps-2.4.2a6/weni/success_orgs/serializers.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 class SuccessOrgSerializer(serializers.Serializer):
     uuid = serializers.UUIDField()
     name = serializers.CharField()
     has_ia = serializers.BooleanField()
     has_flows = serializers.BooleanField()
     has_channel = serializers.BooleanField()
     has_msg = serializers.BooleanField()
+    has_channel_production = serializers.BooleanField()
     is_success_project = serializers.BooleanField()
 
 
 class UserSuccessOrgSerializer(serializers.Serializer):
     email = serializers.EmailField()
     last_login = serializers.CharField()
     orgs = SuccessOrgSerializer(many=True)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/success_orgs/tests/test_business.py` & `weni_rp_apps-2.4.2a6/weni/success_orgs/tests/test_business.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 User = get_user_model()
 
 
 class SetupMixin(object):
     def setUp(self) -> None:
         self.user_email = "fake@weni.ai"
         self.user = User.objects.create(email=self.user_email)
-        self.org = Org.objects.create(created_by=self.user, modified_by=self.user, name="fakeorg")
+        self.org = Org.objects.create(
+            created_by=self.user, modified_by=self.user, name="fakeorg"
+        )
 
 
 class GetUserByEmailTestCase(SetupMixin, TestCase):
     def test_get_user_by_email(self):
         user = get_user_by_email(self.user_email)
         self.assertEqual(user.email, self.user_email)
 
@@ -39,43 +41,58 @@
 class GetUserSuccessOrgsTestCase(SetupMixin, TestCase):
     def test_function_returns_extra_fields(self):
         org = get_user_success_orgs(self.user).first()
         self.assertTrue(hasattr(org, "has_ia"))
         self.assertTrue(hasattr(org, "has_flows"))
         self.assertTrue(hasattr(org, "has_channel"))
         self.assertTrue(hasattr(org, "has_msg"))
+        self.assertTrue(hasattr(org, "has_channel_production"))
 
     def test_when_adding_classifier_it_returns_true(self):
         Classifier.objects.create(
-            org=self.org, created_by=self.user, modified_by=self.user, config={}, classifier_type="bothub"
+            org=self.org,
+            created_by=self.user,
+            modified_by=self.user,
+            config={},
+            classifier_type="bothub",
         )
 
         org = get_user_success_orgs(self.user).first()
         self.assertTrue(org.has_ia)
         self.assertFalse(org.has_flows)
         self.assertFalse(org.has_channel)
         self.assertFalse(org.has_msg)
+        self.assertFalse(org.has_channel_production)
 
     def test_when_adding_flow_it_returns_true(self):
-        Flow.objects.create(org=self.org, created_by=self.user, modified_by=self.user, saved_by=self.user)
+        Flow.objects.create(
+            org=self.org,
+            created_by=self.user,
+            modified_by=self.user,
+            saved_by=self.user,
+        )
 
         org = get_user_success_orgs(self.user).first()
         self.assertFalse(org.has_ia)
         self.assertTrue(org.has_flows)
         self.assertFalse(org.has_channel)
         self.assertFalse(org.has_msg)
+        self.assertFalse(org.has_channel_production)
 
     def test_when_adding_channel_it_returns_true(self):
-        Channel.objects.create(org=self.org, created_by=self.user, modified_by=self.user)
+        Channel.objects.create(
+            org=self.org, created_by=self.user, modified_by=self.user
+        )
 
         org = get_user_success_orgs(self.user).first()
         self.assertFalse(org.has_ia)
         self.assertFalse(org.has_flows)
         self.assertTrue(org.has_channel)
         self.assertFalse(org.has_msg)
+        self.assertTrue(org.has_channel_production)
 
 
 class RetrieveSuccessOrgTestCase(SetupMixin, TestCase):
     def test_returns_org_by_uuid(self):
         org = retrieve_success_org(str(self.org.uuid))
         self.assertEqual(org, self.org)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/success_orgs/views.py` & `weni_rp_apps-2.4.2a6/weni/success_orgs/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,21 +16,19 @@
     UserDoesNotExist,
     OrgDoesNotExist,
 )
 from .serializers import UserSuccessOrgSerializer, SuccessOrgSerializer
 
 
 class ListSuccessOrgAPIView(APIView):
-
     renderer_classes = [JSONRenderer]
     authentication_classes = []
     permission_classes = []
 
     def check_permissions(self, request):
-
         auth = get_authorization_header(request).split()
 
         if not auth:
             raise drf_exceptions.NotAuthenticated()
 
         if len(auth) == 1:
             msg = "Invalid token header. No credentials provided."
@@ -61,21 +59,19 @@
 
         serializer = UserSuccessOrgSerializer(user_sucess_orgs)
 
         return Response(serializer.data)
 
 
 class RetrieveSuccessOrgAPIView(APIView):
-
     authentication_classes = [InternalOIDCAuthentication]
     renderer_classes = [JSONRenderer]
     throttle_classes = []
 
     def get(self, request, uuid) -> Response:
-
         try:
             org = retrieve_success_org(uuid)
         except OrgDoesNotExist:
             raise Http404
         except django_exceptions.ValidationError as error:
             raise drf_exceptions.ValidationError(error.messages)
```

### Comparing `weni_rp_apps-2.4.2a5/weni/template_message/serializers.py` & `weni_rp_apps-2.4.2a6/weni/template_message/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from temba.api.v2.serializers import WriteSerializer
 from temba.channels.types.whatsapp.type import WhatsAppType
 from temba.channels.types.dialog360 import Dialog360Type
 from temba.api.v2 import fields
 
 
 class TemplateMessageSerializers(WriteSerializer):
-
     channel = fields.ChannelField()
     content = serializers.CharField()
     name = serializers.CharField(write_only=True)
     language = serializers.CharField()
     country = serializers.CharField(default=None)
     variable_count = serializers.IntegerField()
     status = serializers.CharField()
```

### Comparing `weni_rp_apps-2.4.2a5/weni/template_message/tests.py` & `weni_rp_apps-2.4.2a6/weni/template_message/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,24 @@
     CONFIG_FB_BUSINESS_ID,
     CONFIG_FB_NAMESPACE,
     CONFIG_FB_TEMPLATE_LIST_DOMAIN,
 )
 
 
 class TembaPostRequestMixin:
-
     url_namespace = None
 
     def request(self, data=None, user=None):
         url = reverse(self.url_namespace)
         token = APIToken.get_or_create(self.org, user if user else self.admin)
 
         return self.client.post(f"{url}.json", HTTP_AUTHORIZATION=f"Token {token.key}", data=data)
 
 
 class CreateTemplateMessageTest(TembaPostRequestMixin, TembaTest):
-
     url_namespace = "api.v2.template_messages"
 
     def setUp(self):
         super().setUp()
         self.wa_channel = self.create_channel(
             "WA",
             "WhatsApp: 1235",
@@ -55,15 +53,14 @@
             name="test_name",
             language="por",
             country="BR",
             status="A",
         )
 
     def test_admin_create_template(self):
-
         data = self.request_data
 
         response = self.request(data)
         template_translation = TemplateTranslation.objects.first()
 
         self.assertEquals(response.status_code, status.HTTP_201_CREATED)
         self.assertEquals(template_translation.content, data["content"])
```

### Comparing `weni_rp_apps-2.4.2a5/weni/template_message/views.py` & `weni_rp_apps-2.4.2a6/weni/template_message/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/templates/context_processors.py` & `weni_rp_apps-2.4.2a6/weni/templates/context_processors.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.conf import settings
 
 
 def enable_weni_layout(request):
-
     host = request.get_host().split(":")[0]
 
     return {"use_weni_layout": host.endswith(settings.WENI_DOMAINS["weni"])}
 
 
 def weni_announcement(request):
     return {
@@ -14,10 +13,8 @@
         "announcement_right": settings.ANNOUNCEMENT_RIGHT,
         "announcement_link": settings.ANNOUNCEMENT_LINK,
         "announcement_button": settings.ANNOUNCEMENT_BUTTON,
     }
 
 
 def hotjar(request):
-    return {
-        "hotjar_id": settings.HOTJAR_ID
-    }
+    return {"hotjar_id": settings.HOTJAR_ID}
```

### Comparing `weni_rp_apps-2.4.2a5/weni/ticketer_queues/tests.py` & `weni_rp_apps-2.4.2a6/weni/ticketer_queues/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/ticketer_queues/views.py` & `weni_rp_apps-2.4.2a6/weni/ticketer_queues/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a5/weni/utils/app_config.py` & `weni_rp_apps-2.4.2a6/weni/utils/app_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def update_urlpatterns(app_urls, urls_module="temba.api.v2.urls"):
     def context_data(cls, **kwargs):
         ctx = context_func(cls, **kwargs)
         added = []
         for url in app_urls:
             if isinstance(url, URLPattern):
-                if hasattr(url.callback, 'view_class'):
+                if hasattr(url.callback, "view_class"):
                     view = url.callback.view_class
                 else:
                     view = url.callback
                 view_id = id(view)
                 if view_id not in added and hasattr(view, "get_read_explorer"):
                     ctx["endpoints"].append(view.get_read_explorer())
                     added.append(view_id)
```

### Comparing `weni_rp_apps-2.4.2a5/PKG-INFO` & `weni_rp_apps-2.4.2a6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weni-rp-apps
-Version: 2.4.2a5
+Version: 2.4.2a6
 Summary: Weni apps for Rapidpro Platform
 License: AGPL-3.0
 Author: jcbalmeida
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

