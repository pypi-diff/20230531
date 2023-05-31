# Comparing `tmp/tautulli-3.2.1.2120.tar.gz` & `tmp/tautulli-3.3.0.2120.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tautulli-3.2.1.2120.tar", last modified: Fri Apr 14 21:34:44 2023, max compression
+gzip compressed data, was "tautulli-3.3.0.2120.tar", last modified: Wed May 31 00:22:16 2023, max compression
```

## Comparing `tautulli-3.2.1.2120.tar` & `tautulli-3.3.0.2120.tar`

### file list

```diff
@@ -1,92 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:44.025164 tautulli-3.2.1.2120/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-14 21:34:44.025164 tautulli-3.2.1.2120/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 21:34:44.025164 tautulli-3.2.1.2120/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-14 21:34:22.000000 tautulli-3.2.1.2120/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:44.013164 tautulli-3.2.1.2120/tautulli/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/API_VERSIONS.json
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/PYTHON_VERSIONS.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:44.013164 tautulli-3.2.1.2120/tautulli/api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    96367 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/api/json_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    66863 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/api/object_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:44.013164 tautulli-3.2.1.2120/tautulli/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/internal/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:44.025164 tautulli-3.2.1.2120/tautulli/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/children_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/collections_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/date_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/export_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/exports_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/geo_ip_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/get_plays_or_stream_types_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/home_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/item_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/item_watch_time_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/libraries_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/library_media_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/library_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/library_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/library_watch_time_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/new_rating_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/newsletter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/newsletter_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/newsletter_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/notification_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/notifier_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/notifier_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/notifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/old_rating_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/playlists_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/plex_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/pms_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/recently_added.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/registered_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/search_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/server_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/server_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/server_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/server_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/server_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/servers_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    25625 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/stream_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/synced_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/tautulli_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/update_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/user_ips.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/user_logins.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/user_player_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/user_watch_time_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/usernames.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/users_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/models/whois_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:44.025164 tautulli-3.2.1.2120/tautulli/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/tools/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-14 21:34:21.000000 tautulli-3.2.1.2120/tautulli/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:44.013164 tautulli-3.2.1.2120/tautulli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-14 21:34:43.000000 tautulli-3.2.1.2120/tautulli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-14 21:34:43.000000 tautulli-3.2.1.2120/tautulli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:34:43.000000 tautulli-3.2.1.2120/tautulli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-14 21:34:43.000000 tautulli-3.2.1.2120/tautulli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 21:34:43.000000 tautulli-3.2.1.2120/tautulli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:22:16.404820 tautulli-3.3.0.2120/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-31 00:22:16.404820 tautulli-3.3.0.2120/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 00:22:16.404820 tautulli-3.3.0.2120/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-31 00:21:54.000000 tautulli-3.3.0.2120/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:22:16.396820 tautulli-3.3.0.2120/tautulli/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/API_VERSIONS.json
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/PYTHON_VERSIONS.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:22:16.396820 tautulli-3.3.0.2120/tautulli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96289 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/api/json_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66833 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/api/object_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:22:16.396820 tautulli-3.3.0.2120/tautulli/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/internal/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:22:16.404820 tautulli-3.3.0.2120/tautulli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/children_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/collections_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/date_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/export_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/exports_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/geo_ip_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/get_plays_or_stream_types_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/home_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/item_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/item_watch_time_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/libraries_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/library_media_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/library_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/library_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/library_watch_time_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/new_rating_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/newsletter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/newsletter_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/newsletter_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/newsletter_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/notification_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/notifier_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/notifier_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/old_rating_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/playlists_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/plex_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/pms_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/recently_added.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/registered_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/search_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/server_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/server_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/server_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/server_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/server_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/servers_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25625 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/stream_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/synced_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/tautulli_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/update_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/user_ips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/user_logins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/user_player_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/user_watch_time_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/usernames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/users_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/models/whois_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:22:16.404820 tautulli-3.3.0.2120/tautulli/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/tools/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-31 00:21:53.000000 tautulli-3.3.0.2120/tautulli/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:22:16.396820 tautulli-3.3.0.2120/tautulli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-31 00:22:16.000000 tautulli-3.3.0.2120/tautulli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-31 00:22:16.000000 tautulli-3.3.0.2120/tautulli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:22:16.000000 tautulli-3.3.0.2120/tautulli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 00:22:16.000000 tautulli-3.3.0.2120/tautulli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 00:22:16.000000 tautulli-3.3.0.2120/tautulli.egg-info/top_level.txt
```

### Comparing `tautulli-3.2.1.2120/LICENSE` & `tautulli-3.3.0.2120/LICENSE`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/PKG-INFO` & `tautulli-3.3.0.2120/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tautulli
-Version: 3.2.1.2120
+Version: 3.3.0.2120
 Summary: A complete Python client for Tautulli's API
 Home-page: https://github.com/nwithan8/pytulli
 Author: Nate Harris
 Author-email: n8gr8gbln@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/3.2.1.2120.tar.gz
+Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/3.3.0.2120.tar.gz
 Description: # A Python client for Tautulli's API
         [![PyPi](https://img.shields.io/pypi/dm/tautulli?label=Downloads&logo=pypi)](https://pypi.org/project/tautulli)
         [![License](https://img.shields.io/pypi/l/tautulli?color=orange&style=flat-square)](https://github.com/nwithan8/pytulli/blob/master/LICENSE)
         
         [![Open Issues](https://img.shields.io/github/issues-raw/nwithan8/pytulli?color=gold&style=flat-square)](https://github.com/nwithan8/pytulli/issues?q=is%3Aopen+is%3Aissue)
         [![Closed Issues](https://img.shields.io/github/issues-closed-raw/nwithan8/pytulli?color=black&style=flat-square)](https://github.com/nwithan8/pytulli/issues?q=is%3Aissue+is%3Aclosed)
         [![Latest Release](https://img.shields.io/github/v/release/nwithan8/pytulli?color=red&label=latest%20release&logo=github&style=flat-square)](https://github.com/nwithan8/pytulli/releases)
```

