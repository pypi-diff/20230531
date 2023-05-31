# Comparing `tmp/inhandtest-0.0.49.tar.gz` & `tmp/inhandtest-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.49.tar", last modified: Fri May 19 01:35:34 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.50.tar", last modified: Wed May 31 02:53:07 2023, max compression
```

## Comparing `inhandtest-0.0.49.tar` & `inhandtest-0.0.50.tar`

### file list

```diff
@@ -1,43 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 01:35:34.000000 inhandtest-0.0.49/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.49/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-05-19 01:35:34.000000 inhandtest-0.0.49/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.49/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 01:35:34.000000 inhandtest-0.0.49/dm/
--rw-rw-rw-   0        0        0      134 2023-04-25 08:38:57.000000 inhandtest-0.0.49/dm/__init__.py
--rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.49/dm/mqtt.py
--rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.49/dm/register_v1.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:35:34.000000 inhandtest-0.0.49/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.49/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:35:34.000000 inhandtest-0.0.49/inhandtest/base_page/
--rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.49/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    39712 2023-05-16 03:23:36.000000 inhandtest-0.0.49/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.49/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.49/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    52406 2023-05-18 09:41:02.000000 inhandtest-0.0.49/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    15461 2023-05-17 09:10:24.000000 inhandtest-0.0.49/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.49/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.49/inhandtest/file.py
--rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.49/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.49/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.49/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    51883 2023-05-16 09:03:39.000000 inhandtest-0.0.49/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.49/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.49/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6847 2023-05-18 06:06:23.000000 inhandtest-0.0.49/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.49/inhandtest/ip.py
--rw-rw-rw-   0        0        0    11620 2023-05-08 10:30:07.000000 inhandtest-0.0.49/inhandtest/mail.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:35:34.000000 inhandtest-0.0.49/inhandtest/pages/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.49/inhandtest/pages/__init__.py
--rw-rw-rw-   0        0        0      303 2023-05-15 09:37:04.000000 inhandtest-0.0.49/inhandtest/pages/locale.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.49/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    32773 2023-05-16 10:13:54.000000 inhandtest-0.0.49/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    25281 2023-05-12 08:18:46.000000 inhandtest-0.0.49/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:35:34.000000 inhandtest-0.0.49/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-05-19 01:35:34.000000 inhandtest-0.0.49/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      890 2023-05-19 01:35:34.000000 inhandtest-0.0.49/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 01:35:34.000000 inhandtest-0.0.49/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-05-19 01:35:34.000000 inhandtest-0.0.49/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-19 01:35:34.000000 inhandtest-0.0.49/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      137 2023-05-15 07:42:26.000000 inhandtest-0.0.49/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 01:35:34.000000 inhandtest-0.0.49/setup.cfg
--rw-rw-rw-   0        0        0     1614 2023-05-19 01:33:42.000000 inhandtest-0.0.49/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.50/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-05-31 02:53:07.000000 inhandtest-0.0.50/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.50/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/dm/
+-rw-rw-rw-   0        0        0      134 2023-04-25 08:38:57.000000 inhandtest-0.0.50/dm/__init__.py
+-rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.50/dm/mqtt.py
+-rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.50/dm/register_v1.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.50/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.50/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    39712 2023-05-16 03:23:36.000000 inhandtest-0.0.50/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.50/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.50/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    56236 2023-05-29 08:18:45.000000 inhandtest-0.0.50/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    22363 2023-05-29 08:30:51.000000 inhandtest-0.0.50/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.50/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.50/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.50/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.50/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.50/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    51883 2023-05-16 09:03:39.000000 inhandtest-0.0.50/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.50/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    14352 2023-05-31 02:52:16.000000 inhandtest-0.0.50/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6847 2023-05-18 06:06:23.000000 inhandtest-0.0.50/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.50/inhandtest/ip.py
+-rw-rw-rw-   0        0        0    11620 2023-05-08 10:30:07.000000 inhandtest-0.0.50/inhandtest/mail.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/pages/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.50/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0      670 2023-05-25 08:19:46.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/edge_computing.py
+-rw-rw-rw-   0        0        0      345 2023-05-25 07:58:59.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0     5342 2023-05-29 08:19:20.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     5007 2023-05-29 08:07:23.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/edge_computing/python_edge_computing_locators.py
+-rw-rw-rw-   0        0        0     2365 2023-05-29 08:24:24.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0     4051 2023-05-25 08:40:52.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      767 2023-05-25 07:59:28.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0     6939 2023-05-25 02:09:36.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/acl_locators.py
+-rw-rw-rw-   0        0        0     3783 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/bridge_locators.py
+-rw-rw-rw-   0        0        0    15320 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/cellular_locators.py
+-rw-rw-rw-   0        0        0     3388 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/dhcp_locators.py
+-rw-rw-rw-   0        0        0     2457 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/dns_locators.py
+-rw-rw-rw-   0        0        0     5274 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/ethernet_locators.py
+-rw-rw-rw-   0        0        0     7476 2023-05-25 08:45:27.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/firewall.py
+-rw-rw-rw-   0        0        0     8415 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/gps_locators.py
+-rw-rw-rw-   0        0        0      470 2023-05-23 03:37:38.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/host_list_locators.py
+-rw-rw-rw-   0        0        0    11017 2023-05-25 06:05:46.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/l2tp_locators.py
+-rw-rw-rw-   0        0        0     3667 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/lan_locators.py
+-rw-rw-rw-   0        0        0     2341 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/loopback_locators.py
+-rw-rw-rw-   0        0        0     5698 2023-05-25 02:19:26.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/nat_locators.py
+-rw-rw-rw-   0        0        0     2628 2023-05-25 05:59:23.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    32342 2023-05-25 08:09:35.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/network_interface.py
+-rw-rw-rw-   0        0        0     1745 2023-05-25 03:11:00.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/network_locators.py
+-rw-rw-rw-   0        0        0    13074 2023-05-25 08:09:35.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/network_services.py
+-rw-rw-rw-   0        0        0     4371 2023-05-25 01:08:23.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/routing.py
+-rw-rw-rw-   0        0        0     1305 2023-05-23 06:46:19.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/routing_status_locators.py
+-rw-rw-rw-   0        0        0     2972 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/static_routing_locators.py
+-rw-rw-rw-   0        0        0     9910 2023-05-25 05:58:37.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/vpn.py
+-rw-rw-rw-   0        0        0     5208 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/wan_locators.py
+-rw-rw-rw-   0        0        0    10254 2023-05-24 10:28:05.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/network/wlan_locators.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6971 2023-05-25 08:09:35.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.50/inhandtest/pages/ingateway/overview/overview_locators.py
+-rw-rw-rw-   0        0        0      303 2023-05-15 09:37:04.000000 inhandtest-0.0.50/inhandtest/pages/locale.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.50/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    32773 2023-05-16 10:13:54.000000 inhandtest-0.0.50/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    25490 2023-05-31 02:52:16.000000 inhandtest-0.0.50/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2784 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 02:53:07.000000 inhandtest-0.0.50/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      137 2023-05-15 07:42:26.000000 inhandtest-0.0.50/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 02:53:07.000000 inhandtest-0.0.50/setup.cfg
+-rw-rw-rw-   0        0        0     1614 2023-05-31 02:52:54.000000 inhandtest-0.0.50/setup.py
```

### Comparing `inhandtest-0.0.49/PKG-INFO` & `inhandtest-0.0.50/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.49
+Version: 0.0.50
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.49/README.md` & `inhandtest-0.0.50/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/dm/mqtt.py` & `inhandtest-0.0.50/dm/mqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/dm/register_v1.py` & `inhandtest-0.0.50/dm/register_v1.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.50/inhandtest/base_page/_ig_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.50/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.50/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/base_page/base_page.py` & `inhandtest-0.0.50/inhandtest/base_page/base_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 """
 import os.path
 import sys
 from os import path
 from inhandtest.base_page._ig_contents_locators import IGContentsLocators
 from typing import List
 from inhandtest.exception import ModelError
-from inhandtest.tools import loop_inspector
+from inhandtest.tools import loop_inspector, replace_str
 from playwright.sync_api import Page, Locator, expect, TimeoutError, sync_playwright
 from inhandtest.base_page._vg710_contents_locators import VGContentsLocators
 from inhandtest.base_page._ir3XX_contents_locators import Ir3XXContentsLocators
 from inhandtest.base_page.table_tr import Table, IgTable
+from collections import Counter
 import allure
 import logging
 import re
 
 
 class BasePage:
 
@@ -99,15 +100,17 @@
         else:
             browser = self.__playwright.chromium
         self.__browser = browser.launch(headless=False)
         if self.model in self.__http_credentials_model:
             http_credentials = {'username': self.username, 'password': self.password}
         else:
             http_credentials = None
-        self.__context = self.__browser.new_context(ignore_https_errors=True, http_credentials=http_credentials)
+        self.__context = self.__browser.new_context(ignore_https_errors=True, http_credentials=http_credentials,
+                                                    viewport={'width': 1366, 'height': 768},
+                                                    permissions=['clipboard-read'])
         logging.info('Start your journey browser is chrome')
         self.page = self.__context.new_page()
         self.page.on("dialog", dialog_)
 
     @allure.step("用户登录")
     def login(self, username=None, password=None, status='success') -> None:
         """
