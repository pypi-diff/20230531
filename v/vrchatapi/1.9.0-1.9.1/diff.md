# Comparing `tmp/vrchatapi-1.9.0.tar.gz` & `tmp/vrchatapi-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vrchatapi-1.9.0.tar", last modified: Thu Nov 17 21:22:06 2022, max compression
+gzip compressed data, was "vrchatapi-1.9.1.tar", last modified: Thu Nov 17 23:01:09 2022, max compression
```

## Comparing `vrchatapi-1.9.0.tar` & `vrchatapi-1.9.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:22:06.079524 vrchatapi-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-11-17 21:21:39.000000 vrchatapi-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3673 2022-11-17 21:22:06.079524 vrchatapi-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-11-17 21:21:39.000000 vrchatapi-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-17 21:21:39.000000 vrchatapi-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-17 21:22:06.079524 vrchatapi-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     7646 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:22:06.067524 vrchatapi-1.9.0/vrchatapi/
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:22:06.067524 vrchatapi-1.9.0/vrchatapi/api/
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31253 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    48252 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/avatars_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    20729 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/economy_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    39642 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/favorites_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    51726 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/files_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    22353 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/friends_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    18684 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/instances_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    42170 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/invite_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    23064 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     8891 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    26335 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/playermoderation_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    29660 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    18949 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    74752 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api/worlds_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    36971 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:22:06.067524 vrchatapi-1.9.0/vrchatapi/apis/
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18538 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     5011 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:22:06.075523 vrchatapi-1.9.0/vrchatapi/model/
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12150 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/add_favorite_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    53449 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/api_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    14419 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/api_event_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    11721 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/api_health.py
--rw-r--r--   0 runner    (1001) docker     (121)    18202 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/avatar.py
--rw-r--r--   0 runner    (1001) docker     (121)    11338 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/avatar_id.py
--rw-r--r--   0 runner    (1001) docker     (121)    11076 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/avatar_unity_package_url_object.py
--rw-r--r--   0 runner    (1001) docker     (121)    13455 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/create_avatar_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12059 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/create_file_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12129 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/create_file_version_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    15605 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/create_world_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    27202 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/current_user.py
--rw-r--r--   0 runner    (1001) docker     (121)    12375 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/deployment_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    12033 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/developer_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    11960 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/download_url_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    13466 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/dynamic_content_row.py
--rw-r--r--   0 runner    (1001) docker     (121)    11118 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/error.py
--rw-r--r--   0 runner    (1001) docker     (121)    12095 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/favorite.py
--rw-r--r--   0 runner    (1001) docker     (121)    13856 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/favorite_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    11359 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/favorite_group_id.py
--rw-r--r--   0 runner    (1001) docker     (121)    11325 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/favorite_group_visibility.py
--rw-r--r--   0 runner    (1001) docker     (121)    11344 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/favorite_id.py
--rw-r--r--   0 runner    (1001) docker     (121)    11268 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/favorite_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    13302 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/file.py
--rw-r--r--   0 runner    (1001) docker     (121)    13490 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/file_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    11332 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/file_id.py
--rw-r--r--   0 runner    (1001) docker     (121)    11352 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/file_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    11062 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/file_upload_url.py
--rw-r--r--   0 runner    (1001) docker     (121)    13076 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/file_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    13150 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/file_version_upload_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    12640 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/finish_file_data_upload_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12175 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/friend_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    14018 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/info_push.py
--rw-r--r--   0 runner    (1001) docker     (121)    13130 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/info_push_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    11300 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/info_push_data_article.py
--rw-r--r--   0 runner    (1001) docker     (121)    11679 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/info_push_data_article_content.py
--rw-r--r--   0 runner    (1001) docker     (121)    11669 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/info_push_data_clickable.py
--rw-r--r--   0 runner    (1001) docker     (121)    19486 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/instance.py
--rw-r--r--   0 runner    (1001) docker     (121)    11960 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/instance_id.py
--rw-r--r--   0 runner    (1001) docker     (121)    11543 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/instance_platforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    11467 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/instance_short_name_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    11642 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/instance_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    13783 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/invite_message.py
--rw-r--r--   0 runner    (1001) docker     (121)    11359 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/invite_message_id.py
--rw-r--r--   0 runner    (1001) docker     (121)    11445 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/invite_message_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    11600 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/invite_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    11228 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/invite_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12570 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/license.py
--rw-r--r--   0 runner    (1001) docker     (121)    11169 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/license_action.py
--rw-r--r--   0 runner    (1001) docker     (121)    12051 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/license_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/license_group_id.py
--rw-r--r--   0 runner    (1001) docker     (121)    11433 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/license_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    11799 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/limited_unity_package.py
--rw-r--r--   0 runner    (1001) docker     (121)    17248 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/limited_user.py
--rw-r--r--   0 runner    (1001) docker     (121)    18293 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/limited_world.py
--rw-r--r--   0 runner    (1001) docker     (121)    12858 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/mime_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    11583 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/moderate_user_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    14284 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/notification.py
--rw-r--r--   0 runner    (1001) docker     (121)    11790 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/notification_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    11446 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/past_display_name.py
--rw-r--r--   0 runner    (1001) docker     (121)    12389 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/permission_id.py
--rw-r--r--   0 runner    (1001) docker     (121)    14012 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/player_moderation.py
--rw-r--r--   0 runner    (1001) docker     (121)    11368 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/player_moderation_id.py
--rw-r--r--   0 runner    (1001) docker     (121)    11556 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/player_moderation_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    11412 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/public_announcement.py
--rw-r--r--   0 runner    (1001) docker     (121)    11426 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/region.py
--rw-r--r--   0 runner    (1001) docker     (121)    11283 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/release_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    11144 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/request_invite_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    11409 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/response.py
--rw-r--r--   0 runner    (1001) docker     (121)    14641 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/sent_notification.py
--rw-r--r--   0 runner    (1001) docker     (121)    12534 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/subscription.py
--rw-r--r--   0 runner    (1001) docker     (121)    11370 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/subscription_period.py
--rw-r--r--   0 runner    (1001) docker     (121)    11134 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/success.py
--rw-r--r--   0 runner    (1001) docker     (121)    13088 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (121)    13843 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/transaction.py
--rw-r--r--   0 runner    (1001) docker     (121)    16108 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/transaction_agreement.py
--rw-r--r--   0 runner    (1001) docker     (121)    11353 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/transaction_id.py
--rw-r--r--   0 runner    (1001) docker     (121)    11391 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/transaction_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    12731 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/transaction_steam_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    12202 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/transaction_steam_wallet_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    11025 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/two_factor_auth_code.py
--rw-r--r--   0 runner    (1001) docker     (121)    14582 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/unity_package.py
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/unity_package_id.py
--rw-r--r--   0 runner    (1001) docker     (121)    13371 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/update_avatar_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    11885 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/update_favorite_group_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    11085 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/update_invite_message_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    13099 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/update_user_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    15208 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/update_world_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    21711 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/user.py
--rw-r--r--   0 runner    (1001) docker     (121)    11339 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/user_exists.py
--rw-r--r--   0 runner    (1001) docker     (121)    12017 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/user_state.py
--rw-r--r--   0 runner    (1001) docker     (121)    12102 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/user_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    15665 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/user_subscription.py
--rw-r--r--   0 runner    (1001) docker     (121)    11066 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/verify2_fa_result.py
--rw-r--r--   0 runner    (1001) docker     (121)    11281 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/verify_auth_token_result.py
--rw-r--r--   0 runner    (1001) docker     (121)    21738 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/world.py
--rw-r--r--   0 runner    (1001) docker     (121)    11655 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/world_id.py
--rw-r--r--   0 runner    (1001) docker     (121)    11286 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/world_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    10976 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model/world_publish_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    81828 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:22:06.075523 vrchatapi-1.9.0/vrchatapi/models/
--rw-r--r--   0 runner    (1001) docker     (121)     6351 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13463 2022-11-17 21:21:54.000000 vrchatapi-1.9.0/vrchatapi/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:22:06.067524 vrchatapi-1.9.0/vrchatapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3673 2022-11-17 21:22:06.000000 vrchatapi-1.9.0/vrchatapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-11-17 21:22:06.000000 vrchatapi-1.9.0/vrchatapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 21:22:06.000000 vrchatapi-1.9.0/vrchatapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-17 21:22:06.000000 vrchatapi-1.9.0/vrchatapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-17 21:22:06.000000 vrchatapi-1.9.0/vrchatapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 23:01:09.368363 vrchatapi-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2022-11-17 23:00:38.000000 vrchatapi-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3673 2022-11-17 23:01:09.368363 vrchatapi-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3333 2022-11-17 23:00:38.000000 vrchatapi-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2022-11-17 23:00:38.000000 vrchatapi-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2022-11-17 23:01:09.368363 vrchatapi-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     7646 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 23:01:09.344363 vrchatapi-1.9.1/vrchatapi/
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 23:01:09.348363 vrchatapi-1.9.1/vrchatapi/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31253 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48252 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/avatars_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20729 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/economy_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39642 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/favorites_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51726 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/files_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22353 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/friends_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18684 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42170 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/invite_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23064 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8891 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26335 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/playermoderation_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29660 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18949 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    74752 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api/worlds_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36971 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 23:01:09.348363 vrchatapi-1.9.1/vrchatapi/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18538 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5011 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 23:01:09.368363 vrchatapi-1.9.1/vrchatapi/model/
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12150 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/add_favorite_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53449 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14419 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/api_event_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11721 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/api_health.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18202 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/avatar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11338 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/avatar_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11076 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/avatar_unity_package_url_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13455 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/create_avatar_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12059 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/create_file_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12129 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/create_file_version_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15605 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/create_world_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27202 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/current_user.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12375 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/deployment_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12033 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/developer_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11960 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/download_url_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13466 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/dynamic_content_row.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11118 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12095 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/favorite.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13856 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/favorite_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11359 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/favorite_group_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11325 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/favorite_group_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11344 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/favorite_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11268 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/favorite_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13302 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13490 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/file_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11332 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11352 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/file_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11062 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/file_upload_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13076 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/file_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13150 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/file_version_upload_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12640 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/finish_file_data_upload_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12175 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/friend_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14018 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/info_push.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13130 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/info_push_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11300 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/info_push_data_article.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11679 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/info_push_data_article_content.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11669 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/info_push_data_clickable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19486 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/instance.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11960 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/instance_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11543 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/instance_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11467 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/instance_short_name_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11642 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13783 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/invite_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11359 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/invite_message_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11445 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/invite_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11600 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/invite_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/invite_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12570 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/license.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11169 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/license_action.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12051 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/license_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11356 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/license_group_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11433 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/license_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11799 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/limited_unity_package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17248 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/limited_user.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18293 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/limited_world.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12858 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/mime_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11583 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/moderate_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14284 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/notification.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11790 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11446 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/past_display_name.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12389 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/permission_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14012 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/player_moderation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11368 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/player_moderation_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11556 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/player_moderation_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11412 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/public_announcement.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11426 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/region.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11283 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/release_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11144 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/request_invite_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11409 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14641 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/sent_notification.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12534 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11370 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/subscription_period.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11134 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/success.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13088 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13843 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16108 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/transaction_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11353 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/transaction_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11391 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/transaction_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12731 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/transaction_steam_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12202 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/transaction_steam_wallet_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11025 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/two_factor_auth_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/unity_package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11356 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/unity_package_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13371 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/update_avatar_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11885 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/update_favorite_group_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11085 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/update_invite_message_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13099 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/update_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15208 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/update_world_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21597 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11339 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/user_exists.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12017 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/user_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12102 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/user_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15665 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/user_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11066 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/verify2_fa_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11281 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/verify_auth_token_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21738 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/world.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11655 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/world_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11286 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/world_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10976 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model/world_publish_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    81828 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 23:01:09.368363 vrchatapi-1.9.1/vrchatapi/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     6351 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13463 2022-11-17 23:00:53.000000 vrchatapi-1.9.1/vrchatapi/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 23:01:09.344363 vrchatapi-1.9.1/vrchatapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3673 2022-11-17 23:01:09.000000 vrchatapi-1.9.1/vrchatapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4454 2022-11-17 23:01:09.000000 vrchatapi-1.9.1/vrchatapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-17 23:01:09.000000 vrchatapi-1.9.1/vrchatapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2022-11-17 23:01:09.000000 vrchatapi-1.9.1/vrchatapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2022-11-17 23:01:09.000000 vrchatapi-1.9.1/vrchatapi.egg-info/top_level.txt
```

### Comparing `vrchatapi-1.9.0/LICENSE` & `vrchatapi-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vrchatapi-1.9.0/PKG-INFO` & `vrchatapi-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vrchatapi
-Version: 1.9.0
+Version: 1.9.1
 Summary: VRChat API Library for Python
 Home-page: 
 Author: Unofficial VRChat API Documentation Project
 Author-email: me@ariesclark.com
 License: The MIT License (MIT)
 Keywords: vrchat,vrchatapi,vrc
 Requires-Python: >=3.6