### Comparing `tautulli-3.2.1.2120/README.md` & `tautulli-3.3.0.2120/README.md`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/setup.py` & `tautulli-3.3.0.2120/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 from typing import List
 
 import setuptools
 
-__version__ = '3.2.1.2120'
+__version__ = '3.3.0.2120'
 
 __title__ = "tautulli"
 __author__ = 'Nate Harris'
 __author_email__ = 'n8gr8gbln@gmail.com'
 __github_username__ = "nwithan8"
 __github_repo__ = "pytulli"
 __copyright__ = "Copyright © 2023 - Nate Harris"
```

### Comparing `tautulli-3.2.1.2120/tautulli/api/json_api.py` & `tautulli-3.3.0.2120/tautulli/api/json_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2017,53 +2017,53 @@
         :param row_ids: List of row IDS to sign out
         :type row_ids: list[int], optional
         :returns: `True` if successful, `False` if unsuccessful
         :rtype: bool
         """
         return 'logout_user_session', {'row_ids': int_list_to_string(int_list=row_ids)}
 
-    @set_and_forget
-    def notify(self, notifier_id: int, subject: str, body: str, headers: str = None, script_args: str = None) -> bool:
+    @raw_json
+    def notify(self, notifier_id: int, subject: str, body: str, headers: str = None, script_args: str = None) -> dict:
         """
         Send a notification using Tautulli
 
         :param notifier_id: ID of the notification agent
         :type notifier_id: int
         :param subject: Subject of the message
         :type subject: str
         :param body: Body of the message
         :type body: str
         :param headers: JSON headers for webhook notifications
         :type headers: str, optional
         :param script_args: Arguments for script notifications
         :type script_args: str, optional
-        :returns: `True` if successful, `False` if unsuccessful
-        :rtype: bool
+        :returns: Dict of data
+        :rtype: dict
         """
         params = build_optional_params(headers=headers, script_args=script_args)
         params['notifier_id'] = notifier_id
         params['subject'] = subject
         params['body'] = body
         return 'notify', params
 
-    @set_and_forget
-    def notify_newsletter(self, newsletter_id: int, subject: str = None, body: str = None, message: str = None) -> bool:
+    @raw_json
+    def notify_newsletter(self, newsletter_id: int, subject: str = None, body: str = None, message: str = None) -> dict:
         """
         Send a newsletter using Tautulli
 
         :param newsletter_id: ID of the newsletter agent
         :type newsletter_id: int
         :param subject: Subject of the newsletter
         :type subject: str, optional
         :param body: Body of the newsletter
         :type body: str, optional
         :param message: Message of the newsletter
         :type message: str, optional
-        :returns: `True` if successful, `False` if unsuccessful
-        :rtype: bool
+        :returns: Dict of data
+        :rtype: dict
         """
         params = build_optional_params(subject=subject, body=body, message=message)
         params['newsletter_id'] = newsletter_id
         return 'notify_newsletter', params
 
     @set_and_forget
     def notify_recently_added(self, rating_key: int, notifier_id: int = None) -> bool:
```

### Comparing `tautulli-3.2.1.2120/tautulli/api/object_api.py` & `tautulli-3.3.0.2120/tautulli/api/object_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1568,51 +1568,51 @@
         :param row_ids: List of row IDS to sign out
         :type row_ids: list[int], optional
         :returns: `True` if successful, `False` if unsuccessful
         :rtype: bool
         """
         return False
 
