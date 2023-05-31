# Comparing `tmp/mautrix-instagram-0.2.3.tar.gz` & `tmp/mautrix-instagram-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mautrix-instagram-0.2.3.tar", last modified: Tue Dec 13 22:06:58 2022, max compression
+gzip compressed data, was "mautrix-instagram-0.3.0.tar", last modified: Wed May 31 20:04:37 2023, max compression
```

## Comparing `mautrix-instagram-0.2.3.tar` & `mautrix-instagram-0.3.0.tar`

### file list

```diff
@@ -1,107 +1,120 @@
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.693978 mautrix-instagram-0.2.3/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4747 2022-12-13 22:03:38.000000 mautrix-instagram-0.2.3/CHANGELOG.md
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    34523 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/LICENSE
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      114 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/MANIFEST.in
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2420 2022-12-13 22:06:58.693978 mautrix-instagram-0.2.3/PKG-INFO
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1407 2022-11-18 19:53:04.000000 mautrix-instagram-0.2.3/README.md
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.685978 mautrix-instagram-0.2.3/mauigpapi/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      167 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/__init__.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.685978 mautrix-instagram-0.2.3/mauigpapi/errors/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      907 2022-12-12 18:36:54.000000 mautrix-instagram-0.2.3/mauigpapi/errors/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      788 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/errors/base.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1209 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/errors/mqtt.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4064 2022-12-12 18:36:54.000000 mautrix-instagram-0.2.3/mauigpapi/errors/response.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1200 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/errors/state.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.685978 mautrix-instagram-0.2.3/mauigpapi/http/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       28 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/http/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5455 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/http/account.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      315 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/http/api.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    12124 2022-12-12 18:36:54.000000 mautrix-instagram-0.2.3/mauigpapi/http/base.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5562 2022-11-18 12:45:57.000000 mautrix-instagram-0.2.3/mauigpapi/http/challenge.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     7734 2022-11-28 10:58:49.000000 mautrix-instagram-0.2.3/mauigpapi/http/login.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1750 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/http/qe.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6843 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/mauigpapi/http/thread.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5947 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/http/upload.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1216 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/http/user.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.685978 mautrix-instagram-0.2.3/mauigpapi/mqtt/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      167 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/mqtt/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    38141 2022-11-29 18:54:51.000000 mautrix-instagram-0.2.3/mauigpapi/mqtt/conn.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      977 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/mqtt/events.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2003 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/mqtt/otclient.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    12229 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/mqtt/subscription.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.689978 mautrix-instagram-0.2.3/mauigpapi/mqtt/thrift/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      224 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/mqtt/thrift/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3006 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/mqtt/thrift/autospec.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3708 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/mqtt/thrift/ig_objects.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2192 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/mqtt/thrift/read.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1023 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/mqtt/thrift/type.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6312 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/mqtt/thrift/write.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1494 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/proxy.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.689978 mautrix-instagram-0.2.3/mauigpapi/state/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       32 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/state/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    20688 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/state/application.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2266 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/state/cookies.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2909 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/state/device.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1114 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/state/experiments.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.689978 mautrix-instagram-0.2.3/mauigpapi/state/samples/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      203 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/state/samples/builds.json
--rw-rw-r--   0 tulir     (1000) tulir     (1000)   123371 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/state/samples/devices.json
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      679 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/state/samples/supported-capabilities.json
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1394 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/state/session.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3638 2022-11-18 12:45:57.000000 mautrix-instagram-0.2.3/mauigpapi/state/state.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.689978 mautrix-instagram-0.2.3/mauigpapi/types/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2536 2022-11-18 12:45:57.000000 mautrix-instagram-0.2.3/mauigpapi/types/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3557 2022-12-12 18:36:54.000000 mautrix-instagram-0.2.3/mauigpapi/types/account.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2420 2022-11-18 12:45:57.000000 mautrix-instagram-0.2.3/mauigpapi/types/challenge.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1730 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/types/direct_inbox.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3933 2022-11-29 09:29:06.000000 mautrix-instagram-0.2.3/mauigpapi/types/error.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1908 2022-12-13 19:04:24.000000 mautrix-instagram-0.2.3/mauigpapi/types/login.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     7561 2022-11-29 21:14:36.000000 mautrix-instagram-0.2.3/mauigpapi/types/mqtt.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1899 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/types/qe.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2896 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/types/thread.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    17290 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/mauigpapi/types/thread_item.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1158 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/types/upload.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1277 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mauigpapi/types/user.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.693978 mautrix-instagram-0.2.3/mautrix_instagram/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       70 2022-12-13 22:03:31.000000 mautrix-instagram-0.2.3/mautrix_instagram/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6313 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/__main__.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.693978 mautrix-instagram-0.2.3/mautrix_instagram/commands/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       99 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/commands/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     8753 2022-11-30 13:04:48.000000 mautrix-instagram-0.2.3/mautrix_instagram/commands/auth.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3556 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/commands/conn.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1809 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/commands/misc.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      282 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/commands/typehint.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4362 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/mautrix_instagram/config.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.693978 mautrix-instagram-0.2.3/mautrix_instagram/db/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      421 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/mautrix_instagram/db/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3814 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/mautrix_instagram/db/message.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5174 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/mautrix_instagram/db/portal.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4164 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/db/puppet.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4171 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/db/reaction.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5448 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/mautrix_instagram/db/upgrade.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3236 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/mautrix_instagram/db/user.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    15870 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/mautrix_instagram/example-config.yaml
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1442 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/get_version.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5631 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/mautrix_instagram/matrix.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    85928 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/mautrix_instagram/portal.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     8822 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/puppet.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    34891 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/mautrix_instagram/user.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.693978 mautrix-instagram-0.2.3/mautrix_instagram/util/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/util/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1509 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/util/color_log.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      176 2022-12-13 22:06:58.000000 mautrix-instagram-0.2.3/mautrix_instagram/version.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.693978 mautrix-instagram-0.2.3/mautrix_instagram/web/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       46 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/web/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    31885 2022-12-12 18:36:54.000000 mautrix-instagram-0.2.3/mautrix_instagram/web/provisioning_api.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      949 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/mautrix_instagram/web/segment.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-13 22:06:58.693978 mautrix-instagram-0.2.3/mautrix_instagram.egg-info/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2420 2022-12-13 22:06:58.000000 mautrix-instagram-0.2.3/mautrix_instagram.egg-info/PKG-INFO
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2581 2022-12-13 22:06:58.000000 mautrix-instagram-0.2.3/mautrix_instagram.egg-info/SOURCES.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        1 2022-12-13 22:06:58.000000 mautrix-instagram-0.2.3/mautrix_instagram.egg-info/dependency_links.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      499 2022-12-13 22:06:58.000000 mautrix-instagram-0.2.3/mautrix_instagram.egg-info/requires.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       28 2022-12-13 22:06:58.000000 mautrix-instagram-0.2.3/mautrix_instagram.egg-info/top_level.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      321 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/optional-requirements.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      203 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/pyproject.toml
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      188 2022-12-12 18:41:33.000000 mautrix-instagram-0.2.3/requirements.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2022-12-13 22:06:58.693978 mautrix-instagram-0.2.3/setup.cfg
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2280 2022-11-07 15:03:21.000000 mautrix-instagram-0.2.3/setup.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.997753 mautrix-instagram-0.3.0/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5770 2023-05-31 19:59:31.000000 mautrix-instagram-0.3.0/CHANGELOG.md
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    34523 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/LICENSE
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      114 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/MANIFEST.in
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2383 2023-05-31 20:04:36.997753 mautrix-instagram-0.3.0/PKG-INFO
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1407 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/README.md
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.985753 mautrix-instagram-0.3.0/mauigpapi/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      135 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/__init__.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.989753 mautrix-instagram-0.3.0/mauigpapi/errors/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      970 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/errors/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      788 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/errors/base.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1262 2023-05-31 19:51:18.000000 mautrix-instagram-0.3.0/mauigpapi/errors/mqtt.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4127 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/errors/response.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1200 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/errors/state.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.989753 mautrix-instagram-0.3.0/mauigpapi/http/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       28 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/http/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5455 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/http/account.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      278 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/http/api.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    13512 2023-05-31 19:51:23.000000 mautrix-instagram-0.3.0/mauigpapi/http/base.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5562 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/http/challenge.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     8283 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/http/login.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     8197 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/http/thread.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5947 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/http/upload.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1216 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/http/user.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.989753 mautrix-instagram-0.3.0/mauigpapi/mqtt/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      167 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/mqtt/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    40999 2023-05-31 19:51:23.000000 mautrix-instagram-0.3.0/mauigpapi/mqtt/conn.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      977 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/mqtt/events.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2003 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/mqtt/otclient.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    12229 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/mqtt/subscription.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.989753 mautrix-instagram-0.3.0/mauigpapi/mqtt/thrift/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      224 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/mqtt/thrift/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3006 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/mqtt/thrift/autospec.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3711 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/mqtt/thrift/ig_objects.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2192 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/mqtt/thrift/read.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1023 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/mqtt/thrift/type.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6312 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/mqtt/thrift/write.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.989753 mautrix-instagram-0.3.0/mauigpapi/scripts/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/scripts/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3095 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/scripts/iglogin.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.989753 mautrix-instagram-0.3.0/mauigpapi/state/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       32 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/state/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1155 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/state/application.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2266 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/state/cookies.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2871 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/state/device.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1307 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/state/session.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3251 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/state/state.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.993753 mautrix-instagram-0.3.0/mauigpapi/types/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2585 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/types/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3664 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/types/account.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2420 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/types/challenge.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1798 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/types/direct_inbox.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3933 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/types/error.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1958 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/types/login.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     7734 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/types/mqtt.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1899 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/types/qe.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2957 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/types/thread.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    19672 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/types/thread_item.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1158 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/types/upload.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1277 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mauigpapi/types/user.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.993753 mautrix-instagram-0.3.0/mautrix_instagram/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       70 2023-05-31 19:59:36.000000 mautrix-instagram-0.3.0/mautrix_instagram/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6460 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/__main__.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.993753 mautrix-instagram-0.3.0/mautrix_instagram/commands/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       99 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/commands/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     9974 2023-05-31 19:51:23.000000 mautrix-instagram-0.3.0/mautrix_instagram/commands/auth.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3556 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/commands/conn.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1809 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/commands/misc.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      282 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/commands/typehint.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5570 2023-05-31 19:51:23.000000 mautrix-instagram-0.3.0/mautrix_instagram/config.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.993753 mautrix-instagram-0.3.0/mautrix_instagram/db/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      480 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5736 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/backfill_queue.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4214 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/message.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5435 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/portal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3976 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/puppet.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4171 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/reaction.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.997753 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1271 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5430 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v00_latest_revision.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1311 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v02_name_avatar_set.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1040 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v03_relay_portal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1047 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v04_message_client_content.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1045 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v05_message_ig_timestamp.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1043 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v06_hidden_events.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1032 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v07_reaction_timestamps.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1113 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v08_sync_sequence_id.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1981 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v09_backfill_queue.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1304 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v10_portal_infinite_backfill.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1293 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v11_per_user_thread_sync_status.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1061 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v12_portal_thread_image_id.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1135 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v13_fix_portal_thread_image_id.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1091 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v14_puppet_contact_info_set.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3746 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/db/user.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    19782 2023-05-31 19:51:23.000000 mautrix-instagram-0.3.0/mautrix_instagram/example-config.yaml
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3601 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/formatter.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1442 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/get_version.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6224 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/matrix.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)   113502 2023-05-31 19:51:23.000000 mautrix-instagram-0.3.0/mautrix_instagram/portal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    10459 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/puppet.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    50012 2023-05-31 19:51:23.000000 mautrix-instagram-0.3.0/mautrix_instagram/user.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.997753 mautrix-instagram-0.3.0/mautrix_instagram/util/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/util/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1509 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/util/color_log.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      176 2023-05-31 20:04:36.000000 mautrix-instagram-0.3.0/mautrix_instagram/version.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.997753 mautrix-instagram-0.3.0/mautrix_instagram/web/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       46 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/web/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    34310 2023-05-16 09:57:34.000000 mautrix-instagram-0.3.0/mautrix_instagram/web/provisioning_api.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1108 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/mautrix_instagram/web/segment.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-31 20:04:36.993753 mautrix-instagram-0.3.0/mautrix_instagram.egg-info/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2383 2023-05-31 20:04:36.000000 mautrix-instagram-0.3.0/mautrix_instagram.egg-info/PKG-INFO
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3309 2023-05-31 20:04:36.000000 mautrix-instagram-0.3.0/mautrix_instagram.egg-info/SOURCES.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        1 2023-05-31 20:04:36.000000 mautrix-instagram-0.3.0/mautrix_instagram.egg-info/dependency_links.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      500 2023-05-31 20:04:36.000000 mautrix-instagram-0.3.0/mautrix_instagram.egg-info/requires.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       28 2023-05-31 20:04:36.000000 mautrix-instagram-0.3.0/mautrix_instagram.egg-info/top_level.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      321 2023-05-31 19:59:44.000000 mautrix-instagram-0.3.0/optional-requirements.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      203 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/pyproject.toml
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      189 2023-05-31 19:59:48.000000 mautrix-instagram-0.3.0/requirements.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2023-05-31 20:04:36.997753 mautrix-instagram-0.3.0/setup.cfg
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2210 2023-05-14 10:32:03.000000 mautrix-instagram-0.3.0/setup.py
```

### Comparing `mautrix-instagram-0.2.3/CHANGELOG.md` & `mautrix-instagram-0.3.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+# v0.3.0 (2023-05-31)
+
+* Improved handling of some message types.
+* Added automatic retrying for sending videos to give Instagram servers more
+  time to transcode the video.
+* Added support for @-mentioning users from Matrix.
+* Added support for bridging incoming avatar stickers.
+* Added automatic fetching of shared reel videos to bridge full video instead
+  of only the thumbnail image.
+* Added real-time bridging of group avatar changes from Instagram.
+* Added option to disable sending typing notifications to Instagram.
+* Added notice message when receiving video calls.
+* Added options to automatically ratchet/delete megolm sessions to minimize
+  access to old messages.
+* Added option to not set room name/avatar even in encrypted rooms.
+* Redid backfill system to support MSC2716.
+  * Note that using Synapse's MSC2716 implementation is not recommended, and
+    the bridge can still backfill messages without MSC2716.
+* Implemented appservice pinging using MSC2659.
+* Possibly improved MQTT connection handling.
+
 # v0.2.3 (2022-12-14)
 
 * Added support for "mentioned in comment" messages.
 * Added support for re-requesting 2FA SMS when logging in.
 * Updated Docker image to Alpine 3.17.
 * Fixed error in image bridging.
 * Fixed logging in with phone/email in provisioning API.
```

### Comparing `mautrix-instagram-0.2.3/LICENSE` & `mautrix-instagram-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/PKG-INFO` & `mautrix-instagram-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mautrix-instagram
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Matrix-Instagram puppeting bridge.
 Home-page: https://github.com/mautrix/instagram
 Author: Tulir Asokan
 Author-email: tulir@maunium.net