@@ -315,29 +318,31 @@
             else:
                 locator.click()
             if log_desc:
                 logging.info(f'Device {self.host} click {log_desc}')
             self.tip_messages(tip_messages, tip_messages_timeout)
             if wait_for_time:
                 self.page.wait_for_timeout(wait_for_time)
+        else:
+            logging.warning(f'Device {self.host} click {log_desc} is disabled')
 
     @allure.step('勾选框')
     def check(self, locator: Locator, action='check', log_desc=None, tip_messages: str or list = None) -> None:
         """ 封装公共的单选操作
         :param locator:  元素定位
         :param log_desc: 功能描述，用英文 如 Static Routing Destination
         :param action: 'check'|'uncheck'| None | '是' | 'Yes'
         :param tip_messages: str or list 点击后等待该tip出现 再等待tip消失，如果有多个，使用列表传入
                             tip_messages 是支持模糊匹配
                             该项校验 页面元素必须停留时间1秒及更多时间，否则不容易检测到导致报错
         :return:
         """
 
         if action is not None:
-            if action in ('check', 'Yes', '是', 'yes'):
+            if action in ('check', 'Yes', '是', 'yes', 'enable', True):
                 locator.check()
             else:
                 locator.uncheck()
             if log_desc:
                 logging.info(f'Device {self.host} {log_desc} {action}')
             self.tip_messages(tip_messages)
 
@@ -384,56 +389,57 @@
                             break
                     else:
                         raise Exception('found more option elements')
                 else:
                     raise Exception('scroll bar too lang, more 100 times')
 
         if value is not None:
+            value = str(value)
             locator.wait_for(state='visible')
             if locator.get_attribute('aria-controls') or locator.locator('.ant-select-selection').get_attribute(
                     'aria-controls'):
                 if locator.get_attribute("aria-controls"):  # ER805 设备的下拉选择
                     now_option = locator.locator('../..').locator('.ant-select-selection-item').inner_text()
                     option_p = self.page.locator(f'//div[@id="{locator.get_attribute("aria-controls")}"]').locator(
                         '..').locator('//div[@class="rc-virtual-list-holder-inner"]')
                     option = option_p.locator(f'//div[@title="{value}"]')
                     all_option = option_p.locator('.ant-select-item.ant-select-item-option')
                 else:  # IG902 设备的下拉选择
                     now_option = locator.locator(
                         '//div/div/div[@class="ant-select-selection-selected-value"]').inner_text()
                     option_id = locator.locator(".ant-select-selection").get_attribute("aria-controls")
                     all_option = self.page.locator(f'//div[@id="{option_id}"]').locator('//ul[@role="listbox"]/li')
-                    option = self.page.locator(f'//div[@id="{option_id}"]').locator('//ul[@role="listbox"]/li',
-                                                                                    has_text=value)
+                    option = self.page.locator(f'//div[@id="{option_id}"]').locator(
+                        f'//ul[@role="listbox"]/li').get_by_text(value, exact=True)
                 if now_option != value:
                     locator.scroll_into_view_if_needed()
                     if not locator.is_editable():
                         locator.click(force=True)
                     else:
                         locator.click()
                     scroll_into_view_action(all_option, option)
             else:  # IR300 等设备的下拉选择
-                locator.select_option(str(value))  # value 可以为label 或者value
+                locator.select_option(value)  # value 可以为label 或者value
                 if locator.locator(f'//option[@value="{value}"]').count() == 1:
                     value = locator.locator(f'//option[@value="{value}"]').inner_text()
             if log_desc:
                 logging.info(f"Device {self.host} select {log_desc} of {value}")
 
     @allure.step('切换按钮')
     def switch_button(self, locator: Locator, action: str = 'enable', log_desc=None) -> None:
         """控制通用开关按钮开关， 如拨号的开关
 
         :param locator:  开关按钮元素
-        :param action: enable, disable, None 可以开启或关闭，但是并没有提交，只是点击了下
+        :param action: enable, disable, None, True, False 可以开启或关闭，但是并没有提交，只是点击了下
         :param log_desc:  开关功能描述
         :return: None
         """
         if action is not None:
             locator.wait_for(state='visible')