-    @raw_api_bool
-    def notify(self, notifier_id: int, subject: str, body: str, headers: str = None, script_args: str = None) -> bool:
+    @make_object
+    def notify(self, notifier_id: int, subject: str, body: str, headers: str = None, script_args: str = None) -> Notification:
         """
         Send a notification using Tautulli
 
         :param notifier_id: ID of the notification agent
         :type notifier_id: int
         :param subject: Subject of the message
         :type subject: str
         :param body: Body of the message
         :type body: str
         :param headers: JSON headers for webhook notifications
         :type headers: str, optional
         :param script_args: Arguments for script notifications
         :type script_args: str, optional
-        :returns: `True` if successful, `False` if unsuccessful
-        :rtype: bool
+        :returns: Notification object
+
         """
-        return False
+        return 'Notification'
 
-    @raw_api_bool
-    def notify_newsletter(self, newsletter_id: int, subject: str = None, body: str = None, message: str = None) -> bool:
+    @make_object
+    def notify_newsletter(self, newsletter_id: int, subject: str = None, body: str = None, message: str = None) -> NewsletterNotification:
         """
         Send a newsletter using Tautulli
 
         :param newsletter_id: ID of the newsletter agent
         :type newsletter_id: int
         :param subject: Subject of the newsletter
         :type subject: str, optional
         :param body: Body of the newsletter
         :type body: str, optional
         :param message: Message of the newsletter
         :type message: str, optional
-        :returns: `True` if successful, `False` if unsuccessful
-        :rtype: bool
+        :returns: NewsletterNotification object
+
         """
