# Comparing `tmp/fb_tools-2.2.2.tar.gz` & `tmp/fb_tools-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb_tools-2.2.2.tar", last modified: Mon Feb  6 10:31:53 2023, max compression
+gzip compressed data, was "fb_tools-2.2.3.tar", last modified: Wed May 31 15:59:53 2023, max compression
```

## Comparing `fb_tools-2.2.2.tar` & `fb_tools-2.2.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.286900 fb_tools-2.2.2/
--rw-r--r--   0 root         (0) root         (0)     7652 2023-02-06 10:31:31.000000 fb_tools-2.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      120 2023-02-06 10:31:31.000000 fb_tools-2.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1729 2023-02-06 10:31:53.286900 fb_tools-2.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      503 2023-02-06 10:31:31.000000 fb_tools-2.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.278900 fb_tools-2.2.2/bin/
--rwxr-xr-x   0 root         (0) root         (0)     2463 2023-02-06 10:31:31.000000 fb_tools-2.2.2/bin/get-file-to-remove
--rwxr-xr-x   0 root         (0) root         (0)     1574 2023-02-06 10:31:31.000000 fb_tools-2.2.2/bin/myip
--rwxr-xr-x   0 root         (0) root         (0)     1588 2023-02-06 10:31:31.000000 fb_tools-2.2.2/bin/update-ddns
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.278900 fb_tools-2.2.2/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.282900 fb_tools-2.2.2/lib/fb_tools/
--rw-r--r--   0 root         (0) root         (0)      406 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28032 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/app.py
--rw-r--r--   0 root         (0) root         (0)     8423 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/argparse_actions.py
--rw-r--r--   0 root         (0) root         (0)     9663 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/cfg_app.py
--rw-r--r--   0 root         (0) root         (0)    36832 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/collections.py
--rw-r--r--   0 root         (0) root         (0)    24990 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/common.py
--rw-r--r--   0 root         (0) root         (0)     8168 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.282900 fb_tools-2.2.2/lib/fb_tools/ddns/
--rw-r--r--   0 root         (0) root         (0)    18929 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/ddns/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10617 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/ddns/config.py
--rw-r--r--   0 root         (0) root         (0)     5564 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/ddns/myip_app.py
--rw-r--r--   0 root         (0) root         (0)    14006 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/ddns/update_app.py
--rw-r--r--   0 root         (0) root         (0)    12596 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/errors.py
--rw-r--r--   0 root         (0) root         (0)    24496 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/get_file_rm_app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.282900 fb_tools-2.2.2/lib/fb_tools/handler/
--rw-r--r--   0 root         (0) root         (0)    14101 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43541 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/handler/lock.py
--rw-r--r--   0 root         (0) root         (0)    39537 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/handling_obj.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-02-06 10:31:53.000000 fb_tools-2.2.2/lib/fb_tools/local_version.py
--rw-r--r--   0 root         (0) root         (0)    34977 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/mailaddress.py
--rw-r--r--   0 root         (0) root         (0)     2391 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/merge.py
--rw-r--r--   0 root         (0) root         (0)    43901 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/multi_config.py
--rw-r--r--   0 root         (0) root         (0)    11766 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/obj.py
--rw-r--r--   0 root         (0) root         (0)    17133 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/pidfile.py
--rw-r--r--   0 root         (0) root         (0)     2954 2023-02-06 10:31:31.000000 fb_tools-2.2.2/lib/fb_tools/xlate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.282900 fb_tools-2.2.2/lib/fb_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1729 2023-02-06 10:31:53.000000 fb_tools-2.2.2/lib/fb_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1378 2023-02-06 10:31:53.000000 fb_tools-2.2.2/lib/fb_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 10:31:53.000000 fb_tools-2.2.2/lib/fb_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-02-06 10:31:53.000000 fb_tools-2.2.2/lib/fb_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-02-06 10:31:53.000000 fb_tools-2.2.2/lib/fb_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.282900 fb_tools-2.2.2/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.278900 fb_tools-2.2.2/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.282900 fb_tools-2.2.2/locale/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    41697 2023-02-06 10:31:53.000000 fb_tools-2.2.2/locale/de/LC_MESSAGES/fb_tools.mo
--rw-r--r--   0 root         (0) root         (0)    60324 2023-02-06 10:31:31.000000 fb_tools-2.2.2/locale/de/LC_MESSAGES/fb_tools.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.278900 fb_tools-2.2.2/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.282900 fb_tools-2.2.2/locale/en/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     5422 2023-02-06 10:31:53.000000 fb_tools-2.2.2/locale/en/LC_MESSAGES/fb_tools.mo
--rw-r--r--   0 root         (0) root         (0)    43138 2023-02-06 10:31:31.000000 fb_tools-2.2.2/locale/en/LC_MESSAGES/fb_tools.po
--rw-r--r--   0 root         (0) root         (0)    41261 2023-02-06 10:31:31.000000 fb_tools-2.2.2/locale/fb_tools.pot
--rw-r--r--   0 root         (0) root         (0)     1790 2023-02-06 10:31:53.286900 fb_tools-2.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8850 2023-02-06 10:31:31.000000 fb_tools-2.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 10:31:53.286900 fb_tools-2.2.2/test/
--rwxr-xr-x   0 root         (0) root         (0)      270 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/call_script.sh
--rwxr-xr-x   0 root         (0) root         (0)      438 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/call_sleep.sh
--rwxr-xr-x   0 root         (0) root         (0)      438 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/do_sleep
--rw-r--r--   0 root         (0) root         (0)     3257 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/general.py
--rwxr-xr-x   0 root         (0) root         (0)     4459 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/test_00_errors.py
--rwxr-xr-x   0 root         (0) root         (0)    24389 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/test_05_common.py
--rwxr-xr-x   0 root         (0) root         (0)     6432 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/test_10_base_object.py
--rwxr-xr-x   0 root         (0) root         (0)    59500 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/test_13_collections.py
--rwxr-xr-x   0 root         (0) root         (0)    52741 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/test_15_mailaddress.py
--rwxr-xr-x   0 root         (0) root         (0)    17995 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/test_17_multicfg.py
--rwxr-xr-x   0 root         (0) root         (0)     5817 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/test_18_pidfile.py
--rwxr-xr-x   0 root         (0) root         (0)    19877 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/test_20_handling_object.py
--rwxr-xr-x   0 root         (0) root         (0)     7626 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/test_30_base_handler.py
--rwxr-xr-x   0 root         (0) root         (0)    14476 2023-02-06 10:31:31.000000 fb_tools-2.2.2/test/test_33_lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.764640 fb_tools-2.2.3/
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-05-31 15:59:30.000000 fb_tools-2.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      120 2023-05-31 15:59:30.000000 fb_tools-2.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-05-31 15:59:53.764640 fb_tools-2.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-31 15:59:30.000000 fb_tools-2.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.756640 fb_tools-2.2.3/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     2463 2023-05-31 15:59:30.000000 fb_tools-2.2.3/bin/get-file-to-remove
+-rwxr-xr-x   0 root         (0) root         (0)     1574 2023-05-31 15:59:30.000000 fb_tools-2.2.3/bin/myip
+-rwxr-xr-x   0 root         (0) root         (0)     1588 2023-05-31 15:59:30.000000 fb_tools-2.2.3/bin/update-ddns
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.756640 fb_tools-2.2.3/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/lib/fb_tools/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28061 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/app.py
+-rw-r--r--   0 root         (0) root         (0)     8423 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/argparse_actions.py
+-rw-r--r--   0 root         (0) root         (0)     9654 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/cfg_app.py
+-rw-r--r--   0 root         (0) root         (0)    36990 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/collections.py
+-rw-r--r--   0 root         (0) root         (0)    24990 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/common.py
+-rw-r--r--   0 root         (0) root         (0)     8163 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/lib/fb_tools/ddns/
+-rw-r--r--   0 root         (0) root         (0)    18917 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/ddns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10614 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/ddns/config.py
+-rw-r--r--   0 root         (0) root         (0)     5560 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/ddns/myip_app.py
+-rw-r--r--   0 root         (0) root         (0)    14002 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/ddns/update_app.py
+-rw-r--r--   0 root         (0) root         (0)    12591 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/errors.py
+-rw-r--r--   0 root         (0) root         (0)    24492 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/get_file_rm_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/lib/fb_tools/handler/
+-rw-r--r--   0 root         (0) root         (0)    14092 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43539 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/handler/lock.py
+-rw-r--r--   0 root         (0) root         (0)    39509 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/handling_obj.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-05-31 15:59:53.000000 fb_tools-2.2.3/lib/fb_tools/local_version.py
+-rw-r--r--   0 root         (0) root         (0)    34973 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/mailaddress.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/merge.py
+-rw-r--r--   0 root         (0) root         (0)    43962 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/multi_config.py
+-rw-r--r--   0 root         (0) root         (0)    11761 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/obj.py
+-rw-r--r--   0 root         (0) root         (0)    17133 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/pidfile.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/xlate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/lib/fb_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-05-31 15:59:53.000000 fb_tools-2.2.3/lib/fb_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-05-31 15:59:53.000000 fb_tools-2.2.3/lib/fb_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:59:53.000000 fb_tools-2.2.3/lib/fb_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-31 15:59:53.000000 fb_tools-2.2.3/lib/fb_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-31 15:59:53.000000 fb_tools-2.2.3/lib/fb_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.756640 fb_tools-2.2.3/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/locale/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    41697 2023-05-31 15:59:53.000000 fb_tools-2.2.3/locale/de/LC_MESSAGES/fb_tools.mo
+-rw-r--r--   0 root         (0) root         (0)    60342 2023-05-31 15:59:30.000000 fb_tools-2.2.3/locale/de/LC_MESSAGES/fb_tools.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.756640 fb_tools-2.2.3/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/locale/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     5422 2023-05-31 15:59:53.000000 fb_tools-2.2.3/locale/en/LC_MESSAGES/fb_tools.mo
+-rw-r--r--   0 root         (0) root         (0)    43156 2023-05-31 15:59:30.000000 fb_tools-2.2.3/locale/en/LC_MESSAGES/fb_tools.po
+-rw-r--r--   0 root         (0) root         (0)    41273 2023-05-31 15:59:30.000000 fb_tools-2.2.3/locale/fb_tools.pot
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-05-31 15:59:53.764640 fb_tools-2.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8889 2023-05-31 15:59:30.000000 fb_tools-2.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.764640 fb_tools-2.2.3/test/
+-rwxr-xr-x   0 root         (0) root         (0)      270 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/call_script.sh
+-rwxr-xr-x   0 root         (0) root         (0)      438 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/call_sleep.sh
+-rwxr-xr-x   0 root         (0) root         (0)      438 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/do_sleep
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/general.py
+-rwxr-xr-x   0 root         (0) root         (0)     4459 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_00_errors.py
+-rwxr-xr-x   0 root         (0) root         (0)    24389 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_05_common.py
+-rwxr-xr-x   0 root         (0) root         (0)     6432 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_10_base_object.py
+-rwxr-xr-x   0 root         (0) root         (0)    59500 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_13_collections.py
+-rwxr-xr-x   0 root         (0) root         (0)    52741 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_15_mailaddress.py
+-rwxr-xr-x   0 root         (0) root         (0)    17995 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_17_multicfg.py
+-rwxr-xr-x   0 root         (0) root         (0)     5817 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_18_pidfile.py
+-rwxr-xr-x   0 root         (0) root         (0)    19877 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_20_handling_object.py
+-rwxr-xr-x   0 root         (0) root         (0)     7626 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_30_base_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)    14476 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_33_lock.py
```

### Comparing `fb_tools-2.2.2/LICENSE` & `fb_tools-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.2/PKG-INFO` & `fb_tools-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_tools
-Version: 2.2.2
+Version: 2.2.3
 Summary: Modules for common used objects, error classes and methods.
 Home-page: https://github.com/fbrehm/python_fb_tools
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_tools-2.2.2/bin/get-file-to-remove` & `fb_tools-2.2.3/bin/get-file-to-remove`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 @summary: Returns a newline separated list of files generated from file globbing patterns
 """
 from __future__ import print_function
 
 # Standard modules
 import sys
 import gettext
@@ -67,15 +67,15 @@
 from fb_tools.xlate import XLATOR
 
 _ = XLATOR.gettext
 
 LOG = logging.getLogger(__name__)
 
 __author__ = 'Frank Brehm <frank.brehm@pixelpark.com>'
-__copyright__ = '(C) 2019 by Frank Brehm, Pixelpark GmbH, Berlin'
+__copyright__ = '(C) 2023 by Frank Brehm, Pixelpark GmbH, Berlin'
 
 appname = my_path.name
 
 locale.setlocale(locale.LC_ALL, '')
 
 app = GetFileRmApplication(appname=appname, base_dir=base_dir)
 app.initialized = True
```

### Comparing `fb_tools-2.2.2/bin/myip` & `fb_tools-2.2.3/bin/myip`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     sys.path.insert(0, lib_dir)
 
 from fb_tools.ddns.myip_app import MyIpApplication
 
 log = logging.getLogger(__name__)
 
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
-__copyright__ = '(C) 2019 by Frank Brehm, Berlin'
+__copyright__ = '(C) 2023 by Frank Brehm, Berlin'
 
 appname = os.path.basename(sys.argv[0])
 
 locale.setlocale(locale.LC_ALL, '')
 
 app = MyIpApplication(appname=appname, base_dir=base_dir)
 app.initialized = True
```

### Comparing `fb_tools-2.2.2/bin/update-ddns` & `fb_tools-2.2.3/bin/update-ddns`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     sys.path.insert(0, lib_dir)
 
 from fb_tools.ddns.update_app import UpdateDdnsApplication
 
 log = logging.getLogger(__name__)
 
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
-__copyright__ = '(C) 2019 by Frank Brehm, Berlin'
+__copyright__ = '(C) 2023 by Frank Brehm, Berlin'
 
 appname = os.path.basename(sys.argv[0])
 
 locale.setlocale(locale.LC_ALL, '')
 
 app = UpdateDdnsApplication(appname=appname, base_dir=base_dir)
 app.initialized = True
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/app.py` & `fb_tools-2.2.3/lib/fb_tools/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a base application object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import sys
-import os
-import logging
-import re
-import traceback
 import argparse
+import copy
 import getpass
+import logging
+import os
+import re
 import signal
+import sys
 import time
-import copy
+import traceback
 
 # Third party modules
 
 # Own modules
 from fb_logging.colored import ColoredFormatter
 
 from . import __version__ as __pkg_version__
-
 from .argparse_actions import TimeoutOptionAction
-
+from .common import terminal_can_colors
 from .errors import FbAppError
 from .errors import FunctionNotImplementedError
-
-from .common import terminal_can_colors
-
 from .handling_obj import HandlingObject
-
-from .xlate import __module_dir__ as __xlate_module_dir__
+from .xlate import DOMAIN, LOCALE_DIR, XLATOR
 from .xlate import __base_dir__ as __xlate_base_dir__
 from .xlate import __mo_file__ as __xlate_mo_file__
-from .xlate import XLATOR, LOCALE_DIR, DOMAIN
+from .xlate import __module_dir__ as __xlate_module_dir__
 
-__version__ = '2.2.0'
+__version__ = '2.2.2'
 LOG = logging.getLogger(__name__)
 
 SIGNAL_NAMES = {
     signal.SIGHUP: 'HUP',
     signal.SIGINT: 'INT',
     signal.SIGABRT: 'ABRT',
     signal.SIGTERM: 'TERM',
@@ -62,15 +57,15 @@
 # =============================================================================
 class BaseApplication(HandlingObject):
     """Class for the base application objects."""
 
     re_prefix = re.compile(r'^[a-z0-9][a-z0-9_]*$', re.IGNORECASE)
     re_anum = re.compile(r'[^A-Z0-9_]+', re.IGNORECASE)
 
-    default_force_desc_msg = _("Forced execution - whatever it means.")
+    default_force_desc_msg = _('Forced execution - whatever it means.')
 
     show_assume_options = False
     show_console_timeout_option = False
     show_force_option = False
     show_simulate_option = True
 
     # -------------------------------------------------------------------------
@@ -144,30 +139,30 @@
             quiet=quiet, simulate=simulate, force=force, assumed_answer=assumed_answer,
             terminal_has_colors=terminal_has_colors, initialized=False,
         )
 
         if env_prefix:
             ep = str(env_prefix).strip()
             if not ep:
-                msg = _("Invalid env_prefix {!r} given - it may not be empty.").format(env_prefix)
+                msg = _('Invalid env_prefix {!r} given - it may not be empty.').format(env_prefix)
                 raise FbAppError(msg)
             match = self.re_prefix.search(ep)
             if not match:
                 msg = _(
-                    "Invalid characters found in env_prefix {!r}, only "
-                    "alphanumeric characters and digits and underscore "
-                    "(this not as the first character) are allowed.").format(env_prefix)
+                    'Invalid characters found in env_prefix {!r}, only '
+                    'alphanumeric characters and digits and underscore '
+                    '(this not as the first character) are allowed.').format(env_prefix)
                 raise FbAppError(msg)
             self._env_prefix = ep
         else:
             ep = self.appname.upper() + '_'
             self._env_prefix = self.re_anum.sub('_', ep)
 
         if not self.description:
-            self._description = _("Unknown and undescriped application.")
+            self._description = _('Unknown and undescriped application.')
 
         if not hasattr(self, '_force_desc_msg'):
             self._force_desc_msg = self.default_force_desc_msg
 
         self._init_arg_parser()
         self._perform_arg_parser()
 
@@ -184,15 +179,15 @@
 
     @exit_value.setter
     def exit_value(self, value):
         v = int(value)
         if v >= 0:
             self._exit_value = v
         else:
-            LOG.warning(_("Wrong exit_value {!r}, must be >= 0.").format(value))
+            LOG.warning(_('Wrong exit_value {!r}, must be >= 0.').format(value))
 
     # -----------------------------------------------------------
     @property
     def force_desc_msg(self):
         """Get the help text for the --force command line option."""
         msg = getattr(self, '_force_desc_msg', None)
         if not msg:
@@ -248,15 +243,15 @@
     # -----------------------------------------------------------
     @property
     def usage_term_len(self):
         """Get the length of the localized version of 'usage: '."""
         return len(self.usage_term)
 
     # -------------------------------------------------------------------------
-    def exit(self, retval=-1, msg=None, trace=False):
+    def exit(self, retval=-1, msg=None, trace=False):                       # noqa A003
         """
         Exit the current application.
 
         Universal method to call sys.exit(). If fake_exit is set, a
         FakeExitError exception is raised instead (useful for unittests.)
 
         @param retval: the return value to give back to theoperating system
@@ -281,17 +276,17 @@
             if has_handlers:
                 if retval:
                     LOG.error(msg)
                 else:
                     LOG.info(msg)
             if not has_handlers:
                 if hasattr(sys.stderr, 'buffer'):
-                    sys.stderr.buffer.write(str(msg) + "\n")
+                    sys.stderr.buffer.write(str(msg) + '\n')
                 else:
-                    sys.stderr.write(str(msg) + "\n")
+                    sys.stderr.write(str(msg) + '\n')
 
         if trace:
             if has_handlers:
                 if retval:
                     LOG.error(traceback.format_exc())
                 else:
                     LOG.info(traceback.format_exc())
@@ -421,92 +416,92 @@
         self.init_logging()
 
         self.perform_arg_parser()
 
     # -------------------------------------------------------------------------
     def get_secret(self, prompt, item_name):
         """Get a secret as input from console."""
-        LOG.debug(_("Trying to get {} via console ...").format(item_name))
+        LOG.debug(_('Trying to get {} via console ...').format(item_name))
 
         # ------------------------
         def signal_handler(signum, frame):
             """
             React to an alarm signal.
 
             Handler as a callback function for getting a signal from somewhere.
 
             @param signum: the gotten signal number
             @type signum: int
             @param frame: the current stack frame
             @type frame: None or a frame object
 
             """
-            signame = "{}".format(signum)
-            msg = _("Got a signal {}.").format(signum)
+            signame = '{}'.format(signum)
+            msg = _('Got a signal {}.').format(signum)
             if signum in SIGNAL_NAMES:
                 signame = SIGNAL_NAMES[signum]
-                msg = _("Got a signal {n!r} ({s}).").format(
+                msg = _('Got a signal {n!r} ({s}).').format(
                     n=signame, s=signum)
             LOG.debug(msg)
 
             if signum in (
                     signal.SIGHUP, signal.SIGINT, signal.SIGABRT,
                     signal.SIGTERM, signal.SIGKILL, signal.SIGQUIT):
-                LOG.info(_("Exit on signal {n!r} ({s}).").format(
+                LOG.info(_('Exit on signal {n!r} ({s}).').format(
                     n=signame, s=signum))
                 self.exit(1)
 
         # ------------------------
         old_handlers = {}
 
         if self.verbose > 2:
-            LOG.debug(_("Tweaking signal handlers."))
+            LOG.debug(_('Tweaking signal handlers.'))
         for signum in (
                 signal.SIGHUP, signal.SIGINT, signal.SIGABRT,
                 signal.SIGTERM, signal.SIGQUIT):
             if self.verbose > 3:
                 signame = SIGNAL_NAMES[signum]
-                LOG.debug(_("Setting signal handler for {n!r} ({s}).").format(
+                LOG.debug(_('Setting signal handler for {n!r} ({s}).').format(
                     n=signame, s=signum))
             old_handlers[signum] = signal.signal(signum, signal_handler)
 
         secret = None
         secret_repeat = None
 
         try:
 
             while True:
 
-                p = _("Enter ") + prompt + ': '
+                p = _('Enter ') + prompt + ': '
                 while True:
                     secret = getpass.getpass(prompt=p)
                     secret = secret.strip()
                     if secret != '':
                         break
 
-                p = _("Repeat enter ") + prompt + ': '
+                p = _('Repeat enter ') + prompt + ': '
                 while True:
                     secret_repeat = getpass.getpass(prompt=p)
                     secret_repeat = secret_repeat.strip()
                     if secret_repeat != '':
                         break
 
                 if secret == secret_repeat:
                     break
 
-                LOG.error(_("{n} and repeated {n} did not match.").format(n=item_name))
+                LOG.error(_('{n} and repeated {n} did not match.').format(n=item_name))
 
         finally:
             if self.verbose > 2:
-                LOG.debug(_("Restoring original signal handlers."))
+                LOG.debug(_('Restoring original signal handlers.'))
             for signum in old_handlers.keys():
                 signal.signal(signum, old_handlers[signum])
 
         if self.force:
-            LOG.debug(_("Got {n!r}: {s!r}").format(n=item_name, s=secret))
+            LOG.debug(_('Got {n!r}: {s!r}').format(n=item_name, s=secret))
 
         return secret
 
     # -------------------------------------------------------------------------
     def pre_run(self):
         """
         Execute some actions before the main routine.
@@ -548,36 +543,36 @@
 
         The visible start point of this object.
 
         @return: None
         """
         if not self.initialized:
             self.handle_error(
-                _("The application is not completely initialized."), '', True)
+                _('The application is not completely initialized.'), '', True)
             self.exit(9)
 
         try:
             self.pre_run()
         except Exception as e:
             self.handle_error(str(e), e.__class__.__name__, True)
             self.exit(98)
 
         if not self.initialized:
             raise FbAppError(
-                _("Object {!r} seems not to be completely initialized.").format(
+                _('Object {!r} seems not to be completely initialized.').format(
                     self.__class__.__name__))
 
         try:
             self._run()
         except Exception as e:
             self.handle_error(str(e), e.__class__.__name__, True)
             self.exit_value = 99
 
         if self.verbose > 1:
-            LOG.info(_("Ending."))
+            LOG.info(_('Ending.'))
 
         try:
             self.post_run()
         except Exception as e:
             self.handle_error(str(e), e.__class__.__name__, True)
             self.exit_value = 97
 
@@ -587,15 +582,15 @@
     def post_run(self):
         """
         Execute some actions after the main routine.
 
         This is a dummy method an could be overwritten by descendant classes.
         """
         if self.verbose > 1:
-            LOG.info(_("Executing {} ...").format('post_run()'))
+            LOG.info(_('Executing {} ...').format('post_run()'))
 
     # -------------------------------------------------------------------------
     def _init_arg_parser(self):
         """
         Initialise the argument parser.
 
         Local called method to initiate the argument parser.
@@ -613,76 +608,76 @@
 
         self.init_arg_parser()
 
         general_group = self.arg_parser.add_argument_group(_('General options'))
 
         if self.show_simulate_option:
             general_group.add_argument(
-                '-s', "--simulate", action="store_true", dest="simulate",
-                help=_("Simulation mode, nothing is really done.")
+                '-s', '--simulate', action='store_true', dest='simulate',
+                help=_('Simulation mode, nothing is really done.')
             )
 
         if self.show_force_option:
             general_group.add_argument(
-                '-f', "--force", action="store_true", dest="force",
+                '-f', '--force', action='store_true', dest='force',
                 help=self.force_desc_msg,
             )
 
         if self.show_assume_options:
             assume_group = general_group.add_mutually_exclusive_group()
 
             assume_group.add_argument(
-                '--yes', '--assume-yes', action="store_true", dest="assume_yes",
+                '--yes', '--assume-yes', action='store_true', dest='assume_yes',
                 help=_("Automatically answer '{}' for all questions.").format(
                     self.colored(_('Yes'), 'CYAN'))
             )
 
             assume_group.add_argument(
-                '--no', '--assume-no', action="store_true", dest="assume_no",
+                '--no', '--assume-no', action='store_true', dest='assume_no',
                 help=_("Automatically answer '{}' for all questions.").format(
                     self.colored(_('No'), 'CYAN'))
             )
 
         if self.show_console_timeout_option:
             general_group.add_argument(
-                '--console-timeout', metavar=_('SECONDS'), dest="console_timeout", type=int,
+                '--console-timeout', metavar=_('SECONDS'), dest='console_timeout', type=int,
                 action=TimeoutOptionAction, max_timeout=self.max_prompt_timeout,
-                help=_("The timeout in seconds for console input. Default: {}").format(
+                help=_('The timeout in seconds for console input. Default: {}').format(
                     self.default_prompt_timeout)
             )
 
         general_group.add_argument(
-            '--color', action="store", dest='color', const='yes',
+            '--color', action='store', dest='color', const='yes',
             default='auto', nargs='?', choices=['yes', 'no', 'auto'],
-            help=_("Use colored output for messages."),
+            help=_('Use colored output for messages.'),
         )
 
         verbose_group = general_group.add_mutually_exclusive_group()
 
         verbose_group.add_argument(
-            "-v", "--verbose", action="count", dest='verbose',
+            '-v', '--verbose', action='count', dest='verbose',
             help=_('Increase the verbosity level'),
         )
 
         verbose_group.add_argument(
-            "-q", "--quiet", action="store_true", dest='quiet',
+            '-q', '--quiet', action='store_true', dest='quiet',
             help=_('Silent execution, only warnings and errors are emitted.'),
         )
 
         general_group.add_argument(
-            "-h", "--help", action='help', dest='help',
+            '-h', '--help', action='help', dest='help',
             help=_('Show this help message and exit.')
         )
         general_group.add_argument(
-            "--usage", action='store_true', dest='usage',
-            help=_("Display brief usage message and exit.")
+            '--usage', action='store_true', dest='usage',
+            help=_('Display brief usage message and exit.')
         )
-        v_msg = _("Version of %(prog)s: {}").format(self.version)
+        v_msg = _('Version of %(prog)s: {}').format(self.version)
         general_group.add_argument(
-            "-V", '--version', action='version', version=v_msg,
+            '-V', '--version', action='version', version=v_msg,
             help=_("Show program's version number and exit.")
         )
 
     # -------------------------------------------------------------------------
     def init_arg_parser(self):
         """
         Initialise the argument parser - the public available method.
@@ -805,45 +800,45 @@
 
     # -------------------------------------------------------------------------
     def countdown(self, number=5, delay=1, prompt=None):
         """Perform a countdown at the console."""
         if prompt:
             prompt = str(prompt).strip()
         if not prompt:
-            prompt = _("Starting in:")
+            prompt = _('Starting in:')
         prompt = self.colored(prompt, 'YELLOW')
 
         try:
             if not self.force:
                 i = number
-                out = self.colored("%d" % (i), 'RED')
+                out = self.colored('%d' % (i), 'RED')
                 msg = '\n{p} {o}'.format(p=prompt, o=out)
                 sys.stdout.write(msg)
                 sys.stdout.flush()
                 while i > 0:
                     sys.stdout.write(' ')
                     sys.stdout.flush()
                     time.sleep(delay)
                     i -= 1
-                    out = self.colored("{}".format(i), 'RED')
+                    out = self.colored('{}'.format(i), 'RED')
                     sys.stdout.write(out)
                     sys.stdout.flush()
-                sys.stdout.write("\n")
+                sys.stdout.write('\n')
                 sys.stdout.flush()
         except KeyboardInterrupt:
-            sys.stderr.write("\n")
-            LOG.warning(_("Aborted by user interrupt."))
+            sys.stderr.write('\n')
+            LOG.warning(_('Aborted by user interrupt.'))
             sys.exit(99)
 
         go = self.colored('Go go go ...', 'GREEN')
-        sys.stdout.write("\n%s\n\n" % (go))
+        sys.stdout.write('\n%s\n\n' % (go))
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/argparse_actions.py` & `fb_tools-2.2.3/lib/fb_tools/argparse_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a collection of useful argparse actions.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import argparse
-import re
-import os
 import logging
+import os
+import re
 
 try:
     from pathlib import Path
 except ImportError:
     from pathlib2 import Path
 
 # Own modules
 
 from . import MAX_TIMEOUT
 from .xlate import XLATOR
 
-__version__ = '2.1.2'
+__version__ = '2.1.3'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class RegexOptionAction(argparse.Action):
@@ -51,15 +51,15 @@
         """Parse the regular expression option."""
         try:
             if self._re_options is None:
                 re_test = re.compile(pattern)                               # noqa
             else:
                 re_test = re.compile(pattern, self._re_options)             # noqa
         except Exception as e:
-            msg = _("Got a {c} for pattern {p!r}: {e}").format(
+            msg = _('Got a {c} for pattern {p!r}: {e}').format(
                 c=e.__class__.__name__, p=pattern, e=e)
             raise argparse.ArgumentError(self, msg)
 
         setattr(namespace, self.dest, pattern)
 
 # =============================================================================
 class DirectoryOptionAction(argparse.Action):
@@ -77,33 +77,33 @@
             option_strings=option_strings, *args, **kwargs)
 
     # -------------------------------------------------------------------------
     def __call__(self, parser, namespace, given_path, option_string=None):
         """Parse the directory option."""
         path = Path(given_path)
         if not path.is_absolute():
-            msg = _("The path {!r} must be an absolute path.").format(given_path)
+            msg = _('The path {!r} must be an absolute path.').format(given_path)
             raise argparse.ArgumentError(self, msg)
 
         if self.must_exists:
 
             if not path.exists():
-                msg = _("The directory {!r} does not exists.").format(str(path))
+                msg = _('The directory {!r} does not exists.').format(str(path))
                 raise argparse.ArgumentError(self, msg)
 
             if not path.is_dir():
-                msg = _("The given path {!r} exists, but is not a directory.").format(str(path))
+                msg = _('The given path {!r} exists, but is not a directory.').format(str(path))
                 raise argparse.ArgumentError(self, msg)
 
             if not os.access(str(path), os.R_OK) or not os.access(str(path), os.X_OK):
-                msg = _("The given directory {!r} is not readable.").format(str(path))
+                msg = _('The given directory {!r} is not readable.').format(str(path))
                 raise argparse.ArgumentError(self, msg)
 
             if self.writeable and not os.access(str(path), os.W_OK):
-                msg = _("The given directory {!r} is not writeable.").format(str(path))
+                msg = _('The given directory {!r} is not writeable.').format(str(path))
                 raise argparse.ArgumentError(self, msg)
 
         setattr(namespace, self.dest, path)
 
 
 # =============================================================================
 class LogFileOptionAction(argparse.Action):
@@ -123,31 +123,31 @@
             return
 
         path = Path(values)
         logdir = path.parent
 
         # Checking the parent directory of the Logfile
         if not logdir.exists():
-            msg = _("Directory {!r} does not exists.").format(str(logdir))
+            msg = _('Directory {!r} does not exists.').format(str(logdir))
             raise argparse.ArgumentError(self, msg)
         if not logdir.is_dir():
-            msg = _("Path {!r} exists, but is not a directory.").format(str(logdir))
+            msg = _('Path {!r} exists, but is not a directory.').format(str(logdir))
             raise argparse.ArgumentError(self, msg)
 
         # Checking logfile, if it is already existing
         if path.exists():
             if not path.is_file():
-                msg = _("File {!r} is not a regular file.").format(values)
+                msg = _('File {!r} is not a regular file.').format(values)
                 raise argparse.ArgumentError(self, msg)
             if not os.access(values, os.W_OK):
-                msg = _("File {!r} is not writeable.").format(values)
+                msg = _('File {!r} is not writeable.').format(values)
                 raise argparse.ArgumentError(self, msg)
         else:
             if not os.access(logdir, os.W_OK):
-                msg = _("Directory {!r} is not writeable.").format(str(logdir))
+                msg = _('Directory {!r} is not writeable.').format(str(logdir))
                 raise argparse.ArgumentError(self, msg)
 
         setattr(namespace, self.dest, path.resolve())
 
 
 # =============================================================================
 class CfgFileOptionAction(argparse.Action):
@@ -164,18 +164,18 @@
         """Parse the configuration file option."""
         if values is None:
             setattr(namespace, self.dest, None)
             return
 
         path = Path(values)
         if not path.exists():
-            msg = _("File {!r} does not exists.").format(values)
+            msg = _('File {!r} does not exists.').format(values)
             raise argparse.ArgumentError(self, msg)
         if not path.is_file():
-            msg = _("File {!r} is not a regular file.").format(values)
+            msg = _('File {!r} is not a regular file.').format(values)
             raise argparse.ArgumentError(self, msg)
 
         setattr(namespace, self.dest, path.resolve())
 
 
 # =============================================================================
 class TimeoutOptionAction(argparse.Action):
@@ -191,27 +191,27 @@
     # -------------------------------------------------------------------------
     def __call__(self, parser, namespace, given_timeout, option_string=None):
         """Parse the timeout option."""
         try:
             timeout = int(given_timeout)
             if timeout <= 0 or timeout > self.max_timeout:
                 msg = _(
-                    "A timeout must be greater than zero and less "
-                    "or equal to {}.").format(self.max_timeout)
+                    'A timeout must be greater than zero and less '
+                    'or equal to {}.').format(self.max_timeout)
                 raise ValueError(msg)
         except (ValueError, TypeError) as e:
-            msg = _("Wrong timeout {!r}:").format(given_timeout)
+            msg = _('Wrong timeout {!r}:').format(given_timeout)
             msg += ' ' + str(e)
             raise argparse.ArgumentError(self, msg)
 
         setattr(namespace, self.dest, timeout)
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/cfg_app.py` & `fb_tools-2.2.3/lib/fb_tools/cfg_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,40 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for the application object with support for configuration files.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2022 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import os
 import logging
-
+import os
 from logging.handlers import WatchedFileHandler
-
 from pathlib import Path
 
 # Third party modules
 # import six
 
 # Own modules
 
 from . import __version__ as __pkg_version__
-
 from .app import BaseApplication
-
+from .argparse_actions import CfgFileOptionAction
+from .argparse_actions import LogFileOptionAction
 # from .error import FbCfgAppError
-
 from .common import pp, to_bool
-
-from .argparse_actions import LogFileOptionAction
-
-from .argparse_actions import CfgFileOptionAction
-
-from .multi_config import UTF8_ENCODING, DEFAULT_ENCODING
-from .multi_config import MultiConfigError, BaseMultiConfig
-
+from .multi_config import BaseMultiConfig, MultiConfigError
+from .multi_config import DEFAULT_ENCODING, UTF8_ENCODING
 from .xlate import XLATOR
 
-__version__ = '2.2.0'
+__version__ = '2.2.1'
 LOG = logging.getLogger(__name__)
 
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
@@ -57,15 +48,15 @@
             usage=None, description=None, cfg_class=BaseMultiConfig,
             argparse_epilog=None, argparse_prefix_chars='-', env_prefix=None,
             append_appname_to_stems=True, config_dir=None, additional_stems=None,
             additional_cfgdirs=None, cfg_encoding=DEFAULT_ENCODING,
             use_chardet=True, initialized=False):
         """Initialise a FbConfigApplication object."""
         if not issubclass(cfg_class, BaseMultiConfig):
-            msg = _("Parameter {cls!r} must be a subclass of {clinfo!r}.").format(
+            msg = _('Parameter {cls!r} must be a subclass of {clinfo!r}.').format(
                 cls='cfg_class', clinfo='BaseMultiConfig')
             raise TypeError(msg)
 
         self.cfg = None
         self._use_chardet = True
         self.use_chardet = use_chardet
         self._additional_cfg_file = None
@@ -139,34 +130,34 @@
     def init_arg_parser(self):
         """
         Initiate the argument parser.
 
         This method should be explicitely called by all init_arg_parser()
         methods in descendant classes.
         """
-        title = _("Config options and options for logging")
+        title = _('Config options and options for logging')
         cfg_options = self.arg_parser.add_argument_group(title)
 
         cfg_options.add_argument(
-            "-C", "--cfgfile", "--cfg-file", "--config",
-            metavar=_("FILE"), dest="cfg_file", action=CfgFileOptionAction,
-            help=_("Configuration files to use additional to the standard configuration files."),
+            '-C', '--cfgfile', '--cfg-file', '--config',
+            metavar=_('FILE'), dest='cfg_file', action=CfgFileOptionAction,
+            help=_('Configuration files to use additional to the standard configuration files.'),
         )
 
         cfg_options.add_argument(
-            "--logfile", "--log",
-            metavar=_("FILE"), dest="logfile", action=LogFileOptionAction,
-            help=_("A logfile for storing all logging output."),
+            '--logfile', '--log',
+            metavar=_('FILE'), dest='logfile', action=LogFileOptionAction,
+            help=_('A logfile for storing all logging output.'),
         )
 
     # -------------------------------------------------------------------------
     def perform_arg_parser(self):
         """Parse the commnd line parameters."""
         if self.verbose > 2:
-            LOG.debug(_("Got command line arguments:") + '\n' + pp(self.args))
+            LOG.debug(_('Got command line arguments:') + '\n' + pp(self.args))
 
         if self.args.cfg_file:
             self._additional_cfg_file = self.args.cfg_file
             if self.cfg:
                 self.cfg.additional_cfg_file = self.args.cfg_file
 
         if self.args.logfile:
@@ -196,15 +187,15 @@
             additional_stems=self._additional_stems, additional_cfgdirs=self._additional_cfgdirs,
             encoding=self._cfg_encoding, use_chardet=self.use_chardet, initialized=True)
 
         try:
             self.cfg.read()
             self.cfg.eval()
         except MultiConfigError as e:
-            msg = _("Error on reading configuration:") + ' ' + str(e)
+            msg = _('Error on reading configuration:') + ' ' + str(e)
             LOG.error(msg)
             self.exit(4)
         if self.cfg.verbose > self.verbose:
             self.verbose = self.cfg.verbose
 
         if self.cfg.prompt_timeout is not None:
             self.prompt_timeout = self.cfg.prompt_timeout
@@ -221,39 +212,39 @@
         if not self.logfile:
             return
 
         logdir = self.logfile.parent
 
         # Checking the parent directory of the Logfile
         if not logdir.exists():
-            msg = _("Directory {!r} does not exists.").format(str(logdir))
+            msg = _('Directory {!r} does not exists.').format(str(logdir))
             LOG.error(msg)
             self.exit(6)
         if not logdir.is_dir():
-            msg = _("Path {!r} exists, but is not a directory.").format(str(logdir))
+            msg = _('Path {!r} exists, but is not a directory.').format(str(logdir))
             LOG.error(msg)
             self.exit(6)
 
         # Checking logfile, if it is already existing
         if self.logfile.exists():
             if not self.logfile.is_file():
-                msg = _("File {!r} is not a regular file.").format(str(self.logfile))
+                msg = _('File {!r} is not a regular file.').format(str(self.logfile))
                 LOG.error(msg)
                 self.exit(6)
             if not os.access(self.logfile, os.W_OK):
-                msg = _("File {!r} is not writeable.").format(self.logfile)
+                msg = _('File {!r} is not writeable.').format(self.logfile)
                 LOG.error(msg)
                 self.exit(6)
         else:
             if not os.access(logdir, os.W_OK):
-                msg = _("Directory {!r} is not writeable.").format(str(logdir))
+                msg = _('Directory {!r} is not writeable.').format(str(logdir))
                 LOG.error(msg)
                 self.exit(6)
 
-        LOG.debug(_("Start logging into file {!r} ...").format(str(self.logfile)))
+        LOG.debug(_('Start logging into file {!r} ...').format(str(self.logfile)))
 
         log_level = logging.INFO
         if self.verbose:
             log_level = logging.DEBUG
 
         root_logger = logging.getLogger()
         format_str = '[%(asctime)s]: ' + self.appname + ': %(levelname)s - %(message)s'
@@ -264,14 +255,14 @@
         lh_file.setFormatter(formatter)
 
         root_logger.addHandler(lh_file)
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/collections.py` & `fb_tools-2.2.3/lib/fb_tools/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,40 +3,37 @@
 """
 @summary: This module implements specialized container datatypes.
 
 They are providing alternatives to Python's general purpose built-in frozen_set, set and dict.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 
 try:
-    from collections.abc import Set, MutableSet
     from collections.abc import Mapping, MutableMapping
+    from collections.abc import MutableSet, Set
 except ImportError:
-    from collections import Set, MutableSet
     from collections import Mapping, MutableMapping
+    from collections import MutableSet, Set
 
 # Third party modules
 
 # Own modules
-from .errors import FbError
-
 from .common import is_sequence
-
+from .errors import FbError
 from .obj import FbGenericBaseObject
-
 from .xlate import XLATOR
 
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
@@ -56,15 +53,15 @@
         self.item = item
         self.expected = expected
         super(WrongItemTypeError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = _("Item {item!r} must be of type {must!r}, but is of type {cls!r} instead.")
+        msg = _('Item {item!r} must be of type {must!r}, but is of type {cls!r} instead.')
         return msg.format(item=self.item, must=self.expected, cls=self.item.__class__.__name__)
 
 
 # =============================================================================
 class WrongCompareSetClassError(TypeError, FbCollectionsError):
     """Exeception class for the case, that a given class ist not of an instance of CIStringSet."""
 
@@ -74,15 +71,15 @@
         self.other_class = other.__class__.__name__
         self.expected = expected
         super(WrongCompareSetClassError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = _("Object {o!r} is not a {e} object.")
+        msg = _('Object {o!r} is not a {e} object.')
         return msg.format(o=self.other_class, e=self.expected)
 
 
 # =============================================================================
 class WrongKeyTypeError(TypeError, FbCollectionsError):
     """Exeception if a given key is from wrong type."""
 
@@ -92,15 +89,15 @@
         self.key = key
         self.expected = expected
         super(WrongKeyTypeError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = _("Key {key!r} must be of type {must!r}, but is of type {cls!r} instead.")
+        msg = _('Key {key!r} must be of type {must!r}, but is of type {cls!r} instead.')
         return msg.format(key=self.key, must=self.expected, cls=self.key.__class__.__name__)
 
 
 # =============================================================================
 class WrongUpdateClassError(TypeError, FbCollectionsError):
     """Exeception if an object for update is from the wrong type."""
 
@@ -110,17 +107,17 @@
         self.other_class = other.__class__.__name__
         super(WrongUpdateClassError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
         msg = _(
-            "Object is neither a {m} object, nor a sequential object, "
-            "but a {o!r} object instead.")
-        return msg.format(o=self.other_class, m="Mapping")
+            'Object is neither a {m} object, nor a sequential object, '
+            'but a {o!r} object instead.')
+        return msg.format(o=self.other_class, m='Mapping')
 
 
 # =============================================================================
 class CaseInsensitiveKeyError(KeyError, FbCollectionsError):
     """Exeception, if a key was not found."""
 
     # -------------------------------------------------------------------------
@@ -128,15 +125,15 @@
         """Initialise a CaseInsensitiveKeyError exception."""
         self.key = key
         super(CaseInsensitiveKeyError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = _("Key {!r} is not existing.")
+        msg = _('Key {!r} is not existing.')
         return msg.format(self.key)
 
 
 # =============================================================================
 class CIInitfromSequenceError(TypeError, FbCollectionsError):
     """Exeception if an object for update is from the wrong type."""
 
@@ -147,15 +144,15 @@
         self.emesg = emesg
         self.expected = expected
         super(CIInitfromSequenceError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = _("Could update {ex} with {i!r}: {m}")
+        msg = _('Could update {ex} with {i!r}: {m}')
         return msg.format(ex=self.expected, i=self.item, m=self.emesg)
 
 
 # =============================================================================
 class CIInitfromTupleError(IndexError, FbCollectionsError):
     """Exeception if an object for update is from the wrong type."""
 
@@ -166,15 +163,15 @@
         self.emesg = emesg
         self.expected = expected
         super(CIInitfromTupleError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = _("Could update {ex} with {i!r}: {m}")
+        msg = _('Could update {ex} with {i!r}: {m}')
         return msg.format(ex=self.expected, i=self.item, m=self.emesg)
 
 
 # =============================================================================
 class FrozenCIStringSet(Set, FbGenericBaseObject):
     """
     An immutable set, where the items are insensitive strings.
@@ -190,15 +187,15 @@
         if iterable is not None:
             ok = False
             if is_sequence(iterable):
                 ok = True
             elif isinstance(iterable, FrozenCIStringSet):
                 ok = True
             if not ok:
-                msg = _("Parameter {p!r} is not a sequence type, but a {c!r} object instead.")
+                msg = _('Parameter {p!r} is not a sequence type, but a {c!r} object instead.')
                 msg = msg.format(p='iterable', c=iterable.__class__.__qualname__)
                 raise TypeError(msg)
 
             for item in iterable:
 
                 if not isinstance(item, str):
                     raise WrongItemTypeError(item)
@@ -363,20 +360,20 @@
         """Return all values as a list."""
         return self.as_list()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into string."""
         if len(self) == 0:
-            return "{}()".format(self.__class__.__name__)
+            return '{}()'.format(self.__class__.__name__)
 
-        ret = "{}(".format(self.__class__.__name__)
+        ret = '{}('.format(self.__class__.__name__)
         if len(self):
             ret += '['
-            ret += ', '.join(map(lambda x: "{!r}".format(x), self.values()))
+            ret += ', '.join(map(lambda x: '{!r}'.format(x), self.values()))        # noqa: C417
             ret += ']'
         ret += ')'
 
         return ret
 
     # -------------------------------------------------------------------------
     def __repr__(self):
@@ -676,15 +673,15 @@
             else:
                 raise KeyError(value)
 
     # -------------------------------------------------------------------------
     def pop(self):
         """Remove and return an arbitrary element from the set."""
         if len(self) == 0:
-            raise IndexError("pop() from empty list")
+            raise IndexError('pop() from empty list')
 
         key = self._items.keys()[0]
         value = self._items[key]
         del self._items[key]
 
         return value
 
@@ -705,15 +702,15 @@
 
     # -------------------------------------------------------------------------
     def __init__(self, first_param=None, **kwargs):
         """Initialise a FrozenCIDict object.
 
         Use the object dict.
         """
-        self._map = dict()
+        self._map = {}
 
         if first_param is not None:
 
             # LOG.debug("First parameter type {t!r}: {p!r}".format(
             #     t=type(first_param), p=first_param))
 
             if isinstance(first_param, Mapping):
@@ -804,20 +801,20 @@
         """Return the the nuber of entries (keys) in this dict."""
         return len(self._map)
 
     # -------------------------------------------------------------------------
     def __repr__(self):
         """Typecast into string for reproduction."""
         if len(self) == 0:
-            return "{}()".format(self.__class__.__name__)
+            return '{}()'.format(self.__class__.__name__)
 
-        ret = "{}({{".format(self.__class__.__name__)
+        ret = '{}({{'.format(self.__class__.__name__)
         kargs = []
         for pair in self.items():
-            arg = "{k!r}: {v!r}".format(k=pair[0], v=pair[1])
+            arg = '{k!r}: {v!r}'.format(k=pair[0], v=pair[1])
             kargs.append(arg)
         ret += ', '.join(kargs)
         ret += '})'
 
         return ret
 
     # -------------------------------------------------------------------------
@@ -846,15 +843,15 @@
             else:
                 val = pair[1]
             res[pair[0]] = val
 
         return res
 
     # -------------------------------------------------------------------------
-    def dict(self):
+    def dict(self):                                                     # noqa: A003
         """Typecast into a regular dict."""
         return self.as_dict(pure=True)
 
     # -------------------------------------------------------------------------
     def real_key(self, key):
         """Return the original notation of the given key."""
         if not isinstance(key, str):
@@ -882,15 +879,15 @@
         if key.lower() in self._map:
             return True
         return False
 
     # -------------------------------------------------------------------------
     def keys(self):
         """Return a list with all keys in original notation."""
-        return list(map(lambda x: self._map[x]['key'], sorted(self._map.keys())))
+        return list(map(lambda x: self._map[x]['key'], sorted(self._map.keys())))   # noqa: C417
 
     # -------------------------------------------------------------------------
     def items(self):
         """Return a list of all items of the current dict.
 
         An item is a tuple, with the key in original notation and the value.
         """
@@ -902,15 +899,15 @@
             item_list.append((key, value))
 
         return item_list
 
     # -------------------------------------------------------------------------
     def values(self):
         """Return a list with all values of the current dict."""
-        return list(map(lambda x: self._map[x]['val'], sorted(self._map.keys())))
+        return list(map(lambda x: self._map[x]['val'], sorted(self._map.keys())))   # noqa: C417
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
         """Return the equality of current dict with another (the '=='-operator)."""
         if not isinstance(other, FrozenCIDict):
             return False
 
@@ -972,15 +969,15 @@
         lkey = key.lower()
         self._map[lkey] = {
             'key': key,
             'val': value,
         }
 
     # -------------------------------------------------------------------------
-    def set(self, key, value):
+    def set(self, key, value):                                          # noqa: A003
         """Set the value of the given key."""
         self[key] = value
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
         """Delete the entry on the given key.
 
@@ -1001,15 +998,15 @@
     # -------------------------------------------------------------------------
     def pop(self, key, *args):
         """Remove and return an arbitrary element from the dict."""
         if not isinstance(key, str):
             raise WrongKeyTypeError(key)
 
         if len(args) > 1:
-            msg = _("The method {met}() expected at most {max} arguments, got {got}.").format(
+            msg = _('The method {met}() expected at most {max} arguments, got {got}.').format(
                 met='pop', max=2, got=(len(args) + 1))
             raise TypeError(msg)
 
         lkey = key.lower()
         if lkey not in self._map:
             if args:
                 return args[0]
@@ -1031,15 +1028,15 @@
         value = self[key]
         del self._map[lkey]
         return (key, value)
 
     # -------------------------------------------------------------------------
     def clear(self):
         """Remove all items from the dict."""
-        self._map = dict()
+        self._map = {}
 
     # -------------------------------------------------------------------------
     def setdefault(self, key, default=None):
         """Set the item of the given key to a default value."""
         if not isinstance(key, str):
             raise WrongKeyTypeError(key)
 
@@ -1060,14 +1057,14 @@
             self._update_from_sequence(other)
         else:
             WrongUpdateClassError(other)
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/common.py` & `fb_tools-2.2.3/lib/fb_tools/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for common used functions.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 
 # Standard modules
-import sys
-import os
+import datetime
+import ipaddress
+import locale
 import logging
-import re
-import pprint
+import os
 import platform
-import locale
-import string
+import pprint
 import random
-import datetime
-import ipaddress
+import re
+import string
+import sys
 try:
     import pathlib
 except ImportError:
     import pathlib2 as pathlib
 
 try:
     from collections.abc import Sequence
@@ -33,15 +33,15 @@
 # Third party modules
 import six
 
 # Own modules
 
 from .xlate import XLATOR
 
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 
 _ = XLATOR.gettext
 
 LOG = logging.getLogger(__name__)
 
 RE_YES = re.compile(r'^\s*(?:y(?:es)?|true)\s*$', re.IGNORECASE)
 RE_NO = re.compile(r'^\s*(?:no?|false|off)\s*$', re.IGNORECASE)
@@ -138,32 +138,32 @@
     if cur_term:
         if cur_term == 'ansi':
             env_term_has_colors = True
             ansi_term = True
         elif re_term.search(cur_term):
             env_term_has_colors = True
     if debug:
-        sys.stderr.write("ansi_term: {a!r}, env_term_has_colors: {h!r}\n".format(
+        sys.stderr.write('ansi_term: {a!r}, env_term_has_colors: {h!r}\n'.format(
             a=ansi_term, h=env_term_has_colors))
 
     has_colors = False
     if env_term_has_colors:
         has_colors = True
     for handle in [sys.stdout, sys.stderr]:
-        if (hasattr(handle, "isatty") and handle.isatty()):
+        if (hasattr(handle, 'isatty') and handle.isatty()):
             if debug:
-                msg = _("{} is a tty.").format(handle.name)
+                msg = _('{} is a tty.').format(handle.name)
                 sys.stderr.write(msg + '\n')
             if (platform.system() == 'Windows' and not ansi_term):
                 if debug:
-                    sys.stderr.write(_("Platform is Windows and not ansi_term.") + "\n")
+                    sys.stderr.write(_('Platform is Windows and not ansi_term.') + '\n')
                 has_colors = False
         else:
             if debug:
-                msg = _("{} is not a tty.").format(handle.name)
+                msg = _('{} is not a tty.').format(handle.name)
                 sys.stderr.write(msg + '\n')
             if ansi_term:
                 pass
             else:
                 has_colors = False
 
     return has_colors
@@ -304,15 +304,15 @@
 
 # =============================================================================
 def is_sequence(arg):
     """Return, whether the given value is a sequential object, but nat a str."""
     if not isinstance(arg, Sequence):
         return False
 
-    if hasattr(arg, "strip"):
+    if hasattr(arg, 'strip'):
         return False
 
     return True
 
 
 # =============================================================================
 def caller_search_path(*additional_paths):
@@ -546,15 +546,15 @@
     @type as_float: bool
 
     @return: amount of MibiBytes
     @rtype:  int or float
 
     """
     if value is None:
-        msg = _("Given value is {!r}.").format(None)
+        msg = _('Given value is {!r}.').format(None)
         raise ValueError(msg)
 
     radix = '.'
     radix = re.escape(radix)
 
     c_radix = locale.nl_langinfo(locale.RADIXCHAR)
     global CUR_RADIX
@@ -585,15 +585,15 @@
     value_raw = ''
     unit = None
     match = H2MB_RE.search(value)
     if match is not None:
         value_raw = match.group(1)
         unit = match.group(2)
     else:
-        msg = _("Could not determine bytes in {!r}.").format(value)
+        msg = _('Could not determine bytes in {!r}.').format(value)
         raise ValueError(msg)
 
     if CUR_THOUSEP:
         value_raw = THOUSEP_RE.sub('', value_raw)
     if CUR_RADIX != '.':
         value_raw = RADIX_RE.sub('.', value_raw)
     value_float = float(value_raw)
@@ -626,15 +626,15 @@
     mbytes = lbytes / final_factor
     if as_float:
         return float(mbytes)
     if mbytes <= sys.maxsize:
         return int(mbytes)
     return mbytes
     if mbytes != int(mbytes):
-        raise ValueError("int {integer!r} != long {long!r}.".format(
+        raise ValueError('int {integer!r} != long {long!r}.'.format(
             integer=int(mbytes), long=mbytes))
 
     mbytes = int(mbytes)
 
     return mbytes
 
 
@@ -765,26 +765,26 @@
     return format_str.format(value=value_str, unit=unit)
 
 
 # =============================================================================
 def generate_password(length=12):
     """Generate a string of random characters with the givlen length."""
     characters = string.ascii_letters + string.punctuation + string.digits
-    password = "".join(random.choice(characters) for x in range(length))
+    password = ''.join(random.choice(characters) for x in range(length))
     return password
 
 
 # =============================================================================
 def get_monday(day):
     """Return the last Monday before the given date.
 
     If the given date is a Monday itself, then this date will be returned.
     """
     if not isinstance(day, (datetime.date, datetime.datetime)):
-        msg = _("Argument {a!r} must be of type {t1!r} or {t2!r}.").format(
+        msg = _('Argument {a!r} must be of type {t1!r} or {t2!r}.').format(
             a=day, t1='datetime.date', t2='datetime.datetime')
         raise TypeError(msg)
 
     # copy of day as datetime.date
     monday = datetime.date(day.year, day.month, day.day)
     # date is Monday => date.weekday() == 0
     if monday.weekday() == 0:
@@ -841,14 +841,14 @@
             lines.append(line)
 
     return ''.join(lines)
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/config.py` & `fb_tools-2.2.3/lib/fb_tools/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: A module for providing a configuration.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard module
-import logging
 import codecs
-
+import logging
+from configparser import Error as ConfigParseError
 try:
     import pathlib
 except ImportError:
     import pathlib2 as pathlib
 
 # Third party modules
 import six
-
 from six import StringIO
 from six.moves import configparser
 
-from configparser import Error as ConfigParseError
-
 # Own modules
 from .errors import FbError
-
 from .obj import FbBaseObject
-
 from .xlate import XLATOR
 
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 LOG = logging.getLogger(__name__)
 DEFAULT_ENCODING = 'utf-8'
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
@@ -95,16 +90,16 @@
         """Return the encoding used to read config files."""
         return self._encoding
 
     @encoding.setter
     def encoding(self, value):
         if not isinstance(value, str):
             msg = _(
-                "Encoding {v!r} must be a {s!r} object, "
-                "but is a {c!r} object instead.").format(
+                'Encoding {v!r} must be a {s!r} object, '
+                'but is a {c!r} object instead.').format(
                 v=value, s='str', c=value.__class__.__name__)
             raise TypeError(msg)
 
         encoder = codecs.lookup(value)
         self._encoding = encoder.name
 
     # -------------------------------------------------------------------------
@@ -112,15 +107,15 @@
     def config_dir(self):
         """Return the directory containing the configuration."""
         return self._config_dir
 
     @config_dir.setter
     def config_dir(self, value):
         if value is None:
-            raise TypeError(_("A configuration directory may not be None."))
+            raise TypeError(_('A configuration directory may not be None.'))
         cdir = pathlib.Path(value)
         if cdir.exists():
             self._config_dir = cdir.resolve()
         else:
             self._config_dir = cdir
 
     # -------------------------------------------------------------------------
@@ -128,28 +123,28 @@
     def config_file(self):
         """Return the configuration file."""
         return self._config_file
 
     @config_file.setter
     def config_file(self, value):
         if value is None:
-            raise TypeError(_("A configuration file may not be None."))
+            raise TypeError(_('A configuration file may not be None.'))
 
         cfile = pathlib.Path(value)
         if cfile.exists():
             if not cfile.is_file():
-                msg = _("Configuration file {!r} exists, but is not a regular file.").format(
+                msg = _('Configuration file {!r} exists, but is not a regular file.').format(
                     str(cfile))
                 raise ConfigError(msg)
             self._config_file = cfile.resolve()
             return
         cfile = self.config_dir.joinpath(cfile)
         if cfile.exists():
             if not cfile.is_file():
-                msg = _("Configuration file {!r} exists, but is not a regular file.").format(
+                msg = _('Configuration file {!r} exists, but is not a regular file.').format(
                     str(cfile))
                 raise ConfigError(msg)
             self._config_file = cfile.resolve()
             return
         self._config_file = cfile
 
     # -------------------------------------------------------------------------
@@ -171,43 +166,43 @@
 
         return res
 
     # -------------------------------------------------------------------------
     def read(self, error_if_not_exists=False):
         """Read the configuration file."""
         if self.verbose > 2:
-            LOG.debug(_("Searching for {!r} ...").format(self.config_file))
+            LOG.debug(_('Searching for {!r} ...').format(self.config_file))
         if not self.config_file.exists():
-            msg = _("Configuration file {!r} not found.").format(str(self.config_file))
+            msg = _('Configuration file {!r} not found.').format(str(self.config_file))
             if error_if_not_exists:
-                self.handle_error(msg, _("Configuration file error"))
+                self.handle_error(msg, _('Configuration file error'))
             else:
                 LOG.debug(msg)
             return
 
         open_opts = {}
         if six.PY3 and self.encoding:
             open_opts['encoding'] = self.encoding
             open_opts['errors'] = 'surrogateescape'
 
         if self.verbose > 1:
-            LOG.debug(_("Reading {!r} ...").format(self.config_file))
+            LOG.debug(_('Reading {!r} ...').format(self.config_file))
 
         config = configparser.ConfigParser()
         try:
             with open(str(self.config_file), 'r', **open_opts) as fh:
-                stream = StringIO("[default]\n" + fh.read())
+                stream = StringIO('[default]\n' + fh.read())
                 if six.PY2:
                     config.readfp(stream)
                 else:
                     config.read_file(stream)
         except ConfigParseError as e:
-            msg = _("Wrong configuration in {!r} found").format(str(self.config_file))
+            msg = _('Wrong configuration in {!r} found').format(str(self.config_file))
             msg += ': ' + str(e)
-            self.handle_error(msg, _("Configuration parse error"))
+            self.handle_error(msg, _('Configuration parse error'))
             return
 
         self.eval_config(config)
 
     # -------------------------------------------------------------------------
     def eval_config(self, config):
         """Evaluate all found configuration options."""
@@ -222,15 +217,15 @@
     # -------------------------------------------------------------------------
     def eval_config_global(self, config, section_name):
         """Evaluate section [global] of configuration.
 
         May be overridden in descendant classes.
         """
         if self.verbose > 1:
-            LOG.debug(_("Checking config section {!r} ...").format(section_name))
+            LOG.debug(_('Checking config section {!r} ...').format(section_name))
 
         for (key, value) in config.items(section_name):
             if key.lower() == 'verbose':
                 val = int(value)
                 if val > self.verbose:
                     self.verbose = val
 
@@ -241,14 +236,14 @@
         Should be overridden in descendant classes.
         """
         pass
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/ddns/__init__.py` & `fb_tools-2.2.3/lib/fb_tools/ddns/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,48 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The base module for all DDNS related classes.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
-import logging
 import copy
-import sys
-import socket
 import errno
-import os
 import ipaddress
+import json
+import logging
+import os
 import re
+import socket
+import sys
+from json import JSONDecodeError
 
 # Third party modules
 import requests
-import urllib3
-import json
 
-from json import JSONDecodeError
+import urllib3
 
 # Own modules
-from .. import __version__ as GLOBAL_VERSION
+from .config import DdnsConfiguration
 from .. import DDNS_CFG_BASENAME
-
-from ..errors import IoTimeoutError
-
-from ..xlate import XLATOR, format_list
-
-from ..common import pp
-
-from ..argparse_actions import DirectoryOptionAction
-
+from .. import __version__ as GLOBAL_VERSION
 from ..app import BaseApplication
-
 from ..argparse_actions import CfgFileOptionAction
-
+from ..argparse_actions import DirectoryOptionAction
+from ..common import pp
 from ..errors import FbAppError
+from ..errors import IoTimeoutError
+from ..xlate import XLATOR, format_list
 
-from .config import DdnsConfiguration
-
-__version__ = '2.0.2'
+__version__ = '2.0.3'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class DdnsAppError(FbAppError):
@@ -69,15 +61,15 @@
         self.code = code
         self.content = content
         self.url = url
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into a string."""
-        msg = _("Got an error {c} on requesting {u!r}: {m}").format(
+        msg = _('Got an error {c} on requesting {u!r}: {m}').format(
             c=self.code, u=self.url, m=self.content)
         return msg
 
 # =============================================================================
 class WorkDirError(DdnsAppError):
     """Special exception class with problems with the working directory."""
 
@@ -88,56 +80,56 @@
 class WorkDirNotExistsError(WorkDirError, FileNotFoundError):
     """Special exception class, if working diretory does not exists."""
 
     # -------------------------------------------------------------------------
     def __init__(self, workdir):
         """Construct a WorkDirNotExistsError object."""
         super(WorkDirNotExistsError, self).__init__(
-            errno.ENOENT, _("Directory does not exists"), str(workdir))
+            errno.ENOENT, _('Directory does not exists'), str(workdir))
 
 
 # =============================================================================
 class WorkDirNotDirError(WorkDirError, NotADirectoryError):
     """Special exception class, if path to working diretory is not a directory."""
 
     # -------------------------------------------------------------------------
     def __init__(self, workdir):
         """Construct a WorkDirNotDirError object."""
         super(WorkDirNotDirError, self).__init__(
-            errno.ENOTDIR, _("Path is not a directory"), str(workdir))
+            errno.ENOTDIR, _('Path is not a directory'), str(workdir))
 
 
 # =============================================================================
 class WorkDirAccessError(WorkDirError, PermissionError):
     """Special exception class, if working diretory is not accessible."""
 
     # -------------------------------------------------------------------------
     def __init__(self, workdir, msg=None):
         """Construct a WorkDirAccessError object."""
         if not msg:
-            msg = _("Invalid permissions")
+            msg = _('Invalid permissions')
 
         super(WorkDirAccessError, self).__init__(errno.EACCES, msg, str(workdir))
 
 
 # =============================================================================
 class BaseDdnsApplication(BaseApplication):
     """Class for the application objects."""
 
-    library_name = "ddns-client"
+    library_name = 'ddns-client'
     loglevel_requests_set = False
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=GLOBAL_VERSION, base_dir=None,
             initialized=False, usage=None, description=None,
             argparse_epilog=None, argparse_prefix_chars='-', env_prefix=None):
         """Construct a BaseDdnsApplication object."""
         if description is None:
-            description = _("This is a base DDNS related application.")
+            description = _('This is a base DDNS related application.')
 
         self._cfg_dir = None
         self._cfg_file = None
         self.config = None
         self._user_agent = '{}/{}'.format(self.library_name, GLOBAL_VERSION)
 
         super(BaseDdnsApplication, self).__init__(
@@ -165,15 +157,15 @@
     def user_agent(self):
         """Return the name of the user agent used in API calls."""
         return self._user_agent
 
     @user_agent.setter
     def user_agent(self, value):
         if value is None or str(value).strip() == '':
-            raise DdnsAppError(_("Invalid user agent {!r} given.").format(value))
+            raise DdnsAppError(_('Invalid user agent {!r} given.').format(value))
         self._user_agent = str(value).strip()
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
         Transform the elements of the object into a dict.
 
@@ -205,31 +197,31 @@
         protocol_group = ddns_group.add_mutually_exclusive_group()
 
         ipv4_help = getattr(self, '_ipv4_help', None)
         ipv6_help = getattr(self, '_ipv6_help', None)
         proto_help = getattr(self, '_proto_help', None)
 
         if ipv4_help is None:
-            ipv4_help = _("Perform action only for {}.").format('IPv4')
+            ipv4_help = _('Perform action only for {}.').format('IPv4')
 
         if ipv6_help is None:
-            ipv6_help = _("Perform action only for {}.").format('IPv6')
+            ipv6_help = _('Perform action only for {}.').format('IPv6')
 
         if proto_help is None:
             proto_help = _(
-                "The IP protocol, for which the action should be performed "
-                "(one of {c}, default {d!r}).").format(
+                'The IP protocol, for which the action should be performed '
+                '(one of {c}, default {d!r}).').format(
                     c=format_list(valid_list, do_repr=True, style='or'), d='any')
 
         protocol_group.add_argument(
-            '-4', '--ipv4', dest='ipv4', action="store_true", help=ipv4_help,
+            '-4', '--ipv4', dest='ipv4', action='store_true', help=ipv4_help,
         )
 
         protocol_group.add_argument(
-            '-6', '--ipv6', dest='ipv6', action="store_true", help=ipv6_help,
+            '-6', '--ipv6', dest='ipv6', action='store_true', help=ipv6_help,
         )
 
         protocol_group.add_argument(
             '-p', '--protocol', dest='protocol', metavar=_('PROTOCOL'),
             choices=valid_list, help=proto_help,
         )
 
@@ -238,29 +230,29 @@
         if self.appname == 'update-ddns':
             dir_must_exists = True
             writeable = True
         ddns_group.add_argument(
             '-d', '--dir', '--work-directory', dest='directory', metavar=_('DIRECTORY'),
             action=DirectoryOptionAction, must_exists=dir_must_exists, writeable=writeable,
             help=_(
-                "The directory, where to read and write the cache files of the "
-                "evaluated IP addresses (default: {!r}).").format(
+                'The directory, where to read and write the cache files of the '
+                'evaluated IP addresses (default: {!r}).').format(
                 str(DdnsConfiguration.default_working_dir)),
         )
 
         ddns_group.add_argument(
             '-T', '--timeout', dest='timeout', type=int, metavar=_('SECONDS'),
-            help=_("The timeout in seconds for Web requests (default: {}).").format(
+            help=_('The timeout in seconds for Web requests (default: {}).').format(
                 DdnsConfiguration.default_timeout),
         )
 
         ddns_group.add_argument(
             '-c', '--config', '--config-file', dest='cfg_file', metavar=_('FILE'),
             action=CfgFileOptionAction,
-            help=_("Configuration file (default: {!r})").format(str(default_cfg_file))
+            help=_('Configuration file (default: {!r})').format(str(default_cfg_file))
         )
 
     # -------------------------------------------------------------------------
     def post_init(self):
         """
         Execute actions after init and befor the underlaying run.
 
@@ -289,15 +281,15 @@
 
         self.config.read()
         if self.config.verbose > self.verbose:
             self.verbose = self.config.verbose
         self.config.initialized = True
 
         if self.verbose > 3:
-            LOG.debug("Read configuration:\n{}".format(pp(self.config.as_dict())))
+            LOG.debug('Read configuration:\n{}'.format(pp(self.config.as_dict())))
 
         if self.args.ipv4:
             self.config.protocol = 'ipv4'
         elif self.args.ipv6:
             self.config.protocol = 'ipv6'
         elif self.args.protocol:
             if self.args.protocol == 'both':
@@ -305,115 +297,115 @@
             else:
                 self.config.protocol = self.args.protocol
 
         if self.args.timeout:
             try:
                 self.config.timeout = self.args.timeout
             except (ValueError, KeyError) as e:
-                msg = _("Invalid value {!r} as timeout:").format(self.args.timeout) + ' ' + str(e)
+                msg = _('Invalid value {!r} as timeout:').format(self.args.timeout) + ' ' + str(e)
                 LOG.error(msg)
                 print()
                 self.arg_parser.print_usage(sys.stdout)
                 self.exit(1)
 
         if self.args.directory:
             self.config.working_dir = self.args.directory
 
         if not self.loglevel_requests_set:
-            msg = _("Setting Loglevel of the {m} module to {ll}.").format(
+            msg = _('Setting Loglevel of the {m} module to {ll}.').format(
                 m='requests', ll='WARNING')
             LOG.debug(msg)
-            logging.getLogger("requests").setLevel(logging.WARNING)
+            logging.getLogger('requests').setLevel(logging.WARNING)
             self.loglevel_requests_set = True
 
         self.initialized = True
 
     # -------------------------------------------------------------------------
     def get_my_ipv(self, protocol):
         """Retrieve the current public IPv64 address."""
-        LOG.debug(_("Trying to get my public IPv{} address.").format(protocol))
+        LOG.debug(_('Trying to get my public IPv{} address.').format(protocol))
 
         url = self.config.get_ipv4_url
         if protocol == 6:
             url = self.config.get_ipv6_url
 
         try:
             json_response = self.perform_request(url)
         except DdnsAppError as e:
             LOG.error(str(e))
             return None
         if self.verbose > 0:
-            LOG.debug(_("Got a response:") + '\n' + pp(json_response))
+            LOG.debug(_('Got a response:') + '\n' + pp(json_response))
 
         return json_response['IP']
 
     # -------------------------------------------------------------------------
     def perform_request(self, url, method='GET', data=None, headers=None, may_simulate=False):
         """Perform the underlying Web request."""
         if headers is None:
-            headers = dict()
+            headers = {}
 
         if self.verbose > 1:
-            LOG.debug(_("Request method: {!r}").format(method))
+            LOG.debug(_('Request method: {!r}').format(method))
 
         if data and self.verbose > 1:
-            data_out = "{!r}".format(data)
+            data_out = '{!r}'.format(data)
             try:
                 data_out = json.loads(data)
             except ValueError:
                 pass
             else:
                 data_out = pp(data_out)
-            LOG.debug("Data:\n{}".format(data_out))
+            LOG.debug('Data:\n{}'.format(data_out))
             if self.verbose > 2:
-                LOG.debug("RAW data:\n{}".format(data))
+                LOG.debug('RAW data:\n{}'.format(data))
 
         headers.update({'User-Agent': self.user_agent})
         headers.update({'Content-Type': 'application/json'})
         if self.verbose > 1:
-            LOG.debug("Headers:\n{}".format(pp(headers)))
+            LOG.debug('Headers:\n{}'.format(pp(headers)))
 
         if may_simulate and self.simulate:
-            LOG.debug(_("Simulation mode, Request will not be sent."))
+            LOG.debug(_('Simulation mode, Request will not be sent.'))
             return ''
 
         try:
 
             session = requests.Session()
             response = session.request(
                 method, url, data=data, headers=headers, timeout=self.config.timeout)
 
         except (
                 socket.timeout, urllib3.exceptions.ConnectTimeoutError,
                 urllib3.exceptions.MaxRetryError, requests.exceptions.ConnectionError,
                 requests.exceptions.ConnectTimeout) as e:
-            msg = _("Got a {c} on requesting {u!r}: {e}.").format(
+            msg = _('Got a {c} on requesting {u!r}: {e}.').format(
                 c=e.__class__.__name__, u=url, e=e)
             raise DdnsAppError(msg)
 
         try:
             self._eval_response(url, response)
         except ValueError:
             raise DdnsAppError(_('Failed to parse the response'), response.text)
 
         if self.verbose > 3:
-            LOG.debug("RAW response: {!r}.".format(response.text))
+            LOG.debug('RAW response: {!r}.'.format(response.text))
         if not response.text:
             return ''
 
         try:
             json_response = response.json()
         except JSONDecodeError:
             if self.verbose > 2:
                 LOG.debug("Setting encoding of response to 'utf-8-sig'.")
             response.encoding = 'utf-8-sig'
             json_response = response.json()
 
         if self.verbose > 3:
-            LOG.debug("JSON response:\n{}".format(pp(json_response)))
+            LOG.debug('JSON response:\n{}'.format(pp(json_response)))
 
         return json_response
 
     # -------------------------------------------------------------------------
     def _eval_response(self, url, response):
 
         if response.ok:
@@ -425,30 +417,30 @@
         raise DdnsRequestError(code, msg, url)
 
     # -------------------------------------------------------------------------
     def verify_working_dir(self):
         """Verify existence and accessibility of working directory."""
         if self.verbose > 1:
             LOG.debug(_(
-                "Checking existence and accessibility of working directory {!r} ...").format(
+                'Checking existence and accessibility of working directory {!r} ...').format(
                 str(self.config.working_dir)))
 
         if not self.config.working_dir.exists():
             raise WorkDirNotExistsError(self.config.working_dir)
 
         if not self.config.working_dir.is_dir():
             raise WorkDirNotDirError(self.config.working_dir)
 
         if not os.access(str(self.config.working_dir), os.R_OK):
             raise WorkDirAccessError(
-                self.config.working_dir, _("No read access"))
+                self.config.working_dir, _('No read access'))
 
         if not os.access(str(self.config.working_dir), os.W_OK):
             raise WorkDirAccessError(
-                self.config.working_dir, _("No write access"))
+                self.config.working_dir, _('No write access'))
 
     # -------------------------------------------------------------------------
     def write_ipv4_cache(self, address):
         """Write the cache for IPv4 addresses."""
         self.write_ip_cache(address, self.config.ipv4_cache_file)
 
     # -------------------------------------------------------------------------
@@ -456,15 +448,15 @@
         """Write the cache for IPv6 addresses."""
         self.write_ip_cache(address, self.config.ipv6_cache_file)
 
     # -------------------------------------------------------------------------
     def write_ip_cache(self, address, cache_file):
         """Write a cache entry."""
         LOG.debug(_(
-            "Writing IP address {a!r} into {f!r} ...").format(
+            'Writing IP address {a!r} into {f!r} ...').format(
                 a=str(address), f=str(cache_file)))
         cont = str(address) + '\n'
         try:
             self.write_file(filename=str(cache_file), content=cont, must_exists=False, quiet=True)
         except (IOError, IoTimeoutError) as e:
             LOG.error(str(e))
             if self.exit_value <= 1:
@@ -483,18 +475,18 @@
     # -------------------------------------------------------------------------
     def get_ip_cache(self, cache_file):
         """Return a common IP address entry."""
         re_comment = re.compile(r'^\s*[;#]')
 
         if not cache_file.exists():
             if self.verbose > 2:
-                LOG.debug(_("File {!r} not found.").format(cache_file))
+                LOG.debug(_('File {!r} not found.').format(cache_file))
             return None
 
-        LOG.debug(_("Reading IP address from {!r}...").format(str(cache_file)))
+        LOG.debug(_('Reading IP address from {!r}...').format(str(cache_file)))
         has_errors = False
         try:
             cont = self.read_file(str(cache_file), quiet=True)
         except (IOError, IoTimeoutError) as e:
             LOG.error(str(e))
             has_errors = True
 
@@ -506,28 +498,28 @@
                 if not line:
                     continue
                 if re_comment.match(line):
                     continue
                 try:
                     addr = ipaddress.ip_address(line)
                 except ValueError as e:
-                    msg = _("Line {li!r} in {f!r} is not a valid IP address:").format(
+                    msg = _('Line {li!r} in {f!r} is not a valid IP address:').format(
                         li=line, f=str(cache_file)) + ' ' + str(e)
                     LOG.error(msg)
                     continue
                 address = addr
                 break
             return address
 
         if self.exit_value <= 1:
             self.exit_value = 5
         return None
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/ddns/config.py` & `fb_tools-2.2.3/lib/fb_tools/ddns/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: A module for providing a configuration for the ddns-update script.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard module
 import logging
 import re
-
 try:
     from pathlib import Path
 except ImportError:
     from pathlib2 import Path
 
 # Third party modules
 
 # Own modules
 from ..common import to_bool
-
-from ..config import ConfigError, BaseConfiguration
-
+from ..config import BaseConfiguration, ConfigError
 from ..xlate import XLATOR, format_list
 
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
@@ -98,15 +95,15 @@
     @timeout.setter
     def timeout(self, value):
         if value is None:
             self._timeout = self.default_timeout
             return
         val = int(value)
         err_msg = _(
-            "Invalid timeout {!r} for Web requests, must be 0 < SECONDS < 3600.")
+            'Invalid timeout {!r} for Web requests, must be 0 < SECONDS < 3600.')
         if val <= 0 or val > 3600:
             msg = err_msg.format(value)
             raise ValueError(msg)
         self._timeout = val
 
     # -------------------------------------------------------------------------
     @property
@@ -166,21 +163,21 @@
             return
 
         if section_name.lower() == 'files':
             self._eval_config_files(config, section_name)
             return
 
         if self.verbose > 1:
-            LOG.debug("Unhandled configuration section {!r}.".format(section_name))
+            LOG.debug('Unhandled configuration section {!r}.'.format(section_name))
 
     # -------------------------------------------------------------------------
     def _eval_config_ddns(self, config, section_name):
 
         if self.verbose > 1:
-            LOG.debug("Checking config section {!r} ...".format(section_name))
+            LOG.debug('Checking config section {!r} ...'.format(section_name))
 
         re_domains = re.compile(r'[,;\s]+')
         re_all_domains = re.compile(r'^all[_-]?domains$', re.IGNORECASE)
         re_with_mx = re.compile(r'^\s*with[_-]?mx\s*$', re.IGNORECASE)
         re_get_url = re.compile(r'^\s*get[_-]?ipv([46])[_-]?url\s*$', re.IGNORECASE)
         re_upd_url = re.compile(r'^\s*upd(?:ate)?[_-]?ipv([46])[_-]?url\s*$', re.IGNORECASE)
 
@@ -203,83 +200,83 @@
             elif re_with_mx.match(key) and value.strip():
                 self.with_mx = to_bool(value.strip())
                 continue
             elif key.lower() == 'timeout':
                 try:
                     self.timeout = value
                 except (ValueError, KeyError) as e:
-                    msg = _("Invalid value {!r} as timeout:").format(value) + ' ' + str(e)
+                    msg = _('Invalid value {!r} as timeout:').format(value) + ' ' + str(e)
                     LOG.error(msg)
                 continue
             match = re_get_url.match(key)
             if match and value.strip():
                 setattr(self, 'get_ipv{}_url'.format(match.group(1)), value.strip())
                 continue
             match = re_upd_url.match(key)
             if match and value.strip():
                 setattr(self, 'upd_ipv{}_url'.format(match.group(1)), value.strip())
                 continue
             if key.lower() == 'protocol' and value.strip():
                 p = value.strip().lower()
                 if p not in self.valid_protocols:
                     LOG.error(_(
-                        "Invalid value {ur} for protocols to update, valid protocols "
-                        "are: ").format(value) + format_list(self.valid_protocols, do_repr=True))
+                        'Invalid value {ur} for protocols to update, valid protocols '
+                        'are: ').format(value) + format_list(self.valid_protocols, do_repr=True))
                 else:
                     if p == 'both':
                         p = 'any'
                     self.protocol = p
                 continue
 
             LOG.warning(_(
-                "Unknown configuration option {o!r} with value {v!r} in "
-                "section {s!r}.").format(o=key, v=value, s=section_name))
+                'Unknown configuration option {o!r} with value {v!r} in '
+                'section {s!r}.').format(o=key, v=value, s=section_name))
 
         return
 
     # -------------------------------------------------------------------------
     def _eval_config_files(self, config, section_name):
 
         if self.verbose > 1:
-            LOG.debug("Checking config section {!r} ...".format(section_name))
+            LOG.debug('Checking config section {!r} ...'.format(section_name))
 
         re_work_dir = re.compile(r'^\s*work(ing)?[_-]?dir(ectory)?\ſ*', re.IGNORECASE)
         re_logfile = re.compile(r'^\s*log[_-]?file\s*$', re.IGNORECASE)
 
         for (key, value) in config.items(section_name):
 
             if re_work_dir.match(key) and value.strip():
                 p = Path(value.strip())
                 if p.is_absolute():
                     self.working_dir = p
                 else:
                     LOG.error(_(
-                        "The path to the working directory must be an absolute path "
-                        "(given: {!r}).").format(value))
+                        'The path to the working directory must be an absolute path '
+                        '(given: {!r}).').format(value))
                 continue
 
             if re_logfile.match(key) and value.strip():
                 p = Path(value.strip())
                 if p.is_absolute():
                     self.logfile = p
                 else:
                     LOG.error(_(
-                        "The path to the logfile must be an absolute path "
-                        "(given: {!r}).").format(value))
+                        'The path to the logfile must be an absolute path '
+                        '(given: {!r}).').format(value))
                 continue
 
             LOG.warning(_(
-                "Unknown configuration option {o!r} with value {v!r} in "
-                "section {s!r}.").format(o=key, v=value, s=section_name))
+                'Unknown configuration option {o!r} with value {v!r} in '
+                'section {s!r}.').format(o=key, v=value, s=section_name))
 
         return
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/ddns/myip_app.py` & `fb_tools-2.2.3/lib/fb_tools/ddns/myip_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for the classes of the myip application.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
-import logging
 import copy
+import logging
 
 # Own modules
-from .. import __version__ as GLOBAL_VERSION
-
-from ..xlate import XLATOR, format_list
-
-from ..common import to_bool
-
 from . import BaseDdnsApplication, WorkDirError
-
 from .config import DdnsConfiguration
+from .. import __version__ as GLOBAL_VERSION
+from ..common import to_bool
+from ..xlate import XLATOR, format_list
 
-__version__ = '2.0.3'
+__version__ = '2.0.4'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 # =============================================================================
 class MyIpApplication(BaseDdnsApplication):
     """Class for the application objects."""
@@ -44,23 +40,23 @@
             initialized=False, usage=None, description=None,
             argparse_epilog=None, argparse_prefix_chars='-', env_prefix=None):
         """Initialise a MyIpApplication object."""
         self._write_ips = False
 
         if description is None:
             description = _(
-                "Tries to detect the public NAT IPv4 address and/or the automatic assigned "
-                "IPv6 address in a local network and print it out.")
+                'Tries to detect the public NAT IPv4 address and/or the automatic assigned '
+                'IPv6 address in a local network and print it out.')
         valid_proto_list = copy.copy(DdnsConfiguration.valid_protocols)
 
-        self._ipv4_help = _("Use only {} to retreive the public IP address.").format('IPv4')
-        self._ipv6_help = _("Use only {} to retreive the public IP address.").format('IPv6')
+        self._ipv4_help = _('Use only {} to retreive the public IP address.').format('IPv4')
+        self._ipv6_help = _('Use only {} to retreive the public IP address.').format('IPv6')
         self._proto_help = _(
-            "The IP protocol, for which the public IP should be retrieved (one of {c}, default "
-            "{d!r}).").format(c=format_list(valid_proto_list, do_repr=True, style='or'), d='any')
+            'The IP protocol, for which the public IP should be retrieved (one of {c}, default '
+            '{d!r}).').format(c=format_list(valid_proto_list, do_repr=True, style='or'), d='any')
 
         super(MyIpApplication, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir,
             description=description, initialized=False,
         )
 
         self.initialized = True
@@ -95,16 +91,16 @@
     def init_arg_parser(self):
         """Initiate th eargument parser."""
         super(MyIpApplication, self).init_arg_parser()
 
         myip_group = self.arg_parser.add_argument_group(_('myip options'))
 
         myip_group.add_argument(
-            '-W', "--write", "--write-ips", action="store_true", dest="write_ips",
-            help=_("Write found public IPs into a cache file in working directory.")
+            '-W', '--write', '--write-ips', action='store_true', dest='write_ips',
+            help=_('Write found public IPs into a cache file in working directory.')
         )
 
     # -------------------------------------------------------------------------
     def post_init(self):
         """Execute some actions before calling run().
 
         Here could be done some finishing actions after reading in
@@ -127,15 +123,15 @@
         """Execute some actions after parsing the command line parameters."""
         if self.args.write_ips:
             self.write_ips = True
 
     # -------------------------------------------------------------------------
     def _run(self):
 
-        LOG.debug(_("Starting {a!r}, version {v!r} ...").format(
+        LOG.debug(_('Starting {a!r}, version {v!r} ...').format(
             a=self.appname, v=self.version))
 
         if self.config.protocol in ('any', 'both', 'ipv4'):
             self.print_my_ipv(4)
         if self.config.protocol in ('any', 'both', 'ipv6'):
             self.print_my_ipv(6)
 
@@ -149,14 +145,14 @@
                 if protocol == 4:
                     self.write_ipv4_cache(my_ip)
                 else:
                     self.write_ipv6_cache(my_ip)
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/ddns/update_app.py` & `fb_tools-2.2.3/lib/fb_tools/ddns/update_app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for the classes of the update-ddns application.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
-import logging
 import copy
-import sys
-import os
 import ipaddress
-
+import logging
+import os
+import sys
 try:
     from pathlib import Path
 except ImportError:
     from pathlib2 import Path
 
 # Third party module
-from six.moves.urllib.parse import quote
-
-# Own modules
 from fb_logging.colored import ColoredFormatter
 
-from .. import __version__ as GLOBAL_VERSION
-
-from ..xlate import XLATOR, format_list
+from six.moves.urllib.parse import quote
 
+# Own modules
 from . import BaseDdnsApplication, WorkDirError
-from . import WorkDirNotExistsError, WorkDirNotDirError, WorkDirAccessError
-
+from . import WorkDirAccessError, WorkDirNotDirError, WorkDirNotExistsError
 from .config import DdnsConfiguration
+from .. import __version__ as GLOBAL_VERSION
+from ..xlate import XLATOR, format_list
 
-__version__ = '2.0.2'
+__version__ = '2.0.3'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class UpdateDdnsApplication(BaseDdnsApplication):
@@ -59,27 +55,27 @@
         """Initialise a UpdateDdnsApplication object."""
         self.last_ipv4_address = None
         self.last_ipv6_address = None
         self.current_ipv4_address = None
         self.current_ipv6_address = None
         self.txt_records = []
 
-        self._force_desc_msg = _("Updating the DDNS records, even if seems not to be changed.")
+        self._force_desc_msg = _('Updating the DDNS records, even if seems not to be changed.')
 
         if description is None:
             description = _(
-                "Tries to update the A and/or AAAA record at ddns.de with the current "
-                "IP address.")
+                'Tries to update the A and/or AAAA record at ddns.de with the current '
+                'IP address.')
         valid_proto_list = copy.copy(DdnsConfiguration.valid_protocols)
 
-        self._ipv4_help = _("Update only the {} record with the public IP address.").format('A')
-        self._ipv6_help = _("Update only the {} record with the public IP address.").format('AAAA')
+        self._ipv4_help = _('Update only the {} record with the public IP address.').format('A')
+        self._ipv6_help = _('Update only the {} record with the public IP address.').format('AAAA')
         self._proto_help = _(
-            "The IP protocol, for which the appropriate DNS record should be updated with the "
-            "public IP (one of {c}, default {d!r}).").format(c=format_list(
+            'The IP protocol, for which the appropriate DNS record should be updated with the '
+            'public IP (one of {c}, default {d!r}).').format(c=format_list(
                 valid_proto_list, do_repr=True, style='or'), d='any')
 
         super(UpdateDdnsApplication, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir,
             description=description, initialized=False,
         )
 
@@ -152,28 +148,28 @@
         if not logfile:
             return
 
         logdir = logfile.parent
 
         if self.verbose > 1:
             LOG.debug(_(
-                "Checking existence and accessibility of log directory {!r} ...").format(
+                'Checking existence and accessibility of log directory {!r} ...').format(
                 str(logdir)))
 
         if not logdir.exists():
             raise WorkDirNotExistsError(logdir)
 
         if not logdir.is_dir():
             raise WorkDirNotDirError(logdir)
 
         if not os.access(str(logdir), os.R_OK):
-            raise WorkDirAccessError(logdir, _("No read access"))
+            raise WorkDirAccessError(logdir, _('No read access'))
 
         if not os.access(str(logdir), os.W_OK):
-            raise WorkDirAccessError(logdir, _("No write access"))
+            raise WorkDirAccessError(logdir, _('No write access'))
 
         root_log = logging.getLogger()
         formatter = self._get_log_formatter(is_term=False)
 
         lh_file = logging.FileHandler(str(logfile), mode='a', encoding='utf-8', delay=True)
         if self.verbose:
             lh_file.setLevel(logging.DEBUG)
@@ -186,38 +182,38 @@
     def init_arg_parser(self):
         """Initiate the argument parser."""
         super(UpdateDdnsApplication, self).init_arg_parser()
 
         update_group = self.arg_parser.add_argument_group(_('Update DDNS options'))
 
         update_group.add_argument(
-            '-U', "--user", metavar=_('USER'), dest="user",
-            help=_("The username to login at ddns.de.")
+            '-U', '--user', metavar=_('USER'), dest='user',
+            help=_('The username to login at ddns.de.')
         )
 
         update_group.add_argument(
-            '-P', "--password", metavar=_('PASSWORD'), dest="password",
-            help=_("The password of the user to login at ddns.de.")
+            '-P', '--password', metavar=_('PASSWORD'), dest='password',
+            help=_('The password of the user to login at ddns.de.')
         )
 
         update_group.add_argument(
-            '--logfile', nargs='?', metavar=_('FILENAME'), dest="logfile", const='',
-            help=_("The filename to use as a logfile. Leave it empty to disable file logging."),
+            '--logfile', nargs='?', metavar=_('FILENAME'), dest='logfile', const='',
+            help=_('The filename to use as a logfile. Leave it empty to disable file logging.'),
         )
 
         domain_group = update_group.add_mutually_exclusive_group()
 
         domain_group.add_argument(
-            '-A', '--all', '--all-domains', action="store_true", dest="all_domains",
-            help=_("Update all domains, which are connected whith the given ddns account."),
+            '-A', '--all', '--all-domains', action='store_true', dest='all_domains',
+            help=_('Update all domains, which are connected whith the given ddns account.'),
         )
 
         domain_group.add_argument(
-            '-D', '--domain', nargs="+", metavar=_("DOMAIN"), dest="domains",
-            help=_("The particular domain(s), which should be updated (if not all).")
+            '-D', '--domain', nargs='+', metavar=_('DOMAIN'), dest='domains',
+            help=_('The particular domain(s), which should be updated (if not all).')
         )
 
     # -------------------------------------------------------------------------
     def post_init(self):
         """
         Execute post-init actions.
 
@@ -227,15 +223,15 @@
         """
         super(UpdateDdnsApplication, self).post_init()
         self.initialized = False
 
         self.perform_arg_parser_late()
 
         if not self.config.all_domains and not self.config.domains:
-            msg = _("No domains to update given, but the option all domains is deactivated.")
+            msg = _('No domains to update given, but the option all domains is deactivated.')
             LOG.error(msg)
             self.exit(6)
 
         try:
             self.init_file_logging()
             self.verify_working_dir()
         except WorkDirError as e:
@@ -268,106 +264,106 @@
             self.config.domains = []
             for domain in self.args.domains:
                 self.config.domains.append(domain)
 
     # -------------------------------------------------------------------------
     def _run(self):
 
-        LOG.info(_("Starting {a!r}, version {v!r} ...").format(
+        LOG.info(_('Starting {a!r}, version {v!r} ...').format(
             a=self.appname, v=self.version))
 
         if self.config.protocol in ('any', 'both', 'ipv4'):
             self.do_update_ipv4()
 
         if self.config.protocol in ('any', 'both', 'ipv6'):
             self.do_update_ipv6()
 
-        LOG.info(_("Ending {a!r}.").format(
+        LOG.info(_('Ending {a!r}.').format(
             a=self.appname, v=self.version))
 
     # -------------------------------------------------------------------------
     def do_update_ipv4(self):
         """Update an IPv4 address entry."""
         last_address = self.get_ipv4_cache()
         if last_address:
-            LOG.debug(_("Last {w} address: {a!r}.").format(w='IPv4', a=str(last_address)))
+            LOG.debug(_('Last {w} address: {a!r}.').format(w='IPv4', a=str(last_address)))
         else:
-            LOG.debug(_("Did not found a last {} address.").format('IPv4'))
+            LOG.debug(_('Did not found a last {} address.').format('IPv4'))
         current_address = self.get_my_ipv(4)
         if not current_address:
-            LOG.error(_("Got no public IPv4 address."))
+            LOG.error(_('Got no public IPv4 address.'))
             return
         try:
             my_ip = ipaddress.ip_address(current_address)
         except ValueError as e:
-            msg = _("Address {a!r} seems not to be a valid {w} address: {e}").format(
+            msg = _('Address {a!r} seems not to be a valid {w} address: {e}').format(
                 a=current_address, w='IP', e=e)
             LOG.error(msg)
             return
         if my_ip.version != 4:
-            msg = _("Address {a!r} seems not to be a valid {w} address.").format(
+            msg = _('Address {a!r} seems not to be a valid {w} address.').format(
                 a=current_address, w='IPv4')
             LOG.error(msg)
             return
 
-        LOG.debug(_("Current {w} address is {a!r}.").format(w='IPv4', a=str(my_ip)))
+        LOG.debug(_('Current {w} address is {a!r}.').format(w='IPv4', a=str(my_ip)))
 
         if last_address == my_ip:
             msg = _(
-                "The public {w} address {a!r} seems not to be changed since "
-                "the last update.").format(w='IPv4', a=str(last_address))
+                'The public {w} address {a!r} seems not to be changed since '
+                'the last update.').format(w='IPv4', a=str(last_address))
             LOG.info(msg)
             if not self.force:
                 return
 
         self.do_update(my_ip, 4)
         self.write_ipv4_cache(my_ip)
 
     # -------------------------------------------------------------------------
     def do_update_ipv6(self):
         """Update an IPv6 address entry."""
         last_address = self.get_ipv6_cache()
         if last_address:
-            LOG.debug(_("Last {w} address: {a!r}.").format(w='IPv6', a=str(last_address)))
+            LOG.debug(_('Last {w} address: {a!r}.').format(w='IPv6', a=str(last_address)))
         else:
-            LOG.debug(_("Did not found a last {} address.").format('IPv6'))
+            LOG.debug(_('Did not found a last {} address.').format('IPv6'))
         current_address = self.get_my_ipv(6)
         if not current_address:
-            LOG.error(_("Got no public IPv6 address."))
+            LOG.error(_('Got no public IPv6 address.'))
             return
         try:
             my_ip = ipaddress.ip_address(current_address)
         except ValueError as e:
-            msg = _("Address {a!r} seems not to be a valid {w} address: {e}").format(
+            msg = _('Address {a!r} seems not to be a valid {w} address: {e}').format(
                 a=current_address, w='IP', e=e)
             LOG.error(msg)
             return
         if my_ip.version != 6:
-            msg = _("Address {a!r} seems not to be a valid {w} address.").format(
+            msg = _('Address {a!r} seems not to be a valid {w} address.').format(
                 a=current_address, w='IPv6')
             LOG.error(msg)
             return
 
-        LOG.debug(_("Current {w} address is {a!r}.").format(w='IPv6', a=str(my_ip)))
+        LOG.debug(_('Current {w} address is {a!r}.').format(w='IPv6', a=str(my_ip)))
 
         if last_address == my_ip:
             msg = _(
-                "The public {w} address {a!r} seems not to be changed since "
-                "the last update.").format(w='IPv6', a=str(last_address))
+                'The public {w} address {a!r} seems not to be changed since '
+                'the last update.').format(w='IPv6', a=str(last_address))
             LOG.info(msg)
             if not self.force:
                 return
 
         self.do_update(my_ip, 6)
         self.write_ipv6_cache(my_ip)
 
     # -------------------------------------------------------------------------
     def do_update(self, my_ip, protocol):
         """Execute the update."""
-        msg = _("Updating DNS records to IPv{p} address {a!r} ...").format(
+        msg = _('Updating DNS records to IPv{p} address {a!r} ...').format(
             p=protocol, a=str(my_ip))
         LOG.info(msg)
 
         url = self.config.upd_ipv4_url
         if protocol == 6:
             url = self.config.upd_ipv6_url
 
@@ -387,22 +383,22 @@
             arg = 'host=' + domains
             args.append(arg)
 
         if self.config.with_mx:
             args.append('mx=1')
 
         url += '?' + '&'.join(args)
-        LOG.debug("Update-URL: {}".format(url))
+        LOG.debug('Update-URL: {}'.format(url))
 
         if self.simulate:
-            LOG.debug("Simulation mode, update will not be sended.")
+            LOG.debug('Simulation mode, update will not be sended.')
             return True
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/errors.py` & `fb_tools-2.2.3/lib/fb_tools/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 @summary: Module for some common used error classes.
 
 @author: Frank Brehm
 """
 
 # Standard modules
 import errno
-import signal
 import os
+import signal
 
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
 class FbError(Exception):
@@ -44,15 +44,15 @@
 # =============================================================================
 class EmptyMailAddressError(BaseMailAddressError):
     """Class for a exception in case of an empty mail address."""
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into a string."""
-        return _("Empty mail address.")
+        return _('Empty mail address.')
 
 
 # =============================================================================
 class InvalidMailAddressError(BaseMailAddressError):
     """Class for a exception in case of a malformed mail address."""
 
     # -------------------------------------------------------------------------
@@ -60,15 +60,15 @@
         """Initialise a InvalidMailAddressError exception."""
         self.address = address
         self.msg = msg
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into a string."""
-        msg = _("Wrong mail address {a!r} ({c})").format(
+        msg = _('Wrong mail address {a!r} ({c})').format(
             a=self.address, c=self.address.__class__.__name__)
         if self.msg:
             msg += ': ' + self.msg
         else:
             msg += '.'
         return msg
 
@@ -136,19 +136,19 @@
     def __init__(self, signum):
         """Initialise a InterruptError exception."""
         self.signum = signum
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into a string."""
-        signame = "{}".format(self.signum)
+        signame = '{}'.format(self.signum)
         if self.signum in self.signal_names:
             signame = self.signal_names[self.signum] + '(' + signame + ')'
 
-        msg = _("Process with PID {pid} got signal {signal}.").format(
+        msg = _('Process with PID {pid} got signal {signal}.').format(
             pid=os.getpid(), signal=signame)
 
         return msg
 
 
 # =============================================================================
 class TerraformObjectError(FbHandlerError):
@@ -179,15 +179,15 @@
     def __init__(self, net_name):
         """Initialise a NetworkNotExistingError exception."""
         self.net_name = net_name
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into a string."""
-        msg = _("The network {!r} is not existing.").format(self.net_name)
+        msg = _('The network {!r} is not existing.').format(self.net_name)
         return msg
 
 
 # =============================================================================
 class FunctionNotImplementedError(FbError, NotImplementedError):
     """Error class for not implemented functions."""
 
@@ -209,15 +209,15 @@
         self.class_name = class_name
         if not class_name:
             self.class_name = '__unkown_class__'
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into a string for error output."""
-        msg = _("Method {func}() has to be overridden in class {cls!r}.")
+        msg = _('Method {func}() has to be overridden in class {cls!r}.')
         return msg.format(func=self.function_name, cls=self.class_name)
 
 
 # =============================================================================
 class IoTimeoutError(FbError, IOError):
     """Special error class indicating a timout error on a read/write operation."""
 
@@ -238,15 +238,15 @@
         try:
             t_o = float(timeout)
         except ValueError:
             pass
         self.timeout = t_o
 
         if t_o is not None:
-            strerror += _(" (timeout after {:0.1f} secs)").format(t_o)
+            strerror += _(' (timeout after {:0.1f} secs)').format(t_o)
 
         if filename is None:
             super(IoTimeoutError, self).__init__(errno.ETIMEDOUT, strerror)
         else:
             super(IoTimeoutError, self).__init__(
                 errno.ETIMEDOUT, strerror, filename)
 
@@ -262,15 +262,15 @@
 
         @param timeout: the timout in seconds leading to the error
         @type timeout: float
         @param filename: the filename leading to the error
         @type filename: str
 
         """
-        strerror = _("Timeout error on reading")
+        strerror = _('Timeout error on reading')
         super(ReadTimeoutError, self).__init__(strerror, timeout, filename)
 
 
 # =============================================================================
 class WriteTimeoutError(IoTimeoutError):
     """Special error class indicating a timout error on a writing into a file."""
 
@@ -281,26 +281,26 @@
 
         @param timeout: the timout in seconds leading to the error
         @type timeout: float
         @param filename: the filename leading to the error
         @type filename: str
 
         """
-        strerror = _("Timeout error on writing")
+        strerror = _('Timeout error on writing')
         super(WriteTimeoutError, self).__init__(strerror, timeout, filename)
 
 
 # =============================================================================
 class TimeoutOnPromptError(AbortAppError, IoTimeoutError):
     """Special exception class on timout on a prompt."""
 
     # -------------------------------------------------------------------------
     def __init__(self, timeout):
         """Initialise a TimeoutOnPromptError exception."""
-        strerror = _("Timeout on answering on the console.")
+        strerror = _('Timeout on answering on the console.')
         super(TimeoutOnPromptError, self).__init__(strerror, timeout)
 
 
 # =============================================================================
 class CommandNotFoundError(HandlerError):
     """Special exception, if one ore more OS commands were not found."""
 
@@ -311,27 +311,27 @@
 
         @param cmd_list: all not found OS commands.
         @type cmd_list: list
 
         """
         self.cmd_list = None
         if cmd_list is None:
-            self.cmd_list = [_("Unknown OS command.")]
+            self.cmd_list = [_('Unknown OS command.')]
         elif isinstance(cmd_list, list):
             self.cmd_list = cmd_list
         else:
             self.cmd_list = [cmd_list]
 
         if len(self.cmd_list) < 1:
-            raise ValueError(_("Empty command list given."))
+            raise ValueError(_('Empty command list given.'))
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into a string for error output."""
-        cmds = ', '.join(map(lambda x: ("'" + str(x) + "'"), self.cmd_list))
+        cmds = ', '.join((("'" + str(x) + "'") for x in self.cmd_list))
         msg = ngettext(
             'Could not found OS command:', 'Could not found OS commands:',
             len(self.cmd_list)) + cmds
 
         return msg
 
 
@@ -361,13 +361,13 @@
         """Typecast into a string for error output."""
         return _("Couldn't occupy lockfile {lf!r} in {d:0.1f} seconds with {tries} tries.").format(
             lf=self.lockfile, d=self.duration, tries=self.tries)
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/get_file_rm_app.py` & `fb_tools-2.2.3/lib/fb_tools/get_file_rm_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for the get-file-to-remove application object.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import logging
-import datetime
 import argparse
+import datetime
 import glob
+import logging
 import re
-import sre_constants
-
 try:
     import pathlib
 except ImportError:
     import pathlib2 as pathlib
 
 # Third party modules
+import sre_constants
 
 # Own modules
-from .xlate import XLATOR
-
-from .errors import FbAppError
-
-from .common import pp, get_monday
-
 from .app import BaseApplication
+from .common import get_monday, pp
+from .errors import FbAppError
+from .xlate import XLATOR
 
-__version__ = '2.0.3'
+__version__ = '2.0.4'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
@@ -59,15 +55,15 @@
         super(KeepOptionAction, self).__init__(
             option_strings=option_strings, *args, **kwargs)
 
     # -------------------------------------------------------------------------
     def __call__(self, parser, namespace, values, option_string=None):
         """Call method on parsing the option."""
         if values < self._min:
-            msg = _("Value must be at least {m} - {v} was given.").format(
+            msg = _('Value must be at least {m} - {v} was given.').format(
                 m=self._min, v=values)
             raise argparse.ArgumentError(self, msg)
 
         setattr(namespace, self.dest, values)
 
 
 # =============================================================================
@@ -101,15 +97,15 @@
         """Initialise a WrongDatePattern exception."""
         self.pattern = pattern
         self.add_info = add_info
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into a string."""
-        msg = _("The given pattern {!r} is not a valid date pattern").format(self.pattern)
+        msg = _('The given pattern {!r} is not a valid date pattern').format(self.pattern)
         if self.add_info:
             msg += ': ' + self.add_info
         else:
             msg += _(". The must be exactly one occurence of '%Y', one of '%m' and one of '%d'.")
         return msg
 
 
@@ -137,17 +133,17 @@
     show_simulate_option = False
 
     # -------------------------------------------------------------------------
     def __init__(
             self, verbose=0, version=__version__, *arg, **kwargs):
         """Initialise of the get-file-to-remove application object."""
         desc = _(
-            "Returns a newline separated list of files generated from file globbing patterns "
-            "given as arguments to this application, where all files are omitted, which "
-            "should not be removed.")
+            'Returns a newline separated list of files generated from file globbing patterns '
+            'given as arguments to this application, where all files are omitted, which '
+            'should not be removed.')
 
         self._keep_days = self.default_keep_days
         self._keep_weeks = self.default_keep_weeks
         self._keep_months = self.default_keep_months
         self._keep_years = self.default_keep_years
         self._keep_last = self.default_keep_last
 
@@ -175,15 +171,15 @@
 
     @keep_days.setter
     def keep_days(self, value):
         v = int(value)
         if v >= self.min_keep_days:
             self._keep_days = v
         else:
-            msg = _("Wrong value {v!r} for {n}, must be >= {m}").format(
+            msg = _('Wrong value {v!r} for {n}, must be >= {m}').format(
                 v=value, n='keep_days', m=self.min_keep_days)
             raise ValueError(msg)
 
     # -----------------------------------------------------------
     @property
     def keep_weeks(self):
         """Return the number of last weeks to keep a file."""
@@ -191,15 +187,15 @@
 
     @keep_weeks.setter
     def keep_weeks(self, value):
         v = int(value)
         if v >= self.min_keep_weeks:
             self._keep_weeks = v
         else:
-            msg = _("Wrong value {v!r} for {n}, must be >= {m}").format(
+            msg = _('Wrong value {v!r} for {n}, must be >= {m}').format(
                 v=value, n='keep_weeks', m=self.min_keep_weeks)
             raise ValueError(msg)
 
     # -----------------------------------------------------------
     @property
     def keep_months(self):
         """Return the number of last months to keep a file."""
@@ -207,15 +203,15 @@
 
     @keep_months.setter
     def keep_months(self, value):
         v = int(value)
         if v >= self.min_keep_months:
             self._keep_months = v
         else:
-            msg = _("Wrong value {v!r} for {n}, must be >= {m}").format(
+            msg = _('Wrong value {v!r} for {n}, must be >= {m}').format(
                 v=value, n='keep_months', m=self.min_keep_months)
             raise ValueError(msg)
 
     # -----------------------------------------------------------
     @property
     def keep_years(self):
         """Return the number of last years to keep a file."""
@@ -223,15 +219,15 @@
 
     @keep_years.setter
     def keep_years(self, value):
         v = int(value)
         if v >= self.min_keep_years:
             self._keep_years = v
         else:
-            msg = _("Wrong value {v!r} for {n}, must be >= {m}").format(
+            msg = _('Wrong value {v!r} for {n}, must be >= {m}').format(
                 v=value, n='keep_years', m=self.min_keep_years)
             raise ValueError(msg)
 
     # -----------------------------------------------------------
     @property
     def keep_last(self):
         """Return the number of last files to keep."""
@@ -239,15 +235,15 @@
 
     @keep_last.setter
     def keep_last(self, value):
         v = int(value)
         if v >= self.min_keep_last:
             self._keep_last = v
         else:
-            msg = _("Wrong value {v!r} for {n}, must be >= {m}").format(
+            msg = _('Wrong value {v!r} for {n}, must be >= {m}').format(
                 v=value, n='keep_last', m=self.min_keep_last)
             raise ValueError(msg)
 
     # -----------------------------------------------------------
     @property
     def date_pattern(self):
         """Return the pattern to extract the date from filename."""
@@ -273,52 +269,52 @@
 
         keep_group = self.arg_parser.add_argument_group(_('Keep options'))
 
         keep_group.add_argument(
             '-L', '--last', metavar=_('NR_FILES'), dest='last', type=int,
             action=KeepOptionAction, min_val=self.min_keep_last,
             help=_(
-                "How many of the last files should be kept "
-                "(default: {default}, minimum: {min})?").format(
+                'How many of the last files should be kept '
+                '(default: {default}, minimum: {min})?').format(
                 default=self.default_keep_last, min=self.min_keep_last),
         )
 
         keep_group.add_argument(
             '-D', '--days', metavar=_('DAYS'), dest='days', type=int,
             action=KeepOptionAction, min_val=self.min_keep_days,
             help=_(
-                "How many files one per day from today on should be kept "
-                "(default: {default}, minimum: {min})?").format(
+                'How many files one per day from today on should be kept '
+                '(default: {default}, minimum: {min})?').format(
                 default=self.default_keep_days, min=self.min_keep_days),
         )
 
         keep_group.add_argument(
             '-W', '--weeks', metavar=_('WEEKS'), dest='weeks', type=int,
             action=KeepOptionAction, min_val=self.min_keep_weeks,
             help=_(
-                "How many files one per week from today on should be kept "
-                "(default: {default}, minimum: {min})?").format(
+                'How many files one per week from today on should be kept '
+                '(default: {default}, minimum: {min})?').format(
                 default=self.default_keep_weeks, min=self.min_keep_weeks),
         )
 
         keep_group.add_argument(
             '-M', '--months', metavar=_('MONTHS'), dest='months', type=int,
             action=KeepOptionAction, min_val=self.min_keep_months,
             help=_(
-                "How many files one per month from today on should be kept "
-                "(default: {default}, minimum: {min})?").format(
+                'How many files one per month from today on should be kept '
+                '(default: {default}, minimum: {min})?').format(
                 default=self.default_keep_months, min=self.min_keep_months),
         )
 
         keep_group.add_argument(
             '-Y', '--years', metavar=_('YEARS'), dest='years', type=int,
             action=KeepOptionAction, min_val=self.min_keep_years,
             help=_(
-                "How many files one per year from today on should be kept "
-                "(default: {default}, minimum: {min})?").format(
+                'How many files one per year from today on should be kept '
+                '(default: {default}, minimum: {min})?').format(
                 default=self.default_keep_years, min=self.min_keep_years),
         )
 
     # -------------------------------------------------------------------------
     def perform_arg_parser(self):
         """Parse the command line options."""
         if self.args.days is not None:
@@ -339,15 +335,15 @@
     # -------------------------------------------------------------------------
     def _xlate_date_pattern(self):
 
         pat = self.date_pattern.strip()
         if not check_date_pattern(pat):
             raise WrongDatePattern(self.date_pattern)
         if self.verbose > 1:
-            LOG.debug(_("Resolving date pattern {!r}.").format(pat))
+            LOG.debug(_('Resolving date pattern {!r}.').format(pat))
 
         self._pattern = pat.replace(
             '%Y', r'(?P<year>\d{4})').replace(
             '%m', r'(?P<month>\d\d?)').replace(
             '%d', r'(?P<day>\d\d?)')
 
         try:
@@ -360,62 +356,62 @@
         """Execute some actions ath the end of the initialisation.."""
         super(GetFileRmApplication, self).post_init()
         self.initialized = False
 
         self._xlate_date_pattern()
 
         if self.verbose > 1:
-            LOG.debug(_("Checking given files..."))
+            LOG.debug(_('Checking given files...'))
 
         for fname in self.args.files:
 
             if self.verbose > 2:
-                LOG.debug(_("Checking given file {!r} ...").format(fname))
+                LOG.debug(_('Checking given file {!r} ...').format(fname))
 
             given_paths = []
             single_fpath = pathlib.Path(fname)
             if single_fpath.exists():
                 given_paths = [single_fpath]
             else:
                 given_paths = glob.glob(fname)
                 if self.verbose > 2:
-                    LOG.debug(_("Resolved paths:") + '\n' + pp(given_paths))
+                    LOG.debug(_('Resolved paths:') + '\n' + pp(given_paths))
                 if not given_paths:
-                    LOG.info(_("File pattern {!r} does not match any files.").format(fname))
+                    LOG.info(_('File pattern {!r} does not match any files.').format(fname))
                     continue
             for f_name in given_paths:
                 fpath = pathlib.Path(f_name)
                 if self.verbose > 2:
-                    LOG.debug(_("Checking {!r} ...").format(fpath))
+                    LOG.debug(_('Checking {!r} ...').format(fpath))
                 if not fpath.exists():
-                    LOG.warning(_("File {!r} does not exists.").format(str(fpath)))
+                    LOG.warning(_('File {!r} does not exists.').format(str(fpath)))
                     continue
                 if fpath.is_file():
                     if self.verbose > 2:
-                        LOG.debug(_("File {!r} is a regular file.").format(str(fpath)))
+                        LOG.debug(_('File {!r} is a regular file.').format(str(fpath)))
                 elif fpath.is_dir():
                     if self.verbose > 2:
-                        LOG.debug(_("Path {!r} is a directory.").format(str(fpath)))
+                        LOG.debug(_('Path {!r} is a directory.').format(str(fpath)))
                 else:
-                    LOG.warning(_("File {!r} is not a regular file.").format(str(fpath)))
+                    LOG.warning(_('File {!r} is not a regular file.').format(str(fpath)))
                     continue
 
                 match = self.re_date.search(str(fpath))
                 if not match:
-                    LOG.warning(_("File {fi!r} does not match pattern {pa!r}.").format(
+                    LOG.warning(_('File {fi!r} does not match pattern {pa!r}.').format(
                         fi=str(fpath), pa=self.date_pattern))
                     continue
 
                 year = int(match.group('year'))
                 month = int(match.group('month'))
                 day = int(match.group('day'))
                 try:
                     fdate = datetime.date(year, month, day)                         # noqa
                 except ValueError as e:
-                    msg = _("Date in file {fi!r} is not a valid date: {e}.").format(
+                    msg = _('Date in file {fi!r} is not a valid date: {e}.').format(
                         fi=str(fpath), e=e)
                     LOG.warning(msg)
                     continue
 
                 fpath_abs = fpath.resolve()
                 if fpath_abs not in self.files_given:
                     self.files_given.append(fpath_abs)
@@ -458,15 +454,15 @@
 
         return res
 
     # -------------------------------------------------------------------------
     def pre_run(self):
         """Execute some actions before calling run()."""
         if not self.files_given:
-            msg = _("Did not found any files to evaluate.")
+            msg = _('Did not found any files to evaluate.')
             LOG.info(msg)
             self.exit(0)
 
     # -------------------------------------------------------------------------
     def _run(self):
         """Run the application."""
         files_assigned = self.get_date_from_filenames()
@@ -490,26 +486,26 @@
             if f not in files_to_keep:
                 files_to_keep.append(f)
         for f in self.get_files_to_keep_day(files_assigned['day']):
             if f not in files_to_keep:
                 files_to_keep.append(f)
 
         if self.keep_last:
-            msg = ngettext("Keeping last file ...", "Keeping last {} files ...", self.keep_last)
+            msg = ngettext('Keeping last file ...', 'Keeping last {} files ...', self.keep_last)
             LOG.debug(msg.format(self.keep_last))
             files = sorted(self.files_given)
             index = self.keep_last * -1
             for f in files[index:]:
                 if self.verbose > 1:
-                    LOG.debug(_("Keep last file {!r}.").format(str(f)))
+                    LOG.debug(_('Keep last file {!r}.').format(str(f)))
                 if f not in files_to_keep:
                     files_to_keep.append(f)
 
         if self.verbose > 2:
-            LOG.debug(_("Files to keep:") + '\n' + pp(files_to_keep))
+            LOG.debug(_('Files to keep:') + '\n' + pp(files_to_keep))
         return files_to_keep
 
     # -------------------------------------------------------------------------
     def get_files_to_keep_year(self, files_assigned):
         """Get all yearly files to keep."""
         files_to_keep = []
 
@@ -522,15 +518,15 @@
                 continue
 
             files = sorted(files_assigned[year_str])
             if len(files) > 0:
                 files_to_keep.append(files[0])
 
         if self.verbose > 2:
-            LOG.debug(_("Files to keep for year:") + '\n' + pp(files_to_keep))
+            LOG.debug(_('Files to keep for year:') + '\n' + pp(files_to_keep))
 
         return files_to_keep
 
     # -------------------------------------------------------------------------
     def get_files_to_keep_month(self, files_assigned):
         """Get all monthly files to keep."""
         files_to_keep = []
@@ -544,87 +540,87 @@
             m = today.month - i
             y = today.year
             while m <= 0:
                 y -= 1
                 m += 12
             last_month = datetime.date(y, m, 1)
             i += 1
-        LOG.debug(_("Got last month: {!r}").format(last_month.strftime('%Y-%m')))
+        LOG.debug(_('Got last month: {!r}').format(last_month.strftime('%Y-%m')))
 
         re_date = re.compile(r'(\d+)-(\d+)')
         for month_str in files_assigned.keys():
             match = re_date.match(month_str)
             this_month = datetime.date(
                 int(match.group(1)), int(match.group(2)), 1)
             if this_month < last_month:
                 continue
             files = sorted(files_assigned[month_str])
             if len(files) > 0:
                 files_to_keep.append(files[0])
 
         if self.verbose > 2:
-            LOG.debug(_("Files to keep for month:") + '\n' + pp(files_to_keep))
+            LOG.debug(_('Files to keep for month:') + '\n' + pp(files_to_keep))
 
         return files_to_keep
 
     # -------------------------------------------------------------------------
     def get_files_to_keep_week(self, files_assigned):
         """Get all weekly files to keep."""
         files_to_keep = []
 
         today = datetime.date.today()
         this_monday = get_monday(today)
         tdelta = datetime.timedelta((self.keep_weeks - 1) * 7)
         last_monday = this_monday - tdelta
 
-        LOG.debug(_("Got last Monday: {!r}").format(last_monday.strftime('%Y-%m-%d')))
+        LOG.debug(_('Got last Monday: {!r}').format(last_monday.strftime('%Y-%m-%d')))
 
         re_date = re.compile(r'(\d+)-(\d+)-(\d+)')
         for day_str in files_assigned.keys():
             match = re_date.match(day_str)
             this_day = datetime.date(
                 int(match.group(1)), int(match.group(2)), int(match.group(3)))
             if this_day < last_monday:
                 continue
             files = sorted(files_assigned[day_str])
             files_to_keep.append(files[0])
 
         if self.verbose > 2:
-            LOG.debug(_("Files to keep for week:") + '\n' + pp(files_to_keep))
+            LOG.debug(_('Files to keep for week:') + '\n' + pp(files_to_keep))
 
         return files_to_keep
 
     # -------------------------------------------------------------------------
     def get_files_to_keep_day(self, files_assigned):
         """Get all daily files to keep."""
         files_to_keep = []
 
         today = datetime.date.today()
         tdelta = datetime.timedelta(self.keep_days - 1)
         last_day = today - tdelta
 
-        LOG.debug(_("Got last day: {!r}").format(last_day.strftime('%Y-%m-%d')))
+        LOG.debug(_('Got last day: {!r}').format(last_day.strftime('%Y-%m-%d')))
 
         re_date = re.compile(r'(\d+)-(\d+)-(\d+)')
         for day_str in files_assigned.keys():
             match = re_date.match(day_str)
             this_day = datetime.date(
                 int(match.group(1)), int(match.group(2)), int(match.group(3)))
             if this_day < last_day:
                 continue
             files = sorted(files_assigned[day_str])
             if this_day == today:
-                LOG.debug(_("Keeping all files from today."))
+                LOG.debug(_('Keeping all files from today.'))
                 for f in files:
                     files_to_keep.append(f)
             elif len(files) > 0:
                 files_to_keep.append(files[0])
 
         if self.verbose > 2:
-            LOG.debug(_("Files to keep for day:") + '\n' + pp(files_to_keep))
+            LOG.debug(_('Files to keep for day:') + '\n' + pp(files_to_keep))
 
         return files_to_keep
 
     # -------------------------------------------------------------------------
     def get_date_from_filenames(self):
         """Evaluate the timestamp from filename."""
         files = {}
@@ -633,26 +629,26 @@
         files['week'] = {}
         files['day'] = {}
 
         for fpath in self.files_given:
 
             fname = str(fpath)
             if self.verbose > 2:
-                LOG.debug(_("Trying to get date of file {!r}.").format(fname))
+                LOG.debug(_('Trying to get date of file {!r}.').format(fname))
 
             match = self.re_date.search(fname)
             if not match:
                 continue
 
             year = int(match.group('year'))
             month = int(match.group('month'))
             day = int(match.group('day'))
             fdate = datetime.date(year, month, day)
             if self.verbose > 2:
-                LOG.debug("Got date {!r}.".format(fdate.isoformat()))
+                LOG.debug('Got date {!r}.'.format(fdate.isoformat()))
 
             y = fdate.strftime('%Y')
             if y not in files['year']:
                 files['year'][y] = []
             if fpath not in files['year'][y]:
                 files['year'][y].append(fpath)
 
@@ -672,19 +668,19 @@
             this_day = fdate.strftime('%Y-%m-%d')
             if this_day not in files['day']:
                 files['day'][this_day] = []
             if fpath not in files['day'][this_day]:
                 files['day'][this_day].append(fpath)
 
         if self.verbose > 1:
-            LOG.debug(_("Explored and assigned files:") + '\n' + pp(files))
+            LOG.debug(_('Explored and assigned files:') + '\n' + pp(files))
         return files
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/handler/__init__.py` & `fb_tools-2.2.3/lib/fb_tools/handler/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,50 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: A base handler module for underlaying actions.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 
 """
 from __future__ import absolute_import, print_function
 
 # Standard module
-import os
+import datetime
+import locale
 import logging
+import os
+import pipes
+import pwd
 import stat
 import subprocess
-import pwd
-import locale
 import time
-import pipes
-import datetime
-from fcntl import fcntl, F_GETFL, F_SETFL
-
+from fcntl import F_GETFL, F_SETFL, fcntl
 try:
     import pathlib
 except ImportError:
     import pathlib2 as pathlib
 
 # Third party modules
-import pytz
-import six
-
 import babel
-
 from babel.dates import LOCALTZ
 
-# Own modules
-from ..xlate import XLATOR
+import pytz
 
-from ..common import to_bool
+import six
 
+# Own modules
+from ..common import to_bool
 from ..errors import HandlerError
+from ..handling_obj import CompletedProcess, HandlingObject
+from ..xlate import XLATOR
 
-from ..handling_obj import HandlingObject, CompletedProcess
-
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 LOG = logging.getLogger(__name__)
 
 CHOWN_CMD = pathlib.Path('/bin/chown')
 ECHO_CMD = pathlib.Path('/bin/echo')
 SUDO_CMD = pathlib.Path('/usr/bin/sudo')
 
 DEFAULT_LOCALE = 'en_US'
@@ -135,16 +131,16 @@
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
         res = super(BaseHandler, self).as_dict(short=short)
-        res['std_file_permissions'] = "{:04o}".format(self.std_file_permissions)
-        res['std_secure_file_permissions'] = "{:04o}".format(self.std_secure_file_permissions)
+        res['std_file_permissions'] = '{:04o}'.format(self.std_file_permissions)
+        res['std_secure_file_permissions'] = '{:04o}'.format(self.std_secure_file_permissions)
         res['open_opts'] = self.open_opts
         res['tz_name'] = self.tz_name
         res['chown_cmd'] = self.chown_cmd
         res['echo_cmd'] = self.echo_cmd
         res['sudo_cmd'] = self.sudo_cmd
         res['sudo'] = self.sudo
         res['default_locale'] = self.default_locale
@@ -152,29 +148,29 @@
         return res
 
     # -------------------------------------------------------------------------
     @classmethod
     def set_tz(cls, tz_name):
         """Set the timezone to the given name."""
         if not tz_name.strip():
-            raise ValueError(_("Invalid time zone name {!r}.").format(tz_name))
+            raise ValueError(_('Invalid time zone name {!r}.').format(tz_name))
         tz_name = tz_name.strip()
-        LOG.debug(_("Setting time zone to {!r}.").format(tz_name))
+        LOG.debug(_('Setting time zone to {!r}.').format(tz_name))
         cls.tz = pytz.timezone(tz_name)
         cls.tz_name = babel.dates.get_timezone_name(
             cls.tz, width='long', locale=cls.default_locale)
-        LOG.debug(_("Name of the time zone: {!r}.").format(cls.tz_name))
+        LOG.debug(_('Name of the time zone: {!r}.').format(cls.tz_name))
 
     # -------------------------------------------------------------------------
     def __call__(self, yaml_file):
         """Execute the underlying action."""
         if not self.initialized:
-            raise HandlerError(_("{}-object not initialized.").format(self.__class__.__name__))
+            raise HandlerError(_('{}-object not initialized.').format(self.__class__.__name__))
 
-        raise HandlerError(_("Method {} must be overridden in descendant classes.").format(
+        raise HandlerError(_('Method {} must be overridden in descendant classes.').format(
             '__call__()'))
 
     # -------------------------------------------------------------------------
     def call(
         self, cmd, sudo=None, simulate=None, quiet=None, shell=False,
             stdout=None, stderr=None, bufsize=0, drop_stderr=False,
             close_fds=False, hb_handler=None, hb_interval=2.0,
@@ -237,21 +233,21 @@
 
         if quiet is None:
             quiet = self.quiet
 
         use_shell = bool(shell)
 
         cmd_list = [str(element) for element in cmd_list]
-        cmd_str = ' '.join(map(lambda x: pipes.quote(x), cmd_list))
+        cmd_str = ' '.join((pipes.quote(x) for x in cmd_list))
 
         if not quiet or self.verbose > 1:
-            LOG.debug(_("Executing: {}").format(cmd_list))
+            LOG.debug(_('Executing: {}').format(cmd_list))
 
         if quiet and self.verbose > 1:
-            LOG.debug(_("Quiet execution."))
+            LOG.debug(_('Quiet execution.'))
 
         used_stdout = subprocess.PIPE
         if stdout is not None:
             used_stdout = stdout
         use_stdout = True
         if used_stdout is None:
             use_stdout = False
@@ -309,35 +305,35 @@
             stdout=stdoutdata, stderr=stderrdata, start_dt=start_dt, end_dt=end_dt)
         return self._eval_call_results(proc, log_output=log_output, quiet=quiet)
 
     # -------------------------------------------------------------------------
     def _eval_call_results(self, proc, log_output=True, quiet=False):
 
         if not isinstance(proc, CompletedProcess):
-            msg = _("Parameter {p!r} is not of type {t!r}.").format(
+            msg = _('Parameter {p!r} is not of type {t!r}.').format(
                 p='proc', t='CompletedProcess')
             raise TypeError(msg)
 
         if self.verbose > 2:
-            LOG.debug(_("Got completed process:") + "\n{}".format(proc))
+            LOG.debug(_('Got completed process:') + '\n{}'.format(proc))
 
         if proc.stderr:
             if not quiet:
-                msg = _("Output on {}:").format('proc.stderr')
+                msg = _('Output on {}:').format('proc.stderr')
                 msg += '\n' + proc.stderr
                 if proc.returncode:
                     LOG.warning(msg)
                 elif log_output:
                     LOG.info(msg)
                 else:
                     LOG.debug(msg)
 
         if proc.stdout:
             if not quiet:
-                msg = _("Output on {}:").format('proc.stdout')
+                msg = _('Output on {}:').format('proc.stdout')
                 msg += '\n' + proc.stdout
                 if log_output:
                     LOG.info(msg)
                 else:
                     LOG.debug(msg)
 
         return proc
@@ -352,67 +348,67 @@
         if six.PY3:
             stdoutdata = bytearray()
             stderrdata = bytearray()
 
         if not quiet or self.verbose > 1:
             LOG.debug(_(
                 "Starting asynchronous communication with '{cmd}', "
-                "heartbeat interval is {interval:0.1f} seconds.").format(
+                'heartbeat interval is {interval:0.1f} seconds.').format(
                     cmd=cmd_str, interval=hb_interval))
 
         out_flags = fcntl(cmd_obj.stdout, F_GETFL)
         err_flags = fcntl(cmd_obj.stderr, F_GETFL)
         fcntl(cmd_obj.stdout, F_SETFL, out_flags | os.O_NONBLOCK)
         fcntl(cmd_obj.stderr, F_SETFL, err_flags | os.O_NONBLOCK)
 
         start_time = time.time()
 
         while True:
 
             if self.verbose > 3:
-                LOG.debug(_("Checking for the end of the communication ..."))
+                LOG.debug(_('Checking for the end of the communication ...'))
             if cmd_obj.poll() is not None:
                 cmd_obj.wait()
                 break
 
             # Heartbeat handling ...
             cur_time = time.time()
             time_diff = cur_time - start_time
             if time_diff >= hb_interval:
                 if not quiet or self.verbose > 1:
-                    LOG.debug(_("Time to execute the heartbeat handler."))
+                    LOG.debug(_('Time to execute the heartbeat handler.'))
                 hb_handler()
                 start_time = cur_time
             if self.verbose > 3:
-                LOG.debug(_("Sleeping {:0.2f} seconds ...").format(poll_interval))
+                LOG.debug(_('Sleeping {:0.2f} seconds ...').format(poll_interval))
             time.sleep(poll_interval)
 
             # Reading out file descriptors
             if use_stdout:
                 try:
                     stdoutdata += os.read(cmd_obj.stdout.fileno(), 1024)
                     if self.verbose > 3:
-                        msg = _("   {w} is now: {o!r}").format(w='stdout', o=stdoutdata)
+                        msg = _('   {w} is now: {o!r}').format(w='stdout', o=stdoutdata)
                         LOG.debug(msg)
                 except OSError:
                     pass
 
             if use_stderr:
                 try:
                     stderrdata += os.read(cmd_obj.stderr.fileno(), 1024)
                     if self.verbose > 3:
-                        msg = _("   {w} is now: {o!r}").format(w='stderr', o=stderrdata)
+                        msg = _('   {w} is now: {o!r}').format(w='stderr', o=stderrdata)
                         LOG.debug(msg)
                 except OSError:
                     pass
 
         return (stdoutdata, stderrdata)
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/handler/lock.py` & `fb_tools-2.2.3/lib/fb_tools/handler/lock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: Module for a extended handler module, which has additional methods for locking.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import sys
-import os
+import datetime
+import errno
+import fcntl
 import logging
+import os
+import sys
 import time
-import errno
 import traceback
-import datetime
-import fcntl
-
+from numbers import Number
 try:
     from pathlib import Path
 except ImportError:
     from pathlib2 import Path
 
-from numbers import Number
-
 # Third party modules
 from six import reraise
 
 # Own modules
+from . import BaseHandler
 from ..common import to_utf8
 from ..errors import CouldntOccupyLockfileError, HandlerError
 from ..obj import FbBaseObject
 from ..xlate import XLATOR
-from . import BaseHandler
 
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 
 LOG = logging.getLogger(__name__)
 
 # Module variables
 DEFAULT_LOCKRETRY_DELAY_START = 0.1
 DEFAULT_LOCKRETRY_DELAY_INCREASE = 0.2
 DEFAULT_LOCKRETRY_MAX_DELAY = 10
@@ -186,29 +184,29 @@
         )
 
         self._simulate = bool(simulate)
         self._autoremove = bool(autoremove)
         self._silent = bool(silent)
 
         if not lockfile:
-            raise LockObjectError(_("No lockfile given on init of a LockObject object."))
+            raise LockObjectError(_('No lockfile given on init of a LockObject object.'))
 
         lfile = Path(lockfile)
 
         if not lfile.exists():
             if self.simulate:
                 LOG.info(_(
                     "Lockfile {!r} doesn't exists, but don't worry, "
                     "it's simulation mode.").format(str(lockfile)))
             else:
                 raise LockObjectError(_("Lockfile {!r} doesn't exists.").format(str(lockfile)))
         else:
             if not lfile.is_file():
                 raise LockObjectError(_(
-                    "Lockfile {!r} is not a regular file.").format(str(lockfile)))
+                    'Lockfile {!r} is not a regular file.').format(str(lockfile)))
 
         if fd is not None:
             self._fd = fd
 
         self._lockfile = lfile.resolve()
 
         self._fcontent = None
@@ -326,53 +324,53 @@
 
     # -------------------------------------------------------------------------
     def __repr__(self):
         """Typecast  the current objectinto a string for reproduction."""
         out = super(LockObject, self).__repr__()[:-2]
 
         fields = []
-        fields.append("lockfile={!r}".format(self.lockfile))
+        fields.append('lockfile={!r}'.format(self.lockfile))
         if self.fcontent:
-            fields.append("fcontent={!r}".format(self.fcontent))
-        fields.append("ctime={!r}".format(self.ctime))
-        fields.append("mtime={!r}".format(self.mtime))
-        fields.append("fcontent={!r}".format(self.fcontent))
-        fields.append("fd={!r}".format(self.fd))
-        fields.append("simulate={!r}".format(self.simulate))
-        fields.append("autoremove={!r}".format(self.autoremove))
-        fields.append("silent={!r}".format(self.silent))
+            fields.append('fcontent={!r}'.format(self.fcontent))
+        fields.append('ctime={!r}'.format(self.ctime))
+        fields.append('mtime={!r}'.format(self.mtime))
+        fields.append('fcontent={!r}'.format(self.fcontent))
+        fields.append('fd={!r}'.format(self.fd))
+        fields.append('simulate={!r}'.format(self.simulate))
+        fields.append('autoremove={!r}'.format(self.autoremove))
+        fields.append('silent={!r}'.format(self.silent))
 
         if fields:
-            out += ', ' + ", ".join(fields)
-        out += ")>"
+            out += ', ' + ', '.join(fields)
+        out += ')>'
         return out
 
     # -------------------------------------------------------------------------
     def __del__(self):
         """Delete this object - a destructor.
 
         Removes the lockfile, if self.autoremove is True
 
         """
         if not getattr(self, '_initialized', False):
             return
 
         if self.fd is not None:
-            msg = _("Closing file descriptor {} ...").format(self.fd)
+            msg = _('Closing file descriptor {} ...').format(self.fd)
             if self.silent:
                 if self.verbose >= 2:
                     LOG.debug(msg)
             else:
                 LOG.debug(msg)
             os.close(self.fd)
             self._fd = None
 
         if self.autoremove and self.exists:
 
-            msg = _("Automatic removing of {!r} ...").format(self.lockfile)
+            msg = _('Automatic removing of {!r} ...').format(self.lockfile)
             if self.silent:
                 if self.verbose >= 2:
                     LOG.debug(msg)
             else:
                 LOG.info(msg)
 
             if not self.simulate:
@@ -392,15 +390,15 @@
         if not self.exists():
             return None
         return self.lockfile.stat()
 
     # -------------------------------------------------------------------------
     def refresh(self):
         """Refresh the atime and mtime of the lockfile to the current time."""
-        msg = _("Refreshing atime and mtime of {!r} to the current timestamp.").format(
+        msg = _('Refreshing atime and mtime of {!r} to the current timestamp.').format(
             str(self.lockfile))
         LOG.debug(msg)
 
         if not self.simulate:
             os.utime(str(self.lockfile), None)
 
         self._mtime = datetime.datetime.utcfromtimestamp(self.stat().st_mtime)
@@ -526,60 +524,60 @@
     def lockretry_delay_start(self):
         """Return the first delay in seconds after an unsuccessful lockfile creation."""
         return self._lockretry_delay_start
 
     @lockretry_delay_start.setter
     def lockretry_delay_start(self, value):
         if not isinstance(value, Number):
-            msg = _("Value {val!r} for {what} is not a Number.").format(
+            msg = _('Value {val!r} for {what} is not a Number.').format(
                 val=value, what='lockretry_delay_start')
             raise LockHandlerError(msg)
 
         if value <= 0:
-            msg = _("The value for {what} must be greater than zero (is {val!r}).").format(
+            msg = _('The value for {what} must be greater than zero (is {val!r}).').format(
                 val=value, what='lockretry_delay_start')
             raise LockHandlerError(msg)
 
         self._lockretry_delay_start = value
 
     # -----------------------------------------------------------
     @property
     def lockretry_delay_increase(self):
         """Return the seconds to increase the delay in every wait cycle."""
         return self._lockretry_delay_increase
 
     @lockretry_delay_increase.setter
     def lockretry_delay_increase(self, value):
         if not isinstance(value, Number):
-            msg = _("Value {val!r} for {what} is not a Number.").format(
+            msg = _('Value {val!r} for {what} is not a Number.').format(
                 val=value, what='lockretry_delay_increase')
             raise LockHandlerError(msg)
 
         if value < 0:
-            msg = _("The value for {what} must be greater than zero (is {val!r}).").format(
+            msg = _('The value for {what} must be greater than zero (is {val!r}).').format(
                 val=value, what='lockretry_delay_increase')
             raise LockHandlerError(msg)
 
         self._lockretry_delay_increase = value
 
     # -----------------------------------------------------------
     @property
     def lockretry_max_delay(self):
         """Return ttotal maximum delay in seconds for trying to create a lockfile."""
         return self._lockretry_max_delay
 
     @lockretry_max_delay.setter
     def lockretry_max_delay(self, value):
         if not isinstance(value, Number):
-            msg = _("Value {val!r} for {what} is not a Number.").format(
+            msg = _('Value {val!r} for {what} is not a Number.').format(
                 val=value, what='lockretry_max_delay')
             raise LockHandlerError(msg)
 
         if value <= 0:
-            msg = _("The value for {what} must be greater than zero (is {val!r}).").format(
+            msg = _('The value for {what} must be greater than zero (is {val!r}).').format(
                 val=value, what='lockretry_max_delay')
             raise LockHandlerError(msg)
 
         self._lockretry_max_delay = value
 
     # -----------------------------------------------------------
     @property
@@ -590,20 +588,20 @@
         is valid (if locking_use_pid is False).
         """
         return self._max_lockfile_age
 
     @max_lockfile_age.setter
     def max_lockfile_age(self, value):
         if not isinstance(value, Number):
-            msg = _("Value {val!r} for {what} is not a Number.").format(
+            msg = _('Value {val!r} for {what} is not a Number.').format(
                 val=value, what='max_lockfile_age')
             raise LockHandlerError(msg)
 
         if value <= 0:
-            msg = _("The value for {what} must be greater than zero (is {val!r}).").format(
+            msg = _('The value for {what} must be greater than zero (is {val!r}).').format(
                 val=value, what='max_lockfile_age')
             raise LockHandlerError(msg)
 
         self._max_lockfile_age = value
 
     # -----------------------------------------------------------
     @property
@@ -664,48 +662,48 @@
     # -------------------------------------------------------------------------
     def __repr__(self):
         """Typecaste into a string for reproduction."""
         out = super(LockHandler, self).__repr__()[:-2]
 
         fields = []
         if self._lockdir:
-            fields.append("lockdir=%r" % (self.lockdir))
-        fields.append("lockretry_delay_start=%r" % (self.lockretry_delay_start))
-        fields.append("lockretry_delay_increase=%r" % (self.lockretry_delay_increase))
-        fields.append("lockretry_max_delay=%r" % (self.lockretry_max_delay))
-        fields.append("max_lockfile_age=%r" % (self.max_lockfile_age))
-        fields.append("locking_use_pid=%r" % (self.locking_use_pid))
-        fields.append("silent=%r" % (self.silent))
-        fields.append("stay_opened=%r" % (self.stay_opened))
+            fields.append('lockdir=%r' % (self.lockdir))
+        fields.append('lockretry_delay_start=%r' % (self.lockretry_delay_start))
+        fields.append('lockretry_delay_increase=%r' % (self.lockretry_delay_increase))
+        fields.append('lockretry_max_delay=%r' % (self.lockretry_max_delay))
+        fields.append('max_lockfile_age=%r' % (self.max_lockfile_age))
+        fields.append('locking_use_pid=%r' % (self.locking_use_pid))
+        fields.append('silent=%r' % (self.silent))
+        fields.append('stay_opened=%r' % (self.stay_opened))
 
         if fields:
-            out += ', ' + ", ".join(fields)
-        out += ")>"
+            out += ', ' + ', '.join(fields)
+        out += ')>'
         return out
 
     # -------------------------------------------------------------------------
     def check_for_number(self, value, default, what, must_gt_zero=False, must_ge_zero=False):
         """Check the given value for a numeric value."""
         if value is None:
             return default
 
         if not isinstance(value, Number):
-            msg = _("Value {val!r} for {what} is not a Number.").format(
+            msg = _('Value {val!r} for {what} is not a Number.').format(
                 val=value, what=what)
             raise LockHandlerError(msg)
 
         if must_gt_zero and value <= 0:
-            msg = _("The value for {what} must be greater than zero (is {val!r}).").format(
+            msg = _('The value for {what} must be greater than zero (is {val!r}).').format(
                 val=value, what=what)
             raise LockHandlerError(msg)
 
         if must_ge_zero and value < 0:
             msg = _(
-                "The value for {what} must be greater than "
-                "or equal to zero (is {val!r}).").format(
+                'The value for {what} must be greater than '
+                'or equal to zero (is {val!r}).').format(
                 val=value, what=what)
             raise LockHandlerError(msg)
 
         return value
 
     # -------------------------------------------------------------------------
     def create_lockfile(
@@ -780,32 +778,32 @@
             what='max_age', must_ge_zero=True)
 
         if pid is None:
             pid = os.getpid()
         else:
             pid = int(pid)
             if pid <= 0:
-                msg = _("Invalid PID {} given on calling create_lockfile().").format(pid)
+                msg = _('Invalid PID {} given on calling create_lockfile().').format(pid)
                 raise LockHandlerError(msg)
 
         lfile = Path(lockfile)
         if not lfile.is_absolute():
             lfile = self.lockdir / lfile
 
         lockdir = lfile.parent
         if self.verbose > 1:
-            LOG.debug(_("Using lock directory {!r} ...").format(str(lockdir)))
+            LOG.debug(_('Using lock directory {!r} ...').format(str(lockdir)))
         if not lockdir.is_dir():
             raise LockdirNotExistsError(lockdir)
 
         lfile = lockdir.resolve() / lfile.name
         if lfile.exists():
             lfile = lfile.resolve()
 
-        LOG.debug(_("Trying to lock lockfile {!r} ...").format(str(lockfile)))
+        LOG.debug(_('Trying to lock lockfile {!r} ...').format(str(lockfile)))
 
         if not os.access(str(lockdir), os.W_OK):
             msg = _("Locking directory {!r} isn't writeable.").format(str(lockdir))
             if self.simulate:
                 LOG.error(msg)
             else:
                 raise LockdirNotWriteableError(lockdir)
@@ -838,83 +836,83 @@
             # Big loop on trying to create the lockfile
             while fd is None and time_diff < max_delay:
 
                 time_diff = time.time() - start_time
                 counter += 1
 
                 if self.verbose > 3:
-                    LOG.debug(_("Current time difference: {:0.3f} seconds.").format(time_diff))
+                    LOG.debug(_('Current time difference: {:0.3f} seconds.').format(time_diff))
                 if time_diff >= max_delay:
                     break
 
                 # Try creating lockfile exclusive
-                LOG.debug(_("Try {try_nr} on creating lockfile {lfile!r} ...").format(
+                LOG.debug(_('Try {try_nr} on creating lockfile {lfile!r} ...').format(
                     try_nr=counter, lfile=str(lockfile)))
                 fd = self._create_lockfile(lockfile)
                 if fd is not None:
                     # success, then exit
                     break
 
                 # Check for other process, using this lockfile
                 if not self.check_lockfile(lockfile, max_age, use_pid):
                     # No other process is using this lockfile
                     if lockfile.exists():
-                        LOG.info(_("Removing lockfile {!r} ...").format(str(lockfile)))
+                        LOG.info(_('Removing lockfile {!r} ...').format(str(lockfile)))
                     try:
                         if not self.simulate:
                             lockfile.unlink()
                     except Exception as e:
-                        msg = _("Error on removing lockfile {lfile!r}: {err}").format(
+                        msg = _('Error on removing lockfile {lfile!r}: {err}').format(
                             lfile=str(lockfile), err=e)
                         LOG.error(msg)
                         time.sleep(delay)
                         delay += delay_increase
                         continue
 
                     fd = self._create_lockfile(lockfile)
                     if fd:
                         break
 
                 # No success, then retry later
                 if self.verbose > 2:
-                    LOG.debug(_("Sleeping for {:0.1f} seconds.").format(float(delay)))
+                    LOG.debug(_('Sleeping for {:0.1f} seconds.').format(float(delay)))
                 time.sleep(delay)
                 delay += delay_increase
 
             # fd is either None, for no success on locking
             if fd is None:
                 time_diff = time.time() - start_time
                 e = CouldntOccupyLockfileError(lockfile, time_diff, counter)
                 if raise_on_fail:
                     raise e
                 else:
                     LOG.error(str(e))
                 return None
 
             # or an int for success
-            msg = _("Got a lock for lockfile {!r}.").format(str(lockfile))
+            msg = _('Got a lock for lockfile {!r}.').format(str(lockfile))
             if self.silent:
                 LOG.debug(msg)
             else:
                 LOG.info(msg)
-            out = to_utf8("{}\n".format(pid))
-            LOG.debug(_("Write {what!r} in lockfile {lfile!r} ...").format(
+            out = to_utf8('{}\n'.format(pid))
+            LOG.debug(_('Write {what!r} in lockfile {lfile!r} ...').format(
                 what=out, lfile=str(lockfile)))
 
         finally:
 
             if fd is not None and not self.simulate:
                 os.write(fd, out)
 
                 if stay_opened:
-                    LOG.debug(_("Seeking and syncing {!r} ...").format(str(lockfile)))
+                    LOG.debug(_('Seeking and syncing {!r} ...').format(str(lockfile)))
                     os.lseek(fd, 0, 0)
                     os.fsync(fd)
                 else:
-                    LOG.debug(_("Closing {!r} ...").format(str(lockfile)))
+                    LOG.debug(_('Closing {!r} ...').format(str(lockfile)))
                     os.close(fd)
                     fd = None
 
         if fd is not None and self.simulate:
             fd = None
 
         lock_object = LockObject(
@@ -931,25 +929,25 @@
 
         @return: a file decriptor of the opened lockfile (if possible),
                  or None, if it isn't.
         @rtype: int or None
 
         """
         if self.verbose > 1:
-            LOG.debug(_("Trying to open {!r} exclusive ...").format(str(lockfile)))
+            LOG.debug(_('Trying to open {!r} exclusive ...').format(str(lockfile)))
         if self.simulate:
-            LOG.debug(_("Simulation mode, no real creation of a lockfile."))
+            LOG.debug(_('Simulation mode, no real creation of a lockfile.'))
             return -1
 
         fd = None
         try:
             fd = os.open(str(lockfile), os.O_CREAT | os.O_EXCL | os.O_WRONLY, 0o644)
             fcntl.flock(fd, fcntl.LOCK_EX | fcntl.LOCK_NB)
         except OSError as e:
-            msg = _("Error on creating lockfile {lfile!r}: {err}").format(
+            msg = _('Error on creating lockfile {lfile!r}: {err}').format(
                 lfile=str(lockfile), err=e)
             if e.errno == errno.EEXIST:
                 LOG.debug(msg)
                 return None
             else:
                 error_tuple = sys.exc_info()
                 reraise(LockHandlerError, msg, error_tuple[2])
@@ -973,27 +971,27 @@
             lfile = self.lockdir / lfile
         lfile = lfile.resolve()
 
         if not lfile.exists():
             LOG.debug(_("Lockfile {!r} to remove doesn't exists.").format(str(lfile)))
             return True
 
-        LOG.info(_("Removing lockfile {!r} ...").format(str(lfile)))
+        LOG.info(_('Removing lockfile {!r} ...').format(str(lfile)))
         if self.simulate:
             LOG.debug(_("Simulation mode - lockfile won't removed."))
             return True
 
         try:
             lfile.unlink()
         except Exception as e:
-            LOG.error(_("Error on removing lockfile {lfile!r}: {err}").format(
+            LOG.error(_('Error on removing lockfile {lfile!r}: {err}').format(
                 lfile=str(lockfile), err=e))
             if self.verbose:
                 tb = traceback.format_exc()
-                LOG.debug("Stacktrace:\n" + tb)
+                LOG.debug('Stacktrace:\n' + tb)
             return False
 
         return True
 
     # -------------------------------------------------------------------------
     def check_lockfile(self, lockfile, max_age=None, use_pid=None):
         """
@@ -1027,66 +1025,66 @@
         else:
             use_pid = bool(use_pid)
 
         if max_age is None:
             max_age = self.max_lockfile_age
         else:
             if not isinstance(max_age, Number):
-                msg = _("Value {val!r} for {what} is not a Number.").format(
+                msg = _('Value {val!r} for {what} is not a Number.').format(
                     val=max_age, what='max_age')
                 raise LockHandlerError(msg)
             if max_age <= 0:
-                msg = _("The value for {what} must be greater than zero (is {val!r}).").format(
+                msg = _('The value for {what} must be greater than zero (is {val!r}).').format(
                     val=max_age, what='max_age')
                 raise LockHandlerError(msg)
 
-        LOG.debug(_("Checking lockfile {!r} ...").format(str(lfile)))
+        LOG.debug(_('Checking lockfile {!r} ...').format(str(lfile)))
 
         if not lfile.exists():
             LOG.debug(_("Lockfile {!r} doesn't exists.").format(str(lfile)))
             return False
 
         if not os.access(str(lfile), os.R_OK):
-            LOG.warning(_("No read access for lockfile {!r}.").format(str(lfile)))
+            LOG.warning(_('No read access for lockfile {!r}.').format(str(lfile)))
             return True
 
         if not os.access(str(lfile), os.W_OK):
-            LOG.warning(_("No write access for lockfile {!r}.").format(str(lfile)))
+            LOG.warning(_('No write access for lockfile {!r}.').format(str(lfile)))
             return True
 
         if use_pid:
             pid = self.get_pid_from_file(lfile, True)
             if pid is None:
-                LOG.warning(_("Unusable lockfile {!r}.").format(str(lfile)))
+                LOG.warning(_('Unusable lockfile {!r}.').format(str(lfile)))
             else:
                 if self.dead(pid):
-                    LOG.warning(_("Process with PID {} is unfortunately dead.").format(pid))
+                    LOG.warning(_('Process with PID {} is unfortunately dead.').format(pid))
                     return False
                 else:
-                    LOG.debug(_("Process with PID {} is still running.").format(pid))
+                    LOG.debug(_('Process with PID {} is still running.').format(pid))
                     return True
 
         fstat = None
         try:
             fstat = lfile.stat()
         except OSError as e:
             if e.errno == errno.ENOENT:
-                LOG.info(_("Could not stat for file {lfile!r}: {err}").format(
+                LOG.info(_('Could not stat for file {lfile!r}: {err}').format(
                     lfile=str(lfile), err=e.strerror))
                 return False
             raise
 
         age = time.time() - fstat.st_mtime
         if age >= max_age:
-            LOG.debug(_("Lockfile {lfile!r} is older than {max} seconds ({age} seconds).").format(
+            LOG.debug(_('Lockfile {lfile!r} is older than {max} seconds ({age} seconds).').format(
                 lfile=str(lfile), max=max_age, age=age))
             return False
         msg = _(
-            "Lockfile {lfile!r} is {age} seconds old, but not old enough "
-            "({max} seconds).").format(lfile=str(lfile), max=max_age, age=age)
+            'Lockfile {lfile!r} is {age} seconds old, but not old enough '
+            '({max} seconds).').format(lfile=str(lfile), max=max_age, age=age)
         LOG.debug(msg)
         return True
 
     # -------------------------------------------------------------------------
     def get_pid_from_file(self, pidfile, force=False):
         """
         Try to read the PID of some process from the given file.
@@ -1103,52 +1101,52 @@
         @rtype: int (or None)
 
         """
         pfile = Path(pidfile)
         fh = None
 
         if self.verbose > 1:
-            LOG.debug(_("Trying to open pidfile {!r} ...").format(str(pfile)))
+            LOG.debug(_('Trying to open pidfile {!r} ...').format(str(pfile)))
         try:
-            fh = pfile.open("rb")
+            fh = pfile.open('rb')
         except Exception as e:
-            msg = _("Could not open pidfile {!r} for reading:").format(str(pfile))
+            msg = _('Could not open pidfile {!r} for reading:').format(str(pfile))
             msg += ' ' + str(e)
             if force:
                 LOG.warning(msg)
                 return None
             else:
                 raise LockHandlerError(str(e))
 
         content = fh.readline()
         fh.close()
 
         content = content.strip()
-        if content == "":
-            msg = _("First line of pidfile {!r} was empty.").format(str(pfile))
+        if content == '':
+            msg = _('First line of pidfile {!r} was empty.').format(str(pfile))
             if force:
                 LOG.warning(msg)
                 return None
             else:
                 raise LockHandlerError(msg)
 
         pid = None
         try:
             pid = int(content)
         except Exception as e:
-            msg = _("Could not interprete {cont!r} as a PID from {file!r}: {err}").format(
+            msg = _('Could not interprete {cont!r} as a PID from {file!r}: {err}').format(
                 cont=content, file=str(pfile), err=e)
             if force:
                 LOG.warning(msg)
                 return None
             else:
                 raise LockHandlerError(msg)
 
         if pid <= 0:
-            msg = _("Invalid PID {pid} in {file!r} found.").format(pid=pid, file=str(pfile))
+            msg = _('Invalid PID {pid} in {file!r} found.').format(pid=pid, file=str(pfile))
             if force:
                 LOG.warning(msg)
                 return None
             else:
                 raise LockHandlerError(msg)
 
         return pid
@@ -1213,14 +1211,14 @@
             else:
                 raise
 
         return dead
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/handling_obj.py` & `fb_tools-2.2.3/lib/fb_tools/handling_obj.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,67 +1,62 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a base object with extended handling.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import os
+import copy
+import datetime
+import errno
+import getpass
+import locale
 import logging
+import os
 import pipes
+import re
 import signal
-import errno
 import sys
-import locale
-import datetime
-import copy
-import re
-import getpass
-
 try:
     import pathlib
 except ImportError:
     import pathlib2 as pathlib
-
-from subprocess import Popen, PIPE
+from subprocess import PIPE, Popen
 if sys.version_info[0] >= 3:
     from subprocess import SubprocessError, TimeoutExpired
 else:
     class SubprocessError(Exception):
         """Dummy exception for Python 2."""
 
         pass
 
     class TimeoutExpired(SubprocessError):
         """Dummy exception for Python 2."""
 
         pass
 
 # Third party modules
+from fb_logging.colored import colorstr
+
 import six
 
 # Own modules
-from fb_logging.colored import colorstr
-
-from .common import pp, to_bool, caller_search_path, to_str, encode_or_bust
+from .common import caller_search_path, encode_or_bust, pp, to_bool, to_str
 from .common import indent, is_sequence
-
-from .xlate import XLATOR
-
-from .errors import InterruptError, IoTimeoutError, ReadTimeoutError, WriteTimeoutError
 from .errors import AbortAppError, TimeoutOnPromptError
-
+from .errors import InterruptError, IoTimeoutError, ReadTimeoutError, WriteTimeoutError
 from .obj import FbBaseObject
+from .xlate import XLATOR
 
-__version__ = '2.1.1'
+__version__ = '2.1.3'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 DEFAULT_FILEIO_TIMEOUT = 2
 DEFAULT_PROMPT_TIMEOUT = 30
@@ -71,15 +66,15 @@
 # =============================================================================
 class ProcessCommunicationTimeout(IoTimeoutError, SubprocessError):
     """Special exception class for process communication errors."""
 
     # -------------------------------------------------------------------------
     def __init__(self, timeout):
         """Initialise a ProcessCommunicationTimeout exception."""
-        msg = _("Timeout on communicating with process.")
+        msg = _('Timeout on communicating with process.')
         super(ProcessCommunicationTimeout, self).__init__(msg, timeout)
 
 
 # =============================================================================
 class CalledProcessError(SubprocessError):
     """
     Raised when run() is called with check=True and the process returns a non-zero exit status.
@@ -97,15 +92,15 @@
         self.cmd = cmd
         self.output = output
         self.stderr = stderr
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into string."""
-        return _("Command {c!r} returned non-zero exit status {rc}.").format(
+        return _('Command {c!r} returned non-zero exit status {rc}.').format(
             c=self.cmd, rc=self.returncode)
 
     # -------------------------------------------------------------------------
     @property
     def stdout(self):
         """Alias for output attribute, to match stderr."""
         return self.output
@@ -136,16 +131,16 @@
         self.output = output
         self.stderr = stderr
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into string."""
         msg = ngettext(
-            "Command {c!r} timed out after {s} second.",
-            "Command {c!r} timed out after {s} seconds.", self.timeout)
+            'Command {c!r} timed out after {s} second.',
+            'Command {c!r} timed out after {s} seconds.', self.timeout)
         return msg.format(c=self.cmd, s=self.timeout)
 
     # -------------------------------------------------------------------------
     @property
     def stdout(self):
         """Return self.output."""
         return self.output
@@ -297,16 +292,16 @@
         return getattr(self, '_prompt_timeout', self.default_prompt_timeout)
 
     @prompt_timeout.setter
     def prompt_timeout(self, value):
         v = int(value)
         if v < 0 or v > self.max_prompt_timeout:
             msg = _(
-                "Wrong prompt timeout {v!r}, must be greater or equal to Null "
-                "and less or equal to {max}.").format(v=value, max=self.max_prompt_timeout)
+                'Wrong prompt timeout {v!r}, must be greater or equal to Null '
+                'and less or equal to {max}.').format(v=value, max=self.max_prompt_timeout)
             LOG.warning(msg)
         else:
             self._prompt_timeout = v
 
     # -------------------------------------------------------------------------
     @classmethod
     def init_yes_no_lists(cls):
@@ -382,50 +377,50 @@
                  if not found
         @rtype: str or None
 
         """
         cmd = pathlib.Path(cmd)
 
         if self.verbose > 2:
-            LOG.debug(_("Searching for command {!r} ...").format(str(cmd)))
+            LOG.debug(_('Searching for command {!r} ...').format(str(cmd)))
 
         # Checking an absolute path
         if cmd.is_absolute():
             if not cmd.exists():
                 LOG.warning(_("Command {!r} doesn't exists.").format(str(cmd)))
                 return None
             if not os.access(str(cmd), os.X_OK):
-                msg = _("Command {!r} is not executable.").format(str(cmd))
+                msg = _('Command {!r} is not executable.').format(str(cmd))
                 LOG.warning(msg)
                 return None
             if resolve:
                 return cmd.resolve()
             return cmd
 
         additional_paths = []
         if self.add_search_paths and is_sequence(self.add_search_paths):
             additional_paths = copy.copy(self.add_search_paths)
 
         # Checking a relative path
         for d in caller_search_path(*additional_paths):
             if self.verbose > 3:
-                LOG.debug(_("Searching command in {!r} ...").format(str(d)))
+                LOG.debug(_('Searching command in {!r} ...').format(str(d)))
             p = d / cmd
             if p.exists():
                 if self.verbose > 2:
-                    LOG.debug("Found {!r} ...".format(str(p)))
+                    LOG.debug('Found {!r} ...'.format(str(p)))
                 if os.access(str(p), os.X_OK):
                     if resolve:
                         return p.resolve()
                     return p
                 else:
-                    LOG.debug(_("Command {!r} is not executable.").format(str(p)))
+                    LOG.debug(_('Command {!r} is not executable.').format(str(p)))
 
         # command not found, sorry
-        msg = _("Command {!r} not found.").format(str(cmd))
+        msg = _('Command {!r} not found.').format(str(cmd))
         if quiet:
             if self.verbose > 2:
                 LOG.debug(msg)
         else:
             LOG.warning(msg)
 
         return None
@@ -456,17 +451,17 @@
 
         If universal_newlines=True is passed, the "input" argument must be a
         string and stdout/stderr in the returned object will be strings rather than
         bytes.
 
         This method was taken from subprocess.py of the standard library of Python 3.5.
         """
-        input = None
+        inp = None
         if 'input' in kwargs:
-            input = kwargs['input']
+            inp = kwargs['input']
             del kwargs['input']
 
         timeout = None
         if 'timeout' in kwargs:
             timeout = kwargs['timeout']
             del kwargs['timeout']
 
@@ -478,54 +473,54 @@
         may_simulate = None
         if 'may_simulate' in kwargs:
             may_simulate = bool(kwargs['may_simulate'])
             del kwargs['may_simulate']
 
         if self.verbose >= 2:
             myargs = {
-                'input': input,
+                'input': inp,
                 'timeout': timeout,
                 'check': check,
                 'may_simulate': may_simulate,
                 'popenargs': popenargs,
                 'kwargs': kwargs,
             }
-            LOG.debug("Args of run():\n{}".format(pp(myargs)))
+            LOG.debug('Args of run():\n{}'.format(pp(myargs)))
 
-        if input is not None:
+        if inp is not None:
             if 'stdin' in kwargs:
                 raise ValueError(_('STDIN and input arguments may not both be used.'))
             kwargs['stdin'] = PIPE
 
-        LOG.debug(_("Executing command args:") + '\n' + pp(popenargs))
+        LOG.debug(_('Executing command args:') + '\n' + pp(popenargs))
         cmd_args = []
         for arg in popenargs[0]:
-            LOG.debug(_("Performing argument {!r}.").format(arg))
+            LOG.debug(_('Performing argument {!r}.').format(arg))
             cmd_args.append(pipes.quote(arg))
         cmd_str = ' '.join(cmd_args)
 
-        cmd_str = ' '.join(map(lambda x: pipes.quote(x), popenargs[0]))
-        LOG.debug(_("Executing: {}").format(cmd_str))
+        cmd_str = ' '.join((pipes.quote(x) for x in popenargs[0]))
+        LOG.debug(_('Executing: {}').format(cmd_str))
 
         if may_simulate and self.simulate:
-            LOG.info(_("Simulation mode, not executing: {}").format(cmd_str))
-            return CompletedProcess(popenargs, 0, "Simulated execution.\n", '')
+            LOG.info(_('Simulation mode, not executing: {}').format(cmd_str))
+            return CompletedProcess(popenargs, 0, 'Simulated execution.\n', '')
 
         process = None
         try:
             start_dt = datetime.datetime.now()
             process = Popen(*popenargs, **kwargs)
             if self.verbose > 0:
-                LOG.debug(_("PID of process: {}").format(process.pid))
+                LOG.debug(_('PID of process: {}').format(process.pid))
             try:
                 stdout, stderr = self._communicate(
-                    process, popenargs, input=input, timeout=timeout)
+                    process, popenargs, inp=inp, timeout=timeout)
             except Exception as e:
                 if self.verbose > 2:
-                    LOG.debug(_("{c} happened, killing process: {e}").format(
+                    LOG.debug(_('{c} happened, killing process: {e}').format(
                         c=e.__class__.__name__, e=e))
                 process.poll()
                 if process.returncode is None:
                     process.kill()
                 process.wait()
                 raise
             retcode = process.poll()
@@ -550,31 +545,31 @@
             return CompletedProcess(
                 process.args, retcode, stdout, stderr, start_dt=start_dt, end_dt=end_dt)
         else:
             return CompletedProcess(
                 popenargs, retcode, stdout, stderr, start_dt=start_dt, end_dt=end_dt)
 
     # -------------------------------------------------------------------------
-    def _communicate(self, process, popenargs, input=None, timeout=None):
+    def _communicate(self, process, popenargs, inp=None, timeout=None):
 
         try:
 
             if timeout is None:
-                return process.communicate(input)
+                return process.communicate(inp)
 
             def communicate_alarm_caller(signum, sigframe):
                 err = InterruptError(signum)
                 self.handle_info(str(err))
                 process.kill()
                 raise ProcessCommunicationTimeout(timeout)
 
             signal.signal(signal.SIGALRM, communicate_alarm_caller)
             signal.alarm(timeout)
 
-            stdout, stderr = process.communicate(input)
+            stdout, stderr = process.communicate(inp)
 
             signal.alarm(0)
 
         except TimeoutExpired:
             stdout, stderr = process.communicate()
             raise TimeoutExpiredError(popenargs, timeout, output=stdout, stderr=stderr)
 
@@ -619,15 +614,15 @@
         @type frame: None or a frame object
 
         """
         err = InterruptError(signum)
 
         if signum in self.signals_dont_interrupt:
             self.handle_info(str(err))
-            LOG.info(_("Nothing to do on signal."))
+            LOG.info(_('Nothing to do on signal.'))
             return
 
         self._interrupted = True
         raise err
 
     # -------------------------------------------------------------------------
     def read_file(
@@ -679,15 +674,15 @@
             raise IOError(
                 errno.ENOENT, _("File doesn't exists."), ifile)
         if not os.access(ifile, os.R_OK):
             raise IOError(
                 errno.EACCES, _('Read permission denied.'), ifile)
 
         if self.verbose > needed_verbose_level:
-            LOG.debug(_("Reading file content of {!r} ...").format(ifile))
+            LOG.debug(_('Reading file content of {!r} ...').format(ifile))
 
         signal.signal(signal.SIGALRM, read_alarm_caller)
         signal.alarm(timeout)
 
         open_args = {}
         if six.PY3 and not binary:
             open_args['encoding'] = encoding
@@ -767,54 +762,54 @@
         if must_exists:
             if not os.path.isfile(ofile):
                 raise IOError(errno.ENOENT, _("File doesn't exists."), ofile)
 
         if os.path.exists(ofile):
             if not os.access(ofile, os.W_OK):
                 if self.simulate:
-                    LOG.error(_("Write permission to {!r} denied.").format(ofile))
+                    LOG.error(_('Write permission to {!r} denied.').format(ofile))
                 else:
                     raise IOError(errno.EACCES, _('Write permission denied.'), ofile)
         else:
             parent_dir = os.path.dirname(ofile)
             if not os.access(parent_dir, os.W_OK):
                 if self.simulate:
-                    LOG.error(_("Write permission to {!r} denied.").format(parent_dir))
+                    LOG.error(_('Write permission to {!r} denied.').format(parent_dir))
                 else:
                     raise IOError(errno.EACCES, _('Write permission denied.'), parent_dir)
 
         if self.verbose > verb_level1:
             if self.verbose > verb_level2:
-                LOG.debug(_("Write {what!r} into {to!r}.").format(what=content, to=ofile))
+                LOG.debug(_('Write {what!r} into {to!r}.').format(what=content, to=ofile))
             else:
-                LOG.debug(_("Writing {!r} ...").format(ofile))
+                LOG.debug(_('Writing {!r} ...').format(ofile))
 
         if isinstance(content, six.binary_type):
             content_bin = content
         else:
             if isinstance(content, six.text_type):
                 content_bin = encode_or_bust(content, encoding)
             else:
                 content_bin = encode_or_bust(str(content), encoding)
 
         if self.simulate:
             if self.verbose > verb_level2:
-                LOG.debug(_("Simulating write into {!r}.").format(ofile))
+                LOG.debug(_('Simulating write into {!r}.').format(ofile))
             return
 
         signal.signal(signal.SIGALRM, write_alarm_caller)
         signal.alarm(timeout)
 
         # Open filename for writing unbuffered
         if self.verbose > verb_level3:
-            LOG.debug(_("Opening {!r} for write unbuffered ...").format(ofile))
+            LOG.debug(_('Opening {!r} for write unbuffered ...').format(ofile))
         with open(ofile, 'wb', 0) as fh:
             fh.write(content_bin)
             if self.verbose > verb_level3:
-                LOG.debug(_("Closing {!r} ...").format(ofile))
+                LOG.debug(_('Closing {!r} ...').format(ofile))
 
         signal.alarm(0)
 
         return
 
     # -------------------------------------------------------------------------
     def get_password(self, first_prompt=None, second_prompt=None, may_empty=True, repeat=True):
@@ -854,28 +849,28 @@
             if not self.quiet:
                 print()
             ret_passwd = self._get_password(first_prompt, may_empty)
             if ret_passwd:
                 if repeat:
                     second_passwd = self._get_password(second_prompt, may_empty=False)
                     if ret_passwd != second_passwd:
-                        msg = _("The entered passwords does not match.")
+                        msg = _('The entered passwords does not match.')
                         LOG.error(msg)
                         continue
             break
 
         return ret_passwd
 
     # -------------------------------------------------------------------------
     def _get_password(self, prompt, may_empty=True):
 
         def passwd_alarm_caller(signum, sigframe):
             raise TimeoutOnPromptError(self.prompt_timeout)
 
-        msg_intr = _("Interrupted on demand.")
+        msg_intr = _('Interrupted on demand.')
         ret_passwd = ''
 
         try:
             signal.signal(signal.SIGALRM, passwd_alarm_caller)
             signal.alarm(self.prompt_timeout)
 
             while True:
@@ -892,20 +887,20 @@
                         return ''
                     else:
                         continue
                 else:
                     break
 
         except (TimeoutOnPromptError, AbortAppError) as e:
-            msg = _("Got a {}:").format(e.__class__.__name__) + ' ' + str(e)
+            msg = _('Got a {}:').format(e.__class__.__name__) + ' ' + str(e)
             LOG.error(msg)
             self.exit(10)
 
         except KeyboardInterrupt:
-            msg = _("Got a {}:").format('KeyboardInterrupt') + ' ' + msg_intr
+            msg = _('Got a {}:').format('KeyboardInterrupt') + ' ' + msg_intr
             LOG.error(msg)
             self.exit(10)
 
         finally:
             signal.alarm(0)
 
         return ret_passwd
@@ -935,22 +930,22 @@
 
         if self.assumed_answer is not None:
             ret = self.assumed_answer
             if not self.quiet:
                 answer = _('No')
                 if ret:
                     answer = _('Yes')
-                answer = " " + _("Automatic answer: '{}'.").format(self.colored(answer, 'CYAN'))
+                answer = ' ' + _("Automatic answer: '{}'.").format(self.colored(answer, 'CYAN'))
                 print(prompt + answer)
             return ret
 
         def prompt_alarm_caller(signum, sigframe):
             raise TimeoutOnPromptError(self.prompt_timeout)
 
-        msg_intr = _("Interrupted on demand.")
+        msg_intr = _('Interrupted on demand.')
         try:
             signal.signal(signal.SIGALRM, prompt_alarm_caller)
             signal.alarm(self.prompt_timeout)
 
             reply = ''
             while True:
                 try:
@@ -976,20 +971,20 @@
                         continue
                 else:
                     continue
                 # Repeat the question
 
         except (TimeoutOnPromptError, AbortAppError) as e:
             print()
-            msg = _("Got a {}:").format(e.__class__.__name__) + ' ' + str(e)
+            msg = _('Got a {}:').format(e.__class__.__name__) + ' ' + str(e)
             LOG.error(msg)
             self.exit(10)
 
         except KeyboardInterrupt:
-            msg = _("Got a {}:").format('KeyboardInterrupt') + ' ' + msg_intr
+            msg = _('Got a {}:').format('KeyboardInterrupt') + ' ' + msg_intr
             print()
             LOG.error(msg)
             self.exit(10)
 
         finally:
             signal.alarm(0)
 
@@ -1024,21 +1019,21 @@
             else:
                 self.encoding = 'utf-8'
 
         self._start_dt = None
         self._end_dt = None
         if start_dt is not None:
             if not isinstance(start_dt, datetime.datetime):
-                msg = _("Parameter {t!r} must be a {e}, {v!r} was given.").format(
+                msg = _('Parameter {t!r} must be a {e}, {v!r} was given.').format(
                     t='start_dt', e='datetime.datetime', v=start_dt)
                 raise TypeError(msg)
             self._start_dt = start_dt
         if end_dt is not None:
             if not isinstance(end_dt, datetime.datetime):
-                msg = _("Parameter {t!r} must be a {e}, {v!r} was given.").format(
+                msg = _('Parameter {t!r} must be a {e}, {v!r} was given.').format(
                     t='end_dt', e='datetime.datetime', v=end_dt)
                 raise TypeError(msg)
             self._end_dt = end_dt
 
         self.stdout = stdout
         if stdout is not None:
             stdout = to_str(stdout, self.encoding)
@@ -1088,15 +1083,15 @@
             args.append('end_dt={!r}'.format(self.end_dt))
         if self.stdout is not None or self.stderr is not None:
             args.append('encoding={!r}'.format(self.encoding))
         if self.stdout is not None:
             args.append('stdout={!r}'.format(self.stdout))
         if self.stderr is not None:
             args.append('stderr={!r}'.format(self.stderr))
-        return "{}({})".format(type(self).__name__, ', '.join(args))
+        return '{}({})'.format(type(self).__name__, ', '.join(args))
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into a string."""
         out = _('Completed process') + ':\n'
         out += '  args:       {!r}\n'.format(self.args)
         out += '  returncode: {}\n'.format(self.returncode)
@@ -1123,14 +1118,14 @@
         """Raise CalledProcessError if the exit code is non-zero."""
         if self.returncode:
             raise CalledProcessError(self.returncode, self.args, self.stdout, self.stderr)
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/mailaddress.py` & `fb_tools-2.2.3/lib/fb_tools/mailaddress.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for the MailAddress object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
+import copy
 import logging
 import re
-import copy
-
 try:
     from collections.abc import MutableSequence
 except ImportError:
     from collections import MutableSequence
 
 # Third party modules
 import six
 
 # Own modules
-from .errors import InvalidMailAddressError
+from .common import is_sequence, pp, to_bool, to_str
 from .errors import EmptyMailAddressError
-
-from .common import to_str, to_bool, is_sequence, pp
-
-from .obj import FbGenericBaseObject, FbBaseObject
-
+from .errors import InvalidMailAddressError
+from .obj import FbBaseObject, FbGenericBaseObject
 from .xlate import XLATOR, format_list
 
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 def convert_attr(value):
@@ -62,34 +58,34 @@
     re_valid_address = re.compile(r'^' + pat_valid_address + r'$', re.IGNORECASE)
 
     # -------------------------------------------------------------------------
     @classmethod
     def valid_address(cls, address, raise_on_failure=False, verbose=0):
         """Check the validity of a mail address."""
         if not address:
-            e = InvalidMailAddressError(address, _("Empty address."))
+            e = InvalidMailAddressError(address, _('Empty address.'))
             if raise_on_failure:
                 raise e
             if verbose > 2:
                 LOG.debug(str(e))
             return False
 
         addr = to_str(address)
         if not isinstance(addr, str):
-            e = InvalidMailAddressError(address, _("Wrong type."))
+            e = InvalidMailAddressError(address, _('Wrong type.'))
             if raise_on_failure:
                 raise e
             if verbose > 2:
                 LOG.debug(str(e))
             return False
 
         if cls.re_valid_address.search(addr):
             return True
 
-        e = InvalidMailAddressError(address, _("Invalid address."))
+        e = InvalidMailAddressError(address, _('Invalid address.'))
         if raise_on_failure:
             raise e
         if verbose > 2:
             LOG.debug(str(e))
         return False
 
     # -------------------------------------------------------------------------
@@ -99,20 +95,20 @@
         self._domain = ''
         self._verbose = 0
         self.verbose = verbose
         self._empty_ok = False
         self.empty_ok = empty_ok
 
         if self.verbose > 3:
-            msg = _("Given user: {u!r}, given domain: {d!r}.")
+            msg = _('Given user: {u!r}, given domain: {d!r}.')
             LOG.debug(msg.format(u=user, d=domain))
 
         if user:
             if not isinstance(user, six.string_types):
-                msg = _("Invalid mail address.")
+                msg = _('Invalid mail address.')
                 raise InvalidMailAddressError(user, msg)
             user = to_str(user)
 
         if not domain:
             if user:
                 addr = convert_attr(user)
                 if self.valid_address(addr, verbose=self.verbose):
@@ -121,37 +117,37 @@
                     self._domain = match.group(2)
                     return
                 match = self.re_valid_domain.search(addr)
                 if match:
                     self._domain = match.group(1)
                     return
                 if not self.re_valid_user.search(user):
-                    msg = _("Invalid user/mailbox name.")
+                    msg = _('Invalid user/mailbox name.')
                     raise InvalidMailAddressError(user, msg)
                 self._user = addr
                 return
 
             e = EmptyMailAddressError()
             if self.empty_ok:
                 if self.verbose > 2:
                     LOG.debug(str(e))
                 return
             raise e
 
         if user:
             c_user = convert_attr(user)
             if not self.re_valid_user.search(c_user):
-                msg = _("Invalid user/mailbox name.")
+                msg = _('Invalid user/mailbox name.')
                 raise InvalidMailAddressError(user, msg)
         else:
             c_user = None
 
         c_domain = convert_attr(domain)
         if not self.re_valid_domain.search('@' + c_domain):
-            msg = _("Invalid domain.")
+            msg = _('Invalid domain.')
             raise InvalidMailAddressError(domain, msg)
 
         self._user = c_user
         self._domain = c_domain
 
     # -------------------------------------------------------------------------
     def _short_init(self, user, domain, verbose=0, empty_ok=False):
@@ -160,15 +156,15 @@
         self._domain = ''
         self._verbose = 0
         self.verbose = verbose
         self._empty_ok = False
         self.empty_ok = empty_ok
 
         if self.verbose > 3:
-            msg = _("Given user: {u!r}, given domain: {d!r}.")
+            msg = _('Given user: {u!r}, given domain: {d!r}.')
             LOG.debug(msg.format(u=user, d=domain))
 
         if user:
             self._user = str(user).lower().strip()
 
         if domain:
             self._domain = str(domain).lower().strip()
@@ -197,15 +193,15 @@
 
     @verbose.setter
     def verbose(self, value):
         v = int(value)
         if v >= 0:
             self._verbose = v
         else:
-            msg = _("Wrong verbose level {!r}, must be >= 0").format(value)
+            msg = _('Wrong verbose level {!r}, must be >= 0').format(value)
             raise ValueError(msg)
 
     # -----------------------------------------------------------
     @property
     def empty_ok(self):
         """Is an empty mail address valid or should there be raised an exceptiom."""
         return self._empty_ok
@@ -271,33 +267,33 @@
             return self.domain
 
         return self.user + '@' + self.domain
 
     # -------------------------------------------------------------------------
     def __repr__(self):
         """Typecast into a string for reproduction."""
-        out = "<%s(" % (self.__class__.__name__)
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
-        fields.append("user={!r}".format(self.user))
-        fields.append("domain={!r}".format(self.domain))
+        fields.append('user={!r}'.format(self.user))
+        fields.append('domain={!r}'.format(self.domain))
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def __hash__(self):
         """Return e hash value of the current object."""
         return hash(str(self).lower())
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
         """Compare for equality."""
         if self.verbose > 5:
-            msg = _("Checking equality {self!r} with {other!r} ...")
+            msg = _('Checking equality {self!r} with {other!r} ...')
             LOG.debug(msg.format(self=self, other=other))
 
         if not isinstance(other, MailAddress):
             return False
 
         if MailAddress is not other.__class__.__mro__[0]:
             if isinstance(other, QualifiedMailAddress):
@@ -345,20 +341,20 @@
             return False
         return True
 
     # -------------------------------------------------------------------------
     def __lt__(self, other):
         """Compare, whether the current address is less than another."""
         if not isinstance(other, MailAddress):
-            msg = _("Object {o!r} for comparing is not a {c} object.").format(
+            msg = _('Object {o!r} for comparing is not a {c} object.').format(
                 o=other, c='MailAddress')
             raise TypeError(msg)
 
         if self.verbose > 5:
-            msg = _("Comparing {self!r} with {other!r} ...")
+            msg = _('Comparing {self!r} with {other!r} ...')
             LOG.debug(msg.format(self=self, other=other))
 
         if MailAddress is not other.__class__.__mro__[0]:
             if isinstance(other, QualifiedMailAddress):
                 other_simple = other.simple()
                 if self == other_simple:
                     if other.name is None:
@@ -461,82 +457,82 @@
     re_only_whitespace = re.compile(r'^\s+$')
 
     # -------------------------------------------------------------------------
     @classmethod
     def valid_full_address(cls, address, raise_on_failure=False, verbose=0):
         """Check the validity of a full qualified mail address."""
         if not address:
-            e = InvalidMailAddressError(address, _("Empty address."))
+            e = InvalidMailAddressError(address, _('Empty address.'))
             if raise_on_failure:
                 raise e
             if verbose > 2:
                 LOG.debug(str(e))
             return False
 
         addr = to_str(address)
         if not isinstance(addr, str):
-            e = InvalidMailAddressError(address, _("Wrong type."))
+            e = InvalidMailAddressError(address, _('Wrong type.'))
             if raise_on_failure:
                 raise e
             if verbose > 2:
                 LOG.debug(str(e))
             return False
 
         if verbose > 4:
-            LOG.debug(_("Evaluating address {!r} ...").format(addr))
-            LOG.debug(_("Search pattern simple: {}").format(cls.re_valid_address))
+            LOG.debug(_('Evaluating address {!r} ...').format(addr))
+            LOG.debug(_('Search pattern simple: {}').format(cls.re_valid_address))
         if cls.re_valid_address.search(addr):
             return True
 
         if verbose > 4:
-            LOG.debug(_("Search pattern full: {}").format(cls.re_valid_full_address))
+            LOG.debug(_('Search pattern full: {}').format(cls.re_valid_full_address))
         if cls.re_valid_full_address.match(addr):
             return True
 
-        e = InvalidMailAddressError(address, _("Invalid address."))
+        e = InvalidMailAddressError(address, _('Invalid address.'))
         if raise_on_failure:
             raise e
         if verbose > 2:
             LOG.debug(str(e))
         return False
 
     # -------------------------------------------------------------------------
     def __init__(
             self, address=None, *, user=None, domain=None, name=None, verbose=0, empty_ok=False):
         """Initialise a QualifiedMailAddress object."""
         self._name = None
 
         if verbose > 3:
-            msg = "Given - address: {a!r}, user: {u!r}, domain: {d!r}, full name: {n!r}."
+            msg = 'Given - address: {a!r}, user: {u!r}, domain: {d!r}, full name: {n!r}.'
             LOG.debug(msg.format(a=address, u=user, d=domain, n=name))
 
         if address:
             if user or domain or name:
                 param_list = ('user', 'domain', 'name')
-                msg = _("Parameters {lst} may not be given, if parameter {a!r} was given.")
+                msg = _('Parameters {lst} may not be given, if parameter {a!r} was given.')
                 msg = msg.format(lst=format_list(param_list, do_repr=True), a='address')
                 raise RuntimeError(msg)
             return self._init_from_address(address, verbose=verbose, empty_ok=empty_ok)
 
         super(QualifiedMailAddress, self).__init__(
             user=user, domain=domain, verbose=verbose, empty_ok=empty_ok)
 
         if name:
             _name = to_str(name).strip()
             if not isinstance(_name, six.string_types):
-                msg = _("Invalid full user name.")
+                msg = _('Invalid full user name.')
                 raise InvalidMailAddressError(name, msg)
             if _name:
                 self._name = _name
 
     # -------------------------------------------------------------------------
     def _init_from_address(self, address, verbose=0, empty_ok=False):
 
         if not self.valid_full_address(address, raise_on_failure=True, verbose=verbose):
-            raise InvalidMailAddressError(address, _("Invalid address."))
+            raise InvalidMailAddressError(address, _('Invalid address.'))
 
         user = None
         domain = None
         name = None
 
         match = self.re_valid_full_address.search(address)
         if match:
@@ -551,15 +547,15 @@
                     self._name = match_quoting.group(1)
                 else:
                     self._name = name
             return
 
         match = self.re_valid_address.search(address)
         if not match:
-            raise InvalidMailAddressError(address, _("Invalid address."))
+            raise InvalidMailAddressError(address, _('Invalid address.'))
 
         user = match.group(1).strip().lower()
         domain = match.group(2).strip().lower()
         super(QualifiedMailAddress, self)._short_init(
             user=user, domain=domain, verbose=verbose, empty_ok=empty_ok)
 
     # -----------------------------------------------------------
@@ -635,29 +631,29 @@
             show_name = '"' + show_name + '"'
 
         return show_name + ' {a}'.format(a=show_addr)
 
     # -------------------------------------------------------------------------
     def __repr__(self):
         """Typecast into a string for reproduction."""
-        out = "<%s(" % (self.__class__.__name__)
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
-        fields.append("user={!r}".format(self.user))
-        fields.append("domain={!r}".format(self.domain))
-        fields.append("name={!r}".format(self.name))
+        fields.append('user={!r}'.format(self.user))
+        fields.append('domain={!r}'.format(self.domain))
+        fields.append('name={!r}'.format(self.name))
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
         """Compare for equality."""
         if self.verbose > 5:
-            msg = _("Checking equality {self!r} with {other!r} ...")
+            msg = _('Checking equality {self!r} with {other!r} ...')
             LOG.debug(msg.format(self=self, other=other))
 
         if not isinstance(other, MailAddress):
             return False
 
         if not isinstance(other, QualifiedMailAddress):
             # Other must be a simple MailAddress
@@ -673,20 +669,20 @@
 
         return self.name == other.name
 
     # -------------------------------------------------------------------------
     def __lt__(self, other):
         """Compare, whether the current address is less than another."""
         if not isinstance(other, MailAddress):
-            msg = _("Object {o!r} for comparing is not a {c} object.").format(
+            msg = _('Object {o!r} for comparing is not a {c} object.').format(
                 o=other, c='MailAddress')
             raise TypeError(msg)
 
         if self.verbose > 5:
-            msg = _("Comparing {self!r} with {other!r} ...")
+            msg = _('Comparing {self!r} with {other!r} ...')
             LOG.debug(msg.format(self=self, other=other))
 
         self_simple = self.simple()
 
         if not isinstance(other, QualifiedMailAddress):
             if self_simple == other:
                 return False
@@ -796,44 +792,44 @@
     def __str__(self):
         """Typecast into a str object."""
         return pp(self.as_list(True))
 
     # -------------------------------------------------------------------------
     def __repr__(self):
         """Typecast into a string for reproduction."""
-        out = "<%s(" % (self.__class__.__name__)
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
-        fields.append("appname={!r}".format(self.appname))
-        fields.append("verbose={!r}".format(self.verbose))
-        fields.append("version={!r}".format(self.version))
-        fields.append("empty_ok={!r}".format(self.empty_ok))
-        fields.append("may_simple={!r}".format(self.may_simple))
+        fields.append('appname={!r}'.format(self.appname))
+        fields.append('verbose={!r}'.format(self.verbose))
+        fields.append('version={!r}'.format(self.version))
+        fields.append('empty_ok={!r}'.format(self.empty_ok))
+        fields.append('may_simple={!r}'.format(self.may_simple))
 
         for address in self:
-            fields.append("{!r}".format(address))
+            fields.append('{!r}'.format(address))
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def _to_address(self, address):
         """Convert given address into a usable MailAddress or QualifiedMailAddress object."""
         if isinstance(address, MailAddress):
             if self.verbose > 5:
-                LOG.debug("Trying to use address {!r} ...".format(address))
+                LOG.debug('Trying to use address {!r} ...'.format(address))
             if not self.may_simple and not isinstance(address, QualifiedMailAddress):
                 addr = QualifiedMailAddress(
                     user=address.user, domain=address.domain,
                     verbose=self.verbose, empty_ok=self.empty_ok)
                 if self.verbose > 4:
-                    LOG.debug("Using qualified address {!r} ...".format(addr))
+                    LOG.debug('Using qualified address {!r} ...'.format(addr))
                 return addr
             if self.verbose > 4:
-                LOG.debug("Using address {!r} ...".format(address))
+                LOG.debug('Using address {!r} ...'.format(address))
             return address
 
         addr = QualifiedMailAddress(address, verbose=self.verbose, empty_ok=self.empty_ok)
         if self.may_simple and addr.name is None:
             return addr.simple()
         return addr
 
@@ -843,15 +839,15 @@
         addr = self._to_address(address)
         self._addresses.append(addr)
 
     # -------------------------------------------------------------------------
     def __copy__(self):
         """Return a copy of the current address list."""
         if self.verbose > 1:
-            LOG.debug("Copying myself ...")
+            LOG.debug('Copying myself ...')
 
         new_list = self.__class__(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             empty_ok=self.empty_ok, may_simple=self.may_simple, initialized=False)
 
         for addr in self:
             new_list.append(copy.copy(addr))
@@ -872,44 +868,44 @@
         new_list.initialized = self.initialized
         return new_list
 
     # -------------------------------------------------------------------------
     def __add__(self, other):
         """Return a copy of the current address list with the other list appended."""
         if not is_sequence(other):
-            msg = _("Given object {o!r} is not a sequence type, but a {t!r} type instead.")
+            msg = _('Given object {o!r} is not a sequence type, but a {t!r} type instead.')
             raise TypeError(msg.format(o=other, t=other.__class__.__qualname__))
 
         result = self.__copy__()
 
         for addr in other:
             result.append(addr)
 
         return result
 
     # -------------------------------------------------------------------------
     def __iadd__(self, other):
         """Append the other list to the current address list."""
         if not is_sequence(other):
-            msg = _("Given object {o!r} is not a sequence type, but a {t!r} type instead.")
+            msg = _('Given object {o!r} is not a sequence type, but a {t!r} type instead.')
             raise TypeError(msg.format(o=other, t=other.__class__.__qualname__))
 
         for addr in other:
             self.append(addr)
 
     # -------------------------------------------------------------------------
     def index(self, address, *args):
         """Get the position of the first occurence of the given address."""
         i = None
         j = None
         addr = self._to_address(address)
 
         if len(args) > 0:
             if len(args) > 2:
-                raise TypeError(_("{m} takes at most {max} arguments ({n} given).").format(
+                raise TypeError(_('{m} takes at most {max} arguments ({n} given).').format(
                     m='index()', max=3, n=len(args) + 1))
             i = int(args[0])
             if len(args) > 1:
                 j = int(args[1])
 
         index = 0
         start = 0
@@ -941,15 +937,15 @@
             for index in list(range(len(self))):
                 item = self._addresses[index]
                 if index >= end:
                     break
             if item == addr:
                 return index
 
-        msg = _("Mail address {} is not in address list.").format(addr)
+        msg = _('Mail address {} is not in address list.').format(addr)
         raise ValueError(msg)
 
     # -------------------------------------------------------------------------
     def __contains__(self, address):
         """Return, whether the given address is existing in current list."""
         if not self._addresses:
             return False
@@ -1012,14 +1008,14 @@
     def clear(self):
         """Remove all items from the MailAddressList."""
         self._addresses = []
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/merge.py` & `fb_tools-2.2.3/lib/fb_tools/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
 """
 
 import itertools
 
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 
 
 # =============================================================================
 class ZipExhausted(Exception):
     """An exception, which is raised, when the longest iterable is exhausted."""
 
     pass
@@ -68,14 +68,14 @@
             return a + b
 
     return a if b is None else b
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/multi_config.py` & `fb_tools-2.2.3/lib/fb_tools/multi_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: A module for providing a configuration based on multiple configuration files.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2022 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard module
-import logging
-import pathlib
 import codecs
-import re
-import sys
 import copy
-import os
 import json
+import logging
+import os
+import pathlib
+import re
 import stat
-
+import sys
+# from configparser import Error as ConfigParseError
+from configparser import ExtendedInterpolation
 from pathlib import Path
 
 # Third party modules
-import six
+import chardet
 
+import six
 from six import StringIO
 from six.moves import configparser
 
-import chardet
-
-# from configparser import Error as ConfigParseError
-from configparser import ExtendedInterpolation
-
 HAS_YAML = False
 try:
     import yaml
     HAS_YAML = True
 except ImportError:
     pass
 
@@ -53,27 +50,22 @@
     from toml import TomlDecodeError
     HAS_TOML = True
 except ImportError:
     pass
 
 
 # Own modules
+from .common import is_sequence, pp, to_bool, to_str
 from .config import ConfigError
-
-from .common import pp, to_bool, to_str, is_sequence
-
-from .obj import FbBaseObject
-
 from .handling_obj import HandlingObject
-
 from .merge import merge_structure
-
+from .obj import FbBaseObject
 from .xlate import XLATOR, format_list
 
-__version__ = '2.0.3'
+__version__ = '2.0.4'
 
 LOG = logging.getLogger(__name__)
 UTF8_ENCODING = 'utf-8'
 DEFAULT_ENCODING = UTF8_ENCODING
 
 _ = XLATOR.gettext
 
@@ -93,15 +85,15 @@
     def __init__(self, method):
         """Initialise a MultiCfgLoaderNotFoundError exception."""
         self.method = method
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typescast into a string."""
-        msg = _("Config loader method {!r} was not found.").format(self.method)
+        msg = _('Config loader method {!r} was not found.').format(self.method)
         return msg
 
 
 # =============================================================================
 class MultiCfgParseError(MultiConfigError, ValueError):
     """Exception class for parsing in BaseMultiConfig class.
 
@@ -204,19 +196,19 @@
         super(BaseMultiConfig, self).__init__(
             appname=appname, verbose=verbose, version=version,
             base_dir=base_dir, initialized=False,
         )
 
         if self.verbose > 1:
             if not HAS_YAML:
-                LOG.debug(_("{} configuration is not supported.").format('Yaml'))
+                LOG.debug(_('{} configuration is not supported.').format('Yaml'))
             if not HAS_HJSON:
-                LOG.debug(_("{} configuration is not supported.").format('HJson'))
+                LOG.debug(_('{} configuration is not supported.').format('HJson'))
             if not HAS_TOML:
-                LOG.debug(_("{} configuration is not supported.").format('Toml'))
+                LOG.debug(_('{} configuration is not supported.').format('Toml'))
 
         if encoding:
             self.encoding = encoding
         else:
             self.encoding = self.default_encoding
 
         if config_dir:
@@ -239,16 +231,16 @@
         """Return the default encoding used to read config files."""
         return self._encoding
 
     @encoding.setter
     def encoding(self, value):
         if not isinstance(value, str):
             msg = _(
-                "Encoding {v!r} must be a {s!r} object, "
-                "but is a {c!r} object instead.").format(
+                'Encoding {v!r} must be a {s!r} object, '
+                'but is a {c!r} object instead.').format(
                 v=value, s='str', c=value.__class__.__name__)
             raise TypeError(msg)
 
         encoder = codecs.lookup(value)
         self._encoding = encoder.name
 
     # -------------------------------------------------------------------------
@@ -261,29 +253,29 @@
     def additional_config_file(self, value):
         if value is None:
             self._additional_config_file = None
             return
 
         cfg_file = Path(value)
         if not cfg_file.exists():
-            msg = _("Additional config file {!r} does not exists.")
+            msg = _('Additional config file {!r} does not exists.')
             if self.raise_on_error:
                 raise MultiConfigError(msg.format(str(cfg_file)))
             LOG.error(msg.format(str(cfg_file)))
             return
 
         if not cfg_file.is_file():
-            msg = _("Configuration file {!r} exists, but is not a regular file.")
+            msg = _('Configuration file {!r} exists, but is not a regular file.')
             if self.raise_on_error:
                 raise MultiConfigError(msg.format(str(cfg_file)))
             LOG.error(msg.format(str(cfg_file)))
             return
 
         if not os.access(cfg_file, os.R_OK):
-            msg = _("Configuration file {!r} is not readable.")
+            msg = _('Configuration file {!r} is not readable.')
             if self.raise_on_error:
                 raise MultiConfigError(msg.format(str(cfg_file)))
             LOG.error(msg.format(str(cfg_file)))
             return
 
         cfg_file = cfg_file.resolve()
         self._additional_config_file = cfg_file
@@ -296,18 +288,18 @@
         This directory contains the configuration relative to different paths.
         """
         return self._config_dir
 
     @config_dir.setter
     def config_dir(self, value):
         if value is None:
-            raise TypeError(_("A configuration directory may not be None."))
+            raise TypeError(_('A configuration directory may not be None.'))
         cdir = pathlib.Path(value)
         if cdir.is_absolute():
-            msg = _("Configuration directory {!r} may not be absolute.").format(str(cdir))
+            msg = _('Configuration directory {!r} may not be absolute.').format(str(cdir))
             raise MultiConfigError(msg)
         self._config_dir = cdir
 
     # -------------------------------------------------------------------------
     @property
     def logfile(self):
         """Return a possible log file.
@@ -379,15 +371,15 @@
             self._ini_delimiters = []
             for character in value:
                 self._ini_delimiters.append(character)
             return
         if is_sequence(value):
             self._ini_delimiters = copy.copy(value)
             return
-        msg = _("Cannot use {!r} as delimiters for ini-files.").format(value)
+        msg = _('Cannot use {!r} as delimiters for ini-files.').format(value)
         raise TypeError(msg)
 
     # -------------------------------------------------------------------------
     @property
     def ini_comment_prefixes(self):
         """Return prefixes for comment lines in ini-files."""
         return self._ini_comment_prefixes
@@ -401,15 +393,15 @@
             self._ini_comment_prefixes = []
             for character in value:
                 self._ini_comment_prefixes.append(character)
             return
         if is_sequence(value):
             self._ini_comment_prefixes = copy.copy(value)
             return
-        msg = _("Cannot use {!r} as comment prefixes for ini-files.").format(value)
+        msg = _('Cannot use {!r} as comment prefixes for ini-files.').format(value)
         raise TypeError(msg)
 
     # -------------------------------------------------------------------------
     @property
     def ini_inline_comment_prefixes(self):
         """Return inline prefixes for comment lines in ini-files."""
         return self._ini_inline_comment_prefixes
@@ -423,15 +415,15 @@
             self._ini_inline_comment_prefixes = []
             for character in value:
                 self._ini_inline_comment_prefixes.append(character)
             return
         if is_sequence(value):
             self._ini_inline_comment_prefixes = copy.copy(value)
             return
-        msg = _("Cannot use {!r} as inline comment prefixes for ini-files.").format(value)
+        msg = _('Cannot use {!r} as inline comment prefixes for ini-files.').format(value)
         raise TypeError(msg)
 
     # -------------------------------------------------------------------------
     @property
     def ini_extended_interpolation(self):
         """Use ExtendedInterpolation for interpolation of ini-files.
 
@@ -609,45 +601,45 @@
 
         self.stems = copy.copy(self.default_stems)
 
         if additional_stems:
             if is_sequence(additional_stems):
                 for stem in additional_stems:
                     if not isinstance(stem, (six.string_types, six.binary_type, pathlib.Path)):
-                        msg = _("Stem {!r} is not a String type.").format(stem)
+                        msg = _('Stem {!r} is not a String type.').format(stem)
                         raise TypeError(msg)
                     s = str(to_str(stem))
                     if not self.valid_stem(s):
-                        msg = _("File name stem {!r} is invalid.").format(s)
+                        msg = _('File name stem {!r} is invalid.').format(s)
                         raise ValueError(msg)
                     if s not in self.stems:
                         self.stems.append(s)
             else:
                 if not isinstance(additional_stems, (
                         six.string_types, six.binary_type, pathlib.Path)):
-                    msg = _("Stem {!r} is not a String type.").format(additional_stems)
+                    msg = _('Stem {!r} is not a String type.').format(additional_stems)
                     raise TypeError(msg)
                 s = str(to_str(additional_stems))
                 if not self.valid_stem(s):
-                    msg = _("File name stem {!r} is invalid.").format(s)
+                    msg = _('File name stem {!r} is invalid.').format(s)
                     raise ValueError(msg)
                 if s not in self.stems:
                     self.stems.append(s)
 
         if not self.stems or append_appname_to_stems:
             if not self.valid_stem(self.appname):
-                msg = _("File name stem {!r} is invalid.").format(self.appname)
+                msg = _('File name stem {!r} is invalid.').format(self.appname)
                 raise ValueError(msg)
             if self.appname not in self.stems:
                 self.stems.append(self.appname)
 
     # -------------------------------------------------------------------------
     def _init_types(self):
         """Initialize configuration types and their assigned file extensions."""
-        invalid_msg = _("Invalid configuration type {t!r} - not found in {w!r}.")
+        invalid_msg = _('Invalid configuration type {t!r} - not found in {w!r}.')
 
         for cfg_type in self.available_cfg_types:
 
             if cfg_type not in self.default_loader_methods:
                 msg = invalid_msg.format(t=cfg_type, w='default_loader_methods')
                 raise RuntimeError(msg)
             if cfg_type not in self.default_type_extension_patterns:
@@ -679,44 +671,44 @@
             else:
                 if ext_pattern in self.ini_style_types:
                     self.ini_style_types.remove(ext_pattern)
 
     # -------------------------------------------------------------------------
     def collect_config_files(self):
         """Collect all appropriate config file from different directories."""
-        LOG.debug(_("Collecting all configuration files."))
+        LOG.debug(_('Collecting all configuration files.'))
 
         self.config_files = []
         self.config_file_pattern = {}
 
         for cfg_dir in self.config_dirs:
             if self.verbose > 1:
-                msg = _("Discovering config directory {!r} ...").format(str(cfg_dir))
+                msg = _('Discovering config directory {!r} ...').format(str(cfg_dir))
                 LOG.debug(msg)
             self._eval_config_dir(cfg_dir)
 
         self._set_additional_file(self.additional_config_file)
 
         self.check_privacy()
 
         if self.verbose > 2:
-            LOG.debug(_("Collected config files:") + '\n' + pp(self.config_files))
+            LOG.debug(_('Collected config files:') + '\n' + pp(self.config_files))
 
         self._cfgfiles_collected = True
 
     # -------------------------------------------------------------------------
     def check_privacy(self):
         """Check the permissions of the given config file.
 
         If it  is not located below /etc and public visible, then raise a MultiConfigError.
         """
         if not self.ensure_privacy:
             return
 
-        LOG.debug(_("Checking permissions of config files ..."))
+        LOG.debug(_('Checking permissions of config files ...'))
 
         def is_relative_to_etc(cfile):
             try:
                 rel = cfile.relative_to('/etc')                 # noqa
                 return True
             except ValueError:
                 return False
@@ -724,65 +716,65 @@
         for cfg_file in self.config_files:
 
             # if cfg_file.is_relative_to('/etc'):
             if is_relative_to_etc(cfg_file):
                 continue
 
             if self.verbose > 1:
-                LOG.debug(_("Checking permissions of {!r} ...").format(str(cfg_file)))
+                LOG.debug(_('Checking permissions of {!r} ...').format(str(cfg_file)))
 
             mode = cfg_file.stat().st_mode
             if self.verbose > 2:
-                msg = _("Found file permissions of {fn!r}: {mode:04o}")
+                msg = _('Found file permissions of {fn!r}: {mode:04o}')
                 LOG.debug(msg.format(fn=str(cfg_file), mode=mode))
             if (mode & stat.S_IRGRP) or (mode & stat.S_IROTH):
-                msg = _("File {fn!r} is readable by group or by others, found mode {mode:04o}.")
+                msg = _('File {fn!r} is readable by group or by others, found mode {mode:04o}.')
                 if self.raise_on_error:
                     raise MultiConfigError(msg.format(fn=str(cfg_file), mode=mode))
                 LOG.error(msg.format(fn=str(cfg_file), mode=mode))
 
     # -------------------------------------------------------------------------
     def _set_additional_file(self, cfg_file):
 
         if not cfg_file:
             return
 
         if self.verbose > 1:
-            msg = _("Trying to detect file type of additional config file {!r}.")
+            msg = _('Trying to detect file type of additional config file {!r}.')
             LOG.debug(msg.format(str(cfg_file)))
 
         performed = False
         for type_name in self.available_cfg_types:
             for ext_pattern in self.ext_patterns[type_name]:
 
                 pat = r'\.' + ext_pattern + r'$'
                 if self.verbose > 3:
-                    msg = _("Checking file {fn!r} for pattern {pat!r}.")
+                    msg = _('Checking file {fn!r} for pattern {pat!r}.')
                     LOG.debug(msg.format(fn=cfg_file.name, pat=pat))
 
                 if re.search(pat, cfg_file.name, re.IGNORECASE):
                     method = self.ext_loader[ext_pattern]
                     if self.verbose > 1:
-                        msg = _("Found config file {fi!r}, loader method {m!r}.")
+                        msg = _('Found config file {fi!r}, loader method {m!r}.')
                         LOG.debug(msg.format(fi=str(cfg_file), m=method))
                     if self.additional_config_file:
                         ocfg = self.additional_config_file
                         if ocfg in self.config_files:
                             self.config_files.remove(ocfg)
                     if cfg_file in self.config_files:
                         self.config_files.remove(cfg_file)
                     self.config_files.append(cfg_file)
                     self.config_file_methods[cfg_file] = method
                     performed = True
                     break
 
             if not performed:
                 msg = _(
-                    "Did not found file type of additional config file {fn!r}. "
-                    "Available config types are: {list}.").format(
+                    'Did not found file type of additional config file {fn!r}. '
+                    'Available config types are: {list}.').format(
                     fn=str(cfg_file), list=format_list(self.available_cfg_types))
                 if self.raise_on_error:
                     raise MultiConfigError(msg)
                 LOG.error(msg)
 
     # -------------------------------------------------------------------------
     def _eval_config_dir(self, cfg_dir):
@@ -791,47 +783,47 @@
         file_list = []
         for found_file in cfg_dir.glob('*'):
             file_list.append(found_file)
 
         for type_name in self.available_cfg_types:
 
             if type_name not in self.ext_patterns:
-                msg = _("Something strange is happend, file type {!r} not found.")
+                msg = _('Something strange is happend, file type {!r} not found.')
                 LOG.error(msg.format(type_name))
                 continue
 
             for found_file in file_list:
 
                 if found_file in performed_files:
                     continue
 
                 if self.verbose > 3:
-                    msg = _("Checking, whether {!r} is a possible config file.").format(
+                    msg = _('Checking, whether {!r} is a possible config file.').format(
                         str(found_file))
                     LOG.debug(msg)
                 if not found_file.is_file():
                     if self.verbose > 2:
-                        msg = _("Path {!r} is not a regular file.").format(str(found_file))
+                        msg = _('Path {!r} is not a regular file.').format(str(found_file))
                         LOG.debug(msg)
                     performed_files.append(found_file)
                     continue
 
                 for stem in self.stems:
 
                     for ext_pattern in self.ext_patterns[type_name]:
 
                         pat = r'^' + re.escape(stem) + r'\.' + ext_pattern + r'$'
                         if self.verbose > 3:
-                            LOG.debug(_("Checking file {fn!r} for pattern {pat!r}.").format(
+                            LOG.debug(_('Checking file {fn!r} for pattern {pat!r}.').format(
                                 fn=found_file.name, pat=pat))
 
                         if re.search(pat, found_file.name, re.IGNORECASE):
                             method = self.ext_loader[ext_pattern]
                             if self.verbose > 1:
-                                msg = _("Found config file {fi!r}, loader method {m!r}.").format(
+                                msg = _('Found config file {fi!r}, loader method {m!r}.').format(
                                     fi=str(found_file), m=method)
                                 LOG.debug(msg)
                             if found_file in self.config_files:
                                 self.config_files.remove(found_file)
                             self.config_files.append(found_file)
                             self.config_file_methods[found_file] = method
                             performed_files.append(found_file)
@@ -842,27 +834,27 @@
         if not self.cfgfiles_collected:
             self.collect_config_files()
 
         self.cfg = {}
         for cfg_file in self.config_files:
 
             if self.verbose:
-                LOG.info(_("Reading configuration file {!r} ...").format(str(cfg_file)))
+                LOG.info(_('Reading configuration file {!r} ...').format(str(cfg_file)))
 
             method = self.config_file_methods[cfg_file]
             if self.verbose > 1:
-                LOG.debug(_("Using loading method {!r}.").format(method))
+                LOG.debug(_('Using loading method {!r}.').format(method))
 
             meth = getattr(self, method, None)
             if not meth:
                 raise MultiCfgLoaderNotFoundError(method)
 
             cfg = meth(cfg_file)
             if self.verbose > 3:
-                msg = _("Read config from {fn!r}:").format(fn=str(cfg_file))
+                msg = _('Read config from {fn!r}:').format(fn=str(cfg_file))
                 msg += '\n' + pp(cfg)
                 LOG.debug(msg)
             if cfg and cfg.keys():
                 self.configs_raw[str(cfg_file)] = cfg
                 self.cfg = merge_structure(self.cfg, cfg)
             else:
                 self.configs_raw[str(cfg_file)] = None
@@ -873,121 +865,121 @@
 
     # -------------------------------------------------------------------------
     def detect_file_encoding(self, cfg_file, force=False):
         """Try to detect the encoding of the given file."""
         if not force and not self.use_chardet:
             if self.verbose > 2:
                 LOG.debug(_(
-                    "Character set detection by module {mod!r} for file {fn!r} should not be "
-                    "used, using character set {enc!r}.").format(
+                    'Character set detection by module {mod!r} for file {fn!r} should not be '
+                    'used, using character set {enc!r}.').format(
                     mod='chardet', fn=str(cfg_file), enc=self.encoding))
             return self.encoding
 
         if self.verbose > 1:
-            LOG.debug(_("Trying to detect character set of file {fn!r} ...").format(
+            LOG.debug(_('Trying to detect character set of file {fn!r} ...').format(
                 fn=str(cfg_file)))
 
         encoding = self.encoding
         confidence = 1
         try:
             rawdata = cfg_file.read_bytes()
             chardet_result = chardet.detect(rawdata)
             confidence = chardet_result['confidence']
             if confidence < self.chardet_min_level_confidence:
                 if chardet_result['encoding'] != self.encoding:
                     msg = _(
-                        "The confidence of {con:0.1f}% is lower than the limit of {lim:0.1f}%, "
-                        "using character set {cs_def!r} instead of {cs_found!r}.").format(
+                        'The confidence of {con:0.1f}% is lower than the limit of {lim:0.1f}%, '
+                        'using character set {cs_def!r} instead of {cs_found!r}.').format(
                         con=(chardet_result['confidence'] * 100),
                         lim=(self.chardet_min_level_confidence * 100),
                         cs_def=self.encoding, cs_found=chardet_result['encoding'])
                     LOG.warn(msg)
                 return self.encoding
             encoding = chardet_result['encoding']
         except Exception as e:
-            msg = _("Got {what} on detecting cheracter set of {fn!r}: {e}").format(
+            msg = _('Got {what} on detecting cheracter set of {fn!r}: {e}').format(
                 what=e.__class__.__name__, fn=str(cfg_file), e=e)
             LOG.error(msg)
 
         if self.verbose > 2:
             msg = _(
-                "Found character set {cs!r} for file {fn!r} with a confidence of "
-                "{con:0.1f}%.").format(cs=encoding, fn=str(cfg_file), con=(confidence * 100))
+                'Found character set {cs!r} for file {fn!r} with a confidence of '
+                '{con:0.1f}%.').format(cs=encoding, fn=str(cfg_file), con=(confidence * 100))
             LOG.debug(msg)
 
         return encoding
 
     # -------------------------------------------------------------------------
     def load_json(self, cfg_file):
         """Read and load the given file as a JSON file."""
-        LOG.debug(_("Reading {tp} file {fn!r} ...").format(tp='JSON', fn=str(cfg_file)))
+        LOG.debug(_('Reading {tp} file {fn!r} ...').format(tp='JSON', fn=str(cfg_file)))
 
         open_opts = {
             'encoding': UTF8_ENCODING,
             'errors': 'surrogateescape',
         }
 
         try:
             with cfg_file.open('r', **open_opts) as fh:
                 js = json.load(fh)
         except json.JSONDecodeError as e:
-            msg = _("{what} parse error in {fn!r}, line {line}, column {col}: {msg}").format(
+            msg = _('{what} parse error in {fn!r}, line {line}, column {col}: {msg}').format(
                 what='JSON', fn=str(cfg_file), line=e.lineno, col=e.colno, msg=e.msg)
             if self.raise_on_error:
                 raise MultiCfgParseError(msg)
             LOG.error(msg)
             return None
         except Exception as e:
-            msg = _("Got {what} on reading and parsing {fn!r}: {e}").format(
+            msg = _('Got {what} on reading and parsing {fn!r}: {e}').format(
                 what=e.__class__.__name__, fn=str(cfg_file), e=e)
             if self.raise_on_error:
                 raise MultiCfgParseError(msg)
             LOG.error(msg)
             return None
 
         return js
 
     # -------------------------------------------------------------------------
     def load_hjson(self, cfg_file):
         """Read and load the given file as an human readable JSON file."""
-        LOG.debug(_("Reading {tp} file {fn!r} ...").format(
+        LOG.debug(_('Reading {tp} file {fn!r} ...').format(
             tp='human readable JSON', fn=str(cfg_file)))
 
         encoding = self.detect_file_encoding(cfg_file)
 
         open_opts = {
             'encoding': encoding,
             'errors': 'surrogateescape',
         }
 
         js = {}
         try:
             with cfg_file.open('r', **open_opts) as fh:
                 js = hjson.load(fh)
         except hjson.HjsonDecodeError as e:
-            msg = _("{what} parse error in {fn!r}, line {line}, column {col}: {msg}").format(
+            msg = _('{what} parse error in {fn!r}, line {line}, column {col}: {msg}').format(
                 what='HJSON', fn=str(cfg_file), line=e.lineno, col=e.colno, msg=e.msg)
             if self.raise_on_error:
                 raise MultiCfgParseError(msg)
             LOG.error(msg)
             return None
         except Exception as e:
-            msg = _("Got {what} on reading and parsing {fn!r}: {e}").format(
+            msg = _('Got {what} on reading and parsing {fn!r}: {e}').format(
                 what=e.__class__.__name__, fn=str(cfg_file), e=e)
             if self.raise_on_error:
                 raise MultiCfgParseError(msg)
             LOG.error(msg)
             return None
 
         return js
 
     # -------------------------------------------------------------------------
     def load_ini(self, cfg_file):
         """Read and load the given file as an INI file."""
-        LOG.debug(_("Reading {tp} file {fn!r} ...").format(tp='INI', fn=str(cfg_file)))
+        LOG.debug(_('Reading {tp} file {fn!r} ...').format(tp='INI', fn=str(cfg_file)))
 
         kargs = {
             'allow_no_value': self.ini_allow_no_value,
             'strict': self.ini_strict,
             'empty_lines_in_values': self.ini_empty_lines_in_values,
         }
         if self.ini_delimiters:
@@ -996,33 +988,33 @@
             kargs['comment_prefixes'] = self.ini_comment_prefixes
         if self.ini_inline_comment_prefixes:
             kargs['cinline_omment_prefixes'] = self.ini_inline_comment_prefixes
         if self.ini_extended_interpolation:
             kargs['interpolation'] = ExtendedInterpolation
 
         if self.verbose > 1:
-            LOG.debug(_("Arguments on initializing {}:").format('ConfigParser') + "\n" + pp(kargs))
+            LOG.debug(_('Arguments on initializing {}:').format('ConfigParser') + '\n' + pp(kargs))
 
         parser = configparser.ConfigParser(**kargs)
 
         encoding = self.detect_file_encoding(cfg_file)
 
         open_opts = {
             'encoding': encoding,
             'errors': 'surrogateescape',
         }
 
         cfg = {}
 
         try:
             with cfg_file.open('r', **open_opts) as fh:
-                stream = StringIO("[/]\n" + fh.read())
+                stream = StringIO('[/]\n' + fh.read())
                 parser.read_file(stream)
         except Exception as e:
-            msg = _("Got {what} on reading and parsing {fn!r}: {e}").format(
+            msg = _('Got {what} on reading and parsing {fn!r}: {e}').format(
                 what=e.__class__.__name__, fn=str(cfg_file), e=e)
             if self.raise_on_error:
                 raise MultiCfgParseError(msg)
             LOG.error(msg)
             return None
 
         for section in parser.sections():
@@ -1036,79 +1028,79 @@
             del cfg['/']
 
         return cfg
 
     # -------------------------------------------------------------------------
     def load_toml(self, cfg_file):
         """Read and load the given file as a TOML file."""
-        LOG.debug(_("Reading {tp} file {fn!r} ...").format(tp='TOML', fn=str(cfg_file)))
+        LOG.debug(_('Reading {tp} file {fn!r} ...').format(tp='TOML', fn=str(cfg_file)))
 
         cfg = {}
 
         try:
             cfg = toml.load(cfg_file)
         except TomlDecodeError as e:
-            msg = _("{what} parse error in {fn!r}, line {line}, column {col}: {msg}").format(
+            msg = _('{what} parse error in {fn!r}, line {line}, column {col}: {msg}').format(
                 what='TOML', fn=str(cfg_file), line=e.lineno, col=e.colno, msg=e.msg)
             if self.raise_on_error:
                 raise MultiCfgParseError(msg)
             LOG.error(msg)
             return None
         except Exception as e:
-            msg = _("Got {what} on reading and parsing {fn!r}: {e}").format(
+            msg = _('Got {what} on reading and parsing {fn!r}: {e}').format(
                 what=e.__class__.__name__, fn=str(cfg_file), e=e)
             if self.raise_on_error:
                 raise MultiCfgParseError(msg)
             LOG.error(msg)
             return None
 
         return cfg
 
     # -------------------------------------------------------------------------
     def load_yaml(self, cfg_file):
         """Read and load the given file as a YAML file."""
-        LOG.debug(_("Reading {tp} file {fn!r} ...").format(tp='YAML', fn=str(cfg_file)))
+        LOG.debug(_('Reading {tp} file {fn!r} ...').format(tp='YAML', fn=str(cfg_file)))
 
         open_opts = {
             'encoding': UTF8_ENCODING,
             'errors': 'surrogateescape',
         }
 
         cfg = {}
         try:
             with cfg_file.open('r', **open_opts) as fh:
                 cfg = yaml.safe_load(fh)
         except yaml.YAMLError as e:
             if hasattr(e, 'problem_mark'):
                 mark = e.problem_mark
-                msg = _("{what} parse error in {fn!r}, line {line}, column {col}: {msg}").format(
+                msg = _('{what} parse error in {fn!r}, line {line}, column {col}: {msg}').format(
                     what='YAML', fn=str(cfg_file),
                     line=(mark.line + 1), col=(mark.column + 1), msg=str(e))
             else:
-                msg = _("Got {what} on reading and parsing {fn!r}: {e}").format(
+                msg = _('Got {what} on reading and parsing {fn!r}: {e}').format(
                     what=e.__class__.__name__, fn=str(cfg_file), e=e)
             if self.raise_on_error:
                 raise MultiCfgParseError(msg)
             LOG.error(msg)
             return None
         except Exception as e:
-            msg = _("Got {what} on reading and parsing {fn!r}: {e}").format(
+            msg = _('Got {what} on reading and parsing {fn!r}: {e}').format(
                 what=e.__class__.__name__, fn=str(cfg_file), e=e)
             if self.raise_on_error:
                 raise MultiCfgParseError(msg)
             LOG.error(msg)
             return None
 
         return cfg
 
     # -------------------------------------------------------------------------
-    def eval(self):
+    def eval(self):                                                         # noqa: A003
         """Evaluate configuration and store it in object properties."""
         if not self.was_read:
-            msg = _("Evaluation of configuration could only be happen after reading it.")
+            msg = _('Evaluation of configuration could only be happen after reading it.')
             raise RuntimeError(msg)
 
         for section_name in self.cfg.keys():
 
             if section_name.lower() in ('default', 'global', 'common'):
                 self.eval_global_section(section_name)
                 continue
@@ -1117,18 +1109,18 @@
     # -------------------------------------------------------------------------
     def eval_global_section(self, section_name):
         """Evaluate section [global] of configuration.
 
         May be overridden in descendant classes.
         """
         if self.verbose > 1:
-            LOG.debug(_("Checking config section {!r} ...").format(section_name))
+            LOG.debug(_('Checking config section {!r} ...').format(section_name))
 
         max_timeout = HandlingObject.max_prompt_timeout
-        invalid_msg = _("Invalid value {val!r} in section {sec!r} for console timeout.")
+        invalid_msg = _('Invalid value {val!r} in section {sec!r} for console timeout.')
 
         config = self.cfg[section_name]
         for key in config.keys():
             value = config[key]
             if key.lower() == 'verbose':
                 val = 0
                 if value is None:
@@ -1148,16 +1140,16 @@
                 except (ValueError, TypeError) as e:
                     msg = invalid_msg.format(val=value, sec=section_name)
                     msg += ' ' + str(e)
                     LOG.error(msg)
                     continue
                 if timeout <= 0 or timeout > max_timeout:
                     msg = invalid_msg.format(val=value, sec=section_name)
-                    msg += " " + _(
-                        "A timeout must be greater than zero and less or equal to {}.").format(
+                    msg += ' ' + _(
+                        'A timeout must be greater than zero and less or equal to {}.').format(
                         max_timeout)
                     LOG.error(msg)
                     continue
                 self._prompt_timeout = timeout
                 continue
 
             if key.lower() in ('logfile', 'log-file', 'log'):
@@ -1171,14 +1163,14 @@
         Should be overridden in descendant classes.
         """
         pass
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/obj.py` & `fb_tools-2.2.3/lib/fb_tools/obj.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: Module for base object classes, which are used everywhere in my projects.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import sys
-import os
-import logging
 import datetime
+import logging
+import os
+import sys
 import traceback
-
+from abc import ABCMeta, abstractmethod
 try:
     import pathlib
 except ImportError:
     import pathlib2 as pathlib
 
-from abc import ABCMeta, abstractmethod
-
 # Third party modules
-
 from six import add_metaclass
 
 # Own modules
 from .common import pp, to_bytes
-
 from .errors import FbError
-
 from .xlate import XLATOR
 
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
@@ -57,16 +52,16 @@
         """Initialise a BasedirNotExistingError exception."""
         self.dir_name = dir_name
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into a string object."""
         msg = _(
-            "The base directory {!r} is not existing or not "
-            "a directory.").format(str(self.dir_name))
+            'The base directory {!r} is not existing or not '
+            'a directory.').format(str(self.dir_name))
         return msg
 
 
 # =============================================================================
 @add_metaclass(ABCMeta)
 class FbGenericBaseObject(object):
     """Base class for all and everything.
@@ -93,15 +88,15 @@
         """
         return pp(self.as_dict(short=True))
 
     # -------------------------------------------------------------------------
     @abstractmethod
     def __repr__(self):
         """Typecast into a string for reproduction."""
-        out = "<%s()>" % (self.__class__.__name__)
+        out = '<%s()>' % (self.__class__.__name__)
         return out
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
         Transform the elements of the object into a dict.
 
@@ -162,16 +157,16 @@
 
         if has_handlers:
             LOG.error(msg)
             if do_traceback:
                 LOG.error(traceback.format_exc())
         else:
             curdate = datetime.datetime.now()
-            curdate_str = "[" + curdate.isoformat(' ') + "]: "
-            msg = curdate_str + msg + "\n"
+            curdate_str = '[' + curdate.isoformat(' ') + ']: '
+            msg = curdate_str + msg + '\n'
             if hasattr(sys.stderr, 'buffer'):
                 sys.stderr.buffer.write(to_bytes(msg))
             else:
                 sys.stderr.write(msg)
             if do_traceback:
                 traceback.print_exc()
 
@@ -202,16 +197,16 @@
         if root_log.handlers:
             has_handlers = True
 
         if has_handlers:
             LOG.info(msg)
         else:
             curdate = datetime.datetime.now()
-            curdate_str = "[" + curdate.isoformat(' ') + "]: "
-            msg = curdate_str + msg + "\n"
+            curdate_str = '[' + curdate.isoformat(' ') + ']: '
+            msg = curdate_str + msg + '\n'
             if hasattr(sys.stderr, 'buffer'):
                 sys.stderr.buffer.write(to_bytes(msg))
             else:
                 sys.stderr.write(msg)
 
         return
 
@@ -245,15 +240,15 @@
 
         self._verbose = int(verbose)
         """
         @ivar: verbosity level (0 - 9)
         @type: int
         """
         if self._verbose < 0:
-            msg = _("Wrong verbose level {!r}, must be >= 0").format(verbose)
+            msg = _('Wrong verbose level {!r}, must be >= 0').format(verbose)
             raise ValueError(msg)
 
         self._initialized = False
         """
         @ivar: initialisation of this object is complete
                after __init__() of this object
         @type: bool
@@ -301,15 +296,15 @@
 
     @verbose.setter
     def verbose(self, value):
         v = int(value)
         if v >= 0:
             self._verbose = v
         else:
-            LOG.warning(_("Wrong verbose level {!r}, must be >= 0").format(value))
+            LOG.warning(_('Wrong verbose level {!r}, must be >= 0').format(value))
 
     # -----------------------------------------------------------
     @property
     def initialized(self):
         """Return whther the initialisation of this object is complete."""
         return getattr(self, '_initialized', False)
 
@@ -325,35 +320,35 @@
 
     @base_dir.setter
     def base_dir(self, value):
         base_dir_path = pathlib.Path(value)
         if str(base_dir_path).startswith('~'):
             base_dir_path = base_dir_path.expanduser()
         if not base_dir_path.exists():
-            msg = _("Base directory {!r} does not exists.").format(str(value))
+            msg = _('Base directory {!r} does not exists.').format(str(value))
             self.handle_error(msg, self.appname)
         elif not base_dir_path.is_dir():
-            msg = _("Path for base directory {!r} is not a directory.").format(str(value))
+            msg = _('Path for base directory {!r} is not a directory.').format(str(value))
             self.handle_error(msg, self.appname)
         else:
             self._base_dir = base_dir_path
 
     # -------------------------------------------------------------------------
     def __repr__(self):
         """Typecasting into a string for reproduction."""
-        out = "<%s(" % (self.__class__.__name__)
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
-        fields.append("appname={!r}".format(self.appname))
-        fields.append("verbose={!r}".format(self.verbose))
-        fields.append("version={!r}".format(self.version))
-        fields.append("base_dir={!r}".format(self.base_dir))
-        fields.append("initialized={!r}".format(self.initialized))
+        fields.append('appname={!r}'.format(self.appname))
+        fields.append('verbose={!r}'.format(self.verbose))
+        fields.append('version={!r}'.format(self.version))
+        fields.append('base_dir={!r}'.format(self.base_dir))
+        fields.append('initialized={!r}'.format(self.initialized))
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
         Transform the elements of the object into a dict.
 
@@ -372,14 +367,14 @@
         res['base_dir'] = self.base_dir
 
         return res
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/pidfile.py` & `fb_tools-2.2.3/lib/fb_tools/pidfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,41 +3,38 @@
 """
 @summary: A module for a pidfile object.
 
 It provides methods to define, check, create and remove a pidfile.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import os
-import sys
+import errno
 import logging
-
+import os
 import re
 import signal
-import errno
-
+import sys
 from pathlib import Path
 
 # Third party modules
 import six
 from six import reraise
 
 # Own modules
-from .errors import ReadTimeoutError
 from .common import to_utf8
-from .obj import FbBaseObjectError, FbBaseObject
-
+from .errors import ReadTimeoutError
+from .obj import FbBaseObject, FbBaseObjectError
 from .xlate import XLATOR
 
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
@@ -65,18 +62,18 @@
         self.reason = reason
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecaste into a string for error output."""
         msg = None
         if self.reason:
-            msg = _("Invalid pidfile {f!r} given: {r}").format(
+            msg = _('Invalid pidfile {f!r} given: {r}').format(
                 f=str(self.pidfile), r=self.reason)
         else:
-            msg = _("Invalid pidfile {!r} given.").format(str(self.pidfile))
+            msg = _('Invalid pidfile {!r} given.').format(str(self.pidfile))
 
         return msg
 
 # =============================================================================
 class PidFileInUseError(PidFileError):
     """Exception indicating, that the pidfile is in use."""
 
@@ -93,15 +90,15 @@
         self.pidfile = pidfile
         self.pid = pid
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecaste into a string for error output."""
         msg = _(
-            "The pidfile {f!r} is currently in use by the application with the PID {p}.").format(
+            'The pidfile {f!r} is currently in use by the application with the PID {p}.').format(
             f=str(self.pidfile), p=self.pid)
 
         return msg
 
 
 # =============================================================================
 class PidFile(FbBaseObject):
@@ -251,27 +248,27 @@
         res['open_args'] = self.open_args
 
         return res
 
     # -------------------------------------------------------------------------
     def __repr__(self):
         """Typecaste into a string for reproduction."""
-        out = "<%s(" % (self.__class__.__name__)
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
-        fields.append("filename={!r}".format(str(self.filename)))
-        fields.append("auto_remove={!r}".format(self.auto_remove))
-        fields.append("appname={!r}".format(self.appname))
-        fields.append("verbose={!r}".format(self.verbose))
-        fields.append("base_dir={!r}".format(str(self.base_dir)))
-        fields.append("initialized={!r}".format(self.initialized))
-        fields.append("simulate={!r}".format(self.simulate))
-        fields.append("timeout={!r}".format(self.timeout))
+        fields.append('filename={!r}'.format(str(self.filename)))
+        fields.append('auto_remove={!r}'.format(self.auto_remove))
+        fields.append('appname={!r}'.format(self.appname))
+        fields.append('verbose={!r}'.format(self.verbose))
+        fields.append('base_dir={!r}'.format(str(self.base_dir)))
+        fields.append('initialized={!r}'.format(self.initialized))
+        fields.append('simulate={!r}'.format(self.simulate))
+        fields.append('timeout={!r}'.format(self.timeout))
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def __del__(self):
         """Destruct the object.
 
         Remove the pidfile, if it was created by ourselfes.
@@ -288,23 +285,23 @@
         if not self.auto_remove:
             if self.verbose > 3:
                 LOG.debug(_("Auto removing disabled, don't deleting {!r}.").format(
                     str(self.filename)))
             return
 
         if self.verbose > 1:
-            LOG.debug(_("Removing pidfile {!r} ...").format(str(self.filename)))
+            LOG.debug(_('Removing pidfile {!r} ...').format(str(self.filename)))
         if self.simulate:
             if self.verbose > 1:
-                LOG.debug(_("Just kidding ..."))
+                LOG.debug(_('Just kidding ...'))
             return
         try:
             self.filename.unlink()
         except OSError as e:
-            LOG.err(_("Could not delete pidfile {f!r}: {e}").format(f=str(self.filename), e=e))
+            LOG.err(_('Could not delete pidfile {f!r}: {e}').format(f=str(self.filename), e=e))
         except Exception as e:
             self.handle_error(str(e), e.__class__.__name__, True)
 
     # -------------------------------------------------------------------------
     def create(self, pid=None):
         """Create the f***ing pidfile.
 
@@ -315,53 +312,53 @@
                     the current process will taken.
         @type pid: int
 
         """
         if pid:
             pid = int(pid)
             if pid <= 0:
-                msg = _("Invalid PID {p} for creating pidfile {f!r} given.").format(
+                msg = _('Invalid PID {p} for creating pidfile {f!r} given.').format(
                     p=pid, f=str(self.filename))
                 raise PidFileError(msg)
         else:
             pid = os.getpid()
 
         if self.check():
 
-            LOG.info(_("Deleting pidfile {!r} ...").format(str(self.filename)))
+            LOG.info(_('Deleting pidfile {!r} ...').format(str(self.filename)))
             if self.simulate:
-                LOG.debug(_("Just kidding ..."))
+                LOG.debug(_('Just kidding ...'))
             else:
                 try:
                     self.filename.unlink()
                 except OSError as e:
                     raise InvalidPidFileError(self.filename, str(e))
 
         if self.verbose > 1:
-            LOG.debug(_("Trying opening {!r} exclusive ...").format(str(self.filename)))
+            LOG.debug(_('Trying opening {!r} exclusive ...').format(str(self.filename)))
 
         if self.simulate:
             LOG.debug(_("Simulation mode - don't real writing in {!r}.").format(
                 str(self.filename)))
             self._created = True
             return
 
         fd = None
         try:
             fd = os.open(
                 str(self.filename), os.O_CREAT | os.O_EXCL | os.O_WRONLY, 0o644)
         except OSError as e:
             error_tuple = sys.exc_info()
-            msg = _("Error on creating pidfile {f!r}: {e}").format(f=str(self.filename), e=e)
+            msg = _('Error on creating pidfile {f!r}: {e}').format(f=str(self.filename), e=e)
             reraise(PidFileError, msg, error_tuple[2])
 
         if self.verbose > 2:
-            LOG.debug(_("Writing {p} into {f!r} ...").format(p=pid, f=str(self.filename)))
+            LOG.debug(_('Writing {p} into {f!r} ...').format(p=pid, f=str(self.filename)))
 
-        out = to_utf8("{}\n".format(pid))
+        out = to_utf8('{}\n'.format(pid))
         try:
             os.write(fd, out)
         finally:
             os.close(fd)
 
         self._created = True
 
@@ -372,43 +369,43 @@
 
         @param pid: the pid to write into the pidfile. If not given, the PID of
                     the current process will taken.
         @type pid: int
 
         """
         if not self.created:
-            msg = _("Calling {} on a not self created pidfile.").format('recreate()')
+            msg = _('Calling {} on a not self created pidfile.').format('recreate()')
             raise PidFileError(msg)
 
         if pid:
             pid = int(pid)
             if pid <= 0:
-                msg = "Invalid PID {p} for creating pidfile {f!r} given.".format(
+                msg = _('Invalid PID {p} for creating pidfile {f!r} given.').format(
                     p=pid, f=str(self.filename))
                 raise PidFileError(msg)
         else:
             pid = os.getpid()
 
         if self.verbose > 1:
-            LOG.debug(_("Trying opening {!r} for recreate ...").format(str(self.filename)))
+            LOG.debug(_('Trying opening {!r} for recreate ...').format(str(self.filename)))
 
         if self.simulate:
             LOG.debug(_("Simulation mode - don't real writing in {!r}.").format(
                 str(self.filename)))
             return
 
-        out = to_utf8("{}\n".format(pid))
+        out = to_utf8('{}\n'.format(pid))
         if self.verbose > 2:
-            LOG.debug(_("Writing {p} into {f!r} ...").format(p=pid, f=str(self.filename)))
+            LOG.debug(_('Writing {p} into {f!r} ...').format(p=pid, f=str(self.filename)))
 
         try:
             self.filename.write_text(out, **self.open_args)
         except OSError as e:
             error_tuple = sys.exc_info()
-            msg = _("Error on recreating pidfile {f!r}: {e}").format(
+            msg = _('Error on recreating pidfile {f!r}: {e}').format(
                 f=str(self.filename), e=e)
             reraise(PidFileError, msg, error_tuple[2])
 
     # -------------------------------------------------------------------------
     def check(self):
         """
         Check the usability of the pidfile.
@@ -430,26 +427,26 @@
         """
         if not self.filename.exists():
             if not self.parent_dir.exists():
                 reason = _("Pidfile parent directory {!r} doesn't exists.").format(
                     str(self.parent_dir))
                 raise InvalidPidFileError(self.filename, reason)
             if not self.parent_dir.is_dir():
-                reason = _("Pidfile parent directory {!r} is not a directory.").format(
+                reason = _('Pidfile parent directory {!r} is not a directory.').format(
                     str(self.parent_dir))
                 raise InvalidPidFileError(self.filename, reason)
             if not os.access(self.parent_dir, os.X_OK):
-                reason = _("No write access to pidfile parent directory {!r}.").format(
+                reason = _('No write access to pidfile parent directory {!r}.').format(
                     str(self.parent_dir))
                 raise InvalidPidFileError(self.filename, reason)
 
             return False
 
         if not self.filename.is_file():
-            reason = _("It is not a regular file.")
+            reason = _('It is not a regular file.')
             raise InvalidPidFileError(self.filename, reason)
 
         # ---------
         def pidfile_read_alarm_caller(signum, sigframe):
             """
             Raise a ReadTimeoutError on a timeout alarm.
 
@@ -459,15 +456,15 @@
             @type signum: int
             @param sigframe: the frame of the signal
             @type sigframe: object
             """
             raise ReadTimeoutError(self.timeout, str(self.filename))
 
         if self.verbose > 1:
-            LOG.debug(_("Reading content of pidfile {!r} ...").format(
+            LOG.debug(_('Reading content of pidfile {!r} ...').format(
                 str(self.filename)))
 
         signal.signal(signal.SIGALRM, pidfile_read_alarm_caller)
         signal.alarm(self.timeout)
 
         content = ''
 
@@ -480,43 +477,43 @@
 
         pid = None
         line = content.strip()
         match = re.search(r'^\s*(\d+)\s*$', line)
         if match:
             pid = int(match.group(1))
         else:
-            msg = _("No useful information found in pidfile {f!r}: {z!r}").format(
+            msg = _('No useful information found in pidfile {f!r}: {z!r}').format(
                 f=str(self.filename), z=line)
             return True
 
         if self.verbose > 1:
-            LOG.debug(_("Trying check for process with PID {} ...").format(pid))
+            LOG.debug(_('Trying check for process with PID {} ...').format(pid))
 
         try:
             os.kill(pid, 0)
         except OSError as err:
             if err.errno == errno.ESRCH:
-                LOG.info(_("Process with PID {} anonymous died.").format(pid))
+                LOG.info(_('Process with PID {} anonymous died.').format(pid))
                 return True
             elif err.errno == errno.EPERM:
                 error_tuple = sys.exc_info()
-                msg = _("No permission to signal the process {} ...").format(pid)
+                msg = _('No permission to signal the process {} ...').format(pid)
                 reraise(PidFileError, msg, error_tuple[2])
             else:
                 error_tuple = sys.exc_info()
-                msg = _("Got a {c}: {e}.").format(err.__class__.__name__, err)
+                msg = _('Got a {c}: {e}.').format(err.__class__.__name__, err)
                 reraise(PidFileError, msg, error_tuple[2])
         else:
             raise PidFileInUseError(self.filename, pid)
 
         return False
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_tools-2.2.2/lib/fb_tools/xlate.py` & `fb_tools-2.2.3/lib/fb_tools/xlate.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 """
 @summary: The module for i18n.
 
 It provides translation object, usable from all other modules in this package.
 
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 by Frank Brehm, Berlin
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
-import logging
-import gettext
 import copy
+import gettext
+import logging
 import sys
-
 try:
     from pathlib import Path
 except ImportError:
     from pathlib2 import Path
 
 # Third party modules
 import babel
@@ -32,15 +31,15 @@
 except ImportError:
     from distutils.version import LooseVersion as Version
 
 DOMAIN = 'fb_tools'
 
 LOG = logging.getLogger(__name__)
 
-__version__ = '2.0.2'
+__version__ = '2.0.3'
 
 __me__ = Path(__file__).resolve()
 __module_dir__ = __me__.parent
 __lib_dir__ = __module_dir__.parent
 __base_dir__ = __lib_dir__.parent
 LOCALE_DIR = __base_dir__.joinpath('locale')
 if LOCALE_DIR.is_dir():
@@ -98,18 +97,18 @@
     if CUR_BABEL_VERSION < NEWER_BABEL_VERSION:
         return babel.lists.format_list(my_list, locale=locale)
     return babel.lists.format_list(my_list, style=style, locale=locale)
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
-    print(_("Module directory: {!r}").format(__module_dir__))
-    print(_("Base directory: {!r}").format(__base_dir__))
-    print(_("Locale directory: {!r}").format(LOCALE_DIR))
-    print(_("Locale domain: {!r}").format(DOMAIN))
-    print(_("Found .mo-file: {!r}").format(__mo_file__))
+    print(_('Module directory: {!r}').format(__module_dir__))
+    print(_('Base directory: {!r}').format(__base_dir__))
+    print(_('Locale directory: {!r}').format(LOCALE_DIR))
+    print(_('Locale domain: {!r}').format(DOMAIN))
+    print(_('Found .mo-file: {!r}').format(__mo_file__))
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

### Comparing `fb_tools-2.2.2/lib/fb_tools.egg-info/PKG-INFO` & `fb_tools-2.2.3/lib/fb_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-tools
-Version: 2.2.2
+Version: 2.2.3
 Summary: Modules for common used objects, error classes and methods.
 Home-page: https://github.com/fbrehm/python_fb_tools
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_tools-2.2.2/lib/fb_tools.egg-info/SOURCES.txt` & `fb_tools-2.2.3/lib/fb_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.2/locale/de/LC_MESSAGES/fb_tools.mo` & `fb_tools-2.2.3/locale/de/LC_MESSAGES/fb_tools.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: fb_tools 2.1.2\n"
+"Project-Id-Version: fb_tools 2.2.3\n"
 "Report-Msgid-Bugs-To: frank@brehm-online.com\n"
-"POT-Creation-Date: 2022-11-21 14:24+0100\n"
-"PO-Revision-Date: 2022-10-14 17:00+0200\n"
+"POT-Creation-Date: 2023-05-31 14:28+0200\n"
+"PO-Revision-Date: 2023-05-31 17:30+0200\n"
 "Last-Translator: Frank Brehm <frank@brehm-online.com>\n"
 "Language: de\n"
 "Language-Team: de <frank@brehm-online.com>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "   {w} is now: {o!r}"
 msgstr "   {w} ist jetzt: {o!r}"
 
 msgid " (timeout after {:0.1f} secs)"
 msgstr " (Timeout nach {:0.1f} Sekunden)"
```

### Comparing `fb_tools-2.2.2/locale/de/LC_MESSAGES/fb_tools.po` & `fb_tools-2.2.3/locale/de/LC_MESSAGES/fb_tools.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,181 +1,181 @@
 # German translations for fb_tools.
-# Copyright (C) 2022 Frank Brehm, Berlin
+# Copyright (C) 2023 Frank Brehm, Berlin
 # This file is distributed under the same license as the fb_tools project.
-# Frank Brehm <frank.brehm@pixelpark.com>, 2022.
+# Frank Brehm <frank@brehm-online.com>, 2023.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: fb_tools 2.1.2\n"
+"Project-Id-Version: fb_tools 2.2.3\n"
 "Report-Msgid-Bugs-To: frank@brehm-online.com\n"
-"POT-Creation-Date: 2022-11-21 14:24+0100\n"
-"PO-Revision-Date: 2022-10-14 17:00+0200\n"
+"POT-Creation-Date: 2023-05-31 14:28+0200\n"
+"PO-Revision-Date: 2023-05-31 17:30+0200\n"
 "Last-Translator: Frank Brehm <frank@brehm-online.com>\n"
 "Language: de\n"
 "Language-Team: de <frank@brehm-online.com>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 #: bin/get-file-to-remove:84
 msgid ""
 "{c}-Object:\n"
 "{a}"
 msgstr ""
 "{c}-Objekt:\n"
 "{a}"
 
-#: lib/fb_tools/app.py:69
+#: lib/fb_tools/app.py:64
 msgid "Forced execution - whatever it means."
 msgstr "Forcierte Ausführung, was auch immer das bedeuten mag."
 
-#: lib/fb_tools/app.py:151
+#: lib/fb_tools/app.py:146
 msgid "Invalid env_prefix {!r} given - it may not be empty."
 msgstr "Ungültiger env_prefix {!r} übergeben - er darf nicht leer sein."
 
-#: lib/fb_tools/app.py:155
+#: lib/fb_tools/app.py:150
 msgid ""
 "Invalid characters found in env_prefix {!r}, only alphanumeric characters and digits and "
 "underscore (this not as the first character) are allowed."
 msgstr ""
 "Ungültige Zeichen in env_prefix {!r} gefunden, nur alphanumerische Zeichen und Unterstriche "
 "(diese aber nicht als erstes Zeichen) sind erlaubt."
 
-#: lib/fb_tools/app.py:166
+#: lib/fb_tools/app.py:161
 msgid "Unknown and undescriped application."
 msgstr "Unbekannte und nicht beschriebene Anwendung."
 
-#: lib/fb_tools/app.py:191
+#: lib/fb_tools/app.py:186
 msgid "Wrong exit_value {!r}, must be >= 0."
 msgstr "Falscher Wert für exit_value {!r}, muss größer als oder gleich Null sein."
 
-#: lib/fb_tools/app.py:428
+#: lib/fb_tools/app.py:423
 msgid "Trying to get {} via console ..."
 msgstr "Versuche {} über die Konsole zu bekommen …"
 
-#: lib/fb_tools/app.py:444
+#: lib/fb_tools/app.py:439
 msgid "Got a signal {}."
 msgstr "Erhielt ein Signal {}."
 
-#: lib/fb_tools/app.py:447
+#: lib/fb_tools/app.py:442
 msgid "Got a signal {n!r} ({s})."
 msgstr "Erhielt ein Signal {n!r} ({s})."
 
-#: lib/fb_tools/app.py:454
+#: lib/fb_tools/app.py:449
 msgid "Exit on signal {n!r} ({s})."
 msgstr "Beendigung auf Signal {n!r} ({s})."
 
-#: lib/fb_tools/app.py:462
+#: lib/fb_tools/app.py:457
 msgid "Tweaking signal handlers."
 msgstr "Schraube an den Signalhandlern."
 
-#: lib/fb_tools/app.py:468
+#: lib/fb_tools/app.py:463
 msgid "Setting signal handler for {n!r} ({s})."
 msgstr "Setze Signalhandler für {n!r} ({s})."
 
-#: lib/fb_tools/app.py:479
+#: lib/fb_tools/app.py:474
 msgid "Enter "
 msgstr "Eingabe von "
 
-#: lib/fb_tools/app.py:486
+#: lib/fb_tools/app.py:481
 msgid "Repeat enter "
 msgstr "Wiederholen der Eingabe von "
 
-#: lib/fb_tools/app.py:496
+#: lib/fb_tools/app.py:491
 msgid "{n} and repeated {n} did not match."
 msgstr "{n} und das wiederholte {n} stimmen nicht überein."
 
-#: lib/fb_tools/app.py:500
+#: lib/fb_tools/app.py:495
 msgid "Restoring original signal handlers."
 msgstr "Stelle original Signalhandler wieder her."
 
-#: lib/fb_tools/app.py:505
+#: lib/fb_tools/app.py:500
 msgid "Got {n!r}: {s!r}"
 msgstr "Erhielt {n!r}: {s!r}"
 
-#: lib/fb_tools/app.py:555
+#: lib/fb_tools/app.py:550
 msgid "The application is not completely initialized."
 msgstr "Die Anwendung ist nicht vollständig initialisiert."
 
-#: lib/fb_tools/app.py:566
+#: lib/fb_tools/app.py:561
 msgid "Object {!r} seems not to be completely initialized."
 msgstr "Das {!r}-Objekt scheit noch nicht vollständig initialisiert zu sein."
 
-#: lib/fb_tools/app.py:576
+#: lib/fb_tools/app.py:571
 msgid "Ending."
 msgstr "Beenden."
 
-#: lib/fb_tools/app.py:594
+#: lib/fb_tools/app.py:589
 msgid "Executing {} ..."
 msgstr "Führe {} aus …"
 
-#: lib/fb_tools/app.py:616
+#: lib/fb_tools/app.py:611
 msgid "General options"
 msgstr "Allgemeine Optionen"
 
-#: lib/fb_tools/app.py:621
+#: lib/fb_tools/app.py:616
 msgid "Simulation mode, nothing is really done."
 msgstr "Simulations-Modus, es wird nichts wirklich verändert."
 
-#: lib/fb_tools/app.py:635 lib/fb_tools/app.py:641
+#: lib/fb_tools/app.py:630 lib/fb_tools/app.py:636
 msgid "Automatically answer '{}' for all questions."
 msgstr "Automatisch alle Fragen mit {} beantworten."
 
-#: lib/fb_tools/app.py:636 lib/fb_tools/handling_obj.py:941
+#: lib/fb_tools/app.py:631 lib/fb_tools/handling_obj.py:936
 msgid "Yes"
 msgstr "Ja"
 
-#: lib/fb_tools/app.py:642 lib/fb_tools/handling_obj.py:939
+#: lib/fb_tools/app.py:637 lib/fb_tools/handling_obj.py:934
 msgid "No"
 msgstr "Nein"
 
-#: lib/fb_tools/app.py:647 lib/fb_tools/ddns/__init__.py:249
+#: lib/fb_tools/app.py:642 lib/fb_tools/ddns/__init__.py:243
 msgid "SECONDS"
 msgstr "SEKUNDEN"
 
-#: lib/fb_tools/app.py:649
+#: lib/fb_tools/app.py:644
 msgid "The timeout in seconds for console input. Default: {}"
 msgstr "Die Zeit für die Zeitüberschreitung in Sekunden für Konsolen-Eingaben Vorgabe: {}."
 
-#: lib/fb_tools/app.py:656
+#: lib/fb_tools/app.py:651
 msgid "Use colored output for messages."
 msgstr "Verwenden kolorierter Ausgabe für Mitteilungen."
 
-#: lib/fb_tools/app.py:663
+#: lib/fb_tools/app.py:658
 msgid "Increase the verbosity level"
 msgstr "Erhöhen des Ausführichkeits-Niveaus"
 
-#: lib/fb_tools/app.py:668
+#: lib/fb_tools/app.py:663
 msgid "Silent execution, only warnings and errors are emitted."
 msgstr "Stillschweigende Ausführung, nur Warnungen und Fehler werden ausgegeben."
 
-#: lib/fb_tools/app.py:673
+#: lib/fb_tools/app.py:668
 msgid "Show this help message and exit."
 msgstr "Zeigt diesen Hilfe-Bildschirm und beendet sich."
 
-#: lib/fb_tools/app.py:677
+#: lib/fb_tools/app.py:672
 msgid "Display brief usage message and exit."
 msgstr "Zeigt eine kurze Darstellug zur Verwendung und beendet sich."
 
-#: lib/fb_tools/app.py:679
+#: lib/fb_tools/app.py:674
 #, python-format
 msgid "Version of %(prog)s: {}"
 msgstr "Version von %(prog)s: {}"
 
-#: lib/fb_tools/app.py:682
+#: lib/fb_tools/app.py:677
 msgid "Show program's version number and exit."
 msgstr "Stellt die Programm-Version dar und beendet sich."
 
-#: lib/fb_tools/app.py:812
+#: lib/fb_tools/app.py:807
 msgid "Starting in:"
 msgstr "Start in:"
 
-#: lib/fb_tools/app.py:834
+#: lib/fb_tools/app.py:829
 msgid "Aborted by user interrupt."
 msgstr "Abbruch durch Benutzer-Unterbrechung."
 
 #: lib/fb_tools/argparse_actions.py:58
 msgid "Got a {c} for pattern {p!r}: {e}"
 msgstr "Habe ein(e) {c} zum Suchmuster {p!r} erhalten: {e}"
 
@@ -195,111 +195,111 @@
 msgid "The given directory {!r} is not readable."
 msgstr "Das angegebene Verzeichnis {!r} ist nicht lesbar."
 
 #: lib/fb_tools/argparse_actions.py:102
 msgid "The given directory {!r} is not writeable."
 msgstr "In das angegebene Verzeichnis {!r} kann nicht geschrieben werden."
 
-#: lib/fb_tools/argparse_actions.py:130 lib/fb_tools/cfg_app.py:228
+#: lib/fb_tools/argparse_actions.py:130 lib/fb_tools/cfg_app.py:219
 msgid "Directory {!r} does not exists."
 msgstr "Das Verzeichnis {!r} existiert nicht."
 
-#: lib/fb_tools/argparse_actions.py:133 lib/fb_tools/cfg_app.py:232
+#: lib/fb_tools/argparse_actions.py:133 lib/fb_tools/cfg_app.py:223
 msgid "Path {!r} exists, but is not a directory."
 msgstr "Der angegebene Pfad {!r} existiert, ist aber kein Verzeichnis."
 
 #: lib/fb_tools/argparse_actions.py:139 lib/fb_tools/argparse_actions.py:174
-#: lib/fb_tools/cfg_app.py:239 lib/fb_tools/get_file_rm_app.py:399
+#: lib/fb_tools/cfg_app.py:230 lib/fb_tools/get_file_rm_app.py:395
 msgid "File {!r} is not a regular file."
 msgstr "Die Datei {!r} ist keine reguläre Datei."
 
-#: lib/fb_tools/argparse_actions.py:142 lib/fb_tools/cfg_app.py:243
+#: lib/fb_tools/argparse_actions.py:142 lib/fb_tools/cfg_app.py:234
 msgid "File {!r} is not writeable."
 msgstr "Die Datei {!r} ist nicht schreibbar."
 
-#: lib/fb_tools/argparse_actions.py:146 lib/fb_tools/cfg_app.py:248
+#: lib/fb_tools/argparse_actions.py:146 lib/fb_tools/cfg_app.py:239
 msgid "Directory {!r} is not writeable."
 msgstr "In das angegebene Verzeichnis {!r} kann nicht geschrieben werden."
 
-#: lib/fb_tools/argparse_actions.py:171 lib/fb_tools/get_file_rm_app.py:390
+#: lib/fb_tools/argparse_actions.py:171 lib/fb_tools/get_file_rm_app.py:386
 msgid "File {!r} does not exists."
 msgstr "Die Datei {!r} existiert nicht."
 
-#: lib/fb_tools/argparse_actions.py:197 lib/fb_tools/multi_config.py:1155
+#: lib/fb_tools/argparse_actions.py:197 lib/fb_tools/multi_config.py:1147
 msgid "A timeout must be greater than zero and less or equal to {}."
 msgstr "Ein Timeout muss größer als Null und kleiner oder gleich {} sein."
 
 #: lib/fb_tools/argparse_actions.py:202
 msgid "Wrong timeout {!r}:"
 msgstr "Ungültiger Timeout {!r}:"
 
-#: lib/fb_tools/cfg_app.py:64
+#: lib/fb_tools/cfg_app.py:55
 msgid "Parameter {cls!r} must be a subclass of {clinfo!r}."
 msgstr "Der Parameter {cls!r} muss eine von {clinfo!r} abgeleitete Klasse sein."
 
-#: lib/fb_tools/cfg_app.py:146
+#: lib/fb_tools/cfg_app.py:137
 msgid "Config options and options for logging"
 msgstr "Konfigurations- und Logging-Optionen"
 
-#: lib/fb_tools/cfg_app.py:151 lib/fb_tools/cfg_app.py:157 lib/fb_tools/ddns/__init__.py:255
-#: lib/fb_tools/get_file_rm_app.py:270
+#: lib/fb_tools/cfg_app.py:142 lib/fb_tools/cfg_app.py:148 lib/fb_tools/ddns/__init__.py:249
+#: lib/fb_tools/get_file_rm_app.py:266
 msgid "FILE"
 msgstr "DATEI"
 
-#: lib/fb_tools/cfg_app.py:152
+#: lib/fb_tools/cfg_app.py:143
 msgid "Configuration files to use additional to the standard configuration files."
 msgstr "Zusätzlich zu den Standard-Konfigurationsdateien zu benutzende Dateien."
 
-#: lib/fb_tools/cfg_app.py:158
+#: lib/fb_tools/cfg_app.py:149
 msgid "A logfile for storing all logging output."
 msgstr "Eine Logdatei, um alle Log-Ausgaben hineinzuschreiben."
 
-#: lib/fb_tools/cfg_app.py:165
+#: lib/fb_tools/cfg_app.py:156
 msgid "Got command line arguments:"
 msgstr "Erhaltene Kommandozeilen-Argumente:"
 
-#: lib/fb_tools/cfg_app.py:203
+#: lib/fb_tools/cfg_app.py:194
 msgid "Error on reading configuration:"
 msgstr "Fehler beim Lesen der Konfiguration:"
 
-#: lib/fb_tools/cfg_app.py:252
+#: lib/fb_tools/cfg_app.py:243
 msgid "Start logging into file {!r} ..."
 msgstr "Beginne Logging in Datei {!r} …"
 
-#: lib/fb_tools/collections.py:63
+#: lib/fb_tools/collections.py:60
 msgid "Item {item!r} must be of type {must!r}, but is of type {cls!r} instead."
 msgstr "Der Eintrag {item!r} muss vom Typ {must!r} sein, ist aber statt dessen vom Typ {cls!r}."
 
-#: lib/fb_tools/collections.py:81
+#: lib/fb_tools/collections.py:78
 msgid "Object {o!r} is not a {e} object."
 msgstr "Das Objekt {o!r} ist kein {e}-Objekt."
 
-#: lib/fb_tools/collections.py:99
+#: lib/fb_tools/collections.py:96
 msgid "Key {key!r} must be of type {must!r}, but is of type {cls!r} instead."
 msgstr "Der Schlüssel muss vom Typ {must!r} sein, ist aber statt dessen vom Typ {cls!r}."
 
-#: lib/fb_tools/collections.py:116
+#: lib/fb_tools/collections.py:113
 msgid "Object is neither a {m} object, nor a sequential object, but a {o!r} object instead."
 msgstr ""
 "Das Objekt ist weder ein {m}-Objekt noch ein sequentielles Objekt, aber statt dessen vom Typ "
 "{o!r}."
 
-#: lib/fb_tools/collections.py:135
+#: lib/fb_tools/collections.py:132
 msgid "Key {!r} is not existing."
 msgstr "Der Schlüssel {!r} existiert nicht."
 
-#: lib/fb_tools/collections.py:154 lib/fb_tools/collections.py:173
+#: lib/fb_tools/collections.py:151 lib/fb_tools/collections.py:170
 msgid "Could update {ex} with {i!r}: {m}"
 msgstr "Konnte {ex} nicht mit {i!r} updaten: {m}"
 
-#: lib/fb_tools/collections.py:197
+#: lib/fb_tools/collections.py:194
 msgid "Parameter {p!r} is not a sequence type, but a {c!r} object instead."
 msgstr "Der Parameter {p!r} ist kein sequentieller Typ, aber statt dessen vom Typ {c!r}."
 
-#: lib/fb_tools/collections.py:1008
+#: lib/fb_tools/collections.py:1005
 msgid "The method {met}() expected at most {max} arguments, got {got}."
 msgstr "Die Methode {met}() erwartet höchstens {max} Argumente, hat aber {got} erhalten."
 
 #: lib/fb_tools/common.py:154
 msgid "{} is a tty."
 msgstr "{} ist ein tty."
 
@@ -323,339 +323,339 @@
 msgid "Couldn't detect unit {!r}."
 msgstr "Konnte die Maßeinheit in {!r} nicht ermitteln."
 
 #: lib/fb_tools/common.py:783
 msgid "Argument {a!r} must be of type {t1!r} or {t2!r}."
 msgstr "Das Argument {a!r} muss vom Typ {t1!r} oder {t2!r} sein."
 
-#: lib/fb_tools/config.py:101 lib/fb_tools/multi_config.py:245
+#: lib/fb_tools/config.py:96 lib/fb_tools/multi_config.py:237
 msgid "Encoding {v!r} must be a {s!r} object, but is a {c!r} object instead."
 msgstr "Die Kodierung {v!r} muss ein {s!r}-Objekt sein, ist aber statt dessen ein {c!r}-Objekt."
 
-#: lib/fb_tools/config.py:119 lib/fb_tools/multi_config.py:303
+#: lib/fb_tools/config.py:114 lib/fb_tools/multi_config.py:295
 msgid "A configuration directory may not be None."
 msgstr "Ein Konfigurations-Verzeichnis darf nicht None sein."
 
-#: lib/fb_tools/config.py:135
+#: lib/fb_tools/config.py:130
 msgid "A configuration file may not be None."
 msgstr "Eine Konfigurations-Datei darf nicht None sein."
 
-#: lib/fb_tools/config.py:140 lib/fb_tools/config.py:148 lib/fb_tools/multi_config.py:275
+#: lib/fb_tools/config.py:135 lib/fb_tools/config.py:143 lib/fb_tools/multi_config.py:267
 msgid "Configuration file {!r} exists, but is not a regular file."
 msgstr "Die Konfigurations-Datei {!r} existiert, ist aber keine reguläre Datei."
 
-#: lib/fb_tools/config.py:178
+#: lib/fb_tools/config.py:173
 msgid "Searching for {!r} ..."
 msgstr "Suche nach {!r} …"
 
-#: lib/fb_tools/config.py:180
+#: lib/fb_tools/config.py:175
 msgid "Configuration file {!r} not found."
 msgstr "Die Konfigurations-Datei {!r} wurde nicht gefunden."
 
-#: lib/fb_tools/config.py:182
+#: lib/fb_tools/config.py:177
 msgid "Configuration file error"
 msgstr "Konfigurationsdatei-Fehler"
 
-#: lib/fb_tools/config.py:193
+#: lib/fb_tools/config.py:188
 msgid "Reading {!r} ..."
 msgstr "Lese {!r} …"
 
-#: lib/fb_tools/config.py:204
+#: lib/fb_tools/config.py:199
 msgid "Wrong configuration in {!r} found"
 msgstr "Falsche Konfiguration in {!r} gefunden"
 
-#: lib/fb_tools/config.py:206
+#: lib/fb_tools/config.py:201
 msgid "Configuration parse error"
 msgstr "Fehler beim Parsen der Konfiguration"
 
-#: lib/fb_tools/config.py:229 lib/fb_tools/multi_config.py:1124
+#: lib/fb_tools/config.py:224 lib/fb_tools/multi_config.py:1116
 msgid "Checking config section {!r} ..."
 msgstr "Überprüfe Konfigurationsabschnitt {!r} …"
 
-#: lib/fb_tools/ddns/__init__.py:74
+#: lib/fb_tools/ddns/__init__.py:68
 msgid "Got an error {c} on requesting {u!r}: {m}"
 msgstr "Habe einen Fehler {c} beim Abfrage der URL {u!r} erhalten: {m}"
 
-#: lib/fb_tools/ddns/__init__.py:93
+#: lib/fb_tools/ddns/__init__.py:87
 msgid "Directory does not exists"
 msgstr "Das Verzwichnis existiert nicht"
 
-#: lib/fb_tools/ddns/__init__.py:104
+#: lib/fb_tools/ddns/__init__.py:98
 msgid "Path is not a directory"
 msgstr "Der Pfad ist kein Verzeichnis"
 
-#: lib/fb_tools/ddns/__init__.py:115
+#: lib/fb_tools/ddns/__init__.py:109
 msgid "Invalid permissions"
 msgstr "Ungültige Zugriffsrechte"
 
-#: lib/fb_tools/ddns/__init__.py:134
+#: lib/fb_tools/ddns/__init__.py:128
 msgid "This is a base DDNS related application."
 msgstr "Das ist eine DDNS-bezogene Basisanwendung."
 
-#: lib/fb_tools/ddns/__init__.py:170
+#: lib/fb_tools/ddns/__init__.py:164
 msgid "Invalid user agent {!r} given."
 msgstr "Ungültiger User-Agent {!r} übergeben."
 
-#: lib/fb_tools/ddns/__init__.py:196
+#: lib/fb_tools/ddns/__init__.py:190
 msgid "DDNS options"
 msgstr "DDNS-Optionen"
 
-#: lib/fb_tools/ddns/__init__.py:210 lib/fb_tools/ddns/__init__.py:213
+#: lib/fb_tools/ddns/__init__.py:204 lib/fb_tools/ddns/__init__.py:207
 msgid "Perform action only for {}."
 msgstr "Führe die Aktion nur für {} aus."
 
-#: lib/fb_tools/ddns/__init__.py:216
+#: lib/fb_tools/ddns/__init__.py:210
 msgid "The IP protocol, for which the action should be performed (one of {c}, default {d!r})."
 msgstr "Das IP-Protokoll, für das die Aktion ausgeführt werden soll (eins ais {c}, Vorgabe {d!r})."
 
-#: lib/fb_tools/ddns/__init__.py:230
+#: lib/fb_tools/ddns/__init__.py:224
 msgid "PROTOCOL"
 msgstr "PROTOKOLL"
 
-#: lib/fb_tools/ddns/__init__.py:240
+#: lib/fb_tools/ddns/__init__.py:234
 msgid "DIRECTORY"
 msgstr "VERZEICHNIS"
 
-#: lib/fb_tools/ddns/__init__.py:242
+#: lib/fb_tools/ddns/__init__.py:236
 msgid ""
 "The directory, where to read and write the cache files of the evaluated IP addresses (default: "
 "{!r})."
 msgstr ""
 "Das Verzeichnis, von wo Cache-Dateien mit den ermittelten IP-Adresses und wohin sie auch "
 "geschrieben werden (Vorgane: {!r})."
 
-#: lib/fb_tools/ddns/__init__.py:250
+#: lib/fb_tools/ddns/__init__.py:244
 msgid "The timeout in seconds for Web requests (default: {})."
 msgstr "Die Zeit für die Zeitüberschreitung in Sekunden für Web-Abfragen (Vorgabe: {})."
 
-#: lib/fb_tools/ddns/__init__.py:257
+#: lib/fb_tools/ddns/__init__.py:251
 msgid "Configuration file (default: {!r})"
 msgstr "Konfigurationsdatei (Vorgabe: {!r})"
 
-#: lib/fb_tools/ddns/__init__.py:310 lib/fb_tools/ddns/config.py:210
+#: lib/fb_tools/ddns/__init__.py:304 lib/fb_tools/ddns/config.py:207
 msgid "Invalid value {!r} as timeout:"
 msgstr "Ungültiger Wert {!r} für die Zeit der Zeitüberschreitung:"
 
-#: lib/fb_tools/ddns/__init__.py:320
+#: lib/fb_tools/ddns/__init__.py:314
 msgid "Setting Loglevel of the {m} module to {ll}."
 msgstr "Setze Loglevel des {m}-Moduls auf {ll}."
 
-#: lib/fb_tools/ddns/__init__.py:331
+#: lib/fb_tools/ddns/__init__.py:325
 msgid "Trying to get my public IPv{} address."
 msgstr "Versuche meine öffentliche IPv{}-Adresse zu ermitteln."
 
-#: lib/fb_tools/ddns/__init__.py:343
+#: lib/fb_tools/ddns/__init__.py:337
 msgid "Got a response:"
 msgstr "Erhaltene Antwort:"
 
-#: lib/fb_tools/ddns/__init__.py:354
+#: lib/fb_tools/ddns/__init__.py:348
 msgid "Request method: {!r}"
 msgstr "Request-Methode: {!r}"
 
-#: lib/fb_tools/ddns/__init__.py:374
+#: lib/fb_tools/ddns/__init__.py:368
 msgid "Simulation mode, Request will not be sent."
 msgstr "Simulationsmodus, der Request wird nicht gesendet."
 
-#: lib/fb_tools/ddns/__init__.py:387
+#: lib/fb_tools/ddns/__init__.py:381
 msgid "Got a {c} on requesting {u!r}: {e}."
 msgstr "Habe ein {c} bei der Abfrage von {u!r} erhalten: {e}."
 
-#: lib/fb_tools/ddns/__init__.py:394
+#: lib/fb_tools/ddns/__init__.py:388
 msgid "Failed to parse the response"
 msgstr "Konnte Rückgabe nicht auswerten"
 
-#: lib/fb_tools/ddns/__init__.py:422
+#: lib/fb_tools/ddns/__init__.py:423
 msgid "Checking existence and accessibility of working directory {!r} ..."
 msgstr "Überprüfe Existenz und Verfügbarkeit des Arbeitverzeichnisses {!r} …"
 
-#: lib/fb_tools/ddns/__init__.py:434 lib/fb_tools/ddns/update_app.py:169
+#: lib/fb_tools/ddns/__init__.py:435 lib/fb_tools/ddns/update_app.py:165
 msgid "No read access"
 msgstr "Kein Lesezugriff"
 
-#: lib/fb_tools/ddns/__init__.py:438 lib/fb_tools/ddns/update_app.py:172
+#: lib/fb_tools/ddns/__init__.py:439 lib/fb_tools/ddns/update_app.py:168
 msgid "No write access"
 msgstr "Kein Schreinzugriff"
 
-#: lib/fb_tools/ddns/__init__.py:453
+#: lib/fb_tools/ddns/__init__.py:454
 msgid "Writing IP address {a!r} into {f!r} ..."
 msgstr "Schreibe IP-Adresse {a!r} nach {f!r} …"
 
-#: lib/fb_tools/ddns/__init__.py:481
+#: lib/fb_tools/ddns/__init__.py:482
 msgid "File {!r} not found."
 msgstr "Datei {!r} nicht gefunden."
 
-#: lib/fb_tools/ddns/__init__.py:484
+#: lib/fb_tools/ddns/__init__.py:485
 msgid "Reading IP address from {!r}..."
 msgstr "Lese IP-Adresse aus {!r} …"
 
-#: lib/fb_tools/ddns/__init__.py:504
+#: lib/fb_tools/ddns/__init__.py:505
 msgid "Line {li!r} in {f!r} is not a valid IP address:"
 msgstr "Zeile {li!r} in {f!r} ist keine gültige IP-Adresse:"
 
-#: lib/fb_tools/ddns/config.py:104
+#: lib/fb_tools/ddns/config.py:101
 msgid "Invalid timeout {!r} for Web requests, must be 0 < SECONDS < 3600."
 msgstr ""
 "Ungültige Zeit {!r} für eine Zeitüberschreitung für aine Webabfrage, sie muss zwischen 0 und "
 "3600 Sekunden liegen."
 
-#: lib/fb_tools/ddns/config.py:224
+#: lib/fb_tools/ddns/config.py:221
 msgid "Invalid value {ur} for protocols to update, valid protocols are: "
 msgstr "Ungültiger Wert {ur} für ein zu aktualisierendes Protokoll, gültige Protokolle sind:"
 
-#: lib/fb_tools/ddns/config.py:233 lib/fb_tools/ddns/config.py:270
+#: lib/fb_tools/ddns/config.py:230 lib/fb_tools/ddns/config.py:267
 msgid "Unknown configuration option {o!r} with value {v!r} in section {s!r}."
 msgstr "Unbekannte Konfigurationsoption {o!r} mit dem Wert {v!r} in Abschnitt {s!r}."
 
-#: lib/fb_tools/ddns/config.py:255
+#: lib/fb_tools/ddns/config.py:252
 msgid "The path to the working directory must be an absolute path (given: {!r})."
 msgstr "Der Pfad zum Arbeitsverzeichnis muss ein absoluter Pfad sein (gegeben: {!r})."
 
-#: lib/fb_tools/ddns/config.py:265
+#: lib/fb_tools/ddns/config.py:262
 msgid "The path to the logfile must be an absolute path (given: {!r})."
 msgstr "Der Pfad zur Logdatei muss absolut sein (gegeben: {!r})."
 
-#: lib/fb_tools/ddns/myip_app.py:50
+#: lib/fb_tools/ddns/myip_app.py:46
 msgid ""
 "Tries to detect the public NAT IPv4 address and/or the automatic assigned IPv6 address in a "
 "local network and print it out."
 msgstr ""
 "Versucht die öffentliche NAT-IPv4-Adresse bzw. die automatisch zugewiesene IPv6-Adresse in einem"
 " lokalem Netzwerk zu ermitten und zu zeigen."
 
-#: lib/fb_tools/ddns/myip_app.py:55 lib/fb_tools/ddns/myip_app.py:56
+#: lib/fb_tools/ddns/myip_app.py:51 lib/fb_tools/ddns/myip_app.py:52
 msgid "Use only {} to retreive the public IP address."
 msgstr "Verwende nur {}, um die öffentliche IP-Adresse zu ermiteln."
 
-#: lib/fb_tools/ddns/myip_app.py:57
+#: lib/fb_tools/ddns/myip_app.py:53
 msgid "The IP protocol, for which the public IP should be retrieved (one of {c}, default {d!r})."
 msgstr ""
 "Das IP-Protokoll, für welches die öffentliche IP-Adresse ermittelt werden soll (eins aus {c}, "
 "Vorgabe: {d!r})."
 
-#: lib/fb_tools/ddns/myip_app.py:99
+#: lib/fb_tools/ddns/myip_app.py:95
 msgid "myip options"
 msgstr "Optionen für myip"
 
-#: lib/fb_tools/ddns/myip_app.py:103
+#: lib/fb_tools/ddns/myip_app.py:99
 msgid "Write found public IPs into a cache file in working directory."
 msgstr "Schreibe die gefundenen öffentliche IP-Adressen in eine Cache-Datei im Arbeitsverzeichnis zurück."
 
-#: lib/fb_tools/ddns/myip_app.py:134 lib/fb_tools/ddns/update_app.py:275
+#: lib/fb_tools/ddns/myip_app.py:130 lib/fb_tools/ddns/update_app.py:271
 msgid "Starting {a!r}, version {v!r} ..."
 msgstr "Starte {a!r}, Version {v!r} …"
 
-#: lib/fb_tools/ddns/update_app.py:66
+#: lib/fb_tools/ddns/update_app.py:62
 msgid "Updating the DDNS records, even if seems not to be changed."
 msgstr "Aktualisieren der DDNS-Einträge, auch wenn sie nicht verändert zu sein scheinen."
 
-#: lib/fb_tools/ddns/update_app.py:69
+#: lib/fb_tools/ddns/update_app.py:65
 msgid "Tries to update the A and/or AAAA record at ddns.de with the current IP address."
 msgstr "Versucht den A- bzw. AAAA-Eintrag bei ddns.de mit der aktuellen IP-Adresse zu aktualisieren."
 
-#: lib/fb_tools/ddns/update_app.py:74 lib/fb_tools/ddns/update_app.py:75
+#: lib/fb_tools/ddns/update_app.py:70 lib/fb_tools/ddns/update_app.py:71
 msgid "Update only the {} record with the public IP address."
 msgstr "Aktualisiere nur den {}-Eintrag mit der aktuellen IP-Adresse."
 
-#: lib/fb_tools/ddns/update_app.py:76
+#: lib/fb_tools/ddns/update_app.py:72
 msgid ""
 "The IP protocol, for which the appropriate DNS record should be updated with the public IP (one "
 "of {c}, default {d!r})."
 msgstr ""
 "Das IP-Protokoll, für welches der entsprechende DNS-Eintrag der üffentlichen IP aktualisiert "
 "werden soll (eins aus {c}, Vorgabe {d!r})."
 
-#: lib/fb_tools/ddns/update_app.py:158
+#: lib/fb_tools/ddns/update_app.py:154
 msgid "Checking existence and accessibility of log directory {!r} ..."
 msgstr "Überprüfe Existenz und Verfügbarkeit des Log-Verzeichnisses {!r} …"
 
-#: lib/fb_tools/ddns/update_app.py:190
+#: lib/fb_tools/ddns/update_app.py:186
 msgid "Update DDNS options"
 msgstr "DDNS-Aktualisierungsoptionen"
 
-#: lib/fb_tools/ddns/update_app.py:193
+#: lib/fb_tools/ddns/update_app.py:189
 msgid "USER"
 msgstr "BENUTZER"
 
-#: lib/fb_tools/ddns/update_app.py:194
+#: lib/fb_tools/ddns/update_app.py:190
 msgid "The username to login at ddns.de."
 msgstr "Der Nutzername, um sich bei ddns.de eizuloggen."
 
-#: lib/fb_tools/ddns/update_app.py:198
+#: lib/fb_tools/ddns/update_app.py:194
 msgid "PASSWORD"
 msgstr "PASSWORT"
 
-#: lib/fb_tools/ddns/update_app.py:199
+#: lib/fb_tools/ddns/update_app.py:195
 msgid "The password of the user to login at ddns.de."
 msgstr "Das Login-Passwort des Nutzers bei ddns.de."
 
-#: lib/fb_tools/ddns/update_app.py:203
+#: lib/fb_tools/ddns/update_app.py:199
 msgid "FILENAME"
 msgstr "DATEINAME"
 
-#: lib/fb_tools/ddns/update_app.py:204
+#: lib/fb_tools/ddns/update_app.py:200
 msgid "The filename to use as a logfile. Leave it empty to disable file logging."
 msgstr "Der Dateiname der Logdatei. Leer lassen, um Dateilogging zu deaktivieren."
 
-#: lib/fb_tools/ddns/update_app.py:211
+#: lib/fb_tools/ddns/update_app.py:207
 msgid "Update all domains, which are connected whith the given ddns account."
 msgstr "Aktualisirung alle Domänen, die mit dem gegebenen DDNS-Konto verbunden sind."
 
-#: lib/fb_tools/ddns/update_app.py:215
+#: lib/fb_tools/ddns/update_app.py:211
 msgid "DOMAIN"
 msgstr "DOMÄNE"
 
-#: lib/fb_tools/ddns/update_app.py:216
+#: lib/fb_tools/ddns/update_app.py:212
 msgid "The particular domain(s), which should be updated (if not all)."
 msgstr ""
 "Die bestimmte Domäne(n)m die aktualisiert werden solln (wenn nicht alle aktualisiert werden "
 "sollen)."
 
-#: lib/fb_tools/ddns/update_app.py:234
+#: lib/fb_tools/ddns/update_app.py:230
 msgid "No domains to update given, but the option all domains is deactivated."
 msgstr "Keine Domänen zur Aktualisierungg angegeben, aber die Option 'für alle Domänen' ist deaktiviert."
 
-#: lib/fb_tools/ddns/update_app.py:284
+#: lib/fb_tools/ddns/update_app.py:280
 msgid "Ending {a!r}."
 msgstr "Beende {a!r}."
 
-#: lib/fb_tools/ddns/update_app.py:292 lib/fb_tools/ddns/update_app.py:330
+#: lib/fb_tools/ddns/update_app.py:288 lib/fb_tools/ddns/update_app.py:326
 msgid "Last {w} address: {a!r}."
 msgstr "Letzte {w}-Adresse: {a!r}."
 
-#: lib/fb_tools/ddns/update_app.py:294 lib/fb_tools/ddns/update_app.py:332
+#: lib/fb_tools/ddns/update_app.py:290 lib/fb_tools/ddns/update_app.py:328
 msgid "Did not found a last {} address."
 msgstr "Fand keine letzte {}-Adresse."
 
-#: lib/fb_tools/ddns/update_app.py:297
+#: lib/fb_tools/ddns/update_app.py:293
 msgid "Got no public IPv4 address."
 msgstr "Keine öffentliche IPv4-Adresse gefunden."
 
-#: lib/fb_tools/ddns/update_app.py:302 lib/fb_tools/ddns/update_app.py:340
+#: lib/fb_tools/ddns/update_app.py:298 lib/fb_tools/ddns/update_app.py:336
 msgid "Address {a!r} seems not to be a valid {w} address: {e}"
 msgstr "Die Adresse {a!r} scheint keine gültige {w}-Adresse zu sein: {e}"
 
-#: lib/fb_tools/ddns/update_app.py:307 lib/fb_tools/ddns/update_app.py:345
+#: lib/fb_tools/ddns/update_app.py:303 lib/fb_tools/ddns/update_app.py:341
 msgid "Address {a!r} seems not to be a valid {w} address."
 msgstr "Die Adresse {a!r} scheint keine gültige {w}-Adresse zu sein."
 
-#: lib/fb_tools/ddns/update_app.py:312 lib/fb_tools/ddns/update_app.py:350
+#: lib/fb_tools/ddns/update_app.py:308 lib/fb_tools/ddns/update_app.py:346
 msgid "Current {w} address is {a!r}."
 msgstr "Aktuelle {w}-Adresse ist {a!r}."
 
-#: lib/fb_tools/ddns/update_app.py:315 lib/fb_tools/ddns/update_app.py:353
+#: lib/fb_tools/ddns/update_app.py:311 lib/fb_tools/ddns/update_app.py:349
 msgid "The public {w} address {a!r} seems not to be changed since the last update."
 msgstr ""
 "Die öffentliche {w}-Adresse {a!r} scheint sich seit der letzten Aktualisierung nicht geändert zu"
 " haben."
 
-#: lib/fb_tools/ddns/update_app.py:335
+#: lib/fb_tools/ddns/update_app.py:331
 msgid "Got no public IPv6 address."
 msgstr "Keine öffentliche IPv6-Adresse gefunden."
 
-#: lib/fb_tools/ddns/update_app.py:366
+#: lib/fb_tools/ddns/update_app.py:362
 msgid "Updating DNS records to IPv{p} address {a!r} ..."
 msgstr "Aktualisier DNS-Einträge zu IPv{p}-Adresse {a!r} …"
 
 #: lib/fb_tools/errors.py:51
 msgid "Empty mail address."
 msgstr "Leere Mailadresse."
 
@@ -705,988 +705,988 @@
 msgstr[0] "Konnte das Betriebssystem-Kommando nicht finden:"
 msgstr[1] "Konnte die Betriebssystem-Kommandos nicht finden:"
 
 #: lib/fb_tools/errors.py:362
 msgid "Couldn't occupy lockfile {lf!r} in {d:0.1f} seconds with {tries} tries."
 msgstr "Konnte die Lock-Datei {lf!r} nicht in {d:0.1f} Sekunden mit {tries} Versuchen vereinnahmen."
 
-#: lib/fb_tools/get_file_rm_app.py:66
+#: lib/fb_tools/get_file_rm_app.py:62
 msgid "Value must be at least {m} - {v} was given."
 msgstr "Der Wert muss mindestens {m} sein - {v} wurde gegeben."
 
-#: lib/fb_tools/get_file_rm_app.py:108
+#: lib/fb_tools/get_file_rm_app.py:104
 msgid "The given pattern {!r} is not a valid date pattern"
 msgstr "Das übergebene Muster {!r} is kein gültiges Datums-Muster"
 
-#: lib/fb_tools/get_file_rm_app.py:112
+#: lib/fb_tools/get_file_rm_app.py:108
 #, python-format
 msgid ". The must be exactly one occurence of '%Y', one of '%m' and one of '%d'."
 msgstr ". Es muss exakt einmal '%Y', einmal '%m' und einmal '%d' angegeben werden."
 
-#: lib/fb_tools/get_file_rm_app.py:143
+#: lib/fb_tools/get_file_rm_app.py:139
 msgid ""
 "Returns a newline separated list of files generated from file globbing patterns given as "
 "arguments to this application, where all files are omitted, which should not be removed."
 msgstr ""
 "Gibt eine mit Zeilenumbruch separierte Liste von Dateien zurück, die aus dem Datei-Muster, "
 "welches als Kommando-Zeilen-Argument dieser Anwendung übergeben wurde, generiert wurde, wobei "
 "alle Datein fehlen, welche nicht gelöscht werden sollen."
 
-#: lib/fb_tools/get_file_rm_app.py:182 lib/fb_tools/get_file_rm_app.py:198
-#: lib/fb_tools/get_file_rm_app.py:214 lib/fb_tools/get_file_rm_app.py:230
-#: lib/fb_tools/get_file_rm_app.py:246
+#: lib/fb_tools/get_file_rm_app.py:178 lib/fb_tools/get_file_rm_app.py:194
+#: lib/fb_tools/get_file_rm_app.py:210 lib/fb_tools/get_file_rm_app.py:226
+#: lib/fb_tools/get_file_rm_app.py:242
 msgid "Wrong value {v!r} for {n}, must be >= {m}"
 msgstr "Ungültiger Wert {v!r} für {n}, muss größer als oder gleich {m} sein"
 
-#: lib/fb_tools/get_file_rm_app.py:267
+#: lib/fb_tools/get_file_rm_app.py:263
 msgid "File options"
 msgstr "Datei-Optionen"
 
-#: lib/fb_tools/get_file_rm_app.py:271
+#: lib/fb_tools/get_file_rm_app.py:267
 msgid "File pattern to generate list of files to remove."
 msgstr "Dateimuster, um die Liste der zu löschenden Dateien zu generieren."
 
-#: lib/fb_tools/get_file_rm_app.py:274
+#: lib/fb_tools/get_file_rm_app.py:270
 msgid "Keep options"
 msgstr "Optionen zum Aufbewahren"
 
-#: lib/fb_tools/get_file_rm_app.py:277
+#: lib/fb_tools/get_file_rm_app.py:273
 msgid "NR_FILES"
 msgstr "ANZAHL_DATEIEN"
 
-#: lib/fb_tools/get_file_rm_app.py:279
+#: lib/fb_tools/get_file_rm_app.py:275
 msgid "How many of the last files should be kept (default: {default}, minimum: {min})?"
 msgstr "Wieviele der letzten Dateien sollen aufbewahrt werden (Vorgabe: {default}, Minimum {min})?"
 
-#: lib/fb_tools/get_file_rm_app.py:286
+#: lib/fb_tools/get_file_rm_app.py:282
 msgid "DAYS"
 msgstr "TAGE"
 
-#: lib/fb_tools/get_file_rm_app.py:288
+#: lib/fb_tools/get_file_rm_app.py:284
 msgid "How many files one per day from today on should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 "Wieviele Dateien (eine pro Tag) sollen von heute an rückwärts aufbewahrt werden (Vorgabe:  "
 "{default}, Minimum {min})?"
 
-#: lib/fb_tools/get_file_rm_app.py:295
+#: lib/fb_tools/get_file_rm_app.py:291
 msgid "WEEKS"
 msgstr "WOCHEN"
 
-#: lib/fb_tools/get_file_rm_app.py:297
+#: lib/fb_tools/get_file_rm_app.py:293
 msgid "How many files one per week from today on should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 "Wieviele Dateien (eine pro Woche) sollen von heute an rückwärts aufbewahrt werden (Vorgabe:  "
 "{default}, Minimum {min})?"
 
-#: lib/fb_tools/get_file_rm_app.py:304
+#: lib/fb_tools/get_file_rm_app.py:300
 msgid "MONTHS"
 msgstr "MONATE"
 
-#: lib/fb_tools/get_file_rm_app.py:306
+#: lib/fb_tools/get_file_rm_app.py:302
 msgid "How many files one per month from today on should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 "Wieviele Dateien (eine pro Monat) sollen von heute an rückwärts aufbewahrt werden (Vorgabe:  "
 "{default}, Minimum {min})?"
 
-#: lib/fb_tools/get_file_rm_app.py:313
+#: lib/fb_tools/get_file_rm_app.py:309
 msgid "YEARS"
 msgstr "JAHRE"
 
-#: lib/fb_tools/get_file_rm_app.py:315
+#: lib/fb_tools/get_file_rm_app.py:311
 msgid "How many files one per year from today on should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 "Wieviele Dateien (eine pro Jahr) sollen von heute an rückwärts aufbewahrt werden (Vorgabe:  "
 "{default}, Minimum {min})?"
 
-#: lib/fb_tools/get_file_rm_app.py:346
+#: lib/fb_tools/get_file_rm_app.py:342
 msgid "Resolving date pattern {!r}."
 msgstr "Löse Datumsmuster {!r} auf."
 
-#: lib/fb_tools/get_file_rm_app.py:367
+#: lib/fb_tools/get_file_rm_app.py:363
 msgid "Checking given files..."
 msgstr "Überprüfe übergebene Dateien …"
 
-#: lib/fb_tools/get_file_rm_app.py:372
+#: lib/fb_tools/get_file_rm_app.py:368
 msgid "Checking given file {!r} ..."
 msgstr "Überprüfe übergebene Datei {!r} …"
 
-#: lib/fb_tools/get_file_rm_app.py:381
+#: lib/fb_tools/get_file_rm_app.py:377
 msgid "Resolved paths:"
 msgstr "Aufgelöste Pfade:"
 
-#: lib/fb_tools/get_file_rm_app.py:383
+#: lib/fb_tools/get_file_rm_app.py:379
 msgid "File pattern {!r} does not match any files."
 msgstr "Das Dateimuster {!r} passt auf keine Dateien."
 
-#: lib/fb_tools/get_file_rm_app.py:388
+#: lib/fb_tools/get_file_rm_app.py:384
 msgid "Checking {!r} ..."
 msgstr "Überprüfe {!r} …"
 
-#: lib/fb_tools/get_file_rm_app.py:394
+#: lib/fb_tools/get_file_rm_app.py:390
 msgid "File {!r} is a regular file."
 msgstr "Die Datei {!r} ist eine reguläre Datei."
 
-#: lib/fb_tools/get_file_rm_app.py:397
+#: lib/fb_tools/get_file_rm_app.py:393
 msgid "Path {!r} is a directory."
 msgstr "Der Pfad {!r} ist ein Verzeichnis."
 
-#: lib/fb_tools/get_file_rm_app.py:404
+#: lib/fb_tools/get_file_rm_app.py:400
 msgid "File {fi!r} does not match pattern {pa!r}."
 msgstr "Die Datei {fi!r} passt nicht in das Dateimuster {pa!r}."
 
-#: lib/fb_tools/get_file_rm_app.py:414
+#: lib/fb_tools/get_file_rm_app.py:410
 msgid "Date in file {fi!r} is not a valid date: {e}."
 msgstr "Das Datum in der Datei {fi!r} ist kein gültiges Datum: {e}."
 
-#: lib/fb_tools/get_file_rm_app.py:465
+#: lib/fb_tools/get_file_rm_app.py:461
 msgid "Did not found any files to evaluate."
 msgstr "Fand keine Dateien zur Auswertung"
 
-#: lib/fb_tools/get_file_rm_app.py:497
+#: lib/fb_tools/get_file_rm_app.py:493
 msgid "Keeping last file ..."
 msgid_plural "Keeping last {} files ..."
 msgstr[0] "Behalte die letzte Datei …"
 msgstr[1] "Behalte die letzten {} Dateien …"
 
-#: lib/fb_tools/get_file_rm_app.py:503
+#: lib/fb_tools/get_file_rm_app.py:499
 msgid "Keep last file {!r}."
 msgstr "Behalte die letzte Datei {!r}."
 
-#: lib/fb_tools/get_file_rm_app.py:508
+#: lib/fb_tools/get_file_rm_app.py:504
 msgid "Files to keep:"
 msgstr "Zu behaltende Dateien:"
 
-#: lib/fb_tools/get_file_rm_app.py:529
+#: lib/fb_tools/get_file_rm_app.py:525
 msgid "Files to keep for year:"
 msgstr "Dateien, die für Jahr zu behalten sind:"
 
-#: lib/fb_tools/get_file_rm_app.py:551
+#: lib/fb_tools/get_file_rm_app.py:547
 msgid "Got last month: {!r}"
 msgstr "Ermittelter letzter Monat: {!r}"
 
-#: lib/fb_tools/get_file_rm_app.py:565
+#: lib/fb_tools/get_file_rm_app.py:561
 msgid "Files to keep for month:"
 msgstr "Dateien, die für Monat zu behalten sind:"
 
-#: lib/fb_tools/get_file_rm_app.py:579
+#: lib/fb_tools/get_file_rm_app.py:575
 msgid "Got last Monday: {!r}"
 msgstr "Ermittelter letzter Montag: {!r}"
 
-#: lib/fb_tools/get_file_rm_app.py:592
+#: lib/fb_tools/get_file_rm_app.py:588
 msgid "Files to keep for week:"
 msgstr "Dateien, die für Woche zu behalten sind:"
 
-#: lib/fb_tools/get_file_rm_app.py:605
+#: lib/fb_tools/get_file_rm_app.py:601
 msgid "Got last day: {!r}"
 msgstr "Ermittelter letzter Tag: {!r}"
 
-#: lib/fb_tools/get_file_rm_app.py:616
+#: lib/fb_tools/get_file_rm_app.py:612
 msgid "Keeping all files from today."
 msgstr "Aufheben aller Dateien von heute."
 
-#: lib/fb_tools/get_file_rm_app.py:623
+#: lib/fb_tools/get_file_rm_app.py:619
 msgid "Files to keep for day:"
 msgstr "Dateien, die für Tag zu behalten sind:"
 
-#: lib/fb_tools/get_file_rm_app.py:640
+#: lib/fb_tools/get_file_rm_app.py:636
 msgid "Trying to get date of file {!r}."
 msgstr "Versuche das Datum aus der Datei {!r} zu entnehmen."
 
-#: lib/fb_tools/get_file_rm_app.py:679
+#: lib/fb_tools/get_file_rm_app.py:675
 msgid "Explored and assigned files:"
 msgstr "Ermittelte und zugewiesene Dateien:"
 
-#: lib/fb_tools/handler/__init__.py:159
+#: lib/fb_tools/handler/__init__.py:155
 msgid "Invalid time zone name {!r}."
 msgstr "Ungültiger Zeitzonenname {!r}."
 
-#: lib/fb_tools/handler/__init__.py:161
+#: lib/fb_tools/handler/__init__.py:157
 msgid "Setting time zone to {!r}."
 msgstr "Setze Zeitzone auf {!r}."
 
-#: lib/fb_tools/handler/__init__.py:165
+#: lib/fb_tools/handler/__init__.py:161
 msgid "Name of the time zone: {!r}."
 msgstr "Name der Zeitzone: {!r}."
 
-#: lib/fb_tools/handler/__init__.py:171
+#: lib/fb_tools/handler/__init__.py:167
 msgid "{}-object not initialized."
 msgstr "Das {}-Objekt ist noch nicht initialisiert."
 
-#: lib/fb_tools/handler/__init__.py:173
+#: lib/fb_tools/handler/__init__.py:169
 msgid "Method {} must be overridden in descendant classes."
 msgstr "Die Methode {} muss in abgeleiteten Klassen überschrieben werden."
 
-#: lib/fb_tools/handler/__init__.py:250
+#: lib/fb_tools/handler/__init__.py:246
 msgid "Quiet execution."
 msgstr "Stillschweigende Ausführung."
 
-#: lib/fb_tools/handler/__init__.py:298
+#: lib/fb_tools/handler/__init__.py:294
 msgid "Starting synchronous communication with '{}'."
 msgstr "Starte synchrone Kommunikation mit '{}'."
 
-#: lib/fb_tools/handler/__init__.py:302
+#: lib/fb_tools/handler/__init__.py:298
 msgid "Finished communication with '{}'."
 msgstr "Kommunikation mit '{}' beendet."
 
-#: lib/fb_tools/handler/__init__.py:316
+#: lib/fb_tools/handler/__init__.py:312
 msgid "Parameter {p!r} is not of type {t!r}."
 msgstr "Der Parameter {p!r} ist nicht vom Typ {t!r}."
 
-#: lib/fb_tools/handler/__init__.py:321
+#: lib/fb_tools/handler/__init__.py:317
 msgid "Got completed process:"
 msgstr "Vollendeten Prozess erhalten:"
 
-#: lib/fb_tools/handler/__init__.py:325 lib/fb_tools/handler/__init__.py:336
+#: lib/fb_tools/handler/__init__.py:321 lib/fb_tools/handler/__init__.py:332
 msgid "Output on {}:"
 msgstr "Ausgabe an {}:"
 
-#: lib/fb_tools/handler/__init__.py:357
+#: lib/fb_tools/handler/__init__.py:353
 msgid "Starting asynchronous communication with '{cmd}', heartbeat interval is {interval:0.1f} seconds."
 msgstr "Starte asynchrone Kommunikation mit '{cmd}', Herzschlag-Intervall ist {interval:0.1f} Sekunden."
 
-#: lib/fb_tools/handler/__init__.py:372
+#: lib/fb_tools/handler/__init__.py:368
 msgid "Checking for the end of the communication ..."
 msgstr "Überprüfe das Ende der Kummunikation …"
 
-#: lib/fb_tools/handler/__init__.py:382
+#: lib/fb_tools/handler/__init__.py:378
 msgid "Time to execute the heartbeat handler."
 msgstr "Es ist an der Zeit, den Herzschlag-Handler auszuführen."
 
-#: lib/fb_tools/handler/__init__.py:386
+#: lib/fb_tools/handler/__init__.py:382
 msgid "Sleeping {:0.2f} seconds ..."
 msgstr "Schlafe für {:0.2f} Sekunden …"
 
-#: lib/fb_tools/handler/__init__.py:394 lib/fb_tools/handler/__init__.py:403
+#: lib/fb_tools/handler/__init__.py:390 lib/fb_tools/handler/__init__.py:399
 msgid "   {w} is now: {o!r}"
 msgstr "   {w} ist jetzt: {o!r}"
 
-#: lib/fb_tools/handler/lock.py:101
+#: lib/fb_tools/handler/lock.py:99
 msgid "Locking directory {!r} doesn't exists or is not a directory."
 msgstr "Das Lockverzeichnis {!r} existiert entweder nicht oder ist kein Verzeichnis."
 
-#: lib/fb_tools/handler/lock.py:128 lib/fb_tools/handler/lock.py:807
+#: lib/fb_tools/handler/lock.py:126 lib/fb_tools/handler/lock.py:805
 msgid "Locking directory {!r} isn't writeable."
 msgstr "Kein Schreibzugriff auf das Lockverzeichnis {!r}."
 
-#: lib/fb_tools/handler/lock.py:193
+#: lib/fb_tools/handler/lock.py:191
 msgid "No lockfile given on init of a LockObject object."
 msgstr "Keine Lockdatei bei der Initialisierung des LockObject-Ojektes angegeben."
 
-#: lib/fb_tools/handler/lock.py:199
+#: lib/fb_tools/handler/lock.py:197
 msgid "Lockfile {!r} doesn't exists, but don't worry, it's simulation mode."
 msgstr "Die Lockdatei {!r} existiert nicht, aber keine Sorge, wir sind im Simulationsmodus."
 
-#: lib/fb_tools/handler/lock.py:203 lib/fb_tools/handler/lock.py:1045
+#: lib/fb_tools/handler/lock.py:201 lib/fb_tools/handler/lock.py:1043
 msgid "Lockfile {!r} doesn't exists."
 msgstr "Die Lockdatei {!r} existiert nicht."
 
-#: lib/fb_tools/handler/lock.py:206
+#: lib/fb_tools/handler/lock.py:204
 msgid "Lockfile {!r} is not a regular file."
 msgstr "Die Lockdatei {!r} ist keine reguläre Datei."
 
-#: lib/fb_tools/handler/lock.py:360
+#: lib/fb_tools/handler/lock.py:358
 msgid "Closing file descriptor {} ..."
 msgstr "Schließe Datei-Deskriptor {} …"
 
-#: lib/fb_tools/handler/lock.py:371
+#: lib/fb_tools/handler/lock.py:369
 msgid "Automatic removing of {!r} ..."
 msgstr "Automatisches Löschen von {!r} …"
 
-#: lib/fb_tools/handler/lock.py:399
+#: lib/fb_tools/handler/lock.py:397
 msgid "Refreshing atime and mtime of {!r} to the current timestamp."
 msgstr "Setze atime und mtime von {!r} auf den aktuellen Zeitstempel."
 
-#: lib/fb_tools/handler/lock.py:533 lib/fb_tools/handler/lock.py:553 lib/fb_tools/handler/lock.py:573
-#: lib/fb_tools/handler/lock.py:597 lib/fb_tools/handler/lock.py:692 lib/fb_tools/handler/lock.py:1034
+#: lib/fb_tools/handler/lock.py:531 lib/fb_tools/handler/lock.py:551 lib/fb_tools/handler/lock.py:571
+#: lib/fb_tools/handler/lock.py:595 lib/fb_tools/handler/lock.py:690 lib/fb_tools/handler/lock.py:1032
 msgid "Value {val!r} for {what} is not a Number."
 msgstr "Der Wert {val!r} für {what} ist keine Zahl."
 
-#: lib/fb_tools/handler/lock.py:538 lib/fb_tools/handler/lock.py:558 lib/fb_tools/handler/lock.py:578
-#: lib/fb_tools/handler/lock.py:602 lib/fb_tools/handler/lock.py:697 lib/fb_tools/handler/lock.py:1038
+#: lib/fb_tools/handler/lock.py:536 lib/fb_tools/handler/lock.py:556 lib/fb_tools/handler/lock.py:576
+#: lib/fb_tools/handler/lock.py:600 lib/fb_tools/handler/lock.py:695 lib/fb_tools/handler/lock.py:1036
 msgid "The value for {what} must be greater than zero (is {val!r})."
 msgstr "Der Wert für {what} muss größer als Null sein (ist {val!r})."
 
-#: lib/fb_tools/handler/lock.py:702
+#: lib/fb_tools/handler/lock.py:700
 msgid "The value for {what} must be greater than or equal to zero (is {val!r})."
 msgstr "Der Wert für {what} muss größer als oder gleich Null sein (ist {val!r})."
 
-#: lib/fb_tools/handler/lock.py:787
+#: lib/fb_tools/handler/lock.py:785
 msgid "Invalid PID {} given on calling create_lockfile()."
 msgstr "Ungültige PID {} beim Aufruf von create_lockfile() übergeben."
 
-#: lib/fb_tools/handler/lock.py:796
+#: lib/fb_tools/handler/lock.py:794
 msgid "Using lock directory {!r} ..."
 msgstr "Verwende Lock-Verzeichnis {!r} …"
 
-#: lib/fb_tools/handler/lock.py:804
+#: lib/fb_tools/handler/lock.py:802
 msgid "Trying to lock lockfile {!r} ..."
 msgstr "Versuche Lockdatei {!r} zu okkupieren …"
 
-#: lib/fb_tools/handler/lock.py:845
+#: lib/fb_tools/handler/lock.py:843
 msgid "Current time difference: {:0.3f} seconds."
 msgstr "Aktuelle Zeitdifferenz: {:0.3f} Sekunden."
 
-#: lib/fb_tools/handler/lock.py:850
+#: lib/fb_tools/handler/lock.py:848
 msgid "Try {try_nr} on creating lockfile {lfile!r} ..."
 msgstr "Versuch Nummer {try_nr} zum Erstellen der Lockdatei {lfile!r} …"
 
-#: lib/fb_tools/handler/lock.py:861 lib/fb_tools/handler/lock.py:980
+#: lib/fb_tools/handler/lock.py:859 lib/fb_tools/handler/lock.py:978
 msgid "Removing lockfile {!r} ..."
 msgstr "Lösche Lockdatei {!r} …"
 
-#: lib/fb_tools/handler/lock.py:866 lib/fb_tools/handler/lock.py:988
+#: lib/fb_tools/handler/lock.py:864 lib/fb_tools/handler/lock.py:986
 msgid "Error on removing lockfile {lfile!r}: {err}"
 msgstr "Fehler beim Löschen der Lockdatei {lfile!r): {err}"
 
-#: lib/fb_tools/handler/lock.py:879
+#: lib/fb_tools/handler/lock.py:877
 msgid "Sleeping for {:0.1f} seconds."
 msgstr "Schlafe für {:0.1f} Sekunden."
 
-#: lib/fb_tools/handler/lock.py:894
+#: lib/fb_tools/handler/lock.py:892
 msgid "Got a lock for lockfile {!r}."
 msgstr "Habe einen Lock für die Lockdatei {!r} erhalten."
 
-#: lib/fb_tools/handler/lock.py:900
+#: lib/fb_tools/handler/lock.py:898
 msgid "Write {what!r} in lockfile {lfile!r} ..."
 msgstr "Schreibe {what!r} in Lockdatei {lfile!r} …"
 
-#: lib/fb_tools/handler/lock.py:909
+#: lib/fb_tools/handler/lock.py:907
 msgid "Seeking and syncing {!r} ..."
 msgstr "Seeken und synchronisieren von {!r} …"
 
-#: lib/fb_tools/handler/lock.py:938
+#: lib/fb_tools/handler/lock.py:936
 msgid "Trying to open {!r} exclusive ..."
 msgstr "Versuche {!r} exklusiv zu öffnen …"
 
-#: lib/fb_tools/handler/lock.py:940
+#: lib/fb_tools/handler/lock.py:938
 msgid "Simulation mode, no real creation of a lockfile."
 msgstr "Simulationsmodus, Lockdatei wird in Wirklichkeit nicht erstellt."
 
-#: lib/fb_tools/handler/lock.py:948
+#: lib/fb_tools/handler/lock.py:946
 msgid "Error on creating lockfile {lfile!r}: {err}"
 msgstr "Fehler beim Erstellen der Lockdatei {lfile!r}: {err}"
 
-#: lib/fb_tools/handler/lock.py:977
+#: lib/fb_tools/handler/lock.py:975
 msgid "Lockfile {!r} to remove doesn't exists."
 msgstr "Die zu löschende Lockdatei {!r} existiert nicht."
 
-#: lib/fb_tools/handler/lock.py:982
+#: lib/fb_tools/handler/lock.py:980
 msgid "Simulation mode - lockfile won't removed."
 msgstr "Simulationsmodus - die Lockdatei wird nicht gelöscht."
 
-#: lib/fb_tools/handler/lock.py:1042
+#: lib/fb_tools/handler/lock.py:1040
 msgid "Checking lockfile {!r} ..."
 msgstr "Überprüfe Lockdatei {!r} …"
 
-#: lib/fb_tools/handler/lock.py:1049
+#: lib/fb_tools/handler/lock.py:1047
 msgid "No read access for lockfile {!r}."
 msgstr "Kein Lesezugriff auf Lockdatei {!r}."
 
-#: lib/fb_tools/handler/lock.py:1053
+#: lib/fb_tools/handler/lock.py:1051
 msgid "No write access for lockfile {!r}."
 msgstr "Kein Schreibzugriff auf Lockdatei {!r}."
 
-#: lib/fb_tools/handler/lock.py:1059
+#: lib/fb_tools/handler/lock.py:1057
 msgid "Unusable lockfile {!r}."
 msgstr "Nicht verwendungsfähige Lockdatei {!r}."
 
-#: lib/fb_tools/handler/lock.py:1062
+#: lib/fb_tools/handler/lock.py:1060
 msgid "Process with PID {} is unfortunately dead."
 msgstr "Der Prozess mit der PID {} ist unglücklicherweise verstorben."
 
-#: lib/fb_tools/handler/lock.py:1065
+#: lib/fb_tools/handler/lock.py:1063
 msgid "Process with PID {} is still running."
 msgstr "Der Prozess mit der PID {} läuft aktuell noch."
 
-#: lib/fb_tools/handler/lock.py:1073
+#: lib/fb_tools/handler/lock.py:1071
 msgid "Could not stat for file {lfile!r}: {err}"
 msgstr "Konnte Stat-Daten für Datei {lfile!r} nicht ermitteln: {err}"
 
-#: lib/fb_tools/handler/lock.py:1080
+#: lib/fb_tools/handler/lock.py:1078
 msgid "Lockfile {lfile!r} is older than {max} seconds ({age} seconds)."
 msgstr "Die Lockdatei {lfile!r} ist älter als {max} Sekunden ({age} Sekunden)."
 
-#: lib/fb_tools/handler/lock.py:1083
+#: lib/fb_tools/handler/lock.py:1081
 msgid "Lockfile {lfile!r} is {age} seconds old, but not old enough ({max} seconds)."
 msgstr "Die Lockdatei {lfile!r} ist {age} Sekunden alt, aber nicht alte genug ({max} Sekunden)."
 
-#: lib/fb_tools/handler/lock.py:1110
+#: lib/fb_tools/handler/lock.py:1108
 msgid "Trying to open pidfile {!r} ..."
 msgstr "Versuche PID-Datei {!r} zu öffnen …"
 
-#: lib/fb_tools/handler/lock.py:1114
+#: lib/fb_tools/handler/lock.py:1112
 msgid "Could not open pidfile {!r} for reading:"
 msgstr "Konnte PID-Datei {!r} nicht zum Lesen öffnen:"
 
-#: lib/fb_tools/handler/lock.py:1127
+#: lib/fb_tools/handler/lock.py:1125
 msgid "First line of pidfile {!r} was empty."
 msgstr "Die erste Zeile der PID-Datei {!r} war leer."
 
-#: lib/fb_tools/handler/lock.py:1138
+#: lib/fb_tools/handler/lock.py:1136
 msgid "Could not interprete {cont!r} as a PID from {file!r}: {err}"
 msgstr "Konnte {cont!r} nicht als PID (in {file!r}) interpretieren: {err}"
 
-#: lib/fb_tools/handler/lock.py:1147
+#: lib/fb_tools/handler/lock.py:1145
 msgid "Invalid PID {pid} in {file!r} found."
 msgstr "Ungültige PID {pid} in Datei {file!r} gefunden."
 
-#: lib/fb_tools/handling_obj.py:78
+#: lib/fb_tools/handling_obj.py:73
 msgid "Timeout on communicating with process."
 msgstr "Zeitüberschreitung in der Kommunikation mit einem Prozess."
 
-#: lib/fb_tools/handling_obj.py:104
+#: lib/fb_tools/handling_obj.py:99
 msgid "Command {c!r} returned non-zero exit status {rc}."
 msgstr "Das Kommando {c!r} gab den Nicht-Null Wert {rc} zurück."
 
-#: lib/fb_tools/handling_obj.py:142
+#: lib/fb_tools/handling_obj.py:137
 msgid "Command {c!r} timed out after {s} second."
 msgid_plural "Command {c!r} timed out after {s} seconds."
 msgstr[0] "Das Kommando {c!r} timte nach einer Sekunde aus."
 msgstr[1] "Das Kommando {c!r} timte nach {s} Sekunden aus."
 
-#: lib/fb_tools/handling_obj.py:303
+#: lib/fb_tools/handling_obj.py:298
 msgid "Wrong prompt timeout {v!r}, must be greater or equal to Null and less or equal to {max}."
 msgstr ""
 "Falscher Eingabe-Timeout {v!r}, er muss größer oder gleich Null sowie kleiner oder gleich {max} "
 "sein."
 
-#: lib/fb_tools/handling_obj.py:314
+#: lib/fb_tools/handling_obj.py:309
 msgid "yes"
 msgstr "ja"
 
-#: lib/fb_tools/handling_obj.py:321
+#: lib/fb_tools/handling_obj.py:316
 msgid "no"
 msgstr "nein"
 
-#: lib/fb_tools/handling_obj.py:389
+#: lib/fb_tools/handling_obj.py:384
 msgid "Searching for command {!r} ..."
 msgstr "Suche nach Befehl {!r} …"
 
-#: lib/fb_tools/handling_obj.py:394
+#: lib/fb_tools/handling_obj.py:389
 msgid "Command {!r} doesn't exists."
 msgstr "Das Befehl {!r} existiert nicht."
 
-#: lib/fb_tools/handling_obj.py:397 lib/fb_tools/handling_obj.py:421
+#: lib/fb_tools/handling_obj.py:392 lib/fb_tools/handling_obj.py:416
 msgid "Command {!r} is not executable."
 msgstr "Das Befehl {!r} ist nicht ausführbar."
 
-#: lib/fb_tools/handling_obj.py:411
+#: lib/fb_tools/handling_obj.py:406
 msgid "Searching command in {!r} ..."
 msgstr "Suche Befehl in {!r} …"
 
-#: lib/fb_tools/handling_obj.py:424
+#: lib/fb_tools/handling_obj.py:419
 msgid "Command {!r} not found."
 msgstr "Das Kommando {!r} wurde nicht gefunden."
 
-#: lib/fb_tools/handling_obj.py:496
+#: lib/fb_tools/handling_obj.py:491
 msgid "STDIN and input arguments may not both be used."
 msgstr "STDIN und Eingabe-Argumente dürfen nicht zusammen verwendet werden."
 
-#: lib/fb_tools/handling_obj.py:499
+#: lib/fb_tools/handling_obj.py:494
 msgid "Executing command args:"
 msgstr "Auszuführende Befehlsargumente:"
 
-#: lib/fb_tools/handling_obj.py:502
+#: lib/fb_tools/handling_obj.py:497
 msgid "Performing argument {!r}."
 msgstr "Verarbeite Argument {!r}."
 
-#: lib/fb_tools/handler/__init__.py:247 lib/fb_tools/handling_obj.py:507
+#: lib/fb_tools/handler/__init__.py:243 lib/fb_tools/handling_obj.py:502
 msgid "Executing: {}"
 msgstr "Ausführung: {}"
 
-#: lib/fb_tools/handling_obj.py:510
+#: lib/fb_tools/handling_obj.py:505
 msgid "Simulation mode, not executing: {}"
 msgstr "Simulations-Modus, führe nicht aus: {}"
 
-#: lib/fb_tools/handling_obj.py:518
+#: lib/fb_tools/handling_obj.py:513
 msgid "PID of process: {}"
 msgstr "PID des Prozesses: {}"
 
-#: lib/fb_tools/handling_obj.py:524
+#: lib/fb_tools/handling_obj.py:519
 msgid "{c} happened, killing process: {e}"
 msgstr "{} aufgetreten, töte Prozess: {e}"
 
-#: lib/fb_tools/handling_obj.py:626
+#: lib/fb_tools/handling_obj.py:621
 msgid "Nothing to do on signal."
 msgstr "Aud das Signal gibt es nichts zu tun."
 
-#: lib/fb_tools/handling_obj.py:680 lib/fb_tools/handling_obj.py:769
+#: lib/fb_tools/handling_obj.py:675 lib/fb_tools/handling_obj.py:764
 msgid "File doesn't exists."
 msgstr "Die Datei existiert nicht."
 
-#: lib/fb_tools/handling_obj.py:683
+#: lib/fb_tools/handling_obj.py:678
 msgid "Read permission denied."
 msgstr "Lesezugriff verboten."
 
-#: lib/fb_tools/handling_obj.py:686
+#: lib/fb_tools/handling_obj.py:681
 msgid "Reading file content of {!r} ..."
 msgstr "Lese Inhalt der Datei {!r} …"
 
-#: lib/fb_tools/handling_obj.py:774 lib/fb_tools/handling_obj.py:781
+#: lib/fb_tools/handling_obj.py:769 lib/fb_tools/handling_obj.py:776
 msgid "Write permission to {!r} denied."
 msgstr "Schreibzugriff auf {!r} verboten."
 
-#: lib/fb_tools/handling_obj.py:776 lib/fb_tools/handling_obj.py:783
+#: lib/fb_tools/handling_obj.py:771 lib/fb_tools/handling_obj.py:778
 msgid "Write permission denied."
 msgstr "Schreibzugriff verboten."
 
-#: lib/fb_tools/handling_obj.py:787
+#: lib/fb_tools/handling_obj.py:782
 msgid "Write {what!r} into {to!r}."
 msgstr "Schreibe {what!r} nach {to!r}."
 
-#: lib/fb_tools/handling_obj.py:789
+#: lib/fb_tools/handling_obj.py:784
 msgid "Writing {!r} ..."
 msgstr "Schreibe {!r} …"
 
-#: lib/fb_tools/handling_obj.py:801
+#: lib/fb_tools/handling_obj.py:796
 msgid "Simulating write into {!r}."
 msgstr "Simuliere das Schreiben nach {!r}."
 
-#: lib/fb_tools/handling_obj.py:809
+#: lib/fb_tools/handling_obj.py:804
 msgid "Opening {!r} for write unbuffered ..."
 msgstr "Öffne {!r} zum ungepufferten Schreiben …"
 
-#: lib/fb_tools/handler/lock.py:913 lib/fb_tools/handling_obj.py:813
+#: lib/fb_tools/handler/lock.py:911 lib/fb_tools/handling_obj.py:808
 msgid "Closing {!r} ..."
 msgstr "Schließe {!r} …"
 
-#: lib/fb_tools/handling_obj.py:844
+#: lib/fb_tools/handling_obj.py:839
 msgid "Password:"
 msgstr "Passwort:"
 
-#: lib/fb_tools/handling_obj.py:847
+#: lib/fb_tools/handling_obj.py:842
 msgid "Repeat password:"
 msgstr "Passwort Wiederholung:"
 
-#: lib/fb_tools/handling_obj.py:861
+#: lib/fb_tools/handling_obj.py:856
 msgid "The entered passwords does not match."
 msgstr "Die eingegebenen Passwörter stimmen nicht überein."
 
-#: lib/fb_tools/handling_obj.py:874 lib/fb_tools/handling_obj.py:949
+#: lib/fb_tools/handling_obj.py:869 lib/fb_tools/handling_obj.py:944
 msgid "Interrupted on demand."
 msgstr "Abbruch auf Verlangen."
 
-#: lib/fb_tools/handling_obj.py:899 lib/fb_tools/handling_obj.py:904 lib/fb_tools/handling_obj.py:983
-#: lib/fb_tools/handling_obj.py:988
+#: lib/fb_tools/handling_obj.py:894 lib/fb_tools/handling_obj.py:899 lib/fb_tools/handling_obj.py:978
+#: lib/fb_tools/handling_obj.py:983
 msgid "Got a {}:"
 msgstr "Habe ein {} erhalten:"
 
-#: lib/fb_tools/handling_obj.py:934
+#: lib/fb_tools/handling_obj.py:929
 msgid "Yes/No"
 msgstr "Ja/Nein"
 
-#: lib/fb_tools/handling_obj.py:942
+#: lib/fb_tools/handling_obj.py:937
 msgid "Automatic answer: '{}'."
 msgstr "Automatische Antwort: '{}'."
 
-#: lib/fb_tools/handling_obj.py:1031 lib/fb_tools/handling_obj.py:1037
+#: lib/fb_tools/handling_obj.py:1026 lib/fb_tools/handling_obj.py:1032
 msgid "Parameter {t!r} must be a {e}, {v!r} was given."
 msgstr "Der Parameter {t!r} muss ein {e} ein, statt dessen wurde {v!r} übergeben."
 
-#: lib/fb_tools/handling_obj.py:1100
+#: lib/fb_tools/handling_obj.py:1095
 msgid "Completed process"
 msgstr "Fertiggestellter Prozess"
 
-#: lib/fb_tools/mailaddress.py:69 lib/fb_tools/mailaddress.py:468
+#: lib/fb_tools/mailaddress.py:65 lib/fb_tools/mailaddress.py:464
 msgid "Empty address."
 msgstr "Leere Adresse."
 
-#: lib/fb_tools/mailaddress.py:78 lib/fb_tools/mailaddress.py:477
+#: lib/fb_tools/mailaddress.py:74 lib/fb_tools/mailaddress.py:473
 msgid "Wrong type."
 msgstr "Falscher Typ."
 
-#: lib/fb_tools/mailaddress.py:88 lib/fb_tools/mailaddress.py:495 lib/fb_tools/mailaddress.py:535
-#: lib/fb_tools/mailaddress.py:558
+#: lib/fb_tools/mailaddress.py:84 lib/fb_tools/mailaddress.py:491 lib/fb_tools/mailaddress.py:531
+#: lib/fb_tools/mailaddress.py:554
 msgid "Invalid address."
 msgstr "Ungültige Adresse."
 
-#: lib/fb_tools/mailaddress.py:106 lib/fb_tools/mailaddress.py:167
+#: lib/fb_tools/mailaddress.py:102 lib/fb_tools/mailaddress.py:163
 msgid "Given user: {u!r}, given domain: {d!r}."
 msgstr "Gegebener Nutzer: {u!r}, gegebene Domäne: {d!r}."
 
-#: lib/fb_tools/mailaddress.py:111
+#: lib/fb_tools/mailaddress.py:107
 msgid "Invalid mail address."
 msgstr "Ungültige Mailadresse."
 
-#: lib/fb_tools/mailaddress.py:128 lib/fb_tools/mailaddress.py:143
+#: lib/fb_tools/mailaddress.py:124 lib/fb_tools/mailaddress.py:139
 msgid "Invalid user/mailbox name."
 msgstr "Ungültiger Nutzer- bzw. Postfachname."
 
-#: lib/fb_tools/mailaddress.py:150
+#: lib/fb_tools/mailaddress.py:146
 msgid "Invalid domain."
 msgstr "Ungültige Domäne."
 
-#: lib/fb_tools/mailaddress.py:204 lib/fb_tools/obj.py:252 lib/fb_tools/obj.py:308
+#: lib/fb_tools/mailaddress.py:200 lib/fb_tools/obj.py:247 lib/fb_tools/obj.py:303
 msgid "Wrong verbose level {!r}, must be >= 0"
 msgstr "Falsches Ausführlichkeits-Niveau, muss größer als oder gleich Null sein"
 
-#: lib/fb_tools/mailaddress.py:296 lib/fb_tools/mailaddress.py:656
+#: lib/fb_tools/mailaddress.py:292 lib/fb_tools/mailaddress.py:652
 msgid "Checking equality {self!r} with {other!r} ..."
 msgstr "Vergleiche Gleichheit von {self!r} mit {other!r} …"
 
-#: lib/fb_tools/mailaddress.py:352 lib/fb_tools/mailaddress.py:680
+#: lib/fb_tools/mailaddress.py:348 lib/fb_tools/mailaddress.py:676
 msgid "Object {o!r} for comparing is not a {c} object."
 msgstr "Das Vergleichsobjekt {o!r} ist kein {c}-Objekt."
 
-#: lib/fb_tools/mailaddress.py:357 lib/fb_tools/mailaddress.py:685
+#: lib/fb_tools/mailaddress.py:353 lib/fb_tools/mailaddress.py:681
 msgid "Comparing {self!r} with {other!r} ..."
 msgstr "Vergleiche {self!r} mit {other!r} …"
 
-#: lib/fb_tools/mailaddress.py:485
+#: lib/fb_tools/mailaddress.py:481
 msgid "Evaluating address {!r} ..."
 msgstr "Untersuche Adresse {!r} …"
 
-#: lib/fb_tools/mailaddress.py:486
+#: lib/fb_tools/mailaddress.py:482
 msgid "Search pattern simple: {}"
 msgstr "Einfaches Suchmuster: {}"
 
-#: lib/fb_tools/mailaddress.py:491
+#: lib/fb_tools/mailaddress.py:487
 msgid "Search pattern full: {}"
 msgstr "Vollständiges Suchmuster: {}"
 
-#: lib/fb_tools/mailaddress.py:515
+#: lib/fb_tools/mailaddress.py:511
 msgid "Parameters {lst} may not be given, if parameter {a!r} was given."
 msgstr "Die Parameter {lst} dürfen nicht übergeben werden, wenn der Parameter {a!r} angegeben wurde."
 
-#: lib/fb_tools/mailaddress.py:526
+#: lib/fb_tools/mailaddress.py:522
 msgid "Invalid full user name."
 msgstr "Ungültiger vollständiger Nutzername."
 
-#: lib/fb_tools/mailaddress.py:879 lib/fb_tools/mailaddress.py:893
+#: lib/fb_tools/mailaddress.py:875 lib/fb_tools/mailaddress.py:889
 msgid "Given object {o!r} is not a sequence type, but a {t!r} type instead."
 msgstr "Das übergebene Objekt {o!r} ist kein sequentieller Typ, aber statt dessen vom Typ {t!r}."
 
-#: lib/fb_tools/mailaddress.py:908
+#: lib/fb_tools/mailaddress.py:904
 msgid "{m} takes at most {max} arguments ({n} given)."
 msgstr "{m} akzeptiert höchstens {max} Argumente ({n} wurden gegeben)."
 
-#: lib/fb_tools/mailaddress.py:948
+#: lib/fb_tools/mailaddress.py:944
 msgid "Mail address {} is not in address list."
 msgstr "Die Mailadresse {} ist nicht in der Adressliste."
 
-#: lib/fb_tools/multi_config.py:100
+#: lib/fb_tools/multi_config.py:92
 msgid "Config loader method {!r} was not found."
 msgstr "Die Konfigurations-Lade-Methode {!r} wurde nicht gefunden."
 
-#: lib/fb_tools/multi_config.py:211 lib/fb_tools/multi_config.py:213 lib/fb_tools/multi_config.py:215
+#: lib/fb_tools/multi_config.py:203 lib/fb_tools/multi_config.py:205 lib/fb_tools/multi_config.py:207
 msgid "{} configuration is not supported."
 msgstr "{}-Konfiguration wird nicht unterstützt."
 
-#: lib/fb_tools/multi_config.py:268
+#: lib/fb_tools/multi_config.py:260
 msgid "Additional config file {!r} does not exists."
 msgstr "Die zusätzliche Konfigurationsdatei {!r} existiert nicht."
 
-#: lib/fb_tools/multi_config.py:282
+#: lib/fb_tools/multi_config.py:274
 msgid "Configuration file {!r} is not readable."
 msgstr "Die Konfigurations-Datei {!r} ist nicht lesbar."
 
-#: lib/fb_tools/multi_config.py:306
+#: lib/fb_tools/multi_config.py:298
 msgid "Configuration directory {!r} may not be absolute."
 msgstr "Das Konfigurations-Verzeichnis {!r} darf nicht absolut sein."
 
-#: lib/fb_tools/multi_config.py:386
+#: lib/fb_tools/multi_config.py:378
 msgid "Cannot use {!r} as delimiters for ini-files."
 msgstr "Kann {!r} nicht als Trennzeichen für ini-Dateien verwenden."
 
-#: lib/fb_tools/multi_config.py:408
+#: lib/fb_tools/multi_config.py:400
 msgid "Cannot use {!r} as comment prefixes for ini-files."
 msgstr "Kann {!r} nicht als Kommentar-Präfix für ini-Dateien verwenden."
 
-#: lib/fb_tools/multi_config.py:430
+#: lib/fb_tools/multi_config.py:422
 msgid "Cannot use {!r} as inline comment prefixes for ini-files."
 msgstr "Kann {!r} nicht als Inline-Kommentar-Präfix für ini-Dateien verwenden."
 
-#: lib/fb_tools/multi_config.py:616 lib/fb_tools/multi_config.py:627
+#: lib/fb_tools/multi_config.py:608 lib/fb_tools/multi_config.py:619
 msgid "Stem {!r} is not a String type."
 msgstr "Der Konfigurations-Namens-Stamm {!r} ist kein String-Typ."
 
-#: lib/fb_tools/multi_config.py:620 lib/fb_tools/multi_config.py:631 lib/fb_tools/multi_config.py:638
+#: lib/fb_tools/multi_config.py:612 lib/fb_tools/multi_config.py:623 lib/fb_tools/multi_config.py:630
 msgid "File name stem {!r} is invalid."
 msgstr "der Konfigurations-Namens-Stamm {!r} ist ungültig."
 
-#: lib/fb_tools/multi_config.py:646
+#: lib/fb_tools/multi_config.py:638
 msgid "Invalid configuration type {t!r} - not found in {w!r}."
 msgstr "Ungültiger Konfigurationstyp {t!r} - wurde nicht in {w!r} gefunden."
 
-#: lib/fb_tools/multi_config.py:686
+#: lib/fb_tools/multi_config.py:678
 msgid "Collecting all configuration files."
 msgstr "Sammle alle Konfigurationsdateien."
 
-#: lib/fb_tools/multi_config.py:693
+#: lib/fb_tools/multi_config.py:685
 msgid "Discovering config directory {!r} ..."
 msgstr "Untersuche Konfigurations-Verzeichnis {!r} …"
 
-#: lib/fb_tools/multi_config.py:702
+#: lib/fb_tools/multi_config.py:694
 msgid "Collected config files:"
 msgstr "Gesammelte Konfigurationsdateien:"
 
-#: lib/fb_tools/multi_config.py:715
+#: lib/fb_tools/multi_config.py:707
 msgid "Checking permissions of config files ..."
 msgstr "Überprüfe Rechte auf Konfigurationsdateien …"
 
-#: lib/fb_tools/multi_config.py:731
+#: lib/fb_tools/multi_config.py:723
 msgid "Checking permissions of {!r} ..."
 msgstr "Überprüfe Rechte auf {!r} …"
 
-#: lib/fb_tools/multi_config.py:735
+#: lib/fb_tools/multi_config.py:727
 msgid "Found file permissions of {fn!r}: {mode:04o}"
 msgstr "Fand Datei-Rechte auf {fn!r}: {mode:04o}"
 
-#: lib/fb_tools/multi_config.py:738
+#: lib/fb_tools/multi_config.py:730
 msgid "File {fn!r} is readable by group or by others, found mode {mode:04o}."
 msgstr "Die Datei {fn!r} ist für die Gruppe oder für andere lesbar, gefundener Modus {mode:04o}."
 
-#: lib/fb_tools/multi_config.py:750
+#: lib/fb_tools/multi_config.py:742
 msgid "Trying to detect file type of additional config file {!r}."
 msgstr "Versuche den Dateityp der zusätzlichen Konfigurationsdatei {!r} zu ermitteln."
 
-#: lib/fb_tools/multi_config.py:759 lib/fb_tools/multi_config.py:824
+#: lib/fb_tools/multi_config.py:751 lib/fb_tools/multi_config.py:816
 msgid "Checking file {fn!r} for pattern {pat!r}."
 msgstr "Überprüfe Datei {fn!r} nach Muster {pat!r}."
 
-#: lib/fb_tools/multi_config.py:765 lib/fb_tools/multi_config.py:830
+#: lib/fb_tools/multi_config.py:757 lib/fb_tools/multi_config.py:822
 msgid "Found config file {fi!r}, loader method {m!r}."
 msgstr "Fand Konfigurationsdatei {fi!r}, Lademethode {m!r}."
 
-#: lib/fb_tools/multi_config.py:779
+#: lib/fb_tools/multi_config.py:771
 msgid "Did not found file type of additional config file {fn!r}. Available config types are: {list}."
 msgstr ""
 "Keinen Dateityp der zusätzlichen Konfigurationsdatei {fn!r} gefunden. Verfügbare Dateitypen "
 "sind: {list}."
 
-#: lib/fb_tools/multi_config.py:798
+#: lib/fb_tools/multi_config.py:790
 msgid "Something strange is happend, file type {!r} not found."
 msgstr "Irgendwas komisches ist passiert, der Dateityp {!r} wurde nicht gefunden."
 
-#: lib/fb_tools/multi_config.py:808
+#: lib/fb_tools/multi_config.py:800
 msgid "Checking, whether {!r} is a possible config file."
 msgstr "Teste, ob {!r} möglicherweise eine Konfigurationsdatei ist."
 
-#: lib/fb_tools/multi_config.py:813
+#: lib/fb_tools/multi_config.py:805
 msgid "Path {!r} is not a regular file."
 msgstr "Der Pfad {!r} ist keine reguläre Datei."
 
-#: lib/fb_tools/multi_config.py:849
+#: lib/fb_tools/multi_config.py:841
 msgid "Reading configuration file {!r} ..."
 msgstr "Lese Konfigurationsdatei {!r} …"
 
-#: lib/fb_tools/multi_config.py:853
+#: lib/fb_tools/multi_config.py:845
 msgid "Using loading method {!r}."
 msgstr "Verwende Lade-Methode {!r}."
 
-#: lib/fb_tools/multi_config.py:861
+#: lib/fb_tools/multi_config.py:853
 msgid "Read config from {fn!r}:"
 msgstr "Von {fn!r} gelesene Konfiguration:"
 
-#: lib/fb_tools/multi_config.py:872
+#: lib/fb_tools/multi_config.py:864
 msgid "Read merged config:"
 msgstr "Gelesene und zusammengeführte Konfiguration:"
 
-#: lib/fb_tools/multi_config.py:879
+#: lib/fb_tools/multi_config.py:871
 msgid ""
 "Character set detection by module {mod!r} for file {fn!r} should not be used, using character "
 "set {enc!r}."
 msgstr ""
 "Die Zeichesatzerkennung durch das Modul {mod!r} für die Datei {fn!r} soll nicht verwendet "
 "werden, verwende Zeichensatz {enc!r}."
 
-#: lib/fb_tools/multi_config.py:886
+#: lib/fb_tools/multi_config.py:878
 msgid "Trying to detect character set of file {fn!r} ..."
 msgstr "Versuche den Zeichensatz der Datei {fn!r} zu ermitteln …"
 
-#: lib/fb_tools/multi_config.py:897
+#: lib/fb_tools/multi_config.py:889
 #, python-format
 msgid ""
 "The confidence of {con:0.1f}% is lower than the limit of {lim:0.1f}%, using character set "
 "{cs_def!r} instead of {cs_found!r}."
 msgstr ""
 "Die Zuverlässigkeit von {con:0.1f}% ist kleiner als das Limit von {lim:0.1f}%, verwende den "
 "Zeichensatz {cs_def!r} anstelle von {cs_found!r}."
 
-#: lib/fb_tools/multi_config.py:907
+#: lib/fb_tools/multi_config.py:899
 msgid "Got {what} on detecting cheracter set of {fn!r}: {e}"
 msgstr "Erhielt {what} bei der Zeichensatzerkennung von {fn!r}: {e}."
 
-#: lib/fb_tools/multi_config.py:912
+#: lib/fb_tools/multi_config.py:904
 msgid "Found character set {cs!r} for file {fn!r} with a confidence of {con:0.1f}%."
 msgstr "Fand Zeichensatz {cs!r} für die Datei {fn!r} mit einer Zuverlässigkeit von {con:0.1f}%."
 
-#: lib/fb_tools/multi_config.py:922 lib/fb_tools/multi_config.py:952 lib/fb_tools/multi_config.py:986
-#: lib/fb_tools/multi_config.py:1043 lib/fb_tools/multi_config.py:1069
+#: lib/fb_tools/multi_config.py:914 lib/fb_tools/multi_config.py:944 lib/fb_tools/multi_config.py:978
+#: lib/fb_tools/multi_config.py:1035 lib/fb_tools/multi_config.py:1061
 msgid "Reading {tp} file {fn!r} ..."
 msgstr "Lese {tp}-Datei {fn!r} …"
 
-#: lib/fb_tools/multi_config.py:933 lib/fb_tools/multi_config.py:967 lib/fb_tools/multi_config.py:1050
-#: lib/fb_tools/multi_config.py:1083
+#: lib/fb_tools/multi_config.py:925 lib/fb_tools/multi_config.py:959 lib/fb_tools/multi_config.py:1042
+#: lib/fb_tools/multi_config.py:1075
 msgid "{what} parse error in {fn!r}, line {line}, column {col}: {msg}"
 msgstr "{what} Parse-Fehler in {fn!r}, Zeine {line}, Spalte {col}: {msg}"
 
-#: lib/fb_tools/multi_config.py:940 lib/fb_tools/multi_config.py:974 lib/fb_tools/multi_config.py:1021
-#: lib/fb_tools/multi_config.py:1057 lib/fb_tools/multi_config.py:1087
-#: lib/fb_tools/multi_config.py:1094
+#: lib/fb_tools/multi_config.py:932 lib/fb_tools/multi_config.py:966 lib/fb_tools/multi_config.py:1013
+#: lib/fb_tools/multi_config.py:1049 lib/fb_tools/multi_config.py:1079
+#: lib/fb_tools/multi_config.py:1086
 msgid "Got {what} on reading and parsing {fn!r}: {e}"
 msgstr "Habe {what} beim Lesen und Parsen von {fn!r} erhalten: {e}."
 
-#: lib/fb_tools/multi_config.py:1003
+#: lib/fb_tools/multi_config.py:995
 msgid "Arguments on initializing {}:"
 msgstr "Argumente zur Initialisierung von {}:"
 
-#: lib/fb_tools/multi_config.py:1107
+#: lib/fb_tools/multi_config.py:1099
 msgid "Evaluation of configuration could only be happen after reading it."
 msgstr "Die Evaluierung der Konfiguration kann erst erfolgen, nachdem die gelesen wurde."
 
-#: lib/fb_tools/multi_config.py:1127
+#: lib/fb_tools/multi_config.py:1119
 msgid "Invalid value {val!r} in section {sec!r} for console timeout."
 msgstr "Ungültiger Wert {val!r} für Konsolen-Timeout in Abschnitt {sec!r}."
 
-#: lib/fb_tools/obj.py:63
+#: lib/fb_tools/obj.py:58
 msgid "The base directory {!r} is not existing or not a directory."
 msgstr "Das Basis-Verzeichnis {!r} existiert nicht oder ist kein Verzeichnis."
 
-#: lib/fb_tools/obj.py:146
+#: lib/fb_tools/obj.py:141
 msgid "undefined error."
 msgstr "unbestimmter Fehler."
 
-#: lib/fb_tools/obj.py:155
+#: lib/fb_tools/obj.py:150
 msgid "Exception happened"
 msgstr "Aufgetretene Ausnahme"
 
-#: lib/fb_tools/obj.py:332
+#: lib/fb_tools/obj.py:327
 msgid "Base directory {!r} does not exists."
 msgstr "Das Basis-Verzeichnis {!r} existiert nicht."
 
-#: lib/fb_tools/obj.py:335
+#: lib/fb_tools/obj.py:330
 msgid "Path for base directory {!r} is not a directory."
 msgstr "Der Pfad zum Basis-Verzeichnis {!r} is kein Verzeichnis"
 
-#: lib/fb_tools/pidfile.py:72
+#: lib/fb_tools/pidfile.py:69
 msgid "Invalid pidfile {f!r} given: {r}"
 msgstr "Ungültige PID-Datei {f!r} übergeben: {r}"
 
-#: lib/fb_tools/pidfile.py:75
+#: lib/fb_tools/pidfile.py:72
 msgid "Invalid pidfile {!r} given."
 msgstr "Ungültige PID-Datei {!r} übergeben."
 
-#: lib/fb_tools/pidfile.py:99
+#: lib/fb_tools/pidfile.py:96
 msgid "The pidfile {f!r} is currently in use by the application with the PID {p}."
 msgstr "Die PID-Datei {f!r} wird gegenwärtig von der Anwendung mit der PID {p} verwendet."
 
-#: lib/fb_tools/pidfile.py:166
+#: lib/fb_tools/pidfile.py:163
 msgid "No filename given on initializing {} object."
 msgstr "Kein Dateiname bei der Initialisierung des {}-Ojektes angegeben."
 
-#: lib/fb_tools/pidfile.py:284
+#: lib/fb_tools/pidfile.py:281
 msgid "Pidfile {!r} doesn't exists, not removing."
 msgstr "Die PID-Datei {!r} existiert nicht, und wird deshalb auch nicht gelöscht."
 
-#: lib/fb_tools/pidfile.py:290
+#: lib/fb_tools/pidfile.py:287
 msgid "Auto removing disabled, don't deleting {!r}."
 msgstr "Automatisches Löschen deaktiviert, {!r} wird nicht gelöscht."
 
-#: lib/fb_tools/pidfile.py:295
+#: lib/fb_tools/pidfile.py:292
 msgid "Removing pidfile {!r} ..."
 msgstr "Lösche PID-Datei {!r} …"
 
-#: lib/fb_tools/pidfile.py:298 lib/fb_tools/pidfile.py:332
+#: lib/fb_tools/pidfile.py:295 lib/fb_tools/pidfile.py:329
 msgid "Just kidding ..."
 msgstr "Ich mach doch nur Spaß …"
 
-#: lib/fb_tools/pidfile.py:303
+#: lib/fb_tools/pidfile.py:300
 msgid "Could not delete pidfile {f!r}: {e}"
 msgstr "Konnte PID-Datei {f!r} nicht löschen: {e}"
 
-#: lib/fb_tools/pidfile.py:322
+#: lib/fb_tools/pidfile.py:319 lib/fb_tools/pidfile.py:382
 msgid "Invalid PID {p} for creating pidfile {f!r} given."
 msgstr "Ungültige PID {p} zur Erstellung der PID-Datei {f!r} übergeben."
 
-#: lib/fb_tools/pidfile.py:330
+#: lib/fb_tools/pidfile.py:327
 msgid "Deleting pidfile {!r} ..."
 msgstr "Lösche PID-Datei {!r} …"
 
-#: lib/fb_tools/pidfile.py:340
+#: lib/fb_tools/pidfile.py:337
 msgid "Trying opening {!r} exclusive ..."
 msgstr "Versuche {!r} exklusiv zu öffnen …"
 
-#: lib/fb_tools/pidfile.py:343 lib/fb_tools/pidfile.py:395
+#: lib/fb_tools/pidfile.py:340 lib/fb_tools/pidfile.py:392
 msgid "Simulation mode - don't real writing in {!r}."
 msgstr "Simulationsmodus - es wird nicht wirklich nach {!r} geschrieben."
 
-#: lib/fb_tools/pidfile.py:354
+#: lib/fb_tools/pidfile.py:351
 msgid "Error on creating pidfile {f!r}: {e}"
 msgstr "Fehler beim Erstellen der PID-Datei {f!r}: {e}"
 
-#: lib/fb_tools/pidfile.py:358 lib/fb_tools/pidfile.py:401
+#: lib/fb_tools/pidfile.py:355 lib/fb_tools/pidfile.py:398
 msgid "Writing {p} into {f!r} ..."
 msgstr "Schreibe {p} nach {f!r} …"
 
-#: lib/fb_tools/pidfile.py:379
+#: lib/fb_tools/pidfile.py:376
 msgid "Calling {} on a not self created pidfile."
 msgstr "Aufruf von {} bei einer nicht selbst erstellten PID-Datei."
 
-#: lib/fb_tools/pidfile.py:392
+#: lib/fb_tools/pidfile.py:389
 msgid "Trying opening {!r} for recreate ..."
 msgstr "Versuche {!r} zum Wiedererstellen zu öffnen …"
 
-#: lib/fb_tools/pidfile.py:407
+#: lib/fb_tools/pidfile.py:404
 msgid "Error on recreating pidfile {f!r}: {e}"
 msgstr "Fehler beim Wiedererstellen der PID-Datei {f!r}: {e}"
 
-#: lib/fb_tools/pidfile.py:433
+#: lib/fb_tools/pidfile.py:430
 msgid "Pidfile parent directory {!r} doesn't exists."
 msgstr "Das Eltern-Verzeichnis der PID-Datei {!r} existiert nicht."
 
-#: lib/fb_tools/pidfile.py:437
+#: lib/fb_tools/pidfile.py:434
 msgid "Pidfile parent directory {!r} is not a directory."
 msgstr "Das Eltern-Verzeichnis der PID-Datei {!r} is kein Verzeichnis"
 
-#: lib/fb_tools/pidfile.py:441
+#: lib/fb_tools/pidfile.py:438
 msgid "No write access to pidfile parent directory {!r}."
 msgstr "Kein Schreibzugriff auf das Eltern-Verzeichnis der PID-Datei {!r}."
 
-#: lib/fb_tools/pidfile.py:448
+#: lib/fb_tools/pidfile.py:445
 msgid "It is not a regular file."
 msgstr "Es ist keine reguläre Datei."
 
-#: lib/fb_tools/pidfile.py:466
+#: lib/fb_tools/pidfile.py:463
 msgid "Reading content of pidfile {!r} ..."
 msgstr "Lese Inhalt der PID-Datei {!r} …"
 
-#: lib/fb_tools/pidfile.py:487
+#: lib/fb_tools/pidfile.py:484
 msgid "No useful information found in pidfile {f!r}: {z!r}"
 msgstr "Keine sinnvollen Informationen in der PID-Datei {f!r} gefunden: {z!r}"
 
-#: lib/fb_tools/pidfile.py:492
+#: lib/fb_tools/pidfile.py:489
 msgid "Trying check for process with PID {} ..."
 msgstr "Versuche den Prozess mit der PID {} zu überprüfen …"
 
-#: lib/fb_tools/pidfile.py:498
+#: lib/fb_tools/pidfile.py:495
 msgid "Process with PID {} anonymous died."
 msgstr "Der Prozess mit der PID {} ist anonym verstorben."
 
-#: lib/fb_tools/pidfile.py:502
+#: lib/fb_tools/pidfile.py:499
 msgid "No permission to signal the process {} ..."
 msgstr "Keine Rechte zum Senden von Signalen an Prozess {} …"
 
-#: lib/fb_tools/pidfile.py:506
+#: lib/fb_tools/pidfile.py:503
 msgid "Got a {c}: {e}."
 msgstr "Hab eine(e) {c} erhalten: {e}."
 
-#: lib/fb_tools/xlate.py:107
+#: lib/fb_tools/xlate.py:106
 msgid "Module directory: {!r}"
 msgstr "Modul-Verzeichnis: {!r}"
 
-#: lib/fb_tools/xlate.py:108
+#: lib/fb_tools/xlate.py:107
 msgid "Base directory: {!r}"
 msgstr "Basis-Verzeichnis: {!r}"
 
-#: lib/fb_tools/xlate.py:109
+#: lib/fb_tools/xlate.py:108
 msgid "Locale directory: {!r}"
 msgstr "Verzeichnis für Locales: {!r}"
 
-#: lib/fb_tools/xlate.py:110
+#: lib/fb_tools/xlate.py:109
 msgid "Locale domain: {!r}"
 msgstr "Locale-Domäne: {!r}"
 
-#: lib/fb_tools/xlate.py:111
+#: lib/fb_tools/xlate.py:110
 msgid "Found .mo-file: {!r}"
 msgstr "Gefundene .mo-Datei: {!r}"
```

### Comparing `fb_tools-2.2.2/locale/en/LC_MESSAGES/fb_tools.mo` & `fb_tools-2.2.3/locale/en/LC_MESSAGES/fb_tools.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: fb_tools 2.1.2\n"
+"Project-Id-Version: fb_tools 2.2.3\n"
 "Report-Msgid-Bugs-To: frank@brehm-online.com\n"
-"POT-Creation-Date: 2022-11-21 14:24+0100\n"
-"PO-Revision-Date: 2022-07-20 16:50+0100\n"
+"POT-Creation-Date: 2023-05-31 14:28+0200\n"
+"PO-Revision-Date: 2023-05-31 17:30+0100\n"
 "Last-Translator: Frank Brehm <frank@brehm-online.com>\n"
 "Language: en\n"
 "Language-Team: en <frank@brehm-online.com>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Automatic removing of {!r} ..."
 msgstr "Automatic removing of {!r} …"
 
 msgid "Checking config section {!r} ..."
 msgstr "Checking config section {!r} …"
```

### Comparing `fb_tools-2.2.2/locale/en/LC_MESSAGES/fb_tools.po` & `fb_tools-2.2.3/locale/en/LC_MESSAGES/fb_tools.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,177 +1,177 @@
 # English translations for fb_tools.
-# Copyright (C) 2022 Frank Brehm, Berlin
+# Copyright (C) 2023 Frank Brehm, Berlin
 # This file is distributed under the same license as the fb_tools project.
-# Frank Brehm <frank.brehm@pixelpark.com>, 2022.
+# Frank Brehm <frank@brehm-online.com>, 2023.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: fb_tools 2.1.2\n"
+"Project-Id-Version: fb_tools 2.2.3\n"
 "Report-Msgid-Bugs-To: frank@brehm-online.com\n"
-"POT-Creation-Date: 2022-11-21 14:24+0100\n"
-"PO-Revision-Date: 2022-07-20 16:50+0100\n"
+"POT-Creation-Date: 2023-05-31 14:28+0200\n"
+"PO-Revision-Date: 2023-05-31 17:30+0100\n"
 "Last-Translator: Frank Brehm <frank@brehm-online.com>\n"
 "Language: en\n"
 "Language-Team: en <frank@brehm-online.com>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 #: bin/get-file-to-remove:84
 msgid ""
 "{c}-Object:\n"
 "{a}"
 msgstr ""
 
-#: lib/fb_tools/app.py:69
+#: lib/fb_tools/app.py:64
 msgid "Forced execution - whatever it means."
 msgstr ""
 
-#: lib/fb_tools/app.py:151
+#: lib/fb_tools/app.py:146
 msgid "Invalid env_prefix {!r} given - it may not be empty."
 msgstr ""
 
-#: lib/fb_tools/app.py:155
+#: lib/fb_tools/app.py:150
 msgid ""
 "Invalid characters found in env_prefix {!r}, only alphanumeric characters and digits and "
 "underscore (this not as the first character) are allowed."
 msgstr ""
 
-#: lib/fb_tools/app.py:166
+#: lib/fb_tools/app.py:161
 msgid "Unknown and undescriped application."
 msgstr ""
 
-#: lib/fb_tools/app.py:191
+#: lib/fb_tools/app.py:186
 msgid "Wrong exit_value {!r}, must be >= 0."
 msgstr ""
 
-#: lib/fb_tools/app.py:428
+#: lib/fb_tools/app.py:423
 msgid "Trying to get {} via console ..."
 msgstr "Trying to get {} via console …"
 
-#: lib/fb_tools/app.py:444
+#: lib/fb_tools/app.py:439
 msgid "Got a signal {}."
 msgstr ""
 
-#: lib/fb_tools/app.py:447
+#: lib/fb_tools/app.py:442
 msgid "Got a signal {n!r} ({s})."
 msgstr ""
 
-#: lib/fb_tools/app.py:454
+#: lib/fb_tools/app.py:449
 msgid "Exit on signal {n!r} ({s})."
 msgstr ""
 
-#: lib/fb_tools/app.py:462
+#: lib/fb_tools/app.py:457
 msgid "Tweaking signal handlers."
 msgstr ""
 
-#: lib/fb_tools/app.py:468
+#: lib/fb_tools/app.py:463
 msgid "Setting signal handler for {n!r} ({s})."
 msgstr ""
 
-#: lib/fb_tools/app.py:479
+#: lib/fb_tools/app.py:474
 msgid "Enter "
 msgstr ""
 
-#: lib/fb_tools/app.py:486
+#: lib/fb_tools/app.py:481
 msgid "Repeat enter "
 msgstr ""
 
-#: lib/fb_tools/app.py:496
+#: lib/fb_tools/app.py:491
 msgid "{n} and repeated {n} did not match."
 msgstr ""
 
-#: lib/fb_tools/app.py:500
+#: lib/fb_tools/app.py:495
 msgid "Restoring original signal handlers."
 msgstr ""
 
-#: lib/fb_tools/app.py:505
+#: lib/fb_tools/app.py:500
 msgid "Got {n!r}: {s!r}"
 msgstr ""
 
-#: lib/fb_tools/app.py:555
+#: lib/fb_tools/app.py:550
 msgid "The application is not completely initialized."
 msgstr ""
 
-#: lib/fb_tools/app.py:566
+#: lib/fb_tools/app.py:561
 msgid "Object {!r} seems not to be completely initialized."
 msgstr ""
 
-#: lib/fb_tools/app.py:576
+#: lib/fb_tools/app.py:571
 msgid "Ending."
 msgstr ""
 
-#: lib/fb_tools/app.py:594
+#: lib/fb_tools/app.py:589
 msgid "Executing {} ..."
 msgstr "Executing {} …"
 
-#: lib/fb_tools/app.py:616
+#: lib/fb_tools/app.py:611
 msgid "General options"
 msgstr ""
 
-#: lib/fb_tools/app.py:621
+#: lib/fb_tools/app.py:616
 msgid "Simulation mode, nothing is really done."
 msgstr ""
 
-#: lib/fb_tools/app.py:635 lib/fb_tools/app.py:641
+#: lib/fb_tools/app.py:630 lib/fb_tools/app.py:636
 msgid "Automatically answer '{}' for all questions."
 msgstr ""
 
-#: lib/fb_tools/app.py:636 lib/fb_tools/handling_obj.py:941
+#: lib/fb_tools/app.py:631 lib/fb_tools/handling_obj.py:936
 msgid "Yes"
 msgstr ""
 
-#: lib/fb_tools/app.py:642 lib/fb_tools/handling_obj.py:939
+#: lib/fb_tools/app.py:637 lib/fb_tools/handling_obj.py:934
 msgid "No"
 msgstr ""
 
-#: lib/fb_tools/app.py:647 lib/fb_tools/ddns/__init__.py:249
+#: lib/fb_tools/app.py:642 lib/fb_tools/ddns/__init__.py:243
 msgid "SECONDS"
 msgstr ""
 
-#: lib/fb_tools/app.py:649
+#: lib/fb_tools/app.py:644
 msgid "The timeout in seconds for console input. Default: {}"
 msgstr ""
 
-#: lib/fb_tools/app.py:656
+#: lib/fb_tools/app.py:651
 msgid "Use colored output for messages."
 msgstr ""
 
-#: lib/fb_tools/app.py:663
+#: lib/fb_tools/app.py:658
 msgid "Increase the verbosity level"
 msgstr ""
 
-#: lib/fb_tools/app.py:668
+#: lib/fb_tools/app.py:663
 msgid "Silent execution, only warnings and errors are emitted."
 msgstr ""
 
-#: lib/fb_tools/app.py:673
+#: lib/fb_tools/app.py:668
 msgid "Show this help message and exit."
 msgstr ""
 
-#: lib/fb_tools/app.py:677
+#: lib/fb_tools/app.py:672
 msgid "Display brief usage message and exit."
 msgstr ""
 
-#: lib/fb_tools/app.py:679
+#: lib/fb_tools/app.py:674
 #, python-format
 msgid "Version of %(prog)s: {}"
 msgstr ""
 
-#: lib/fb_tools/app.py:682
+#: lib/fb_tools/app.py:677
 msgid "Show program's version number and exit."
 msgstr ""
 
-#: lib/fb_tools/app.py:812
+#: lib/fb_tools/app.py:807
 msgid "Starting in:"
 msgstr ""
 
-#: lib/fb_tools/app.py:834
+#: lib/fb_tools/app.py:829
 msgid "Aborted by user interrupt."
 msgstr ""
 
 #: lib/fb_tools/argparse_actions.py:58
 msgid "Got a {c} for pattern {p!r}: {e}"
 msgstr ""
 
@@ -191,109 +191,109 @@
 msgid "The given directory {!r} is not readable."
 msgstr ""
 
 #: lib/fb_tools/argparse_actions.py:102
 msgid "The given directory {!r} is not writeable."
 msgstr ""
 
-#: lib/fb_tools/argparse_actions.py:130 lib/fb_tools/cfg_app.py:228
+#: lib/fb_tools/argparse_actions.py:130 lib/fb_tools/cfg_app.py:219
 msgid "Directory {!r} does not exists."
 msgstr ""
 
-#: lib/fb_tools/argparse_actions.py:133 lib/fb_tools/cfg_app.py:232
+#: lib/fb_tools/argparse_actions.py:133 lib/fb_tools/cfg_app.py:223
 msgid "Path {!r} exists, but is not a directory."
 msgstr ""
 
 #: lib/fb_tools/argparse_actions.py:139 lib/fb_tools/argparse_actions.py:174
-#: lib/fb_tools/cfg_app.py:239 lib/fb_tools/get_file_rm_app.py:399
+#: lib/fb_tools/cfg_app.py:230 lib/fb_tools/get_file_rm_app.py:395
 msgid "File {!r} is not a regular file."
 msgstr ""
 
-#: lib/fb_tools/argparse_actions.py:142 lib/fb_tools/cfg_app.py:243
+#: lib/fb_tools/argparse_actions.py:142 lib/fb_tools/cfg_app.py:234
 msgid "File {!r} is not writeable."
 msgstr ""
 
-#: lib/fb_tools/argparse_actions.py:146 lib/fb_tools/cfg_app.py:248
+#: lib/fb_tools/argparse_actions.py:146 lib/fb_tools/cfg_app.py:239
 msgid "Directory {!r} is not writeable."
 msgstr ""
 
-#: lib/fb_tools/argparse_actions.py:171 lib/fb_tools/get_file_rm_app.py:390
+#: lib/fb_tools/argparse_actions.py:171 lib/fb_tools/get_file_rm_app.py:386
 msgid "File {!r} does not exists."
 msgstr ""
 
-#: lib/fb_tools/argparse_actions.py:197 lib/fb_tools/multi_config.py:1155
+#: lib/fb_tools/argparse_actions.py:197 lib/fb_tools/multi_config.py:1147
 msgid "A timeout must be greater than zero and less or equal to {}."
 msgstr ""
 
 #: lib/fb_tools/argparse_actions.py:202
 msgid "Wrong timeout {!r}:"
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:64
+#: lib/fb_tools/cfg_app.py:55
 msgid "Parameter {cls!r} must be a subclass of {clinfo!r}."
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:146
+#: lib/fb_tools/cfg_app.py:137
 msgid "Config options and options for logging"
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:151 lib/fb_tools/cfg_app.py:157 lib/fb_tools/ddns/__init__.py:255
-#: lib/fb_tools/get_file_rm_app.py:270
+#: lib/fb_tools/cfg_app.py:142 lib/fb_tools/cfg_app.py:148 lib/fb_tools/ddns/__init__.py:249
+#: lib/fb_tools/get_file_rm_app.py:266
 msgid "FILE"
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:152
+#: lib/fb_tools/cfg_app.py:143
 msgid "Configuration files to use additional to the standard configuration files."
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:158
+#: lib/fb_tools/cfg_app.py:149
 msgid "A logfile for storing all logging output."
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:165
+#: lib/fb_tools/cfg_app.py:156
 msgid "Got command line arguments:"
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:203
+#: lib/fb_tools/cfg_app.py:194
 msgid "Error on reading configuration:"
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:252
+#: lib/fb_tools/cfg_app.py:243
 msgid "Start logging into file {!r} ..."
 msgstr "Start logging into file {!r} …"
 
-#: lib/fb_tools/collections.py:63
+#: lib/fb_tools/collections.py:60
 msgid "Item {item!r} must be of type {must!r}, but is of type {cls!r} instead."
 msgstr ""
 
-#: lib/fb_tools/collections.py:81
+#: lib/fb_tools/collections.py:78
 msgid "Object {o!r} is not a {e} object."
 msgstr ""
 
-#: lib/fb_tools/collections.py:99
+#: lib/fb_tools/collections.py:96
 msgid "Key {key!r} must be of type {must!r}, but is of type {cls!r} instead."
 msgstr ""
 
-#: lib/fb_tools/collections.py:116
+#: lib/fb_tools/collections.py:113
 msgid "Object is neither a {m} object, nor a sequential object, but a {o!r} object instead."
 msgstr ""
 
-#: lib/fb_tools/collections.py:135
+#: lib/fb_tools/collections.py:132
 msgid "Key {!r} is not existing."
 msgstr ""
 
-#: lib/fb_tools/collections.py:154 lib/fb_tools/collections.py:173
+#: lib/fb_tools/collections.py:151 lib/fb_tools/collections.py:170
 msgid "Could update {ex} with {i!r}: {m}"
 msgstr ""
 
-#: lib/fb_tools/collections.py:197
+#: lib/fb_tools/collections.py:194
 msgid "Parameter {p!r} is not a sequence type, but a {c!r} object instead."
 msgstr ""
 
-#: lib/fb_tools/collections.py:1008
+#: lib/fb_tools/collections.py:1005
 msgid "The method {met}() expected at most {max} arguments, got {got}."
 msgstr ""
 
 #: lib/fb_tools/common.py:154
 msgid "{} is a tty."
 msgstr ""
 
@@ -317,325 +317,325 @@
 msgid "Couldn't detect unit {!r}."
 msgstr ""
 
 #: lib/fb_tools/common.py:783
 msgid "Argument {a!r} must be of type {t1!r} or {t2!r}."
 msgstr ""
 
-#: lib/fb_tools/config.py:101 lib/fb_tools/multi_config.py:245
+#: lib/fb_tools/config.py:96 lib/fb_tools/multi_config.py:237
 msgid "Encoding {v!r} must be a {s!r} object, but is a {c!r} object instead."
 msgstr ""
 
-#: lib/fb_tools/config.py:119 lib/fb_tools/multi_config.py:303
+#: lib/fb_tools/config.py:114 lib/fb_tools/multi_config.py:295
 msgid "A configuration directory may not be None."
 msgstr ""
 
-#: lib/fb_tools/config.py:135
+#: lib/fb_tools/config.py:130
 msgid "A configuration file may not be None."
 msgstr ""
 
-#: lib/fb_tools/config.py:140 lib/fb_tools/config.py:148 lib/fb_tools/multi_config.py:275
+#: lib/fb_tools/config.py:135 lib/fb_tools/config.py:143 lib/fb_tools/multi_config.py:267
 msgid "Configuration file {!r} exists, but is not a regular file."
 msgstr ""
 
-#: lib/fb_tools/config.py:178
+#: lib/fb_tools/config.py:173
 msgid "Searching for {!r} ..."
 msgstr "Searching for {!r} …"
 
-#: lib/fb_tools/config.py:180
+#: lib/fb_tools/config.py:175
 msgid "Configuration file {!r} not found."
 msgstr ""
 
-#: lib/fb_tools/config.py:182
+#: lib/fb_tools/config.py:177
 msgid "Configuration file error"
 msgstr ""
 
-#: lib/fb_tools/config.py:193
+#: lib/fb_tools/config.py:188
 msgid "Reading {!r} ..."
 msgstr "Reading {!r} …"
 
-#: lib/fb_tools/config.py:204
+#: lib/fb_tools/config.py:199
 msgid "Wrong configuration in {!r} found"
 msgstr ""
 
-#: lib/fb_tools/config.py:206
+#: lib/fb_tools/config.py:201
 msgid "Configuration parse error"
 msgstr ""
 
-#: lib/fb_tools/config.py:229 lib/fb_tools/multi_config.py:1124
+#: lib/fb_tools/config.py:224 lib/fb_tools/multi_config.py:1116
 msgid "Checking config section {!r} ..."
 msgstr "Checking config section {!r} …"
 
-#: lib/fb_tools/ddns/__init__.py:74
+#: lib/fb_tools/ddns/__init__.py:68
 msgid "Got an error {c} on requesting {u!r}: {m}"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:93
+#: lib/fb_tools/ddns/__init__.py:87
 msgid "Directory does not exists"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:104
+#: lib/fb_tools/ddns/__init__.py:98
 msgid "Path is not a directory"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:115
+#: lib/fb_tools/ddns/__init__.py:109
 msgid "Invalid permissions"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:134
+#: lib/fb_tools/ddns/__init__.py:128
 msgid "This is a base DDNS related application."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:170
+#: lib/fb_tools/ddns/__init__.py:164
 msgid "Invalid user agent {!r} given."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:196
+#: lib/fb_tools/ddns/__init__.py:190
 msgid "DDNS options"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:210 lib/fb_tools/ddns/__init__.py:213
+#: lib/fb_tools/ddns/__init__.py:204 lib/fb_tools/ddns/__init__.py:207
 msgid "Perform action only for {}."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:216
+#: lib/fb_tools/ddns/__init__.py:210
 msgid "The IP protocol, for which the action should be performed (one of {c}, default {d!r})."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:230
+#: lib/fb_tools/ddns/__init__.py:224
 msgid "PROTOCOL"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:240
+#: lib/fb_tools/ddns/__init__.py:234
 msgid "DIRECTORY"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:242
+#: lib/fb_tools/ddns/__init__.py:236
 msgid ""
 "The directory, where to read and write the cache files of the evaluated IP addresses (default: "
 "{!r})."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:250
+#: lib/fb_tools/ddns/__init__.py:244
 msgid "The timeout in seconds for Web requests (default: {})."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:257
+#: lib/fb_tools/ddns/__init__.py:251
 msgid "Configuration file (default: {!r})"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:310 lib/fb_tools/ddns/config.py:210
+#: lib/fb_tools/ddns/__init__.py:304 lib/fb_tools/ddns/config.py:207
 msgid "Invalid value {!r} as timeout:"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:320
+#: lib/fb_tools/ddns/__init__.py:314
 msgid "Setting Loglevel of the {m} module to {ll}."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:331
+#: lib/fb_tools/ddns/__init__.py:325
 msgid "Trying to get my public IPv{} address."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:343
+#: lib/fb_tools/ddns/__init__.py:337
 msgid "Got a response:"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:354
+#: lib/fb_tools/ddns/__init__.py:348
 msgid "Request method: {!r}"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:374
+#: lib/fb_tools/ddns/__init__.py:368
 msgid "Simulation mode, Request will not be sent."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:387
+#: lib/fb_tools/ddns/__init__.py:381
 msgid "Got a {c} on requesting {u!r}: {e}."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:394
+#: lib/fb_tools/ddns/__init__.py:388
 msgid "Failed to parse the response"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:422
+#: lib/fb_tools/ddns/__init__.py:423
 msgid "Checking existence and accessibility of working directory {!r} ..."
 msgstr "Checking existence and accessibility of working directory {!r} …"
 
-#: lib/fb_tools/ddns/__init__.py:434 lib/fb_tools/ddns/update_app.py:169
+#: lib/fb_tools/ddns/__init__.py:435 lib/fb_tools/ddns/update_app.py:165
 msgid "No read access"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:438 lib/fb_tools/ddns/update_app.py:172
+#: lib/fb_tools/ddns/__init__.py:439 lib/fb_tools/ddns/update_app.py:168
 msgid "No write access"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:453
+#: lib/fb_tools/ddns/__init__.py:454
 msgid "Writing IP address {a!r} into {f!r} ..."
 msgstr "Writing IP address {a!r} into {f!r} …"
 
-#: lib/fb_tools/ddns/__init__.py:481
+#: lib/fb_tools/ddns/__init__.py:482
 msgid "File {!r} not found."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:484
+#: lib/fb_tools/ddns/__init__.py:485
 msgid "Reading IP address from {!r}..."
 msgstr "Reading IP address from {!r} …"
 
-#: lib/fb_tools/ddns/__init__.py:504
+#: lib/fb_tools/ddns/__init__.py:505
 msgid "Line {li!r} in {f!r} is not a valid IP address:"
 msgstr ""
 
-#: lib/fb_tools/ddns/config.py:104
+#: lib/fb_tools/ddns/config.py:101
 msgid "Invalid timeout {!r} for Web requests, must be 0 < SECONDS < 3600."
 msgstr ""
 
-#: lib/fb_tools/ddns/config.py:224
+#: lib/fb_tools/ddns/config.py:221
 msgid "Invalid value {ur} for protocols to update, valid protocols are: "
 msgstr ""
 
-#: lib/fb_tools/ddns/config.py:233 lib/fb_tools/ddns/config.py:270
+#: lib/fb_tools/ddns/config.py:230 lib/fb_tools/ddns/config.py:267
 msgid "Unknown configuration option {o!r} with value {v!r} in section {s!r}."
 msgstr ""
 
-#: lib/fb_tools/ddns/config.py:255
+#: lib/fb_tools/ddns/config.py:252
 msgid "The path to the working directory must be an absolute path (given: {!r})."
 msgstr ""
 
-#: lib/fb_tools/ddns/config.py:265
+#: lib/fb_tools/ddns/config.py:262
 msgid "The path to the logfile must be an absolute path (given: {!r})."
 msgstr ""
 
-#: lib/fb_tools/ddns/myip_app.py:50
+#: lib/fb_tools/ddns/myip_app.py:46
 msgid ""
 "Tries to detect the public NAT IPv4 address and/or the automatic assigned IPv6 address in a "
 "local network and print it out."
 msgstr ""
 
-#: lib/fb_tools/ddns/myip_app.py:55 lib/fb_tools/ddns/myip_app.py:56
+#: lib/fb_tools/ddns/myip_app.py:51 lib/fb_tools/ddns/myip_app.py:52
 msgid "Use only {} to retreive the public IP address."
 msgstr ""
 
-#: lib/fb_tools/ddns/myip_app.py:57
+#: lib/fb_tools/ddns/myip_app.py:53
 msgid "The IP protocol, for which the public IP should be retrieved (one of {c}, default {d!r})."
 msgstr ""
 
-#: lib/fb_tools/ddns/myip_app.py:99
+#: lib/fb_tools/ddns/myip_app.py:95
 msgid "myip options"
 msgstr ""
 
-#: lib/fb_tools/ddns/myip_app.py:103
+#: lib/fb_tools/ddns/myip_app.py:99
 msgid "Write found public IPs into a cache file in working directory."
 msgstr ""
 
-#: lib/fb_tools/ddns/myip_app.py:134 lib/fb_tools/ddns/update_app.py:275
+#: lib/fb_tools/ddns/myip_app.py:130 lib/fb_tools/ddns/update_app.py:271
 msgid "Starting {a!r}, version {v!r} ..."
 msgstr "Starting {a!r}, version {v!r} …"
 
-#: lib/fb_tools/ddns/update_app.py:66
+#: lib/fb_tools/ddns/update_app.py:62
 msgid "Updating the DDNS records, even if seems not to be changed."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:69
+#: lib/fb_tools/ddns/update_app.py:65
 msgid "Tries to update the A and/or AAAA record at ddns.de with the current IP address."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:74 lib/fb_tools/ddns/update_app.py:75
+#: lib/fb_tools/ddns/update_app.py:70 lib/fb_tools/ddns/update_app.py:71
 msgid "Update only the {} record with the public IP address."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:76
+#: lib/fb_tools/ddns/update_app.py:72
 msgid ""
 "The IP protocol, for which the appropriate DNS record should be updated with the public IP (one "
 "of {c}, default {d!r})."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:158
+#: lib/fb_tools/ddns/update_app.py:154
 msgid "Checking existence and accessibility of log directory {!r} ..."
 msgstr "Checking existence and accessibility of log directory {!r} …"
 
-#: lib/fb_tools/ddns/update_app.py:190
+#: lib/fb_tools/ddns/update_app.py:186
 msgid "Update DDNS options"
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:193
+#: lib/fb_tools/ddns/update_app.py:189
 msgid "USER"
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:194
+#: lib/fb_tools/ddns/update_app.py:190
 msgid "The username to login at ddns.de."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:198
+#: lib/fb_tools/ddns/update_app.py:194
 msgid "PASSWORD"
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:199
+#: lib/fb_tools/ddns/update_app.py:195
 msgid "The password of the user to login at ddns.de."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:203
+#: lib/fb_tools/ddns/update_app.py:199
 msgid "FILENAME"
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:204
+#: lib/fb_tools/ddns/update_app.py:200
 msgid "The filename to use as a logfile. Leave it empty to disable file logging."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:211
+#: lib/fb_tools/ddns/update_app.py:207
 msgid "Update all domains, which are connected whith the given ddns account."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:215
+#: lib/fb_tools/ddns/update_app.py:211
 msgid "DOMAIN"
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:216
+#: lib/fb_tools/ddns/update_app.py:212
 msgid "The particular domain(s), which should be updated (if not all)."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:234
+#: lib/fb_tools/ddns/update_app.py:230
 msgid "No domains to update given, but the option all domains is deactivated."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:284
+#: lib/fb_tools/ddns/update_app.py:280
 msgid "Ending {a!r}."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:292 lib/fb_tools/ddns/update_app.py:330
+#: lib/fb_tools/ddns/update_app.py:288 lib/fb_tools/ddns/update_app.py:326
 msgid "Last {w} address: {a!r}."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:294 lib/fb_tools/ddns/update_app.py:332
+#: lib/fb_tools/ddns/update_app.py:290 lib/fb_tools/ddns/update_app.py:328
 msgid "Did not found a last {} address."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:297
+#: lib/fb_tools/ddns/update_app.py:293
 msgid "Got no public IPv4 address."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:302 lib/fb_tools/ddns/update_app.py:340
+#: lib/fb_tools/ddns/update_app.py:298 lib/fb_tools/ddns/update_app.py:336
 msgid "Address {a!r} seems not to be a valid {w} address: {e}"
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:307 lib/fb_tools/ddns/update_app.py:345
+#: lib/fb_tools/ddns/update_app.py:303 lib/fb_tools/ddns/update_app.py:341
 msgid "Address {a!r} seems not to be a valid {w} address."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:312 lib/fb_tools/ddns/update_app.py:350
+#: lib/fb_tools/ddns/update_app.py:308 lib/fb_tools/ddns/update_app.py:346
 msgid "Current {w} address is {a!r}."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:315 lib/fb_tools/ddns/update_app.py:353
+#: lib/fb_tools/ddns/update_app.py:311 lib/fb_tools/ddns/update_app.py:349
 msgid "The public {w} address {a!r} seems not to be changed since the last update."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:335
+#: lib/fb_tools/ddns/update_app.py:331
 msgid "Got no public IPv6 address."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:366
+#: lib/fb_tools/ddns/update_app.py:362
 msgid "Updating DNS records to IPv{p} address {a!r} ..."
 msgstr "Updating DNS records to IPv{p} address {a!r} …"
 
 #: lib/fb_tools/errors.py:51
 msgid "Empty mail address."
 msgstr ""
 
@@ -685,969 +685,969 @@
 msgstr[0] ""
 msgstr[1] ""
 
 #: lib/fb_tools/errors.py:362
 msgid "Couldn't occupy lockfile {lf!r} in {d:0.1f} seconds with {tries} tries."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:66
+#: lib/fb_tools/get_file_rm_app.py:62
 msgid "Value must be at least {m} - {v} was given."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:108
+#: lib/fb_tools/get_file_rm_app.py:104
 msgid "The given pattern {!r} is not a valid date pattern"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:112
+#: lib/fb_tools/get_file_rm_app.py:108
 #, python-format
 msgid ". The must be exactly one occurence of '%Y', one of '%m' and one of '%d'."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:143
+#: lib/fb_tools/get_file_rm_app.py:139
 msgid ""
 "Returns a newline separated list of files generated from file globbing patterns given as "
 "arguments to this application, where all files are omitted, which should not be removed."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:182 lib/fb_tools/get_file_rm_app.py:198
-#: lib/fb_tools/get_file_rm_app.py:214 lib/fb_tools/get_file_rm_app.py:230
-#: lib/fb_tools/get_file_rm_app.py:246
+#: lib/fb_tools/get_file_rm_app.py:178 lib/fb_tools/get_file_rm_app.py:194
+#: lib/fb_tools/get_file_rm_app.py:210 lib/fb_tools/get_file_rm_app.py:226
+#: lib/fb_tools/get_file_rm_app.py:242
 msgid "Wrong value {v!r} for {n}, must be >= {m}"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:267
+#: lib/fb_tools/get_file_rm_app.py:263
 msgid "File options"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:271
+#: lib/fb_tools/get_file_rm_app.py:267
 msgid "File pattern to generate list of files to remove."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:274
+#: lib/fb_tools/get_file_rm_app.py:270
 msgid "Keep options"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:277
+#: lib/fb_tools/get_file_rm_app.py:273
 msgid "NR_FILES"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:279
+#: lib/fb_tools/get_file_rm_app.py:275
 msgid "How many of the last files should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:286
+#: lib/fb_tools/get_file_rm_app.py:282
 msgid "DAYS"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:288
+#: lib/fb_tools/get_file_rm_app.py:284
 msgid "How many files one per day from today on should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:295
+#: lib/fb_tools/get_file_rm_app.py:291
 msgid "WEEKS"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:297
+#: lib/fb_tools/get_file_rm_app.py:293
 msgid "How many files one per week from today on should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:304
+#: lib/fb_tools/get_file_rm_app.py:300
 msgid "MONTHS"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:306
+#: lib/fb_tools/get_file_rm_app.py:302
 msgid "How many files one per month from today on should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:313
+#: lib/fb_tools/get_file_rm_app.py:309
 msgid "YEARS"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:315
+#: lib/fb_tools/get_file_rm_app.py:311
 msgid "How many files one per year from today on should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:346
+#: lib/fb_tools/get_file_rm_app.py:342
 msgid "Resolving date pattern {!r}."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:367
+#: lib/fb_tools/get_file_rm_app.py:363
 msgid "Checking given files..."
 msgstr "Checking given files …"
 
-#: lib/fb_tools/get_file_rm_app.py:372
+#: lib/fb_tools/get_file_rm_app.py:368
 msgid "Checking given file {!r} ..."
 msgstr "Checking given file {!r} …"
 
-#: lib/fb_tools/get_file_rm_app.py:381
+#: lib/fb_tools/get_file_rm_app.py:377
 msgid "Resolved paths:"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:383
+#: lib/fb_tools/get_file_rm_app.py:379
 msgid "File pattern {!r} does not match any files."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:388
+#: lib/fb_tools/get_file_rm_app.py:384
 msgid "Checking {!r} ..."
 msgstr "Checking {!r} …"
 
-#: lib/fb_tools/get_file_rm_app.py:394
+#: lib/fb_tools/get_file_rm_app.py:390
 msgid "File {!r} is a regular file."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:397
+#: lib/fb_tools/get_file_rm_app.py:393
 msgid "Path {!r} is a directory."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:404
+#: lib/fb_tools/get_file_rm_app.py:400
 msgid "File {fi!r} does not match pattern {pa!r}."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:414
+#: lib/fb_tools/get_file_rm_app.py:410
 msgid "Date in file {fi!r} is not a valid date: {e}."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:465
+#: lib/fb_tools/get_file_rm_app.py:461
 msgid "Did not found any files to evaluate."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:497
+#: lib/fb_tools/get_file_rm_app.py:493
 msgid "Keeping last file ..."
 msgid_plural "Keeping last {} files ..."
 msgstr[0] "Keeping last file …"
 msgstr[1] "Keeping last {} files …"
 
-#: lib/fb_tools/get_file_rm_app.py:503
+#: lib/fb_tools/get_file_rm_app.py:499
 msgid "Keep last file {!r}."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:508
+#: lib/fb_tools/get_file_rm_app.py:504
 msgid "Files to keep:"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:529
+#: lib/fb_tools/get_file_rm_app.py:525
 msgid "Files to keep for year:"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:551
+#: lib/fb_tools/get_file_rm_app.py:547
 msgid "Got last month: {!r}"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:565
+#: lib/fb_tools/get_file_rm_app.py:561
 msgid "Files to keep for month:"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:579
+#: lib/fb_tools/get_file_rm_app.py:575
 msgid "Got last Monday: {!r}"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:592
+#: lib/fb_tools/get_file_rm_app.py:588
 msgid "Files to keep for week:"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:605
+#: lib/fb_tools/get_file_rm_app.py:601
 msgid "Got last day: {!r}"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:616
+#: lib/fb_tools/get_file_rm_app.py:612
 msgid "Keeping all files from today."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:623
+#: lib/fb_tools/get_file_rm_app.py:619
 msgid "Files to keep for day:"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:640
+#: lib/fb_tools/get_file_rm_app.py:636
 msgid "Trying to get date of file {!r}."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:679
+#: lib/fb_tools/get_file_rm_app.py:675
 msgid "Explored and assigned files:"
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:159
+#: lib/fb_tools/handler/__init__.py:155
 msgid "Invalid time zone name {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:161
+#: lib/fb_tools/handler/__init__.py:157
 msgid "Setting time zone to {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:165
+#: lib/fb_tools/handler/__init__.py:161
 msgid "Name of the time zone: {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:171
+#: lib/fb_tools/handler/__init__.py:167
 msgid "{}-object not initialized."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:173
+#: lib/fb_tools/handler/__init__.py:169
 msgid "Method {} must be overridden in descendant classes."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:250
+#: lib/fb_tools/handler/__init__.py:246
 msgid "Quiet execution."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:298
+#: lib/fb_tools/handler/__init__.py:294
 msgid "Starting synchronous communication with '{}'."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:302
+#: lib/fb_tools/handler/__init__.py:298
 msgid "Finished communication with '{}'."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:316
+#: lib/fb_tools/handler/__init__.py:312
 msgid "Parameter {p!r} is not of type {t!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:321
+#: lib/fb_tools/handler/__init__.py:317
 msgid "Got completed process:"
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:325 lib/fb_tools/handler/__init__.py:336
+#: lib/fb_tools/handler/__init__.py:321 lib/fb_tools/handler/__init__.py:332
 msgid "Output on {}:"
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:357
+#: lib/fb_tools/handler/__init__.py:353
 msgid "Starting asynchronous communication with '{cmd}', heartbeat interval is {interval:0.1f} seconds."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:372
+#: lib/fb_tools/handler/__init__.py:368
 msgid "Checking for the end of the communication ..."
 msgstr "Checking for the end of the communication …"
 
-#: lib/fb_tools/handler/__init__.py:382
+#: lib/fb_tools/handler/__init__.py:378
 msgid "Time to execute the heartbeat handler."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:386
+#: lib/fb_tools/handler/__init__.py:382
 msgid "Sleeping {:0.2f} seconds ..."
 msgstr "Sleeping {:0.2f} seconds …"
 
-#: lib/fb_tools/handler/__init__.py:394 lib/fb_tools/handler/__init__.py:403
+#: lib/fb_tools/handler/__init__.py:390 lib/fb_tools/handler/__init__.py:399
 msgid "   {w} is now: {o!r}"
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:101
+#: lib/fb_tools/handler/lock.py:99
 msgid "Locking directory {!r} doesn't exists or is not a directory."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:128 lib/fb_tools/handler/lock.py:807
+#: lib/fb_tools/handler/lock.py:126 lib/fb_tools/handler/lock.py:805
 msgid "Locking directory {!r} isn't writeable."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:193
+#: lib/fb_tools/handler/lock.py:191
 msgid "No lockfile given on init of a LockObject object."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:199
+#: lib/fb_tools/handler/lock.py:197
 msgid "Lockfile {!r} doesn't exists, but don't worry, it's simulation mode."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:203 lib/fb_tools/handler/lock.py:1045
+#: lib/fb_tools/handler/lock.py:201 lib/fb_tools/handler/lock.py:1043
 msgid "Lockfile {!r} doesn't exists."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:206
+#: lib/fb_tools/handler/lock.py:204
 msgid "Lockfile {!r} is not a regular file."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:360
+#: lib/fb_tools/handler/lock.py:358
 msgid "Closing file descriptor {} ..."
 msgstr "Closing file descriptor {} …"
 
-#: lib/fb_tools/handler/lock.py:371
+#: lib/fb_tools/handler/lock.py:369
 msgid "Automatic removing of {!r} ..."
 msgstr "Automatic removing of {!r} …"
 
-#: lib/fb_tools/handler/lock.py:399
+#: lib/fb_tools/handler/lock.py:397
 msgid "Refreshing atime and mtime of {!r} to the current timestamp."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:533 lib/fb_tools/handler/lock.py:553 lib/fb_tools/handler/lock.py:573
-#: lib/fb_tools/handler/lock.py:597 lib/fb_tools/handler/lock.py:692 lib/fb_tools/handler/lock.py:1034
+#: lib/fb_tools/handler/lock.py:531 lib/fb_tools/handler/lock.py:551 lib/fb_tools/handler/lock.py:571
+#: lib/fb_tools/handler/lock.py:595 lib/fb_tools/handler/lock.py:690 lib/fb_tools/handler/lock.py:1032
 msgid "Value {val!r} for {what} is not a Number."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:538 lib/fb_tools/handler/lock.py:558 lib/fb_tools/handler/lock.py:578
-#: lib/fb_tools/handler/lock.py:602 lib/fb_tools/handler/lock.py:697 lib/fb_tools/handler/lock.py:1038
+#: lib/fb_tools/handler/lock.py:536 lib/fb_tools/handler/lock.py:556 lib/fb_tools/handler/lock.py:576
+#: lib/fb_tools/handler/lock.py:600 lib/fb_tools/handler/lock.py:695 lib/fb_tools/handler/lock.py:1036
 msgid "The value for {what} must be greater than zero (is {val!r})."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:702
+#: lib/fb_tools/handler/lock.py:700
 msgid "The value for {what} must be greater than or equal to zero (is {val!r})."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:787
+#: lib/fb_tools/handler/lock.py:785
 msgid "Invalid PID {} given on calling create_lockfile()."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:796
+#: lib/fb_tools/handler/lock.py:794
 msgid "Using lock directory {!r} ..."
 msgstr "Using lock directory {!r} …"
 
-#: lib/fb_tools/handler/lock.py:804
+#: lib/fb_tools/handler/lock.py:802
 msgid "Trying to lock lockfile {!r} ..."
 msgstr "Trying to lock lockfile {!r} …"
 
-#: lib/fb_tools/handler/lock.py:845
+#: lib/fb_tools/handler/lock.py:843
 msgid "Current time difference: {:0.3f} seconds."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:850
+#: lib/fb_tools/handler/lock.py:848
 msgid "Try {try_nr} on creating lockfile {lfile!r} ..."
 msgstr "Try {try_nr} on creating lockfile {lfile!r} …"
 
-#: lib/fb_tools/handler/lock.py:861 lib/fb_tools/handler/lock.py:980
+#: lib/fb_tools/handler/lock.py:859 lib/fb_tools/handler/lock.py:978
 msgid "Removing lockfile {!r} ..."
 msgstr "Removing lockfile {!r} …"
 
-#: lib/fb_tools/handler/lock.py:866 lib/fb_tools/handler/lock.py:988
+#: lib/fb_tools/handler/lock.py:864 lib/fb_tools/handler/lock.py:986
 msgid "Error on removing lockfile {lfile!r}: {err}"
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:879
+#: lib/fb_tools/handler/lock.py:877
 msgid "Sleeping for {:0.1f} seconds."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:894
+#: lib/fb_tools/handler/lock.py:892
 msgid "Got a lock for lockfile {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:900
+#: lib/fb_tools/handler/lock.py:898
 msgid "Write {what!r} in lockfile {lfile!r} ..."
 msgstr "Write {what!r} in lockfile {lfile!r} …"
 
-#: lib/fb_tools/handler/lock.py:909
+#: lib/fb_tools/handler/lock.py:907
 msgid "Seeking and syncing {!r} ..."
 msgstr "Seeking and syncing {!r} …"
 
-#: lib/fb_tools/handler/lock.py:938
+#: lib/fb_tools/handler/lock.py:936
 msgid "Trying to open {!r} exclusive ..."
 msgstr "Trying to open {!r} exclusive …"
 
-#: lib/fb_tools/handler/lock.py:940
+#: lib/fb_tools/handler/lock.py:938
 msgid "Simulation mode, no real creation of a lockfile."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:948
+#: lib/fb_tools/handler/lock.py:946
 msgid "Error on creating lockfile {lfile!r}: {err}"
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:977
+#: lib/fb_tools/handler/lock.py:975
 msgid "Lockfile {!r} to remove doesn't exists."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:982
+#: lib/fb_tools/handler/lock.py:980
 msgid "Simulation mode - lockfile won't removed."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1042
+#: lib/fb_tools/handler/lock.py:1040
 msgid "Checking lockfile {!r} ..."
 msgstr "Checking lockfile {!r} …"
 
-#: lib/fb_tools/handler/lock.py:1049
+#: lib/fb_tools/handler/lock.py:1047
 msgid "No read access for lockfile {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1053
+#: lib/fb_tools/handler/lock.py:1051
 msgid "No write access for lockfile {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1059
+#: lib/fb_tools/handler/lock.py:1057
 msgid "Unusable lockfile {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1062
+#: lib/fb_tools/handler/lock.py:1060
 msgid "Process with PID {} is unfortunately dead."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1065
+#: lib/fb_tools/handler/lock.py:1063
 msgid "Process with PID {} is still running."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1073
+#: lib/fb_tools/handler/lock.py:1071
 msgid "Could not stat for file {lfile!r}: {err}"
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1080
+#: lib/fb_tools/handler/lock.py:1078
 msgid "Lockfile {lfile!r} is older than {max} seconds ({age} seconds)."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1083
+#: lib/fb_tools/handler/lock.py:1081
 msgid "Lockfile {lfile!r} is {age} seconds old, but not old enough ({max} seconds)."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1110
+#: lib/fb_tools/handler/lock.py:1108
 msgid "Trying to open pidfile {!r} ..."
 msgstr "Trying to open pidfile {!r} …"
 
-#: lib/fb_tools/handler/lock.py:1114
+#: lib/fb_tools/handler/lock.py:1112
 msgid "Could not open pidfile {!r} for reading:"
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1127
+#: lib/fb_tools/handler/lock.py:1125
 msgid "First line of pidfile {!r} was empty."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1138
+#: lib/fb_tools/handler/lock.py:1136
 msgid "Could not interprete {cont!r} as a PID from {file!r}: {err}"
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1147
+#: lib/fb_tools/handler/lock.py:1145
 msgid "Invalid PID {pid} in {file!r} found."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:78
+#: lib/fb_tools/handling_obj.py:73
 msgid "Timeout on communicating with process."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:104
+#: lib/fb_tools/handling_obj.py:99
 msgid "Command {c!r} returned non-zero exit status {rc}."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:142
+#: lib/fb_tools/handling_obj.py:137
 msgid "Command {c!r} timed out after {s} second."
 msgid_plural "Command {c!r} timed out after {s} seconds."
 msgstr[0] ""
 msgstr[1] ""
 
-#: lib/fb_tools/handling_obj.py:303
+#: lib/fb_tools/handling_obj.py:298
 msgid "Wrong prompt timeout {v!r}, must be greater or equal to Null and less or equal to {max}."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:314
+#: lib/fb_tools/handling_obj.py:309
 msgid "yes"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:321
+#: lib/fb_tools/handling_obj.py:316
 msgid "no"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:389
+#: lib/fb_tools/handling_obj.py:384
 msgid "Searching for command {!r} ..."
 msgstr "Searching for command {!r} …"
 
-#: lib/fb_tools/handling_obj.py:394
+#: lib/fb_tools/handling_obj.py:389
 msgid "Command {!r} doesn't exists."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:397 lib/fb_tools/handling_obj.py:421
+#: lib/fb_tools/handling_obj.py:392 lib/fb_tools/handling_obj.py:416
 msgid "Command {!r} is not executable."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:411
+#: lib/fb_tools/handling_obj.py:406
 msgid "Searching command in {!r} ..."
 msgstr "Searching command in {!r} …"
 
-#: lib/fb_tools/handling_obj.py:424
+#: lib/fb_tools/handling_obj.py:419
 msgid "Command {!r} not found."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:496
+#: lib/fb_tools/handling_obj.py:491
 msgid "STDIN and input arguments may not both be used."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:499
+#: lib/fb_tools/handling_obj.py:494
 msgid "Executing command args:"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:502
+#: lib/fb_tools/handling_obj.py:497
 msgid "Performing argument {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:247 lib/fb_tools/handling_obj.py:507
+#: lib/fb_tools/handler/__init__.py:243 lib/fb_tools/handling_obj.py:502
 msgid "Executing: {}"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:510
+#: lib/fb_tools/handling_obj.py:505
 msgid "Simulation mode, not executing: {}"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:518
+#: lib/fb_tools/handling_obj.py:513
 msgid "PID of process: {}"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:524
+#: lib/fb_tools/handling_obj.py:519
 msgid "{c} happened, killing process: {e}"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:626
+#: lib/fb_tools/handling_obj.py:621
 msgid "Nothing to do on signal."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:680 lib/fb_tools/handling_obj.py:769
+#: lib/fb_tools/handling_obj.py:675 lib/fb_tools/handling_obj.py:764
 msgid "File doesn't exists."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:683
+#: lib/fb_tools/handling_obj.py:678
 msgid "Read permission denied."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:686
+#: lib/fb_tools/handling_obj.py:681
 msgid "Reading file content of {!r} ..."
 msgstr "Reading file content of {!r} …"
 
-#: lib/fb_tools/handling_obj.py:774 lib/fb_tools/handling_obj.py:781
+#: lib/fb_tools/handling_obj.py:769 lib/fb_tools/handling_obj.py:776
 msgid "Write permission to {!r} denied."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:776 lib/fb_tools/handling_obj.py:783
+#: lib/fb_tools/handling_obj.py:771 lib/fb_tools/handling_obj.py:778
 msgid "Write permission denied."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:787
+#: lib/fb_tools/handling_obj.py:782
 msgid "Write {what!r} into {to!r}."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:789
+#: lib/fb_tools/handling_obj.py:784
 msgid "Writing {!r} ..."
 msgstr "Writing {!r} …"
 
-#: lib/fb_tools/handling_obj.py:801
+#: lib/fb_tools/handling_obj.py:796
 msgid "Simulating write into {!r}."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:809
+#: lib/fb_tools/handling_obj.py:804
 msgid "Opening {!r} for write unbuffered ..."
 msgstr "Opening {!r} for write unbuffered …"
 
-#: lib/fb_tools/handler/lock.py:913 lib/fb_tools/handling_obj.py:813
+#: lib/fb_tools/handler/lock.py:911 lib/fb_tools/handling_obj.py:808
 msgid "Closing {!r} ..."
 msgstr "Closing {!r} …"
 
-#: lib/fb_tools/handling_obj.py:844
+#: lib/fb_tools/handling_obj.py:839
 msgid "Password:"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:847
+#: lib/fb_tools/handling_obj.py:842
 msgid "Repeat password:"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:861
+#: lib/fb_tools/handling_obj.py:856
 msgid "The entered passwords does not match."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:874 lib/fb_tools/handling_obj.py:949
+#: lib/fb_tools/handling_obj.py:869 lib/fb_tools/handling_obj.py:944
 msgid "Interrupted on demand."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:899 lib/fb_tools/handling_obj.py:904 lib/fb_tools/handling_obj.py:983
-#: lib/fb_tools/handling_obj.py:988
+#: lib/fb_tools/handling_obj.py:894 lib/fb_tools/handling_obj.py:899 lib/fb_tools/handling_obj.py:978
+#: lib/fb_tools/handling_obj.py:983
 msgid "Got a {}:"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:934
+#: lib/fb_tools/handling_obj.py:929
 msgid "Yes/No"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:942
+#: lib/fb_tools/handling_obj.py:937
 msgid "Automatic answer: '{}'."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:1031 lib/fb_tools/handling_obj.py:1037
+#: lib/fb_tools/handling_obj.py:1026 lib/fb_tools/handling_obj.py:1032
 msgid "Parameter {t!r} must be a {e}, {v!r} was given."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:1100
+#: lib/fb_tools/handling_obj.py:1095
 msgid "Completed process"
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:69 lib/fb_tools/mailaddress.py:468
+#: lib/fb_tools/mailaddress.py:65 lib/fb_tools/mailaddress.py:464
 msgid "Empty address."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:78 lib/fb_tools/mailaddress.py:477
+#: lib/fb_tools/mailaddress.py:74 lib/fb_tools/mailaddress.py:473
 msgid "Wrong type."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:88 lib/fb_tools/mailaddress.py:495 lib/fb_tools/mailaddress.py:535
-#: lib/fb_tools/mailaddress.py:558
+#: lib/fb_tools/mailaddress.py:84 lib/fb_tools/mailaddress.py:491 lib/fb_tools/mailaddress.py:531
+#: lib/fb_tools/mailaddress.py:554
 msgid "Invalid address."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:106 lib/fb_tools/mailaddress.py:167
+#: lib/fb_tools/mailaddress.py:102 lib/fb_tools/mailaddress.py:163
 msgid "Given user: {u!r}, given domain: {d!r}."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:111
+#: lib/fb_tools/mailaddress.py:107
 msgid "Invalid mail address."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:128 lib/fb_tools/mailaddress.py:143
+#: lib/fb_tools/mailaddress.py:124 lib/fb_tools/mailaddress.py:139
 msgid "Invalid user/mailbox name."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:150
+#: lib/fb_tools/mailaddress.py:146
 msgid "Invalid domain."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:204 lib/fb_tools/obj.py:252 lib/fb_tools/obj.py:308
+#: lib/fb_tools/mailaddress.py:200 lib/fb_tools/obj.py:247 lib/fb_tools/obj.py:303
 msgid "Wrong verbose level {!r}, must be >= 0"
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:296 lib/fb_tools/mailaddress.py:656
+#: lib/fb_tools/mailaddress.py:292 lib/fb_tools/mailaddress.py:652
 msgid "Checking equality {self!r} with {other!r} ..."
 msgstr "Checking equality {self!r} with {other!r} …"
 
-#: lib/fb_tools/mailaddress.py:352 lib/fb_tools/mailaddress.py:680
+#: lib/fb_tools/mailaddress.py:348 lib/fb_tools/mailaddress.py:676
 msgid "Object {o!r} for comparing is not a {c} object."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:357 lib/fb_tools/mailaddress.py:685
+#: lib/fb_tools/mailaddress.py:353 lib/fb_tools/mailaddress.py:681
 msgid "Comparing {self!r} with {other!r} ..."
 msgstr "Comparing {self!r} with {other!r} …"
 
-#: lib/fb_tools/mailaddress.py:485
+#: lib/fb_tools/mailaddress.py:481
 msgid "Evaluating address {!r} ..."
 msgstr "Evaluating address {!r} …"
 
-#: lib/fb_tools/mailaddress.py:486
+#: lib/fb_tools/mailaddress.py:482
 msgid "Search pattern simple: {}"
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:491
+#: lib/fb_tools/mailaddress.py:487
 msgid "Search pattern full: {}"
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:515
+#: lib/fb_tools/mailaddress.py:511
 msgid "Parameters {lst} may not be given, if parameter {a!r} was given."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:526
+#: lib/fb_tools/mailaddress.py:522
 msgid "Invalid full user name."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:879 lib/fb_tools/mailaddress.py:893
+#: lib/fb_tools/mailaddress.py:875 lib/fb_tools/mailaddress.py:889
 msgid "Given object {o!r} is not a sequence type, but a {t!r} type instead."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:908
+#: lib/fb_tools/mailaddress.py:904
 msgid "{m} takes at most {max} arguments ({n} given)."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:948
+#: lib/fb_tools/mailaddress.py:944
 msgid "Mail address {} is not in address list."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:100
+#: lib/fb_tools/multi_config.py:92
 msgid "Config loader method {!r} was not found."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:211 lib/fb_tools/multi_config.py:213 lib/fb_tools/multi_config.py:215
+#: lib/fb_tools/multi_config.py:203 lib/fb_tools/multi_config.py:205 lib/fb_tools/multi_config.py:207
 msgid "{} configuration is not supported."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:268
+#: lib/fb_tools/multi_config.py:260
 msgid "Additional config file {!r} does not exists."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:282
+#: lib/fb_tools/multi_config.py:274
 msgid "Configuration file {!r} is not readable."
 msgstr "Configuration file {!r} is not readable."
 
-#: lib/fb_tools/multi_config.py:306
+#: lib/fb_tools/multi_config.py:298
 msgid "Configuration directory {!r} may not be absolute."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:386
+#: lib/fb_tools/multi_config.py:378
 msgid "Cannot use {!r} as delimiters for ini-files."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:408
+#: lib/fb_tools/multi_config.py:400
 msgid "Cannot use {!r} as comment prefixes for ini-files."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:430
+#: lib/fb_tools/multi_config.py:422
 msgid "Cannot use {!r} as inline comment prefixes for ini-files."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:616 lib/fb_tools/multi_config.py:627
+#: lib/fb_tools/multi_config.py:608 lib/fb_tools/multi_config.py:619
 msgid "Stem {!r} is not a String type."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:620 lib/fb_tools/multi_config.py:631 lib/fb_tools/multi_config.py:638
+#: lib/fb_tools/multi_config.py:612 lib/fb_tools/multi_config.py:623 lib/fb_tools/multi_config.py:630
 msgid "File name stem {!r} is invalid."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:646
+#: lib/fb_tools/multi_config.py:638
 msgid "Invalid configuration type {t!r} - not found in {w!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:686
+#: lib/fb_tools/multi_config.py:678
 msgid "Collecting all configuration files."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:693
+#: lib/fb_tools/multi_config.py:685
 msgid "Discovering config directory {!r} ..."
 msgstr "Discovering config directory {!r} …"
 
-#: lib/fb_tools/multi_config.py:702
+#: lib/fb_tools/multi_config.py:694
 msgid "Collected config files:"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:715
+#: lib/fb_tools/multi_config.py:707
 msgid "Checking permissions of config files ..."
 msgstr "Checking permissions of config files …"
 
-#: lib/fb_tools/multi_config.py:731
+#: lib/fb_tools/multi_config.py:723
 msgid "Checking permissions of {!r} ..."
 msgstr "Checking permissions of {!r} …"
 
-#: lib/fb_tools/multi_config.py:735
+#: lib/fb_tools/multi_config.py:727
 msgid "Found file permissions of {fn!r}: {mode:04o}"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:738
+#: lib/fb_tools/multi_config.py:730
 msgid "File {fn!r} is readable by group or by others, found mode {mode:04o}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:750
+#: lib/fb_tools/multi_config.py:742
 msgid "Trying to detect file type of additional config file {!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:759 lib/fb_tools/multi_config.py:824
+#: lib/fb_tools/multi_config.py:751 lib/fb_tools/multi_config.py:816
 msgid "Checking file {fn!r} for pattern {pat!r}."
 msgstr "Checking file {fn!r} for pattern {pat!r}."
 
-#: lib/fb_tools/multi_config.py:765 lib/fb_tools/multi_config.py:830
+#: lib/fb_tools/multi_config.py:757 lib/fb_tools/multi_config.py:822
 msgid "Found config file {fi!r}, loader method {m!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:779
+#: lib/fb_tools/multi_config.py:771
 msgid "Did not found file type of additional config file {fn!r}. Available config types are: {list}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:798
+#: lib/fb_tools/multi_config.py:790
 msgid "Something strange is happend, file type {!r} not found."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:808
+#: lib/fb_tools/multi_config.py:800
 msgid "Checking, whether {!r} is a possible config file."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:813
+#: lib/fb_tools/multi_config.py:805
 msgid "Path {!r} is not a regular file."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:849
+#: lib/fb_tools/multi_config.py:841
 msgid "Reading configuration file {!r} ..."
 msgstr "Reading configuration file {!r} …"
 
-#: lib/fb_tools/multi_config.py:853
+#: lib/fb_tools/multi_config.py:845
 msgid "Using loading method {!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:861
+#: lib/fb_tools/multi_config.py:853
 msgid "Read config from {fn!r}:"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:872
+#: lib/fb_tools/multi_config.py:864
 msgid "Read merged config:"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:879
+#: lib/fb_tools/multi_config.py:871
 msgid ""
 "Character set detection by module {mod!r} for file {fn!r} should not be used, using character "
 "set {enc!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:886
+#: lib/fb_tools/multi_config.py:878
 msgid "Trying to detect character set of file {fn!r} ..."
 msgstr "Trying to detect character set of file {fn!r} …"
 
-#: lib/fb_tools/multi_config.py:897
+#: lib/fb_tools/multi_config.py:889
 #, python-format
 msgid ""
 "The confidence of {con:0.1f}% is lower than the limit of {lim:0.1f}%, using character set "
 "{cs_def!r} instead of {cs_found!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:907
+#: lib/fb_tools/multi_config.py:899
 msgid "Got {what} on detecting cheracter set of {fn!r}: {e}"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:912
+#: lib/fb_tools/multi_config.py:904
 msgid "Found character set {cs!r} for file {fn!r} with a confidence of {con:0.1f}%."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:922 lib/fb_tools/multi_config.py:952 lib/fb_tools/multi_config.py:986
-#: lib/fb_tools/multi_config.py:1043 lib/fb_tools/multi_config.py:1069
+#: lib/fb_tools/multi_config.py:914 lib/fb_tools/multi_config.py:944 lib/fb_tools/multi_config.py:978
+#: lib/fb_tools/multi_config.py:1035 lib/fb_tools/multi_config.py:1061
 msgid "Reading {tp} file {fn!r} ..."
 msgstr "Reading {tp} file {fn!r} …"
 
-#: lib/fb_tools/multi_config.py:933 lib/fb_tools/multi_config.py:967 lib/fb_tools/multi_config.py:1050
-#: lib/fb_tools/multi_config.py:1083
+#: lib/fb_tools/multi_config.py:925 lib/fb_tools/multi_config.py:959 lib/fb_tools/multi_config.py:1042
+#: lib/fb_tools/multi_config.py:1075
 msgid "{what} parse error in {fn!r}, line {line}, column {col}: {msg}"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:940 lib/fb_tools/multi_config.py:974 lib/fb_tools/multi_config.py:1021
-#: lib/fb_tools/multi_config.py:1057 lib/fb_tools/multi_config.py:1087
-#: lib/fb_tools/multi_config.py:1094
+#: lib/fb_tools/multi_config.py:932 lib/fb_tools/multi_config.py:966 lib/fb_tools/multi_config.py:1013
+#: lib/fb_tools/multi_config.py:1049 lib/fb_tools/multi_config.py:1079
+#: lib/fb_tools/multi_config.py:1086
 msgid "Got {what} on reading and parsing {fn!r}: {e}"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:1003
+#: lib/fb_tools/multi_config.py:995
 msgid "Arguments on initializing {}:"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:1107
+#: lib/fb_tools/multi_config.py:1099
 msgid "Evaluation of configuration could only be happen after reading it."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:1127
+#: lib/fb_tools/multi_config.py:1119
 msgid "Invalid value {val!r} in section {sec!r} for console timeout."
 msgstr ""
 
-#: lib/fb_tools/obj.py:63
+#: lib/fb_tools/obj.py:58
 msgid "The base directory {!r} is not existing or not a directory."
 msgstr ""
 
-#: lib/fb_tools/obj.py:146
+#: lib/fb_tools/obj.py:141
 msgid "undefined error."
 msgstr ""
 
-#: lib/fb_tools/obj.py:155
+#: lib/fb_tools/obj.py:150
 msgid "Exception happened"
 msgstr ""
 
-#: lib/fb_tools/obj.py:332
+#: lib/fb_tools/obj.py:327
 msgid "Base directory {!r} does not exists."
 msgstr ""
 
-#: lib/fb_tools/obj.py:335
+#: lib/fb_tools/obj.py:330
 msgid "Path for base directory {!r} is not a directory."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:72
+#: lib/fb_tools/pidfile.py:69
 msgid "Invalid pidfile {f!r} given: {r}"
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:75
+#: lib/fb_tools/pidfile.py:72
 msgid "Invalid pidfile {!r} given."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:99
+#: lib/fb_tools/pidfile.py:96
 msgid "The pidfile {f!r} is currently in use by the application with the PID {p}."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:166
+#: lib/fb_tools/pidfile.py:163
 msgid "No filename given on initializing {} object."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:284
+#: lib/fb_tools/pidfile.py:281
 msgid "Pidfile {!r} doesn't exists, not removing."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:290
+#: lib/fb_tools/pidfile.py:287
 msgid "Auto removing disabled, don't deleting {!r}."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:295
+#: lib/fb_tools/pidfile.py:292
 msgid "Removing pidfile {!r} ..."
 msgstr "Removing lockfile {!r} …"
 
-#: lib/fb_tools/pidfile.py:298 lib/fb_tools/pidfile.py:332
+#: lib/fb_tools/pidfile.py:295 lib/fb_tools/pidfile.py:329
 msgid "Just kidding ..."
 msgstr "Just kidding …"
 
-#: lib/fb_tools/pidfile.py:303
+#: lib/fb_tools/pidfile.py:300
 msgid "Could not delete pidfile {f!r}: {e}"
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:322
+#: lib/fb_tools/pidfile.py:319 lib/fb_tools/pidfile.py:382
 msgid "Invalid PID {p} for creating pidfile {f!r} given."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:330
+#: lib/fb_tools/pidfile.py:327
 msgid "Deleting pidfile {!r} ..."
 msgstr "Deleting pidfile {!r} …"
 
-#: lib/fb_tools/pidfile.py:340
+#: lib/fb_tools/pidfile.py:337
 msgid "Trying opening {!r} exclusive ..."
 msgstr "Trying opening {!r} exclusive …"
 
-#: lib/fb_tools/pidfile.py:343 lib/fb_tools/pidfile.py:395
+#: lib/fb_tools/pidfile.py:340 lib/fb_tools/pidfile.py:392
 msgid "Simulation mode - don't real writing in {!r}."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:354
+#: lib/fb_tools/pidfile.py:351
 msgid "Error on creating pidfile {f!r}: {e}"
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:358 lib/fb_tools/pidfile.py:401
+#: lib/fb_tools/pidfile.py:355 lib/fb_tools/pidfile.py:398
 msgid "Writing {p} into {f!r} ..."
 msgstr "Writing {p} into {f!r} …"
 
-#: lib/fb_tools/pidfile.py:379
+#: lib/fb_tools/pidfile.py:376
 msgid "Calling {} on a not self created pidfile."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:392
+#: lib/fb_tools/pidfile.py:389
 msgid "Trying opening {!r} for recreate ..."
 msgstr "Trying opening {!r} for recreate …"
 
-#: lib/fb_tools/pidfile.py:407
+#: lib/fb_tools/pidfile.py:404
 msgid "Error on recreating pidfile {f!r}: {e}"
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:433
+#: lib/fb_tools/pidfile.py:430
 msgid "Pidfile parent directory {!r} doesn't exists."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:437
+#: lib/fb_tools/pidfile.py:434
 msgid "Pidfile parent directory {!r} is not a directory."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:441
+#: lib/fb_tools/pidfile.py:438
 msgid "No write access to pidfile parent directory {!r}."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:448
+#: lib/fb_tools/pidfile.py:445
 msgid "It is not a regular file."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:466
+#: lib/fb_tools/pidfile.py:463
 msgid "Reading content of pidfile {!r} ..."
 msgstr "Reading content of pidfile {!r} …"
 
-#: lib/fb_tools/pidfile.py:487
+#: lib/fb_tools/pidfile.py:484
 msgid "No useful information found in pidfile {f!r}: {z!r}"
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:492
+#: lib/fb_tools/pidfile.py:489
 msgid "Trying check for process with PID {} ..."
 msgstr "Trying check for process with PID {} …"
 
-#: lib/fb_tools/pidfile.py:498
+#: lib/fb_tools/pidfile.py:495
 msgid "Process with PID {} anonymous died."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:502
+#: lib/fb_tools/pidfile.py:499
 msgid "No permission to signal the process {} ..."
 msgstr "No permission to signal the process {} …"
 
-#: lib/fb_tools/pidfile.py:506
+#: lib/fb_tools/pidfile.py:503
 msgid "Got a {c}: {e}."
 msgstr ""
 
-#: lib/fb_tools/xlate.py:107
+#: lib/fb_tools/xlate.py:106
 msgid "Module directory: {!r}"
 msgstr ""
 
-#: lib/fb_tools/xlate.py:108
+#: lib/fb_tools/xlate.py:107
 msgid "Base directory: {!r}"
 msgstr ""
 
-#: lib/fb_tools/xlate.py:109
+#: lib/fb_tools/xlate.py:108
 msgid "Locale directory: {!r}"
 msgstr ""
 
-#: lib/fb_tools/xlate.py:110
+#: lib/fb_tools/xlate.py:109
 msgid "Locale domain: {!r}"
 msgstr ""
 
-#: lib/fb_tools/xlate.py:111
+#: lib/fb_tools/xlate.py:110
 msgid "Found .mo-file: {!r}"
 msgstr ""
```

### Comparing `fb_tools-2.2.2/locale/fb_tools.pot` & `fb_tools-2.2.3/locale/fb_tools.pot`

 * *Files 1% similar despite different names*

```diff
@@ -1,176 +1,176 @@
 # Translations template for fb_tools.
-# Copyright (C) 2022 Frank Brehm, Berlin
+# Copyright (C) 2023 Frank Brehm, Berlin
 # This file is distributed under the same license as the fb_tools project.
-# Frank Brehm <frank.brehm@pixelpark.com>, 2022.
+# Frank Brehm <frank@brehm-online.com>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: fb_tools 2.1.2\n"
-"Report-Msgid-Bugs-To: frank.brehm@pixelpark.com\n"
-"POT-Creation-Date: 2022-11-21 14:24+0100\n"
+"Project-Id-Version: fb_tools 2.2.3\n"
+"Report-Msgid-Bugs-To: frank@brehm-online.com\n"
+"POT-Creation-Date: 2023-05-31 14:28+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <frank.brehm@pixelpark.com>\n"
+"Last-Translator: FULL NAME <frank@brehm-online.com>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 #: bin/get-file-to-remove:84
 msgid ""
 "{c}-Object:\n"
 "{a}"
 msgstr ""
 
-#: lib/fb_tools/app.py:69
+#: lib/fb_tools/app.py:64
 msgid "Forced execution - whatever it means."
 msgstr ""
 
-#: lib/fb_tools/app.py:151
+#: lib/fb_tools/app.py:146
 msgid "Invalid env_prefix {!r} given - it may not be empty."
 msgstr ""
 
-#: lib/fb_tools/app.py:155
+#: lib/fb_tools/app.py:150
 msgid ""
 "Invalid characters found in env_prefix {!r}, only alphanumeric characters and digits and "
 "underscore (this not as the first character) are allowed."
 msgstr ""
 
-#: lib/fb_tools/app.py:166
+#: lib/fb_tools/app.py:161
 msgid "Unknown and undescriped application."
 msgstr ""
 
-#: lib/fb_tools/app.py:191
+#: lib/fb_tools/app.py:186
 msgid "Wrong exit_value {!r}, must be >= 0."
 msgstr ""
 
-#: lib/fb_tools/app.py:428
+#: lib/fb_tools/app.py:423
 msgid "Trying to get {} via console ..."
 msgstr ""
 
-#: lib/fb_tools/app.py:444
+#: lib/fb_tools/app.py:439
 msgid "Got a signal {}."
 msgstr ""
 
-#: lib/fb_tools/app.py:447
+#: lib/fb_tools/app.py:442
 msgid "Got a signal {n!r} ({s})."
 msgstr ""
 
-#: lib/fb_tools/app.py:454
+#: lib/fb_tools/app.py:449
 msgid "Exit on signal {n!r} ({s})."
 msgstr ""
 
-#: lib/fb_tools/app.py:462
+#: lib/fb_tools/app.py:457
 msgid "Tweaking signal handlers."
 msgstr ""
 
-#: lib/fb_tools/app.py:468
+#: lib/fb_tools/app.py:463
 msgid "Setting signal handler for {n!r} ({s})."
 msgstr ""
 
-#: lib/fb_tools/app.py:479
+#: lib/fb_tools/app.py:474
 msgid "Enter "
 msgstr ""
 
-#: lib/fb_tools/app.py:486
+#: lib/fb_tools/app.py:481
 msgid "Repeat enter "
 msgstr ""
 
-#: lib/fb_tools/app.py:496
+#: lib/fb_tools/app.py:491
 msgid "{n} and repeated {n} did not match."
 msgstr ""
 
-#: lib/fb_tools/app.py:500
+#: lib/fb_tools/app.py:495
 msgid "Restoring original signal handlers."
 msgstr ""
 
-#: lib/fb_tools/app.py:505
+#: lib/fb_tools/app.py:500
 msgid "Got {n!r}: {s!r}"
 msgstr ""
 
-#: lib/fb_tools/app.py:555
+#: lib/fb_tools/app.py:550
 msgid "The application is not completely initialized."
 msgstr ""
 
-#: lib/fb_tools/app.py:566
+#: lib/fb_tools/app.py:561
 msgid "Object {!r} seems not to be completely initialized."
 msgstr ""
 
-#: lib/fb_tools/app.py:576
+#: lib/fb_tools/app.py:571
 msgid "Ending."
 msgstr ""
 
-#: lib/fb_tools/app.py:594
+#: lib/fb_tools/app.py:589
 msgid "Executing {} ..."
 msgstr ""
 
-#: lib/fb_tools/app.py:616
+#: lib/fb_tools/app.py:611
 msgid "General options"
 msgstr ""
 
-#: lib/fb_tools/app.py:621
+#: lib/fb_tools/app.py:616
 msgid "Simulation mode, nothing is really done."
 msgstr ""
 
-#: lib/fb_tools/app.py:635 lib/fb_tools/app.py:641
+#: lib/fb_tools/app.py:630 lib/fb_tools/app.py:636
 msgid "Automatically answer '{}' for all questions."
 msgstr ""
 
-#: lib/fb_tools/app.py:636 lib/fb_tools/handling_obj.py:941
+#: lib/fb_tools/app.py:631 lib/fb_tools/handling_obj.py:936
 msgid "Yes"
 msgstr ""
 
-#: lib/fb_tools/app.py:642 lib/fb_tools/handling_obj.py:939
+#: lib/fb_tools/app.py:637 lib/fb_tools/handling_obj.py:934
 msgid "No"
 msgstr ""
 
-#: lib/fb_tools/app.py:647 lib/fb_tools/ddns/__init__.py:249
+#: lib/fb_tools/app.py:642 lib/fb_tools/ddns/__init__.py:243
 msgid "SECONDS"
 msgstr ""
 
-#: lib/fb_tools/app.py:649
+#: lib/fb_tools/app.py:644
 msgid "The timeout in seconds for console input. Default: {}"
 msgstr ""
 
-#: lib/fb_tools/app.py:656
+#: lib/fb_tools/app.py:651
 msgid "Use colored output for messages."
 msgstr ""
 
-#: lib/fb_tools/app.py:663
+#: lib/fb_tools/app.py:658
 msgid "Increase the verbosity level"
 msgstr ""
 
-#: lib/fb_tools/app.py:668
+#: lib/fb_tools/app.py:663
 msgid "Silent execution, only warnings and errors are emitted."
 msgstr ""
 
-#: lib/fb_tools/app.py:673
+#: lib/fb_tools/app.py:668
 msgid "Show this help message and exit."
 msgstr ""
 
-#: lib/fb_tools/app.py:677
+#: lib/fb_tools/app.py:672
 msgid "Display brief usage message and exit."
 msgstr ""
 
-#: lib/fb_tools/app.py:679
+#: lib/fb_tools/app.py:674
 #, python-format
 msgid "Version of %(prog)s: {}"
 msgstr ""
 
-#: lib/fb_tools/app.py:682
+#: lib/fb_tools/app.py:677
 msgid "Show program's version number and exit."
 msgstr ""
 
-#: lib/fb_tools/app.py:812
+#: lib/fb_tools/app.py:807
 msgid "Starting in:"
 msgstr ""
 
-#: lib/fb_tools/app.py:834
+#: lib/fb_tools/app.py:829
 msgid "Aborted by user interrupt."
 msgstr ""
 
 #: lib/fb_tools/argparse_actions.py:58
 msgid "Got a {c} for pattern {p!r}: {e}"
 msgstr ""
 
@@ -190,109 +190,109 @@
 msgid "The given directory {!r} is not readable."
 msgstr ""
 
 #: lib/fb_tools/argparse_actions.py:102
 msgid "The given directory {!r} is not writeable."
 msgstr ""
 
-#: lib/fb_tools/argparse_actions.py:130 lib/fb_tools/cfg_app.py:228
+#: lib/fb_tools/argparse_actions.py:130 lib/fb_tools/cfg_app.py:219
 msgid "Directory {!r} does not exists."
 msgstr ""
 
-#: lib/fb_tools/argparse_actions.py:133 lib/fb_tools/cfg_app.py:232
+#: lib/fb_tools/argparse_actions.py:133 lib/fb_tools/cfg_app.py:223
 msgid "Path {!r} exists, but is not a directory."
 msgstr ""
 
 #: lib/fb_tools/argparse_actions.py:139 lib/fb_tools/argparse_actions.py:174
-#: lib/fb_tools/cfg_app.py:239 lib/fb_tools/get_file_rm_app.py:399
+#: lib/fb_tools/cfg_app.py:230 lib/fb_tools/get_file_rm_app.py:395
 msgid "File {!r} is not a regular file."
 msgstr ""
 
-#: lib/fb_tools/argparse_actions.py:142 lib/fb_tools/cfg_app.py:243
+#: lib/fb_tools/argparse_actions.py:142 lib/fb_tools/cfg_app.py:234
 msgid "File {!r} is not writeable."
 msgstr ""
 
-#: lib/fb_tools/argparse_actions.py:146 lib/fb_tools/cfg_app.py:248
+#: lib/fb_tools/argparse_actions.py:146 lib/fb_tools/cfg_app.py:239
 msgid "Directory {!r} is not writeable."
 msgstr ""
 
-#: lib/fb_tools/argparse_actions.py:171 lib/fb_tools/get_file_rm_app.py:390
+#: lib/fb_tools/argparse_actions.py:171 lib/fb_tools/get_file_rm_app.py:386
 msgid "File {!r} does not exists."
 msgstr ""
 
-#: lib/fb_tools/argparse_actions.py:197 lib/fb_tools/multi_config.py:1155
+#: lib/fb_tools/argparse_actions.py:197 lib/fb_tools/multi_config.py:1147
 msgid "A timeout must be greater than zero and less or equal to {}."
 msgstr ""
 
 #: lib/fb_tools/argparse_actions.py:202
 msgid "Wrong timeout {!r}:"
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:64
+#: lib/fb_tools/cfg_app.py:55
 msgid "Parameter {cls!r} must be a subclass of {clinfo!r}."
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:146
+#: lib/fb_tools/cfg_app.py:137
 msgid "Config options and options for logging"
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:151 lib/fb_tools/cfg_app.py:157 lib/fb_tools/ddns/__init__.py:255
-#: lib/fb_tools/get_file_rm_app.py:270
+#: lib/fb_tools/cfg_app.py:142 lib/fb_tools/cfg_app.py:148 lib/fb_tools/ddns/__init__.py:249
+#: lib/fb_tools/get_file_rm_app.py:266
 msgid "FILE"
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:152
+#: lib/fb_tools/cfg_app.py:143
 msgid "Configuration files to use additional to the standard configuration files."
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:158
+#: lib/fb_tools/cfg_app.py:149
 msgid "A logfile for storing all logging output."
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:165
+#: lib/fb_tools/cfg_app.py:156
 msgid "Got command line arguments:"
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:203
+#: lib/fb_tools/cfg_app.py:194
 msgid "Error on reading configuration:"
 msgstr ""
 
-#: lib/fb_tools/cfg_app.py:252
+#: lib/fb_tools/cfg_app.py:243
 msgid "Start logging into file {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/collections.py:63
+#: lib/fb_tools/collections.py:60
 msgid "Item {item!r} must be of type {must!r}, but is of type {cls!r} instead."
 msgstr ""
 
-#: lib/fb_tools/collections.py:81
+#: lib/fb_tools/collections.py:78
 msgid "Object {o!r} is not a {e} object."
 msgstr ""
 
-#: lib/fb_tools/collections.py:99
+#: lib/fb_tools/collections.py:96
 msgid "Key {key!r} must be of type {must!r}, but is of type {cls!r} instead."
 msgstr ""
 
-#: lib/fb_tools/collections.py:116
+#: lib/fb_tools/collections.py:113
 msgid "Object is neither a {m} object, nor a sequential object, but a {o!r} object instead."
 msgstr ""
 
-#: lib/fb_tools/collections.py:135
+#: lib/fb_tools/collections.py:132
 msgid "Key {!r} is not existing."
 msgstr ""
 
-#: lib/fb_tools/collections.py:154 lib/fb_tools/collections.py:173
+#: lib/fb_tools/collections.py:151 lib/fb_tools/collections.py:170
 msgid "Could update {ex} with {i!r}: {m}"
 msgstr ""
 
-#: lib/fb_tools/collections.py:197
+#: lib/fb_tools/collections.py:194
 msgid "Parameter {p!r} is not a sequence type, but a {c!r} object instead."
 msgstr ""
 
-#: lib/fb_tools/collections.py:1008
+#: lib/fb_tools/collections.py:1005
 msgid "The method {met}() expected at most {max} arguments, got {got}."
 msgstr ""
 
 #: lib/fb_tools/common.py:154
 msgid "{} is a tty."
 msgstr ""
 
@@ -316,325 +316,325 @@
 msgid "Couldn't detect unit {!r}."
 msgstr ""
 
 #: lib/fb_tools/common.py:783
 msgid "Argument {a!r} must be of type {t1!r} or {t2!r}."
 msgstr ""
 
-#: lib/fb_tools/config.py:101 lib/fb_tools/multi_config.py:245
+#: lib/fb_tools/config.py:96 lib/fb_tools/multi_config.py:237
 msgid "Encoding {v!r} must be a {s!r} object, but is a {c!r} object instead."
 msgstr ""
 
-#: lib/fb_tools/config.py:119 lib/fb_tools/multi_config.py:303
+#: lib/fb_tools/config.py:114 lib/fb_tools/multi_config.py:295
 msgid "A configuration directory may not be None."
 msgstr ""
 
-#: lib/fb_tools/config.py:135
+#: lib/fb_tools/config.py:130
 msgid "A configuration file may not be None."
 msgstr ""
 
-#: lib/fb_tools/config.py:140 lib/fb_tools/config.py:148 lib/fb_tools/multi_config.py:275
+#: lib/fb_tools/config.py:135 lib/fb_tools/config.py:143 lib/fb_tools/multi_config.py:267
 msgid "Configuration file {!r} exists, but is not a regular file."
 msgstr ""
 
-#: lib/fb_tools/config.py:178
+#: lib/fb_tools/config.py:173
 msgid "Searching for {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/config.py:180
+#: lib/fb_tools/config.py:175
 msgid "Configuration file {!r} not found."
 msgstr ""
 
-#: lib/fb_tools/config.py:182
+#: lib/fb_tools/config.py:177
 msgid "Configuration file error"
 msgstr ""
 
-#: lib/fb_tools/config.py:193
+#: lib/fb_tools/config.py:188
 msgid "Reading {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/config.py:204
+#: lib/fb_tools/config.py:199
 msgid "Wrong configuration in {!r} found"
 msgstr ""
 
-#: lib/fb_tools/config.py:206
+#: lib/fb_tools/config.py:201
 msgid "Configuration parse error"
 msgstr ""
 
-#: lib/fb_tools/config.py:229 lib/fb_tools/multi_config.py:1124
+#: lib/fb_tools/config.py:224 lib/fb_tools/multi_config.py:1116
 msgid "Checking config section {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:74
+#: lib/fb_tools/ddns/__init__.py:68
 msgid "Got an error {c} on requesting {u!r}: {m}"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:93
+#: lib/fb_tools/ddns/__init__.py:87
 msgid "Directory does not exists"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:104
+#: lib/fb_tools/ddns/__init__.py:98
 msgid "Path is not a directory"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:115
+#: lib/fb_tools/ddns/__init__.py:109
 msgid "Invalid permissions"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:134
+#: lib/fb_tools/ddns/__init__.py:128
 msgid "This is a base DDNS related application."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:170
+#: lib/fb_tools/ddns/__init__.py:164
 msgid "Invalid user agent {!r} given."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:196
+#: lib/fb_tools/ddns/__init__.py:190
 msgid "DDNS options"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:210 lib/fb_tools/ddns/__init__.py:213
+#: lib/fb_tools/ddns/__init__.py:204 lib/fb_tools/ddns/__init__.py:207
 msgid "Perform action only for {}."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:216
+#: lib/fb_tools/ddns/__init__.py:210
 msgid "The IP protocol, for which the action should be performed (one of {c}, default {d!r})."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:230
+#: lib/fb_tools/ddns/__init__.py:224
 msgid "PROTOCOL"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:240
+#: lib/fb_tools/ddns/__init__.py:234
 msgid "DIRECTORY"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:242
+#: lib/fb_tools/ddns/__init__.py:236
 msgid ""
 "The directory, where to read and write the cache files of the evaluated IP addresses (default: "
 "{!r})."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:250
+#: lib/fb_tools/ddns/__init__.py:244
 msgid "The timeout in seconds for Web requests (default: {})."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:257
+#: lib/fb_tools/ddns/__init__.py:251
 msgid "Configuration file (default: {!r})"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:310 lib/fb_tools/ddns/config.py:210
+#: lib/fb_tools/ddns/__init__.py:304 lib/fb_tools/ddns/config.py:207
 msgid "Invalid value {!r} as timeout:"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:320
+#: lib/fb_tools/ddns/__init__.py:314
 msgid "Setting Loglevel of the {m} module to {ll}."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:331
+#: lib/fb_tools/ddns/__init__.py:325
 msgid "Trying to get my public IPv{} address."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:343
+#: lib/fb_tools/ddns/__init__.py:337
 msgid "Got a response:"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:354
+#: lib/fb_tools/ddns/__init__.py:348
 msgid "Request method: {!r}"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:374
+#: lib/fb_tools/ddns/__init__.py:368
 msgid "Simulation mode, Request will not be sent."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:387
+#: lib/fb_tools/ddns/__init__.py:381
 msgid "Got a {c} on requesting {u!r}: {e}."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:394
+#: lib/fb_tools/ddns/__init__.py:388
 msgid "Failed to parse the response"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:422
+#: lib/fb_tools/ddns/__init__.py:423
 msgid "Checking existence and accessibility of working directory {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:434 lib/fb_tools/ddns/update_app.py:169
+#: lib/fb_tools/ddns/__init__.py:435 lib/fb_tools/ddns/update_app.py:165
 msgid "No read access"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:438 lib/fb_tools/ddns/update_app.py:172
+#: lib/fb_tools/ddns/__init__.py:439 lib/fb_tools/ddns/update_app.py:168
 msgid "No write access"
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:453
+#: lib/fb_tools/ddns/__init__.py:454
 msgid "Writing IP address {a!r} into {f!r} ..."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:481
+#: lib/fb_tools/ddns/__init__.py:482
 msgid "File {!r} not found."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:484
+#: lib/fb_tools/ddns/__init__.py:485
 msgid "Reading IP address from {!r}..."
 msgstr ""
 
-#: lib/fb_tools/ddns/__init__.py:504
+#: lib/fb_tools/ddns/__init__.py:505
 msgid "Line {li!r} in {f!r} is not a valid IP address:"
 msgstr ""
 
-#: lib/fb_tools/ddns/config.py:104
+#: lib/fb_tools/ddns/config.py:101
 msgid "Invalid timeout {!r} for Web requests, must be 0 < SECONDS < 3600."
 msgstr ""
 
-#: lib/fb_tools/ddns/config.py:224
+#: lib/fb_tools/ddns/config.py:221
 msgid "Invalid value {ur} for protocols to update, valid protocols are: "
 msgstr ""
 
-#: lib/fb_tools/ddns/config.py:233 lib/fb_tools/ddns/config.py:270
+#: lib/fb_tools/ddns/config.py:230 lib/fb_tools/ddns/config.py:267
 msgid "Unknown configuration option {o!r} with value {v!r} in section {s!r}."
 msgstr ""
 
-#: lib/fb_tools/ddns/config.py:255
+#: lib/fb_tools/ddns/config.py:252
 msgid "The path to the working directory must be an absolute path (given: {!r})."
 msgstr ""
 
-#: lib/fb_tools/ddns/config.py:265
+#: lib/fb_tools/ddns/config.py:262
 msgid "The path to the logfile must be an absolute path (given: {!r})."
 msgstr ""
 
-#: lib/fb_tools/ddns/myip_app.py:50
+#: lib/fb_tools/ddns/myip_app.py:46
 msgid ""
 "Tries to detect the public NAT IPv4 address and/or the automatic assigned IPv6 address in a "
 "local network and print it out."
 msgstr ""
 
-#: lib/fb_tools/ddns/myip_app.py:55 lib/fb_tools/ddns/myip_app.py:56
+#: lib/fb_tools/ddns/myip_app.py:51 lib/fb_tools/ddns/myip_app.py:52
 msgid "Use only {} to retreive the public IP address."
 msgstr ""
 
-#: lib/fb_tools/ddns/myip_app.py:57
+#: lib/fb_tools/ddns/myip_app.py:53
 msgid "The IP protocol, for which the public IP should be retrieved (one of {c}, default {d!r})."
 msgstr ""
 
-#: lib/fb_tools/ddns/myip_app.py:99
+#: lib/fb_tools/ddns/myip_app.py:95
 msgid "myip options"
 msgstr ""
 
-#: lib/fb_tools/ddns/myip_app.py:103
+#: lib/fb_tools/ddns/myip_app.py:99
 msgid "Write found public IPs into a cache file in working directory."
 msgstr ""
 
-#: lib/fb_tools/ddns/myip_app.py:134 lib/fb_tools/ddns/update_app.py:275
+#: lib/fb_tools/ddns/myip_app.py:130 lib/fb_tools/ddns/update_app.py:271
 msgid "Starting {a!r}, version {v!r} ..."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:66
+#: lib/fb_tools/ddns/update_app.py:62
 msgid "Updating the DDNS records, even if seems not to be changed."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:69
+#: lib/fb_tools/ddns/update_app.py:65
 msgid "Tries to update the A and/or AAAA record at ddns.de with the current IP address."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:74 lib/fb_tools/ddns/update_app.py:75
+#: lib/fb_tools/ddns/update_app.py:70 lib/fb_tools/ddns/update_app.py:71
 msgid "Update only the {} record with the public IP address."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:76
+#: lib/fb_tools/ddns/update_app.py:72
 msgid ""
 "The IP protocol, for which the appropriate DNS record should be updated with the public IP (one "
 "of {c}, default {d!r})."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:158
+#: lib/fb_tools/ddns/update_app.py:154
 msgid "Checking existence and accessibility of log directory {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:190
+#: lib/fb_tools/ddns/update_app.py:186
 msgid "Update DDNS options"
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:193
+#: lib/fb_tools/ddns/update_app.py:189
 msgid "USER"
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:194
+#: lib/fb_tools/ddns/update_app.py:190
 msgid "The username to login at ddns.de."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:198
+#: lib/fb_tools/ddns/update_app.py:194
 msgid "PASSWORD"
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:199
+#: lib/fb_tools/ddns/update_app.py:195
 msgid "The password of the user to login at ddns.de."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:203
+#: lib/fb_tools/ddns/update_app.py:199
 msgid "FILENAME"
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:204
+#: lib/fb_tools/ddns/update_app.py:200
 msgid "The filename to use as a logfile. Leave it empty to disable file logging."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:211
+#: lib/fb_tools/ddns/update_app.py:207
 msgid "Update all domains, which are connected whith the given ddns account."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:215
+#: lib/fb_tools/ddns/update_app.py:211
 msgid "DOMAIN"
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:216
+#: lib/fb_tools/ddns/update_app.py:212
 msgid "The particular domain(s), which should be updated (if not all)."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:234
+#: lib/fb_tools/ddns/update_app.py:230
 msgid "No domains to update given, but the option all domains is deactivated."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:284
+#: lib/fb_tools/ddns/update_app.py:280
 msgid "Ending {a!r}."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:292 lib/fb_tools/ddns/update_app.py:330
+#: lib/fb_tools/ddns/update_app.py:288 lib/fb_tools/ddns/update_app.py:326
 msgid "Last {w} address: {a!r}."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:294 lib/fb_tools/ddns/update_app.py:332
+#: lib/fb_tools/ddns/update_app.py:290 lib/fb_tools/ddns/update_app.py:328
 msgid "Did not found a last {} address."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:297
+#: lib/fb_tools/ddns/update_app.py:293
 msgid "Got no public IPv4 address."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:302 lib/fb_tools/ddns/update_app.py:340
+#: lib/fb_tools/ddns/update_app.py:298 lib/fb_tools/ddns/update_app.py:336
 msgid "Address {a!r} seems not to be a valid {w} address: {e}"
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:307 lib/fb_tools/ddns/update_app.py:345
+#: lib/fb_tools/ddns/update_app.py:303 lib/fb_tools/ddns/update_app.py:341
 msgid "Address {a!r} seems not to be a valid {w} address."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:312 lib/fb_tools/ddns/update_app.py:350
+#: lib/fb_tools/ddns/update_app.py:308 lib/fb_tools/ddns/update_app.py:346
 msgid "Current {w} address is {a!r}."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:315 lib/fb_tools/ddns/update_app.py:353
+#: lib/fb_tools/ddns/update_app.py:311 lib/fb_tools/ddns/update_app.py:349
 msgid "The public {w} address {a!r} seems not to be changed since the last update."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:335
+#: lib/fb_tools/ddns/update_app.py:331
 msgid "Got no public IPv6 address."
 msgstr ""
 
-#: lib/fb_tools/ddns/update_app.py:366
+#: lib/fb_tools/ddns/update_app.py:362
 msgid "Updating DNS records to IPv{p} address {a!r} ..."
 msgstr ""
 
 #: lib/fb_tools/errors.py:51
 msgid "Empty mail address."
 msgstr ""
 
@@ -684,969 +684,969 @@
 msgstr[0] ""
 msgstr[1] ""
 
 #: lib/fb_tools/errors.py:362
 msgid "Couldn't occupy lockfile {lf!r} in {d:0.1f} seconds with {tries} tries."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:66
+#: lib/fb_tools/get_file_rm_app.py:62
 msgid "Value must be at least {m} - {v} was given."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:108
+#: lib/fb_tools/get_file_rm_app.py:104
 msgid "The given pattern {!r} is not a valid date pattern"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:112
+#: lib/fb_tools/get_file_rm_app.py:108
 #, python-format
 msgid ". The must be exactly one occurence of '%Y', one of '%m' and one of '%d'."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:143
+#: lib/fb_tools/get_file_rm_app.py:139
 msgid ""
 "Returns a newline separated list of files generated from file globbing patterns given as "
 "arguments to this application, where all files are omitted, which should not be removed."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:182 lib/fb_tools/get_file_rm_app.py:198
-#: lib/fb_tools/get_file_rm_app.py:214 lib/fb_tools/get_file_rm_app.py:230
-#: lib/fb_tools/get_file_rm_app.py:246
+#: lib/fb_tools/get_file_rm_app.py:178 lib/fb_tools/get_file_rm_app.py:194
+#: lib/fb_tools/get_file_rm_app.py:210 lib/fb_tools/get_file_rm_app.py:226
+#: lib/fb_tools/get_file_rm_app.py:242
 msgid "Wrong value {v!r} for {n}, must be >= {m}"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:267
+#: lib/fb_tools/get_file_rm_app.py:263
 msgid "File options"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:271
+#: lib/fb_tools/get_file_rm_app.py:267
 msgid "File pattern to generate list of files to remove."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:274
+#: lib/fb_tools/get_file_rm_app.py:270
 msgid "Keep options"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:277
+#: lib/fb_tools/get_file_rm_app.py:273
 msgid "NR_FILES"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:279
+#: lib/fb_tools/get_file_rm_app.py:275
 msgid "How many of the last files should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:286
+#: lib/fb_tools/get_file_rm_app.py:282
 msgid "DAYS"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:288
+#: lib/fb_tools/get_file_rm_app.py:284
 msgid "How many files one per day from today on should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:295
+#: lib/fb_tools/get_file_rm_app.py:291
 msgid "WEEKS"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:297
+#: lib/fb_tools/get_file_rm_app.py:293
 msgid "How many files one per week from today on should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:304
+#: lib/fb_tools/get_file_rm_app.py:300
 msgid "MONTHS"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:306
+#: lib/fb_tools/get_file_rm_app.py:302
 msgid "How many files one per month from today on should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:313
+#: lib/fb_tools/get_file_rm_app.py:309
 msgid "YEARS"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:315
+#: lib/fb_tools/get_file_rm_app.py:311
 msgid "How many files one per year from today on should be kept (default: {default}, minimum: {min})?"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:346
+#: lib/fb_tools/get_file_rm_app.py:342
 msgid "Resolving date pattern {!r}."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:367
+#: lib/fb_tools/get_file_rm_app.py:363
 msgid "Checking given files..."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:372
+#: lib/fb_tools/get_file_rm_app.py:368
 msgid "Checking given file {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:381
+#: lib/fb_tools/get_file_rm_app.py:377
 msgid "Resolved paths:"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:383
+#: lib/fb_tools/get_file_rm_app.py:379
 msgid "File pattern {!r} does not match any files."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:388
+#: lib/fb_tools/get_file_rm_app.py:384
 msgid "Checking {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:394
+#: lib/fb_tools/get_file_rm_app.py:390
 msgid "File {!r} is a regular file."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:397
+#: lib/fb_tools/get_file_rm_app.py:393
 msgid "Path {!r} is a directory."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:404
+#: lib/fb_tools/get_file_rm_app.py:400
 msgid "File {fi!r} does not match pattern {pa!r}."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:414
+#: lib/fb_tools/get_file_rm_app.py:410
 msgid "Date in file {fi!r} is not a valid date: {e}."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:465
+#: lib/fb_tools/get_file_rm_app.py:461
 msgid "Did not found any files to evaluate."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:497
+#: lib/fb_tools/get_file_rm_app.py:493
 msgid "Keeping last file ..."
 msgid_plural "Keeping last {} files ..."
 msgstr[0] ""
 msgstr[1] ""
 
-#: lib/fb_tools/get_file_rm_app.py:503
+#: lib/fb_tools/get_file_rm_app.py:499
 msgid "Keep last file {!r}."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:508
+#: lib/fb_tools/get_file_rm_app.py:504
 msgid "Files to keep:"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:529
+#: lib/fb_tools/get_file_rm_app.py:525
 msgid "Files to keep for year:"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:551
+#: lib/fb_tools/get_file_rm_app.py:547
 msgid "Got last month: {!r}"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:565
+#: lib/fb_tools/get_file_rm_app.py:561
 msgid "Files to keep for month:"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:579
+#: lib/fb_tools/get_file_rm_app.py:575
 msgid "Got last Monday: {!r}"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:592
+#: lib/fb_tools/get_file_rm_app.py:588
 msgid "Files to keep for week:"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:605
+#: lib/fb_tools/get_file_rm_app.py:601
 msgid "Got last day: {!r}"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:616
+#: lib/fb_tools/get_file_rm_app.py:612
 msgid "Keeping all files from today."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:623
+#: lib/fb_tools/get_file_rm_app.py:619
 msgid "Files to keep for day:"
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:640
+#: lib/fb_tools/get_file_rm_app.py:636
 msgid "Trying to get date of file {!r}."
 msgstr ""
 
-#: lib/fb_tools/get_file_rm_app.py:679
+#: lib/fb_tools/get_file_rm_app.py:675
 msgid "Explored and assigned files:"
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:159
+#: lib/fb_tools/handler/__init__.py:155
 msgid "Invalid time zone name {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:161
+#: lib/fb_tools/handler/__init__.py:157
 msgid "Setting time zone to {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:165
+#: lib/fb_tools/handler/__init__.py:161
 msgid "Name of the time zone: {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:171
+#: lib/fb_tools/handler/__init__.py:167
 msgid "{}-object not initialized."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:173
+#: lib/fb_tools/handler/__init__.py:169
 msgid "Method {} must be overridden in descendant classes."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:250
+#: lib/fb_tools/handler/__init__.py:246
 msgid "Quiet execution."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:298
+#: lib/fb_tools/handler/__init__.py:294
 msgid "Starting synchronous communication with '{}'."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:302
+#: lib/fb_tools/handler/__init__.py:298
 msgid "Finished communication with '{}'."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:316
+#: lib/fb_tools/handler/__init__.py:312
 msgid "Parameter {p!r} is not of type {t!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:321
+#: lib/fb_tools/handler/__init__.py:317
 msgid "Got completed process:"
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:325 lib/fb_tools/handler/__init__.py:336
+#: lib/fb_tools/handler/__init__.py:321 lib/fb_tools/handler/__init__.py:332
 msgid "Output on {}:"
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:357
+#: lib/fb_tools/handler/__init__.py:353
 msgid "Starting asynchronous communication with '{cmd}', heartbeat interval is {interval:0.1f} seconds."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:372
+#: lib/fb_tools/handler/__init__.py:368
 msgid "Checking for the end of the communication ..."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:382
+#: lib/fb_tools/handler/__init__.py:378
 msgid "Time to execute the heartbeat handler."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:386
+#: lib/fb_tools/handler/__init__.py:382
 msgid "Sleeping {:0.2f} seconds ..."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:394 lib/fb_tools/handler/__init__.py:403
+#: lib/fb_tools/handler/__init__.py:390 lib/fb_tools/handler/__init__.py:399
 msgid "   {w} is now: {o!r}"
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:101
+#: lib/fb_tools/handler/lock.py:99
 msgid "Locking directory {!r} doesn't exists or is not a directory."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:128 lib/fb_tools/handler/lock.py:807
+#: lib/fb_tools/handler/lock.py:126 lib/fb_tools/handler/lock.py:805
 msgid "Locking directory {!r} isn't writeable."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:193
+#: lib/fb_tools/handler/lock.py:191
 msgid "No lockfile given on init of a LockObject object."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:199
+#: lib/fb_tools/handler/lock.py:197
 msgid "Lockfile {!r} doesn't exists, but don't worry, it's simulation mode."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:203 lib/fb_tools/handler/lock.py:1045
+#: lib/fb_tools/handler/lock.py:201 lib/fb_tools/handler/lock.py:1043
 msgid "Lockfile {!r} doesn't exists."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:206
+#: lib/fb_tools/handler/lock.py:204
 msgid "Lockfile {!r} is not a regular file."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:360
+#: lib/fb_tools/handler/lock.py:358
 msgid "Closing file descriptor {} ..."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:371
+#: lib/fb_tools/handler/lock.py:369
 msgid "Automatic removing of {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:399
+#: lib/fb_tools/handler/lock.py:397
 msgid "Refreshing atime and mtime of {!r} to the current timestamp."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:533 lib/fb_tools/handler/lock.py:553 lib/fb_tools/handler/lock.py:573
-#: lib/fb_tools/handler/lock.py:597 lib/fb_tools/handler/lock.py:692 lib/fb_tools/handler/lock.py:1034
+#: lib/fb_tools/handler/lock.py:531 lib/fb_tools/handler/lock.py:551 lib/fb_tools/handler/lock.py:571
+#: lib/fb_tools/handler/lock.py:595 lib/fb_tools/handler/lock.py:690 lib/fb_tools/handler/lock.py:1032
 msgid "Value {val!r} for {what} is not a Number."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:538 lib/fb_tools/handler/lock.py:558 lib/fb_tools/handler/lock.py:578
-#: lib/fb_tools/handler/lock.py:602 lib/fb_tools/handler/lock.py:697 lib/fb_tools/handler/lock.py:1038
+#: lib/fb_tools/handler/lock.py:536 lib/fb_tools/handler/lock.py:556 lib/fb_tools/handler/lock.py:576
+#: lib/fb_tools/handler/lock.py:600 lib/fb_tools/handler/lock.py:695 lib/fb_tools/handler/lock.py:1036
 msgid "The value for {what} must be greater than zero (is {val!r})."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:702
+#: lib/fb_tools/handler/lock.py:700
 msgid "The value for {what} must be greater than or equal to zero (is {val!r})."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:787
+#: lib/fb_tools/handler/lock.py:785
 msgid "Invalid PID {} given on calling create_lockfile()."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:796
+#: lib/fb_tools/handler/lock.py:794
 msgid "Using lock directory {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:804
+#: lib/fb_tools/handler/lock.py:802
 msgid "Trying to lock lockfile {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:845
+#: lib/fb_tools/handler/lock.py:843
 msgid "Current time difference: {:0.3f} seconds."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:850
+#: lib/fb_tools/handler/lock.py:848
 msgid "Try {try_nr} on creating lockfile {lfile!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:861 lib/fb_tools/handler/lock.py:980
+#: lib/fb_tools/handler/lock.py:859 lib/fb_tools/handler/lock.py:978
 msgid "Removing lockfile {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:866 lib/fb_tools/handler/lock.py:988
+#: lib/fb_tools/handler/lock.py:864 lib/fb_tools/handler/lock.py:986
 msgid "Error on removing lockfile {lfile!r}: {err}"
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:879
+#: lib/fb_tools/handler/lock.py:877
 msgid "Sleeping for {:0.1f} seconds."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:894
+#: lib/fb_tools/handler/lock.py:892
 msgid "Got a lock for lockfile {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:900
+#: lib/fb_tools/handler/lock.py:898
 msgid "Write {what!r} in lockfile {lfile!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:909
+#: lib/fb_tools/handler/lock.py:907
 msgid "Seeking and syncing {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:938
+#: lib/fb_tools/handler/lock.py:936
 msgid "Trying to open {!r} exclusive ..."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:940
+#: lib/fb_tools/handler/lock.py:938
 msgid "Simulation mode, no real creation of a lockfile."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:948
+#: lib/fb_tools/handler/lock.py:946
 msgid "Error on creating lockfile {lfile!r}: {err}"
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:977
+#: lib/fb_tools/handler/lock.py:975
 msgid "Lockfile {!r} to remove doesn't exists."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:982
+#: lib/fb_tools/handler/lock.py:980
 msgid "Simulation mode - lockfile won't removed."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1042
+#: lib/fb_tools/handler/lock.py:1040
 msgid "Checking lockfile {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1049
+#: lib/fb_tools/handler/lock.py:1047
 msgid "No read access for lockfile {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1053
+#: lib/fb_tools/handler/lock.py:1051
 msgid "No write access for lockfile {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1059
+#: lib/fb_tools/handler/lock.py:1057
 msgid "Unusable lockfile {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1062
+#: lib/fb_tools/handler/lock.py:1060
 msgid "Process with PID {} is unfortunately dead."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1065
+#: lib/fb_tools/handler/lock.py:1063
 msgid "Process with PID {} is still running."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1073
+#: lib/fb_tools/handler/lock.py:1071
 msgid "Could not stat for file {lfile!r}: {err}"
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1080
+#: lib/fb_tools/handler/lock.py:1078
 msgid "Lockfile {lfile!r} is older than {max} seconds ({age} seconds)."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1083
+#: lib/fb_tools/handler/lock.py:1081
 msgid "Lockfile {lfile!r} is {age} seconds old, but not old enough ({max} seconds)."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1110
+#: lib/fb_tools/handler/lock.py:1108
 msgid "Trying to open pidfile {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1114
+#: lib/fb_tools/handler/lock.py:1112
 msgid "Could not open pidfile {!r} for reading:"
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1127
+#: lib/fb_tools/handler/lock.py:1125
 msgid "First line of pidfile {!r} was empty."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1138
+#: lib/fb_tools/handler/lock.py:1136
 msgid "Could not interprete {cont!r} as a PID from {file!r}: {err}"
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:1147
+#: lib/fb_tools/handler/lock.py:1145
 msgid "Invalid PID {pid} in {file!r} found."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:78
+#: lib/fb_tools/handling_obj.py:73
 msgid "Timeout on communicating with process."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:104
+#: lib/fb_tools/handling_obj.py:99
 msgid "Command {c!r} returned non-zero exit status {rc}."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:142
+#: lib/fb_tools/handling_obj.py:137
 msgid "Command {c!r} timed out after {s} second."
 msgid_plural "Command {c!r} timed out after {s} seconds."
 msgstr[0] ""
 msgstr[1] ""
 
-#: lib/fb_tools/handling_obj.py:303
+#: lib/fb_tools/handling_obj.py:298
 msgid "Wrong prompt timeout {v!r}, must be greater or equal to Null and less or equal to {max}."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:314
+#: lib/fb_tools/handling_obj.py:309
 msgid "yes"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:321
+#: lib/fb_tools/handling_obj.py:316
 msgid "no"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:389
+#: lib/fb_tools/handling_obj.py:384
 msgid "Searching for command {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:394
+#: lib/fb_tools/handling_obj.py:389
 msgid "Command {!r} doesn't exists."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:397 lib/fb_tools/handling_obj.py:421
+#: lib/fb_tools/handling_obj.py:392 lib/fb_tools/handling_obj.py:416
 msgid "Command {!r} is not executable."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:411
+#: lib/fb_tools/handling_obj.py:406
 msgid "Searching command in {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:424
+#: lib/fb_tools/handling_obj.py:419
 msgid "Command {!r} not found."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:496
+#: lib/fb_tools/handling_obj.py:491
 msgid "STDIN and input arguments may not both be used."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:499
+#: lib/fb_tools/handling_obj.py:494
 msgid "Executing command args:"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:502
+#: lib/fb_tools/handling_obj.py:497
 msgid "Performing argument {!r}."
 msgstr ""
 
-#: lib/fb_tools/handler/__init__.py:247 lib/fb_tools/handling_obj.py:507
+#: lib/fb_tools/handler/__init__.py:243 lib/fb_tools/handling_obj.py:502
 msgid "Executing: {}"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:510
+#: lib/fb_tools/handling_obj.py:505
 msgid "Simulation mode, not executing: {}"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:518
+#: lib/fb_tools/handling_obj.py:513
 msgid "PID of process: {}"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:524
+#: lib/fb_tools/handling_obj.py:519
 msgid "{c} happened, killing process: {e}"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:626
+#: lib/fb_tools/handling_obj.py:621
 msgid "Nothing to do on signal."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:680 lib/fb_tools/handling_obj.py:769
+#: lib/fb_tools/handling_obj.py:675 lib/fb_tools/handling_obj.py:764
 msgid "File doesn't exists."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:683
+#: lib/fb_tools/handling_obj.py:678
 msgid "Read permission denied."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:686
+#: lib/fb_tools/handling_obj.py:681
 msgid "Reading file content of {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:774 lib/fb_tools/handling_obj.py:781
+#: lib/fb_tools/handling_obj.py:769 lib/fb_tools/handling_obj.py:776
 msgid "Write permission to {!r} denied."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:776 lib/fb_tools/handling_obj.py:783
+#: lib/fb_tools/handling_obj.py:771 lib/fb_tools/handling_obj.py:778
 msgid "Write permission denied."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:787
+#: lib/fb_tools/handling_obj.py:782
 msgid "Write {what!r} into {to!r}."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:789
+#: lib/fb_tools/handling_obj.py:784
 msgid "Writing {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:801
+#: lib/fb_tools/handling_obj.py:796
 msgid "Simulating write into {!r}."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:809
+#: lib/fb_tools/handling_obj.py:804
 msgid "Opening {!r} for write unbuffered ..."
 msgstr ""
 
-#: lib/fb_tools/handler/lock.py:913 lib/fb_tools/handling_obj.py:813
+#: lib/fb_tools/handler/lock.py:911 lib/fb_tools/handling_obj.py:808
 msgid "Closing {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:844
+#: lib/fb_tools/handling_obj.py:839
 msgid "Password:"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:847
+#: lib/fb_tools/handling_obj.py:842
 msgid "Repeat password:"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:861
+#: lib/fb_tools/handling_obj.py:856
 msgid "The entered passwords does not match."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:874 lib/fb_tools/handling_obj.py:949
+#: lib/fb_tools/handling_obj.py:869 lib/fb_tools/handling_obj.py:944
 msgid "Interrupted on demand."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:899 lib/fb_tools/handling_obj.py:904 lib/fb_tools/handling_obj.py:983
-#: lib/fb_tools/handling_obj.py:988
+#: lib/fb_tools/handling_obj.py:894 lib/fb_tools/handling_obj.py:899 lib/fb_tools/handling_obj.py:978
+#: lib/fb_tools/handling_obj.py:983
 msgid "Got a {}:"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:934
+#: lib/fb_tools/handling_obj.py:929
 msgid "Yes/No"
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:942
+#: lib/fb_tools/handling_obj.py:937
 msgid "Automatic answer: '{}'."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:1031 lib/fb_tools/handling_obj.py:1037
+#: lib/fb_tools/handling_obj.py:1026 lib/fb_tools/handling_obj.py:1032
 msgid "Parameter {t!r} must be a {e}, {v!r} was given."
 msgstr ""
 
-#: lib/fb_tools/handling_obj.py:1100
+#: lib/fb_tools/handling_obj.py:1095
 msgid "Completed process"
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:69 lib/fb_tools/mailaddress.py:468
+#: lib/fb_tools/mailaddress.py:65 lib/fb_tools/mailaddress.py:464
 msgid "Empty address."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:78 lib/fb_tools/mailaddress.py:477
+#: lib/fb_tools/mailaddress.py:74 lib/fb_tools/mailaddress.py:473
 msgid "Wrong type."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:88 lib/fb_tools/mailaddress.py:495 lib/fb_tools/mailaddress.py:535
-#: lib/fb_tools/mailaddress.py:558
+#: lib/fb_tools/mailaddress.py:84 lib/fb_tools/mailaddress.py:491 lib/fb_tools/mailaddress.py:531
+#: lib/fb_tools/mailaddress.py:554
 msgid "Invalid address."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:106 lib/fb_tools/mailaddress.py:167
+#: lib/fb_tools/mailaddress.py:102 lib/fb_tools/mailaddress.py:163
 msgid "Given user: {u!r}, given domain: {d!r}."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:111
+#: lib/fb_tools/mailaddress.py:107
 msgid "Invalid mail address."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:128 lib/fb_tools/mailaddress.py:143
+#: lib/fb_tools/mailaddress.py:124 lib/fb_tools/mailaddress.py:139
 msgid "Invalid user/mailbox name."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:150
+#: lib/fb_tools/mailaddress.py:146
 msgid "Invalid domain."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:204 lib/fb_tools/obj.py:252 lib/fb_tools/obj.py:308
+#: lib/fb_tools/mailaddress.py:200 lib/fb_tools/obj.py:247 lib/fb_tools/obj.py:303
 msgid "Wrong verbose level {!r}, must be >= 0"
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:296 lib/fb_tools/mailaddress.py:656
+#: lib/fb_tools/mailaddress.py:292 lib/fb_tools/mailaddress.py:652
 msgid "Checking equality {self!r} with {other!r} ..."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:352 lib/fb_tools/mailaddress.py:680
+#: lib/fb_tools/mailaddress.py:348 lib/fb_tools/mailaddress.py:676
 msgid "Object {o!r} for comparing is not a {c} object."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:357 lib/fb_tools/mailaddress.py:685
+#: lib/fb_tools/mailaddress.py:353 lib/fb_tools/mailaddress.py:681
 msgid "Comparing {self!r} with {other!r} ..."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:485
+#: lib/fb_tools/mailaddress.py:481
 msgid "Evaluating address {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:486
+#: lib/fb_tools/mailaddress.py:482
 msgid "Search pattern simple: {}"
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:491
+#: lib/fb_tools/mailaddress.py:487
 msgid "Search pattern full: {}"
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:515
+#: lib/fb_tools/mailaddress.py:511
 msgid "Parameters {lst} may not be given, if parameter {a!r} was given."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:526
+#: lib/fb_tools/mailaddress.py:522
 msgid "Invalid full user name."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:879 lib/fb_tools/mailaddress.py:893
+#: lib/fb_tools/mailaddress.py:875 lib/fb_tools/mailaddress.py:889
 msgid "Given object {o!r} is not a sequence type, but a {t!r} type instead."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:908
+#: lib/fb_tools/mailaddress.py:904
 msgid "{m} takes at most {max} arguments ({n} given)."
 msgstr ""
 
-#: lib/fb_tools/mailaddress.py:948
+#: lib/fb_tools/mailaddress.py:944
 msgid "Mail address {} is not in address list."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:100
+#: lib/fb_tools/multi_config.py:92
 msgid "Config loader method {!r} was not found."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:211 lib/fb_tools/multi_config.py:213 lib/fb_tools/multi_config.py:215
+#: lib/fb_tools/multi_config.py:203 lib/fb_tools/multi_config.py:205 lib/fb_tools/multi_config.py:207
 msgid "{} configuration is not supported."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:268
+#: lib/fb_tools/multi_config.py:260
 msgid "Additional config file {!r} does not exists."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:282
+#: lib/fb_tools/multi_config.py:274
 msgid "Configuration file {!r} is not readable."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:306
+#: lib/fb_tools/multi_config.py:298
 msgid "Configuration directory {!r} may not be absolute."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:386
+#: lib/fb_tools/multi_config.py:378
 msgid "Cannot use {!r} as delimiters for ini-files."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:408
+#: lib/fb_tools/multi_config.py:400
 msgid "Cannot use {!r} as comment prefixes for ini-files."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:430
+#: lib/fb_tools/multi_config.py:422
 msgid "Cannot use {!r} as inline comment prefixes for ini-files."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:616 lib/fb_tools/multi_config.py:627
+#: lib/fb_tools/multi_config.py:608 lib/fb_tools/multi_config.py:619
 msgid "Stem {!r} is not a String type."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:620 lib/fb_tools/multi_config.py:631 lib/fb_tools/multi_config.py:638
+#: lib/fb_tools/multi_config.py:612 lib/fb_tools/multi_config.py:623 lib/fb_tools/multi_config.py:630
 msgid "File name stem {!r} is invalid."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:646
+#: lib/fb_tools/multi_config.py:638
 msgid "Invalid configuration type {t!r} - not found in {w!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:686
+#: lib/fb_tools/multi_config.py:678
 msgid "Collecting all configuration files."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:693
+#: lib/fb_tools/multi_config.py:685
 msgid "Discovering config directory {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:702
+#: lib/fb_tools/multi_config.py:694
 msgid "Collected config files:"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:715
+#: lib/fb_tools/multi_config.py:707
 msgid "Checking permissions of config files ..."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:731
+#: lib/fb_tools/multi_config.py:723
 msgid "Checking permissions of {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:735
+#: lib/fb_tools/multi_config.py:727
 msgid "Found file permissions of {fn!r}: {mode:04o}"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:738
+#: lib/fb_tools/multi_config.py:730
 msgid "File {fn!r} is readable by group or by others, found mode {mode:04o}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:750
+#: lib/fb_tools/multi_config.py:742
 msgid "Trying to detect file type of additional config file {!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:759 lib/fb_tools/multi_config.py:824
+#: lib/fb_tools/multi_config.py:751 lib/fb_tools/multi_config.py:816
 msgid "Checking file {fn!r} for pattern {pat!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:765 lib/fb_tools/multi_config.py:830
+#: lib/fb_tools/multi_config.py:757 lib/fb_tools/multi_config.py:822
 msgid "Found config file {fi!r}, loader method {m!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:779
+#: lib/fb_tools/multi_config.py:771
 msgid "Did not found file type of additional config file {fn!r}. Available config types are: {list}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:798
+#: lib/fb_tools/multi_config.py:790
 msgid "Something strange is happend, file type {!r} not found."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:808
+#: lib/fb_tools/multi_config.py:800
 msgid "Checking, whether {!r} is a possible config file."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:813
+#: lib/fb_tools/multi_config.py:805
 msgid "Path {!r} is not a regular file."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:849
+#: lib/fb_tools/multi_config.py:841
 msgid "Reading configuration file {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:853
+#: lib/fb_tools/multi_config.py:845
 msgid "Using loading method {!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:861
+#: lib/fb_tools/multi_config.py:853
 msgid "Read config from {fn!r}:"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:872
+#: lib/fb_tools/multi_config.py:864
 msgid "Read merged config:"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:879
+#: lib/fb_tools/multi_config.py:871
 msgid ""
 "Character set detection by module {mod!r} for file {fn!r} should not be used, using character "
 "set {enc!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:886
+#: lib/fb_tools/multi_config.py:878
 msgid "Trying to detect character set of file {fn!r} ..."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:897
+#: lib/fb_tools/multi_config.py:889
 #, python-format
 msgid ""
 "The confidence of {con:0.1f}% is lower than the limit of {lim:0.1f}%, using character set "
 "{cs_def!r} instead of {cs_found!r}."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:907
+#: lib/fb_tools/multi_config.py:899
 msgid "Got {what} on detecting cheracter set of {fn!r}: {e}"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:912
+#: lib/fb_tools/multi_config.py:904
 msgid "Found character set {cs!r} for file {fn!r} with a confidence of {con:0.1f}%."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:922 lib/fb_tools/multi_config.py:952 lib/fb_tools/multi_config.py:986
-#: lib/fb_tools/multi_config.py:1043 lib/fb_tools/multi_config.py:1069
+#: lib/fb_tools/multi_config.py:914 lib/fb_tools/multi_config.py:944 lib/fb_tools/multi_config.py:978
+#: lib/fb_tools/multi_config.py:1035 lib/fb_tools/multi_config.py:1061
 msgid "Reading {tp} file {fn!r} ..."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:933 lib/fb_tools/multi_config.py:967 lib/fb_tools/multi_config.py:1050
-#: lib/fb_tools/multi_config.py:1083
+#: lib/fb_tools/multi_config.py:925 lib/fb_tools/multi_config.py:959 lib/fb_tools/multi_config.py:1042
+#: lib/fb_tools/multi_config.py:1075
 msgid "{what} parse error in {fn!r}, line {line}, column {col}: {msg}"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:940 lib/fb_tools/multi_config.py:974 lib/fb_tools/multi_config.py:1021
-#: lib/fb_tools/multi_config.py:1057 lib/fb_tools/multi_config.py:1087
-#: lib/fb_tools/multi_config.py:1094
+#: lib/fb_tools/multi_config.py:932 lib/fb_tools/multi_config.py:966 lib/fb_tools/multi_config.py:1013
+#: lib/fb_tools/multi_config.py:1049 lib/fb_tools/multi_config.py:1079
+#: lib/fb_tools/multi_config.py:1086
 msgid "Got {what} on reading and parsing {fn!r}: {e}"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:1003
+#: lib/fb_tools/multi_config.py:995
 msgid "Arguments on initializing {}:"
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:1107
+#: lib/fb_tools/multi_config.py:1099
 msgid "Evaluation of configuration could only be happen after reading it."
 msgstr ""
 
-#: lib/fb_tools/multi_config.py:1127
+#: lib/fb_tools/multi_config.py:1119
 msgid "Invalid value {val!r} in section {sec!r} for console timeout."
 msgstr ""
 
-#: lib/fb_tools/obj.py:63
+#: lib/fb_tools/obj.py:58
 msgid "The base directory {!r} is not existing or not a directory."
 msgstr ""
 
-#: lib/fb_tools/obj.py:146
+#: lib/fb_tools/obj.py:141
 msgid "undefined error."
 msgstr ""
 
-#: lib/fb_tools/obj.py:155
+#: lib/fb_tools/obj.py:150
 msgid "Exception happened"
 msgstr ""
 
-#: lib/fb_tools/obj.py:332
+#: lib/fb_tools/obj.py:327
 msgid "Base directory {!r} does not exists."
 msgstr ""
 
-#: lib/fb_tools/obj.py:335
+#: lib/fb_tools/obj.py:330
 msgid "Path for base directory {!r} is not a directory."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:72
+#: lib/fb_tools/pidfile.py:69
 msgid "Invalid pidfile {f!r} given: {r}"
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:75
+#: lib/fb_tools/pidfile.py:72
 msgid "Invalid pidfile {!r} given."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:99
+#: lib/fb_tools/pidfile.py:96
 msgid "The pidfile {f!r} is currently in use by the application with the PID {p}."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:166
+#: lib/fb_tools/pidfile.py:163
 msgid "No filename given on initializing {} object."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:284
+#: lib/fb_tools/pidfile.py:281
 msgid "Pidfile {!r} doesn't exists, not removing."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:290
+#: lib/fb_tools/pidfile.py:287
 msgid "Auto removing disabled, don't deleting {!r}."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:295
+#: lib/fb_tools/pidfile.py:292
 msgid "Removing pidfile {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:298 lib/fb_tools/pidfile.py:332
+#: lib/fb_tools/pidfile.py:295 lib/fb_tools/pidfile.py:329
 msgid "Just kidding ..."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:303
+#: lib/fb_tools/pidfile.py:300
 msgid "Could not delete pidfile {f!r}: {e}"
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:322
+#: lib/fb_tools/pidfile.py:319 lib/fb_tools/pidfile.py:382
 msgid "Invalid PID {p} for creating pidfile {f!r} given."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:330
+#: lib/fb_tools/pidfile.py:327
 msgid "Deleting pidfile {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:340
+#: lib/fb_tools/pidfile.py:337
 msgid "Trying opening {!r} exclusive ..."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:343 lib/fb_tools/pidfile.py:395
+#: lib/fb_tools/pidfile.py:340 lib/fb_tools/pidfile.py:392
 msgid "Simulation mode - don't real writing in {!r}."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:354
+#: lib/fb_tools/pidfile.py:351
 msgid "Error on creating pidfile {f!r}: {e}"
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:358 lib/fb_tools/pidfile.py:401
+#: lib/fb_tools/pidfile.py:355 lib/fb_tools/pidfile.py:398
 msgid "Writing {p} into {f!r} ..."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:379
+#: lib/fb_tools/pidfile.py:376
 msgid "Calling {} on a not self created pidfile."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:392
+#: lib/fb_tools/pidfile.py:389
 msgid "Trying opening {!r} for recreate ..."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:407
+#: lib/fb_tools/pidfile.py:404
 msgid "Error on recreating pidfile {f!r}: {e}"
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:433
+#: lib/fb_tools/pidfile.py:430
 msgid "Pidfile parent directory {!r} doesn't exists."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:437
+#: lib/fb_tools/pidfile.py:434
 msgid "Pidfile parent directory {!r} is not a directory."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:441
+#: lib/fb_tools/pidfile.py:438
 msgid "No write access to pidfile parent directory {!r}."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:448
+#: lib/fb_tools/pidfile.py:445
 msgid "It is not a regular file."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:466
+#: lib/fb_tools/pidfile.py:463
 msgid "Reading content of pidfile {!r} ..."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:487
+#: lib/fb_tools/pidfile.py:484
 msgid "No useful information found in pidfile {f!r}: {z!r}"
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:492
+#: lib/fb_tools/pidfile.py:489
 msgid "Trying check for process with PID {} ..."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:498
+#: lib/fb_tools/pidfile.py:495
 msgid "Process with PID {} anonymous died."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:502
+#: lib/fb_tools/pidfile.py:499
 msgid "No permission to signal the process {} ..."
 msgstr ""
 
-#: lib/fb_tools/pidfile.py:506
+#: lib/fb_tools/pidfile.py:503
 msgid "Got a {c}: {e}."
 msgstr ""
 
-#: lib/fb_tools/xlate.py:107
+#: lib/fb_tools/xlate.py:106
 msgid "Module directory: {!r}"
 msgstr ""
 
-#: lib/fb_tools/xlate.py:108
+#: lib/fb_tools/xlate.py:107
 msgid "Base directory: {!r}"
 msgstr ""
 
-#: lib/fb_tools/xlate.py:109
+#: lib/fb_tools/xlate.py:108
 msgid "Locale directory: {!r}"
 msgstr ""
 
-#: lib/fb_tools/xlate.py:110
+#: lib/fb_tools/xlate.py:109
 msgid "Locale domain: {!r}"
 msgstr ""
 
-#: lib/fb_tools/xlate.py:111
+#: lib/fb_tools/xlate.py:110
 msgid "Found .mo-file: {!r}"
 msgstr ""
```

### Comparing `fb_tools-2.2.2/setup.cfg` & `fb_tools-2.2.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -79,13 +79,13 @@
 
 [pep8]
 max-line-length = 99
 
 [flake8]
 max-line-length = 99
 max-complexity = 20
-ignore = E226,E302,E41,E402,W503
+ignore = E226,E302,E41,E402,W503,B902
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fb_tools-2.2.2/setup.py` & `fb_tools-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,35 +3,28 @@
 
 """
 @summary: Modules for common used objects, error classes and methods.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
 @license: LGPL3+
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 """
 from __future__ import print_function
 
-import os
-import sys
-import re
-import pprint
 import datetime
-import textwrap
 import glob
+import os
+import pprint
+import re
 import subprocess
-
+import sys
+import textwrap
 from pathlib import Path
 
-# Third party modules
-from setuptools import setup
-from setuptools.command.sdist import sdist
-
-from babel.messages import frontend as babel
-
 # own modules:
 __base_dir__ = os.path.abspath(os.path.dirname(__file__))
 __bin_dir__ = os.path.join(__base_dir__, 'bin')
 __lib_dir__ = os.path.join(__base_dir__, 'lib')
 __module_dir__ = os.path.join(__lib_dir__, 'fb_tools')
 __init_py__ = os.path.join(__module_dir__, '__init__.py')
 __local_usr_dir__ = Path(__base_dir__) / 'usr'
@@ -56,28 +49,34 @@
 
 
 # print("Paths:\n{}".format(pp(PATHS)))
 
 if os.path.exists(__module_dir__) and os.path.isfile(__init_py__):
     sys.path.insert(0, os.path.abspath(__lib_dir__))
 
+# Third party modules
+from babel.messages import frontend as babel
+
 import fb_tools
 
+from setuptools import setup
+from setuptools.command.sdist import sdist
+
 # from fb_tools.common import pp
 
-ENCODING = "utf-8"
+ENCODING = 'utf-8'
 
 __packet_version__ = fb_tools.__version__
 
 __packet_name__ = 'fb_tools'
 __debian_pkg_name__ = 'fb-tools'
 
 __author__ = 'Frank Brehm'
 __contact__ = 'frank@brehm-online.com'
-__copyright__ = '(C) 2022 Frank Brehm, Berlin'
+__copyright__ = '(C) 2023 Frank Brehm, Berlin'
 __license__ = 'LGPL3+'
 __url__ = 'https://github.com/fbrehm/python_fb_tools'
 
 
 __open_args__ = {}
 if sys.version_info[0] < 3:
     __open_args__ = {'encoding': ENCODING, 'errors': 'surrogateescape'}
@@ -285,14 +284,15 @@
 
 
 # -----------------------------------
 class Sdist(sdist):
     """Custom ``sdist`` command to ensure that mo files are always created."""
 
     def run(self):
+        """Compile the l18n catalog."""
         self.run_command('compile_catalog')
         # sdist is an old style class so super cannot be used.
         sdist.run(self)
 
 
 # -----------------------------------
 setup(
```

### Comparing `fb_tools-2.2.2/test/general.py` & `fb_tools-2.2.3/test/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: GPL3
 @summary: general used functions an objects used for unit tests on
           the base python modules
 """
 
 import os
 import sys
```

### Comparing `fb_tools-2.2.2/test/test_00_errors.py` & `fb_tools-2.2.3/test/test_00_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on error (exception) classes
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_tools-2.2.2/test/test_05_common.py` & `fb_tools-2.2.3/test/test_05_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on common.py
 """
 
 import os
 import sys
 import logging
```

### Comparing `fb_tools-2.2.2/test/test_10_base_object.py` & `fb_tools-2.2.3/test/test_10_base_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on base object
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_tools-2.2.2/test/test_13_collections.py` & `fb_tools-2.2.3/test/test_13_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on fb_tools.collections
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_tools-2.2.2/test/test_15_mailaddress.py` & `fb_tools-2.2.3/test/test_15_mailaddress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank.brehm@pixelpark.com
-@copyright: © 2021 Frank Brehm, Digitas Pixelpark GmbH Berlin
+@copyright: © 2023 Frank Brehm, Digitas Pixelpark GmbH Berlin
 @license: LGPL3
 @summary: test script (and module) for unit tests on mailaddress class and objects
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_tools-2.2.2/test/test_17_multicfg.py` & `fb_tools-2.2.3/test/test_17_multicfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on multi config class
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_tools-2.2.2/test/test_18_pidfile.py` & `fb_tools-2.2.3/test/test_18_pidfile.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.2/test/test_20_handling_object.py` & `fb_tools-2.2.3/test/test_20_handling_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on handling object
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_tools-2.2.2/test/test_30_base_handler.py` & `fb_tools-2.2.3/test/test_30_base_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on base handler object
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_tools-2.2.2/test/test_33_lock.py` & `fb_tools-2.2.3/test/test_33_lock.py`

 * *Files identical despite different names*