```

### Comparing `vrchatapi-1.9.0/README.md` & `vrchatapi-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `vrchatapi-1.9.0/setup.py` & `vrchatapi-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,24 +70,24 @@
 
 ## Contributing
 
 Contributions are welcome, but do not add features that should be handled by the OpenAPI specification.
 
 Join the [Discord server](https://discord.gg/Ge2APMhPfD) to get in touch with us.
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "vrchatapi"
-VERSION = "1.9.0"
+VERSION = "1.9.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `vrchatapi-1.9.0/vrchatapi/__init__.py` & `vrchatapi-1.9.1/vrchatapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # flake8: noqa
 
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/authentication_api.py` & `vrchatapi-1.9.1/vrchatapi/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/avatars_api.py` & `vrchatapi-1.9.1/vrchatapi/api/avatars_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/economy_api.py` & `vrchatapi-1.9.1/vrchatapi/api/economy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/favorites_api.py` & `vrchatapi-1.9.1/vrchatapi/api/favorites_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/files_api.py` & `vrchatapi-1.9.1/vrchatapi/api/files_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/friends_api.py` & `vrchatapi-1.9.1/vrchatapi/api/friends_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/instances_api.py` & `vrchatapi-1.9.1/vrchatapi/api/instances_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/invite_api.py` & `vrchatapi-1.9.1/vrchatapi/api/invite_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/notifications_api.py` & `vrchatapi-1.9.1/vrchatapi/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/permissions_api.py` & `vrchatapi-1.9.1/vrchatapi/api/permissions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/playermoderation_api.py` & `vrchatapi-1.9.1/vrchatapi/api/playermoderation_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/system_api.py` & `vrchatapi-1.9.1/vrchatapi/api/system_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/users_api.py` & `vrchatapi-1.9.1/vrchatapi/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api/worlds_api.py` & `vrchatapi-1.9.1/vrchatapi/api/worlds_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/api_client.py` & `vrchatapi-1.9.1/vrchatapi/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
```

### Comparing `vrchatapi-1.9.0/vrchatapi/apis/__init__.py` & `vrchatapi-1.9.1/vrchatapi/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `vrchatapi-1.9.0/vrchatapi/configuration.py` & `vrchatapi-1.9.1/vrchatapi/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -451,15 +451,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.9.0\n"\
+               "Version of the API: 1.9.1\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `vrchatapi-1.9.0/vrchatapi/exceptions.py` & `vrchatapi-1.9.1/vrchatapi/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/add_favorite_request.py` & `vrchatapi-1.9.1/vrchatapi/model/add_favorite_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/api_config.py` & `vrchatapi-1.9.1/vrchatapi/model/api_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/api_event_config.py` & `vrchatapi-1.9.1/vrchatapi/model/api_event_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/api_health.py` & `vrchatapi-1.9.1/vrchatapi/model/api_health.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/avatar.py` & `vrchatapi-1.9.1/vrchatapi/model/avatar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/avatar_id.py` & `vrchatapi-1.9.1/vrchatapi/model/avatar_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/avatar_unity_package_url_object.py` & `vrchatapi-1.9.1/vrchatapi/model/avatar_unity_package_url_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/create_avatar_request.py` & `vrchatapi-1.9.1/vrchatapi/model/create_avatar_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/create_file_request.py` & `vrchatapi-1.9.1/vrchatapi/model/create_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/create_file_version_request.py` & `vrchatapi-1.9.1/vrchatapi/model/create_file_version_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/create_world_request.py` & `vrchatapi-1.9.1/vrchatapi/model/create_world_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/current_user.py` & `vrchatapi-1.9.1/vrchatapi/model/current_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/deployment_group.py` & `vrchatapi-1.9.1/vrchatapi/model/deployment_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/developer_type.py` & `vrchatapi-1.9.1/vrchatapi/model/developer_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/download_url_list.py` & `vrchatapi-1.9.1/vrchatapi/model/download_url_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/dynamic_content_row.py` & `vrchatapi-1.9.1/vrchatapi/model/dynamic_content_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/error.py` & `vrchatapi-1.9.1/vrchatapi/model/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/favorite.py` & `vrchatapi-1.9.1/vrchatapi/model/favorite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/favorite_group.py` & `vrchatapi-1.9.1/vrchatapi/model/favorite_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/favorite_group_id.py` & `vrchatapi-1.9.1/vrchatapi/model/favorite_group_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/favorite_group_visibility.py` & `vrchatapi-1.9.1/vrchatapi/model/favorite_group_visibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/favorite_id.py` & `vrchatapi-1.9.1/vrchatapi/model/favorite_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/favorite_type.py` & `vrchatapi-1.9.1/vrchatapi/model/favorite_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/file.py` & `vrchatapi-1.9.1/vrchatapi/model/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/file_data.py` & `vrchatapi-1.9.1/vrchatapi/model/file_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/file_id.py` & `vrchatapi-1.9.1/vrchatapi/model/file_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/file_status.py` & `vrchatapi-1.9.1/vrchatapi/model/file_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/file_upload_url.py` & `vrchatapi-1.9.1/vrchatapi/model/file_upload_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/file_version.py` & `vrchatapi-1.9.1/vrchatapi/model/file_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/file_version_upload_status.py` & `vrchatapi-1.9.1/vrchatapi/model/file_version_upload_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/finish_file_data_upload_request.py` & `vrchatapi-1.9.1/vrchatapi/model/finish_file_data_upload_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/friend_status.py` & `vrchatapi-1.9.1/vrchatapi/model/friend_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/info_push.py` & `vrchatapi-1.9.1/vrchatapi/model/info_push.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/info_push_data.py` & `vrchatapi-1.9.1/vrchatapi/model/info_push_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/info_push_data_article.py` & `vrchatapi-1.9.1/vrchatapi/model/info_push_data_article.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/info_push_data_article_content.py` & `vrchatapi-1.9.1/vrchatapi/model/info_push_data_article_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/info_push_data_clickable.py` & `vrchatapi-1.9.1/vrchatapi/model/info_push_data_clickable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/instance.py` & `vrchatapi-1.9.1/vrchatapi/model/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/instance_id.py` & `vrchatapi-1.9.1/vrchatapi/model/instance_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/instance_platforms.py` & `vrchatapi-1.9.1/vrchatapi/model/instance_platforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/instance_short_name_response.py` & `vrchatapi-1.9.1/vrchatapi/model/instance_short_name_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/instance_type.py` & `vrchatapi-1.9.1/vrchatapi/model/instance_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/invite_message.py` & `vrchatapi-1.9.1/vrchatapi/model/invite_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/invite_message_id.py` & `vrchatapi-1.9.1/vrchatapi/model/invite_message_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/invite_message_type.py` & `vrchatapi-1.9.1/vrchatapi/model/invite_message_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/invite_request.py` & `vrchatapi-1.9.1/vrchatapi/model/invite_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/invite_response.py` & `vrchatapi-1.9.1/vrchatapi/model/invite_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/license.py` & `vrchatapi-1.9.1/vrchatapi/model/license.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/license_action.py` & `vrchatapi-1.9.1/vrchatapi/model/license_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/license_group.py` & `vrchatapi-1.9.1/vrchatapi/model/license_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/license_group_id.py` & `vrchatapi-1.9.1/vrchatapi/model/license_group_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/license_type.py` & `vrchatapi-1.9.1/vrchatapi/model/license_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/limited_unity_package.py` & `vrchatapi-1.9.1/vrchatapi/model/limited_unity_package.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/limited_user.py` & `vrchatapi-1.9.1/vrchatapi/model/limited_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/limited_world.py` & `vrchatapi-1.9.1/vrchatapi/model/limited_world.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/mime_type.py` & `vrchatapi-1.9.1/vrchatapi/model/mime_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/moderate_user_request.py` & `vrchatapi-1.9.1/vrchatapi/model/moderate_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/notification.py` & `vrchatapi-1.9.1/vrchatapi/model/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/notification_type.py` & `vrchatapi-1.9.1/vrchatapi/model/notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/past_display_name.py` & `vrchatapi-1.9.1/vrchatapi/model/past_display_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/permission.py` & `vrchatapi-1.9.1/vrchatapi/model/permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/permission_id.py` & `vrchatapi-1.9.1/vrchatapi/model/permission_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/player_moderation.py` & `vrchatapi-1.9.1/vrchatapi/model/player_moderation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/player_moderation_id.py` & `vrchatapi-1.9.1/vrchatapi/model/player_moderation_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/player_moderation_type.py` & `vrchatapi-1.9.1/vrchatapi/model/player_moderation_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/public_announcement.py` & `vrchatapi-1.9.1/vrchatapi/model/public_announcement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/region.py` & `vrchatapi-1.9.1/vrchatapi/model/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/release_status.py` & `vrchatapi-1.9.1/vrchatapi/model/release_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/request_invite_request.py` & `vrchatapi-1.9.1/vrchatapi/model/request_invite_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/response.py` & `vrchatapi-1.9.1/vrchatapi/model/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/sent_notification.py` & `vrchatapi-1.9.1/vrchatapi/model/sent_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/subscription.py` & `vrchatapi-1.9.1/vrchatapi/model/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/subscription_period.py` & `vrchatapi-1.9.1/vrchatapi/model/subscription_period.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/success.py` & `vrchatapi-1.9.1/vrchatapi/model/success.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/tag.py` & `vrchatapi-1.9.1/vrchatapi/model/tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/transaction.py` & `vrchatapi-1.9.1/vrchatapi/model/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/transaction_agreement.py` & `vrchatapi-1.9.1/vrchatapi/model/transaction_agreement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/transaction_id.py` & `vrchatapi-1.9.1/vrchatapi/model/transaction_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/transaction_status.py` & `vrchatapi-1.9.1/vrchatapi/model/transaction_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/transaction_steam_info.py` & `vrchatapi-1.9.1/vrchatapi/model/transaction_steam_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/transaction_steam_wallet_info.py` & `vrchatapi-1.9.1/vrchatapi/model/transaction_steam_wallet_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/two_factor_auth_code.py` & `vrchatapi-1.9.1/vrchatapi/model/two_factor_auth_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/unity_package.py` & `vrchatapi-1.9.1/vrchatapi/model/unity_package.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/unity_package_id.py` & `vrchatapi-1.9.1/vrchatapi/model/unity_package_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/update_avatar_request.py` & `vrchatapi-1.9.1/vrchatapi/model/update_avatar_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/update_favorite_group_request.py` & `vrchatapi-1.9.1/vrchatapi/model/update_favorite_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/update_invite_message_request.py` & `vrchatapi-1.9.1/vrchatapi/model/update_invite_message_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/update_user_request.py` & `vrchatapi-1.9.1/vrchatapi/model/update_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/update_world_request.py` & `vrchatapi-1.9.1/vrchatapi/model/update_world_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/user.py` & `vrchatapi-1.9.1/vrchatapi/model/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -106,26 +106,26 @@
             'bio_links': ([str],),  # noqa: E501
             'current_avatar_image_url': (str,),  # noqa: E501
             'current_avatar_thumbnail_image_url': (str,),  # noqa: E501
             'date_joined': (date,),  # noqa: E501
             'developer_type': (DeveloperType,),  # noqa: E501
             'display_name': (str,),  # noqa: E501
             'friend_key': (str,),  # noqa: E501