-        return False
+        return 'NewsletterNotification'
 
     @raw_api_bool
     def notify_recently_added(self, rating_key: int, notifier_id: int = None) -> bool:
         """
         Send a recently added notification using Tautulli
 
         :param rating_key: Rating key for the media item
```

### Comparing `tautulli-3.2.1.2120/tautulli/internal/decorators.py` & `tautulli-3.3.0.2120/tautulli/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/internal/static.py` & `tautulli-3.3.0.2120/tautulli/internal/static.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/internal/utils.py` & `tautulli-3.3.0.2120/tautulli/internal/utils.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/__init__.py` & `tautulli-3.3.0.2120/tautulli/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from tautulli.models.item_user_stats import ItemUserStat
 from tautulli.models.item_watch_time_stats import ItemWatchTimeStat
 from tautulli.models.get_plays_or_stream_types_by import PlaysOrStreamTypesBy
 from tautulli.models.metadata import Metadata
 from tautulli.models.new_rating_keys import NewRatingKeys
 from tautulli.models.newsletter_config import NewsletterConfig
 from tautulli.models.newsletter_log import NewsletterLog
+from tautulli.models.newsletter_notification import NewsletterNotification
+from tautulli.models.notification import Notification
 from tautulli.models.notification_log import NotificationLog
 from tautulli.models.notifier_config import NotifierConfig
 from tautulli.models.notifiers import Notifier
 from tautulli.models.old_rating_keys import OldRatingKeys
 from tautulli.models.playlists_table import PlaylistsTable
 from tautulli.models.plex_log import PlexLog
 from tautulli.models.recently_added import RecentlyAdded
```

### Comparing `tautulli-3.2.1.2120/tautulli/models/activity.py` & `tautulli-3.3.0.2120/tautulli/models/activity.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/children_metadata.py` & `tautulli-3.3.0.2120/tautulli/models/children_metadata.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/collections_table.py` & `tautulli-3.3.0.2120/tautulli/models/collections_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/docs.py` & `tautulli-3.3.0.2120/tautulli/models/docs.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/export_fields.py` & `tautulli-3.3.0.2120/tautulli/models/export_fields.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/exports_table.py` & `tautulli-3.3.0.2120/tautulli/models/exports_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/geo_ip_lookup.py` & `tautulli-3.3.0.2120/tautulli/models/geo_ip_lookup.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/get_plays_or_stream_types_by.py` & `tautulli-3.3.0.2120/tautulli/models/get_plays_or_stream_types_by.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/history.py` & `tautulli-3.3.0.2120/tautulli/models/history.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/home_stats.py` & `tautulli-3.3.0.2120/tautulli/models/home_stats.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/item_user_stats.py` & `tautulli-3.3.0.2120/tautulli/models/item_user_stats.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/libraries.py` & `tautulli-3.3.0.2120/tautulli/models/libraries.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/libraries_table.py` & `tautulli-3.3.0.2120/tautulli/models/libraries_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/library.py` & `tautulli-3.3.0.2120/tautulli/models/library.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/library_media_info.py` & `tautulli-3.3.0.2120/tautulli/models/library_media_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/library_user_stats.py` & `tautulli-3.3.0.2120/tautulli/models/library_user_stats.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/metadata.py` & `tautulli-3.3.0.2120/tautulli/models/metadata.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/newsletter.py` & `tautulli-3.3.0.2120/tautulli/models/newsletter.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/newsletter_config.py` & `tautulli-3.3.0.2120/tautulli/models/newsletter_config.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/newsletter_log.py` & `tautulli-3.3.0.2120/tautulli/models/newsletter_log.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/notification_log.py` & `tautulli-3.3.0.2120/tautulli/models/notification_log.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/notifier_config.py` & `tautulli-3.3.0.2120/tautulli/models/notifier_config.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/notifiers.py` & `tautulli-3.3.0.2120/tautulli/models/notifiers.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/parser.py` & `tautulli-3.3.0.2120/tautulli/models/parser.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/playlists_table.py` & `tautulli-3.3.0.2120/tautulli/models/playlists_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/pms_update.py` & `tautulli-3.3.0.2120/tautulli/models/pms_update.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/registered_device.py` & `tautulli-3.3.0.2120/tautulli/models/registered_device.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/search_results.py` & `tautulli-3.3.0.2120/tautulli/models/search_results.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/server_info.py` & `tautulli-3.3.0.2120/tautulli/models/server_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/server_list.py` & `tautulli-3.3.0.2120/tautulli/models/server_list.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/servers_info.py` & `tautulli-3.3.0.2120/tautulli/models/servers_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/settings.py` & `tautulli-3.3.0.2120/tautulli/models/settings.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/stream_data.py` & `tautulli-3.3.0.2120/tautulli/models/stream_data.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/synced_items.py` & `tautulli-3.3.0.2120/tautulli/models/synced_items.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/tautulli_info.py` & `tautulli-3.3.0.2120/tautulli/models/tautulli_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/user.py` & `tautulli-3.3.0.2120/tautulli/models/user.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/user_ips.py` & `tautulli-3.3.0.2120/tautulli/models/user_ips.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/user_logins.py` & `tautulli-3.3.0.2120/tautulli/models/user_logins.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/user_player_stats.py` & `tautulli-3.3.0.2120/tautulli/models/user_player_stats.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/users.py` & `tautulli-3.3.0.2120/tautulli/models/users.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/users_table.py` & `tautulli-3.3.0.2120/tautulli/models/users_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/models/whois_lookup.py` & `tautulli-3.3.0.2120/tautulli/models/whois_lookup.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/tools/api_helper.py` & `tautulli-3.3.0.2120/tautulli/tools/api_helper.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli/tools/utils.py` & `tautulli-3.3.0.2120/tautulli/tools/utils.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.2.1.2120/tautulli.egg-info/PKG-INFO` & `tautulli-3.3.0.2120/tautulli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tautulli
-Version: 3.2.1.2120
+Version: 3.3.0.2120
 Summary: A complete Python client for Tautulli's API
 Home-page: https://github.com/nwithan8/pytulli
 Author: Nate Harris
 Author-email: n8gr8gbln@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/3.2.1.2120.tar.gz
+Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/3.3.0.2120.tar.gz
 Description: # A Python client for Tautulli's API
         [![PyPi](https://img.shields.io/pypi/dm/tautulli?label=Downloads&logo=pypi)](https://pypi.org/project/tautulli)
         [![License](https://img.shields.io/pypi/l/tautulli?color=orange&style=flat-square)](https://github.com/nwithan8/pytulli/blob/master/LICENSE)
         
         [![Open Issues](https://img.shields.io/github/issues-raw/nwithan8/pytulli?color=gold&style=flat-square)](https://github.com/nwithan8/pytulli/issues?q=is%3Aopen+is%3Aissue)
         [![Closed Issues](https://img.shields.io/github/issues-closed-raw/nwithan8/pytulli?color=black&style=flat-square)](https://github.com/nwithan8/pytulli/issues?q=is%3Aissue+is%3Aclosed)
         [![Latest Release](https://img.shields.io/github/v/release/nwithan8/pytulli?color=red&label=latest%20release&logo=github&style=flat-square)](https://github.com/nwithan8/pytulli/releases)
```

### Comparing `tautulli-3.2.1.2120/tautulli.egg-info/SOURCES.txt` & `tautulli-3.3.0.2120/tautulli.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 tautulli/models/library_watch_time_stats.py
 tautulli/models/logs.py
 tautulli/models/metadata.py
 tautulli/models/new_rating_keys.py
 tautulli/models/newsletter.py
 tautulli/models/newsletter_config.py
 tautulli/models/newsletter_log.py
+tautulli/models/newsletter_notification.py
+tautulli/models/notification.py
 tautulli/models/notification_log.py
 tautulli/models/notifier_config.py
 tautulli/models/notifier_parameters.py
 tautulli/models/notifiers.py
 tautulli/models/old_rating_keys.py
 tautulli/models/parser.py
 tautulli/models/playlists_table.py
```