-            if action.lower() == 'enable':
+            if (isinstance(action, str) and action.lower() == 'enable') or (isinstance(action, bool) and action):
                 if locator.get_attribute('aria-checked') == 'false' or not locator.get_attribute('aria-checked'):
                     locator.click(force=True)
                     if log_desc:
                         logging.info(f"Device {self.host} {log_desc} enabled")
             else:
                 if locator.get_attribute('aria-checked') == 'false' or not locator.get_attribute('aria-checked'):
                     pass
@@ -449,22 +455,25 @@
         :param locator: 在所有label元素的上级div定位
         :param value: 选项的值，注意国际化
         :param log_desc: 选项的描述
         :return:
         """
         if value:
             locator.wait_for(state='visible')
-            locator_label = locator.locator(f'//label[text()="{value}"]')
-            if locator_label.count() == 1:
-                if 'ant-radio-wrapper-checked' not in locator_label.get_attribute('class'):
-                    locator.click(force=True)
+            option = locator.locator(f'//label', has_text=re.compile(value))
+            if option.count() == 1:
+                if 'ant-radio-wrapper-checked' not in option.get_attribute('class'):
+                    option.click(force=True)
                     if log_desc:
                         logging.info(f"Device {self.host} {log_desc} radio select {value}")
+                else:
+                    if log_desc:
+                        logging.info(f"Device {self.host} {log_desc} radio already select {value}")
             else:
-                raise Exception(f'found {value} option {locator_label.count()} elements')
+                raise Exception(f'found {value} option {option.count()} elements')
 
     @allure.step('伸缩按钮')
     def expand(self, left_text: str, action: str = 'expand') -> None:
         """ 伸缩按钮
 
         :param left_text: 伸缩按钮 左边的文本，需要注意国际化
         :param action: expand|close|None
@@ -508,15 +517,15 @@
         def upload():
             if path_:
                 if os.path.isfile(path_) and os.path.exists(path_):
                     with self.page.expect_file_chooser() as fc:
                         locator.click()
                     file_chooser = fc.value
                     file_chooser.set_files(path_)
-                    logging.info(f'Device {self.host} upload file Successful')
+                    logging.info(f'Device {self.host} upload {path_} Successful')
                 else:
                     logging.error(f'{path_} Does Not Exist.')
 
         if dialog_massage:
             self.dialog_massage(upload, dialog_massage)
         else:
             upload()
@@ -551,14 +560,15 @@
         :return:
         """
         if message:
             message = self.locale.get(message) if self.locale.get(message) else message
             with self.page.expect_event('dialog') as dialog_info:
                 f()
             assert message in dialog_info.value.message, f'{self.host} assert {message} dialog error'
+            logging.info(f'Device {self.host} assert dialog {message} successful')
 
     @allure.step("校验tip messages")
     def tip_messages(self, messages: str or list = None, timeout=30) -> None:
         """ 某些提交操作会出现文本的提示，提示在过几秒钟后会消失，对于该类消息的验证使用该方法，
             使用时需要在base_locator tip_messages 且返回字典数据
 
         :param messages: str or list 点击后等待该tip出现 再等待tip消失，如果有多个，使用列表传入
@@ -569,40 +579,49 @@
         """
         if messages:
             tip_messages = [messages] if isinstance(messages, str) else messages
             for message in tip_messages:
                 message = self.locale.get(message) if self.locale.get(message) else message  # 国际化转换
                 expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_visible(timeout=timeout * 1000)
                 expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_hidden(timeout=timeout * 1000)
+                logging.info(f'{self.host} assert tip {message} visible successful')
 
     @allure.step("校验text messages")
     def text_messages(self, messages: str or list = None, timeout=10) -> None:
         """ 对文本内容做验证，如在输入框输入错误内容时出现的文本，该类文本会一直存在
         :param messages: str or list 文本内容，如果有多个，使用列表传入
         :param timeout: 校验超时时间
         :return:
         """
         if messages:
             text_messages = [messages] if isinstance(messages, str) else messages
-            for message in text_messages:
+            text_messages = Counter(text_messages)  # 处理多个相同的文本
+            for message, count in text_messages.items():
                 message = self.locale.get(message) if self.locale.get(message) else message  # 国际化转换
-                expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_visible(timeout=timeout * 1000)
+                for i_ in range(0, count):
+                    expect(self.page.get_by_text(re.compile(message, re.IGNORECASE)).nth(i_)).to_be_visible(
+                        timeout=timeout * 1000)
+                    logging.info(f'{self.host} assert text the {i_}th {message}  visible successful')
 
     @allure.step("校验元素Title")
     def title_messages(self, messages: str or list = None, timeout=10) -> None:
         """ 对元素的属性title做内容验证，
         :param messages: str or list 文本内容，如果有多个，使用列表传入
         :param timeout: 校验超时时间
         :return:
         """
         if messages:
             text_messages = [messages] if isinstance(messages, str) else messages
-            for message in text_messages:
+            text_messages = Counter(text_messages)
+            for message, count in text_messages.items():
                 message = self.locale.get(message) if self.locale.get(message) else message  # 国际化转换
-                expect(self.page.get_by_title(re.compile(message, re.IGNORECASE))).to_be_visible(timeout=timeout * 1000)
+                for i_ in range(0, count):
+                    expect(self.page.get_by_title(re.compile(message, re.IGNORECASE)).nth(i_)).to_be_visible(
+                        timeout=timeout * 1000)
+                    logging.info(f'{self.host} assert title the {i_}th {message} visible successful')
 
     @allure.step('设置页面翻页')
     def page_refresh(self, refresh_time: str, select_locator: Locator) -> None:
         """
         :param refresh_time: str
                         '0'|'3'|'4'|'5'|'10'|'15'|'30'|'60'|'120'|'180'|'240'|'300'|'600'|'900'|'1200'|'1800'
         :param select_locator: 元素定位
@@ -616,38 +635,63 @@
             else:
                 if select_locator.is_disabled():
                     self.click(select_locator.locator('..').locator('#refresh-button'), 'refresh button')
                     self.page.wait_for_timeout(500)
                 self.select_option(select_locator, refresh_time, 'refresh time select')
                 self.click(select_locator.locator('..').locator('#refresh-button'), 'refresh button ok')
 
-    @allure.step("Table tr action")
+    @allure.step("操作表格")
     def table_tr(self, locators: dict, value: list, log_desc=None) -> List[int or None] or None:
         """
 
         :param locators: {"locator": $locator2, "param": {$key2: $value2}, "columns": list, 'unique_columns': list}
         :param value: [($action,{**kwarg})] ex: [('delete_all', )],  [('edit', $old, $new)]多个操作时使用列表 [('add',{}), ('add',{})]
         :param log_desc: 日志描述
         :return:
         """
         if self.model in ('IG902', 'IG502'):