-            'friend_request_status': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'is_friend': (bool,),  # noqa: E501
             'last_activity': (str,),  # noqa: E501
             'last_login': (str,),  # noqa: E501
             'last_platform': (str,),  # noqa: E501
             'profile_pic_override': (str,),  # noqa: E501
             'state': (UserState,),  # noqa: E501
             'status': (UserStatus,),  # noqa: E501
             'status_description': (str,),  # noqa: E501
             'tags': ([Tag],),  # noqa: E501
             'user_icon': (str,),  # noqa: E501
+            'friend_request_status': (str,),  # noqa: E501
             'instance_id': (InstanceID,),  # noqa: E501
             'location': (WorldID,),  # noqa: E501
             'note': (str,),  # noqa: E501
             'traveling_to_instance': (str,),  # noqa: E501
             'traveling_to_location': (str,),  # noqa: E501
             'traveling_to_world': (str,),  # noqa: E501
             'username': (str,),  # noqa: E501
@@ -143,26 +143,26 @@
         'bio_links': 'bioLinks',  # noqa: E501
         'current_avatar_image_url': 'currentAvatarImageUrl',  # noqa: E501
         'current_avatar_thumbnail_image_url': 'currentAvatarThumbnailImageUrl',  # noqa: E501
         'date_joined': 'date_joined',  # noqa: E501
         'developer_type': 'developerType',  # noqa: E501
         'display_name': 'displayName',  # noqa: E501
         'friend_key': 'friendKey',  # noqa: E501
