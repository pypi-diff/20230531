# Comparing `tmp/ProjectB_clientside_template_package-0.7.tar.gz` & `tmp/ProjectB_clientside_template_package-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjectB_clientside_template_package-0.7.tar", last modified: Wed May 31 07:35:50 2023, max compression
+gzip compressed data, was "ProjectB_clientside_template_package-0.8.tar", last modified: Wed May 31 07:45:54 2023, max compression
```

## Comparing `ProjectB_clientside_template_package-0.7.tar` & `ProjectB_clientside_template_package-0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:50.376771 ProjectB_clientside_template_package-0.7/
--rw-rw-rw-   0        0        0      489 2023-05-31 07:35:50.375594 ProjectB_clientside_template_package-0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:50.302678 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:50.340319 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/ClientSocketControl/
--rw-rw-rw-   0        0        0      840 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py
--rw-rw-rw-   0        0        0     3670 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py
--rw-rw-rw-   0        0        0     3945 2023-05-31 07:34:07.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/MainController.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:50.359796 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/
--rw-rw-rw-   0        0        0     2403 2023-05-30 02:37:11.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/Order.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:50.371758 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/
--rw-rw-rw-   0        0        0      162 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Action.py
--rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Direction.py
--rw-rw-rw-   0        0        0      161 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/ExpiryDate.py
--rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/StrikePrice.py
--rw-rw-rw-   0        0        0      365 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/Profile.py
--rw-rw-rw-   0        0        0     2037 2023-05-30 02:36:48.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/TradeController.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:50.331370 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package.egg-info/
--rw-rw-rw-   0        0        0      489 2023-05-31 07:35:50.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      981 2023-05-31 07:35:50.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 07:35:50.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-31 07:35:50.000000 ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      526 2023-05-31 07:35:15.000000 ProjectB_clientside_template_package-0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 07:35:50.377969 ProjectB_clientside_template_package-0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 07:45:54.032586 ProjectB_clientside_template_package-0.8/
+-rw-rw-rw-   0        0        0      489 2023-05-31 07:45:54.031520 ProjectB_clientside_template_package-0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 07:45:54.001767 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:45:54.012839 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/ClientSocketControl/
+-rw-rw-rw-   0        0        0      840 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py
+-rw-rw-rw-   0        0        0     3670 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py
+-rw-rw-rw-   0        0        0     3943 2023-05-31 07:45:14.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/MainController.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:45:54.020516 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/TradeControl/
+-rw-rw-rw-   0        0        0     2403 2023-05-30 02:37:11.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/TradeControl/Order.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:45:54.029223 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/
+-rw-rw-rw-   0        0        0      162 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Action.py
+-rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Direction.py
+-rw-rw-rw-   0        0        0      161 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/ExpiryDate.py
+-rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/StrikePrice.py
+-rw-rw-rw-   0        0        0      365 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/TradeControl/Profile.py
+-rw-rw-rw-   0        0        0     2037 2023-05-30 02:36:48.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/TradeControl/TradeController.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:45:54.010940 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package.egg-info/
+-rw-rw-rw-   0        0        0      489 2023-05-31 07:45:53.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2023-05-31 07:45:53.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:45:53.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-31 07:45:53.000000 ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      526 2023-05-31 07:45:29.000000 ProjectB_clientside_template_package-0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:45:54.032586 ProjectB_clientside_template_package-0.8/setup.cfg
```

### Comparing `ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py` & `ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py` & `ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/MainController.py` & `ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/MainController.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import json
 
 class MainController(ABC):
     
     dataStreaming = None
     dataStreamingRequest = None
-    tradeController = None
+    tradeController = TradeController()
     
     def login(self, loginname, password):
         try:
             self.dataStreaming = SocketClient(loginname, password)
         except:
             self.dataStreaming = None
             raise Exception("Login fail")
@@ -52,20 +52,19 @@
                 "enddate":enddate,
                 "starttime":starttime,
                 "endtime":endtime,
                 "interval":int(interval),
             }
             self.dataStreaming.request(dataStreamingRequest)
             
-    def projectBTradeController(slippageRangeInPercentage):
-        tradeController = TradeController()
-        tradeController.setSlippage(0.0005)
+    def projectBTradeController(self, slippageRangeInPercentage):
+        self.tradeController.setSlippage(slippageRangeInPercentage)
     
     @abstractmethod
-    def logicHandler(datastructure:DataStructure):
+    def logicHandler(self, datastructure:DataStructure):
         pass
         
     def run(self):
         while True:
             #get the response
             response = self.dataStreaming.getResponse()
             if response:
@@ -91,8 +90,7 @@
                 '''
                 
                 self.logicHandler(dataStructure)
                 
                 '''
                 <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
                 '''
-
```

### Comparing `ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/Order.py` & `ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/TradeControl/Order.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package/TradeControl/TradeController.py` & `ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package/TradeControl/TradeController.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.7/ProjectB_clientside_template_package.egg-info/SOURCES.txt` & `ProjectB_clientside_template_package-0.8/ProjectB_clientside_template_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.7/pyproject.toml` & `ProjectB_clientside_template_package-0.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ProjectB_clientside_template_package"
-version = "0.7"
+version = "0.8"
 authors = [
   { name="ProjectB", email="admin@projectb.click" },
 ]
 description = "This is the pip package of ProjectB_clientside_template_package"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