-            tr = IgTable(locators.get('columns'), locators.get('locator'), locators.get('param'), log_desc)
+            tr = IgTable(locators.get('columns'), locators.get('locator'), locators.get('param'), log_desc,
+                         locators.get('action_confirm'), locators.get('pop_up_locator'))
             exist_tr = []
             if value:
                 for value_ in value:
                     if value_[0] == 'add':
                         tr.add(self.agg_in, **value_[1])
                     elif value_[0] == 'delete_all':
                         tr.delete_all()
-                    elif value_[0] == 'delete':
+                    elif value_[0] in ('delete', 'clear_log', 'uninstall'):
                         tr.delete(value_[1])
                     elif value_[0] == 'exist':
                         exist_tr.append(tr.exist(value_[1], self.locale))
                     elif value_[0] == 'edit':
                         tr.edit(self.agg_in, value_[1], **value_[2])
+                    elif value_[0] == 'connect':
+                        tr.connect(value_[1])
+                    elif value_[0] == 'associate_delete':
+                        tr.associate_delete(value_[1])
+                    elif value_[0] in ('download_log', 'export_config'):
+                        if isinstance(value_[2], str):
+                            file_path = value_[2]
+                            file_name = None
+                        elif isinstance(value_[2], dict):
+                            file_path = value_[2].get('file_path')
+                            file_name = value_[2].get('file_name')
+                        else:
+                            raise TypeError('download file_path type error')
+                        tr.download(self.download_file, value_[1], file_path, file_name)
+                    elif value_[0] in ('upload', 'import_config'):
+                        tr.upload(self.upload_file, value_[1], value_[2])
+                    elif value_[0] == 'start':
+                        tr.start(value_[1])
+                    elif value_[0] == 'stop':
+                        tr.stop(value_[1])
+                    elif value_[0] == 'restart':
+                        tr.restart(value_[1])
+                    elif value_[0] in ('check', 'enable'):
+                        tr.check(self.check, value_[1], value_[2])
                 return exist_tr
         else:
             tr = Table(locators.get('columns'), locators.get('locator'),
                        locators.get('unique_columns'), locators.get('param'), log_desc)
             exist_tr = []
             if value:
                 for value_ in value:
@@ -669,15 +713,15 @@
                     [($param1, {"locator": $locator1, "type": $type1, "relation": [($param2, $value2)], "param": {$key1: $value1}}),
                     ($param2, {"locator": $locator2, "type": $type2, "relation": [($param3, $value3),……], "param": {$key2: $value2}}),
                     ($param3, {"locator": $locator2, "type": 'table_tr', "relation": [($param3, $value3),……], "param": {$key2: $value2},
                                 "columns": list, 'unique_columns': list}),]
                     $param: 操作项的名称，如 'language'|'sim'|'status'
                     $locator: 操作项的元素定位， locator or [locator,locator,...]
                     $type: 操作项的类型 text|select|button|check|upload_file|download_file|tip_messages|text_messages|title_messages|
-                                     multi_select|multi_check|multi_fill|table_tr|switch_button|radio|expand|
+                                     multi_select|multi_check|multi_fill|table_tr|switch_button|radio_select|expand|
                             select value值可以是label|Value
                             multi_select指一个参数有多个select, 对应操作项的多个locator及value用[]传入
                     "relation":[($param, $value)]: 操作项的关联项，若有多个则首个为最先操作的关联项，其中$param为关联项的名称，$value为关联项的预期值
                     "param":{$key, $value}: 参数转换，如大小写转换{"ab":"AB"} {"wan":"Wan"}等.
                 :param action_dict: 要做操作的参数名称与对应的值{$param1: $value1, $param2: $value2}
                 :return:
                 """
@@ -688,15 +732,15 @@
                 self.page.wait_for_timeout(param_locator.get('wait_for'))
             if param_locator.get('type') == 'text':
                 self.fill(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'select':
                 if param_locator.get('param') and value in param_locator.get('param').keys():
                     value = param_locator.get('param').get(value)
                 self.select_option(param_locator.get('locator'), value, param)
-            elif param_locator.get('type') == 'radio':
+            elif param_locator.get('type') == 'radio_select':
                 if param_locator.get('param') and value in param_locator.get('param').keys():
                     value = param_locator.get('param').get(value)
                 self.radio_select(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'switch_button':
                 self.switch_button(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'expand':
                 self.expand(param_locator.get('locator'), value)  # 此处获取到的locator 是一个str
@@ -786,47 +830,57 @@
                         # 对关系项操作之前检查关系项
                         for relation_ in option[1].get("relation"):
                             relation_locator = [i[1] for i in locators if i[0] == relation_[0]][0]
                             operation(relation_[0], relation_locator, relation_[1])  # 关系项操作
                         relations.append(option[1].get("relation"))
                     operation(option[0], option[1], action_dict.get(option[0]))  # 本身操作
 
-    @allure.step("计算判断表达式{expect_}")
-    def eval_inner_text(self, expect_: dict, locators: list) -> bool:
+    @allure.step("计算元素表达式")
+    def eval_locator_attribute(self, expect_: dict, locators: list) -> bool:
         """对页面特定元素值做判断
 
         :param expect_: {$status: $expressions}
                         status: 状态名称， 比如可以传定义好的 current_sim
                         expressions: 完整表达式, 当判断int型的关系时${value}和期望值可加"",而当需要调用str型的关系时${value}和期望值都要加"",
                          例:（'${value}==1', '${value}!=1', '${value}>1', '${value}>=1', '${value}<1', '${value}<=1', "${value}"=="abc"
                         '"${value}".startswith("123")', '"${value}".endswith("23")', '"${value}" in a', '"${value}" not in b',
                         '"${value}".__contains__("234")', 'time.strptime("${value}}", "%Y-%m-%d %H:%M:%S")'）
                         ex: '${value}==8' 多个使用元组或者列表，注意期望值是字符串时需要带上引号， 如'${value}=="sim1"'
         :param locators: [($param1, {"locator": $locator1, "type": $type1, "relation": [($param2, $value2)], "param": {$key1: $value1}}),
                           ($param2, {"locator": $locator2, "type": $type2, "relation": [($param3, $value3),……], "param": {$key2: $value2}}),
                           ($param3, {"locator": $locator2, "type": 'table_tr', "relation": [($param3, $value3),……], "param": {$key2: $value2},
                                 "columns": list, 'unique_columns': list}),]