-License: UNKNOWN
 Project-URL: Changelog, https://github.com/mautrix/instagram/blob/master/CHANGELOG.md
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Communications :: Chat
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -48,9 +46,7 @@
 
 ### Features & Roadmap
 [ROADMAP.md](https://github.com/mautrix/instagram/blob/master/ROADMAP.md)
 contains a general overview of what is supported by the bridge.
 
 ## Discussion
 Matrix room: [`#instagram:maunium.net`](https://matrix.to/#/#instagram:maunium.net)
-
-
```

### Comparing `mautrix-instagram-0.2.3/README.md` & `mautrix-instagram-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/errors/__init__.py` & `mautrix-instagram-0.3.0/mauigpapi/errors/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .base import IGError
 from .mqtt import (
     IGMQTTError,
     IrisSubscribeError,
     MQTTConnectionUnauthorized,
     MQTTNotConnected,
     MQTTNotLoggedIn,
+    MQTTReconnectionError,
 )
 from .response import (
     IG2FACodeExpiredError,
     IGActionSpamError,
     IGBad2FACodeError,
     IGChallengeError,
     IGChallengeWrongCodeError,
@@ -16,14 +17,15 @@
     IGConsentRequiredError,
     IGFBEmailTaken,
     IGFBNoContactPointFoundError,
     IGFBSSODisabled,
     IGInactiveUserError,
     IGLoginBadPasswordError,
     IGLoginError,
+    IGLoginInvalidCredentialsError,
     IGLoginInvalidUserError,
     IGLoginRequiredError,
     IGLoginTwoFactorRequiredError,
     IGLoginUnusablePasswordError,
     IGNotFoundError,
     IGNotLoggedInError,
     IGPrivateUserError,
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/errors/base.py` & `mautrix-instagram-0.3.0/mauigpapi/errors/base.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/errors/mqtt.py` & `mautrix-instagram-0.3.0/mauigpapi/errors/mqtt.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     pass
 
 
 class MQTTNotLoggedIn(IGMQTTError):
     pass
 
 
+class MQTTReconnectionError(IGMQTTError):
+    pass
+
+
 class MQTTNotConnected(IGMQTTError):
     pass
 
 
 class MQTTConnectionUnauthorized(IGMQTTError):
     def __init__(self) -> None:
         super().__init__("Server refused connection with error code 5")
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/errors/response.py` & `mautrix-instagram-0.3.0/mauigpapi/errors/response.py`

 * *Files 7% similar despite different names*

```diff
@@ -148,14 +148,18 @@
     pass
 
 
 class IGLoginInvalidUserError(IGLoginError):
     pass
 
 
+class IGLoginInvalidCredentialsError(IGLoginError):
+    pass
+
+
 class IGBad2FACodeError(IGResponseError):
     pass
 
 
 class IG2FACodeExpiredError(IGResponseError):
     pass
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/errors/state.py` & `mautrix-instagram-0.3.0/mauigpapi/errors/state.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/http/account.py` & `mautrix-instagram-0.3.0/mauigpapi/http/account.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/http/base.py` & `mautrix-instagram-0.3.0/mauigpapi/http/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mautrix-instagram - A Matrix-Instagram puppeting bridge.
-# Copyright (C) 2022 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -11,51 +11,52 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-from typing import Any, Type, TypeVar
+from typing import Any, Awaitable, Callable, Type, TypeVar
+from functools import partial
 import json
 import logging
-import random
 import time
 
 from aiohttp import ClientResponse, ClientSession, ContentTypeError, CookieJar
 from yarl import URL
 
 from mautrix.types import JSON, Serializable
 from mautrix.util.logging import TraceLogger
+from mautrix.util.proxy import ProxyHandler, proxy_with_retry
 
 from ..errors import (
     IG2FACodeExpiredError,
     IGActionSpamError,
     IGBad2FACodeError,
     IGChallengeError,
     IGCheckpointError,
     IGConsentRequiredError,
     IGFBEmailTaken,
     IGFBNoContactPointFoundError,
     IGFBSSODisabled,
     IGInactiveUserError,
     IGLoginBadPasswordError,
+    IGLoginInvalidCredentialsError,
     IGLoginInvalidUserError,
     IGLoginRequiredError,
     IGLoginTwoFactorRequiredError,
     IGLoginUnusablePasswordError,
     IGNotFoundError,
     IGPrivateUserError,
     IGRateLimitError,
     IGResponseError,
     IGSentryBlockError,
     IGUnknownError,
     IGUserHasLoggedOutError,
 )
-from ..proxy import ProxyHandler
 from ..state import AndroidState
 from ..types import ChallengeContext
 
 try:
     from aiohttp_socks import ProxyConnector
 except ImportError:
     ProxyConnector = None
@@ -76,22 +77,36 @@
     log: TraceLogger
 
     def __init__(
         self,
         state: AndroidState,
         log: TraceLogger | None = None,
         proxy_handler: ProxyHandler | None = None,
+        on_proxy_update: Callable[[], Awaitable[None]] | None = None,
+        on_response_error: Callable[[IGResponseError], Awaitable[None]] | None = None,
     ) -> None:
         self.log = log or logging.getLogger("mauigpapi.http")
 
         self.proxy_handler = proxy_handler
+        self.on_proxy_update = on_proxy_update
+        self.on_response_error = on_response_error
         self.setup_http(cookie_jar=state.cookies.jar)
 
         self.state = state
 
+        self.proxy_with_retry = partial(
+            proxy_with_retry,
+            logger=self.log,
+            proxy_handler=self.proxy_handler,
+            on_proxy_change=self.on_proxy_update,
+            # Wait 1s * errors, max 10s for fast failure
+            max_wait_seconds=10,
+            multiply_wait_seconds=1,
+        )
+
     @staticmethod
     def sign(req: Any, filter_nulls: bool = False) -> dict[str, str]:
         if isinstance(req, Serializable):
             req = req.serialize()
         if isinstance(req, dict):
             req = json.dumps(remove_nulls(req) if filter_nulls else req)
         return {"signed_body": f"SIGNATURE.{req}"}
@@ -99,73 +114,74 @@
     @property
     def _headers(self) -> dict[str, str]:
         headers = {
             "x-ads-opt-out": str(int(self.state.session.ads_opt_out)),
             "x-device-id": self.state.device.uuid,
             "x-ig-app-locale": self.state.device.language,
             "x-ig-device-locale": self.state.device.language,
-            "x-pigeon-session-id": self.state.pigeon_session_id,
+            "x-ig-mapped-locale": self.state.device.language,
+            "x-pigeon-session-id": f"UFS-{self.state.pigeon_session_id}-0",
             "x-pigeon-rawclienttime": str(round(time.time(), 3)),
-            "x-ig-connection-speed": f"{random.randint(1000, 3700)}kbps",
             "x-ig-bandwidth-speed-kbps": "-1.000",
             "x-ig-bandwidth-totalbytes-b": "0",
             "x-ig-bandwidth-totaltime-ms": "0",
-            "x-ig-eu-dc-enabled": (
-                str(self.state.session.eu_dc_enabled).lower()
-                if self.state.session.eu_dc_enabled is not None
-                else None
-            ),
             "x-ig-app-startup-country": self.state.device.language.split("_")[1],
             "x-bloks-version-id": self.state.application.BLOKS_VERSION_ID,
             "x-ig-www-claim": self.state.session.ig_www_claim or "0",
             "x-bloks-is-layout-rtl": str(self.state.device.is_layout_rtl).lower(),
-            "x-bloks-is-panorama-enabled": "true",
             "x-ig-timezone-offset": self.state.device.timezone_offset,
-            # "x-messenger": "1",
             "x-ig-device-id": self.state.device.uuid,
+            "x-ig-family-device-id": self.state.device.fdid,
             "x-ig-android-id": self.state.device.id,
             "x-ig-connection-type": self.state.device.connection_type,
+            "x-fb-connection-type": self.state.device.connection_type,
             "x-ig-capabilities": self.state.application.CAPABILITIES,
             "x-ig-app-id": self.state.application.FACEBOOK_ANALYTICS_APPLICATION_ID,
             "user-agent": self.state.user_agent,
             "accept-language": self.state.device.language.replace("_", "-"),
             "authorization": self.state.session.authorization,
             "x-mid": self.state.cookies.get_value("mid"),
             "ig-u-ig-direct-region-hint": self.state.session.region_hint,
             "ig-u-shbid": self.state.session.shbid,
             "ig-u-shbts": self.state.session.shbts,
             "ig-u-ds-user-id": self.state.session.ds_user_id,
             "ig-u-rur": self.state.session.rur,
+            "ig-intended-user-id": self.state.session.ds_user_id or "0",
+            "ig-client-endpoint": "unknown",
             "x-fb-http-engine": "Liger",
             "x-fb-client-ip": "True",
+            "x-fb-rmd": "cached=0;state=NO_MATCH",
+            "x-fb-server-cluster": "True",
+            "x-tigon-is-retry": "False",
             "accept-encoding": "gzip",
         }
         return {k: v for k, v in headers.items() if v is not None}
 
     def setup_http(self, cookie_jar: CookieJar) -> None:
         connector = None
-        http_proxy = self.proxy_handler.get_proxy_url()
+        http_proxy = self.proxy_handler.get_proxy_url() if self.proxy_handler else None
         if http_proxy:
             if ProxyConnector:
                 connector = ProxyConnector.from_url(http_proxy)
             else:
                 self.log.warning("http_proxy is set, but aiohttp-socks is not installed")
 
         self.http = ClientSession(connector=connector, cookie_jar=cookie_jar)
         return None
 
-    def raw_http_get(self, url: URL | str):
+    def raw_http_get(self, url: URL | str, **kwargs):
         if isinstance(url, str):
             url = URL(url, encoded=True)
         return self.http.get(
             url,
             headers={
                 "user-agent": self.state.user_agent,
                 "accept-language": self.state.device.language.replace("_", "-"),
             },
+            **kwargs,
         )
 
     async def std_http_post(
         self,
         path: str,
         data: JSON = None,
         raw: bool = False,
@@ -174,15 +190,18 @@
         query: dict[str, str] | None = None,
         response_type: Type[T] | None = JSON,
     ) -> T:
         headers = {**self._headers, **headers} if headers else self._headers
         if not raw:
             data = self.sign(data, filter_nulls=filter_nulls)
         url = self.url.with_path(path).with_query(query or {})
-        resp = await self.http.post(url=url, headers=headers, data=data)
+        resp = await self.proxy_with_retry(
+            f"AndroidAPI.std_http_post: {url}",
+            lambda: self.http.post(url=url, headers=headers, data=data),
+        )
         self.log.trace(f"{path} response: {await resp.text()}")
         if response_type is str or response_type is None:
             self._handle_response_headers(resp)
             if response_type is str:
                 return await resp.text()
             return None
         json_data = await self._handle_response(resp)
@@ -195,15 +214,19 @@
         path: str,
         query: dict[str, str] | None = None,
         headers: dict[str, str] | None = None,
         response_type: Type[T] | None = JSON,
     ) -> T:
         headers = {**self._headers, **headers} if headers else self._headers
         query = {k: v for k, v in (query or {}).items() if v is not None}
-        resp = await self.http.get(url=self.url.with_path(path).with_query(query), headers=headers)
+        url = self.url.with_path(path).with_query(query)
+        resp = await self.proxy_with_retry(
+            f"AndroidAPI.std_http_get: {url}",
+            lambda: self.http.get(url=url, headers=headers),
+        )
         self.log.trace(f"{path} response: {await resp.text()}")
         if response_type is None:
             self._handle_response_headers(resp)
             return None
         json_data = await self._handle_response(resp)
         if response_type is not JSON:
             return response_type.deserialize(json_data)
@@ -214,30 +237,33 @@
         try:
             body = await resp.json()
         except (json.JSONDecodeError, ContentTypeError) as e:
             raise IGUnknownError(resp) from e
         if body.get("status", "fail") == "ok":
             return body
         else:
-            await self._raise_response_error(resp)
+            err = await self._get_response_error(resp)
+            if self.on_response_error:
+                await self.on_response_error(err)
+            raise err
 
-    async def _raise_response_error(self, resp: ClientResponse) -> None:
+    async def _get_response_error(self, resp: ClientResponse) -> IGResponseError:
         try:
             data = await resp.json()
         except json.JSONDecodeError:
             data = {}
 
         if data.get("spam", False):
-            raise IGActionSpamError(resp, data)
+            return IGActionSpamError(resp, data)
         elif data.get("two_factor_required", False):
-            raise IGLoginTwoFactorRequiredError(resp, data)
+            return IGLoginTwoFactorRequiredError(resp, data)
         elif resp.status == 404:
-            raise IGNotFoundError(resp, data)
+            return IGNotFoundError(resp, data)
         elif resp.status == 429:
-            raise IGRateLimitError(resp, data)
+            return IGRateLimitError(resp, data)
 
         message = data.get("message")
         if isinstance(message, str):
             if message == "challenge_required":
                 err = IGChallengeError(resp, data)
                 self.log.debug(f"Storing challenge URL {err.url}")
                 self.state.challenge_path = err.url
@@ -246,51 +272,55 @@
                         err.body.challenge.challenge_context
                     )
                 except Exception:
                     self.log.exception(
                         "Failed to deserialize challenge_context %s",
                         err.body.challenge.challenge_context,
                     )
-                raise err
+                return err
             elif message == "checkpoint_required":
-                raise IGCheckpointError(resp, data)
+                return IGCheckpointError(resp, data)
             elif message == "consent_required":
-                raise IGConsentRequiredError(resp, data)
+                return IGConsentRequiredError(resp, data)
             elif message == "user_has_logged_out":
-                raise IGUserHasLoggedOutError(resp, data)
+                return IGUserHasLoggedOutError(resp, data)
             elif message == "login_required":
-                raise IGLoginRequiredError(resp, data)
+                return IGLoginRequiredError(resp, data)
             elif message.lower() == "not authorized to view user":
-                raise IGPrivateUserError(resp, data)
+                return IGPrivateUserError(resp, data)
 
         error_type = data.get("error_type")
         if error_type == "sentry_block":
-            raise IGSentryBlockError(resp, data)
+            return IGSentryBlockError(resp, data)
         elif error_type == "inactive_user":
-            raise IGInactiveUserError(resp, data)
+            return IGInactiveUserError(resp, data)
         elif error_type == "bad_password":
-            raise IGLoginBadPasswordError(resp, data)
+            return IGLoginBadPasswordError(resp, data)
         elif error_type == "unusable_password":
-            raise IGLoginUnusablePasswordError(resp, data)
+            return IGLoginUnusablePasswordError(resp, data)
         elif error_type == "invalid_user":
-            raise IGLoginInvalidUserError(resp, data)
+            return IGLoginInvalidUserError(resp, data)
         elif error_type == "sms_code_validation_code_invalid":
-            raise IGBad2FACodeError(resp, data)
+            return IGBad2FACodeError(resp, data)
         elif error_type == "invalid_nonce":
-            raise IG2FACodeExpiredError(resp, data)
+            return IG2FACodeExpiredError(resp, data)
         elif error_type == "fb_no_contact_point_found":
-            raise IGFBNoContactPointFoundError(resp, data)
+            return IGFBNoContactPointFoundError(resp, data)
         elif error_type == "fb_email_taken":
-            raise IGFBEmailTaken(resp, data)
+            return IGFBEmailTaken(resp, data)
         elif error_type == "sso_disabled":
-            raise IGFBSSODisabled(resp, data)
+            return IGFBSSODisabled(resp, data)
         elif error_type == "rate_limit_error":
-            raise IGRateLimitError(resp, data)
+            return IGRateLimitError(resp, data)
+
+        exception_name = data.get("exception_name")
+        if exception_name == "UserInvalidCredentials":
+            return IGLoginInvalidCredentialsError(resp, data)
 
-        raise IGResponseError(resp, data)
+        return IGResponseError(resp, data)
 
     def _handle_response_headers(self, resp: ClientResponse) -> None:
         fields = {
             "x-ig-set-www-claim": "ig_www_claim",
             "ig-set-authorization": "authorization",
             "ig-set-password-encryption-key-id": "password_encryption_key_id",
             "ig-set-password-encryption-pub-key": "password_encryption_pubkey",
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/http/challenge.py` & `mautrix-instagram-0.3.0/mauigpapi/http/challenge.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/http/login.py` & `mautrix-instagram-0.3.0/mauigpapi/http/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,38 @@
 from __future__ import annotations
 
 import base64
 import io
 import json
 import struct
 import time
+import uuid
 
 from Crypto.Cipher import AES, PKCS1_v1_5
 from Crypto.PublicKey import RSA
 from Crypto.Random import get_random_bytes
 
 from ..types import FacebookLoginResponse, LoginErrorResponse, LoginResponse, LogoutResponse
 from .base import BaseAndroidAPI
 
 
 class LoginAPI(BaseAndroidAPI):
+    async def get_mobile_config(self) -> None:
+        req = {
+            "bool_opt_policy": "0",
+            "mobileconfigsessionless": "",
+            "api_version": "3",
+            "unit_type": "1",
+            "query_hash": "dae17f1d3276207ebfe78f7a67cc9a04d4b88ff8c88dfc17e148fafb3f655b8e",
+            "device_id": self.state.device.id,
+            "fetch_type": "ASYNC_FULL",
+            "family_device_id": self.state.device.fdid.upper(),
+        }
+        await self.std_http_post("/api/v1/launcher/mobileconfig/", data=req)
+
     async def login(
         self,
         username: str,
         password: str | None = None,
         encrypted_password: str | None = None,
     ) -> LoginResponse:
         if password:
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/http/thread.py` & `mautrix-instagram-0.3.0/mauigpapi/http/thread.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mautrix-instagram - A Matrix-Instagram puppeting bridge.
-# Copyright (C) 2022 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -11,114 +11,138 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-from typing import AsyncIterable, Type
+from typing import AsyncIterable, Callable, Type
+import asyncio
 import json
 
+from mauigpapi.errors.response import IGRateLimitError
+
 from ..types import (
     CommandResponse,
     DMInboxResponse,
     DMThreadResponse,
+    FetchedClipInfo,
     Thread,
     ThreadAction,
-    ThreadItem,
     ThreadItemType,
 )
 from .base import BaseAndroidAPI, T
 
 
 class ThreadAPI(BaseAndroidAPI):
     async def get_inbox(
         self,
         cursor: str | None = None,
         seq_id: str | None = None,
-        message_limit: int = 10,
+        message_limit: int | None = 10,
         limit: int = 20,
         pending: bool = False,
+        spam: bool = False,
         direction: str = "older",
     ) -> DMInboxResponse:
         query = {
             "visual_message_return_type": "unseen",
             "cursor": cursor,
             "direction": direction if cursor else None,
             "seq_id": seq_id,
             "thread_message_limit": message_limit,
             "persistentBadging": "true",
             "limit": limit,
+            "push_disabled": "true",
+            "is_prefetching": "false",
+        }
+        inbox_type = "inbox"
+        if pending:
+            inbox_type = "pending_inbox"
+            if spam:
+                inbox_type = "spam_inbox"
+        elif not cursor:
+            query["fetch_reason"] = "initial_snapshot"  # can also be manual_refresh
+        headers = {
+            # MainFeedFragment:feed_timeline for limit=0 cold start fetch
+            "ig-client-endpoint": "DirectInboxFragment:direct_inbox",
         }
-        inbox_type = "pending_inbox" if pending else "inbox"
         return await self.std_http_get(
             f"/api/v1/direct_v2/{inbox_type}/", query=query, response_type=DMInboxResponse
         )
 
     async def iter_inbox(
-        self, start_at: DMInboxResponse | None = None, message_limit: int = 10
+        self,
+        update_seq_id_and_cursor: Callable[[int, str | None], None],
+        start_at: DMInboxResponse | None = None,
+        local_limit: int | None = None,
+        rate_limit_exceeded_backoff: float = 60.0,
     ) -> AsyncIterable[Thread]:
+        thread_counter = 0
         if start_at:
             cursor = start_at.inbox.oldest_cursor
             seq_id = start_at.seq_id
             has_more = start_at.inbox.has_older
             for thread in start_at.inbox.threads:
                 yield thread
+                thread_counter += 1
+                if local_limit and thread_counter >= local_limit:
+                    return
+            update_seq_id_and_cursor(seq_id, cursor)
         else:
             cursor = None
             seq_id = None
             has_more = True
         while has_more:
-            resp = await self.get_inbox(message_limit=message_limit, cursor=cursor, seq_id=seq_id)
+            try:
+                resp = await self.get_inbox(cursor=cursor, seq_id=seq_id)
+            except IGRateLimitError:
+                self.log.warning(
+                    "Fetching more threads failed due to rate limit. Waiting for "
+                    f"{rate_limit_exceeded_backoff} seconds before resuming."
+                )
+                await asyncio.sleep(rate_limit_exceeded_backoff)
+                continue
+            except Exception:
+                self.log.exception("Failed to fetch more threads")
+                raise
+
             seq_id = resp.seq_id
             cursor = resp.inbox.oldest_cursor
             has_more = resp.inbox.has_older
             for thread in resp.inbox.threads:
                 yield thread
+                thread_counter += 1
+                if local_limit and thread_counter >= local_limit:
+                    return
+            update_seq_id_and_cursor(seq_id, cursor)
 
     async def get_thread(
         self,
         thread_id: str,
         cursor: str | None = None,
-        limit: int = 10,
+        limit: int = 20,
         direction: str = "older",
         seq_id: int | None = None,
     ) -> DMThreadResponse:
         query = {
             "visual_message_return_type": "unseen",
             "cursor": cursor,
             "direction": direction,
             "seq_id": seq_id,
             "limit": limit,
         }
+        headers = {
+            "ig-client-endpoint": "DirectThreadFragment:direct_thread",
+            "x-ig-nav-chain": "MainFeedFragment:feed_timeline:1:cold_start::,DirectInboxFragment:direct_inbox:4:on_launch_direct_inbox::",
+        }
         return await self.std_http_get(
             f"/api/v1/direct_v2/threads/{thread_id}/", query=query, response_type=DMThreadResponse
         )
 
-    async def iter_thread(
-        self,
-        thread_id: str,
-        seq_id: int | None = None,
-        cursor: str | None = None,
-        start_at: Thread | None = None,
-    ) -> AsyncIterable[ThreadItem]:
-        if start_at:
-            for item in start_at.items:
-                yield item
-            cursor = start_at.oldest_cursor
-            has_more = start_at.has_older
-        else:
-            has_more = True
-        while has_more:
-            resp = await self.get_thread(thread_id, seq_id=seq_id, cursor=cursor)
-            cursor = resp.thread.oldest_cursor
-            has_more = resp.thread.has_older
-            for item in resp.thread.items:
-                yield item
-
     async def create_group_thread(self, recipient_users: list[int | str]) -> Thread:
         return await self.std_http_post(
             "/api/v1/direct_v2/create_group_thread/",
             data={
                 "_csrftoken": self.state.cookies.csrf_token,
                 "_uuid": self.state.device.uuid,
                 "_uid": self.state.session.ds_user_id,
@@ -193,7 +217,14 @@
         signed: bool = False,
         client_context: str | None = None,
         **kwargs,
     ) -> CommandResponse:
         return await self._broadcast(
             thread_id, item_type.value, CommandResponse, signed, client_context, **kwargs
         )
+
+    async def fetch_clip(self, media_id: int) -> FetchedClipInfo:
+        return await self.std_http_get(
+            f"/api/v1/clips/item/",
+            query={"clips_media_id": str(media_id)},
+            response_type=FetchedClipInfo,
+        )
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/http/upload.py` & `mautrix-instagram-0.3.0/mauigpapi/http/upload.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/http/user.py` & `mautrix-instagram-0.3.0/mauigpapi/http/user.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/mqtt/conn.py` & `mautrix-instagram-0.3.0/mauigpapi/mqtt/conn.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 from collections import defaultdict
 from socket import error as SocketError, socket
 import asyncio
 import json
 import logging
 import re
 import time
-import urllib.request
 import zlib
 
 from yarl import URL
 import paho.mqtt.client as pmc
 
+from mautrix.util import background_task
 from mautrix.util.logging import TraceLogger
+from mautrix.util.proxy import ProxyHandler, proxy_with_retry
 
 from ..errors import (
     IrisSubscribeError,
     MQTTConnectionUnauthorized,
     MQTTNotConnected,
     MQTTNotLoggedIn,
+    MQTTReconnectionError,
 )
-from ..proxy import ProxyHandler
 from ..state import AndroidState
 from ..types import (
     AppPresenceEventPayload,
     ClientConfigUpdatePayload,
     CommandResponse,
     IrisPayload,
     IrisPayloadData,
@@ -53,14 +54,15 @@
     PubsubPayload,
     ReactionStatus,
     ReactionType,
     RealtimeDirectEvent,
     RealtimeZeroProvisionPayload,
     ThreadAction,
     ThreadItemType,
+    ThreadRemoveEvent,
     ThreadSyncEvent,
     TypingStatus,
 )
 from .events import Connect, Disconnect, NewSequenceID, ProxyUpdate
 from .otclient import MQTToTClient
 from .subscription import GraphQLQueryID, RealtimeTopic, everclear_subscriptions
 from .thrift import ForegroundStateConfig, IncomingMessage, RealtimeClientInfo, RealtimeConfig
@@ -74,14 +76,18 @@
 
 ACTIVITY_INDICATOR_REGEX = re.compile(
     r"/direct_v2/threads/([\w_]+)/activity_indicator_id/([\w_]+)"
 )
 
 INBOX_THREAD_REGEX = re.compile(r"/direct_v2/inbox/threads/([\w_]+)")
 
+REQUEST_TIMEOUT = 60 * 3
+DEFAULT_KEEPALIVE = 60
+REQUEST_KEEPALIVE = 5
+
 
 class AndroidMQTT:
     _loop: asyncio.AbstractEventLoop
     _client: MQTToTClient
     log: TraceLogger
     state: AndroidState
     _graphql_subs: set[str]
@@ -100,15 +106,14 @@
     _event_dispatcher_task: asyncio.Task | None
 
     # region Initialization
 
     def __init__(
         self,
         state: AndroidState,
-        loop: asyncio.AbstractEventLoop | None = None,
         log: TraceLogger | None = None,
         proxy_handler: ProxyHandler | None = None,
     ) -> None:
         self._graphql_subs = set()
         self._skywalker_subs = set()
         self._iris_seq_id = None
         self._iris_snapshot_at_ms = None
@@ -119,15 +124,15 @@
         self._message_response_waiter = None
         self._disconnect_error = None
         self._response_waiter_locks = defaultdict(lambda: asyncio.Lock())
         self._event_handlers = defaultdict(lambda: [])
         self._event_dispatcher_task = None
         self._outgoing_events = asyncio.Queue()
         self.log = log or logging.getLogger("mauigpapi.mqtt")
-        self._loop = loop or asyncio.get_event_loop()
+        self._loop = asyncio.get_running_loop()
         self.state = state
         self._client = MQTToTClient(
             client_id=self._form_client_id(),
             clean_session=True,
             protocol=pmc.MQTTv31,
             transport="tcp",
         )
@@ -146,15 +151,15 @@
         self._client.on_disconnect = self._on_disconnect_handler
         self._client.on_socket_open = self._on_socket_open
         self._client.on_socket_close = self._on_socket_close
         self._client.on_socket_register_write = self._on_socket_register_write
         self._client.on_socket_unregister_write = self._on_socket_unregister_write
 
     def setup_proxy(self):
-        http_proxy = self.proxy_handler.get_proxy_url()
+        http_proxy = self.proxy_handler.get_proxy_url() if self.proxy_handler else None
         if http_proxy:
             if not socks:
                 self.log.warning("http_proxy is set, but pysocks is not installed")
             else:
                 proxy_url = URL(http_proxy)
                 proxy_type = {
                     "http": socks.HTTP,
@@ -167,32 +172,18 @@
                     proxy_type=proxy_type,
                     proxy_addr=proxy_url.host,
                     proxy_port=proxy_url.port,
                     proxy_username=proxy_url.user,
                     proxy_password=proxy_url.password,
                 )
 
-    def _clear_response_waiters(self) -> None:
-        for waiter in self._response_waiters.values():
-            if not waiter.done():
-                waiter.set_exception(
-                    MQTTNotConnected("MQTT disconnected before request returned response")
-                )
+    def _clear_publish_waiters(self) -> None:
         for waiter in self._publish_waiters.values():
             if not waiter.done():
-                waiter.set_exception(
-                    MQTTNotConnected("MQTT disconnected before request was published")
-                )
-        if self._message_response_waiter and not self._message_response_waiter.done():
-            self._message_response_waiter.set_exception(
-                MQTTNotConnected("MQTT disconnected before message send returned response")
-            )
-            self._message_response_waiter = None
-            self._message_response_waiter_id = None
-        self._response_waiters = {}
+                waiter.set_exception(MQTTNotConnected("MQTT disconnected before PUBACK received"))
         self._publish_waiters = {}
 
     def _form_client_id(self) -> bytes:
         subscribe_topics = [
             RealtimeTopic.PUBSUB,  # 88
             RealtimeTopic.SUB_IRIS_RESPONSE,  # 135
             RealtimeTopic.RS_REQ,  # 244
@@ -203,42 +194,40 @@
             RealtimeTopic.SEND_MESSAGE_RESPONSE,  # 133
             RealtimeTopic.MESSAGE_SYNC,  # 146
             RealtimeTopic.LIGHTSPEED_RESPONSE,  # 179
             RealtimeTopic.UNKNOWN_PP,  # 34
         ]
         subscribe_topic_ids = [int(topic.encoded) for topic in subscribe_topics]
         password = f"authorization={self.state.session.authorization}"
-        # if not self.state.session.authorization:
-        #     password = f"sessionid={self.state.cookies['sessionid']}"
         cfg = RealtimeConfig(
             client_identifier=self.state.device.phone_id[:20],
             client_info=RealtimeClientInfo(
                 user_id=int(self.state.user_id),
                 user_agent=self.state.user_agent,
                 client_capabilities=0b10110111,
                 endpoint_capabilities=0,
                 publish_format=1,
                 no_automatic_foreground=True,
                 make_user_available_in_foreground=False,
                 device_id=self.state.device.phone_id,
                 is_initially_foreground=False,
                 network_type=1,
-                network_subtype=0,
+                network_subtype=-1,
                 client_mqtt_session_id=int(time.time() * 1000) & 0xFFFFFFFF,
                 subscribe_topics=subscribe_topic_ids,
                 client_type="cookie_auth",
                 app_id=567067343352427,
-                region_preference=self.state.session.region_hint or "LLA",
+                # region_preference=self.state.session.region_hint or "LLA",
                 device_secret="",
                 client_stack=3,
             ),
             password=password,
             app_specific_info={
+                "capabilities": self.state.application.CAPABILITIES,
                 "app_version": self.state.application.APP_VERSION,
-                "X-IG-Capabilities": self.state.application.CAPABILITIES,
                 "everclear_subscriptions": json.dumps(everclear_subscriptions),
                 "User-Agent": self.state.user_agent,
                 "Accept-Language": self.state.device.language.replace("_", "-"),
                 "platform": "android",
                 "ig_mqtt_route": "django",
                 "pubsub_msg_type_blacklist": "direct, typing_type",
                 "auth_cache_enabled": "1",
@@ -271,16 +260,16 @@
                 self.disconnect()
             return
 
         self._loop.create_task(self._post_connect())
 
     def _on_disconnect_handler(self, client: MQTToTClient, _: Any, rc: int) -> None:
         err_str = "Generic error." if rc == pmc.MQTT_ERR_NOMEM else pmc.error_string(rc)
-        self.log.debug(f"MQTT disconnection code %d: %s", rc, err_str)
-        self._clear_response_waiters()
+        self.log.debug("MQTT disconnection code %d: %s", rc, err_str)
+        self._clear_publish_waiters()
 
     async def _post_connect(self) -> None:
         await self._dispatch(Connect())
         self.log.debug("Re-subscribing to things after connect")
         if self._graphql_subs:
             res = await self.graphql_subscribe(self._graphql_subs)
             self.log.trace("GraphQL subscribe response: %s", res)
@@ -306,15 +295,16 @@
     def _on_publish_handler(self, client: MQTToTClient, _: Any, mid: int) -> None:
         try:
             waiter = self._publish_waiters[mid]
         except KeyError:
             self.log.trace(f"Got publish confirmation for {mid}, but no waiters")
             return
         self.log.trace(f"Got publish confirmation for {mid}")
-        waiter.set_result(None)
+        if not waiter.done():
+            waiter.set_result(None)
 
     # region Incoming event parsing
 
     def _parse_direct_thread_path(self, path: str) -> dict:
         try:
             blank, direct_v2, threads, thread_id, *rest = path.split("/")
         except (ValueError, IndexError) as e:
@@ -324,14 +314,16 @@
             self.log.debug(f"Got unexpected first parts in direct thread path {path}")
             raise ValueError("unexpected first three parts in _parse_direct_thread_path")
         additional = {"thread_id": thread_id}
         if rest:
             subitem_key = rest[0]
             if subitem_key == "approval_required_for_new_members":
                 additional["approval_required_for_new_members"] = True
+            elif subitem_key == "thread_image":
+                additional["is_thread_image"] = True
             elif subitem_key == "participants" and len(rest) > 2 and rest[2] == "has_seen":
                 additional["has_seen"] = int(rest[1])
             elif subitem_key == "items":
                 additional["item_id"] = rest[1]
                 if len(rest) > 4 and rest[2] == "reactions":
                     additional["reaction_type"] = ReactionType(rest[3])
                     additional["reaction_user_id"] = int(rest[4])
@@ -366,20 +358,32 @@
                         **json_value,
                     }
             except (json.JSONDecodeError, TypeError):
                 raw_message["value"] = part.value
             message = MessageSyncMessage.deserialize(raw_message)
             evt = MessageSyncEvent(iris=parsed_item, message=message)
         elif part.path.startswith("/direct_v2/inbox/threads/"):
-            raw_message = {
-                "path": part.path,
-                "op": part.op,
-                **json.loads(part.value),
-            }
-            evt = ThreadSyncEvent.deserialize(raw_message)
+            if part.op == Operation.REMOVE:
+                blank, direct_v2, inbox, threads, thread_id, *_ = part.path.split("/")
+                evt = ThreadRemoveEvent.deserialize(
+                    {
+                        "thread_id": thread_id,
+                        "path": part.path,
+                        "op": part.op,
+                        **json.loads(part.value),
+                    }
+                )
+            else:
+                evt = ThreadSyncEvent.deserialize(
+                    {
+                        "path": part.path,
+                        "op": part.op,
+                        **json.loads(part.value),
+                    }
+                )
         else:
             self.log.warning(f"Unsupported path {part.path}")
             return False
         self._outgoing_events.put_nowait(evt)
         return True
 
     def _on_message_sync(self, payload: bytes) -> None:
@@ -388,15 +392,15 @@
         has_items = False
         for sync_item in parsed:
             parsed_item = IrisPayload.deserialize(sync_item)
             if self._iris_seq_id < parsed_item.seq_id:
                 self.log.trace(f"Got new seq_id: {parsed_item.seq_id}")
                 self._iris_seq_id = parsed_item.seq_id
                 self._iris_snapshot_at_ms = int(time.time() * 1000)
-                asyncio.create_task(
+                background_task.create(
                     self._dispatch(NewSequenceID(self._iris_seq_id, self._iris_snapshot_at_ms))
                 )
             for part in parsed_item.data:
                 has_items = self._on_messager_sync_item(part, parsed_item) or has_items
         if has_items and not self._event_dispatcher_task:
             self._event_dispatcher_task = asyncio.create_task(self._dispatcher_loop())
 
@@ -493,37 +497,47 @@
                 self._on_message_sync(message.payload)
             elif topic == RealtimeTopic.PUBSUB:
                 self._on_pubsub(message.payload)
             elif topic == RealtimeTopic.REALTIME_SUB:
                 self._on_realtime_sub(message.payload)
             elif topic == RealtimeTopic.SEND_MESSAGE_RESPONSE:
                 self._handle_send_response(message)
+            elif topic == RealtimeTopic.UNKNOWN_PP:
+                self.log.warning("Reconnecting after receiving /pp message")
+                background_task.create(self._reconnect())
             else:
                 try:
                     waiter = self._response_waiters.pop(topic)
                 except KeyError:
                     self.log.debug(
                         "No handler for MQTT message in %s: %s", topic.value, message.payload
                     )
                 else:
-                    self.log.trace("Got response %s: %s", topic.value, message.payload)
-                    waiter.set_result(message)
+                    if not waiter.done():
+                        waiter.set_result(message)
+                        self.log.trace("Got response %s: %s", topic.value, message.payload)
+                    else:
+                        self.log.debug(
+                            "Got response in %s, but waiter was already cancelled: %s",
+                            topic,
+                            message.payload,
+                        )
         except Exception:
             self.log.exception("Error in incoming MQTT message handler")
             self.log.trace("Errored MQTT payload: %s", message.payload)
 
     # endregion
 
     async def _reconnect(self) -> None:
         try:
-            self.log.trace("Trying to reconnect to MQTT")
             self._client.reconnect()
+            return
         except (SocketError, OSError, pmc.WebsocketConnectionError) as e:
-            # TODO custom class
-            raise MQTTNotLoggedIn("MQTT reconnection failed") from e
+            self.log.exception("Error reconnecting to MQTT")
+            raise MQTTReconnectionError("MQTT reconnection failed") from e
 
     def add_event_handler(
         self, evt_type: Type[T], handler: Callable[[T], Awaitable[None]]
     ) -> None:
         self._event_handlers[evt_type].append(handler)
 
     async def _dispatch(self, evt: T) -> None:
@@ -558,112 +572,148 @@
 
     async def listen(
         self,
         graphql_subs: set[str] | None = None,
         skywalker_subs: set[str] | None = None,
         seq_id: int = None,
         snapshot_at_ms: int = None,
-        retry_limit: int = 5,
+        retry_limit: int = 10,
     ) -> None:
         self._graphql_subs = graphql_subs or set()
         self._skywalker_subs = skywalker_subs or set()
         self._iris_seq_id = seq_id
         self._iris_snapshot_at_ms = snapshot_at_ms
 
         self.log.debug("Connecting to Instagram MQTT")
-        await self._reconnect()
-        connection_retries = 0
 
-        while True:
-            try:
-                await asyncio.sleep(1)
-            except asyncio.CancelledError:
-                self.disconnect()
-                # this might not be necessary
-                self._client.loop_misc()
-                break
-            rc = self._client.loop_misc()
-
-            # If disconnect() has been called
-            # Beware, internal API, may have to change this to something more stable!
-            if self._client._state == pmc.mqtt_cs_disconnecting:
-                break  # Stop listening
-
-            if rc != pmc.MQTT_ERR_SUCCESS:
-                # If known/expected error
-                if rc == pmc.MQTT_ERR_CONN_LOST:
-                    await self._dispatch(Disconnect(reason="Connection lost, retrying"))
-                elif rc == pmc.MQTT_ERR_NOMEM:
-                    # This error is wrongly classified
-                    # See https://github.com/eclipse/paho.mqtt.python/issues/340
-                    await self._dispatch(Disconnect(reason="Connection lost, retrying"))
-                elif rc == pmc.MQTT_ERR_CONN_REFUSED:
-                    raise MQTTNotLoggedIn("MQTT connection refused")
-                elif rc == pmc.MQTT_ERR_NO_CONN:
-                    if connection_retries > retry_limit:
-                        raise MQTTNotConnected(f"Connection failed {connection_retries} times")
-                    if self.proxy_handler.update_proxy_url():
-                        self.setup_proxy()
-                        await self._dispatch(ProxyUpdate())
-                    sleep = connection_retries * 2
-                    await self._dispatch(
-                        Disconnect(
-                            reason="MQTT Error: no connection, retrying "
-                            f"in {connection_retries} seconds"
-                        )
-                    )
-                    await asyncio.sleep(sleep)
-                else:
-                    err = pmc.error_string(rc)
-                    self.log.error("MQTT Error: %s", err)
-                    await self._dispatch(Disconnect(reason=f"MQTT Error: {err}, retrying"))
+        async def connect_and_watch():
+            await self._reconnect()
+
+            while True:
+                try:
+                    await asyncio.sleep(1)
+                except asyncio.CancelledError:
+                    self.disconnect()
+                    # this might not be necessary
+                    self._client.loop_misc()
+                    return
+                rc = self._client.loop_misc()
+
+                # If disconnect() has been called
+                # Beware, internal API, may have to change this to something more stable!
+                if self._client._state == pmc.mqtt_cs_disconnecting:
+                    return  # Stop listening
+
+                if rc != pmc.MQTT_ERR_SUCCESS:
+                    # If known/expected error
+                    if rc == pmc.MQTT_ERR_CONN_LOST:
+                        await self._dispatch(Disconnect(reason="Connection lost, retrying"))
+                        raise MQTTNotConnected("MQTT_ERR_CONN_LOST")
+                    elif rc == pmc.MQTT_ERR_NOMEM:
+                        # This error is wrongly classified
+                        # See https://github.com/eclipse/paho.mqtt.python/issues/340
+                        await self._dispatch(Disconnect(reason="Connection lost, retrying"))
+                        raise MQTTNotConnected("MQTT_ERR_NOMEM")
+                    elif rc == pmc.MQTT_ERR_CONN_REFUSED:
+                        await self._dispatch(Disconnect(reason="Connection refused, retrying"))
+                        raise MQTTNotLoggedIn("MQTT_ERR_CONN_REFUSED")
+                    elif rc == pmc.MQTT_ERR_NO_CONN:
+                        await self._dispatch(Disconnect(reason="Connection dropped, retrying"))
+                        raise MQTTNotConnected("MQTT_ERR_NO_CONN")
+                    else:
+                        err = pmc.error_string(rc)
+                        self.log.error("MQTT Error: %s", err)
+                        await self._dispatch(Disconnect(reason=f"MQTT Error: {err}, retrying"))
+                        raise MQTTNotConnected(err)
+
+        await proxy_with_retry(
+            "mqtt.listen",
+            lambda: connect_and_watch(),
+            logger=self.log,
+            proxy_handler=self.proxy_handler,
+            on_proxy_change=lambda: self._dispatch(ProxyUpdate()),
+            max_retries=retry_limit,
+            retryable_exceptions=(MQTTNotConnected, MQTTReconnectionError),
+            # Wait 1s * errors, max 5s for fast reconnect or die
+            max_wait_seconds=5,
+            multiply_wait_seconds=1,
+            # If connection stable for >1h, reset the error counter
+            reset_after_seconds=3600,
+        )
 
-                await self._reconnect()
-                connection_retries += 1
-            else:
-                connection_retries = 0
         if self._event_dispatcher_task:
             self._event_dispatcher_task.cancel()
             self._event_dispatcher_task = None
         if self._disconnect_error:
             self.log.info("disconnect_error is set, raising and clearing variable")
             err = self._disconnect_error
             self._disconnect_error = None
             raise err
 
     # region Basic outgoing MQTT
 
+    @staticmethod
+    def _publish_cancel_later(fut: asyncio.Future) -> None:
+        if not fut.done():
+            fut.set_exception(asyncio.TimeoutError("MQTT publish timed out"))
+
+    @staticmethod
+    def _request_cancel_later(fut: asyncio.Future) -> None:
+        if not fut.done():
+            fut.set_exception(asyncio.TimeoutError("MQTT request timed out"))
+
+    # The following two functions mutate the client keepalive (cheeky) to temporarily increase
+    # ping attempts during read/write to MQTT. If things are flowing this should change nothing,
+    # as pings only send when idle. It should, however, allow the client to detect a bad MQTT
+    # connection much quicker than the default keepalive.
+    def set_request_keepalive(self):
+        self._client._keepalive = REQUEST_KEEPALIVE
+
+    def maybe_reset_keepalive(self):
+        # Reset the keepalive back to the default value if we have no pending publish/receive
+        if not self._response_waiters and not self._publish_waiters:
+            self._client._keepalive = DEFAULT_KEEPALIVE
+
     def publish(self, topic: RealtimeTopic, payload: str | bytes | dict) -> asyncio.Future:
         if isinstance(payload, dict):
             payload = json.dumps(payload)
         if isinstance(payload, str):
             payload = payload.encode("utf-8")
         self.log.trace(f"Publishing message in {topic.value} ({topic.encoded}): {payload}")
         payload = zlib.compress(payload, level=9)
+        self.set_request_keepalive()
         info = self._client.publish(topic.encoded, payload, qos=1)
         self.log.trace(f"Published message ID: {info.mid}")
-        fut = asyncio.Future()
+        fut = self._loop.create_future()
+        timeout_handle = self._loop.call_later(REQUEST_TIMEOUT, self._publish_cancel_later, fut)
+        fut.add_done_callback(lambda _: timeout_handle.cancel())
+        fut.add_done_callback(lambda _: self.maybe_reset_keepalive())
         self._publish_waiters[info.mid] = fut
         return fut
 
     async def request(
         self,
         topic: RealtimeTopic,
         response: RealtimeTopic,
         payload: str | bytes | dict,
         timeout: int | None = None,
     ) -> pmc.MQTTMessage:
         async with self._response_waiter_locks[response]:
-            fut = asyncio.Future()
+            fut = self._loop.create_future()
             self._response_waiters[response] = fut
-            await self.publish(topic, payload)
+            background_task.create(self.publish(topic, payload))
             self.log.trace(
-                f"Request published to {topic.value}, waiting for response {response.name}"
+                f"Request publish to {topic.value} queued, waiting for response {response.name}"
             )
-            return await asyncio.wait_for(fut, timeout)
+            timeout_handle = self._loop.call_later(
+                timeout or REQUEST_TIMEOUT, self._request_cancel_later, fut
+            )
+            fut.add_done_callback(lambda _: timeout_handle.cancel())
+            fut.add_done_callback(lambda _: self.maybe_reset_keepalive())
+            return await fut
 
     async def iris_subscribe(self, seq_id: int, snapshot_at_ms: int) -> None:
         self.log.debug(f"Requesting iris subscribe {seq_id}/{snapshot_at_ms}")
         resp = await self.request(
             RealtimeTopic.SUB_IRIS,
             RealtimeTopic.SUB_IRIS_RESPONSE,
             {
@@ -680,15 +730,15 @@
         if resp_dict["error_type"] and resp_dict["error_message"]:
             raise IrisSubscribeError(resp_dict["error_type"], resp_dict["error_message"])
         latest_seq_id = resp_dict.get("latest_seq_id")
         if latest_seq_id > self._iris_seq_id:
             self.log.info(f"Latest sequence ID is {latest_seq_id}, catching up from {seq_id}")
             self._iris_seq_id = latest_seq_id
             self._iris_snapshot_at_ms = resp_dict.get("subscribed_at_ms", int(time.time() * 1000))
-            asyncio.create_task(
+            background_task.create(
                 self._dispatch(NewSequenceID(self._iris_seq_id, self._iris_snapshot_at_ms))
             )
 
     def graphql_subscribe(self, subs: set[str]) -> asyncio.Future:
         self._graphql_subs |= subs
         return self.publish(RealtimeTopic.REALTIME_SUB, {"sub": list(subs)})
 
@@ -718,37 +768,39 @@
     async def send_command(
         self,
         thread_id: str,
         action: ThreadAction,
         client_context: str | None = None,
         **kwargs: Any,
     ) -> CommandResponse | None:
+        self.log.debug(f"Preparing to send {action} to {thread_id} with {client_context}")
         client_context = client_context or self.state.gen_client_context()
         req = {
             "thread_id": thread_id,
             "client_context": client_context,
             "offline_threading_id": client_context,
             "action": action.value,
             # "device_id": self.state.cookies["ig_did"],
             **kwargs,
         }
         lock_start = time.monotonic()
         async with self._message_response_waiter_lock:
             lock_wait_dur = time.monotonic() - lock_start
             if lock_wait_dur > 1:
-                self.log.debug(f"Waited {lock_wait_dur:.3f} seconds to send {client_context}")
+                self.log.warning(f"Waited {lock_wait_dur:.3f} seconds to send {client_context}")
             fut = self._message_response_waiter = asyncio.Future()
             self._message_response_waiter_id = client_context
-            await self.publish(RealtimeTopic.SEND_MESSAGE, req)
-            self.log.trace(
-                f"Request published to {RealtimeTopic.SEND_MESSAGE}, "
+            background_task.create(self.publish(RealtimeTopic.SEND_MESSAGE, req))
+            self.log.debug(
+                f"Request publish to {RealtimeTopic.SEND_MESSAGE} queued, "
                 f"waiting for response {RealtimeTopic.SEND_MESSAGE_RESPONSE}"
             )
+            fut.add_done_callback(lambda _: self.maybe_reset_keepalive())
             try:
-                resp = await asyncio.wait_for(fut, timeout=30000)
+                resp = await asyncio.wait_for(fut, timeout=REQUEST_TIMEOUT)
             except asyncio.TimeoutError:
                 self.log.error(f"Request with ID {client_context} timed out!")
                 raise
             return CommandResponse.parse_json(resp.payload.decode("utf-8"))
 
     def send_item(
         self,
@@ -891,25 +943,29 @@
         thread_id: str,
         text: str = "",
         urls: list[str] | None = None,
         shh_mode: bool = False,
         client_context: str | None = None,
         replied_to_item_id: str | None = None,
         replied_to_client_context: str | None = None,
+        mentioned_user_ids: list[int] | None = None,
     ) -> Awaitable[CommandResponse]:
         args = {
             "text": text,
         }
         item_type = ThreadItemType.TEXT
         if urls is not None:
             args = {
                 "link_text": text,
                 "link_urls": json.dumps(urls or []),
             }
             item_type = ThreadItemType.LINK
+        if mentioned_user_ids:
+            args["mentioned_user_ids"] = json.dumps([str(x) for x in mentioned_user_ids])
+            args["sampled"] = True
         return self.send_item(
             thread_id,
             **args,
             shh_mode=shh_mode,
             item_type=item_type,
             client_context=client_context,
             replied_to_item_id=replied_to_item_id,
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/mqtt/events.py` & `mautrix-instagram-0.3.0/mauigpapi/mqtt/events.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/mqtt/otclient.py` & `mautrix-instagram-0.3.0/mauigpapi/mqtt/otclient.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/mqtt/subscription.py` & `mautrix-instagram-0.3.0/mauigpapi/mqtt/subscription.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/mqtt/thrift/autospec.py` & `mautrix-instagram-0.3.0/mauigpapi/mqtt/thrift/autospec.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/mqtt/thrift/ig_objects.py` & `mautrix-instagram-0.3.0/mauigpapi/mqtt/thrift/ig_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,35 +40,35 @@
     client_mqtt_session_id: int = field(TType.I64)
     client_ip_address: str = None
     subscribe_topics: List[int] = field(TType.LIST, TType.I32)
     client_type: str
     app_id: int = field(TType.I64)
     override_nectar_logging: bool = None
     connect_token_hash: str = None
-    region_preference: str
+    region_preference: str = None
     device_secret: str
     client_stack: int = field(TType.BYTE)
     fbns_connection_key: int = field(TType.I64, default=None)
     fbns_connection_secret: str = None
     fbns_device_id: str = None
     fbns_device_secret: str = None
-    another_unknown: int = field(TType.I64, default=None)
+    luid: int = field(TType.I64, default=None)
 
 
 @autospec
 @dataclass(kw_only=True)
 class RealtimeConfig:
     client_identifier: str
     will_topic: str = None
     will_message: str = None
     client_info: RealtimeClientInfo
     password: str
     get_diffs_request: List[str] = None
     zero_rating_token_hash: str = None
-    app_specific_info: Dict[str, str]
+    app_specific_info: Dict[str, str] = None
 
     def to_thrift(self) -> bytes:
         buf = ThriftWriter()
         buf.write_struct(self)
         return buf.getvalue()
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/mqtt/thrift/read.py` & `mautrix-instagram-0.3.0/mauigpapi/mqtt/thrift/read.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/mqtt/thrift/type.py` & `mautrix-instagram-0.3.0/mauigpapi/mqtt/thrift/type.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/mqtt/thrift/write.py` & `mautrix-instagram-0.3.0/mauigpapi/mqtt/thrift/write.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/state/cookies.py` & `mautrix-instagram-0.3.0/mauigpapi/state/cookies.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/state/device.py` & `mautrix-instagram-0.3.0/mauigpapi/state/device.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mautrix-instagram - A Matrix-Instagram puppeting bridge.
-# Copyright (C) 2020 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -11,38 +11,33 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from typing import Optional, Union
 from uuid import UUID
-import json
-import pkgutil
 import random
 import string
 import time
 
 from attr import dataclass
 import attr
 
 from mautrix.types import SerializableAttrs
 
-builds = json.loads(pkgutil.get_data("mauigpapi.state", "samples/builds.json"))
-descriptors = json.loads(pkgutil.get_data("mauigpapi.state", "samples/devices.json"))
-
 
 @dataclass
 class AndroidDevice(SerializableAttrs):
     id: Optional[str] = None
     descriptor: Optional[str] = None
     uuid: Optional[str] = None
+    fdid: Optional[str] = None
     phone_id: Optional[str] = attr.ib(default=None, metadata={"json": "phoneId"})
     # Google Play advertising ID
     adid: Optional[str] = None
-    build: Optional[str] = None
 
     language: str = "en_US"
     radio_type: str = "wifi-none"
     connection_type: str = "WIFI"
     timezone_offset: str = str(-time.timezone)
     is_layout_rtl: bool = False
 
@@ -70,11 +65,12 @@
             "model": model,
         }
 
     def generate(self, seed: Union[str, bytes]) -> None:
         rand = random.Random(seed)
         self.phone_id = str(UUID(int=rand.getrandbits(128), version=4))
         self.adid = str(UUID(int=rand.getrandbits(128), version=4))
-        self.id = f"android-{''.join(rand.choices(string.hexdigits, k=16))}"
-        self.descriptor = rand.choice(descriptors)
+        self.id = f"android-{''.join(rand.choices(string.hexdigits, k=16))}".lower()
+        self.descriptor = "33/13; 420dpi; 1080x2219; Google/google; Pixel 6; oriole; oriole"
+        # "33/13; 560dpi; 1440x2934; Google/google; Pixel 6 Pro; raven; raven",
         self.uuid = str(UUID(int=rand.getrandbits(128), version=4))
-        self.build = rand.choice(builds)
+        self.fdid = str(UUID(int=rand.getrandbits(128), version=4))
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/state/experiments.py` & `mautrix-instagram-0.3.0/mauigpapi/state/application.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # mautrix-instagram - A Matrix-Instagram puppeting bridge.
-# Copyright (C) 2021 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
-from typing import Dict
+from attr import dataclass
 
-from ..types import AndroidExperiment, QeSyncResponse
+from mautrix.types import SerializableAttrs
 
 
-class AndroidExperiments:
-    experiments: Dict[str, AndroidExperiment]
+@dataclass
+class AndroidApplication(SerializableAttrs):
+    APP_VERSION: str = "256.0.0.18.105"
+    APP_VERSION_CODE: str = "407842973"
+    FACEBOOK_ANALYTICS_APPLICATION_ID: str = "567067343352427"
 
-    def __init__(self) -> None:
-        self.experiments = {}
-
-    def update(self, updated: QeSyncResponse) -> None:
-        self.experiments.update({item.name: item.parse() for item in updated.experiments})
+    BLOKS_VERSION_ID: str = "0928297a84f74885ff39fc1628f8a40da3ef1c467555d555bfd9f8fe1aaacafe"
+    CAPABILITIES: str = "3brTv10="
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/state/session.py` & `mautrix-instagram-0.3.0/mauigpapi/state/session.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 from attr import dataclass
 
 from mautrix.types import SerializableAttrs
 
 
 @dataclass
 class AndroidSession(SerializableAttrs):
-    eu_dc_enabled: Optional[bool] = None
-    thumbnail_cache_busting_value: int = 1000
     ads_opt_out: bool = False
 
     ig_www_claim: Optional[str] = None
     authorization: Optional[str] = None
     password_encryption_pubkey: Optional[str] = None
     password_encryption_key_id: Union[None, str, int] = None
     region_hint: Optional[str] = None
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/state/state.py` & `mautrix-instagram-0.3.0/mauigpapi/state/state.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,56 +10,54 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from typing import Optional
-from uuid import UUID
+from uuid import uuid4
 import random
 import time
 
 from attr import dataclass
 
 from mautrix.types import SerializableAttrs, field
 
 from ..errors import IGNoChallengeError, IGUserIDNotFoundError
 from ..types import ChallengeContext, ChallengeStateResponse
 from .application import AndroidApplication
 from .cookies import Cookies
 from .device import AndroidDevice
-from .experiments import AndroidExperiments
 from .session import AndroidSession
 
 
 @dataclass
 class AndroidState(SerializableAttrs):
     device: AndroidDevice = field(factory=lambda: AndroidDevice())
     session: AndroidSession = field(factory=lambda: AndroidSession())
-    application: AndroidApplication = field(factory=lambda: AndroidApplication())
-    experiments: AndroidExperiments = field(factory=lambda: AndroidExperiments(), hidden=True)
-    client_session_id_lifetime: int = 1_200_000
-    pigeon_session_id_lifetime: int = 1_200_000
+    application: AndroidApplication = field(factory=lambda: AndroidApplication(), hidden=True)
     challenge: Optional[ChallengeStateResponse] = None
     challenge_context: Optional[ChallengeContext] = None
     _challenge_path: Optional[str] = field(default=None, json="challenge_path")
     cookies: Cookies = field(factory=lambda: Cookies())
     login_2fa_username: Optional[str] = field(default=None, hidden=True)
+    _pigeon_session_id: Optional[str] = field(default=None, hidden=True)
 
     def __attrs_post_init__(self) -> None:
         if self.application.APP_VERSION_CODE != AndroidApplication().APP_VERSION_CODE:
             self.application = AndroidApplication()
 
     @property
-    def client_session_id(self) -> str:
-        return str(self._gen_temp_uuid("clientSessionId", self.client_session_id_lifetime))
-
-    @property
     def pigeon_session_id(self) -> str:
-        return str(self._gen_temp_uuid("pigeonSessionId", self.pigeon_session_id_lifetime))
+        if not self._pigeon_session_id:
+            self._pigeon_session_id = str(uuid4())
+        return self._pigeon_session_id
+
+    def reset_pigeon_session_id(self) -> None:
+        self._pigeon_session_id = None
 
     @property
     def user_agent(self) -> str:
         return (
             f"Instagram {self.application.APP_VERSION} Android ({self.device.descriptor}; "
             f"{self.device.language}; {self.application.APP_VERSION_CODE})"
         )
@@ -82,11 +80,7 @@
     @challenge_path.setter
     def challenge_path(self, val: str) -> None:
         self._challenge_path = val
 
     @staticmethod
     def gen_client_context() -> str:
         return str((int(time.time() * 1000) << 22) + random.randint(10000, 5000000))
-
-    def _gen_temp_uuid(self, seed: str, lifetime: int) -> UUID:
-        rand = random.Random(f"{seed}{self.device.id}{round(time.time() * 1000 / lifetime)}")
-        return UUID(int=rand.getrandbits(128), version=4)
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/types/__init__.py` & `mautrix-instagram-0.3.0/mauigpapi/types/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,29 +53,31 @@
     PubsubPayloadData,
     PubsubPublishMetadata,
     ReactionStatus,
     RealtimeDirectData,
     RealtimeDirectEvent,
     RealtimeZeroProvisionPayload,
     ThreadAction,
+    ThreadRemoveEvent,
     ThreadSyncEvent,
     TypingStatus,
     ZeroProductProvisioningEvent,
 )
 from .qe import AndroidExperiment, QeSyncExperiment, QeSyncExperimentParam, QeSyncResponse
-from .thread import Thread, ThreadItem, ThreadTheme, ThreadUser, ThreadUserLastSeenAt
+from .thread import Thread, ThreadTheme, ThreadUser, ThreadUserLastSeenAt
 from .thread_item import (
     AnimatedMediaImage,
     AnimatedMediaImages,
     AnimatedMediaItem,
     AudioInfo,
     Caption,
     CreateModeAttribution,
     CreativeConfig,
     ExpiredMediaItem,
+    FetchedClipInfo,
     ImageVersion,
     ImageVersions,
     LinkContext,
     LinkItem,
     Location,
     MediaShareItem,
     MediaType,
@@ -85,14 +87,15 @@
     ReelMediaShareItem,
     ReelShareItem,
     ReelShareReactionInfo,
     ReelShareType,
     RegularMediaItem,
     ReplayableMediaItem,
     SharingFrictionInfo,
+    ThreadImage,
     ThreadItem,
     ThreadItemActionLog,
     ThreadItemType,
     VideoVersion,
     ViewMode,
     VisualMedia,
     VoiceMediaData,
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/types/account.py` & `mautrix-instagram-0.3.0/mauigpapi/types/account.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 class UserIdentifier(SerializableAttrs):
     pk: int
     username: str
 
 
 @dataclass(kw_only=True)
 class BaseResponseUser(UserIdentifier, SerializableAttrs):
-    full_name: str
+    full_name: Optional[str] = None
     is_private: bool = False
     is_verified: bool = False
     profile_pic_url: str
     profile_pic_id: Optional[str] = None
     has_anonymous_profile_picture: bool = False
     # TODO find type
     account_badges: Optional[List[Any]] = None
@@ -101,27 +101,25 @@
     FEMALE = 2
     UNSET = 3
     CUSTOM = 4
 
 
 @dataclass(kw_only=True)
 class CurrentUser(BaseFullResponseUser, SerializableAttrs):
-    biography: str
-    can_link_entities_in_bio: bool
-    biography_with_entities: EntityText
-    external_url: str
+    biography: Optional[str] = None
+    can_link_entities_in_bio: bool = True
+    biography_with_entities: Optional[EntityText] = None
+    external_url: Optional[str] = None
     has_biography_translation: bool = False
     hd_profile_pic_versions: List[HDProfilePictureVersion] = attr.ib(factory=lambda: [])
-    hd_profile_pic_url_info: HDProfilePictureVersion
-    show_conversion_edit_entry: bool
-    # TODO type
-    # birthday: Any
-    gender: Gender
-    custom_gender: str
-    email: str
-    profile_edit_params: Dict[str, ProfileEditParams]
+    show_conversion_edit_entry: bool = True
+    birthday: Optional[str] = None
+    gender: Gender = Gender.UNSET
+    custom_gender: Optional[str] = None
+    email: Optional[str] = None
+    profile_edit_params: Dict[str, ProfileEditParams] = attr.ib(factory=lambda: {})
 
 
 @dataclass
 class CurrentUserResponse(SerializableAttrs):
     status: str
     user: CurrentUser
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/types/challenge.py` & `mautrix-instagram-0.3.0/mauigpapi/types/challenge.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/types/direct_inbox.py` & `mautrix-instagram-0.3.0/mauigpapi/types/direct_inbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,20 +40,20 @@
     newest_cursor: Optional[str] = None
     oldest_cursor: Optional[str] = None
 
 
 @dataclass
 class DMInboxResponse(SerializableAttrs):
     status: str
-    seq_id: int
-    snapshot_at_ms: int
     pending_requests_total: int
     has_pending_top_requests: bool
-    viewer: ThreadUser
-    inbox: DMInbox
+    seq_id: Optional[int] = None
+    snapshot_at_ms: Optional[int] = None
+    viewer: Optional[ThreadUser] = None
+    inbox: Optional[DMInbox] = None
     # TODO type
     most_recent_inviter: Any = None
 
 
 @dataclass
 class DMThreadResponse(SerializableAttrs):
     thread: Thread
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/types/error.py` & `mautrix-instagram-0.3.0/mauigpapi/types/error.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/types/login.py` & `mautrix-instagram-0.3.0/mauigpapi/types/login.py`

 * *Files 21% similar despite different names*

```diff
@@ -42,23 +42,24 @@
     total_igtv_videos: int
     interop_messaging_user_fbid: int
     is_using_unified_inbox_for_direct: bool
 
 
 @dataclass
 class LoginResponse(SerializableAttrs):
-    logged_in_user: LoginResponseUser
     status: str
+    logged_in_user: Optional[LoginResponseUser] = None
 
 
 @dataclass
 class FacebookLoginResponse(LoginResponse, SerializableAttrs):
     code: int = 0
     fb_access_token: Optional[str] = None
     fb_user_id: Optional[str] = None
     session_flush_nonce: Optional[str] = None
+    account_created: bool = True
 
 
 @dataclass
 class LogoutResponse(SerializableAttrs):
     status: str
     login_nonce: Optional[str] = None
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/types/mqtt.py` & `mautrix-instagram-0.3.0/mauigpapi/types/mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 class MessageSyncMessage(ThreadItem, SerializableAttrs):
     path: str
     op: Operation = Operation.ADD
 
     # These come from parsing the path
     admin_user_id: Optional[int] = None
     approval_required_for_new_members: Optional[bool] = None
+    is_thread_image: Optional[bool] = None
     has_seen: Optional[int] = None
     thread_id: Optional[str] = None
 
 
 @dataclass(kw_only=True)
 class MessageSyncEvent(SerializableAttrs):
     iris: IrisPayload
@@ -122,14 +123,23 @@
 
 @dataclass
 class ThreadSyncEvent(Thread, SerializableAttrs):
     path: str
     op: Operation
 
 
+@dataclass
+class ThreadRemoveEvent(SerializableAttrs):
+    thread_id: str
+
+    path: str
+    op: Operation
+    data: Any = None
+
+
 @dataclass(kw_only=True)
 class PubsubPublishMetadata(SerializableAttrs):
     publish_time_ms: str
     topic_publish_id: int
 
 
 @dataclass(kw_only=True)
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/types/qe.py` & `mautrix-instagram-0.3.0/mauigpapi/types/qe.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/types/thread.py` & `mautrix-instagram-0.3.0/mauigpapi/types/thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from attr import dataclass
 import attr
 
 from mautrix.types import SerializableAttrs
 
 from .account import BaseResponseUser
-from .thread_item import ThreadItem
+from .thread_item import ThreadImage, ThreadItem
 
 
 @dataclass
 class ThreadUser(BaseResponseUser, SerializableAttrs):
     interop_messaging_user_fbid: int
     interop_user_type: Optional[int] = None
     is_using_unified_inbox_for_direct: Optional[bool] = None
@@ -81,14 +81,16 @@
     last_non_sender_item_at: int
     assigned_admin_id: int
     shh_mode_enabled: bool
     is_close_friend_thread: bool
     has_older: bool
     has_newer: bool
 
+    thread_image: Optional[ThreadImage] = None
+
     theme: ThreadTheme
     last_seen_at: Dict[str, ThreadUserLastSeenAt] = attr.ib(factory=lambda: {})
 
     newest_cursor: Optional[str] = None
     oldest_cursor: Optional[str] = None
     next_cursor: Optional[str] = None
     prev_cursor: Optional[str] = None
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/types/thread_item.py` & `mautrix-instagram-0.3.0/mauigpapi/types/thread_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from typing import List, Optional, Union
 import logging
 
 from attr import dataclass
+from yarl import URL
 import attr
 
 from mautrix.types import (
     JSON,
     ExtensibleEnum,
     Obj,
     SerializableAttrs,
@@ -77,14 +78,17 @@
     REACTION = "reaction"
     CLIP = "clip"
     GUIDE_SHARE = "guide_share"
     XMA_MEDIA_SHARE = "xma_media_share"
     XMA_REEL_SHARE = "xma_reel_share"
     XMA_STORY_SHARE = "xma_story_share"
     XMA_REEL_MENTION = "xma_reel_mention"
+    XMA_CLIP = "xma_clip"
+    EXPIRED_PLACEHOLDER = "expired_placeholder"
+    AVATAR_STICKER = "avatar_sticker"
 
 
 @dataclass(kw_only=True)
 class ThreadItemActionLog(SerializableAttrs):
     description: str
     # TODO bold, text_attributes
 
@@ -117,14 +121,33 @@
 
 
 @dataclass(kw_only=True)
 class ImageVersions(SerializableAttrs):
     candidates: List[ImageVersion]
 
 
+@dataclass
+class ImageVersionsContainer(SerializableAttrs):
+    image_versions2: Optional[ImageVersions] = None
+    original_width: Optional[int] = None
+    original_height: Optional[int] = None
+
+    @property
+    def best_image(self) -> Optional[ImageVersion]:
+        if not self.image_versions2:
+            return None
+        best: Optional[ImageVersion] = None
+        for version in self.image_versions2.candidates:
+            if version.width == self.original_width and version.height == self.original_height:
+                return version
+            elif not best or (version.width * version.height > best.width * best.height):
+                best = version
+        return best
+
+
 @dataclass(kw_only=True)
 class VideoVersion(SerializableAttrs):
     type: int
     width: int
     height: int
     url: str
     id: Optional[str] = None
@@ -149,41 +172,26 @@
 @dataclass(kw_only=True)
 class ExpiredMediaItem(SerializableAttrs):
     media_type: Optional[MediaType] = None
     user: Optional[BaseResponseUser] = None
 
 
 @dataclass(kw_only=True)
-class RegularMediaItem(SerializableAttrs):
+class RegularMediaItem(ImageVersionsContainer, SerializableAttrs):
     id: str
-    image_versions2: Optional[ImageVersions] = None
     video_versions: Optional[List[VideoVersion]] = None
-    original_width: Optional[int] = None
-    original_height: Optional[int] = None
     media_type: MediaType
     media_id: Optional[int] = None
     organic_tracking_token: Optional[str] = None
     creative_config: Optional[CreativeConfig] = None
     create_mode_attribution: Optional[CreateModeAttribution] = None
     is_commercial: Optional[bool] = None
     commerciality_status: Optional[str] = None  # TODO enum? commercial
 
     @property
-    def best_image(self) -> Optional[ImageVersion]:
-        if not self.image_versions2:
-            return None
-        best: Optional[ImageVersion] = None
-        for version in self.image_versions2.candidates:
-            if version.width == self.original_width and version.height == self.original_height:
-                return version
-            elif not best or (version.width * version.height > best.width * best.height):
-                best = version
-        return best
-
-    @property
     def best_video(self) -> Optional[VideoVersion]:
         if not self.video_versions:
             return None
         best: Optional[VideoVersion] = None
         for version in self.video_versions:
             if version.width == self.original_width and version.height == self.original_height:
                 return version
@@ -495,27 +503,61 @@
     # TODO enum?
     media_share_type: str  # tag
     tagged_user_id: int
     media: MediaShareItem
 
 
 @dataclass
+class PreviewURLInfo(SerializableAttrs):
+    url: str
+    width: int
+    height: int
+
+
+@dataclass
 class XMAMediaShareItem(SerializableAttrs):
     xma_layout_type: int
 
-    target_url: str
+    title_text: Optional[str] = None
 
-    title_text: str
-    header_title_text: str
-    subtitle_text: Optional[str]
+    target_url: Optional[str] = None
+
+    header_title_text: Optional[str] = None
+    subtitle_text: Optional[str] = None
+    caption_body_text: Optional[str] = None
+
+    preview_url: Optional[str] = None
+    preview_url_mime_type: Optional[str] = None
+    preview_url_info: Optional[PreviewURLInfo] = None
+    preview_width: Optional[int] = None
+    preview_height: Optional[int] = None
+
+    # For avatar_stickers
+    is_sharable: Optional[bool] = None
+    is_borderless: Optional[bool] = None
+    should_respect_server_preview_size: Optional[bool] = None
 
-    preview_url: str
-    preview_url_mime_type: str
-    preview_width: int
-    preview_height: int
+    @property
+    def reel_share_clip_id(self) -> Optional[int]:
+        if "instagram.com/reel/" not in self.target_url:
+            return None
+        try:
+            real_id, extra_id = URL(self.target_url).query["id"].split("_")
+            return int(real_id)
+        except (ValueError, KeyError):
+            return None
+
+
+@dataclass
+class XMAMediaProfileShareItem(SerializableAttrs):
+    xma_layout_type: int
+
+    header_title_text: str
+    header_subtitle_text: Optional[str]
+    target_url: str
 
 
 @dataclass
 class ClipItem(SerializableAttrs):
     # TODO there are some additional fields in clips
     clip: MediaShareItem
 
@@ -527,27 +569,69 @@
 
 
 @dataclass
 class ProfileItem(BaseResponseUser, SerializableAttrs):
     pass
 
 
+@dataclass
+class VideoCallEvent(SerializableAttrs):
+    action: str
+    description: str
+
+
+@dataclass
+class PlaceholderItem(SerializableAttrs):
+    title: Optional[str] = None
+    message: Optional[str] = None
+    reason: Optional[int] = None
+    # is_linked: bool
+
+
+@dataclass
+class FetchedClipInfo(SerializableAttrs):
+    media: MediaShareItem
+    status: str
+
+
+@dataclass
+class TextEntities(SerializableAttrs):
+    mentioned_user_ids: List[int] = attr.ib(factory=lambda: [])
+
+
+@dataclass
+class MentionedEntity(SerializableAttrs):
+    fbid: str
+    offset: int
+    length: int
+    interop_user_type: int
+
+
+@dataclass(kw_only=True)
+class ThreadImage(ImageVersionsContainer, SerializableAttrs):
+    id: int
+    media_type: int
+
+
 @dataclass(kw_only=True)
 class ThreadItem(SerializableAttrs):
     item_id: Optional[str] = None
     user_id: Optional[int] = None
     timestamp: int = 0
     item_type: Optional[ThreadItemType] = None
     is_shh_mode: bool = False
     new_reaction: Optional[Reaction] = None
 
     text: Optional[str] = None
+    text_entities: Optional[TextEntities] = None
+    mentioned_entities: List[MentionedEntity] = None
     client_context: Optional[str] = None
     show_forward_attribution: Optional[bool] = None
     action_log: Optional[ThreadItemActionLog] = None
+    thread_image: Optional[ThreadImage] = None
     auxiliary_text: Optional[str] = None
     auxiliary_text_source_type: Optional[int] = None
     message_item_type: Optional[str] = None
 
     replied_to_message: Optional["ThreadItem"] = None
 
     media: Optional[RegularMediaItem] = None
@@ -557,23 +641,28 @@
     media_share: Optional[MediaShareItem] = None
     direct_media_share: Optional[DirectMediaShareItem] = None
     generic_xma: Optional[List[XMAMediaShareItem]] = None
     xma_media_share: Optional[List[XMAMediaShareItem]] = None
     xma_story_share: Optional[List[XMAMediaShareItem]] = None
     xma_reel_share: Optional[List[XMAMediaShareItem]] = None
     xma_reel_mention: Optional[List[XMAMediaShareItem]] = None
+    xma_clip: Optional[List[XMAMediaShareItem]] = None
+    xma_profile: Optional[List[XMAMediaProfileShareItem]] = None
+    avatar_sticker: Optional[List[XMAMediaShareItem]] = None
     reel_share: Optional[ReelShareItem] = None
     story_share: Optional[StoryShareItem] = None
     location: Optional[Location] = None
     reactions: Optional[Reactions] = None
     like: Optional[str] = None
     link: Optional[LinkItem] = None
     clip: Optional[ClipItem] = None
     felix_share: Optional[FelixShareItem] = None
     profile: Optional[ProfileItem] = None
+    placeholder: Optional[PlaceholderItem] = None
+    video_call_event: Optional[VideoCallEvent] = None
 
     @property
     def timestamp_ms(self) -> int:
         return self.timestamp // 1000
 
     @classmethod
     def deserialize(cls, data: JSON, catch_errors: bool = True) -> Union["ThreadItem", Obj]:
```

### Comparing `mautrix-instagram-0.2.3/mauigpapi/types/upload.py` & `mautrix-instagram-0.3.0/mauigpapi/types/upload.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mauigpapi/types/user.py` & `mautrix-instagram-0.3.0/mauigpapi/types/user.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/__main__.py` & `mautrix-instagram-0.3.0/mautrix_instagram/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from .version import linkified_version, version
 from .web import ProvisioningAPI
 
 
 class InstagramBridge(Bridge):
     name = "mautrix-instagram"
     module = "mautrix_instagram"
+    beeper_service_name = "instagram"
+    beeper_network_name = "instagram"
     command = "python -m mautrix-instagram"
     description = "A Matrix-Instagram DM puppeting bridge."
     repo_url = "https://github.com/mautrix/instagram"
     version = version
     markdown_version = linkified_version
     config_class = Config
     matrix_class = MatrixHandler
@@ -62,14 +64,15 @@
     def prepare_bridge(self) -> None:
         super().prepare_bridge()
         cfg = self.config["bridge.provisioning"]
         self.provisioning_api = ProvisioningAPI(
             shared_secret=cfg["shared_secret"],
             device_seed=self.config["instagram.device_seed"],
             segment_key=cfg["segment_key"],
+            segment_user_id=cfg["segment_user_id"],
         )
         self.az.app.add_subapp(cfg["prefix"], self.provisioning_api.app)
 
     async def start(self) -> None:
         self.add_startup_actions(User.init_cls(self))
         self.add_startup_actions(Puppet.init_cls(self))
         Portal.init_cls(self)
@@ -120,15 +123,15 @@
             log.info("Executing periodic reconnections")
             for user in User.by_igpk.values():
                 if not user.client or (not user.is_connected and not always_reconnect):
                     log.debug("Not reconnecting %s: not connected", user.mxid)
                     continue
                 log.debug("Executing periodic reconnect for %s", user.mxid)
                 try:
-                    await user.refresh(resync=resync)
+                    await user.refresh(resync=resync, update_proxy=True)
                 except asyncio.CancelledError:
                     log.debug("Periodic reconnect loop stopped")
                     return
                 except Exception:
                     log.exception("Error while reconnecting %s", user.mxid)
 
     async def get_portal(self, room_id: RoomID) -> Portal:
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/commands/auth.py` & `mautrix-instagram-0.3.0/mautrix_instagram/commands/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mautrix-instagram - A Matrix-Instagram puppeting bridge.
-# Copyright (C) 2022 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -11,29 +11,33 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
+import base64
 import hashlib
 import hmac
+import zlib
 
 from mauigpapi.errors import (
     IGBad2FACodeError,
     IGChallengeError,
     IGChallengeWrongCodeError,
     IGLoginBadPasswordError,
+    IGLoginInvalidCredentialsError,
     IGLoginInvalidUserError,
     IGLoginTwoFactorRequiredError,
 )
 from mauigpapi.http import AndroidAPI
 from mauigpapi.state import AndroidState
 from mauigpapi.types import BaseResponseUser
 from mautrix.bridge.commands import HelpSection, command_handler
+from mautrix.types import EventID
 
 from .. import user as u
 from .typehint import CommandEvent
 
 SECTION_AUTH = HelpSection("Authentication", 10, "")
 
 
@@ -41,29 +45,35 @@
     if user.command_status and user.command_status["action"] == "Login":
         api: AndroidAPI = user.command_status["api"]
         state: AndroidState = user.command_status["state"]
     else:
         state = AndroidState()
         seed = hmac.new(seed.encode("utf-8"), user.mxid.encode("utf-8"), hashlib.sha256).digest()
         state.device.generate(seed)
-        api = AndroidAPI(state, log=user.api_log, proxy_handler=user.proxy_handler)
-        await api.qe_sync_login_experiments()
+        api = AndroidAPI(
+            state,
+            log=user.api_log,
+            proxy_handler=user.proxy_handler,
+            on_proxy_update=user.on_proxy_update,
+            on_response_error=user.on_response_error,
+        )
+        await api.get_mobile_config()
         user.command_status = {
             "action": "Login",
             "state": state,
             "api": api,
         }
     return api, state
 
 
 @command_handler(
     needs_auth=False,
     management_only=True,
     help_section=SECTION_AUTH,
-    help_text="Log in to Instagram",
+    help_text="Log into Instagram",
     help_args="<_username_> <_password_>",
 )
 async def login(evt: CommandEvent) -> None:
     if await evt.sender.is_logged_in():
         await evt.reply("You're already logged in")
         return
     elif len(evt.args) < 2:
@@ -116,14 +126,16 @@
             "Username and password accepted, but Instagram wants to verify it's really"
             " you. Please confirm the login and enter the security code here."
         )
     except IGLoginInvalidUserError:
         await evt.reply("Invalid username")
     except IGLoginBadPasswordError:
         await evt.reply("Incorrect password")
+    except IGLoginInvalidCredentialsError:
+        await evt.reply("Incorrect username or password")
     except Exception as e:
         evt.log.exception("Failed to log in")
         await evt.reply(f"Failed to log in: {e}")
     else:
         await _post_login(evt, state, resp.logged_in_user)
 
 
@@ -217,7 +229,31 @@
     needs_auth=True,
     help_section=SECTION_AUTH,
     help_text="Disconnect the bridge from your Instagram account",
 )
 async def logout(evt: CommandEvent) -> None:
     await evt.sender.logout()
     await evt.reply("Successfully logged out")
+
+
+@command_handler(
+    needs_auth=False,
+    management_only=True,
+    help_section=SECTION_AUTH,
+    help_text="Log into Instagram with a pre-generated session blob",
+    help_args="<_blob_>",
+)
+async def login_blob(evt: CommandEvent) -> EventID:
+    if await evt.sender.is_logged_in():
+        return await evt.reply("You're already logged in")
+    elif len(evt.args) < 1:
+        return await evt.reply("**Usage:** `$cmdprefix+sp login-blob <blob>`")
+    await evt.redact()
+    try:
+        state = AndroidState.parse_json(zlib.decompress(base64.b64decode("".join(evt.args))))
+    except Exception:
+        evt.log.exception(f"{evt.sender} provided an invalid login blob")
+        return await evt.reply("Invalid blob")
+    evt.sender.state = state
+    await evt.reply("Connecting...")
+    await evt.sender.try_connect()
+    await evt.reply("Maybe connected now, try pinging?")
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/commands/conn.py` & `mautrix-instagram-0.3.0/mautrix_instagram/commands/conn.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/commands/misc.py` & `mautrix-instagram-0.3.0/mautrix_instagram/commands/misc.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/config.py` & `mautrix-instagram-0.3.0/mautrix_instagram/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mautrix-instagram - A Matrix-Instagram puppeting bridge.
-# Copyright (C) 2022 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -49,51 +49,73 @@
         copy("bridge.username_template")
         copy("bridge.displayname_template")
         copy("bridge.private_chat_name_template")
         copy("bridge.group_chat_name_template")
 
         copy("bridge.displayname_max_length")
 
-        copy("bridge.portal_create_max_age")
-        copy("bridge.chat_sync_limit")
-        copy("bridge.chat_create_limit")
-        copy("bridge.resync_on_startup")
+        copy("bridge.max_startup_thread_sync_count")
         copy("bridge.sync_with_custom_puppets")
         copy("bridge.sync_direct_chat_list")
         copy("bridge.double_puppet_server_map")
         copy("bridge.double_puppet_allow_discovery")
         copy("bridge.login_shared_secret_map")
         copy("bridge.federate_rooms")
-        copy("bridge.backfill.invite_own_puppet")
-        copy("bridge.backfill.initial_limit")
-        copy("bridge.backfill.missed_limit")
-        copy("bridge.backfill.disable_notifications")
+        copy("bridge.backfill.enable_initial")
+        copy("bridge.backfill.enable")
+        copy("bridge.backfill.msc2716")
+        copy("bridge.backfill.double_puppet_backfill")
+        if "bridge.initial_chat_sync" in self:
+            initial_chat_sync = self["bridge.initial_chat_sync"]
+            base["bridge.backfill.max_conversations"] = self.get(
+                "bridge.backfill.max_conversations", initial_chat_sync
+            )
+        else:
+            copy("bridge.backfill.max_conversations")
+        copy("bridge.backfill.min_sync_thread_delay")
+        copy("bridge.backfill.unread_hours_threshold")
+        copy("bridge.backfill.backoff.thread_list")
+        copy("bridge.backfill.backoff.message_history")
+        copy("bridge.backfill.incremental.max_pages")
+        copy("bridge.backfill.incremental.max_total_pages")
+        copy("bridge.backfill.incremental.page_delay")
+        copy("bridge.backfill.incremental.post_batch_delay")
         copy("bridge.periodic_reconnect.interval")
         copy("bridge.periodic_reconnect.resync")
         copy("bridge.periodic_reconnect.always")
-        copy("bridge.private_chat_portal_meta")
+        if isinstance(self.get("bridge.private_chat_portal_meta", "default"), bool):
+            base["bridge.private_chat_portal_meta"] = (
+                "always" if self["bridge.private_chat_portal_meta"] else "default"
+            )
+        else:
+            copy("bridge.private_chat_portal_meta")
+            if base["bridge.private_chat_portal_meta"] not in ("default", "always", "never"):
+                base["bridge.private_chat_portal_meta"] = "default"
         copy("bridge.delivery_receipts")
         copy("bridge.delivery_error_reports")
         copy("bridge.message_status_events")
         copy("bridge.resend_bridge_info")
         copy("bridge.unimportant_bridge_notices")
         copy("bridge.disable_bridge_notices")
         copy("bridge.caption_in_message")
         copy("bridge.bridge_notices")
+        copy("bridge.bridge_matrix_typing")
 
         copy("bridge.provisioning.enabled")
         copy("bridge.provisioning.prefix")
         copy("bridge.provisioning.shared_secret")
         if base["bridge.provisioning.shared_secret"] == "generate":
             base["bridge.provisioning.shared_secret"] = self._new_token()
         copy("bridge.provisioning.segment_key")
+        copy("bridge.provisioning.segment_user_id")
 
         copy("bridge.command_prefix")
 
         copy("bridge.get_proxy_api_url")
+        copy("bridge.use_proxy_for_media")
 
         copy_dict("bridge.permissions")
 
     def _get_permissions(self, key: str) -> Permissions:
         level = self["bridge.permissions"].get(key, "")
         admin = level == "admin"
         user = level == "user" or admin
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/db/message.py` & `mautrix-instagram-0.3.0/mautrix_instagram/db/message.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, ClassVar
 
 from attr import dataclass
+import attr
 
 from mautrix.types import EventID, RoomID
-from mautrix.util.async_db import Database
+from mautrix.util.async_db import Database, Scheme
 
 fake_db = Database.create("") if TYPE_CHECKING else None
 
 
 @dataclass
 class Message:
     db: ClassVar[Database] = fake_db
@@ -33,45 +34,51 @@
     mx_room: RoomID
     item_id: str
     client_context: str | None
     receiver: int
     sender: int
     ig_timestamp: int | None
 
+    _columns = "mxid, mx_room, item_id, client_context, receiver, sender, ig_timestamp"
+    _insert_query = f"INSERT INTO message ({_columns}) VALUES ($1, $2, $3, $4, $5, $6, $7)"
+
     @property
     def ig_timestamp_ms(self) -> int:
         return (self.ig_timestamp // 1000) if self.ig_timestamp else 0
 
     async def insert(self) -> None:
-        q = """
-            INSERT INTO message (mxid, mx_room, item_id, client_context, receiver, sender,
-                                 ig_timestamp)
-            VALUES ($1, $2, $3, $4, $5, $6, $7)
-        """
         await self.db.execute(
-            q,
+            self._insert_query,
             self.mxid,
             self.mx_room,
             self.item_id,
             self.client_context,
             self.receiver,
             self.sender,
             self.ig_timestamp,
         )
 
+    @classmethod
+    async def bulk_insert(cls, messages: list[Message]) -> None:
+        columns = cls._columns.split(", ")
+        records = [attr.astuple(message) for message in messages]
+        async with cls.db.acquire() as conn, conn.transaction():
+            if cls.db.scheme == Scheme.POSTGRES:
+                await conn.copy_records_to_table("message", records=records, columns=columns)
+            else:
+                await conn.executemany(cls._insert_query, records)
+
     async def delete(self) -> None:
         q = "DELETE FROM message WHERE item_id=$1 AND receiver=$2"
         await self.db.execute(q, self.item_id, self.receiver)
 
     @classmethod
     async def delete_all(cls, room_id: RoomID) -> None:
         await cls.db.execute("DELETE FROM message WHERE mx_room=$1", room_id)
 
-    _columns = "mxid, mx_room, item_id, client_context, receiver, sender, ig_timestamp"
-
     @classmethod
     async def get_by_mxid(cls, mxid: EventID, mx_room: RoomID) -> Message | None:
         q = f"SELECT {cls._columns} FROM message WHERE mxid=$1 AND mx_room=$2"
         row = await cls.db.fetchrow(q, mxid, mx_room)
         if not row:
             return None
         return cls(**row)
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/db/portal.py` & `mautrix-instagram-0.3.0/mautrix_instagram/db/portal.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, ClassVar
 
+from asyncpg import Record
 from attr import dataclass
-import asyncpg
 
-from mautrix.types import ContentURI, RoomID, UserID
+from mautrix.types import BatchID, ContentURI, EventID, RoomID, UserID
 from mautrix.util.async_db import Database
 
 fake_db = Database.create("") if TYPE_CHECKING else None
 
 
 @dataclass
 class Portal:
@@ -36,109 +36,132 @@
     mxid: RoomID | None
     name: str | None
     avatar_url: ContentURI | None
     encrypted: bool
     name_set: bool
     avatar_set: bool
     relay_user_id: UserID | None
+    first_event_id: EventID | None
+    next_batch_id: BatchID | None
+    historical_base_insertion_event_id: EventID | None
+    cursor: str | None
+    thread_image_id: int | None
 
     @property
     def _values(self):
         return (
             self.thread_id,
             self.receiver,
             self.other_user_pk,
             self.mxid,
             self.name,
             self.avatar_url,
             self.encrypted,
             self.name_set,
             self.avatar_set,
             self.relay_user_id,
+            self.first_event_id,
+            self.next_batch_id,
+            self.historical_base_insertion_event_id,
+            self.cursor,
+            self.thread_image_id,
+        )
+
+    column_names = ",".join(
+        (
+            "thread_id",
+            "receiver",
+            "other_user_pk",
+            "mxid",
+            "name",
+            "avatar_url",
+            "encrypted",
+            "name_set",
+            "avatar_set",
+            "relay_user_id",
+            "first_event_id",
+            "next_batch_id",
+            "historical_base_insertion_event_id",
+            "cursor",
+            "thread_image_id",
         )
+    )
 
     async def insert(self) -> None:
         q = (
-            "INSERT INTO portal (thread_id, receiver, other_user_pk, mxid, name, avatar_url, "
-            "                    encrypted, name_set, avatar_set, relay_user_id) "
-            "VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9, $10)"
+            f"INSERT INTO portal ({self.column_names}) "
+            "VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9, $10, $11, $12, $13, $14, $15)"
         )
         await self.db.execute(q, *self._values)
 
     async def update(self) -> None:
         q = (
             "UPDATE portal SET other_user_pk=$3, mxid=$4, name=$5, avatar_url=$6, encrypted=$7,"
-            "                  name_set=$8, avatar_set=$9, relay_user_id=$10 "
+            "                  name_set=$8, avatar_set=$9, relay_user_id=$10, first_event_id=$11,"
+            "                  next_batch_id=$12, historical_base_insertion_event_id=$13,"
+            "                  cursor=$14, thread_image_id=$15 "
             "WHERE thread_id=$1 AND receiver=$2"
         )
         await self.db.execute(q, *self._values)
 
     @classmethod
-    def _from_row(cls, row: asyncpg.Record) -> Portal:
+    def _from_row(cls, row: Record | None) -> Portal | None:
+        if row is None:
+            return None
         return cls(**row)
 
     @classmethod
     async def get_by_mxid(cls, mxid: RoomID) -> Portal | None:
-        q = (
-            "SELECT thread_id, receiver, other_user_pk, mxid, name, avatar_url, encrypted, "
-            "       name_set, avatar_set, relay_user_id "
-            "FROM portal WHERE mxid=$1"
-        )
+        q = f"SELECT {cls.column_names} FROM portal WHERE mxid=$1"
         row = await cls.db.fetchrow(q, mxid)
-        if not row:
-            return None
         return cls._from_row(row)
 
     @classmethod
     async def get_by_thread_id(
         cls, thread_id: str, receiver: int, rec_must_match: bool = True
     ) -> Portal | None:
-        q = (
-            "SELECT thread_id, receiver, other_user_pk, mxid, name, avatar_url, encrypted, "
-            "       name_set, avatar_set, relay_user_id "
-            "FROM portal WHERE thread_id=$1 AND receiver=$2"
-        )
+        q = f"SELECT {cls.column_names} FROM portal WHERE thread_id=$1 AND receiver=$2"
         if not rec_must_match:
-            q = (
-                "SELECT thread_id, receiver, other_user_pk, mxid, name, avatar_url, encrypted, "
-                "       name_set, avatar_set "
-                "FROM portal WHERE thread_id=$1 AND (receiver=$2 OR receiver=0)"
-            )
+            q = f"""
+                SELECT {cls.column_names}
+                FROM portal
+                WHERE thread_id=$1
+                    AND (receiver=$2 OR receiver=0)
+            """
         row = await cls.db.fetchrow(q, thread_id, receiver)
-        if not row:
-            return None
         return cls._from_row(row)
 
     @classmethod
     async def find_private_chats_of(cls, receiver: int) -> list[Portal]:
-        q = (
-            "SELECT thread_id, receiver, other_user_pk, mxid, name, avatar_url, encrypted, "
-            "       name_set, avatar_set, relay_user_id "
-            "FROM portal WHERE receiver=$1 AND other_user_pk IS NOT NULL"
-        )
+        q = f"""
+            SELECT {cls.column_names}
+            FROM portal
+            WHERE receiver=$1
+                AND other_user_pk IS NOT NULL
+        """
         rows = await cls.db.fetch(q, receiver)
         return [cls._from_row(row) for row in rows]
 
     @classmethod
     async def find_private_chats_with(cls, other_user: int) -> list[Portal]:
-        q = (
-            "SELECT thread_id, receiver, other_user_pk, mxid, name, avatar_url, encrypted, "
-            "       name_set, avatar_set, relay_user_id "
-            "FROM portal WHERE other_user_pk=$1"
-        )
+        q = f"""
+            SELECT {cls.column_names}
+            FROM portal
+            WHERE other_user_pk=$1
+        """
         rows = await cls.db.fetch(q, other_user)
         return [cls._from_row(row) for row in rows]
 
     @classmethod
     async def find_private_chat_id(cls, receiver: int, other_user: int) -> str | None:
         q = "SELECT thread_id FROM portal WHERE receiver=$1 AND other_user_pk=$2"
         return await cls.db.fetchval(q, receiver, other_user)
 
     @classmethod
     async def all_with_room(cls) -> list[Portal]:
-        q = (
-            "SELECT thread_id, receiver, other_user_pk, mxid, name, avatar_url, encrypted, "
-            "       name_set, avatar_set, relay_user_id "
-            "FROM portal WHERE mxid IS NOT NULL"
-        )
+        q = f"""
+            SELECT {cls.column_names}
+            FROM portal
+            WHERE mxid IS NOT NULL
+        """
         rows = await cls.db.fetch(q)
         return [cls._from_row(row) for row in rows]
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/db/puppet.py` & `mautrix-instagram-0.3.0/mautrix_instagram/db/puppet.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     pk: int
     name: str | None
     username: str | None
     photo_id: str | None
     photo_mxc: ContentURI | None
     name_set: bool
     avatar_set: bool
+    contact_info_set: bool
 
     is_registered: bool
 
     custom_mxid: UserID | None
     access_token: str | None
     next_batch: SyncToken | None
     base_url: URL | None
@@ -52,71 +53,71 @@
             self.pk,
             self.name,
             self.username,
             self.photo_id,
             self.photo_mxc,
             self.name_set,
             self.avatar_set,
+            self.contact_info_set,
             self.is_registered,
             self.custom_mxid,
             self.access_token,
             self.next_batch,
             str(self.base_url) if self.base_url else None,
         )
 
+    columns: ClassVar[str] = (
+        "pk, name, username, photo_id, photo_mxc, name_set, avatar_set, contact_info_set, "
+        "is_registered, custom_mxid, access_token, next_batch, base_url"
+    )
+
     async def insert(self) -> None:
-        q = (
-            "INSERT INTO puppet (pk, name, username, photo_id, photo_mxc, name_set, avatar_set,"
-            "                    is_registered, custom_mxid, access_token, next_batch, base_url) "
-            "VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9, $10, $11, $12)"
-        )
+        q = f"""
+            INSERT INTO puppet ({self.columns})
+            VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9, $10, $11, $12, $13)
+        """
         await self.db.execute(q, *self._values)
 
     async def update(self) -> None:
-        q = (
-            "UPDATE puppet SET name=$2, username=$3, photo_id=$4, photo_mxc=$5, name_set=$6,"
-            "                  avatar_set=$7, is_registered=$8, custom_mxid=$9, access_token=$10,"
-            "                  next_batch=$11, base_url=$12 "
-            "WHERE pk=$1"
-        )
+        q = """
+            UPDATE puppet
+            SET name=$2, username=$3, photo_id=$4, photo_mxc=$5, name_set=$6, avatar_set=$7,
+                contact_info_set=$8, is_registered=$9, custom_mxid=$10, access_token=$11,
+                next_batch=$12, base_url=$13
+            WHERE pk=$1
+        """
         await self.db.execute(q, *self._values)
 
     @classmethod
     def _from_row(cls, row: asyncpg.Record) -> Puppet:
         data = {**row}
         base_url_str = data.pop("base_url")
         base_url = URL(base_url_str) if base_url_str is not None else None
         return cls(base_url=base_url, **data)
 
     @classmethod
     async def get_by_pk(cls, pk: int) -> Puppet | None:
-        q = (
-            "SELECT pk, name, username, photo_id, photo_mxc, name_set, avatar_set, is_registered,"
-            "       custom_mxid, access_token, next_batch, base_url "
-            "FROM puppet WHERE pk=$1"
-        )
+        q = f"SELECT {cls.columns} FROM puppet WHERE pk=$1"
         row = await cls.db.fetchrow(q, pk)
         if not row:
             return None
         return cls._from_row(row)
 
     @classmethod
     async def get_by_custom_mxid(cls, mxid: UserID) -> Puppet | None:
-        q = (
-            "SELECT pk, name, username, photo_id, photo_mxc, name_set, avatar_set, is_registered,"
-            "       custom_mxid, access_token, next_batch, base_url "
-            "FROM puppet WHERE custom_mxid=$1"
-        )
+        q = f"SELECT {cls.columns} FROM puppet WHERE custom_mxid=$1"
         row = await cls.db.fetchrow(q, mxid)
         if not row:
             return None
         return cls._from_row(row)
 
     @classmethod
     async def all_with_custom_mxid(cls) -> list[Puppet]:
-        q = (
-            "SELECT pk, name, username, photo_id, photo_mxc, name_set, avatar_set, is_registered,"
-            "       custom_mxid, access_token, next_batch, base_url "
-            "FROM puppet WHERE custom_mxid IS NOT NULL"
-        )
+        q = f"SELECT {cls.columns} FROM puppet WHERE custom_mxid IS NOT NULL"
+        rows = await cls.db.fetch(q)
+        return [cls._from_row(row) for row in rows]
+
+    @classmethod
+    async def get_all(cls) -> list[Puppet]:
+        q = f"SELECT {cls.columns} FROM puppet"
         rows = await cls.db.fetch(q)
         return [cls._from_row(row) for row in rows]
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/db/reaction.py` & `mautrix-instagram-0.3.0/mautrix_instagram/db/reaction.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/db/upgrade.py` & `mautrix-instagram-0.3.0/mautrix_instagram/db/upgrade/v00_latest_revision.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 # mautrix-instagram - A Matrix-Instagram puppeting bridge.
-# Copyright (C) 2020 Tulir Asokan
+# Copyright (C) 2022 Tulir Asokan, Sumner Evans
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
-from asyncpg import Connection
+from mautrix.util.async_db import Connection, Scheme
 
-from mautrix.util.async_db import UpgradeTable
+from . import upgrade_table
 
-upgrade_table = UpgradeTable()
 
-
-@upgrade_table.register(description="Latest revision", upgrades_to=8)
-async def upgrade_latest(conn: Connection) -> None:
+@upgrade_table.register(description="Latest revision", upgrades_to=13)
+async def upgrade_latest(conn: Connection, scheme: Scheme) -> None:
     await conn.execute(
         """CREATE TABLE portal (
-            thread_id     TEXT,
-            receiver      BIGINT,
-            other_user_pk BIGINT,
-            mxid          TEXT,
-            name          TEXT,
-            avatar_url    TEXT,
-            name_set      BOOLEAN NOT NULL DEFAULT false,
-            avatar_set    BOOLEAN NOT NULL DEFAULT false,
-            encrypted     BOOLEAN NOT NULL DEFAULT false,
-            relay_user_id TEXT,
+            thread_id                           TEXT,
+            receiver                            BIGINT,
+            other_user_pk                       BIGINT,
+            mxid                                TEXT,
+            name                                TEXT,
+            avatar_url                          TEXT,
+            name_set                            BOOLEAN NOT NULL DEFAULT false,
+            avatar_set                          BOOLEAN NOT NULL DEFAULT false,
+            encrypted                           BOOLEAN NOT NULL DEFAULT false,
+            relay_user_id                       TEXT,
+            first_event_id                      TEXT,
+            next_batch_id                       TEXT,
+            historical_base_insertion_event_id  TEXT,
+            cursor                              TEXT,
+            thread_image_id                     BIGINT,
             PRIMARY KEY (thread_id, receiver)
         )"""
     )
     await conn.execute(
         """CREATE TABLE "user" (
-            mxid           TEXT PRIMARY KEY,
-            igpk           BIGINT,
-            state          jsonb,
-            seq_id         BIGINT,
-            snapshot_at_ms BIGINT,
-            notice_room    TEXT
+            mxid                        TEXT PRIMARY KEY,
+            igpk                        BIGINT,
+            state                       jsonb,
+            seq_id                      BIGINT,
+            snapshot_at_ms              BIGINT,
+            notice_room                 TEXT,
+            oldest_cursor               TEXT,
+            total_backfilled_portals    INTEGER,
+            thread_sync_completed       BOOLEAN NOT NULL DEFAULT false
         )"""
     )
     await conn.execute(
         """CREATE TABLE puppet (
             pk            BIGINT PRIMARY KEY,
             name          TEXT,
             username      TEXT,
@@ -99,45 +105,32 @@
             PRIMARY KEY (ig_item_id, ig_receiver, ig_sender),
             FOREIGN KEY (ig_item_id, ig_receiver) REFERENCES message(item_id, receiver)
                 ON DELETE CASCADE ON UPDATE CASCADE,
             UNIQUE (mxid, mx_room)
         )"""
     )
 
-
-@upgrade_table.register(description="Add name_set and avatar_set to portal table")
-async def upgrade_v2(conn: Connection) -> None:
-    await conn.execute("ALTER TABLE portal ADD COLUMN avatar_url TEXT")
-    await conn.execute("ALTER TABLE portal ADD COLUMN name_set BOOLEAN NOT NULL DEFAULT false")
-    await conn.execute("ALTER TABLE portal ADD COLUMN avatar_set BOOLEAN NOT NULL DEFAULT false")
-    await conn.execute("UPDATE portal SET name_set=true WHERE name<>''")
-
-
-@upgrade_table.register(description="Add relay user field to portal table")
-async def upgrade_v3(conn: Connection) -> None:
-    await conn.execute("ALTER TABLE portal ADD COLUMN relay_user_id TEXT")
-
-
-@upgrade_table.register(description="Add client context field to message table")
-async def upgrade_v4(conn: Connection) -> None:
-    await conn.execute("ALTER TABLE message ADD COLUMN client_context TEXT")
-
-
-@upgrade_table.register(description="Add ig_timestamp field to message table")
-async def upgrade_v5(conn: Connection) -> None:
-    await conn.execute("ALTER TABLE message ADD COLUMN ig_timestamp BIGINT")
-
-
-@upgrade_table.register(description="Allow hidden events in message table")
-async def upgrade_v6(conn: Connection) -> None:
-    await conn.execute("ALTER TABLE message ALTER COLUMN mxid DROP NOT NULL")
-
-
-@upgrade_table.register(description="Store reaction timestamps")
-async def upgrade_v7(conn: Connection) -> None:
-    await conn.execute("ALTER TABLE reaction ADD COLUMN mx_timestamp BIGINT")
-
-
-@upgrade_table.register(description="Store sync sequence ID in user table")
-async def upgrade_v8(conn: Connection) -> None:
-    await conn.execute('ALTER TABLE "user" ADD COLUMN seq_id BIGINT')
-    await conn.execute('ALTER TABLE "user" ADD COLUMN snapshot_at_ms BIGINT')
+    gen = ""
+    if scheme in (Scheme.POSTGRES, Scheme.COCKROACH):
+        gen = "GENERATED ALWAYS AS IDENTITY"
+    await conn.execute(
+        f"""
+        CREATE TABLE backfill_queue (
+            queue_id            INTEGER PRIMARY KEY {gen},
+            user_mxid           TEXT,
+            priority            INTEGER NOT NULL,
+            portal_thread_id    TEXT,
+            portal_receiver     BIGINT,
+            num_pages           INTEGER NOT NULL,
+            page_delay          INTEGER NOT NULL,
+            post_batch_delay    INTEGER NOT NULL,
+            max_total_pages     INTEGER NOT NULL,
+            dispatch_time       TIMESTAMP,
+            completed_at        TIMESTAMP,
+            cooldown_timeout    TIMESTAMP,
+
+            FOREIGN KEY (user_mxid) REFERENCES "user"(mxid) ON DELETE CASCADE ON UPDATE CASCADE,
+            FOREIGN KEY (portal_thread_id, portal_receiver)
+                REFERENCES portal(thread_id, receiver) ON DELETE CASCADE
+        )
+        """
+    )
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/db/user.py` & `mautrix-instagram-0.3.0/mautrix_instagram/db/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,52 +33,72 @@
 
     mxid: UserID
     igpk: int | None
     state: AndroidState | None
     notice_room: RoomID | None
     seq_id: int | None
     snapshot_at_ms: int | None
+    oldest_cursor: str | None
+    total_backfilled_portals: int | None
+    thread_sync_completed: bool
 
     @property
     def _values(self):
         return (
             self.mxid,
             self.igpk,
             self.state.json() if self.state else None,
             self.notice_room,
             self.seq_id,
             self.snapshot_at_ms,
+            self.oldest_cursor,
+            self.total_backfilled_portals,
+            self.thread_sync_completed,
         )
 
+    _columns = ",".join(
+        (
+            "mxid",
+            "igpk",
+            "state",
+            "notice_room",
+            "seq_id",
+            "snapshot_at_ms",
+            "oldest_cursor",
+            "total_backfilled_portals",
+            "thread_sync_completed",
+        )
+    )
+
     async def insert(self) -> None:
-        q = """
-        INSERT INTO "user" (mxid, igpk, state, notice_room, seq_id, snapshot_at_ms)
-        VALUES ($1, $2, $3, $4, $5, $6)
+        q = f"""
+        INSERT INTO "user" ({self._columns})
+        VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9)
         """
         await self.db.execute(q, *self._values)
 
     async def update(self) -> None:
         q = """
-        UPDATE "user" SET igpk=$2, state=$3, notice_room=$4, seq_id=$5, snapshot_at_ms=$6
+        UPDATE "user"
+        SET igpk=$2, state=$3, notice_room=$4, seq_id=$5, snapshot_at_ms=$6,
+            oldest_cursor=$7, total_backfilled_portals=$8, thread_sync_completed=$9
         WHERE mxid=$1
         """
         await self.db.execute(q, *self._values)
 
     async def save_seq_id(self) -> None:
         q = 'UPDATE "user" SET seq_id=$2, snapshot_at_ms=$3 WHERE mxid=$1'
         await self.db.execute(q, self.mxid, self.seq_id, self.snapshot_at_ms)
 
     @classmethod
     def _from_row(cls, row: asyncpg.Record) -> User:
         data = {**row}
         state_str = data.pop("state")
         return cls(state=AndroidState.parse_json(state_str) if state_str else None, **data)
 
-    _columns = "mxid, igpk, state, notice_room, seq_id, snapshot_at_ms"
-
     @classmethod
     async def get_by_mxid(cls, mxid: UserID) -> User | None:
         q = f'SELECT {cls._columns} FROM "user" WHERE mxid=$1'
         row = await cls.db.fetchrow(q, mxid)
         if not row:
             return None
         return cls._from_row(row)
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/example-config.yaml` & `mautrix-instagram-0.3.0/mautrix_instagram/example-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -105,23 +105,17 @@
     private_chat_name_template: "{displayname}"
     # Displayname template for group chat portals. Only {name} is available.
     group_chat_name_template: "{name}"
 
     # Maximum length of displayname
     displayname_max_length: 100
 
-    # Maximum number of seconds since the last activity in a chat to automatically create portals.
-    portal_create_max_age: 259200
-    # Maximum number of chats to fetch for startup sync
-    chat_sync_limit: 20
-    # Maximum number of chats to create during startup sync
-    chat_create_limit: 10
-    # Should the chat list be synced on startup?
-    # If false, the bridge will try to reconnect to MQTT directly and ask the server to send missed events.
-    resync_on_startup: true
+    # The maximum number of conversations that should be synced when we get a
+    # message sync error. In general, 1 page (20) is sufficient.
+    max_startup_thread_sync_count: 20
     # Whether or not to use /sync to get read receipts and typing notifications
     # when double puppeting is enabled
     sync_with_custom_puppets: false
     # Whether or not to update the m.direct account data event when double puppeting is enabled.
     # Note that updating the m.direct event is not atomic (except with mautrix-asmux)
     # and is therefore prone to race conditions.
     sync_direct_chat_list: false
@@ -140,40 +134,90 @@
     login_shared_secret_map:
         example.com: foo
     # Whether or not created rooms should have federation enabled.
     # If false, created portal rooms will never be federated.
     federate_rooms: true
     # Settings for backfilling messages from Instagram.
     backfill:
-        # Whether or not the Instagram users of logged in Matrix users should be
-        # invited to private chats when backfilling history from Instagram. This is
-        # usually needed to prevent rate limits and to allow timestamp massaging.
-        invite_own_puppet: true
-        # Maximum number of messages to backfill initially.
-        # Set to 0 to disable backfilling when creating portal.
-        initial_limit: 0
-        # Maximum number of messages to backfill if messages were missed while
-        # the bridge was disconnected.
-        # Set to 0 to disable backfilling missed messages.
-        missed_limit: 1000
-        # If using double puppeting, should notifications be disabled
-        # while the initial backfill is in progress?
-        disable_notifications: false
+        # Enable initial backfill (~10 messages after creating portal)?
+        enable_initial: true
+        # Enable backfill queue? This is used for backfilling additional threads after the initial sync,
+        # and when MSC2716 is enabled, to backfill message history going backwards.
+        enable: false
+        # Use MSC2716 for backfilling? If this is disabled, backfilling only happens when syncing threads,
+        # and the incremental settings below don't apply.
+        #
+        # This requires a server with MSC2716 support, which is currently an experimental feature in Synapse.
+        # It can be enabled by setting experimental_features -> msc2716_enabled to true in homeserver.yaml.
+        msc2716: false
+        # Use double puppets for backfilling?
+        # In order to use this, the double puppets must be in the appservice's user ID namespace
+        # (because the bridge can't use the double puppet access token with batch sending).
+        # This only affects double puppets on the local server, double puppets on other servers will never be used.
+        double_puppet_backfill: false
+        # The maximum number of conversations that should be synced.
+        # Other conversations will be backfilled on demand when the start PM
+        # provisioning endpoint is used or when a message comes in from that
+        # chat.
+        # If set to -1, all conversations will by synced.
+        max_conversations: 20
+        # The minimum amount of time to wait between syncing each thread. This
+        # helps avoid situations where you sync too quickly.
+        min_sync_thread_delay: 5
+        # If this value is greater than 0, then if the conversation's last
+        # message was more than this number of hours ago, then the conversation
+        # will automatically be marked it as read.
+        # Conversations that have a last message that is less than this number
+        # of hours ago will have their unread status synced from Instagram.
+        unread_hours_threshold: 0
+
+        # Settings for how quickly to backoff when rate-limits are encountered
+        # while backfilling.
+        backoff:
+            # How many seconds to wait after getting rate limited during a
+            # thread list fetch.
+            thread_list: 300
+            # How many seconds to wait after getting rate limited during a
+            # message history fetch.
+            message_history: 300
+
+        # Settings for backfills.
+        #
+        # During initial/incremental sync, the entirety of the thread that is
+        # available will be backfilled. For example, on initial sync, about 20
+        # messages are included for each thread in the thread list returned by
+        # the server. After that, incremental backfills will be run for each of
+        # the portals in a round-robin fashion until all portals have been
+        # backfilled as configured below.
+        incremental:
+            # The maximum number of pages to backfill per batch.
+            max_pages: 10
+            # The maximum number of total pages to backfill per portal.
+            # If set to -1, infinite pages will be synced.
+            max_total_pages: -1
+            # The number of seconds to wait between backfilling each page.
+            page_delay: 5
+            # The number of seconds to wait after backfilling the batch of
+            # messages.
+            post_batch_delay: 20
+
     periodic_reconnect:
         # Interval in seconds in which to automatically reconnect all users.
         # This can be used to automatically mitigate the bug where Instagram stops sending messages.
         # Set to -1 to disable periodic reconnections entirely.
         interval: -1
         # Whether or not the bridge should backfill chats when reconnecting.
         resync: true
         # Should even disconnected users be reconnected?
         always: false
 
     # URL to call to retrieve a proxy URL from (defaults to the http_proxy environment variable).
     get_proxy_api_url: null
+    # Whether to use proxy for downloading media from Instagram.
+    use_proxy_for_media: true
 
     # End-to-bridge encryption support options.
     #
     # See https://docs.mau.fi/bridges/general/end-to-bridge-encryption.html for more info.
     encryption:
         # Allow encryption, work in group chat rooms with e2ee enabled
         allow: false
@@ -183,14 +227,31 @@
         # Whether to use MSC2409/MSC3202 instead of /sync long polling for receiving encryption-related data.
         appservice: false
         # Require encryption, drop any unencrypted messages.
         require: false
         # Enable key sharing? If enabled, key requests for rooms where users are in will be fulfilled.
         # You must use a client that supports requesting keys from other users to use this feature.
         allow_key_sharing: false
+        # Options for deleting megolm sessions from the bridge.
+        delete_keys:
+            # Beeper-specific: delete outbound sessions when hungryserv confirms
+            # that the user has uploaded the key to key backup.
+            delete_outbound_on_ack: false
+            # Don't store outbound sessions in the inbound table.
+            dont_store_outbound: false
+            # Ratchet megolm sessions forward after decrypting messages.
+            ratchet_on_decrypt: false
+            # Delete fully used keys (index >= max_messages) after decrypting messages.
+            delete_fully_used_on_decrypt: false
+            # Delete previous megolm sessions from same device when receiving a new one.
+            delete_prev_on_new_session: false
+            # Delete megolm sessions received from a device when the device is deleted.
+            delete_on_device_delete: false
+            # Periodically delete megolm sessions when 2x max_age has passed since receiving the session.
+            periodically_delete_expired: false
         # What level of device verification should be required from users?
         #
         # Valid levels:
         #   unverified - Send keys to all device in the room.
         #   cross-signed-untrusted - Require valid cross-signing, but trust all cross-signing keys.
         #   cross-signed-tofu - Require valid cross-signing, trust cross-signing keys on first use (and reject changes).
         #   cross-signed-verified - Require valid cross-signing, plus a valid user signature from the bridge bot.
@@ -218,17 +279,19 @@
             # as the default.
             milliseconds: 604800000
             # The maximum number of messages that should be sent with a given a
             # session before changing it. The Matrix spec recommends 100 as the
             # default.
             messages: 100
 
-    # Whether or not to explicitly set the avatar and room name for private
-    # chat portal rooms. This will be implicitly enabled if encryption.default is true.
-    private_chat_portal_meta: false
+    # Whether to explicitly set the avatar and room name for private chat portal rooms.
+    # If set to `default`, this will be enabled in encrypted rooms and disabled in unencrypted rooms.
+    # If set to `always`, all DM rooms will have explicit names and avatars set.
+    # If set to `never`, DM rooms will never have names and avatars set.
+    private_chat_portal_meta: default
     # Whether or not the bridge should send a read receipt from the bridge bot when a message has
     # been sent to Instagram.
     delivery_receipts: false
     # Whether or not delivery errors should be reported as messages in the Matrix room.
     delivery_error_reports: false
     # Whether the bridge should send the message status as a custom com.beeper.message_send_status event.
     message_status_events: false
@@ -244,26 +307,32 @@
     # Send captions in the same message as images. This will send data compatible with both MSC2530 and MSC3552.
     # This is currently not supported in most clients.
     caption_in_message: false
 
     # Should Matrix m.notice-type messages be bridged?
     bridge_notices: true
 
+    # Should Matrix typing notices be sent to Instagram? Typing notifications
+    # from Instagram will still be bridged.
+    bridge_matrix_typing: true
+
     # Provisioning API part of the web server for automated portal creation and fetching information.
     # Used by things like mautrix-manager (https://github.com/tulir/mautrix-manager).
     provisioning:
         # Whether or not the provisioning API should be enabled.
         enabled: true
         # The prefix to use in the provisioning API endpoints.
         prefix: /_matrix/provision/v1
         # The shared secret to authorize users of the API.
         # Set to "generate" to generate and save a new token.
         shared_secret: generate
         # Segment API key to enable analytics tracking for web server endpoints. Set to null to disable.
         segment_key: null
+        # Optional user_id to use when sending Segment events. If null, defaults to using mxID.
+        segment_user_id: null
 
     # The prefix for commands. Only required in non-management rooms.
     command_prefix: "!ig"
 
     # Permissions for using the bridge.
     # Permitted values:
     #      relay - Allowed to be relayed through the bridge, no access to commands.
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/get_version.py` & `mautrix-instagram-0.3.0/mautrix_instagram/get_version.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/matrix.py` & `mautrix-instagram-0.3.0/mautrix_instagram/matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
+import sys
 
 from mautrix.bridge import BaseMatrixHandler
 from mautrix.types import (
     Event,
     EventID,
     EventType,
     PresenceEvent,
@@ -47,14 +48,29 @@
         prefix, suffix = bridge.config["bridge.username_template"].format(userid=":").split(":")
         homeserver = bridge.config["homeserver.domain"]
         self.user_id_prefix = f"@{prefix}"
         self.user_id_suffix = f"{suffix}:{homeserver}"
 
         super().__init__(bridge=bridge)
 
+    async def check_versions(self) -> None:
+        await super().check_versions()
+        if self.config["bridge.backfill.msc2716"] and not (
+            support := self.versions.supports("org.matrix.msc2716")
+        ):
+            self.log.fatal(
+                "Backfilling is enabled in bridge config, but "
+                + (
+                    "MSC2716 batch sending is not enabled on homeserver"
+                    if support is False
+                    else "homeserver does not support MSC2716 batch sending"
+                )
+            )
+            sys.exit(18)
+
     async def send_welcome_message(self, room_id: RoomID, inviter: u.User) -> None:
         await super().send_welcome_message(room_id, inviter)
         if not inviter.notice_room:
             inviter.notice_room = room_id
             await inviter.update()
             await self.az.intent.send_notice(
                 room_id, "This room has been marked as your Instagram bridge notice room."
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/portal.py` & `mautrix-instagram-0.3.0/mautrix_instagram/portal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mautrix-instagram - A Matrix-Instagram puppeting bridge.
-# Copyright (C) 2022 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -11,81 +11,103 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Awaitable, Callable, Union, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    AsyncGenerator,
+    Awaitable,
+    Callable,
+    Literal,
+    Optional,
+    Union,
+    cast,
+)
 from collections import deque
 from io import BytesIO
+from urllib.parse import urlparse
 import asyncio
+import base64
+import hashlib
 import html
 import json
 import mimetypes
 import re
 import sqlite3
 import time
 
+from aiohttp import ClientResponse, ClientSession
 from yarl import URL
 import asyncpg
 import magic
 
+from mauigpapi.errors import IGRateLimitError, IGResponseError
 from mauigpapi.types import (
     AnimatedMediaItem,
     CommandResponse,
     ExpiredMediaItem,
     MediaShareItem,
     MediaType,
     MessageSyncMessage,
     Reaction,
     ReactionStatus,
     ReelMediaShareItem,
     ReelShareType,
     RegularMediaItem,
     Thread,
+    ThreadImage,
     ThreadItem,
     ThreadItemType,
     ThreadUser,
     ThreadUserLastSeenAt,
     TypingStatus,
     VoiceMediaItem,
     XMAMediaShareItem,
 )
-from mautrix.appservice import AppService, IntentAPI
-from mautrix.bridge import BasePortal, NotificationDisabler, async_getter_lock
-from mautrix.errors import MatrixError, MForbidden, MNotFound, SessionNotFound
+from mautrix.appservice import DOUBLE_PUPPET_SOURCE_KEY, IntentAPI
+from mautrix.bridge import BasePortal, async_getter_lock
+from mautrix.errors import DecryptionError, MatrixError, MForbidden, MNotFound
 from mautrix.types import (
     AudioInfo,
+    BatchID,
+    BatchSendEvent,
+    BatchSendStateEvent,
     BeeperMessageStatusEventContent,
     ContentURI,
     EventID,
     EventType,
     Format,
     ImageInfo,
     LocationMessageEventContent,
     MediaMessageEventContent,
+    Membership,
+    MemberStateEventContent,
     MessageEventContent,
     MessageStatus,
     MessageStatusReason,
     MessageType,
+    ReactionEventContent,
     RelatesTo,
     RelationType,
     RoomID,
     TextMessageEventContent,
     UserID,
     VideoInfo,
 )
-from mautrix.util import ffmpeg
+from mautrix.util import background_task, ffmpeg
+from mautrix.util.bridge_state import BridgeStateEvent
 from mautrix.util.message_send_checkpoint import MessageSendCheckpointStatus
-from mautrix.util.simple_lock import SimpleLock
 
-from . import matrix as m, puppet as p, user as u
+from . import formatter as fmt, matrix as m, puppet as p, user as u
 from .config import Config
-from .db import Message as DBMessage, Portal as DBPortal, Reaction as DBReaction
+from .db import Backfill, Message as DBMessage, Portal as DBPortal, Reaction as DBReaction
 
 if TYPE_CHECKING:
     from .__main__ import InstagramBridge
 
 try:
     from mautrix.crypto.attachments import decrypt_attachment, encrypt_attachment
 except ImportError:
@@ -106,14 +128,18 @@
     ReelMediaShareItem,
     RegularMediaItem,
     VoiceMediaItem,
     XMAMediaShareItem,
 ]
 MediaUploadFunc = Callable[["u.User", MediaData, IntentAPI], Awaitable[MediaMessageEventContent]]
 
+PortalCreateDummy = EventType.find("fi.mau.dummy.portal_created", EventType.Class.MESSAGE)
+HistorySyncMarkerMessage = EventType.find("org.matrix.msc2716.marker", EventType.Class.MESSAGE)
+ConvertedMessage = tuple[EventType, MessageEventContent]
+
 # This doesn't need to capture all valid URLs, it's enough to catch most of them.
 # False negatives simply mean the link won't be linkified on Instagram,
 # but false positives will cause the message to fail to send.
 SIMPLE_URL_REGEX = re.compile(
     r"(?P<url>https?://[\da-z.-]+\.[a-z]{2,}(?:/[^\s]*)?)", flags=re.IGNORECASE
 )
 
@@ -123,88 +149,98 @@
 
 
 class Portal(DBPortal, BasePortal):
     by_mxid: dict[RoomID, Portal] = {}
     by_thread_id: dict[tuple[str, int], Portal] = {}
     config: Config
     matrix: m.MatrixHandler
-    az: AppService
-    private_chat_portal_meta: bool
+    private_chat_portal_meta: Literal["default", "always", "never"]
 
     _main_intent: IntentAPI | None
     _create_room_lock: asyncio.Lock
-    backfill_lock: SimpleLock
     _msgid_dedup: deque[str]
     _reqid_dedup: set[str]
 
     _last_participant_update: set[int]
     _reaction_lock: asyncio.Lock
-    _backfill_leave: set[IntentAPI] | None
     _typing: set[UserID]
 
     def __init__(
         self,
         thread_id: str,
         receiver: int,
         other_user_pk: int | None,
         mxid: RoomID | None = None,
         name: str | None = None,
         avatar_url: ContentURI | None = None,
         encrypted: bool = False,
         name_set: bool = False,
         avatar_set: bool = False,
         relay_user_id: UserID | None = None,
+        first_event_id: EventID | None = None,
+        next_batch_id: BatchID | None = None,
+        historical_base_insertion_event_id: EventID | None = None,
+        cursor: str | None = None,
+        thread_image_id: int | None = None,
     ) -> None:
         super().__init__(
             thread_id,
             receiver,
             other_user_pk,
             mxid,
             name,
             avatar_url,
             encrypted,
             name_set,
             avatar_set,
             relay_user_id,
+            first_event_id,
+            next_batch_id,
+            historical_base_insertion_event_id,
+            cursor,
+            thread_image_id,
         )
         self._create_room_lock = asyncio.Lock()
         self.log = self.log.getChild(thread_id)
         self._msgid_dedup = deque(maxlen=100)
         self._reqid_dedup = set()
         self._last_participant_update = set()
 
-        self.backfill_lock = SimpleLock(
-            "Waiting for backfilling to finish before handling %s", log=self.log
-        )
-        self._backfill_leave = None
         self._main_intent = None
         self._reaction_lock = asyncio.Lock()
         self._typing = set()
         self._relay_user = None
 
     @property
     def is_direct(self) -> bool:
         return self.other_user_pk is not None
 
     @property
+    def set_dm_room_metadata(self) -> bool:
+        return (
+            not self.is_direct
+            or self.private_chat_portal_meta == "always"
+            or (self.encrypted and self.private_chat_portal_meta != "never")
+        )
+
+    @property
     def main_intent(self) -> IntentAPI:
         if not self._main_intent:
             raise ValueError("Portal must be postinit()ed before main_intent can be used")
         return self._main_intent
 
     @classmethod
     def init_cls(cls, bridge: "InstagramBridge") -> None:
+        BasePortal.bridge = bridge
         cls.config = bridge.config
         cls.matrix = bridge.matrix
         cls.az = bridge.az
         cls.loop = bridge.loop
         cls.bridge = bridge
         cls.private_chat_portal_meta = cls.config["bridge.private_chat_portal_meta"]
-        NotificationDisabler.puppet_cls = p.Puppet
-        NotificationDisabler.config_enabled = cls.config["bridge.backfill.disable_notifications"]
 
     # region Misc
 
     async def _send_delivery_receipt(self, event_id: EventID) -> None:
         if event_id and self.config["bridge.delivery_receipts"]:
             try:
                 await self.az.intent.mark_read(self.mxid, event_id)
@@ -221,15 +257,15 @@
         sender.send_remote_checkpoint(
             status=MessageSendCheckpointStatus.SUCCESS,
             event_id=event_id,
             room_id=self.mxid,
             event_type=event_type,
             message_type=msgtype,
         )
-        asyncio.create_task(self._send_message_status(event_id, err=None))
+        background_task.create(self._send_message_status(event_id, err=None))
         await self._send_delivery_receipt(event_id)
 
     async def _send_bridge_error(
         self,
         sender: u.User,
         err: Exception,
         event_id: EventID,
@@ -255,15 +291,15 @@
             await self._send_message(
                 self.main_intent,
                 TextMessageEventContent(
                     msgtype=MessageType.NOTICE,
                     body=f"\u26a0 Your {event_type_str} {error_type} bridged: {str(err)}",
                 ),
             )
-        asyncio.create_task(self._send_message_status(event_id, err))
+        background_task.create(self._send_message_status(event_id, err))
 
     async def _send_message_status(self, event_id: EventID, err: Exception | None) -> None:
         if not self.config["bridge.message_status_events"]:
             return
         intent = self.az.intent if self.encrypted else self.main_intent
         status = BeeperMessageStatusEventContent(
             network=self.bridge_info_state_key,
@@ -280,15 +316,14 @@
                 status.reason = MessageStatusReason.UNSUPPORTED
                 status.status = MessageStatus.FAIL
             else:
                 status.reason = MessageStatusReason.GENERIC_ERROR
                 status.status = MessageStatus.RETRIABLE
         else:
             status.status = MessageStatus.SUCCESS
-        status.fill_legacy_booleans()
 
         await intent.send_message_event(
             room_id=self.mxid,
             event_type=EventType.BEEPER_MESSAGE_STATUS,
             content=status,
         )
 
@@ -400,45 +435,98 @@
             self.thread_id,
             ThreadItemType.CONFIGURE_PHOTO,
             client_context=request_id,
             upload_id=upload_resp.upload_id,
             allow_full_aspect_ratio="true",
         )
 
+    async def _needs_conversion(
+        self,
+        data: bytes,
+        mime_type: str,
+    ) -> bool:
+        if mime_type != "video/mp4":
+            self.log.info(f"Will convert: mime_type is {mime_type}")
+            return True
+        # Comment this out for now, as it seems like retrying on 500
+        # might be sufficient to fix the video upload problems
+        # (but keep it handy in case it turns out videos are still failing)
+        # else:
+        #     probe = await ffmpeg.probe_bytes(data, input_mime=mime_type, logger=self.log)
+        #     is_there_correct_stream = any(
+        #         "pix_fmt" in stream and stream["pix_fmt"] == "yuv420p"
+        #         for stream in probe["streams"]
+        #     )
+        #     if not is_there_correct_stream:
+        #         self.log.info(f"Will convert: no yuv420p stream found")
+        #         return True
+        #     return False
+
     async def _handle_matrix_video(
         self,
         sender: u.User,
         event_id: EventID,
         request_id: str,
         data: bytes,
         mime_type: str,
         duration: int | None = None,
         width: int | None = None,
         height: int | None = None,
     ) -> CommandResponse:
-        if mime_type != "video/mp4":
+        if await self._needs_conversion(data, mime_type):
             data = await ffmpeg.convert_bytes(
                 data,
                 output_extension=".mp4",
-                output_args=("-c:v", "libx264", "-c:a", "aac"),
+                output_args=(
+                    "-c:v",
+                    "libx264",
+                    "-pix_fmt",
+                    "yuv420p",
+                    "-c:a",
+                    "aac",
+                    "-movflags",
+                    "+faststart",
+                ),
                 input_mime=mime_type,
+                logger=self.log,
             )
+            self.log.info(f"Uploaded video converted")
 
         self.log.trace(f"Uploading video from {event_id}")
         _, upload_id = await sender.client.upload_mp4(
             data, duration_ms=duration, width=width, height=height
         )
         self.log.trace(f"Broadcasting uploaded video with request ID {request_id}")
-        return await sender.client.broadcast(
-            self.thread_id,
-            ThreadItemType.CONFIGURE_VIDEO,
-            client_context=request_id,
-            upload_id=upload_id,
-            video_result="",
-        )
+        retry_num = 0
+        max_retries = 4
+        while True:
+            try:
+                return await sender.client.broadcast(
+                    self.thread_id,
+                    ThreadItemType.CONFIGURE_VIDEO,
+                    client_context=request_id,
+                    upload_id=upload_id,
+                    video_result="",
+                )
+            except IGResponseError as e:
+                if e.response.status == 500 and retry_num < max_retries:
+                    self.log.warning("Received 500 on broadcast, retrying in 5 seconds")
+                    sender.send_remote_checkpoint(
+                        status=MessageSendCheckpointStatus.WILL_RETRY,
+                        event_id=event_id,
+                        room_id=self.mxid,
+                        event_type=EventType.ROOM_MESSAGE,
+                        message_type=MessageType.VIDEO,
+                        error=e,
+                        retry_num=retry_num,
+                    )
+                    await asyncio.sleep(5)
+                    retry_num += 1
+                else:
+                    raise e
 
     async def _handle_matrix_audio(
         self,
         sender: u.User,
         event_id: EventID,
         request_id: str,
         data: bytes,
@@ -464,15 +552,15 @@
         )
 
     async def _handle_matrix_message(
         self, orig_sender: u.User, message: MessageEventContent, event_id: EventID
     ) -> None:
         sender, is_relay = await self.get_relay_sender(orig_sender, f"message {event_id}")
         assert sender, "user is not logged in"
-        assert sender.is_connected, "You're not connected to Instagram"
+        await sender.ensure_connected()
 
         if is_relay:
             await self.apply_relay_message_format(orig_sender, message)
 
         reply_to = {}
         if message.get_reply_to():
             msg = await DBMessage.get_by_mxid(message.get_reply_to(), self.mxid)
@@ -486,18 +574,23 @@
         self._reqid_dedup.add(request_id)
         self.log.debug(
             f"Handling Matrix message {event_id} from {sender.mxid}/{sender.igpk} "
             f"with request ID {request_id}"
         )
 
         if message.msgtype == MessageType.NOTICE and not self.config["bridge.bridge_notices"]:
+            self.log.debug(f"Dropping m.notice event {event_id}")
+            # TODO send checkpoint
             return
 
         if message.msgtype in (MessageType.EMOTE, MessageType.TEXT, MessageType.NOTICE):
-            text = message.body
+            if message.format == Format.HTML:
+                text, reply_to["mentioned_user_ids"] = await fmt.matrix_to_instagram(message)
+            else:
+                text = message.body
             if message.msgtype == MessageType.EMOTE:
                 text = f"/me {text}"
             self.log.trace(f"Sending Matrix text from {event_id} with request ID {request_id}")
             urls = SIMPLE_URL_REGEX.findall(text) or None
             if not self.is_direct:
                 # Instagram groups don't seem to support sending link previews,
                 # and the client_context-based deduplication breaks when trying to send them.
@@ -556,14 +649,16 @@
                 )
         else:
             raise NotImplementedError(f"Unknown message type {message.msgtype}")
 
         self.log.trace(f"Got response to message send {request_id}: {resp}")
         if resp.status != "ok" or not resp.payload:
             self.log.warning(f"Failed to handle {event_id}: {resp}")
+            if resp.exception == "ThreadUserIdDoesNotExist":
+                await orig_sender.logout()
             raise Exception(f"Sending message failed: {resp.error_message}")
         else:
             self._msgid_dedup.appendleft(resp.payload.item_id)
             try:
                 await DBMessage(
                     mxid=event_id,
                     mx_room=self.mxid,
@@ -654,16 +749,15 @@
                 EventType.ROOM_REDACTION,
                 confirmed=True,
             )
         else:
             await self._send_bridge_success(sender, redaction_event_id, EventType.ROOM_REDACTION)
 
     async def _handle_matrix_redaction(self, sender: u.User, event_id: EventID) -> None:
-        if not sender.is_connected:
-            raise Exception("You're not connected to Instagram")
+        await sender.ensure_connected()
 
         reaction = await DBReaction.get_by_mxid(event_id, self.mxid)
         if reaction:
             try:
                 await reaction.delete()
                 await sender.mqtt.send_reaction(
                     self.thread_id,
@@ -696,14 +790,16 @@
             return
         old_typing = self._typing
         self._typing = users
         await self._handle_matrix_typing(old_typing - users, TypingStatus.OFF)
         await self._handle_matrix_typing(users - old_typing, TypingStatus.TEXT)
 
     async def _handle_matrix_typing(self, users: set[UserID], status: TypingStatus) -> None:
+        if not self.config["bridge.bridge_matrix_typing"]:
+            return
         for mxid in users:
             user = await u.User.get_by_mxid(mxid, create=False)
             if (
                 not user
                 or not await user.is_logged_in()
                 or user.remote_typing_status == status
                 or not user.is_connected
@@ -766,19 +862,45 @@
             width=int(media.images.fixed_height.width),
         )
         return await self._reupload_instagram_file(source, url, MessageType.IMAGE, info, intent)
 
     async def _reupload_instagram_xma(
         self, source: u.User, media: XMAMediaShareItem, intent: IntentAPI
     ) -> MediaMessageEventContent:
-        url = media.preview_url
-        info = ImageInfo(
-            mimetype=media.preview_url_mime_type,
+        if media.preview_url:
+            url = media.preview_url
+            info = ImageInfo(mimetype=media.preview_url_mime_type)
+        elif media.preview_url_info:
+            url = media.preview_url_info.url
+            info = ImageInfo(
+                height=media.preview_url_info.height,
+                width=media.preview_url_info.width,
+            )
+        else:
+            raise ValueError("XMA media has now preview URL")
+        reuploaded_image = await self._reupload_instagram_file(
+            source, url, MessageType.IMAGE, info, intent
         )
-        return await self._reupload_instagram_file(source, url, MessageType.IMAGE, info, intent)
+        reel_clip_id = media.reel_share_clip_id
+        if reel_clip_id:
+            try:
+                fetched_clip = await source.client.fetch_clip(reel_clip_id)
+                reuploaded_video = await self._reupload_instagram_media(
+                    source, fetched_clip.media, intent
+                )
+            except Exception:
+                self.log.exception(f"Failed to fetch clip {reel_clip_id}, using fallback")
+            else:
+                reuploaded_video.info.thumbnail_file = reuploaded_image.file
+                reuploaded_video.info.thumbnail_url = reuploaded_image.url
+                reuploaded_video.info.thumbnail_info = reuploaded_image.info
+                return reuploaded_video
+        elif "/reel/" in media.target_url:
+            self.log.warning(f"No reel share clip ID found in {media.target_url}")
+        return reuploaded_image
 
     async def _reupload_instagram_voice(
         self, source: u.User, media: VoiceMediaItem, intent: IntentAPI
     ) -> MediaMessageEventContent:
         async def convert_to_ogg(data, mimetype):
             converted = await ffmpeg.convert_bytes(
                 data, ".ogg", output_args=("-c:a", "libopus"), input_mime=mimetype
@@ -794,43 +916,71 @@
         content["org.matrix.msc1767.audio"] = {
             "duration": media.media.audio.duration,
             "waveform": waveform,
         }
         content["org.matrix.msc3245.voice"] = {}
         return content
 
-    async def _reupload_instagram_file(
-        self,
-        source: u.User,
-        url: str,
-        msgtype: MessageType | None,
-        info: ImageInfo | VideoInfo | AudioInfo,
-        intent: IntentAPI,
-        convert_fn: Callable[[bytes, str], Awaitable[tuple[bytes, str]]] | None = None,
-        allow_encrypt: bool = True,
-    ) -> MediaMessageEventContent:
-        data = None
-        async with source.client.raw_http_get(url) as resp:
+    async def _download_instagram_file(
+        self, source: u.User, url: str
+    ) -> tuple[Optional[bytes], str]:
+        parsed_url = URL(url)
+        if "/" in parsed_url.query_string:
+            # Hacky hacks for forcing encoded slashes in query parameters. Normally yarl/aiohttp
+            # forces decoding slashes in query parameters, but that breaks Instagram's URL signature
+            # and the CDN rejects the request. (the reason there are slashes in the URL in the
+            # first place is presumably that Instagram hasn't heard of URL-safe base64).
+            urlparsed = urlparse(url)
+            parsed_url = parsed_url.with_query(None).with_path(
+                f"{urlparsed.path}?{urlparsed.query}", encoded=True
+            )
+
+        async def handle_resp(resp: ClientResponse) -> tuple[Optional[bytes], str]:
             try:
                 length = int(resp.headers["Content-Length"])
             except KeyError:
                 # TODO can the download be short-circuited if there's too much data?
                 self.log.warning(
                     "Got file download response with no Content-Length header,"
                     "reading data dangerously"
                 )
                 length = 0
             if length > self.matrix.media_config.upload_size:
                 self.log.debug(
-                    f"{url} was too large ({length} > {self.matrix.media_config.upload_size})"
+                    f"{parsed_url} was too large ({length} > {self.matrix.media_config.upload_size})"
                 )
                 raise ValueError("Attachment not available: too large")
+            self.log.debug(f"Downloading file with length {length}: {parsed_url}")
             data = await resp.read()
-            info.mimetype = resp.headers["Content-Type"] or magic.from_buffer(data, mime=True)
+            if not data:
+                return None, ""
+            mimetype = resp.headers["Content-Type"] or magic.from_buffer(data, mime=True)
+            return data, mimetype
+
+        if self.config["bridge.use_proxy_for_media"]:
+            async with source.client.raw_http_get(parsed_url, raise_for_status=True) as resp:
+                return await handle_resp(resp)
+        else:
+            async with ClientSession() as session:
+                async with session.get(parsed_url, raise_for_status=True) as resp:
+                    return await handle_resp(resp)
+
+    async def _reupload_instagram_file(
+        self,
+        source: u.User,
+        url: str,
+        msgtype: MessageType | None,
+        info: ImageInfo | VideoInfo | AudioInfo,
+        intent: IntentAPI,
+        convert_fn: Callable[[bytes, str], Awaitable[tuple[bytes, str]]] | None = None,
+        allow_encrypt: bool = True,
+    ) -> MediaMessageEventContent:
+        data, mimetype = await self._download_instagram_file(source, url)
         assert data is not None
+        info.mimetype = mimetype
 
         # Run the conversion function on the data.
         if convert_fn is not None:
             data, info.mimetype = await convert_fn(data, info.mimetype)
 
         if info.mimetype.startswith("image/") and not info.width and not info.height:
             with BytesIO(data) as inp, Image.open(inp) as img:
@@ -878,22 +1028,26 @@
         # TODO maybe use a dict and item.item_type instead of a ton of ifs
         method = self._reupload_instagram_media
         if (
             item.xma_media_share
             or item.xma_story_share
             or item.xma_reel_share
             or item.xma_reel_mention
+            or item.xma_clip
             or item.generic_xma
+            or item.avatar_sticker
         ):
             media_data = (
                 item.xma_media_share
                 or item.xma_story_share
                 or item.xma_reel_share
                 or item.xma_reel_mention
+                or item.xma_clip
                 or item.generic_xma
+                or item.avatar_sticker
             )[0]
             method = self._reupload_instagram_xma
         elif item.media:
             media_data = item.media
         elif item.visual_media:
             media_data = item.visual_media.media
         elif item.animated_media:
@@ -923,48 +1077,49 @@
         elif isinstance(media_data, ExpiredMediaItem):
             self.log.debug(f"Expired media in item {item}")
             raise ValueError("Attachment not available: media expired")
         return method, media_data
 
     async def _convert_instagram_media(
         self, source: u.User, intent: IntentAPI, item: ThreadItem
-    ) -> MessageEventContent:
+    ) -> ConvertedMessage:
         try:
             reupload_func, media_data = self._get_instagram_media_info(item)
             content = await reupload_func(source, media_data, intent)
         except ValueError as e:
             content = TextMessageEventContent(body=str(e), msgtype=MessageType.NOTICE)
         except Exception:
             self.log.warning("Failed to upload media", exc_info=True)
             content = TextMessageEventContent(
                 body="Attachment not available: failed to copy file", msgtype=MessageType.NOTICE
             )
 
         await self._add_instagram_reply(content, item.replied_to_message)
-        return content
+        return EventType.ROOM_MESSAGE, content
 
     # TODO this might be unused
-    async def _handle_instagram_media_share(
+    async def _convert_instagram_media_share(
         self, source: u.User, intent: IntentAPI, item: ThreadItem
-    ) -> EventID | None:
+    ) -> list[ConvertedMessage]:
         item_type_name = None
         if item.media_share:
             share_item = item.media_share
         elif item.clip:
             share_item = item.clip.clip
             item_type_name = "clip"
         elif item.felix_share and item.felix_share.video:
             share_item = item.felix_share.video
         elif item.story_share:
             share_item = item.story_share.media
             item_type_name = "story"
         elif item.direct_media_share:
             share_item = item.direct_media_share.media
         else:
-            return None
+            self.log.debug("No media share to bridge")
+            return []
         item_type_name = item_type_name or share_item.media_type.human_name
         user_text = f"@{share_item.user.username}"
         user_link = (
             f'<a href="https://www.instagram.com/{share_item.user.username}/">{user_text}</a>'
         )
         prefix = TextMessageEventContent(
             msgtype=MessageType.NOTICE,
@@ -975,25 +1130,25 @@
         if item.direct_media_share and item.direct_media_share.media_share_type == "tag":
             tagged_user_id = item.direct_media_share.tagged_user_id
             if tagged_user_id == source.igpk and share_item.user.pk == self.other_user_pk:
                 prefix.body = prefix.formatted_body = "Tagged you in their post"
             elif share_item.user.pk == source.igpk and tagged_user_id == self.other_user_pk:
                 prefix.body = prefix.formatted_body = "Tagged them in your post"
 
-        content = await self._convert_instagram_media(source, intent, item)
+        _, content = await self._convert_instagram_media(source, intent, item)
 
         external_url = f"https://www.instagram.com/p/{share_item.code}/"
-        if share_item.caption:
+        if share_item.caption and item_type_name != "clip":
             caption_body = (
                 f"> {share_item.caption.user.username}: {share_item.caption.text}\n\n"
                 f"{external_url}"
             )
             caption_formatted_body = (
-                f"<blockquote><strong>{share_item.caption.user.username}</strong>"
-                f" {html.escape(share_item.caption.text)}</blockquote>"
+                f"<strong>{share_item.caption.user.username}</strong>"
+                f" {html.escape(share_item.caption.text)}"
                 f'<a href="{external_url}">instagram.com/p/{share_item.code}</a>'
             )
         else:
             caption_body = external_url
             caption_formatted_body = (
                 f'<a href="{external_url}">instagram.com/p/{share_item.code}</a>'
             )
@@ -1035,55 +1190,62 @@
                 combined["format"] = str(Format.HTML)
                 combined["org.matrix.msc1767.caption"] = {
                     "org.matrix.msc1767.text": combined_body,
                     "org.matrix.msc1767.html": combined_formatted_body,
                 }
                 combined["formatted_body"] = combined_formatted_body
 
-            event_id = await self._send_message(intent, combined, timestamp=item.timestamp_ms)
+            return [(EventType.ROOM_MESSAGE, combined)]
         else:
-            await self._send_message(intent, prefix, timestamp=item.timestamp_ms)
-            event_id = await self._send_message(intent, content, timestamp=item.timestamp_ms)
-            await self._send_message(intent, caption, timestamp=item.timestamp_ms)
-
-        return event_id
+            return [
+                (EventType.ROOM_MESSAGE, prefix),
+                (EventType.ROOM_MESSAGE, content),
+                (EventType.ROOM_MESSAGE, caption),
+            ]
 
-    async def _handle_instagram_xma_media_share(
+    async def _convert_instagram_xma_media_share(
         self, source: u.User, intent: IntentAPI, item: ThreadItem
-    ) -> EventID | None:
+    ) -> list[ConvertedMessage]:
         # N.B. _get_instagram_media_info also only supports downloading the first xma item
         xma_list = (
             item.xma_media_share
             or item.xma_story_share
             or item.xma_reel_share
             or item.xma_reel_mention
+            or item.xma_clip
             or item.generic_xma
+            or item.avatar_sticker
         )
         media = xma_list[0]
         if len(xma_list) != 1:
             self.log.warning(f"Item {item.item_id} has multiple xma media share parts")
         if media.xma_layout_type not in (0, 4):
             self.log.warning(f"Unrecognized xma layout type {media.xma_layout_type}")
-        content = await self._convert_instagram_media(source, intent, item)
+        if media.preview_url or media.preview_url_info:
+            _, content = await self._convert_instagram_media(source, intent, item)
+        else:
+            content = None
 
         # Post shares (layout type 0): media title text
         # Reel shares/replies/reactions (layout type 4): item text
         caption_text = media.title_text or item.text or ""
+        post_caption_text = None
         if media.subtitle_text:
             caption_text = (
                 f"{caption_text}\n{media.subtitle_text}" if caption_text else media.subtitle_text
             )
-        if media.target_url:
-            caption_body = (
-                f"> {caption_text}\n\n{media.target_url}" if caption_text else media.target_url
-            )
-        else:
-            caption_body = f"> {caption_text}"
+        header_text = media.header_title_text or ""
+        # Note replies have title_text for sender username, caption_body_text for the original note
+        # and item.text for the reply itself.
+        if not header_text and media.caption_body_text:
+            header_text = caption_text
+            caption_text = media.caption_body_text
+            post_caption_text = item.text
         escaped_caption_text = html.escape(caption_text).replace("\n", "<br>")
-        escaped_header_text = html.escape(media.header_title_text or "")
+        escaped_header_text = html.escape(header_text)
         # For post shares, the media title starts with the username, which is also the header.
         # That part should be bolded.
         if (
             escaped_header_text
             and escaped_caption_text
             and escaped_caption_text.startswith(escaped_header_text)
         ):
@@ -1107,38 +1269,56 @@
             )
             escaped_caption_text = (
                 f"{escaped_caption_text}<br/>{inline_img}" if escaped_caption_text else inline_img
             )
         caption_formatted_body = (
             f"<blockquote>{escaped_caption_text}</blockquote>" if escaped_caption_text else ""
         )
-        if media.target_url:
+        if media.target_url and media.target_url.startswith("https://"):
+            caption_body = (
+                f"> {caption_text}\n\n{media.target_url}" if caption_text else media.target_url
+            )
             target_url_pretty = str(URL(media.target_url).with_query(None)).replace(
                 "https://www.", ""
             )
             caption_formatted_body += (
                 f'<p><a href="{media.target_url}">{target_url_pretty}</a></p>'
             )
+        else:
+            caption_body = f"> {caption_text}" if caption_text else ""
+        if post_caption_text:
+            caption_formatted_body += f"<p>{html.escape(post_caption_text)}</p>"
+            caption_body += f"\n\n{post_caption_text}"
         # Add auxiliary text as prefix for caption
         if item.auxiliary_text:
             caption_formatted_body = (
                 f"<p>{html.escape(item.auxiliary_text)}</p>{caption_formatted_body}"
             )
             caption_body = f"{item.auxiliary_text}\n\n{caption_body}"
+        elif len(xma_list) > 1:
+            caption_formatted_body = f"<p>Sent {len(xma_list)} items</p>{caption_formatted_body}"
+            caption_body = f"Sent {len(xma_list)} items\n\n{caption_body}"
+
         caption = TextMessageEventContent(
             msgtype=MessageType.TEXT,
             body=caption_body,
             formatted_body=caption_formatted_body,
             format=Format.HTML,
         )
-        if media.target_url:
+        if content and media.target_url:
             content.external_url = media.target_url
             caption.external_url = media.target_url
 
-        if self.bridge.config["bridge.caption_in_message"]:
+        if not caption_body:
+            if content is None:
+                return []
+            return [(EventType.ROOM_MESSAGE, content)]
+        elif content is None:
+            return [(EventType.ROOM_MESSAGE, caption)]
+        elif self.bridge.config["bridge.caption_in_message"]:
             if isinstance(content, TextMessageEventContent):
                 content.ensure_has_html()
                 caption.ensure_has_html()
                 content.body += f"\n\n{caption.body}"
                 content.formatted_body = (
                     f"<p><b>{content.formatted_body}</b></p>{caption.formatted_body}"
                 )
@@ -1148,25 +1328,22 @@
                 content["format"] = str(Format.HTML)
                 content["formatted_body"] = caption.formatted_body
                 content["org.matrix.msc1767.caption"] = {
                     "org.matrix.msc1767.text": content.body,
                     "org.matrix.msc1767.html": content["formatted_body"],
                 }
 
-            event_id = await self._send_message(intent, content, timestamp=item.timestamp_ms)
+            return [(EventType.ROOM_MESSAGE, content)]
         else:
-            event_id = await self._send_message(intent, content, timestamp=item.timestamp_ms)
-            await self._send_message(intent, caption, timestamp=item.timestamp_ms)
-
-        return event_id
+            return [(EventType.ROOM_MESSAGE, content), (EventType.ROOM_MESSAGE, caption)]
 
     # TODO this is probably unused
-    async def _handle_instagram_reel_share(
+    async def _convert_instagram_reel_share(
         self, source: u.User, intent: IntentAPI, item: ThreadItem
-    ) -> EventID | None:
+    ) -> list[ConvertedMessage]:
         assert item.reel_share
         media = item.reel_share.media
         prefix_html = None
         if item.reel_share.type == ReelShareType.REPLY:
             if item.reel_share.reel_owner_id == source.igpk:
                 prefix = "Replied to your story"
             else:
@@ -1184,15 +1361,15 @@
         elif item.reel_share.type == ReelShareType.MENTION:
             if item.reel_share.mentioned_user_id == source.igpk:
                 prefix = "Mentioned you in their story"
             else:
                 prefix = "You mentioned them in your story"
         else:
             self.log.debug(f"Unsupported reel share type {item.reel_share.type}")
-            return None
+            return []
         prefix_content = TextMessageEventContent(msgtype=MessageType.NOTICE, body=prefix)
         if prefix_html:
             prefix_content.format = Format.HTML
             prefix_content.formatted_body = prefix_html
         caption_content = TextMessageEventContent(
             msgtype=MessageType.TEXT, body=item.reel_share.text
         )
@@ -1210,15 +1387,15 @@
         else:
             existing = await DBMessage.get_by_item_id(fake_item_id, self.receiver)
             if existing:
                 # If the user already reacted or replied to the same reel share item,
                 # use a Matrix reply instead of reposting the image.
                 caption_content.set_reply(existing.mxid)
             else:
-                media_content = await self._convert_instagram_media(source, intent, item)
+                _, media_content = await self._convert_instagram_media(source, intent, item)
 
         if self.bridge.config["bridge.caption_in_message"]:
             if media_content:
                 if isinstance(media_content, TextMessageEventContent):
                     media_content.ensure_has_html()
                     prefix_content.ensure_has_html()
                     caption_content.ensure_has_html()
@@ -1251,41 +1428,29 @@
                         "org.matrix.msc1767.text": combined_body,
                         "org.matrix.msc1767.html": combined_formatted_body,
                     }
                     combined["formatted_body"] = combined_formatted_body
             else:
                 combined = caption_content
 
-            event_id = await self._send_message(intent, combined, timestamp=item.timestamp_ms)
+            return [(EventType.ROOM_MESSAGE, combined)]
         else:
             await self._send_message(intent, prefix_content, timestamp=item.timestamp_ms)
+            converted: list[ConvertedMessage] = []
             if media_content:
-                media_event_id = await self._send_message(
-                    intent, media_content, timestamp=item.timestamp_ms
-                )
-                await DBMessage(
-                    mxid=media_event_id,
-                    mx_room=self.mxid,
-                    item_id=fake_item_id,
-                    client_context=None,
-                    receiver=self.receiver,
-                    sender=media.user.pk,
-                    ig_timestamp=None,
-                ).insert()
-            event_id = await self._send_message(
-                intent, caption_content, timestamp=item.timestamp_ms
-            )
-        return event_id
+                converted.append((EventType.ROOM_MESSAGE, media_content))
+            converted.append((EventType.ROOM_MESSAGE, caption_content))
+            return converted
 
-    async def _handle_instagram_link(
+    async def _convert_instagram_link(
         self,
         source: u.User,
         intent: IntentAPI,
         item: ThreadItem,
-    ) -> EventID:
+    ) -> ConvertedMessage:
         content = TextMessageEventContent(msgtype=MessageType.TEXT, body=item.link.text)
         link = item.link.link_context
         preview = {
             "og:url": link.link_url,
             "og:title": link.link_title,
             "og:description": link.link_summary,
         }
@@ -1299,36 +1464,56 @@
             preview["og:image:height"] = reuploaded.info.height
             preview["matrix:image:size"] = reuploaded.info.size
             if reuploaded.file:
                 preview["beeper:image:encryption"] = reuploaded.file.serialize()
         preview = {k: v for k, v in preview.items() if v}
         content["com.beeper.linkpreviews"] = [preview] if "og:title" in preview else []
         await self._add_instagram_reply(content, item.replied_to_message)
-        return await self._send_message(intent, content, timestamp=item.timestamp_ms)
+        return EventType.ROOM_MESSAGE, content
 
-    async def _handle_instagram_text(
-        self, intent: IntentAPI, item: ThreadItem, text: str
-    ) -> EventID:
+    async def _convert_expired_placeholder(
+        self, source: u.User, item: ThreadItem, action: str
+    ) -> ConvertedMessage:
+        if item.user_id == source.igpk:
+            prefix = f"{action} your story"
+        elif item.user_id == source.igpk:
+            prefix = f"You {action.lower()} their story"
+        else:
+            prefix = f"{action} a story"
+        body = f"{prefix}\n\nNo longer available"
+        html = f"<p>{prefix}</p><p><i>No longer available</i></p>"
+        content = TextMessageEventContent(
+            msgtype=MessageType.NOTICE, body=body, format=Format.HTML, formatted_body=html
+        )
+        return EventType.ROOM_MESSAGE, content
+
+    async def _convert_instagram_text(self, item: ThreadItem, text: str) -> ConvertedMessage:
         content = TextMessageEventContent(msgtype=MessageType.TEXT, body=text)
         content["com.beeper.linkpreviews"] = []
         await self._add_instagram_reply(content, item.replied_to_message)
-        return await self._send_message(intent, content, timestamp=item.timestamp_ms)
+        return EventType.ROOM_MESSAGE, content
+
+    async def _convert_instagram_placeholder(self, item: ThreadItem) -> ConvertedMessage:
+        content = TextMessageEventContent(
+            msgtype=MessageType.NOTICE, body=item.placeholder.message
+        )
+        content["com.beeper.linkpreviews"] = []
+        await self._add_instagram_reply(content, item.replied_to_message)
+        return EventType.ROOM_MESSAGE, content
 
-    async def _send_instagram_unhandled(self, intent: IntentAPI, item: ThreadItem) -> EventID:
+    async def _convert_instagram_unhandled(self, item: ThreadItem) -> ConvertedMessage:
         content = TextMessageEventContent(
             msgtype=MessageType.NOTICE, body=f"Unsupported message type {item.item_type.value}"
         )
         await self._add_instagram_reply(content, item.replied_to_message)
-        return await self._send_message(intent, content, timestamp=item.timestamp_ms)
+        return EventType.ROOM_MESSAGE, content
 
-    async def _handle_instagram_location(
-        self, intent: IntentAPI, item: ThreadItem
-    ) -> EventID | None:
+    async def _convert_instagram_location(self, item: ThreadItem) -> ConvertedMessage | None:
         loc = item.location
-        if not loc.lng or not loc.lat:
+        if not loc or not loc.lng or not loc.lat:
             # TODO handle somehow
             return None
         long_char = "E" if loc.lng > 0 else "W"
         lat_char = "N" if loc.lat > 0 else "S"
 
         body = (
             f"{loc.name} - {round(abs(loc.lat), 4)}° {lat_char}, "
@@ -1346,38 +1531,43 @@
             body=f"Location: {body}\n{url}",
             external_url=external_url,
         )
         content["format"] = str(Format.HTML)
         content["formatted_body"] = f"Location: <a href='{url}'>{body}</a>"
 
         await self._add_instagram_reply(content, item.replied_to_message)
+        return EventType.ROOM_MESSAGE, content
 
-        return await self._send_message(intent, content, timestamp=item.timestamp_ms)
-
-    async def _handle_instagram_profile(
-        self, intent: IntentAPI, item: ThreadItem
-    ) -> EventID | None:
+    async def _convert_instagram_profile(self, item: ThreadItem) -> ConvertedMessage:
         username = item.profile.username
         user_link = f'<a href="https://www.instagram.com/{username}/">@{username}</a>'
         text = f"Shared @{username}'s profile"
         html = f"Shared {user_link}'s profile"
         content = TextMessageEventContent(
             msgtype=MessageType.TEXT, format=Format.HTML, body=text, formatted_body=html
         )
         await self._add_instagram_reply(content, item.replied_to_message)
-        return await self._send_message(intent, content, timestamp=item.timestamp_ms)
+        return EventType.ROOM_MESSAGE, content
 
-    async def handle_instagram_item(
-        self, source: u.User, sender: p.Puppet, item: ThreadItem, is_backfill: bool = False
-    ) -> None:
-        try:
-            await self._handle_instagram_item(source, sender, item, is_backfill)
-        except Exception:
-            self.log.exception("Fatal error handling Instagram item")
-            self.log.trace("Item content: %s", item.serialize())
+    async def _convert_instagram_xma_profile_share(
+        self, item: ThreadItem
+    ) -> list[ConvertedMessage]:
+        assert item.xma_profile
+        profile_messages = []
+        for profile in item.xma_profile:
+            username = profile.header_title_text
+            user_link = f'<a href="{profile.target_url}">@{username}</a>'
+            text = f"Shared @{username}'s profile"
+            html = f"Shared {user_link}'s profile"
+            content = TextMessageEventContent(
+                msgtype=MessageType.TEXT, format=Format.HTML, body=text, formatted_body=html
+            )
+            await self._add_instagram_reply(content, item.replied_to_message)
+            profile_messages.append((EventType.ROOM_MESSAGE, content))
+        return profile_messages
 
     async def _add_instagram_reply(
         self, content: MessageEventContent, reply_to: ThreadItem | None
     ) -> None:
         if not reply_to:
             return
 
@@ -1395,150 +1585,211 @@
             evt = None
         if not evt:
             return
 
         if evt.type == EventType.ROOM_ENCRYPTED:
             try:
                 evt = await self.matrix.e2ee.decrypt(evt, wait_session_timeout=0)
-            except SessionNotFound:
+            except DecryptionError:
                 return
 
         if isinstance(evt.content, TextMessageEventContent):
             evt.content.trim_reply_fallback()
 
         content.set_reply(evt)
 
-    async def _handle_instagram_item(
-        self, source: u.User, sender: p.Puppet, item: ThreadItem, is_backfill: bool = False
-    ) -> None:
-        if not isinstance(item, ThreadItem):
-            # Parsing these items failed, they should have been logged already
-            return
-
+    async def handle_instagram_item(
+        self, source: u.User, sender: p.Puppet, item: MessageSyncMessage
+    ):
         client_context = item.client_context
         link_client_context = item.link.client_context if item.link else None
         cc = client_context
         if link_client_context:
             if not client_context:
                 cc = f"link:{link_client_context}"
             elif client_context != link_client_context:
                 cc = f"{client_context}/link:{link_client_context}"
         if client_context and client_context in self._reqid_dedup:
             self.log.debug(
                 f"Ignoring message {item.item_id} ({cc}) by {item.user_id}"
                 " as it was sent by us (client_context in dedup queue)"
             )
-            return
+            return []
         elif link_client_context and link_client_context in self._reqid_dedup:
             self.log.debug(
                 f"Ignoring message {item.item_id} ({cc}) by {item.user_id}"
                 " as it was sent by us (link.client_context in dedup queue)"
             )
-            return
+            return []
 
+        # Check in-memory queues for duplicates
         if item.item_id in self._msgid_dedup:
             self.log.debug(
-                f"Ignoring message {item.item_id} ({cc}) by {item.user_id}"
+                f"Ignoring message {item.item_id} ({item.client_context}) by {item.user_id}"
                 " as it was already handled (message.id in dedup queue)"
             )
             return
         self._msgid_dedup.appendleft(item.item_id)
 
+        # Check database for duplicates
         if await DBMessage.get_by_item_id(item.item_id, self.receiver) is not None:
             self.log.debug(
-                f"Ignoring message {item.item_id} ({cc}) by {item.user_id}"
+                f"Ignoring message {item.item_id} ({item.client_context}) by {item.user_id}"
                 " as it was already handled (message.id in database)"
             )
             return
 
-        self.log.debug(f"Starting handling of message {item.item_id} ({cc}) by {item.user_id}")
-        asyncio.create_task(sender.intent_for(self).set_typing(self.mxid, is_typing=False))
-        await self._handle_deduplicated_instagram_item(source, sender, item, is_backfill)
+        self.log.debug(
+            f"Handling Instagram message {item.item_id} ({item.client_context}) by {item.user_id}"
+        )
 
-    async def _handle_deduplicated_instagram_item(
-        self, source: u.User, sender: p.Puppet, item: ThreadItem, is_backfill: bool = False
-    ) -> None:
-        if self.backfill_lock.locked and sender.need_backfill_invite(self):
-            self.log.debug("Adding %s's default puppet to room for backfilling", sender.mxid)
-            if self.is_direct:
-                await self.main_intent.invite_user(self.mxid, sender.default_mxid)
-            intent = sender.default_mxid_intent
-            await intent.ensure_joined(self.mxid)
-            self._backfill_leave.add(intent)
-        else:
-            intent = sender.intent_for(self)
-        event_id = None
-        needs_handling = True
-        allow_text_handle = True
+        intent = sender.intent_for(self)
+        background_task.create(intent.set_typing(self.mxid, timeout=0))
+        event_ids = []
+        for event_type, content in await self.convert_instagram_item(source, sender, item):
+            event_ids.append(
+                await self._send_message(
+                    intent, content, event_type=event_type, timestamp=item.timestamp_ms
+                )
+            )
+        event_ids = [event_id for event_id in event_ids if event_id]
+        if not event_ids:
+            self.log.warning(f"Unhandled Instagram message {item.item_id}")
+            return
+        self.log.debug(f"Handled Instagram message {item.item_id} -> {event_ids}")
+        await DBMessage(
+            mxid=event_ids[-1],
+            mx_room=self.mxid,
+            item_id=item.item_id,
+            client_context=item.client_context,
+            receiver=self.receiver,
+            sender=sender.igpk,
+            ig_timestamp=item.timestamp,
+        ).insert()
+        await self._send_delivery_receipt(event_ids[-1])
+
+    async def convert_instagram_item(
+        self, source: u.User, sender: p.Puppet, item: ThreadItem
+    ) -> list[ConvertedMessage]:
+        if not isinstance(item, ThreadItem):
+            # Parsing these items failed, they should have been logged already
+            return []
+
+        try:
+            return await self._convert_instagram_item(source, sender, item)
+        except Exception:
+            self.log.exception("Fatal error converting Instagram item")
+            self.log.trace("Item content: %s", item.serialize())
+            return []
+
+    async def _convert_instagram_item(
+        self, source: u.User, sender: p.Puppet, item: ThreadItem
+    ) -> list[ConvertedMessage]:
+        intent = sender.intent_for(self)
         if (
             item.xma_media_share
             or item.xma_reel_share
             or item.xma_reel_mention
             or item.xma_story_share
+            or item.xma_clip
             or item.generic_xma
+            or item.avatar_sticker
         ):
-            event_id = await self._handle_instagram_xma_media_share(source, intent, item)
-            allow_text_handle = False
-        elif item.media or item.animated_media or item.voice_media or item.visual_media:
-            content = await self._convert_instagram_media(source, intent, item)
-            event_id = await self._send_message(intent, content, timestamp=item.timestamp_ms)
+            return await self._convert_instagram_xma_media_share(source, intent, item)
+
+        converted: list[ConvertedMessage] = []
+        handle_text = True
+
+        if item.media or item.animated_media or item.voice_media or item.visual_media:
+            converted.append(await self._convert_instagram_media(source, intent, item))
         elif item.location:
-            event_id = await self._handle_instagram_location(intent, item)
+            if loc_content := await self._convert_instagram_location(item):
+                converted.append(loc_content)
         elif item.profile:
-            event_id = await self._handle_instagram_profile(intent, item)
+            converted.append(await self._convert_instagram_profile(item))
+        elif item.xma_profile:
+            converted.extend(await self._convert_instagram_xma_profile_share(item))
         elif item.reel_share:
-            event_id = await self._handle_instagram_reel_share(source, intent, item)
+            converted.extend(await self._convert_instagram_reel_share(source, intent, item))
         elif (
             item.media_share
             or item.direct_media_share
             or item.story_share
             or item.clip
             or item.felix_share
         ):
-            event_id = await self._handle_instagram_media_share(source, intent, item)
+            converted.extend(await self._convert_instagram_media_share(source, intent, item))
+        elif item.item_type == ThreadItemType.EXPIRED_PLACEHOLDER:
+            if item.message_item_type == "reaction":
+                action = "Reacted to"
+            else:
+                action = "Shared"
+            msg_type, expired = await self._convert_expired_placeholder(source, item, action)
+            if self.bridge.config["bridge.caption_in_message"] and item.text:
+                _, text = await self._convert_instagram_text(item, item.text)
+                expired.ensure_has_html()
+                text.ensure_has_html()
+                combined = TextMessageEventContent(
+                    msgtype=MessageType.TEXT,
+                    body="\n".join((expired.body, text.body)),
+                    formatted_body=f"{expired.formatted_body}<p>{text.formatted_body}</p>",
+                    format=Format.HTML,
+                )
+                handle_text = False
+                converted.append((msg_type, combined))
+            else:
+                converted.append((msg_type, expired))
+        elif item.video_call_event:
+            msg_type = (
+                MessageType.NOTICE
+                if item.video_call_event.action == "video_call_ended"
+                else MessageType.TEXT
+            )
+            video_call_notification = TextMessageEventContent(
+                msgtype=msg_type,
+                body=item.video_call_event.description,
+                formatted_body=f"<b>{item.video_call_event.description}</b>",
+                format=Format.HTML,
+            )
+            converted.append((EventType.ROOM_MESSAGE, video_call_notification))
         elif item.action_log:
             # These probably don't need to be bridged
-            needs_handling = False
             self.log.debug(f"Ignoring action log message {item.item_id}")
+            return []
+
         # TODO handle item.clip?
-        if item.text and allow_text_handle:
-            event_id = await self._handle_instagram_text(intent, item, item.text)
+        # TODO should these be put into a caption?
+        if handle_text and item.text:
+            converted.append(await self._convert_instagram_text(item, item.text))
         elif item.like:
             # We handle likes as text because Matrix clients do big emoji on their own.
-            event_id = await self._handle_instagram_text(intent, item, item.like)
+            converted.append(await self._convert_instagram_text(item, item.like))
         elif item.link:
-            event_id = await self._handle_instagram_link(source, intent, item)
-        handled = bool(event_id)
-        if not event_id and needs_handling:
+            converted.append(await self._convert_instagram_link(source, intent, item))
+        elif item.placeholder and len(converted) == 0:
+            self.log.warning(
+                f"Got placeholder item in {item.item_id}: {item.placeholder.serialize()}"
+            )
+            converted.append(await self._convert_instagram_placeholder(item))
+
+        if len(converted) == 0:
             self.log.debug(f"Unhandled Instagram message {item.item_id}")
-            event_id = await self._send_instagram_unhandled(intent, item)
+            converted.append(await self._convert_instagram_unhandled(item))
 
-        cc = item.client_context
-        if not cc and item.link and item.link.client_context:
-            cc = item.link.client_context
-        msg = DBMessage(
-            mxid=event_id,
-            mx_room=self.mxid,
-            item_id=item.item_id,
-            client_context=cc,
-            receiver=self.receiver,
-            sender=sender.pk,
-            ig_timestamp=item.timestamp,
-        )
-        await msg.insert()
-        await self._send_delivery_receipt(event_id)
-        if handled:
-            self.log.debug(f"Handled Instagram message {item.item_id} -> {event_id}")
-        elif needs_handling:
-            self.log.debug(
-                f"Unhandled Instagram message {item.item_id} "
-                f"(type {item.item_type} -> fallback error {event_id})"
-            )
-        if is_backfill and item.reactions:
-            await self._handle_instagram_reactions(msg, item.reactions.emojis, is_backfill=True)
+        return converted
+
+    def _deterministic_event_id(
+        self, sender: p.Puppet, item_id: str, part_name: int | None = None
+    ) -> EventID:
+        hash_content = f"{self.mxid}/instagram/{sender.igpk}/{item_id}"
+        if part_name:
+            hash_content += f"/{part_name}"
+        hashed = hashlib.sha256(hash_content.encode("utf-8")).digest()
+        b64hash = base64.urlsafe_b64encode(hashed).decode("utf-8").rstrip("=")
+        return EventID(f"${b64hash}:instagram.com")
 
     async def handle_instagram_remove(self, item_id: str) -> None:
         message = await DBMessage.get_by_item_id(item_id, self.receiver)
         if message is None:
             return
         await message.delete()
         if message.mxid:
@@ -1582,32 +1833,28 @@
                     existing, intent, reaction_event_id, message, sender, emoji, timestamp
                 )
                 self.log.debug(
                     f"Handled {sender.pk}'s reaction to {item.item_id} -> {reaction_event_id}"
                 )
 
     async def _handle_instagram_reactions(
-        self, message: DBMessage, reactions: list[Reaction], is_backfill: bool = False
+        self, message: DBMessage, reactions: list[Reaction]
     ) -> None:
         old_reactions: dict[int, DBReaction]
         old_reactions = {
             reaction.ig_sender: reaction
             for reaction in await DBReaction.get_all_by_item_id(message.item_id, self.receiver)
         }
-        timestamp_deduplicator = 1
         for new_reaction in reactions:
             old_reaction = old_reactions.pop(new_reaction.sender_id, None)
             if old_reaction and old_reaction.reaction == new_reaction.emoji:
                 continue
             puppet = await p.Puppet.get_by_pk(new_reaction.sender_id)
             intent = puppet.intent_for(self)
-            timestamp = new_reaction.timestamp_ms if is_backfill else int(time.time() * 1000)
-            if is_backfill:
-                timestamp += timestamp_deduplicator
-                timestamp_deduplicator += 1
+            timestamp = int(time.time() * 1000)
             reaction_event_id = await intent.react(
                 self.mxid, message.mxid, new_reaction.emoji, timestamp=timestamp
             )
             await self._upsert_reaction(
                 old_reaction,
                 intent,
                 reaction_event_id,
@@ -1641,77 +1888,104 @@
     def _get_thread_name(self, thread: Thread) -> str:
         if self.is_direct:
             if self.other_user_pk == thread.viewer_id and len(thread.users) == 0:
                 return "Instagram chat with yourself"
             elif len(thread.users) == 1:
                 tpl = self.config["bridge.private_chat_name_template"]
                 ui = thread.users[0]
-                return tpl.format(displayname=ui.full_name, id=ui.pk, username=ui.username)
-            pass
+                return tpl.format(
+                    displayname=ui.full_name or ui.username, id=ui.pk, username=ui.username
+                )
         elif thread.thread_title:
             return self.config["bridge.group_chat_name_template"].format(name=thread.thread_title)
-        else:
-            return ""
+
+        return ""
+
+    async def update_thread_image(
+        self, source: u.User, thread_image: ThreadImage, sender: p.Puppet | None = None
+    ) -> bool:
+        if (
+            self.is_direct
+            or not thread_image
+            or (self.thread_image_id == thread_image.id and self.avatar_set)
+        ):
+            return False
+
+        best = thread_image.best_image
+        if not best:
+            return False
+        data, mimetype = await self._download_instagram_file(source, best.url)
+        if not data:
+            return False
+        self.thread_image_id = thread_image.id
+        self.avatar_set = False
+        mxc = await self.main_intent.upload_media(
+            data=data,
+            mime_type=mimetype,
+            filename=str(thread_image.id),
+            async_upload=self.config["homeserver.async_media"],
+        )
+        return await self._update_photo(mxc, sender=sender)
 
     async def update_info(self, thread: Thread, source: u.User) -> None:
         changed = await self._update_name(self._get_thread_name(thread))
+        changed = await self.update_thread_image(source, thread.thread_image) or changed
         changed = await self._update_participants(thread.users, source) or changed
         if changed:
             await self.update_bridge_info()
             await self.update()
         # TODO update power levels with thread.admin_user_ids
 
     async def update_info_from_puppet(self, puppet: p.Puppet | None = None) -> None:
         if not self.is_direct:
             return
         if not puppet:
             puppet = await self.get_dm_puppet()
-        await self._update_photo_from_puppet(puppet)
+        await self._update_photo(puppet.photo_mxc)
         if self.name and not self.name_set:
             await self._update_name(self.name)
 
     async def _update_name(self, name: str) -> bool:
-        if name and (self.name != name or not self.name_set):
+        if name and (self.name != name or (not self.name_set and self.set_dm_room_metadata)):
             self.name = name
             if self.mxid:
                 try:
                     await self.main_intent.set_room_name(self.mxid, name)
                     self.name_set = True
                 except Exception:
                     self.log.exception("Failed to update name")
                     self.name_set = False
             return True
         return False
 
-    async def _update_photo_from_puppet(self, puppet: p.Puppet) -> bool:
-        if not self.private_chat_portal_meta and not self.encrypted:
+    async def _update_photo(self, photo_mxc: ContentURI, sender: p.Puppet | None = None) -> bool:
+        if self.avatar_url == photo_mxc and (self.avatar_set or not self.set_dm_room_metadata):
             return False
-        if self.avatar_set and self.avatar_url == puppet.photo_mxc:
-            return False
-        self.avatar_url = puppet.photo_mxc
-        if self.mxid:
+        self.avatar_url = photo_mxc
+        self.avatar_set = False
+        if self.mxid and self.set_dm_room_metadata:
             try:
-                await self.main_intent.set_room_avatar(self.mxid, puppet.photo_mxc)
+                # TODO use sender intent
+                await self.main_intent.set_room_avatar(self.mxid, photo_mxc)
                 self.avatar_set = True
             except Exception:
                 self.log.exception("Failed to set room avatar")
-                self.avatar_set = False
         return True
 
     async def _update_participants(self, users: list[ThreadUser], source: u.User) -> bool:
         meta_changed = False
 
         # Make sure puppets who should be here are here
         for user in users:
             puppet = await p.Puppet.get_by_pk(user.pk)
             await puppet.update_info(user, source)
             if self.mxid:
                 await puppet.intent_for(self).ensure_joined(self.mxid)
             if puppet.pk == self.other_user_pk:
-                meta_changed = await self._update_photo_from_puppet(puppet)
+                meta_changed = await self._update_photo(puppet.photo_mxc)
 
         if self.mxid:
             # Kick puppets who shouldn't be here
             current_members = {int(user.pk) for user in users}
             for user_id in await self.main_intent.get_room_members(self.mxid):
                 pk = p.Puppet.get_id_from_mxid(user_id)
                 if pk and pk not in current_members and pk != self.other_user_pk:
@@ -1754,78 +2028,483 @@
 
     async def get_dm_puppet(self) -> p.Puppet | None:
         if not self.is_direct:
             return None
         return await p.Puppet.get_by_pk(self.other_user_pk)
 
     # endregion
-    # region Backfilling
+    # region Backfill
 
-    async def backfill(self, source: u.User, thread: Thread, is_initial: bool = False) -> None:
-        limit = (
-            self.config["bridge.backfill.initial_limit"]
-            if is_initial
-            else self.config["bridge.backfill.missed_limit"]
-        )
-        if limit == 0:
-            return
-        elif limit < 0:
-            limit = None
-        with self.backfill_lock:
-            await self._backfill(source, thread, is_initial, limit)
+    async def enqueue_immediate_backfill(self, source: u.User, priority: int) -> None:
+        assert self.config["bridge.backfill.msc2716"]
+        max_pages = self.config["bridge.backfill.incremental.max_pages"]
+        max_total_pages = self.config["bridge.backfill.incremental.max_total_pages"]
+        if max_pages <= 0 or max_total_pages == 0:
+            return
+        if not await Backfill.get(source.mxid, self.thread_id, self.receiver):
+            await Backfill.new(
+                source.mxid,
+                priority,
+                self.thread_id,
+                self.receiver,
+                max_pages,
+                self.config["bridge.backfill.incremental.page_delay"],
+                self.config["bridge.backfill.incremental.post_batch_delay"],
+                max_total_pages,
+            ).insert()
 
-    async def _backfill(
-        self, source: u.User, thread: Thread, is_initial: bool, limit: int
-    ) -> None:
-        self.log.debug("Backfilling history through %s", source.mxid)
+    async def backfill(self, source: u.User, backfill_request: Backfill) -> None:
+        try:
+            last_message_ig_timestamp = await self._backfill(source, backfill_request)
+            if (
+                last_message_ig_timestamp is not None
+                and not self.bridge.homeserver_software.is_hungry
+                and self.config["bridge.backfill.msc2716"]
+            ):
+                await self.send_post_backfill_dummy(last_message_ig_timestamp)
+        finally:
+            # Always sleep after the backfill request is finished processing, even if it errors.
+            await asyncio.sleep(backfill_request.post_batch_delay)
+
+    async def _backfill(self, source: u.User, backfill_request: Backfill) -> int | None:
+        assert source.client
+        self.log.debug("Backfill request: %s", backfill_request)
+
+        num_pages = backfill_request.num_pages
+        self.log.debug(
+            "Backfilling up to %d pages of history in %s through %s",
+            num_pages,
+            self.mxid,
+            source.mxid,
+        )
 
-        entries = await self._fetch_backfill_items(source, thread, is_initial, limit)
-        if not entries:
-            self.log.debug("Didn't get any items to backfill from server")
-            return
-
-        self.log.debug("Got %d entries from server", len(entries))
-
-        self._backfill_leave = set()
-        async with NotificationDisabler(self.mxid, source):
-            for entry in reversed(entries):
-                sender = await p.Puppet.get_by_pk(int(entry.user_id))
-                await self.handle_instagram_item(source, sender, entry, is_backfill=True)
-        for intent in self._backfill_leave:
-            self.log.trace("Leaving room with %s post-backfill", intent.mxid)
-            await intent.leave_room(self.mxid)
-        self._backfill_leave = None
-        self.log.info("Backfilled %d messages through %s", len(entries), source.mxid)
-
-    async def _fetch_backfill_items(
-        self, source: u.User, thread: Thread, is_initial: bool, limit: int
-    ) -> list[ThreadItem]:
-        items = []
-        excluded_count = 0
-        self.log.debug("Fetching up to %d messages through %s", limit, source.igpk)
-        async for item in source.client.iter_thread(self.thread_id, start_at=thread):
-            if len(items) - excluded_count >= limit:
-                self.log.debug(f"Fetched {len(items)} messages (the limit)")
-                break
-            elif not is_initial:
-                msg = await DBMessage.get_by_item_id(item.item_id, receiver=self.receiver)
-                if msg is not None:
+        try:
+            if self.cursor:
+                self.log.debug(
+                    f"There is a cursor for the chat, fetching messages before {self.cursor}"
+                )
+                resp = await source.client.get_thread(
+                    self.thread_id, seq_id=source.seq_id, cursor=self.cursor
+                )
+            else:
+                self.log.debug(
+                    "There is no first message in the chat, starting with the most recent messages"
+                )
+                resp = await source.client.get_thread(self.thread_id, seq_id=source.seq_id)
+        except IGRateLimitError as e:
+            backoff = self.config.get("bridge.backfill.backoff.message_history", 300)
+            self.log.warning(
+                f"Backfilling failed due to rate limit. Waiting for {backoff} seconds before "
+                f"resuming. Error: {e}"
+            )
+            await asyncio.sleep(backoff)
+            raise
+
+        async def dedup_messages(messages: list[ThreadItem]) -> list[ThreadItem]:
+            deduped = []
+            # Sometimes (seems like on Facebook chats) it fetches the first message in the chat over
+            # and over again.
+            for item in messages:
+                # Check in-memory queues for duplicates
+                if item.item_id in self._msgid_dedup:
                     self.log.debug(
-                        f"Fetched {len(items)} messages and hit a message"
-                        " that's already in the database."
+                        f"Ignoring message {item.item_id} ({item.client_context}) by {item.user_id}"
+                        " as it was already handled (message.id in dedup queue)"
+                    )
+                    continue
+                self._msgid_dedup.appendleft(item.item_id)
+
+                # Check database for duplicates
+                if await DBMessage.get_by_item_id(item.item_id, self.receiver) is not None:
+                    self.log.debug(
+                        f"Ignoring message {item.item_id} ({item.client_context}) by {item.user_id}"
+                        " as it was already handled (message.id in database)"
+                    )
+                    continue
+
+                deduped.append(item)
+            return deduped
+
+        messages = await dedup_messages(resp.thread.items)
+        cursor = resp.thread.oldest_cursor
+        backfill_more = resp.thread.has_older
+        if len(messages) == 0:
+            self.log.debug("No messages to backfill.")
+            return None
+
+        last_message_timestamp = messages[-1].timestamp_ms
+
+        pages_to_backfill = backfill_request.num_pages
+        if backfill_request.max_total_pages > -1:
+            pages_to_backfill = min(pages_to_backfill, backfill_request.max_total_pages)
+
+        pages_backfilled = 0
+        for i in range(pages_to_backfill):
+            base_insertion_event_id = await self.backfill_message_page(
+                source, list(reversed(messages))
+            )
+            self.cursor = cursor
+            await self.save()
+            pages_backfilled += 1
+
+            if base_insertion_event_id:
+                self.historical_base_insertion_event_id = base_insertion_event_id
+                await self.save()
+
+            if backfill_more and i < pages_to_backfill - 1:
+                # Sleep before fetching another page of messages.
+                await asyncio.sleep(backfill_request.page_delay)
+
+                # Fetch more messages
+                try:
+                    resp = await source.client.get_thread(
+                        self.thread_id, seq_id=source.seq_id, cursor=self.cursor
+                    )
+                    messages = await dedup_messages(resp.thread.items)
+                    cursor = resp.thread.oldest_cursor
+                    backfill_more &= resp.thread.has_older
+                except IGRateLimitError as e:
+                    backoff = self.config.get("bridge.backfill.backoff.message_history", 300)
+                    self.log.warning(
+                        f"Backfilling failed due to rate limit. Waiting for {backoff} seconds "
+                        "before resuming."
                     )
+                    await asyncio.sleep(backoff)
+
+                    # If we hit the rate limit, then we will want to give up for now, but enqueue
+                    # additional backfill to do later.
                     break
-            elif not item.is_handleable:
-                self.log.debug(
-                    f"Not counting {item.unhandleable_type} item {item.item_id}"
-                    " against backfill limit"
+
+        if backfill_request.max_total_pages == -1:
+            new_max_total_pages = -1
+        else:
+            new_max_total_pages = backfill_request.max_total_pages - pages_backfilled
+            if new_max_total_pages <= 0:
+                backfill_more = False
+
+        if backfill_more:
+            self.log.debug("Enqueueing more backfill")
+            await Backfill.new(
+                source.mxid,
+                # Always enqueue subsequent backfills at the lowest priority
+                2,
+                self.thread_id,
+                self.receiver,
+                backfill_request.num_pages,
+                backfill_request.page_delay,
+                backfill_request.post_batch_delay,
+                new_max_total_pages,
+            ).insert()
+        else:
+            self.log.debug("No more messages to backfill")
+
+        await self._update_read_receipts(resp.thread.last_seen_at)
+        return last_message_timestamp
+
+    async def backfill_message_page(
+        self,
+        source: u.User,
+        message_page: list[ThreadItem],
+        forward: bool = False,
+        last_message: DBMessage | None = None,
+        mark_read: bool = False,
+    ) -> EventID | None:
+        """
+        Backfills a page of messages to Matrix. The messages should be in order from oldest to
+        newest.
+
+        Returns: a tuple containing the number of messages that were actually bridged, the
+            timestamp of the oldest bridged message and the base insertion event ID if it exists.
+        """
+        assert source.client
+        if len(message_page) == 0:
+            return None
+
+        if forward:
+            assert (last_message and last_message.mxid) or self.first_event_id
+            prev_event_id = last_message.mxid if last_message else self.first_event_id
+        else:
+            assert self.config["bridge.backfill.msc2716"]
+            assert self.first_event_id
+            prev_event_id = self.first_event_id
+
+        assert self.mxid
+
+        oldest_message_in_page = message_page[0]
+        oldest_msg_timestamp = oldest_message_in_page.timestamp_ms
+
+        batch_messages: list[BatchSendEvent] = []
+        state_events_at_start: list[BatchSendStateEvent] = []
+
+        added_members = set()
+        current_members = await self.main_intent.state_store.get_members(
+            self.mxid, memberships=(Membership.JOIN,)
+        )
+
+        def add_member(puppet: p.Puppet, mxid: UserID):
+            assert self.mxid
+            if mxid in added_members:
+                return
+            if (
+                self.bridge.homeserver_software.is_hungry
+                or not self.config["bridge.backfill.msc2716"]
+            ):
+                # Hungryserv doesn't expect or check state events at start.
+                added_members.add(mxid)
+                return
+
+            content_args = {"avatar_url": puppet.photo_mxc, "displayname": puppet.name}
+            state_events_at_start.extend(
+                [
+                    BatchSendStateEvent(
+                        content=MemberStateEventContent(Membership.INVITE, **content_args),
+                        type=EventType.ROOM_MEMBER,
+                        sender=self.main_intent.mxid,
+                        state_key=mxid,
+                        timestamp=oldest_msg_timestamp,
+                    ),
+                    BatchSendStateEvent(
+                        content=MemberStateEventContent(Membership.JOIN, **content_args),
+                        type=EventType.ROOM_MEMBER,
+                        sender=mxid,
+                        state_key=mxid,
+                        timestamp=oldest_msg_timestamp,
+                    ),
+                ]
+            )
+            added_members.add(mxid)
+
+        async def intent_for(user_id: int) -> tuple[p.Puppet, IntentAPI]:
+            puppet: p.Puppet = await p.Puppet.get_by_pk(user_id)
+            if puppet:
+                intent = puppet.intent_for(self)
+            else:
+                intent = self.main_intent
+            if puppet.is_real_user and not self._can_double_puppet_backfill(intent.mxid):
+                intent = puppet.default_mxid_intent
+            return puppet, intent
+
+        message_infos: list[tuple[ThreadItem | Reaction, int]] = []
+        intents: list[IntentAPI] = []
+
+        for message in message_page:
+            puppet, intent = await intent_for(message.user_id)
+
+            # Convert the message
+            converted = await self.convert_instagram_item(source, puppet, message)
+            if not converted:
+                self.log.debug(f"Skipping unsupported message in backfill {message.item_id}")
+                continue
+
+            if intent.mxid not in current_members:
+                add_member(puppet, intent.mxid)
+
+            d_event_id = None
+            for index, (event_type, content) in enumerate(converted):
+                if self.encrypted and self.matrix.e2ee:
+                    event_type, content = await self.matrix.e2ee.encrypt(
+                        self.mxid, event_type, content
+                    )
+                if intent.api.is_real_user and intent.api.bridge_name is not None:
+                    content[DOUBLE_PUPPET_SOURCE_KEY] = intent.api.bridge_name
+
+                if self.bridge.homeserver_software.is_hungry:
+                    d_event_id = self._deterministic_event_id(puppet, message.item_id, index)
+
+                message_infos.append((message, index))
+                batch_messages.append(
+                    BatchSendEvent(
+                        content=content,
+                        type=event_type,
+                        sender=intent.mxid,
+                        timestamp=message.timestamp_ms,
+                        event_id=d_event_id,
+                    )
+                )
+                intents.append(intent)
+
+            if self.bridge.homeserver_software.is_hungry and message.reactions:
+                for reaction in message.reactions.emojis:
+                    puppet, intent = await intent_for(reaction.sender_id)
+
+                    reaction_event = ReactionEventContent()
+                    reaction_event.relates_to = RelatesTo(
+                        rel_type=RelationType.ANNOTATION, event_id=d_event_id, key=reaction.emoji
+                    )
+                    if intent.api.is_real_user and intent.api.bridge_name is not None:
+                        reaction_event[DOUBLE_PUPPET_SOURCE_KEY] = intent.api.bridge_name
+
+                    message_infos.append((reaction, 0))
+                    batch_messages.append(
+                        BatchSendEvent(
+                            content=reaction_event,
+                            type=EventType.REACTION,
+                            sender=intent.mxid,
+                            timestamp=message.timestamp_ms,
+                        )
+                    )
+
+        if not batch_messages:
+            return None
+
+        if (
+            not self.bridge.homeserver_software.is_hungry
+            and self.config["bridge.backfill.msc2716"]
+            and (forward or self.next_batch_id is None)
+        ):
+            self.log.debug("Sending dummy event to avoid forward extremity errors")
+            await self.az.intent.send_message_event(
+                self.mxid, EventType("fi.mau.dummy.pre_backfill", EventType.Class.MESSAGE), {}
+            )
+
+        self.log.info(
+            "Sending %d %s messages to %s with batch ID %s and previous event ID %s",
+            len(batch_messages),
+            "new" if forward else "historical",
+            self.mxid,
+            self.next_batch_id,
+            prev_event_id,
+        )
+        if self.bridge.homeserver_software.is_hungry:
+            self.log.debug("Batch message event IDs %s", [m.event_id for m in batch_messages])
+
+        base_insertion_event_id = None
+        if self.config["bridge.backfill.msc2716"]:
+            batch_send_resp = await self.main_intent.batch_send(
+                self.mxid,
+                prev_event_id,
+                batch_id=self.next_batch_id,
+                events=batch_messages,
+                state_events_at_start=state_events_at_start,
+                beeper_new_messages=forward,
+                beeper_mark_read_by=source.mxid if mark_read else None,
+            )
+            base_insertion_event_id = batch_send_resp.base_insertion_event_id
+            event_ids = batch_send_resp.event_ids
+        else:
+            batch_send_resp = None
+            event_ids = [
+                await intent.send_message_event(
+                    self.mxid, evt.type, evt.content, timestamp=evt.timestamp
+                )
+                for evt, intent in zip(batch_messages, intents)
+            ]
+        await self._finish_batch(event_ids, message_infos)
+        if not forward:
+            assert batch_send_resp
+            self.log.debug("Got next batch ID %s for %s", batch_send_resp.next_batch_id, self.mxid)
+            self.next_batch_id = batch_send_resp.next_batch_id
+        await self.save()
+
+        return base_insertion_event_id
+
+    def _can_double_puppet_backfill(self, custom_mxid: UserID) -> bool:
+        return self.config["bridge.backfill.double_puppet_backfill"] and (
+            # Hungryserv can batch send any users
+            self.bridge.homeserver_software.is_hungry
+            # Non-MSC2716 backfill can use any double puppet
+            or not self.config["bridge.backfill.msc2716"]
+            # Local users can be double puppeted even with MSC2716
+            or (custom_mxid[custom_mxid.index(":") + 1 :] == self.config["homeserver.domain"])
+        )
+
+    async def _finish_batch(
+        self, event_ids: list[EventID], message_infos: list[tuple[ThreadItem | Reaction, int]]
+    ):
+        # We have to do this slightly annoying processing of the event IDs and message infos so
+        # that we only map the last event ID to the message.
+        # When inline captions are enabled, this will have no effect since index will always be 0
+        # since there's only ever one event per message.
+        current_message = None
+        messages = []
+        reactions = []
+        message_id = None
+        for event_id, (message_or_reaction, index) in zip(event_ids, message_infos):
+            if isinstance(message_or_reaction, ThreadItem):
+                message = message_or_reaction
+                if index == 0 and current_message:
+                    # This means that all of the events for the previous message have been processed,
+                    # and the current_message is the most recent event for that message.
+                    messages.append(current_message)
+
+                current_message = DBMessage(
+                    mxid=event_id,
+                    mx_room=self.mxid,
+                    item_id=message.item_id,
+                    client_context=message.client_context,
+                    receiver=self.receiver,
+                    sender=message.user_id,
+                    ig_timestamp=message.timestamp,
                 )
-                excluded_count += 1
-            items.append(item)
-        return items
+                message_id = message.item_id
+            else:
+                assert message_id
+                reaction = message_or_reaction
+                reactions.append(
+                    DBReaction(
+                        mxid=event_id,
+                        mx_room=self.mxid,
+                        ig_item_id=message_id,
+                        ig_receiver=self.receiver,
+                        ig_sender=reaction.sender_id,
+                        reaction=reaction.emoji,
+                        mx_timestamp=reaction.timestamp_ms,
+                    )
+                )
+
+        if current_message:
+            messages.append(current_message)
+
+        try:
+            await DBMessage.bulk_insert(messages)
+        except Exception:
+            self.log.exception("Failed to store batch message IDs")
+
+        try:
+            for reaction in reactions:
+                await reaction.insert()
+        except Exception:
+            self.log.exception("Failed to store backfilled reactions")
+
+    async def send_post_backfill_dummy(
+        self,
+        last_message_ig_timestamp: int,
+        base_insertion_event_id: EventID | None = None,
+    ):
+        if not self.config["bridge.backfill.msc2716"]:
+            return
+        assert self.mxid
+
+        if not base_insertion_event_id:
+            base_insertion_event_id = self.historical_base_insertion_event_id
+
+        if not base_insertion_event_id:
+            self.log.debug(
+                "No base insertion event ID in database or from batch send response. Not sending"
+                " dummy event."
+            )
+            return
+
+        event_id = await self.main_intent.send_message_event(
+            self.mxid,
+            event_type=HistorySyncMarkerMessage,
+            content={
+                "org.matrix.msc2716.marker.insertion": base_insertion_event_id,
+                "m.marker.insertion": base_insertion_event_id,
+            },
+        )
+        await DBMessage(
+            mxid=event_id,
+            mx_room=self.mxid,
+            item_id=f"fi.mau.instagram.post_backfill_dummy.{last_message_ig_timestamp}",
+            client_context=None,
+            receiver=self.receiver,
+            sender=0,
+            ig_timestamp=last_message_ig_timestamp,
+        ).insert()
 
     # endregion
     # region Bridge info state event
 
     @property
     def bridge_info_state_key(self) -> str:
         return f"net.maunium.instagram://instagram/{self.thread_id}"
@@ -1870,60 +2549,50 @@
         if self.mxid:
             try:
                 await self.update_matrix_room(source, info)
             except Exception:
                 self.log.exception("Failed to update portal")
             return self.mxid
         async with self._create_room_lock:
-            return await self._create_matrix_room(source, info)
+            try:
+                return await self._create_matrix_room(source, info)
+            except Exception:
+                self.log.exception("Failed to create portal")
+                return None
 
     def _get_invite_content(self, double_puppet: p.Puppet | None) -> dict[str, bool]:
         invite_content = {}
         if double_puppet:
             invite_content["fi.mau.will_auto_accept"] = True
         if self.is_direct:
             invite_content["is_direct"] = True
         return invite_content
 
-    async def update_matrix_room(
-        self, source: u.User, info: Thread, backfill: bool = False
-    ) -> None:
+    async def update_matrix_room(self, source: u.User, info: Thread) -> None:
         puppet = await p.Puppet.get_by_custom_mxid(source.mxid)
         await self.main_intent.invite_user(
             self.mxid,
             source.mxid,
             check_cache=True,
             extra_content=self._get_invite_content(puppet),
         )
         if puppet:
             did_join = await puppet.intent.ensure_joined(self.mxid)
             if did_join and self.is_direct:
                 await source.update_direct_chats({self.main_intent.mxid: [self.mxid]})
 
         await self.update_info(info, source)
-
-        if backfill:
-            last_msg = await DBMessage.get_by_item_id(
-                info.last_permanent_item.item_id, receiver=self.receiver
-            )
-            if last_msg is None:
-                self.log.debug(
-                    f"Last permanent item ({info.last_permanent_item.item_id})"
-                    " not found in database, starting backfilling"
-                )
-                await self.backfill(source, thread=info, is_initial=False)
         await self._update_read_receipts(info.last_seen_at)
 
     async def _create_matrix_room(self, source: u.User, info: Thread) -> RoomID | None:
         if self.mxid:
             await self.update_matrix_room(source, info)
             return self.mxid
         await self.update_info(info, source)
         self.log.debug("Creating Matrix room")
-        name: str | None = None
         initial_state = [
             {
                 "type": str(StateBridge),
                 "state_key": self.bridge_info_state_key,
                 "content": self.bridge_info,
             },
             # TODO remove this once https://github.com/matrix-org/matrix-doc/pull/2346 is in spec
@@ -1940,65 +2609,70 @@
                 {
                     "type": "m.room.encryption",
                     "content": self.get_encryption_state_event_json(),
                 }
             )
             if self.is_direct:
                 invites.append(self.az.bot_mxid)
-        if self.encrypted or self.private_chat_portal_meta or not self.is_direct:
-            name = self.name
-
-        # We lock backfill lock here so any messages that come between the room being created
-        # and the initial backfill finishing wouldn't be bridged before the backfill messages.
-        with self.backfill_lock:
-            creation_content = {}
-            if not self.config["bridge.federate_rooms"]:
-                creation_content["m.federate"] = False
-            self.mxid = await self.main_intent.create_room(
-                name=name,
-                is_direct=self.is_direct,
-                initial_state=initial_state,
-                invitees=invites,
-                creation_content=creation_content,
-            )
-            if not self.mxid:
-                raise Exception("Failed to create room: no mxid returned")
 
-            if self.encrypted and self.matrix.e2ee and self.is_direct:
-                try:
-                    await self.az.intent.ensure_joined(self.mxid)
-                except Exception:
-                    self.log.warning(f"Failed to add bridge bot to new private chat {self.mxid}")
+        if self.set_dm_room_metadata:
+            self.name_set = bool(self.name)
+            if self.avatar_url is not None:
+                initial_state.append(
+                    {
+                        "type": str(EventType.ROOM_AVATAR),
+                        "content": {"url": self.avatar_url},
+                    }
+                )
+                self.avatar_set = True
 
-            await self.update()
-            self.log.debug(f"Matrix room created: {self.mxid}")
-            self.by_mxid[self.mxid] = self
+        creation_content = {}
+        if not self.config["bridge.federate_rooms"]:
+            creation_content["m.federate"] = False
+        self.mxid = await self.main_intent.create_room(
+            name=self.name if self.set_dm_room_metadata else None,
+            is_direct=self.is_direct,
+            initial_state=initial_state,
+            invitees=invites,
+            creation_content=creation_content,
+        )
+        if not self.mxid:
+            raise Exception("Failed to create room: no mxid returned")
 
-            puppet = await p.Puppet.get_by_custom_mxid(source.mxid)
-            await self.main_intent.invite_user(
-                self.mxid, source.mxid, extra_content=self._get_invite_content(puppet)
-            )
-            if puppet:
-                try:
-                    if self.is_direct:
-                        await source.update_direct_chats({self.main_intent.mxid: [self.mxid]})
-                    await puppet.intent.join_room_by_id(self.mxid)
-                except MatrixError:
-                    self.log.debug(
-                        "Failed to join custom puppet into newly created portal", exc_info=True
-                    )
+        if self.encrypted and self.matrix.e2ee and self.is_direct:
+            try:
+                await self.az.intent.ensure_joined(self.mxid)
+            except Exception:
+                self.log.warning(f"Failed to add bridge bot to new private chat {self.mxid}")
 
-            await self._update_participants(info.users, source)
+        await self.update()
+        self.log.debug(f"Matrix room created: {self.mxid}")
+        self.by_mxid[self.mxid] = self
 
+        puppet = await p.Puppet.get_by_custom_mxid(source.mxid)
+        await self.main_intent.invite_user(
+            self.mxid, source.mxid, extra_content=self._get_invite_content(puppet)
+        )
+        if puppet:
             try:
-                await self.backfill(source, thread=info, is_initial=True)
-            except Exception:
-                self.log.exception("Failed to backfill new portal")
-            await self._update_read_receipts(info.last_seen_at)
+                if self.is_direct:
+                    await source.update_direct_chats({self.main_intent.mxid: [self.mxid]})
+                await puppet.intent.join_room_by_id(self.mxid)
+            except MatrixError:
+                self.log.debug(
+                    "Failed to join custom puppet into newly created portal", exc_info=True
+                )
 
+        await self._update_participants(info.users, source)
+
+        self.log.trace("Sending portal post-create dummy event")
+        self.first_event_id = await self.main_intent.send_message_event(
+            self.mxid, PortalCreateDummy, {}
+        )
+        await self.update()
         return self.mxid
 
     # endregion
     # region Database getters
 
     async def postinit(self) -> None:
         self.by_thread_id[(self.thread_id, self.receiver)] = self
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/puppet.py` & `mautrix-instagram-0.3.0/mautrix_instagram/puppet.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, AsyncGenerator, AsyncIterable, Awaitable, cast
+from typing import TYPE_CHECKING, Any, AsyncGenerator, AsyncIterable, Awaitable, cast
 import os.path
 
 from yarl import URL
 
 from mauigpapi.types import BaseResponseUser
 from mautrix.appservice import IntentAPI
 from mautrix.bridge import BasePuppet, async_getter_lock
@@ -36,56 +36,60 @@
 
 class Puppet(DBPuppet, BasePuppet):
     by_pk: dict[int, Puppet] = {}
     by_custom_mxid: dict[UserID, Puppet] = {}
     hs_domain: str
     mxid_template: SimpleTemplate[int]
 
+    bridge: InstagramBridge
     config: Config
 
     default_mxid_intent: IntentAPI
     default_mxid: UserID
 
     def __init__(
         self,
         pk: int,
         name: str | None = None,
         username: str | None = None,
         photo_id: str | None = None,
         photo_mxc: ContentURI | None = None,
         name_set: bool = False,
         avatar_set: bool = False,
+        contact_info_set: bool = False,
         is_registered: bool = False,
         custom_mxid: UserID | None = None,
         access_token: str | None = None,
         next_batch: SyncToken | None = None,
         base_url: URL | None = None,
     ) -> None:
         super().__init__(
             pk=pk,
             name=name,
             username=username,
             photo_id=photo_id,
             name_set=name_set,
             photo_mxc=photo_mxc,
             avatar_set=avatar_set,
+            contact_info_set=contact_info_set,
             is_registered=is_registered,
             custom_mxid=custom_mxid,
             access_token=access_token,
             next_batch=next_batch,
             base_url=base_url,
         )
         self.log = self.log.getChild(str(pk))
 
         self.default_mxid = self.get_mxid_from_id(pk)
         self.default_mxid_intent = self.az.intent.user(self.default_mxid)
         self.intent = self._fresh_intent()
 
     @classmethod
     def init_cls(cls, bridge: "InstagramBridge") -> AsyncIterable[Awaitable[None]]:
+        cls.bridge = bridge
         cls.config = bridge.config
         cls.loop = bridge.loop
         cls.mx = bridge.matrix
         cls.az = bridge.az
         cls.hs_domain = cls.config["homeserver.domain"]
         cls.mxid_template = SimpleTemplate(
             cls.config["bridge.username_template"],
@@ -121,19 +125,46 @@
             portal.other_user_pk != self.pk
             and (self.is_real_user or portal.is_direct)
             and self.config["bridge.backfill.invite_own_puppet"]
         )
 
     async def update_info(self, info: BaseResponseUser, source: u.User) -> None:
         update = False
+        if info.username and self.username != info.username:
+            self.username = info.username
+            update = True
+        update = await self.update_contact_info() or update
         update = await self._update_name(info) or update
         update = await self._update_avatar(info, source) or update
         if update:
             await self.update()
 
+    async def update_contact_info(self) -> bool:
+        if not self.bridge.homeserver_software.is_hungry:
+            return False
+
+        if self.contact_info_set:
+            return False
+
+        try:
+            contact_info: dict[str, Any] = {
+                "com.beeper.bridge.remote_id": str(self.igpk),
+                "com.beeper.bridge.service": self.bridge.beeper_service_name,
+                "com.beeper.bridge.network": self.bridge.beeper_network_name,
+            }
+            if self.username:
+                contact_info["com.beeper.bridge.identifiers"] = [f"instagram:{self.username}"]
+
+            await self.default_mxid_intent.beeper_update_profile(contact_info)
+            self.contact_info_set = True
+        except Exception:
+            self.log.exception("Error updating contact info")
+            self.contact_info_set = False
+        return True
+
     @classmethod
     def _get_displayname(cls, info: BaseResponseUser) -> str:
         return cls.config["bridge.displayname_template"].format(
             displayname=info.full_name or info.username, id=info.pk, username=info.username
         )
 
     async def _update_name(self, info: BaseResponseUser) -> bool:
@@ -156,17 +187,20 @@
             else os.path.basename(URL(info.profile_pic_url).path)
         )
         if pic_id != self.photo_id or not self.avatar_set:
             self.photo_id = pic_id
             if info.has_anonymous_profile_picture:
                 mxc = ""
             else:
-                async with source.client.raw_http_get(info.profile_pic_url) as resp:
-                    content_type = resp.headers["Content-Type"]
-                    resp_data = await resp.read()
+                resp = await source.client.proxy_with_retry(
+                    "Puppet._update_avatar",
+                    lambda: source.client.raw_http_get(info.profile_pic_url),
+                )
+                content_type = resp.headers["Content-Type"]
+                resp_data = await resp.read()
                 mxc = await self.default_mxid_intent.upload_media(
                     data=resp_data,
                     mime_type=content_type,
                     filename=pic_id,
                     async_upload=self.config["homeserver.async_media"],
                 )
             try:
@@ -244,15 +278,26 @@
 
         return None
 
     @classmethod
     async def all_with_custom_mxid(cls) -> AsyncGenerator[Puppet, None]:
         puppets = await super().all_with_custom_mxid()
         puppet: cls
-        for index, puppet in enumerate(puppets):
+        for puppet in puppets:
+            try:
+                yield cls.by_pk[puppet.pk]
+            except KeyError:
+                puppet._add_to_cache()
+                yield puppet
+
+    @classmethod
+    async def get_all(cls) -> AsyncGenerator[Puppet, None]:
+        puppets = await super().get_all()
+        puppet: cls
+        for puppet in puppets:
             try:
                 yield cls.by_pk[puppet.pk]
             except KeyError:
                 puppet._add_to_cache()
                 yield puppet
 
     # endregion
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/user.py` & `mautrix-instagram-0.3.0/mautrix_instagram/user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mautrix-instagram - A Matrix-Instagram puppeting bridge.
-# Copyright (C) 2022 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -11,33 +11,36 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, AsyncGenerator, AsyncIterable, Awaitable, cast
+from typing import TYPE_CHECKING, AsyncGenerator, AsyncIterable, Awaitable, Callable, cast
+from datetime import datetime, timedelta
+from functools import partial
 import asyncio
 import logging
 import time
 
-from aiohttp import ClientConnectionError
-
-from mauigpapi import AndroidAPI, AndroidMQTT, AndroidState, ProxyHandler
+from mauigpapi import AndroidAPI, AndroidMQTT, AndroidState
 from mauigpapi.errors import (
     IGChallengeError,
     IGCheckpointError,
     IGConsentRequiredError,
     IGNotLoggedInError,
     IGRateLimitError,
+    IGResponseError,
+    IGUnknownError,
     IGUserIDNotFoundError,
     IrisSubscribeError,
     MQTTConnectionUnauthorized,
     MQTTNotConnected,
     MQTTNotLoggedIn,
+    MQTTReconnectionError,
 )
 from mauigpapi.mqtt import (
     Connect,
     Disconnect,
     GraphQLSubscription,
     NewSequenceID,
     ProxyUpdate,
@@ -46,59 +49,55 @@
 from mauigpapi.types import (
     ActivityIndicatorData,
     CurrentUser,
     MessageSyncEvent,
     Operation,
     RealtimeDirectEvent,
     Thread,
+    ThreadRemoveEvent,
     ThreadSyncEvent,
     TypingStatus,
 )
+from mauigpapi.types.direct_inbox import DMInbox, DMInboxResponse
 from mautrix.appservice import AppService
 from mautrix.bridge import BaseUser, async_getter_lock
 from mautrix.types import EventID, MessageType, RoomID, TextMessageEventContent, UserID
+from mautrix.util import background_task
 from mautrix.util.bridge_state import BridgeState, BridgeStateEvent
 from mautrix.util.logging import TraceLogger
 from mautrix.util.opt_prometheus import Gauge, Summary, async_time
+from mautrix.util.proxy import RETRYABLE_PROXY_EXCEPTIONS, ProxyHandler
+from mautrix.util.simple_lock import SimpleLock
 
 from . import portal as po, puppet as pu
 from .config import Config
-from .db import Portal as DBPortal, User as DBUser
+from .db import Backfill, Message as DBMessage, Portal as DBPortal, User as DBUser
 
 if TYPE_CHECKING:
     from .__main__ import InstagramBridge
 
-try:
-    from aiohttp_socks import ProxyConnectionError, ProxyError, ProxyTimeoutError
-except ImportError:
-
-    class ProxyError(Exception):
-        pass
-
-    ProxyConnectionError = ProxyTimeoutError = ProxyError
 
 METRIC_MESSAGE = Summary("bridge_on_message", "calls to handle_message")
 METRIC_THREAD_SYNC = Summary("bridge_on_thread_sync", "calls to handle_thread_sync")
 METRIC_RTD = Summary("bridge_on_rtd", "calls to handle_rtd")
 METRIC_LOGGED_IN = Gauge("bridge_logged_in", "Users logged into the bridge")
 METRIC_CONNECTED = Gauge("bridge_connected", "Bridged users connected to Instagram")
 
 BridgeState.human_readable_errors.update(
     {
         "ig-connection-error": "Instagram disconnected unexpectedly",
         "ig-refresh-connection-error": "Reconnecting failed again after refresh: {message}",
         "ig-connection-fatal-error": "Instagram disconnected unexpectedly",
-        "ig-auth-error": "Authentication error from Instagram: {message}",
+        "ig-auth-error": "Authentication error from Instagram: {message}, please login again to continue",
         "ig-checkpoint": "Instagram checkpoint error. Please check the Instagram website.",
         "ig-consent-required": "Instagram requires a consent update. Please check the Instagram website.",
         "ig-checkpoint-locked": "Instagram checkpoint error. Please check the Instagram website.",
         "ig-rate-limit": "Got Instagram ratelimit error, waiting a few minutes before retrying...",
         "ig-disconnected": None,
-        "ig-no-mqtt": "You're not connected to Instagram",
-        "logged-out": "You're not logged into Instagram",
+        "logged-out": "You've been logged out of instagram, please login again to continue",
     }
 )
 
 
 class User(DBUser, BaseUser):
     ig_base_log: TraceLogger = logging.getLogger("mau.instagram")
     _activity_indicator_ids: dict[str, int] = {}
@@ -107,14 +106,17 @@
     config: Config
     az: AppService
     loop: asyncio.AbstractEventLoop
 
     client: AndroidAPI | None
     mqtt: AndroidMQTT | None
     _listen_task: asyncio.Task | None = None
+    _sync_lock: SimpleLock
+    _backfill_loop_task: asyncio.Task | None
+    _thread_sync_task: asyncio.Task | None
     _seq_id_save_task: asyncio.Task | None
 
     permission_level: str
     username: str | None
 
     _notice_room_lock: asyncio.Lock
     _notice_send_lock: asyncio.Lock
@@ -127,36 +129,48 @@
         self,
         mxid: UserID,
         igpk: int | None = None,
         state: AndroidState | None = None,
         notice_room: RoomID | None = None,
         seq_id: int | None = None,
         snapshot_at_ms: int | None = None,
+        oldest_cursor: str | None = None,
+        total_backfilled_portals: int | None = None,
+        thread_sync_completed: bool = False,
     ) -> None:
         super().__init__(
             mxid=mxid,
             igpk=igpk,
             state=state,
             notice_room=notice_room,
             seq_id=seq_id,
             snapshot_at_ms=snapshot_at_ms,
+            oldest_cursor=oldest_cursor,
+            total_backfilled_portals=total_backfilled_portals,
+            thread_sync_completed=thread_sync_completed,
         )
         BaseUser.__init__(self)
         self._notice_room_lock = asyncio.Lock()
         self._notice_send_lock = asyncio.Lock()
+        self.command_status = None
         perms = self.config.get_permissions(mxid)
         self.relay_whitelisted, self.is_whitelisted, self.is_admin, self.permission_level = perms
         self.client = None
         self.mqtt = None
         self.username = None
         self._is_logged_in = False
         self._is_connected = False
         self._is_refreshing = False
         self.shutdown = False
+        self._sync_lock = SimpleLock(
+            "Waiting for thread sync to finish before handling %s", log=self.log
+        )
         self._listen_task = None
+        self._thread_sync_task = None
+        self._backfill_loop_task = None
         self.remote_typing_status = None
         self._seq_id_save_task = None
 
         self.proxy_handler = ProxyHandler(
             api_url=self.config["bridge.get_proxy_api_url"],
         )
 
@@ -189,38 +203,66 @@
             thread = await self.client.create_group_thread([puppet.pk])
             portal = await po.Portal.get_by_thread(thread, self.igpk)
             await portal.update_info(thread, self)
             return portal
         return None
 
     async def try_connect(self) -> None:
-        try:
-            await self.connect()
-        except Exception as e:
-            self.log.exception("Error while connecting to Instagram")
-            await self.push_bridge_state(
-                BridgeStateEvent.UNKNOWN_ERROR, info={"python_error": str(e)}
-            )
+        while True:
+            try:
+                await self.connect()
+            except RETRYABLE_PROXY_EXCEPTIONS as e:
+                # These are retried by the client up to 10 times, but we actually want to retry
+                # these indefinitely so we capture them here again and retry.
+                self.log.warning(
+                    f"Proxy error connecting to Instagram: {e}, retrying in 1 minute",
+                )
+                await asyncio.sleep(60)
+                continue
+            except Exception as e:
+                self.log.exception("Error while connecting to Instagram")
+                await self.push_bridge_state(
+                    BridgeStateEvent.UNKNOWN_ERROR, info={"python_error": str(e)}
+                )
+            return
 
     @property
     def api_log(self) -> TraceLogger:
         return self.ig_base_log.getChild("http").getChild(self.mxid)
 
     @property
     def is_connected(self) -> bool:
         return bool(self.client) and bool(self.mqtt) and self._is_connected
 
+    async def ensure_connected(self, max_wait_seconds: int = 5) -> None:
+        sleep_interval = 0.1
+        max_attempts = max_wait_seconds / sleep_interval
+        attempts = 0
+        while True:
+            if self.is_connected:
+                return
+            attempts += 1
+            if attempts > max_attempts:
+                raise Exception("You're not connected to instagram")
+            await asyncio.sleep(sleep_interval)
+
     async def connect(self, user: CurrentUser | None = None) -> None:
         if not self.state:
-            await self.push_bridge_state(BridgeStateEvent.BAD_CREDENTIALS, error="logged-out")
+            await self.push_bridge_state(
+                BridgeStateEvent.BAD_CREDENTIALS,
+                error="logged-out",
+                info={"cnd_action": "reauth"},
+            )
             return
         client = AndroidAPI(
             self.state,
             log=self.api_log,
             proxy_handler=self.proxy_handler,
+            on_proxy_update=self.on_proxy_update,
+            on_response_error=self.on_response_error,
         )
 
         if not user:
             try:
                 resp = await client.current_user()
                 user = resp.user
             except IGNotLoggedInError as e:
@@ -239,35 +281,86 @@
         self.username = user.username
         await self.push_bridge_state(BridgeStateEvent.CONNECTING)
         self._track_metric(METRIC_LOGGED_IN, True)
         self.by_igpk[self.igpk] = self
 
         self.mqtt = AndroidMQTT(
             self.state,
-            loop=self.loop,
             log=self.ig_base_log.getChild("mqtt").getChild(self.mxid),
             proxy_handler=self.proxy_handler,
         )
         self.mqtt.add_event_handler(Connect, self.on_connect)
         self.mqtt.add_event_handler(Disconnect, self.on_disconnect)
         self.mqtt.add_event_handler(NewSequenceID, self.update_seq_id)
         self.mqtt.add_event_handler(MessageSyncEvent, self.handle_message)
         self.mqtt.add_event_handler(ThreadSyncEvent, self.handle_thread_sync)
+        self.mqtt.add_event_handler(ThreadRemoveEvent, self.handle_thread_remove)
         self.mqtt.add_event_handler(RealtimeDirectEvent, self.handle_rtd)
         self.mqtt.add_event_handler(ProxyUpdate, self.on_proxy_update)
 
         await self.update()
 
         self.loop.create_task(self._try_sync_puppet(user))
-        if not self.seq_id or self.config["bridge.resync_on_startup"]:
-            self.loop.create_task(self._try_sync())
+        self.loop.create_task(self._post_connect())
+
+    async def _post_connect(self):
+        # Backfill requests are handled synchronously so as not to overload the homeserver.
+        # Users can configure their backfill stages to be more or less aggressive with backfilling
+        # to try and avoid getting banned.
+        if not self._backfill_loop_task or self._backfill_loop_task.done():
+            self._backfill_loop_task = asyncio.create_task(self._handle_backfill_requests_loop())
+
+        if not self.seq_id:
+            await self._try_sync()
         else:
             self.log.debug("Connecting to MQTT directly as resync_on_startup is false")
             self.start_listen()
 
+        if self.config["bridge.backfill.enable"]:
+            if self._thread_sync_task and not self._thread_sync_task.done():
+                self.log.warning("Cancelling existing background thread sync task")
+                self._thread_sync_task.cancel()
+            self._thread_sync_task = asyncio.create_task(self.backfill_threads())
+
+        if self.bridge.homeserver_software.is_hungry:
+            self.log.info("Updating contact info for all users")
+            asyncio.gather(*[puppet.update_contact_info() async for puppet in pu.Puppet.get_all()])
+
+    async def _handle_backfill_requests_loop(self) -> None:
+        if not self.config["bridge.backfill.enable"] or not self.config["bridge.backfill.msc2716"]:
+            return
+
+        while True:
+            await self._sync_lock.wait("backfill request")
+            req = await Backfill.get_next(self.mxid)
+            if not req:
+                await asyncio.sleep(30)
+                continue
+            self.log.info("Backfill request %s", req)
+            try:
+                portal = await po.Portal.get_by_thread_id(
+                    req.portal_thread_id, receiver=req.portal_receiver
+                )
+                await req.mark_dispatched()
+                await portal.backfill(self, req)
+                await req.mark_done()
+            except IGNotLoggedInError as e:
+                self.log.exception("User got logged out during backfill loop")
+                break
+            except (IGChallengeError, IGConsentRequiredError) as e:
+                self.log.exception("User got a challenge during backfill loop")
+                await self._handle_checkpoint(e, on="backfill")
+                break
+            except Exception as e:
+                self.log.exception("Failed to backfill portal %s: %s", req.portal_thread_id, e)
+
+                # Don't try again to backfill this portal for a minute.
+                await req.set_cooldown_timeout(60)
+        self._backfill_loop_task = None
+
     async def on_connect(self, evt: Connect) -> None:
         self.log.debug("Connected to Instagram")
         self._track_metric(METRIC_CONNECTED, True)
         self._is_connected = True
         await self.send_bridge_notice("Connected to Instagram")
         await self.push_bridge_state(BridgeStateEvent.CONNECTED)
 
@@ -275,14 +368,23 @@
         self.log.debug("Disconnected from Instagram")
         self._track_metric(METRIC_CONNECTED, False)
         self._is_connected = False
 
     async def on_proxy_update(self, evt: ProxyUpdate | None = None) -> None:
         if self.client:
             self.client.setup_http(self.state.cookies.jar)
+        if self.mqtt:
+            self.mqtt.setup_proxy()
+        if self.command_status:
+            self.command_status["api"].setup_http(self.command_status["state"].cookies.jar)
+
+    async def on_response_error(self, err: IGResponseError) -> None:
+        if isinstance(err, IGNotLoggedInError) and (await self.is_logged_in()):
+            self.log.warning(f"Noticed logout in API error response: {err}")
+            await self.logout(error=err)
 
     # TODO this stuff could probably be moved to mautrix-python
     async def get_notice_room(self) -> RoomID:
         if not self.notice_room:
             async with self._notice_room_lock:
                 # If someone already created the room while this call was waiting,
                 # don't make a new room
@@ -359,23 +461,23 @@
         except Exception:
             self.log.warning("Failed to send bridge notice", exc_info=True)
         return edit or event_id
 
     async def _try_sync_puppet(self, user_info: CurrentUser) -> None:
         puppet = await pu.Puppet.get_by_pk(self.igpk)
         try:
-            await puppet.update_info(user_info, self)
-        except Exception:
-            self.log.exception("Failed to update own puppet info")
-        try:
             if puppet.custom_mxid != self.mxid and puppet.can_auto_login(self.mxid):
-                self.log.info(f"Automatically enabling custom puppet")
+                self.log.info("Automatically enabling custom puppet")
                 await puppet.switch_mxid(access_token="auto", mxid=self.mxid)
         except Exception:
             self.log.exception("Failed to automatically enable custom puppet")
+        try:
+            await puppet.update_info(user_info, self)
+        except Exception:
+            self.log.exception("Failed to update own puppet info")
 
     async def _try_sync(self) -> None:
         try:
             await self.sync()
         except Exception as e:
             self.log.exception("Exception while syncing")
             if isinstance(e, IGCheckpointError):
@@ -387,18 +489,21 @@
     async def get_direct_chats(self) -> dict[UserID, list[RoomID]]:
         return {
             pu.Puppet.get_mxid_from_id(portal.other_user_pk): [portal.mxid]
             for portal in await DBPortal.find_private_chats_of(self.igpk)
             if portal.mxid
         }
 
-    async def refresh(self, resync: bool = True) -> None:
+    async def refresh(self, resync: bool = True, update_proxy: bool = False) -> None:
         self._is_refreshing = True
         try:
             await self.stop_listen()
+            self.state.reset_pigeon_session_id()
+            if update_proxy and self.proxy_handler.update_proxy_url(reason="reconnect"):
+                await self.on_proxy_update()
             if resync:
                 retry_count = 0
                 minutes = 1
                 while True:
                     try:
                         await self.sync()
                         return
@@ -419,15 +524,14 @@
                             info={"python_error": str(e)},
                         )
                         await asyncio.sleep(minutes * 60)
             else:
                 self.start_listen()
         finally:
             self._is_refreshing = False
-            self.proxy_handler.update_proxy_url()
 
     async def _handle_checkpoint(
         self,
         e: IGChallengeError | IGConsentRequiredError,
         on: str,
         client: AndroidAPI | None = None,
     ) -> None:
@@ -460,57 +564,132 @@
             if resp.challenge_context.challenge_type_enum == "HACKED_LOCK":
                 error_code = "ig-checkpoint-locked"
         except Exception:
             self.log.exception("Error resetting challenge state")
             info = {"challenge": e.body.challenge.serialize() if e.body.challenge else None}
         await self.push_bridge_state(BridgeStateEvent.BAD_CREDENTIALS, error=error_code, info=info)
 
-    async def _sync_thread(self, thread: Thread, allow_create: bool) -> None:
-        portal = await po.Portal.get_by_thread(thread, self.igpk)
-        if portal.mxid:
-            self.log.debug(f"{thread.thread_id} has a portal, syncing and backfilling...")
-            await portal.update_matrix_room(self, thread, backfill=True)
-        elif allow_create:
-            self.log.debug(f"{thread.thread_id} has been active recently, creating portal...")
-            await portal.create_matrix_room(self, thread)
+    async def _sync_thread(
+        self, thread: Thread, enqueue_backfill: bool = True, portal: po.Portal | None = None
+    ) -> bool:
+        """
+        Sync a specific thread. Returns whether the thread had messages after the last message in
+        the database before the sync.
+        """
+        self.log.debug(f"Syncing thread {thread.thread_id}")
+
+        forward_messages = thread.items
+
+        assert self.client
+        if not portal:
+            portal = await po.Portal.get_by_thread(thread, self.igpk)
+            assert portal
         else:
-            self.log.debug(f"{thread.thread_id} is not active and doesn't have a portal")
+            assert portal.thread_id == thread.thread_id
 
-    async def _maybe_update_proxy(self, source: str) -> None:
-        if not self._listen_task:
-            self.proxy_handler.update_proxy_url()
-            await self.on_proxy_update()
+        # Create or update the Matrix room
+        if not portal.mxid:
+            await portal.create_matrix_room(self, thread)
         else:
-            self.log.debug(f"Not updating proxy: listen_task is still running? (caller: {source})")
+            await portal.update_matrix_room(self, thread)
+
+        if not self.config["bridge.backfill.enable_initial"]:
+            return True
+
+        last_message = await DBMessage.get_last(portal.mxid)
+        cursor = thread.oldest_cursor
+        if last_message:
+            original_number_of_messages = len(thread.items)
+            new_messages = [
+                m for m in thread.items if last_message.ig_timestamp_ms < m.timestamp_ms
+            ]
+            forward_messages = new_messages
+
+            portal.log.debug(
+                f"{len(new_messages)}/{original_number_of_messages} messages are after most recent"
+                " message."
+            )
+
+            # Fetch more messages until we get back to messages that have been bridged already.
+            while len(new_messages) > 0 and len(new_messages) == original_number_of_messages:
+                await asyncio.sleep(self.config["bridge.backfill.incremental.page_delay"])
+
+                portal.log.debug("Fetching more messages for forward backfill")
+                resp = await self.client.get_thread(portal.thread_id, cursor=cursor)
+                if len(resp.thread.items) == 0:
+                    break
+                original_number_of_messages = len(resp.thread.items)
+                new_messages = [
+                    m for m in resp.thread.items if last_message.ig_timestamp_ms < m.timestamp_ms
+                ]
+                forward_messages = new_messages + forward_messages
+                cursor = resp.thread.oldest_cursor
+                portal.log.debug(
+                    f"{len(new_messages)}/{original_number_of_messages} messages are after most "
+                    "recent message."
+                )
+        elif not portal.first_event_id:
+            self.log.debug(
+                f"Skipping backfilling {portal.thread_id} as the first event ID is not known"
+            )
+            return False
+
+        if forward_messages:
+            portal.cursor = cursor
+            await portal.update()
+
+            mark_read = thread.read_state == 0 or (
+                (hours := self.config["bridge.backfill.unread_hours_threshold"]) > 0
+                and (
+                    datetime.fromtimestamp(forward_messages[0].timestamp_ms / 1000)
+                    < datetime.now() - timedelta(hours=hours)
+                )
+            )
+            base_insertion_event_id = await portal.backfill_message_page(
+                self,
+                list(reversed(forward_messages)),
+                forward=True,
+                last_message=last_message,
+                mark_read=mark_read,
+            )
+            if (
+                not self.bridge.homeserver_software.is_hungry
+                and self.config["bridge.backfill.msc2716"]
+            ):
+                await portal.send_post_backfill_dummy(
+                    forward_messages[0].timestamp, base_insertion_event_id=base_insertion_event_id
+                )
+            if (
+                mark_read
+                and not self.bridge.homeserver_software.is_hungry
+                and (puppet := await self.get_puppet())
+            ):
+                last_message = await DBMessage.get_last(portal.mxid)
+                if last_message:
+                    await puppet.intent_for(portal).mark_read(portal.mxid, last_message.mxid)
+
+            await portal._update_read_receipts(thread.last_seen_at)
+
+        if self.config["bridge.backfill.msc2716"] and enqueue_backfill:
+            await portal.enqueue_immediate_backfill(self, 1)
+        return len(forward_messages) > 0
+
+    async def sync(self, increment_total_backfilled_portals: bool = False) -> None:
+        await self.run_with_sync_lock(partial(self._sync, increment_total_backfilled_portals))
 
-    async def sync(self) -> None:
+    async def _sync(self, increment_total_backfilled_portals: bool = False) -> None:
+        if not self._listen_task:
+            self.state.reset_pigeon_session_id()
         sleep_minutes = 2
-        errors = 0
         while True:
             try:
                 resp = await self.client.get_inbox()
                 break
-            except (
-                ProxyError,
-                ProxyTimeoutError,
-                ProxyConnectionError,
-                ClientConnectionError,
-                ConnectionError,
-                asyncio.TimeoutError,
-            ) as e:
-                errors += 1
-                wait = min(errors * 10, 60)
-                self.log.warning(
-                    f"{e.__class__.__name__} while trying to sync, retrying in {wait} seconds: {e}"
-                )
-                await asyncio.sleep(wait)
-                await self._maybe_update_proxy("sync error")
             except IGNotLoggedInError as e:
                 self.log.exception("Got not logged in error while syncing")
-                await self.logout(error=e)
                 return
             except IGRateLimitError as e:
                 self.log.error(
                     "Got ratelimit error while trying to get inbox (%s), retrying in %d minutes",
                     e.body,
                     sleep_minutes,
                 )
@@ -529,72 +708,211 @@
         self.seq_id = resp.seq_id
         self.snapshot_at_ms = resp.snapshot_at_ms
         await self.save_seq_id()
 
         if not self._listen_task:
             self.start_listen(is_after_sync=True)
 
-        max_age = self.config["bridge.portal_create_max_age"] * 1_000_000
-        limit = self.config["bridge.chat_sync_limit"]
-        create_limit = self.config["bridge.chat_create_limit"]
-        min_active_at = (time.time() * 1_000_000) - max_age
-        i = 0
-        await self.push_bridge_state(BridgeStateEvent.BACKFILLING)
-        async for thread in self.client.iter_inbox(start_at=resp):
-            try:
-                await self._sync_thread(
-                    thread=thread,
-                    allow_create=thread.last_activity_at > min_active_at and i < create_limit,
-                )
-            except Exception:
-                self.log.exception(f"Error syncing thread {thread.thread_id}")
-            i += 1
-            if i >= limit:
-                break
+        sync_count = min(
+            self.config["bridge.backfill.max_conversations"],
+            self.config["bridge.max_startup_thread_sync_count"],
+        )
+        self.log.debug(f"Fetching {sync_count} threads, 20 at a time...")
+
+        local_limit: int | None = sync_count
+        if sync_count == 0:
+            return
+        elif sync_count < 0:
+            local_limit = None
+
+        await self._sync_threads_with_delay(
+            self.client.iter_inbox(
+                self._update_seq_id_and_cursor, start_at=resp, local_limit=local_limit
+            ),
+            stop_when_threads_have_no_messages_to_backfill=True,
+            increment_total_backfilled_portals=increment_total_backfilled_portals,
+            local_limit=local_limit,
+        )
+
         try:
             await self.update_direct_chats()
         except Exception:
             self.log.exception("Error updating direct chat list")
 
+    async def backfill_threads(self):
+        try:
+            await self.run_with_sync_lock(self._backfill_threads)
+        except Exception:
+            self.log.exception("Error in thread backfill loop")
+
+    async def _backfill_threads(self):
+        assert self.client
+        if not self.config["bridge.backfill.enable"]:
+            return
+
+        max_conversations = self.config["bridge.backfill.max_conversations"] or 0
+        if 0 <= max_conversations <= (self.total_backfilled_portals or 0):
+            self.log.info("Backfill max_conversations count reached, not syncing any more portals")
+            return
+        elif self.thread_sync_completed:
+            self.log.debug("Thread backfill is marked as completed, not syncing more portals")
+            return
+        local_limit = (
+            max_conversations - (self.total_backfilled_portals or 0)
+            if max_conversations >= 0
+            else None
+        )
+
+        start_at = None
+        if self.oldest_cursor:
+            start_at = DMInboxResponse(
+                status="",
+                seq_id=self.seq_id,
+                snapshot_at_ms=0,
+                pending_requests_total=0,
+                has_pending_top_requests=False,
+                viewer=None,
+                inbox=DMInbox(
+                    threads=[],
+                    has_older=True,
+                    unseen_count=0,
+                    unseen_count_ts=0,
+                    blended_inbox_enabled=False,
+                    oldest_cursor=self.oldest_cursor,
+                ),
+            )
+        backoff = self.config.get("bridge.backfill.backoff.thread_list", 300)
+        await self._sync_threads_with_delay(
+            self.client.iter_inbox(
+                self._update_seq_id_and_cursor,
+                start_at=start_at,
+                local_limit=local_limit,
+                rate_limit_exceeded_backoff=backoff,
+            ),
+            increment_total_backfilled_portals=True,
+            local_limit=local_limit,
+        )
+        await self.update_direct_chats()
+
+    def _update_seq_id_and_cursor(self, seq_id: int, cursor: str | None):
+        self.seq_id = seq_id
+        if cursor:
+            self.oldest_cursor = cursor
+
+    async def _sync_threads_with_delay(
+        self,
+        threads: AsyncIterable[Thread],
+        increment_total_backfilled_portals: bool = False,
+        stop_when_threads_have_no_messages_to_backfill: bool = False,
+        local_limit: int | None = None,
+    ):
+        sync_delay = self.config["bridge.backfill.min_sync_thread_delay"]
+        last_thread_sync_ts = 0.0
+        found_thread_count = 0
+        async for thread in threads:
+            found_thread_count += 1
+            now = time.monotonic()
+            if now < last_thread_sync_ts + sync_delay:
+                delay = last_thread_sync_ts + sync_delay - now
+                self.log.debug("Thread sync is happening too quickly. Waiting for %ds", delay)
+                await asyncio.sleep(delay)
+
+            last_thread_sync_ts = time.monotonic()
+            had_new_messages = await self._sync_thread(thread)
+            if not had_new_messages and stop_when_threads_have_no_messages_to_backfill:
+                self.log.debug("Got to threads with no new messages. Stopping sync.")
+                return
+
+            if increment_total_backfilled_portals:
+                self.total_backfilled_portals = (self.total_backfilled_portals or 0) + 1
+            await self.update()
+        if local_limit is None or found_thread_count < local_limit:
+            if local_limit is None:
+                self.log.info(
+                    "Reached end of thread list with no limit, marking thread sync as completed"
+                )
+            else:
+                self.log.info(
+                    f"Reached end of thread list (got {found_thread_count} with "
+                    f"limit {local_limit}), marking thread sync as completed"
+                )
+            self.thread_sync_completed = True
+        await self.update()
+
+    async def run_with_sync_lock(self, func: Callable[[], Awaitable]):
+        with self._sync_lock:
+            retry_count = 0
+            while retry_count < 5:
+                try:
+                    retry_count += 1
+                    await func()
+
+                    # The sync was successful. Exit the loop.
+                    return
+                except IGNotLoggedInError as e:
+                    return
+                except Exception:
+                    self.log.exception(
+                        "Failed to sync threads. Waiting 30 seconds before retrying sync."
+                    )
+                    await asyncio.sleep(30)
+
+            # If we get here, it means that the sync has failed five times. If this happens, most
+            # likely something very bad has happened.
+            self.log.error("Failed to sync threads five times. Will not retry.")
+
     def start_listen(self, is_after_sync: bool = False) -> None:
         self.shutdown = False
         task = self._listen(
             seq_id=self.seq_id, snapshot_at_ms=self.snapshot_at_ms, is_after_sync=is_after_sync
         )
         self._listen_task = self.loop.create_task(task)
 
-    async def fetch_user_and_reconnect(self) -> None:
+    async def delayed_start_listen(self, sleep: int) -> None:
+        await asyncio.sleep(sleep)
+        if self.is_connected:
+            self.log.debug(
+                "Already reconnected before delay after MQTT reconnection error finished"
+            )
+        else:
+            self.log.debug("Reconnecting after MQTT connection error")
+            self.start_listen()
+
+    async def fetch_user_and_reconnect(self, sleep_first: int | None = None) -> None:
+        if sleep_first:
+            await asyncio.sleep(sleep_first)
+            if self.is_connected:
+                self.log.debug("Canceling user fetch, already reconnected")
+                return
         self.log.debug("Refetching current user after disconnection")
         errors = 0
         while True:
             try:
                 resp = await self.client.current_user()
-            except (
-                ProxyError,
-                ProxyTimeoutError,
-                ProxyConnectionError,
-                ClientConnectionError,
-                ConnectionError,
-                asyncio.TimeoutError,
-            ) as e:
-                errors += 1
-                wait = min(errors * 10, 60)
+            except RETRYABLE_PROXY_EXCEPTIONS as e:
+                # These are retried by the client up to 10 times, but we actually want to retry
+                # these indefinitely so we capture them here again and retry.
                 self.log.warning(
-                    f"{e.__class__.__name__} while trying to check user for reconnection, "
-                    f"retrying in {wait} seconds: {e}"
+                    f"Proxy error fetching user from Instagram: {e}, retrying in 1 minute",
                 )
-                await asyncio.sleep(wait)
-                await self._maybe_update_proxy("fetch_user_and_reconnect error")
+                await asyncio.sleep(60)
             except IGNotLoggedInError as e:
                 self.log.warning(f"Failed to reconnect to Instagram: {e}, logging out")
-                await self.logout(error=e)
                 return
             except (IGChallengeError, IGConsentRequiredError) as e:
                 await self._handle_checkpoint(e, on="reconnect")
                 return
+            except IGUnknownError:
+                errors += 1
+                if errors > 10:
+                    raise
+                self.log.warning(
+                    "Non-JSON body while trying to check user for reconnection, retrying in 10s"
+                )
+                await asyncio.sleep(10)
             except Exception as e:
                 self.log.exception("Error while reconnecting to Instagram")
                 if isinstance(e, IGCheckpointError):
                     self.log.debug("Checkpoint error content: %s", e.body)
                 await self.push_bridge_state(
                     BridgeStateEvent.UNKNOWN_ERROR, info={"python_error": str(e)}
                 )
@@ -628,37 +946,48 @@
                     state_event=BridgeStateEvent.UNKNOWN_ERROR,
                     error_code="ig-refresh-connection-error",
                     error_message=str(e),
                     info={"python_error": str(e)},
                 )
             else:
                 self.log.warning(f"Got IrisSubscribeError {e}, refreshing...")
-                asyncio.create_task(self.refresh())
-        except (MQTTNotConnected, MQTTNotLoggedIn, MQTTConnectionUnauthorized) as e:
+                background_task.create(self.refresh())
+        except MQTTReconnectionError as e:
             self.log.warning(
-                f"Unexpected connection error: {e}", exc_info="MQTT reconnection failed" in str(e)
+                f"Unexpected connection error: {e}, reconnecting in 1 minute", exc_info=True
             )
             await self.send_bridge_notice(
                 f"Error in listener: {e}",
                 important=True,
-                state_event=BridgeStateEvent.UNKNOWN_ERROR,
-                error_code="ig-connection-error",
+                state_event=BridgeStateEvent.TRANSIENT_DISCONNECT,
+                error_code="ig-connection-error-socket",
             )
             self.mqtt.disconnect()
-            asyncio.create_task(self.fetch_user_and_reconnect())
+            background_task.create(self.delayed_start_listen(sleep=60))
+        except (MQTTNotConnected, MQTTNotLoggedIn, MQTTConnectionUnauthorized) as e:
+            self.log.warning(f"Unexpected connection error: {e}, checking auth and reconnecting")
+            await self.send_bridge_notice(
+                f"Error in listener: {e}",
+                important=True,
+                state_event=BridgeStateEvent.TRANSIENT_DISCONNECT,
+                error_code="ig-connection-error-maybe-auth",
+            )
+            self.mqtt.disconnect()
+            background_task.create(self.fetch_user_and_reconnect())
         except Exception as e:
-            self.log.exception("Fatal error in listener")
+            self.log.exception("Fatal error in listener, reconnecting in 5 minutes")
             await self.send_bridge_notice(
                 "Fatal error in listener (see logs for more info)",
                 state_event=BridgeStateEvent.UNKNOWN_ERROR,
                 important=True,
                 error_code="ig-unknown-connection-error",
                 info={"python_error": str(e)},
             )
             self.mqtt.disconnect()
+            background_task.create(self.fetch_user_and_reconnect(sleep_first=300))
         else:
             if not self.shutdown:
                 await self.send_bridge_notice(
                     "Instagram connection closed without error",
                     state_event=BridgeStateEvent.UNKNOWN_ERROR,
                     error_code="ig-disconnected",
                 )
@@ -674,15 +1003,25 @@
             if self._listen_task:
                 await self._listen_task
             self.shutdown = False
         self._track_metric(METRIC_CONNECTED, False)
         self._is_connected = False
         await self.update()
 
+    def stop_backfill_tasks(self) -> None:
+        if self._backfill_loop_task:
+            self._backfill_loop_task.cancel()
+            self._backfill_loop_task = None
+        if self._thread_sync_task:
+            self._thread_sync_task.cancel()
+            self._thread_sync_task = None
+
     async def logout(self, error: IGNotLoggedInError | None = None) -> None:
+        await self.stop_listen()
+        self.stop_backfill_tasks()
         if self.client and error is None:
             try:
                 await self.client.logout(one_tap_app_login=False)
             except Exception:
                 self.log.debug("Exception logging out", exc_info=True)
         if self.mqtt:
             self.mqtt.disconnect()
@@ -702,28 +1041,35 @@
             self.log.debug("Auth error body: %s", error.body.serialize())
             await self.send_bridge_notice(
                 f"You have been logged out of Instagram: {error.proper_message}",
                 important=True,
                 state_event=BridgeStateEvent.BAD_CREDENTIALS,
                 error_code="ig-auth-error",
                 error_message=error.proper_message,
+                info={"cnd_action": "reauth"},
             )
         self.client = None
         self.mqtt = None
         self.state = None
         self.seq_id = None
+        if self._seq_id_save_task and not self._seq_id_save_task.done():
+            self._seq_id_save_task.cancel()
+            self._seq_id_save_task = None
         self.snapshot_at_ms = None
+        self.thread_sync_completed = False
         self._is_logged_in = False
         await self.update()
 
     # endregion
     # region Event handlers
 
     async def _save_seq_id_after_sleep(self) -> None:
         await asyncio.sleep(120)
+        if self.seq_id is None:
+            return
         self._seq_id_save_task = None
         self.log.trace("Saving sequence ID %d/%d", self.seq_id, self.snapshot_at_ms)
         try:
             await self.save_seq_id()
         except Exception:
             self.log.exception("Error saving sequence ID")
 
@@ -736,34 +1082,36 @@
         else:
             self.log.trace("Not starting seq id save task (%d/%d)", evt.seq_id, evt.snapshot_at_ms)
 
     @async_time(METRIC_MESSAGE)
     async def handle_message(self, evt: MessageSyncEvent) -> None:
         portal = await po.Portal.get_by_thread_id(evt.message.thread_id, receiver=self.igpk)
         if not portal or not portal.mxid:
-            self.log.debug("Got message in thread with no portal, getting info...")
+            self.log.debug(
+                "Got message in thread with no portal, getting info and syncing thread..."
+            )
             resp = await self.client.get_thread(evt.message.thread_id)
             portal = await po.Portal.get_by_thread(resp.thread, self.igpk)
-            self.log.debug("Got info for unknown portal, creating room")
-            await portal.create_matrix_room(self, resp.thread)
+            await self._sync_thread(resp.thread, enqueue_backfill=False, portal=portal)
             if not portal.mxid:
                 self.log.warning(
                     "Room creation appears to have failed, "
                     f"dropping message in {evt.message.thread_id}"
                 )
                 return
         self.log.trace(f"Received message sync event {evt.message}")
-        await portal.backfill_lock.wait(f"{evt.message.op} {evt.message.item_id}")
         if evt.message.new_reaction:
             await portal.handle_instagram_reaction(
                 evt.message, remove=evt.message.op == Operation.REMOVE
             )
             return
         sender = await pu.Puppet.get_by_pk(evt.message.user_id) if evt.message.user_id else None
-        if evt.message.op == Operation.ADD:
+        if evt.message.is_thread_image:
+            await portal.update_thread_image(self, evt.message.thread_image, sender=sender)
+        elif evt.message.op == Operation.ADD:
             if not sender:
                 # I don't think we care about adds with no sender
                 return
             await portal.handle_instagram_item(self, sender, evt.message)
         elif evt.message.op == Operation.REMOVE:
             # Removes don't have a sender, only the message sender can unsend messages anyway
             await portal.handle_instagram_remove(evt.message.item_id)
@@ -772,26 +1120,29 @@
 
     @async_time(METRIC_THREAD_SYNC)
     async def handle_thread_sync(self, evt: ThreadSyncEvent) -> None:
         self.log.trace("Thread sync event content: %s", evt)
         portal = await po.Portal.get_by_thread(evt, receiver=self.igpk)
         if portal.mxid:
             self.log.debug("Got thread sync event for %s with existing portal", portal.thread_id)
-            await portal.update_matrix_room(self, evt)
         elif evt.is_group:
             self.log.debug(
                 "Got thread sync event for group %s without existing portal, creating room",
                 portal.thread_id,
             )
-            await portal.create_matrix_room(self, evt)
         else:
             self.log.debug(
                 "Got thread sync event for DM %s without existing portal, ignoring",
                 portal.thread_id,
             )
+            return
+        await self._sync_thread(evt, enqueue_backfill=False, portal=portal)
+
+    async def handle_thread_remove(self, evt: ThreadRemoveEvent) -> None:
+        self.log.debug("Got thread remove event: %s", evt.serialize())
 
     @async_time(METRIC_RTD)
     async def handle_rtd(self, evt: RealtimeDirectEvent) -> None:
         if not isinstance(evt.value, ActivityIndicatorData):
             return
 
         now = int(time.time() * 1000)
@@ -809,17 +1160,15 @@
         portal = await po.Portal.get_by_thread_id(evt.thread_id, receiver=self.igpk)
         if not puppet or not portal or not portal.mxid:
             return
 
         is_typing = evt.value.activity_status != TypingStatus.OFF
         if puppet.pk == self.igpk:
             self.remote_typing_status = TypingStatus.TEXT if is_typing else TypingStatus.OFF
-        await puppet.intent_for(portal).set_typing(
-            portal.mxid, is_typing=is_typing, timeout=evt.value.ttl
-        )
+        await puppet.intent_for(portal).set_typing(portal.mxid, timeout=evt.value.ttl)
 
     # endregion
     # region Database getters
 
     def _add_to_cache(self) -> None:
         self.by_mxid[self.mxid] = self
         if self.igpk:
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/util/color_log.py` & `mautrix-instagram-0.3.0/mautrix_instagram/util/color_log.py`

 * *Files identical despite different names*

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/web/provisioning_api.py` & `mautrix-instagram-0.3.0/mautrix_instagram/web/provisioning_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,41 +34,48 @@
     IGChallengeWrongCodeError,
     IGCheckpointError,
     IGConsentRequiredError,
     IGFBEmailTaken,
     IGFBNoContactPointFoundError,
     IGFBSSODisabled,
     IGLoginBadPasswordError,
+    IGLoginInvalidCredentialsError,
     IGLoginInvalidUserError,
     IGLoginRequiredError,
     IGLoginTwoFactorRequiredError,
     IGLoginUnusablePasswordError,
     IGNotLoggedInError,
     IGRateLimitError,
     IGResponseError,
 )
-from mauigpapi.types import ChallengeStateResponse, LoginResponse
+from mauigpapi.types import ChallengeStateResponse, FacebookLoginResponse, LoginResponse
 from mautrix.types import JSON, Serializable, UserID
 from mautrix.util.logging import TraceLogger
 
 from .. import user as u
 from ..commands.auth import get_login_state
 from .segment import init as init_segment, track
 
 
 class ProvisioningAPI:
     log: TraceLogger = logging.getLogger("mau.web.provisioning")
     app: web.Application
 
-    def __init__(self, shared_secret: str, device_seed: str, segment_key: str | None) -> None:
+    def __init__(
+        self,
+        shared_secret: str,
+        device_seed: str,
+        segment_key: str | None,
+        segment_user_id: str | None,
+    ) -> None:
         self.app = web.Application()
         self.shared_secret = shared_secret
         self.device_seed = device_seed
         if segment_key:
-            init_segment(segment_key)
+            init_segment(segment_key, segment_user_id)
         self.app.router.add_get("/api/whoami", self.status)
         self.app.router.add_options("/api/login", self.login_options)
         self.app.router.add_options("/api/login/2fa", self.login_options)
         self.app.router.add_options("/api/login/resend_2fa_sms", self.login_options)
         self.app.router.add_options("/api/login/checkpoint", self.login_options)
         self.app.router.add_options("/api/login/fb", self.login_options)
         self.app.router.add_options("/api/logout", self.login_options)
@@ -212,15 +219,15 @@
                 ),
                 "status": "logged-out",
             },
             status=401,
             headers=self._acao_headers,
         )
 
-    def _unknown_error(
+    async def _unknown_error(
         self, user: u.User, username: str, e: Exception, after: str, track_error: bool = True
     ) -> web.Response:
         self.log.exception(
             "Unknown error while %s was trying to log in as %s (after %s)",
             user.mxid,
             username,
             after,
@@ -231,17 +238,20 @@
                 "Login error body: %s",
                 e.body.serialize() if isinstance(e.body, Serializable) else e.body,
             )
             if "error_type" in e.body:
                 error_code = e.body["error_type"]
         if track_error:
             track(user, "$login_failed", {"error": error_code})
+        if error_code == "ip_block" and user.proxy_handler:
+            user.proxy_handler.update_proxy_url(reason=error_code)
+            await user.on_proxy_update()
         return web.json_response(
             data={
-                "error": "Unknown error while logging in",
+                "error": "Unknown error while logging in, please try logging in again.",
                 "status": "unknown-error",
                 "ig_error_code": error_code,
             },
             status=500,
             headers=self._acao_headers,
         )
 
@@ -284,14 +294,23 @@
             self.log.debug("%s tried to log in as non-existent user %s", user.mxid, username)
             track(user, "$login_failed", {"error": "invalid-username"})
             return web.json_response(
                 data={"error": "Invalid username", "status": "invalid-username"},
                 status=404,
                 headers=self._acao_headers,
             )
+        except IGLoginInvalidCredentialsError as e:
+            self.log.debug("%s tried to log in with invalid credentials %s", user.mxid, username)
+            self.log.debug("Login error body: %s", e.body.serialize())
+            track(user, "$login_failed", {"error": "invalid-credentials"})
+            return web.json_response(
+                data={"error": "Invalid username or password", "status": "invalid-credentials"},
+                status=403,
+                headers=self._acao_headers,
+            )
         except IGLoginBadPasswordError:
             self.log.debug("%s tried to log in as %s with the wrong password", user.mxid, username)
             track(user, "$login_failed", {"error": "incorrect-password"})
             return web.json_response(
                 data={"error": "Incorrect password", "status": "incorrect-password"},
                 status=403,
                 headers=self._acao_headers,
@@ -309,15 +328,15 @@
                     "error": "Unusable password - please check the Instagram website or app first",
                     "status": "unusable-password",
                 },
                 status=403,
                 headers=self._acao_headers,
             )
         except Exception as e:
-            return self._unknown_error(user, username, e, after="password")
+            return await self._unknown_error(user, username, e, after="password")
         return await self._finish_login(user, state, api, login_resp=resp, after="password")
 
     def _2fa_required(
         self, user: u.User, username: str, state: AndroidState, err: IGLoginTwoFactorRequiredError
     ) -> web.Response:
         track(user, "$login_2fa")
         found_username = err.body.two_factor_info.username if err.body.two_factor_info else None
@@ -393,15 +412,15 @@
                     "status": "2fa-resend-ratelimit",
                     "error": message,
                 },
                 status=429,
             )
         except Exception as e:
             track(user, "$login_resend_2fa_sms_fail", {"error": "unknown"})
-            return self._unknown_error(
+            return await self._unknown_error(
                 user, username, e, after="2fa sms request", track_error=False
             )
         return web.json_response(
             data={
                 "status": "two-factor",
                 "response": resp.serialize(),
             },
@@ -447,15 +466,15 @@
                     "status": "incorrect-2fa-code",
                 },
                 status=403,
                 headers=self._acao_headers,
             )
         except IG2FACodeExpiredError as e:
             self.log.debug("%s submitted an expired 2-factor auth code", user.mxid)
-            self.log.debug("Login error body: %s", e.body.serialize())
+            self.log.debug("Login error body: %s", e.body)
             track(user, "$login_failed", {"error": "expired-2fa-code"})
             return web.json_response(
                 data={
                     "error": e.body.get("message") or str(e),
                     "status": "expired-2fa-code",
                 },
                 status=403,
@@ -465,15 +484,15 @@
             self.log.debug("%s submitted a 2-factor auth code, but got a challenge", user.mxid)
             return await self.start_checkpoint(user, state, api, e, after="2fa")
         except IGConsentRequiredError as e:
             return self._consent_error(user, username, e, after="2fa")
         except IGCheckpointError as e:
             return self._checkpoint_error(user, username, e, after="2fa")
         except Exception as e:
-            return self._unknown_error(user, username, e, after="2fa")
+            return await self._unknown_error(user, username, e, after="2fa")
         return await self._finish_login(user, state, api, login_resp=resp, after="2-factor auth")
 
     async def start_checkpoint(
         self, user: u.User, state: AndroidState, api: AndroidAPI, err: IGChallengeError, after: str
     ) -> web.Response:
         try:
             resp = await api.challenge_auto(reset=after == "2fa")
@@ -555,15 +574,15 @@
                 headers=self._acao_headers,
             )
         except IGConsentRequiredError as e:
             return self._consent_error(user, "<username not known>", e, after="challenge")
         except IGCheckpointError as e:
             return self._checkpoint_error(user, "<username not known>", e, after="challenge")
         except Exception as e:
-            return self._unknown_error(user, "<username not known>", e, after="challenge")
+            return await self._unknown_error(user, "<username not known>", e, after="challenge")
         liu = resp.logged_in_user
         challenge_data = resp.serialize()
         challenge_data.pop("logged_in_user", None)
         self.log.debug(
             "Challenge state for %s after sending security code: %s (logged in user: %s)",
             user.mxid,
             challenge_data,
@@ -613,16 +632,16 @@
         except IGConsentRequiredError as e:
             return self._consent_error(user, username, e, after=f"{after}/success")
         except IGCheckpointError as e:
             return self._checkpoint_error(user, username, e, after=f"{after}/success")
         except IGLoginRequiredError as e:
             return self._login_required_error(user, username, e, after=f"{after}/success")
         except Exception as e:
-            return self._unknown_error(user, username, e, after=f"{after}/success")
-        track(user, "$login_success")
+            return await self._unknown_error(user, username, e, after=f"{after}/success")
+        track(user, "$login_success", {"after": after})
         await user.connect(user=resp.user)
         return web.json_response(
             data={
                 "status": "logged-in",
                 "device_displayname": f"{manufacturer} {model}",
                 "user": resp.user.serialize() if resp and resp.user else None,
             },
@@ -685,32 +704,18 @@
         self.log.debug(
             "%s is attempting to log in with Facebook token (logger ID %s)", user.mxid, logger_id
         )
         track(user, "$login_start", {"type": "facebook"})
         api, state = await get_login_state(user, self.device_seed)
         try:
             resp = await api.facebook_signup(fb_access_token)
+            if not resp.account_created:
+                return self._no_fb_account(user, resp=resp)
         except IGFBNoContactPointFoundError as e:
-            self.log.debug(
-                "%s sent a valid Facebook token, "
-                "but it didn't seem to have an Instagram account linked",
-                user.mxid,
-            )
-            self.log.debug("Login error body: %s", e.body.serialize())
-            track(
-                user, "$login_failed", {"error": "fb-no-account-found", "after": "facebook auth"}
-            )
-            return web.json_response(
-                data={
-                    "error": "You don't have an Instagram account linked to that Facebook account",
-                    "status": e.body.error_type,
-                },
-                status=403,
-                headers=self._acao_headers,
-            )
+            return self._no_fb_account(user, e)
         except IGFBEmailTaken as e:
             maybe_username = None
             for button in e.body.buttons or []:
                 if button.title == "username_log_in":
                     maybe_username = button.username
                     break
             self.log.debug(
@@ -750,16 +755,68 @@
                     ),
                     "username": e.body.username,
                     "status": e.body.error_type,
                 },
                 status=403,
                 headers=self._acao_headers,
             )
+        except IGRateLimitError as e:
+            track(user, "$login_failed", {"error": "fb-ratelimit"})
+            try:
+                message = e.body["message"]
+            except (KeyError, TypeError, AttributeError):
+                message = "Please wait a few minutes before you try again."
+            self.log.debug("%s got a ratelimit error trying to post FB login token", user.mxid)
+            self.log.debug(
+                "Login error body: %s",
+                e.body.serialize() if isinstance(e.body, Serializable) else e.body,
+            )
+            return web.json_response(
+                data={
+                    "status": "fb-ratelimit",
+                    "error": message,
+                },
+                status=429,
+            )
         except IGLoginTwoFactorRequiredError as e:
             return self._2fa_required(user, "<facebook credentials>", state, e)
         except IGCheckpointError as e:
             return self._checkpoint_error(user, "<facebook credentials>", e, after="facebook auth")
+        except IGChallengeError as e:
+            self.log.debug(
+                "%s logged in with facebook credentials, but got a challenge", user.mxid
+            )
+            return await self.start_checkpoint(user, state, api, e, after="facebook auth")
         except IGConsentRequiredError as e:
             return self._consent_error(user, "<facebook credentials>", e, after="facebook auth")
         except Exception as e:
-            return self._unknown_error(user, "<facebook credentials>", e, after="facebook auth")
+            return await self._unknown_error(
+                user, "<facebook credentials>", e, after="facebook auth"
+            )
         return await self._finish_login(user, state, api, login_resp=resp, after="facebook auth")
+
+    def _no_fb_account(
+        self,
+        user: u.User,
+        e: IGFBNoContactPointFoundError | None = None,
+        resp: FacebookLoginResponse | None = None,
+    ) -> web.Response:
+        self.log.debug(
+            "%s sent a valid Facebook token, "
+            "but it didn't seem to have an Instagram account linked",
+            user.mxid,
+        )
+        if e:
+            self.log.debug("Login error body: %s", e.body.serialize() if e else "<N/A>")
+        elif resp:
+            self.log.debug("Login response body: %s", resp.serialize())
+        else:
+            self.log.debug("Login response body: not found")
+        track(user, "$login_failed", {"error": "fb-no-account-found", "after": "facebook auth"})
+        return web.json_response(
+            data={
+                "error": "You don't have an Instagram account linked to that Facebook account",
+                "status": e.body.error_type,
+            },
+            status=403,
+            headers=self._acao_headers,
+        )
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram/web/segment.py` & `mautrix-instagram-0.3.0/mautrix_instagram/web/segment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from __future__ import annotations
 
-import asyncio
 import logging
 
 from yarl import URL
 import aiohttp
 
+from mautrix.util import background_task
+
 from .. import user as u
 
 log = logging.getLogger("mau.web.public.analytics")
 segment_url: URL = URL("https://api.segment.io/v1/track")
 http: aiohttp.ClientSession | None = None
 segment_key: str | None = None
+segment_user_id: str | None = None
 
 
 async def _track(user: u.User, event: str, properties: dict) -> None:
     await http.post(
         segment_url,
         json={
-            "userId": user.mxid,
+            "userId": segment_user_id or user.mxid,
             "event": event,
             "properties": {"bridge": "instagram", **properties},
         },
         auth=aiohttp.BasicAuth(login=segment_key, encoding="utf-8"),
     )
     log.debug(f"Tracked {event}")
 
 
 def track(user: u.User, event: str, properties: dict | None = None):
     if segment_key:
-        asyncio.create_task(_track(user, event, properties or {}))
+        background_task.create(_track(user, event, properties or {}))
 
 
-def init(key):
-    global segment_key, http
+def init(key, user_id: str | None = None):
+    global segment_key, segment_user_id, http
     segment_key = key
+    segment_user_id = user_id
     http = aiohttp.ClientSession()
```

### Comparing `mautrix-instagram-0.2.3/mautrix_instagram.egg-info/PKG-INFO` & `mautrix-instagram-0.3.0/mautrix_instagram.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mautrix-instagram
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Matrix-Instagram puppeting bridge.
 Home-page: https://github.com/mautrix/instagram
 Author: Tulir Asokan
 Author-email: tulir@maunium.net
-License: UNKNOWN
 Project-URL: Changelog, https://github.com/mautrix/instagram/blob/master/CHANGELOG.md
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Communications :: Chat
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -48,9 +46,7 @@
 
 ### Features & Roadmap
 [ROADMAP.md](https://github.com/mautrix/instagram/blob/master/ROADMAP.md)
 contains a general overview of what is supported by the bridge.
 
 ## Discussion
 Matrix room: [`#instagram:maunium.net`](https://matrix.to/#/#instagram:maunium.net)
-
-
```

### Comparing `mautrix-instagram-0.2.3/setup.py` & `mautrix-instagram-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,12 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     package_data={
         "mautrix_instagram": [
             "example-config.yaml",
         ],
-        "mauigpapi.state": [
-            "samples/*.json",
-        ],
     },
     data_files=[
         (".", ["mautrix_instagram/example-config.yaml"]),
     ],
 )
```