-        'friend_request_status': 'friendRequestStatus',  # noqa: E501
         'id': 'id',  # noqa: E501
         'is_friend': 'isFriend',  # noqa: E501
         'last_activity': 'last_activity',  # noqa: E501
         'last_login': 'last_login',  # noqa: E501
         'last_platform': 'last_platform',  # noqa: E501
         'profile_pic_override': 'profilePicOverride',  # noqa: E501
         'state': 'state',  # noqa: E501
         'status': 'status',  # noqa: E501
         'status_description': 'statusDescription',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'user_icon': 'userIcon',  # noqa: E501
+        'friend_request_status': 'friendRequestStatus',  # noqa: E501
         'instance_id': 'instanceId',  # noqa: E501
         'location': 'location',  # noqa: E501
         'note': 'note',  # noqa: E501
         'traveling_to_instance': 'travelingToInstance',  # noqa: E501
         'traveling_to_location': 'travelingToLocation',  # noqa: E501
         'traveling_to_world': 'travelingToWorld',  # noqa: E501
         'username': 'username',  # noqa: E501
@@ -172,27 +172,26 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, bio, bio_links, current_avatar_image_url, current_avatar_thumbnail_image_url, date_joined, developer_type, display_name, friend_key, friend_request_status, id, is_friend, last_activity, last_login, last_platform, profile_pic_override, state, status, status_description, tags, user_icon, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, bio, bio_links, current_avatar_image_url, current_avatar_thumbnail_image_url, date_joined, developer_type, display_name, friend_key, id, is_friend, last_activity, last_login, last_platform, profile_pic_override, state, status, status_description, tags, user_icon, *args, **kwargs):  # noqa: E501
         """User - a model defined in OpenAPI
 
         Args:
             bio (str):
             bio_links ([str]):
             current_avatar_image_url (str): When profilePicOverride is not empty, use it instead.
             current_avatar_thumbnail_image_url (str): When profilePicOverride is not empty, use it instead.
             date_joined (date):
             developer_type (DeveloperType):
             display_name (str): A users visual display name. This is what shows up in-game, and can different from their `username`. Changing display name is restricted to a cooldown period.
             friend_key (str):
-            friend_request_status (str):
             id (str): A users unique ID, usually in the form of `usr_c1644b5b-3ca4-45b4-97c6-a2a0de70d469`. Legacy players can have old IDs in the form of `8JoV9XEdpo`. The ID can never be changed.
             is_friend (bool): Either their `friendKey`, or empty string if you are not friends. Unknown usage.
             last_activity (str): Either a date-time or empty string.
             last_login (str): Either a date-time or empty string.
             last_platform (str): This can be `standalonewindows` or `android`, but can also pretty much be any random Unity verison such as `2019.2.4-801-Release` or `2019.2.2-772-Release` or even `unknownplatform`.
             profile_pic_override (str):
             state (UserState):
@@ -229,14 +228,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            friend_request_status (str): [optional]  # noqa: E501
             instance_id (InstanceID): [optional]  # noqa: E501
             location (WorldID): [optional]  # noqa: E501
             note (str): [optional]  # noqa: E501
             traveling_to_instance (str): [optional]  # noqa: E501
             traveling_to_location (str): [optional]  # noqa: E501
             traveling_to_world (str): [optional]  # noqa: E501
             username (str): -| A users unique name, used during login. This is different from `displayName` which is what shows up in-game. A users `username` can never be changed.' **DEPRECATED:** VRChat API no longer return usernames of other users. [See issue by Tupper for more information](https://github.com/pypy-vrc/VRCX/issues/429).. [optional]  # noqa: E501
@@ -274,15 +274,14 @@
         self.bio_links = bio_links
         self.current_avatar_image_url = current_avatar_image_url
         self.current_avatar_thumbnail_image_url = current_avatar_thumbnail_image_url
         self.date_joined = date_joined
         self.developer_type = developer_type
         self.display_name = display_name
         self.friend_key = friend_key
-        self.friend_request_status = friend_request_status
         self.id = id
         self.is_friend = is_friend
         self.last_activity = last_activity
         self.last_login = last_login
         self.last_platform = last_platform
         self.profile_pic_override = profile_pic_override
         self.state = state
@@ -306,27 +305,26 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, bio, bio_links, current_avatar_image_url, current_avatar_thumbnail_image_url, date_joined, developer_type, display_name, friend_key, friend_request_status, id, is_friend, last_activity, last_login, last_platform, profile_pic_override, state, status, status_description, tags, user_icon, *args, **kwargs):  # noqa: E501
+    def __init__(self, bio, bio_links, current_avatar_image_url, current_avatar_thumbnail_image_url, date_joined, developer_type, display_name, friend_key, id, is_friend, last_activity, last_login, last_platform, profile_pic_override, state, status, status_description, tags, user_icon, *args, **kwargs):  # noqa: E501
         """User - a model defined in OpenAPI
 
         Args:
             bio (str):
             bio_links ([str]):
             current_avatar_image_url (str): When profilePicOverride is not empty, use it instead.
             current_avatar_thumbnail_image_url (str): When profilePicOverride is not empty, use it instead.
             date_joined (date):
             developer_type (DeveloperType):
             display_name (str): A users visual display name. This is what shows up in-game, and can different from their `username`. Changing display name is restricted to a cooldown period.
             friend_key (str):
