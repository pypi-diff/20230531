# Comparing `tmp/ProjectB_clientside_template_package-0.5.tar.gz` & `tmp/ProjectB_clientside_template_package-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjectB_clientside_template_package-0.5.tar", last modified: Tue May 30 02:38:14 2023, max compression
+gzip compressed data, was "ProjectB_clientside_template_package-0.6.tar", last modified: Wed May 31 07:31:45 2023, max compression
```

## Comparing `ProjectB_clientside_template_package-0.5.tar` & `ProjectB_clientside_template_package-0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 02:38:14.208033 ProjectB_clientside_template_package-0.5/
--rw-rw-rw-   0        0        0      489 2023-05-30 02:38:14.207033 ProjectB_clientside_template_package-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 02:38:14.171531 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/
-drwxrwxrwx   0        0        0        0 2023-05-30 02:38:14.189433 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/ClientSocketControl/
--rw-rw-rw-   0        0        0      840 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py
--rw-rw-rw-   0        0        0     3670 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py
--rw-rw-rw-   0        0        0     4129 2023-05-30 02:27:12.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/MainController.py
-drwxrwxrwx   0        0        0        0 2023-05-30 02:38:14.195963 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/
--rw-rw-rw-   0        0        0     2403 2023-05-30 02:37:11.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/Order.py
-drwxrwxrwx   0        0        0        0 2023-05-30 02:38:14.204023 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/
--rw-rw-rw-   0        0        0      162 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Action.py
--rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Direction.py
--rw-rw-rw-   0        0        0      161 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/ExpiryDate.py
--rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/StrikePrice.py
--rw-rw-rw-   0        0        0      365 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/Profile.py
--rw-rw-rw-   0        0        0     2037 2023-05-30 02:36:48.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/TradeController.py
-drwxrwxrwx   0        0        0        0 2023-05-30 02:38:14.184935 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package.egg-info/
--rw-rw-rw-   0        0        0      489 2023-05-30 02:38:14.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      981 2023-05-30 02:38:14.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 02:38:14.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-30 02:38:14.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      526 2023-05-30 02:37:38.000000 ProjectB_clientside_template_package-0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 02:38:14.209032 ProjectB_clientside_template_package-0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 07:31:45.267501 ProjectB_clientside_template_package-0.6/
+-rw-rw-rw-   0        0        0      489 2023-05-31 07:31:45.265257 ProjectB_clientside_template_package-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 07:31:45.228676 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:31:45.245086 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/ClientSocketControl/
+-rw-rw-rw-   0        0        0      840 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py
+-rw-rw-rw-   0        0        0     3670 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py
+-rw-rw-rw-   0        0        0     3931 2023-05-31 07:24:39.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/MainController.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:31:45.254134 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/
+-rw-rw-rw-   0        0        0     2403 2023-05-30 02:37:11.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/Order.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:31:45.263179 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/
+-rw-rw-rw-   0        0        0      162 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Action.py
+-rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Direction.py
+-rw-rw-rw-   0        0        0      161 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/ExpiryDate.py
+-rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/StrikePrice.py
+-rw-rw-rw-   0        0        0      365 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/Profile.py
+-rw-rw-rw-   0        0        0     2037 2023-05-30 02:36:48.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/TradeController.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:31:45.241082 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package.egg-info/
+-rw-rw-rw-   0        0        0      489 2023-05-31 07:31:45.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2023-05-31 07:31:45.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:31:45.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-31 07:31:45.000000 ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      526 2023-05-31 07:31:20.000000 ProjectB_clientside_template_package-0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:31:45.267501 ProjectB_clientside_template_package-0.6/setup.cfg
```

### Comparing `ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py` & `ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py` & `ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/MainController.py` & `ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/MainController.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,42 +16,46 @@
     def login(self, loginname, password):
         try:
             self.dataStreaming = SocketClient(loginname, password)
         except:
             self.dataStreaming = None
             raise Exception("Login fail")
     
-    def createDataStreamingRequest(self, activity:str, market:str, index:str, startdate:datetime, enddate:datetime, starttime:datetime, endtime:datetime, interval:int):
+    def createDataStreamingRequest(self, activity:str, market:str, index:str, startdate:str, enddate:str, starttime:str, endtime:str, interval:int):
         if(self.dataStreaming is None):
-            raise Exception("Please login first");
+            raise Exception("Please login first")
         else:
             try:
-                datetime.datetime(int(startdate.strftime('%Y')),int(startdate.strftime('%m')),int(startdate.strftime('%d')))
+                date_format = '%Y%m%d'
+                datetime.strptime(startdate, date_format)
             except ValueError:
                 raise Exception("startdate invaild")
             try:
-                datetime.datetime(int(enddate.strftime('%Y')),int(enddate.strftime('%m')),int(enddate.strftime('%d')))
+                date_format = '%Y%m%d'
+                datetime.strptime(enddate, date_format)
             except ValueError:
                 raise Exception("enddate invaild")
             try:
-                datetime.datetime(int(starttime.strftime('%H')),int(starttime.strftime('%M')),int(starttime.strftime('%S')))
+                date_format = '%H%M%S'
+                datetime.strptime(starttime, date_format)
             except ValueError:
                 raise Exception("starttime invaild")
             try:
-                datetime.datetime(int(endtime.strftime('%H')),int(endtime.strftime('%M')),int(endtime.strftime('%S')))
+                date_format = '%H%M%S'
+                datetime.strptime(endtime, date_format)
             except ValueError:
                 raise Exception("endtime invaild")
             dataStreamingRequest = {
                 "activity":activity,
                 "market":market,
                 "index":index,
-                "startdate":startdate.strftime('%Y%m%d'),
-                "enddate":enddate.strftime('%Y%m%d'),
-                "starttime":starttime.strftime('%H%M%S'),
-                "endtime":endtime.strftime('%H%M%S'),
+                "startdate":startdate,
+                "enddate":enddate,
+                "starttime":starttime,
+                "endtime":endtime,
                 "interval":int(interval),
             }
             self.dataStreaming.request(dataStreamingRequest)
             
     def projectBTradeController(slippageRangeInPercentage):
         tradeController = TradeController()
         tradeController.setSlippage(0.0005)
@@ -82,13 +86,13 @@
                 self.tradeController.tradeCheckingAndBalanceUpdate(dataStructure)
                 
                 '''
                 You may write your back test program below within the while loop
                 >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
                 '''
                 
-                self.logicHandler(dataStructure);
+                self.logicHandler(dataStructure)
                 
                 '''
                 <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
                 '''
```

### Comparing `ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/Order.py` & `ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/Order.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/TradeController.py` & `ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package/TradeControl/TradeController.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package.egg-info/SOURCES.txt` & `ProjectB_clientside_template_package-0.6/ProjectB_clientside_template_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.5/pyproject.toml` & `ProjectB_clientside_template_package-0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ProjectB_clientside_template_package"
-version = "0.5"
+version = "0.6"
 authors = [
   { name="ProjectB", email="admin@projectb.click" },
 ]
 description = "This is the pip package of ProjectB_clientside_template_package"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

