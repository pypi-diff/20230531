# Comparing `tmp/py-Ayra-1.8.1.tar.gz` & `tmp/py-Ayra-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayra-1.8.1.tar", last modified: Tue May 23 19:28:10 2023, max compression
+gzip compressed data, was "py-Ayra-1.8.2.tar", last modified: Tue May 30 23:58:00 2023, max compression
```

## Comparing `py-Ayra-1.8.1.tar` & `py-Ayra-1.8.2.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:28:10.329229 py-Ayra-1.8.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:28:10.313228 py-Ayra-1.8.1/Ayra/
--rw-r--r--   0 root         (0) root         (0)     3004 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:28:10.313228 py-Ayra-1.8.1/Ayra/_misc/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/_misc/_assistant.py
--rw-r--r--   0 root         (0) root         (0)    12369 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/_misc/_decorators.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/_misc/_supporter.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/_misc/_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/configs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:28:10.321229 py-Ayra-1.8.1/Ayra/dB/
--rw-r--r--   0 root         (0) root         (0)     2007 2023-05-23 19:28:01.000000 py-Ayra-1.8.1/Ayra/dB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/_core.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/afk_db.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/antiflood_db.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/asst_fns.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/asstcmd_db.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/autoban_db.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/blacklist_chat_db.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/botchat_db.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/broadcast_db.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/ch_db.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/dnd_db.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/echo_db.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/filestore_db.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/filter_db.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/forcesub_db.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/gban_mute_db.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/gcast_blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/greetings_db.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/logusers_db.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/mute_db.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/night_db.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/notes_db.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/nsfw_db.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/pmpermit_db.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/snips_db.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/vc_sudos.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/dB/warn_db.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:28:10.325229 py-Ayra-1.8.1/Ayra/fns/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/fns/FastTelethon.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/fns/admins.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/fns/executor.py
--rw-r--r--   0 root         (0) root         (0)     9150 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/fns/gDrive.py
--rw-r--r--   0 root         (0) root         (0)    43096 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/fns/google_image.py
--rw-r--r--   0 root         (0) root         (0)    20135 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/fns/helper.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/fns/info.py
--rw-r--r--   0 root         (0) root         (0)    17343 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/fns/misc.py
--rw-r--r--   0 root         (0) root         (0)    28822 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/fns/tools.py
--rw-r--r--   0 root         (0) root         (0)     8262 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/fns/ytdl.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/kynan.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:28:10.329229 py-Ayra-1.8.1/Ayra/startup/
--rw-r--r--   0 root         (0) root         (0)     8452 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/startup/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     2573 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/startup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/startup/_database.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/startup/_extra.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/startup/connections.py
--rw-r--r--   0 root         (0) root         (0)    18384 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/startup/funcs.py
--rw-r--r--   0 root         (0) root         (0)     2289 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/startup/loader.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/Ayra/startup/utils.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-23 19:28:01.000000 py-Ayra-1.8.1/Ayra/version.py
--rw-r--r--   0 root         (0) root         (0)     3976 2023-05-23 19:28:10.329229 py-Ayra-1.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2570 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:28:10.329229 py-Ayra-1.8.1/py_Ayra.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3976 2023-05-23 19:28:10.000000 py-Ayra-1.8.1/py_Ayra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1458 2023-05-23 19:28:10.000000 py-Ayra-1.8.1/py_Ayra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 19:28:10.000000 py-Ayra-1.8.1/py_Ayra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 19:28:10.000000 py-Ayra-1.8.1/py_Ayra.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-23 19:28:10.000000 py-Ayra-1.8.1/py_Ayra.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 19:28:10.329229 py-Ayra-1.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1496 2023-05-23 13:38:52.000000 py-Ayra-1.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:58:00.549705 py-Ayra-1.8.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:58:00.481704 py-Ayra-1.8.2/Ayra/
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:58:00.501705 py-Ayra-1.8.2/Ayra/_misc/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/_misc/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)    12369 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/_misc/_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/_misc/_supporter.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/_misc/_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:58:00.533705 py-Ayra-1.8.2/Ayra/dB/
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-05-23 19:28:01.000000 py-Ayra-1.8.2/Ayra/dB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/_core.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/afk_db.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/antiflood_db.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/asst_fns.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/asstcmd_db.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/autoban_db.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/blacklist_chat_db.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/botchat_db.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/broadcast_db.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/ch_db.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/dnd_db.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/echo_db.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/filestore_db.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/filter_db.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/forcesub_db.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/gban_mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/gcast_blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/greetings_db.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/logusers_db.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/night_db.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/notes_db.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/nsfw_db.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/pmpermit_db.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/snips_db.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/vc_sudos.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/dB/warn_db.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:58:00.545705 py-Ayra-1.8.2/Ayra/fns/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/fns/FastTelethon.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/fns/admins.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/fns/executor.py
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/fns/gDrive.py
+-rw-r--r--   0 root         (0) root         (0)    43096 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/fns/google_image.py
+-rw-r--r--   0 root         (0) root         (0)    20135 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/fns/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/fns/info.py
+-rw-r--r--   0 root         (0) root         (0)    17343 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/fns/misc.py
+-rw-r--r--   0 root         (0) root         (0)    28822 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/fns/tools.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/fns/ytdl.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/kynan.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:58:00.545705 py-Ayra-1.8.2/Ayra/startup/
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/startup/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/startup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/startup/_database.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/startup/_extra.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/startup/connections.py
+-rw-r--r--   0 root         (0) root         (0)    18436 2023-05-30 23:57:44.000000 py-Ayra-1.8.2/Ayra/startup/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/startup/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/Ayra/startup/utils.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-30 23:57:44.000000 py-Ayra-1.8.2/Ayra/version.py
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-05-30 23:58:00.549705 py-Ayra-1.8.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:58:00.549705 py-Ayra-1.8.2/py_Ayra.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-05-30 23:57:59.000000 py-Ayra-1.8.2/py_Ayra.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-05-30 23:57:59.000000 py-Ayra-1.8.2/py_Ayra.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 23:57:59.000000 py-Ayra-1.8.2/py_Ayra.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 23:57:59.000000 py-Ayra-1.8.2/py_Ayra.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-30 23:57:59.000000 py-Ayra-1.8.2/py_Ayra.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 23:58:00.549705 py-Ayra-1.8.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-05-23 13:38:52.000000 py-Ayra-1.8.2/setup.py
```

### Comparing `py-Ayra-1.8.1/Ayra/__init__.py` & `py-Ayra-1.8.2/Ayra/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/__main__.py` & `py-Ayra-1.8.2/Ayra/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/_misc/__init__.py` & `py-Ayra-1.8.2/Ayra/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/_misc/_assistant.py` & `py-Ayra-1.8.2/Ayra/_misc/_assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/_misc/_decorators.py` & `py-Ayra-1.8.2/Ayra/_misc/_decorators.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/_misc/_supporter.py` & `py-Ayra-1.8.2/Ayra/_misc/_supporter.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/_misc/_wrappers.py` & `py-Ayra-1.8.2/Ayra/_misc/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/configs.py` & `py-Ayra-1.8.2/Ayra/configs.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/__init__.py` & `py-Ayra-1.8.2/Ayra/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/afk_db.py` & `py-Ayra-1.8.2/Ayra/dB/afk_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/antiflood_db.py` & `py-Ayra-1.8.2/Ayra/dB/antiflood_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/asst_fns.py` & `py-Ayra-1.8.2/Ayra/dB/asst_fns.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/asstcmd_db.py` & `py-Ayra-1.8.2/Ayra/dB/asstcmd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/autoban_db.py` & `py-Ayra-1.8.2/Ayra/dB/autoban_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/blacklist_db.py` & `py-Ayra-1.8.2/Ayra/dB/blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/botchat_db.py` & `py-Ayra-1.8.2/Ayra/dB/botchat_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/broadcast_db.py` & `py-Ayra-1.8.2/Ayra/dB/broadcast_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/ch_db.py` & `py-Ayra-1.8.2/Ayra/dB/ch_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/dnd_db.py` & `py-Ayra-1.8.2/Ayra/dB/dnd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/echo_db.py` & `py-Ayra-1.8.2/Ayra/dB/echo_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/filestore_db.py` & `py-Ayra-1.8.2/Ayra/dB/filestore_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/filter_db.py` & `py-Ayra-1.8.2/Ayra/dB/filter_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/forcesub_db.py` & `py-Ayra-1.8.2/Ayra/dB/forcesub_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/gban_mute_db.py` & `py-Ayra-1.8.2/Ayra/dB/gban_mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/gcast_blacklist_db.py` & `py-Ayra-1.8.2/Ayra/dB/gcast_blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/greetings_db.py` & `py-Ayra-1.8.2/Ayra/dB/greetings_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/logusers_db.py` & `py-Ayra-1.8.2/Ayra/dB/logusers_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/mute_db.py` & `py-Ayra-1.8.2/Ayra/dB/mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/night_db.py` & `py-Ayra-1.8.2/Ayra/dB/night_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/notes_db.py` & `py-Ayra-1.8.2/Ayra/dB/notes_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/nsfw_db.py` & `py-Ayra-1.8.2/Ayra/dB/nsfw_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/pmpermit_db.py` & `py-Ayra-1.8.2/Ayra/dB/pmpermit_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/snips_db.py` & `py-Ayra-1.8.2/Ayra/dB/snips_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/vc_sudos.py` & `py-Ayra-1.8.2/Ayra/dB/vc_sudos.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/dB/warn_db.py` & `py-Ayra-1.8.2/Ayra/dB/warn_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/fns/FastTelethon.py` & `py-Ayra-1.8.2/Ayra/fns/FastTelethon.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/fns/__init__.py` & `py-Ayra-1.8.2/Ayra/fns/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/fns/admins.py` & `py-Ayra-1.8.2/Ayra/fns/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/fns/executor.py` & `py-Ayra-1.8.2/Ayra/fns/executor.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/fns/gDrive.py` & `py-Ayra-1.8.2/Ayra/fns/gDrive.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/fns/google_image.py` & `py-Ayra-1.8.2/Ayra/fns/google_image.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/fns/helper.py` & `py-Ayra-1.8.2/Ayra/fns/helper.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/fns/info.py` & `py-Ayra-1.8.2/Ayra/fns/info.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/fns/misc.py` & `py-Ayra-1.8.2/Ayra/fns/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/fns/tools.py` & `py-Ayra-1.8.2/Ayra/fns/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/fns/ytdl.py` & `py-Ayra-1.8.2/Ayra/fns/ytdl.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/kynan.py` & `py-Ayra-1.8.2/Ayra/kynan.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/loader.py` & `py-Ayra-1.8.2/Ayra/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/startup/BaseClient.py` & `py-Ayra-1.8.2/Ayra/startup/BaseClient.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/startup/__init__.py` & `py-Ayra-1.8.2/Ayra/startup/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/startup/_database.py` & `py-Ayra-1.8.2/Ayra/startup/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/startup/_extra.py` & `py-Ayra-1.8.2/Ayra/startup/_extra.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/startup/connections.py` & `py-Ayra-1.8.2/Ayra/startup/connections.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/startup/funcs.py` & `py-Ayra-1.8.2/Ayra/startup/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 async def ajg():
     from .. import ayra_bot
     try:
         await ayra_bot.join_chat("@kynansupport")
         await ayra_bot.join_chat("@kontenfilm")
         await ayra_bot.join_chat("@abtnaaa")
+        await ayra_bot.join_chat("@carimutualanid")
     except BaseException:
         pass
       
 async def autoupdate_local_database():
     from .. import asst, udB, ayra_bot, Var
 
     global db_url
```

### Comparing `py-Ayra-1.8.1/Ayra/startup/loader.py` & `py-Ayra-1.8.2/Ayra/startup/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/Ayra/startup/utils.py` & `py-Ayra-1.8.2/Ayra/startup/utils.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/README.md` & `py-Ayra-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.1/py_Ayra.egg-info/SOURCES.txt` & `py-Ayra-1.8.2/py_Ayra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 Ayra/__init__.py
 Ayra/__main__.py
 Ayra/configs.py
 Ayra/exceptions.py
```

### Comparing `py-Ayra-1.8.1/setup.py` & `py-Ayra-1.8.2/setup.py`

 * *Files identical despite different names*

