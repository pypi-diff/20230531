# Comparing `tmp/ProjectB_clientside_template_package-0.6.tar.gz` & `tmp/ProjectB_clientside_template_package-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjectB_clientside_template_package-0.6.tar", last modified: Wed May 31 07:31:45 2023, max compression
+gzip compressed data, was "ProjectB_clientside_template_package-0.7.tar", last modified: Wed May 31 07:35:50 2023, max compression
```

## Comparing `ProjectB_clientside_template_package-0.6.tar` & `ProjectB_clientside_template_package-0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 07:31:45.267501 ProjectB_clientside_template_package-0.6/
--rw-rw-rw-   0        0        0      489 2023-05-31 07:31:45.265257 ProjectB_clientside_template_package-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-31 07:31:45.228676 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:31:45.245086 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/ClientSocketControl/
--rw-rw-rw-   0        0        0      840 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py
--rw-rw-rw-   0        0        0     3670 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py
--rw-rw-rw-   0        0        0     3931 2023-05-31 07:24:39.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/MainController.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:31:45.254134 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/
--rw-rw-rw-   0        0        0     2403 2023-05-30 02:37:11.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/Order.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:31:45.263179 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/
--rw-rw-rw-   0        0        0      162 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Action.py
--rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Direction.py
--rw-rw-rw-   0        0        0      161 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/ExpiryDate.py
--rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/StrikePrice.py
--rw-rw-rw-   0        0        0      365 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/Profile.py
--rw-rw-rw-   0        0        0     2037 2023-05-30 02:36:48.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/TradeController.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:31:45.241082 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package.egg-info/
--rw-rw-rw-   0        0        0      489 2023-05-31 07:31:45.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      981 2023-05-31 07:31:45.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 07:31:45.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-31 07:31:45.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      526 2023-05-31 07:31:20.000000 ProjectB_clientside_template_package-0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 07:31:45.267501 ProjectB_clientside_template_package-0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:50.376771 ProjectB_clientside_template_package-0.7/
+-rw-rw-rw-   0        0        0      489 2023-05-31 07:35:50.375594 ProjectB_clientside_template_package-0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:50.302678 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:50.340319 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/ClientSocketControl/
+-rw-rw-rw-   0        0        0      840 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py
+-rw-rw-rw-   0        0        0     3670 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py
+-rw-rw-rw-   0        0        0     3945 2023-05-31 07:34:07.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/MainController.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:50.359796 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/
+-rw-rw-rw-   0        0        0     2403 2023-05-30 02:37:11.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/Order.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:50.371758 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/
+-rw-rw-rw-   0        0        0      162 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Action.py
+-rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Direction.py
+-rw-rw-rw-   0        0        0      161 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/ExpiryDate.py
+-rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/StrikePrice.py
+-rw-rw-rw-   0        0        0      365 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/Profile.py
+-rw-rw-rw-   0        0        0     2037 2023-05-30 02:36:48.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/TradeController.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:50.331370 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package.egg-info/
+-rw-rw-rw-   0        0        0      489 2023-05-31 07:35:50.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2023-05-31 07:35:50.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:35:50.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-31 07:35:50.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      526 2023-05-31 07:35:15.000000 ProjectB_clientside_template_package-0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:35:50.377969 ProjectB_clientside_template_package-0.7/setup.cfg
```

### Comparing `ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py` & `ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py` & `ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/MainController.py` & `ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/MainController.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-import datetime
+from datetime import datetime
 from ProjectB_clientside_template_package.ClientSocketControl.SocketClient import SocketClient
 from ProjectB_clientside_template_package.ClientSocketControl.DataStructure import DataStructure
 from ProjectB_clientside_template_package.TradeControl.OrderActionConstants.Action import Action
 from ProjectB_clientside_template_package.TradeControl.TradeController import TradeController
 
 import json
```

### Comparing `ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/Order.py` & `ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/Order.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/TradeController.py` & `ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/TradeController.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package.egg-info/SOURCES.txt` & `ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.6/pyproject.toml` & `ProjectB_clientside_template_package-0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ProjectB_clientside_template_package"
-version = "0.6"
+version = "0.7"
 authors = [
   { name="ProjectB", email="admin@projectb.click" },
 ]
 description = "This is the pip package of ProjectB_clientside_template_package"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