+                          type:  text, switch_button
+
         :return: 只返回True or False 不做断言
         """
         if expect_:
             for key in expect_.keys():
                 filter_key = list(filter(lambda x: x[0] == key, locators))
                 if len(filter_key) == 1:
                     option = filter_key[0]
                     locator = option[1].get('locator')
-                    if isinstance(locator, Locator):
-                        value = locator.first.inner_text() if locator.count() != 0 else 'None'
-                    else:
-                        value = str(locator)
+                    if option[1].get('type') == 'switch_button':
+                        if 'ant-switch-checked' in locator.first.get_attribute('class'):
+                            value = 'enable'
+                        else:
+                            value = 'disable'
+                    else:  # type is text
+                        if isinstance(locator, Locator):
+                            value = locator.first.inner_text() if locator.count() != 0 else 'None'
+                        else:
+                            value = str(locator)
                     try:
-                        expression = expect_.get(key).replace('${value}', value).replace('\n', ' ')
+                        if '${value}' in expect_.get(key):
+                            expression = expect_.get(key).replace('${value}', value).replace('\n', ' ')
+                        else:
+                            expression = f'"{expect_.get(key)}" == "{value}"'  # 默认使用等于判断
                         if option[1].get('param'):
-                            for replace_k, replace_v in option[1].get('param').items():
-                                expression = expression.replace(replace_k, replace_v)
-                        if eval(expression, {'repr': repr}):
+                            expression = replace_str(expression, option[1].get('param'))
+                        if eval(expression):
                             logging.info(f'Check {option[0]} , {expression} is true')
                         else:
                             logging.info(f'Check {option[0]} , {expression} is false')
                             return False
                     except TypeError:
                         logging.info(f'get {key} inner_text failed')
                         return False
@@ -836,15 +890,15 @@
 
     @allure.step("获取页面元素文本值")
     def get_text(self, keys: str or list or tuple, locators: list) -> str or dict or None:
         """获取页面元素文本值
 
         :param keys: None or str or list or tuple, 需要获取对应文本的元素的关键字
         :param locators: [($param1, {"locator": $locator1, "type": $type1}),
-                         type: 支持的类型有：'text'|'fill'|'select'
+                         type: 支持的类型有：'text'|'fill'|'select'|'clipboard'|'switch_button'
                          该select 为select标签的文本值， ER805 和ER605 直接使用text
         :return: 当key为None时，返回None
                  当key为str时，只能获取某一个字段的信息，同时使用str返回
                  当key为列表或者元组时， 使用字典返回相关关键字的信息
         """
         result = {}
         if keys:
@@ -856,14 +910,22 @@
                     locator = option[1].get('locator')
                     if isinstance(locator, Locator):
                         if locator.count() != 0:
                             if option[1].get('type') == 'select':
                                 value = locator.first.text_content()
                             elif option[1].get('type') == 'fill':
                                 value = locator.first.input_value()
+                            elif option[1].get('type') == 'clipboard':
+                                locator.first.click()
+                                value = self.page.evaluate('navigator.clipboard.readText()')
+                            elif option[1].get('type') == 'switch_button':
+                                if 'ant-switch-checked' in locator.first.get_attribute('class'):
+                                    value = 'enable'
+                                else:
+                                    value = 'disable'
                             else:
                                 value = locator.first.inner_text()
                         else:
                             raise
                     else:
                         value = str(locator)
                     result[key] = value
```

### Comparing `inhandtest-0.0.49/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.50/inhandtest/base_page/table_tr.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # @Author  : Pane Li
 # @File    : table_tr.py
 """
 table_tr
 
 """
 import logging
+import re
 from typing import List
 from inhandtest.tools import replace_str
 from playwright.sync_api import Locator
 
 
 class Table:
 
@@ -232,88 +233,212 @@
                 self.edit(**value_[0], **value_[1])
 
 
 class IgTable:
     __doc__ = """ 适配新产品架构，前端的表格，如IG
     """
 
-    def __init__(self, columns: list, table_locator: Locator, locale: dict = None, log_desc=None):
+    def __init__(self, columns: list, table_locator: Locator, locale: dict = None, log_desc=None, action_confirm=None,
+                 pop_up_locator=None):
         """
 
 
-        :param columns: [("add", {'locator': self.page.locator(''), 'type': 'button'}),
-                         ('name',{'locator': self.page.locator(''), 'type': 'fill'}),
+        :param columns: [('name',{'locator': self.page.locator(''), 'type': 'fill'}),
                          ('model',{'locator': self.page.locator(''), 'type': 'radio', param: {'value': '1'}}),
                          ('save',{'locator': self.page.locator(''), 'type': 'button'}),]
                          说明列的表名以及类型， 必须定义"add"、"save" 按钮， 因为添加按钮和保存按钮的定位不能自动获取
                         eg:[("列名称变量","列字段对应类型"), ...]
                         在选择时只接收label, 不支持value选择， 因为查找时也使用的label，
                         在表格只有查找功能是时，只要列属性不定义为check 都可以
         :param table_locator: 添加按钮元素上面的div定位
         :param locale: dict, 国际化文件,
+        :param log_desc: str, 日志描述
+        :param action_confirm: Locator, 是否操作有确认弹窗， 如delete，
+        :param pop_up_locator: Locator, 弹窗定位, 只有在操作表格操作时如果有弹窗需要给出该定位， 如edge import config
         """
         self.columns = columns  # 列名要与实际的列相对应，不能多也不能少
         self.table_locator = table_locator
         self.locale = locale
         self.log_desc = log_desc
+        self.action_confirm = action_confirm
+        self.pop_up_locator = pop_up_locator
 
     def exist(self, value: str, locale: dict) -> bool:
         """ 传入的资源是否存在, 对于check 项是不计入重复选项的，因为勾选其实只是开启功能而已
 
         :param value: str 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化 ex: 192.168.2.1255.255.255.0
         :param locale: dict 国际化， 默认为类初始化的locale, 也可以单独传入
         :return: True|False
         """
         locale = self.locale if locale is None else locale
         if value:
-            value = replace_str(value, locale)  # 期望的值
-            exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
+            value = replace_str(str(value), locale)  # 期望的值
+            exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
             if exist_tr.count() > 0:
                 return True
         return False
 
-    def add(self, agg_in, **kwargs,) -> None:
+    def add(self, agg_in, **kwargs, ) -> None:
         """ add 前是不查找是否存在的，直接加
 
         :param agg_in: function, 导致该方法不能单独使用
         :param kwargs str, 待添加列 及对应值
         :return:
         """
-        self.table_locator.locator('//button').first.click()
-        if 'save' not in list(kwargs.keys()):
+        if ('save' not in list(kwargs.keys())) and ('cancel' not in list(kwargs.keys())):
             kwargs['save'] = True
-        agg_in(self.columns, kwargs)
-        logging.info(f'table resource {kwargs} add success')
+        if kwargs.get('is_exists'):
+            is_exists = kwargs.pop('is_exists')
+            if not self.exist(is_exists, self.locale):
+                self.table_locator.locator('//button').first.click()
+                agg_in(self.columns, kwargs)
+                logging.info(f'table resource {kwargs} add success')
+            else:
+                logging.info(f'table resource {kwargs} exist')
+        else:
+            self.table_locator.locator('//button').first.click()
+            agg_in(self.columns, kwargs)
+            if not kwargs.get('cancel'):
+                logging.info(f'table resource {kwargs} add success')
 
-    def edit(self, agg_in, old_value, **kwargs,) -> None:
+    def edit(self, agg_in, old_value, **kwargs) -> None:
         """ 只能编辑匹配到的第一条记录
 
         :param agg_in: function, 导致该方法不能单独使用
         :param old_value: str, 旧值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值
         :param kwargs str, 待添加列 及对应值
         :return:
         """
         old_value = replace_str(old_value, self.locale)
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=old_value)
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(old_value))
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-form"]').click()
-            if 'save' not in list(kwargs.keys()):
+            if ('save' not in list(kwargs.keys())) and ('cancel' not in list(kwargs.keys())):
                 kwargs['save'] = True
             agg_in(self.columns, kwargs)
-            logging.info(f'table resource {kwargs} edit success')
+            if not kwargs.get('cancel'):
+                logging.info(f'table resource {kwargs} edit success')
+        else:
+            logging.info(f'table resource {old_value} not exist')
 
     def delete(self, value: str) -> None:
         """
         :param value str, 待删除列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         while exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-delete"]').click()
+            if isinstance(self.action_confirm, Locator):
+                self.action_confirm.click()  # 二次确认
         logging.info(f'table resource {value} all delete')
 
+    def associate_delete(self, value: str) -> None:
+        """
+        :param value str, 关联删除按钮，如VPN 中l2tp client表格中的删除按钮
+        :return:
+        """
+        value = replace_str(value, self.locale)
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        while exist_tr.count() > 0:
+            exist_tr.first.locator('//i[@class="anticon anticon-close"]').click()
+        logging.info(f'table resource {value} all delete associate')
+
+    def download(self, action, value: str, file_path: str, file_name: str = None):
+        """
+        :param action: function, 导致该方法不能单独使用
+        :param value str,
+        :param file_path: str, 下载文件存放路径
+        :param file_name: str, 下载文件名
+        :return:
+        """
+        value = replace_str(value, self.locale)
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        if exist_tr.count() > 0:
+            action(exist_tr.first.locator('//i[@class="anticon.anticon-download"]').first, file_path, file_name=file_name)
+        logging.info(f'table resource {value} download success')
+
+    def upload(self, action, value, file_path):
+        """
+        :param action: function, 导致该方法不能单独使用
+        :param value str, 待上传列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
+        :param file_path: str, 上传文件全路径
+        :return:
+        """
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        if exist_tr.count() > 0:
+            exist_tr.first.locator('//i[@class="anticon.anticon-upload"]').click()
+            action(self.pop_up_locator.locator('.anticon.anticon-upload').nth(0), file_path)
+            self.pop_up_locator.locator('.ant-btn.ant-btn-primary').nth(0).click()
+        logging.info(f'table resource {value}  click upload')
+
+    def check(self, action, value, check_value):
+        """
+        :param action: function, 导致该方法不能单独使用
+        :param value str, 待check 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
+        :param check_value: str, 待check值
+        :return:
+        """
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        if exist_tr.count() > 0:
+            action(exist_tr.first.locator('//input[@type="checkbox"][@class="ant-checkbox-input"]').nth(0), check_value)
+        logging.info(f'table resource {value}  {check_value}')
+
+    def start(self, value: str) -> None:
+        """
+        :param value str, 待开始列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
+        :return:
+        """
+        value = replace_str(value, self.locale)
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        if exist_tr.count() > 0:
+            exist_tr.first.locator('//i[@class="anticon anticon-play-circle"]').first.click()
+            if isinstance(self.action_confirm, Locator):
+                self.action_confirm.click()  # 二次确认
+        logging.info(f'table resource {value} all start')
+
+    def stop(self, value: str) -> None:
+        """
+        :param value str, 待停止列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
+        :return:
+        """
+        value = replace_str(value, self.locale)
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        if exist_tr.count() > 0:
+            exist_tr.first.locator('//i[@class="anticon anticon-pause-circle"]').first.click()
+            if isinstance(self.action_confirm, Locator):
+                self.action_confirm.click()  # 二次确认
+        logging.info(f'table resource {value} all stop')
+
+    def restart(self, value: str) -> None:
+        """
+        :param value str, 待重启列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
+        :return:
+        """
+        value = replace_str(value, self.locale)
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        if exist_tr.count() > 0:
+            exist_tr.first.locator('//i[@class="anticon anticon-undo"]').first.click()
+            if isinstance(self.action_confirm, Locator):
+                self.action_confirm.click()  # 二次确认
+        logging.info(f'table resource {value} all restart')
+
+    def connect(self, value: str) -> None:
+        """
+        :param value str, WLAN 页面connect连接，每列值可按顺序直接连接在一起传入，当然也可以传一列的值
+        :return:
+        """
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        if exist_tr.count() > 0:
+            if exist_tr.first.locator('//button[@class="ant-btn ant-btn-background-ghost"]').is_enabled():
+                exist_tr.first.locator('//button[@class="ant-btn ant-btn-background-ghost"]').click()
+                logging.info(f'table resource {value} connect success')
+            else:
+                logging.info(f'table resource {value} already connected')
+
     def delete_all(self) -> None:
-        tr_locators = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr').locator('//i[@class="anticon anticon-delete"]')
+        tr_locators = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr').locator(
+            '//i[@class="anticon anticon-delete"]')
         while tr_locators.count() > 0:
             tr_locators.first.click()
         logging.info('table resource all delete')
```

### Comparing `inhandtest-0.0.49/inhandtest/exception.py` & `inhandtest-0.0.50/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/file.py` & `inhandtest-0.0.50/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/inmodbus.py` & `inhandtest-0.0.50/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/inmongodb.py` & `inhandtest-0.0.50/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/inmqtt.py` & `inhandtest-0.0.50/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/inrequest.py` & `inhandtest-0.0.50/inhandtest/inrequest.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/inserial.py` & `inhandtest-0.0.50/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/insocket.py` & `inhandtest-0.0.50/inhandtest/insocket.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,124 +9,156 @@
 
 import logging
 import threading
 import time
 import socket
 
 
-def tcp_server_data(host, port, recv_content: str or list = None, connect_time=10,
-                    send_msg_to_server: str or list = None, function=None, **kwargs):
+def tcp_server_data(host, port, recv_content: dict = None, connect_time=10,
+                    send_msg_to_server: str or list = None, function=None, timeout=5, **kwargs):
     """ 开启tcp_server, 并且接收数据，对数据做验证, 该连接为阻塞式，所以要确保客户端能正常连接过来，还要确保防火墙是关闭的
         该连接使用with，所以不管是客户端还是服务端，还是在异常状态下都会正常关闭
 
-    :param host:  server地址
-    :param port:  server端口
-    :param recv_content: 判断recv_content 在接收到的内容里面 也可以不做校验
+    :param host:  server地址 ex: 10.5.24.224
+    :param port:  server端口 ex: 3001
+    :param recv_content: {('10.5.24.224', 3002): "hello world"} 判断客户端('10.5.24.224', 3002) 在接收到的内容里面是否包含"hello world",  value可以是list，判断多个内容
+                         {'content': "hello world"}, 判断连接过来的客户端在接收到的内容里面是否包含"hello world"
     :param connect_time:  服务器和客户端建立连接后，需要连接的时间
     :param send_msg_to_server: 当客户端连接成功后，已连接客户端向服务端发送的内容
     :param function: tcp_server 连接上后做的操作
+    :param timeout: 接收数据的或连接的超时时间
     :param kwargs:  function接入的参数
     :return: AssertionError or None
     """
+    all_datas = {}
+    socket.setdefaulttimeout(timeout)
 
     def client_send_msg_to_server(conn, addr, msg: str or list):
         if msg is not None:
             msg = [msg] if isinstance(msg, str) else [msg_ for msg_ in msg]
             for msg_ in msg:
                 conn.send(msg_.encode('utf-8'))
                 logging.info(f'tcp client {addr} send msg {msg_} to server {host}: {port}')
 
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:  # 使用with， 不用担心没有关闭server
         s.bind((host, port))  # 绑定服务器IP地址和端口号
         s.listen()  # 等待客户端连接
-        for i_ in range(0, 4):  # 有些端口错误的客户端会连接上来，导致收到的消息始终为空，需要过滤掉
-            client = True
-            logging.info(f'tcp server {host}:{port} start wait client connect')
-            __conn, __addr = s.accept()
-            if function is not None:
-                threading.Thread(target=function, kwargs=kwargs).start()
-            with __conn:
-                logging.info(f'tcp server {host}:{port} connect from client {__addr}')
-                datas = b''
-                now_time = int(time.time())
-                send_msg_status = False
-                while int(time.time()) <= now_time + connect_time:
-                    # 接收客户端数据
-                    recv_data = __conn.recv(1024)
-                    if not recv_data:
-                        client = False
-                        __conn.close()
-                        logging.info(f'client {__addr} is a error client')
-                        break
-                    if not send_msg_status:
-                        threading.Thread(target=client_send_msg_to_server,
-                                         args=(__conn, __addr, send_msg_to_server)).start()
-                        send_msg_status = True
-                    logging.info(f'tcp server {host}:{port} recv data {recv_data}')
-                    datas = datas + recv_data
-                    if recv_content is not None:
-                        contents = [recv_content.encode('utf-8')] if isinstance(recv_content, str) else [
-                            c_.encode('utf-8') for c_ in recv_content]
-                        # 校验数据内容
-
-                        if not list(filter(lambda x: x not in datas, contents)):
+        try:
+            for i_ in range(0, 4):  # 有些端口错误的客户端会连接上来，导致收到的消息始终为空，需要过滤掉
+                client = True
+                logging.info(f'tcp server {host}:{port} start wait client connect')
+                __conn, __addr = s.accept()
+                if function is not None:
+                    threading.Thread(target=function, kwargs=kwargs).start()
+                with __conn:
+                    logging.info(f'tcp server {host}:{port} connect from client {__addr}')
+                    datas = b''
+                    now_time = int(time.time())
+                    send_msg_status = False
+                    while int(time.time()) <= now_time + connect_time:
+                        # 接收客户端数据
+                        recv_data = __conn.recv(1024)
+                        if not recv_data:
+                            client = False
+                            __conn.close()
+                            logging.info(f'client {__addr} is a error client')
                             break
+                        if not send_msg_status:
+                            threading.Thread(target=client_send_msg_to_server,
+                                             args=(__conn, __addr, send_msg_to_server)).start()
+                            send_msg_status = True
+                        logging.info(f'tcp server {host}:{port} recv client {__addr} data {recv_data}')
+                        datas = datas + recv_data
+                        all_datas.update({__addr: datas})
+                    else:
+                        __conn.close()
+                if client:
+                    break
+        except socket.timeout:
+            logging.warning(f'tcp server {host}:{port} connect timeout or reva data timeout')
+    # 数据校验
+    if recv_content is not None:
+        if all_datas:
+            for k, v in recv_content.items():
+                if k == 'content':
+                    datas = b''.join([v_ for v_ in all_datas.values()])
+                    contents = [v.encode('utf-8')] if isinstance(v, str) else [c_.encode('utf-8') for c_ in v]
+                    # 校验数据内容
+                    if list(filter(lambda x: x not in datas, contents)):
+                        raise AssertionError(f'tcp server {host}:{port} all clients not recv  content {v}')
+                    else:
+                        logging.info(f'tcp server {host}:{port} all clients recv content {v} success')
                 else:
-                    __conn.close()
-                    if recv_content is not None:
-                        logging.error(f'recv all data is {datas}')
-                        raise AssertionError('recv data error')
-            if client:
-                break
+                    datas = all_datas.get(k)
+                    if datas is not None:
+                        contents = [v.encode('utf-8')] if isinstance(v, str) else [c_.encode('utf-8') for c_ in v]
+                        # 校验数据内容
+                        if list(filter(lambda x: x not in datas, contents)):
+                            raise AssertionError(f'tcp server {host}:{port} client {k} not recv content {v}')
+                        else:
+                            logging.info(f'tcp server {host}:{port} client {k} recv content {v} success')
+                    else:
+                        raise AssertionError(f'tcp server {host}:{port} client {k} not connected')
+        else:
+            raise AssertionError(f'tcp server {host}:{port} client not connected')
 
 
 def tcp_client_data(server: tuple, client: tuple = None, recv_content: str or list = None, connect_time=10,
-                    send_msg_to_server: str or list = None, function=None, **kwargs):
+                    send_msg_to_server: str or list = None, function=None, timeout=5, **kwargs):
     """ 开启tcp_client, 并且接收数据，对数据做验证
         该连接使用with，所以不管是客户端还是服务端，还是在异常状态下都会正常关闭
 
     :param server: ($host, $port), 客户端需要连接的服务器地址和端口，使用元组，必填('192.168.2.1', 502)
     :param client:  ($host, $port) 绑定指定地址和端口，如果为None ，本机直接开启一个， 跟server参数一样
     :param recv_content: 判断客户端 在接收到的内容里面包含recv_content 也可以不做校验
     :param connect_time:  服务器和客户端建立连接后，需要连接的时间
     :param send_msg_to_server: 当客户端连接成功后，客户端向服务端发送的内容
     :param function: 当客户端 连接上后做的操作
+    :param timeout: 接收数据的或连接的超时时间
     :param kwargs:  function接入的参数
     :return: AssertionError or None
     """