-            friend_request_status (str):
             id (str): A users unique ID, usually in the form of `usr_c1644b5b-3ca4-45b4-97c6-a2a0de70d469`. Legacy players can have old IDs in the form of `8JoV9XEdpo`. The ID can never be changed.
             is_friend (bool): Either their `friendKey`, or empty string if you are not friends. Unknown usage.
             last_activity (str): Either a date-time or empty string.
             last_login (str): Either a date-time or empty string.
             last_platform (str): This can be `standalonewindows` or `android`, but can also pretty much be any random Unity verison such as `2019.2.4-801-Release` or `2019.2.2-772-Release` or even `unknownplatform`.
             profile_pic_override (str):
             state (UserState):
@@ -363,14 +361,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            friend_request_status (str): [optional]  # noqa: E501
             instance_id (InstanceID): [optional]  # noqa: E501
             location (WorldID): [optional]  # noqa: E501
             note (str): [optional]  # noqa: E501
             traveling_to_instance (str): [optional]  # noqa: E501
             traveling_to_location (str): [optional]  # noqa: E501
             traveling_to_world (str): [optional]  # noqa: E501
             username (str): -| A users unique name, used during login. This is different from `displayName` which is what shows up in-game. A users `username` can never be changed.' **DEPRECATED:** VRChat API no longer return usernames of other users. [See issue by Tupper for more information](https://github.com/pypy-vrc/VRCX/issues/429).. [optional]  # noqa: E501