+    socket.setdefaulttimeout(timeout)
+    datas = b''
 
     def client_send_msg_to_server(client_, msg: str or list):
         if msg is not None:
             msg = [msg] if isinstance(msg, str) else [msg_ for msg_ in msg]
             for msg_ in msg:
                 client_.send(msg_.encode("utf-8"))
                 logging.info(f'tcp client send msg {msg_} to server {server}')
 
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:  # 使用with， 不用担心没有关闭server
         if client:
             s.bind(client)  # 绑定客户端IP地址和端口号
-        s.connect(server)  # 客户端连接服务端
-        threading.Thread(target=client_send_msg_to_server, args=(s, send_msg_to_server)).start()
-        threading.Thread(target=function, kwargs=kwargs).start()
-        now_time = int(time.time())
-        while int(time.time()) <= now_time + connect_time:
-            # 接收客户端数据
-            recv_data = s.recv(1024)
-            logging.info(f'tcp client recv data from server {server}: {recv_data}')
-            datas = datas + recv_data
-            if recv_content is not None:
-                contents = [recv_content.encode('utf-8')] if isinstance(recv_content, str) else [c_.encode('utf-8') for
-                                                                                                 c_ in recv_content]
-                # 校验数据内容
-                if not list(filter(lambda x: x not in datas, contents)):
-                    break
+        try:
+            s.connect(server)  # 客户端连接服务端
+            threading.Thread(target=client_send_msg_to_server, args=(s, send_msg_to_server)).start()
+            threading.Thread(target=function, kwargs=kwargs).start()
+            now_time = int(time.time())
+            while int(time.time()) <= now_time + connect_time:
+                # 接收客户端数据
+                recv_data = s.recv(1024)
+                logging.info(f'tcp client recv data from server {server}: {recv_data}')
+                datas = datas + recv_data
+                time.sleep(0.5)
+        except socket.timeout:
+            logging.warning(f'tcp client {client} connect timeout or reva data timeout')
+
+    if recv_content is not None:
+        if datas:
+            contents = [recv_content.encode('utf-8')] if isinstance(recv_content, str) else [c_.encode('utf-8') for
+                                                                                             c_ in recv_content]
+            # 校验数据内容
+            if list(filter(lambda x: x not in datas, contents)):
+                raise AssertionError(f'tcp client {client} not recv content {recv_content}')
+            else:
+                logging.info(f'tcp client {client} recv content {recv_content} success')
         else:
-            if recv_content is not None:
-                logging.error(f'recv all data is {datas}')
-                raise AssertionError('recv data error')
+            raise AssertionError(f'tcp client {client} not connected')
 
 
 def udp_server_data(host, port, recv_content: str or list = None, connect_time=10, send_msg_to_client: dict = None):
     """ 开启udp_server, 并且接收数据，对数据做验证, udp 校验数据时未区分客户端，所以保证接入时只有一个客户端
         该连接使用with，所以不管是客户端还是服务端，还是在异常状态下都会正常关闭
 
     :param host:  server地址
@@ -217,8 +249,7 @@
 
 
 if __name__ == '__main__':
     import sys
 
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
                         stream=sys.stdout)
-    # udp_server_data('10.5.24.224', 1112, send_msg_to_client=None)
```

### Comparing `inhandtest-0.0.49/inhandtest/inssh.py` & `inhandtest-0.0.50/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/mail.py` & `inhandtest-0.0.50/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/pytest_email.html` & `inhandtest-0.0.50/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/telnet.py` & `inhandtest-0.0.50/inhandtest/telnet.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.49/inhandtest/tools.py` & `inhandtest-0.0.50/inhandtest/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,17 +248,20 @@
     :param last_read_replace: 对最后一条命令读取的内容做替换
     :return:
     """
     command = [command] if isinstance(command, str) else command
     last_read_content = None
     for command_ in command:
         logging.info(f'windows cmd do {command_}')