@@ -406,15 +405,14 @@
         self.bio_links = bio_links
         self.current_avatar_image_url = current_avatar_image_url
         self.current_avatar_thumbnail_image_url = current_avatar_thumbnail_image_url
         self.date_joined = date_joined
         self.developer_type = developer_type
         self.display_name = display_name
         self.friend_key = friend_key
-        self.friend_request_status = friend_request_status
         self.id = id
         self.is_friend = is_friend
         self.last_activity = last_activity
         self.last_login = last_login
         self.last_platform = last_platform
         self.profile_pic_override = profile_pic_override
         self.state = state
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/user_exists.py` & `vrchatapi-1.9.1/vrchatapi/model/user_exists.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/user_state.py` & `vrchatapi-1.9.1/vrchatapi/model/user_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/user_status.py` & `vrchatapi-1.9.1/vrchatapi/model/user_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/user_subscription.py` & `vrchatapi-1.9.1/vrchatapi/model/user_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/verify2_fa_result.py` & `vrchatapi-1.9.1/vrchatapi/model/verify2_fa_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/verify_auth_token_result.py` & `vrchatapi-1.9.1/vrchatapi/model/verify_auth_token_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/world.py` & `vrchatapi-1.9.1/vrchatapi/model/world.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/world_id.py` & `vrchatapi-1.9.1/vrchatapi/model/world_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/world_metadata.py` & `vrchatapi-1.9.1/vrchatapi/model/world_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model/world_publish_status.py` & `vrchatapi-1.9.1/vrchatapi/model/world_publish_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `vrchatapi-1.9.0/vrchatapi/model_utils.py` & `vrchatapi-1.9.1/vrchatapi/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

### Comparing `vrchatapi-1.9.0/vrchatapi/models/__init__.py` & `vrchatapi-1.9.1/vrchatapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vrchatapi-1.9.0/vrchatapi/rest.py` & `vrchatapi-1.9.1/vrchatapi/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     VRChat API Documentation
 
 
-    The version of the OpenAPI document: 1.9.0
+    The version of the OpenAPI document: 1.9.1
     Contact: me@ariesclark.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `vrchatapi-1.9.0/vrchatapi.egg-info/PKG-INFO` & `vrchatapi-1.9.1/vrchatapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vrchatapi
-Version: 1.9.0
+Version: 1.9.1
 Summary: VRChat API Library for Python
 Home-page: 
 Author: Unofficial VRChat API Documentation Project
 Author-email: me@ariesclark.com
 License: The MIT License (MIT)
 Keywords: vrchat,vrchatapi,vrc
 Requires-Python: >=3.6
```

### Comparing `vrchatapi-1.9.0/vrchatapi.egg-info/SOURCES.txt` & `vrchatapi-1.9.1/vrchatapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