-        p = subprocess.Popen(command_, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
-        last_read_content = p.communicate()[0].strip()
-        logging.info(last_read_content)
+        if expect is None and last_read_replace is None:
+            subprocess.Popen(command_, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
+        else:
+            p = subprocess.Popen(command_, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
+            last_read_content = p.communicate()[0].strip()
+            logging.info(last_read_content)
     if last_read_replace and last_read_content is not None:
         last_read_content = replace_str(last_read_content, last_read_replace)
     if expect is not None:
         if isinstance(expect, str):
             if expect not in last_read_content:
                 raise AssertionError(f'{expect} not in last read content')
         elif isinstance(expect, list):
@@ -289,15 +292,15 @@
 
     if svn.get("url") and svn.get('username') and svn.get('password') and file_path:
         url_path = svn.get("url")
         firmware_name = url_path.split('/')[-1]
         local_firmware_path = os.path.join(file_path, firmware_name)
         svn_hash_file_path = url_path.replace(firmware_name, 'sha256.txt')
         auth = HTTPBasicAuth(svn.get('username'), svn.get('password'))
-        if not os.path.isfile(local_firmware_path):
+        if (not os.path.isfile(local_firmware_path)) and (not os.path.exists(local_firmware_path)):
             logging.info(f"download {local_firmware_path} from svn and wait for a moment!")
             s = requests.Session()
             s.mount('http://', HTTPAdapter(max_retries=3))  # 本身请求失败会重试3次
             for i in range(3):  # 文件下载错误再继续下载
                 r = s.get(url_path, auth=auth)
                 if r.status_code == 401:
                     raise Exception("svn username or password error")
@@ -597,12 +600,11 @@
 
 
 if __name__ == '__main__':
     import sys
 
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
                         stream=sys.stdout)
-    check_windows_process('sscom', True)
     # is_installed('Google Chrome123')
     # print(windows_cmd('route delete 192.168.2.102 mask 255.255.255.255 192.168.4.2', '操作完成', {' ': '', '\n': ''}))
     # print(generate_password(length=2, lowercase=True, uppercase=True, special_chars=True, chinese_chars=True))
     # print(get_time_stamp('2022-02-18T13:39:32Z', -2))
```

### Comparing `inhandtest-0.0.49/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.50/inhandtest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.49
+Version: 0.0.50
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.49/setup.py` & `inhandtest-0.0.50/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.49',
+    version='0.0.50',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

