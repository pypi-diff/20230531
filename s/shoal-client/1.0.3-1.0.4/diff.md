# Comparing `tmp/shoal-client-1.0.3.tar.gz` & `tmp/shoal-client-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/hepuser/colsond/projects/shoal/shoal-client/dist/tmp3p3hmfzv/shoal-client-1.0.3.tar", last modified: Fri Apr 28 17:52:39 2023, max compression
+gzip compressed data, was "/hepuser/colsond/projects/shoal/shoal-client/dist/tmpycejgq3g/shoal-client-1.0.4.tar", last modified: Wed May 31 21:39:39 2023, max compression
```

## Comparing `shoal-client-1.0.3.tar` & `shoal-client-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 colsond  (115344) hep      (34244)        0 2023-04-28 17:52:39.000000 shoal-client-1.0.3/
-drwxr-xr-x   0 colsond  (115344) hep      (34244)        0 2023-04-28 17:52:39.000000 shoal-client-1.0.3/shoal_client.egg-info/
--rw-r--r--   0 colsond  (115344) hep      (34244)       13 2023-04-28 17:52:38.000000 shoal-client-1.0.3/shoal_client.egg-info/top_level.txt
--rw-r--r--   0 colsond  (115344) hep      (34244)       34 2023-04-28 17:52:38.000000 shoal-client-1.0.3/shoal_client.egg-info/requires.txt
--rw-r--r--   0 colsond  (115344) hep      (34244)        1 2023-04-28 17:52:38.000000 shoal-client-1.0.3/shoal_client.egg-info/dependency_links.txt
--rw-r--r--   0 colsond  (115344) hep      (34244)      321 2023-04-28 17:52:38.000000 shoal-client-1.0.3/shoal_client.egg-info/SOURCES.txt
--rw-r--r--   0 colsond  (115344) hep      (34244)     4090 2023-04-28 17:52:38.000000 shoal-client-1.0.3/shoal_client.egg-info/PKG-INFO
-drwxr-xr-x   0 colsond  (115344) hep      (34244)        0 2023-04-28 17:52:39.000000 shoal-client-1.0.3/shoal_client/
--rw-r--r--   0 colsond  (115344) hep      (34244)        0 2023-04-20 18:14:31.000000 shoal-client-1.0.3/shoal_client/__init__.py
--rw-r--r--   0 colsond  (115344) hep      (34244)     3484 2023-04-20 18:14:31.000000 shoal-client-1.0.3/shoal_client/config.py
--rw-r--r--   0 colsond  (115344) hep      (34244)       18 2023-04-28 17:38:17.000000 shoal-client-1.0.3/shoal_client/__version__.py
--rw-r--r--   0 colsond  (115344) hep      (34244)     1346 2023-04-20 18:14:31.000000 shoal-client-1.0.3/setup.py
--rw-r--r--   0 colsond  (115344) hep      (34244)     4090 2023-04-28 17:52:39.000000 shoal-client-1.0.3/PKG-INFO
--rw-r--r--   0 colsond  (115344) hep      (34244)       38 2023-04-28 17:52:39.000000 shoal-client-1.0.3/setup.cfg
-drwxr-xr-x   0 colsond  (115344) hep      (34244)        0 2023-04-28 17:52:39.000000 shoal-client-1.0.3/conf/
--rw-r--r--   0 colsond  (115344) hep      (34244)      609 2023-04-20 18:14:31.000000 shoal-client-1.0.3/conf/shoal_client.conf
--rwxr-xr-x   0 colsond  (115344) hep      (34244)    18651 2023-04-26 18:08:03.000000 shoal-client-1.0.3/shoal-client
--rw-r--r--   0 colsond  (115344) hep      (34244)     3645 2023-04-20 18:14:31.000000 shoal-client-1.0.3/README.md
--rw-r--r--   0 colsond  (115344) hep      (34244)       25 2023-04-20 18:14:31.000000 shoal-client-1.0.3/MANIFEST.in
+drwxr-xr-x   0 colsond  (115344) hep      (34244)        0 2023-05-31 21:39:39.000000 shoal-client-1.0.4/
+-rwxr-xr-x   0 colsond  (115344) hep      (34244)    19652 2023-05-31 17:44:56.000000 shoal-client-1.0.4/shoal-client
+-rw-r--r--   0 colsond  (115344) hep      (34244)       25 2023-04-20 18:14:31.000000 shoal-client-1.0.4/MANIFEST.in
+-rw-r--r--   0 colsond  (115344) hep      (34244)     4383 2023-05-31 21:39:39.000000 shoal-client-1.0.4/PKG-INFO
+-rw-r--r--   0 colsond  (115344) hep      (34244)     3938 2023-05-30 16:37:51.000000 shoal-client-1.0.4/README.md
+-rw-r--r--   0 colsond  (115344) hep      (34244)     1346 2023-04-20 18:14:31.000000 shoal-client-1.0.4/setup.py
+drwxr-xr-x   0 colsond  (115344) hep      (34244)        0 2023-05-31 21:39:39.000000 shoal-client-1.0.4/shoal_client/
+-rw-r--r--   0 colsond  (115344) hep      (34244)       18 2023-05-31 21:08:47.000000 shoal-client-1.0.4/shoal_client/__version__.py
+-rw-r--r--   0 colsond  (115344) hep      (34244)     3484 2023-04-20 18:14:31.000000 shoal-client-1.0.4/shoal_client/config.py
+-rw-r--r--   0 colsond  (115344) hep      (34244)        0 2023-04-20 18:14:31.000000 shoal-client-1.0.4/shoal_client/__init__.py
+-rw-r--r--   0 colsond  (115344) hep      (34244)       38 2023-05-31 21:39:39.000000 shoal-client-1.0.4/setup.cfg
+drwxr-xr-x   0 colsond  (115344) hep      (34244)        0 2023-05-31 21:39:39.000000 shoal-client-1.0.4/conf/
+-rw-r--r--   0 colsond  (115344) hep      (34244)      609 2023-04-20 18:14:31.000000 shoal-client-1.0.4/conf/shoal_client.conf
+drwxr-xr-x   0 colsond  (115344) hep      (34244)        0 2023-05-31 21:39:39.000000 shoal-client-1.0.4/shoal_client.egg-info/
+-rw-r--r--   0 colsond  (115344) hep      (34244)       34 2023-05-31 21:39:39.000000 shoal-client-1.0.4/shoal_client.egg-info/requires.txt
+-rw-r--r--   0 colsond  (115344) hep      (34244)       13 2023-05-31 21:39:39.000000 shoal-client-1.0.4/shoal_client.egg-info/top_level.txt
+-rw-r--r--   0 colsond  (115344) hep      (34244)        1 2023-05-31 21:39:39.000000 shoal-client-1.0.4/shoal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 colsond  (115344) hep      (34244)     4383 2023-05-31 21:39:39.000000 shoal-client-1.0.4/shoal_client.egg-info/PKG-INFO
+-rw-r--r--   0 colsond  (115344) hep      (34244)      321 2023-05-31 21:39:39.000000 shoal-client-1.0.4/shoal_client.egg-info/SOURCES.txt
```

### Comparing `shoal-client-1.0.3/shoal_client.egg-info/PKG-INFO` & `shoal-client-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: shoal-client
-Version: 1.0.3
+Version: 1.0.4
 Summary: A squid cache publishing and advertising tool designed to work in fast changing environments
 Home-page: http://github.com/hep-gc/shoal
 Author: Mike Chester, Colson Drimiel, Ian Gable, Alex Lam, Rob Prior, Ryan Taylor, Steve Traylen, Marcus Ebert, Da Meng
 Author-email: heprc-shoal@uvic.ca
 License: 'GPL3' or 'Apache 2'
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Shoal Client README
-# Version: v1.0.1
 
 shoal-client will configure cvmfs to use the closest squid server to you by contacting the shoal server
 and using cvmfs-talk to update the active proxy configuration.
 
 shoal-client is a simple python script typically configured to run with cron to check for new squids 
 periodically. Before setting the cronjob in place make sure that shoal-client is
 configured correctly (see Usage below).
@@ -29,15 +28,15 @@
 **Note**: Requires Python 2.4+
 
 **Note**: Shoal config files will be located either at `~/.shoal/` or `/etc/shoal/` if installed 
 root permissions.
 
 ### Recommended Instalation Method: Use pip
 
-1. `pip install shoal-client`
+1. `sudo python3 -m pip install shoal-client` or, if using an old python2 version of pip: `pip install shoal-client`
 2. Copy the configuration file to proper location
     ```
     # For python3
     cp /usr/local/share/shoal-client/shoal_client.conf /etc/shoal/
     
     # For python2
     cp /usr/share/shoal-client/shoal_client.conf /etc/shoal/
@@ -65,16 +64,17 @@
     (serverurl=http://PresetServer.ca:3128)(proxyurl=http://PROXY.FROM.SHOAL.1:3128)(proxyurl=http://PROXY.FROM.SHOAL.2:3128)
 
 ### Flags and Options
 | Option | Description |
 | --- | --- |
 | -d or --dump | Print closest proxies to terminal for testing or debugging. |
 | -s `hostname` or --server `hostname`| Specifies URL of the desired shoal-server to contact. Takes precedence over the option in config file. |
-| -n `int` or --squids `int` | Specifies the number of squids to retrieve from the shoal-server |
-| -f or --frontier| Outputs a string appropriate for use as the frontier proxy enviroment variable instead of using cvmfs-talk to update the active proxy configuration|
+| -n `int` or --squids `int` | Specifies the number of squids to retrieve from the shoal-server. |
+| -f or --frontier | Outputs a string appropriate for use as the frontier proxy enviroment variable instead of using cvmfs-talk to update the active proxy configuration. |
+| -k or --skip-broadcast | Skips waiting to hear from a shoal-agent on the local network and goes directly to the shoal server for a squid. Only reccomended when you know there is no squid//agent on the local network. |
 
 Shoal client now uses the cvmfs_talk protocol. To view the list of returned squids issue:
 
      cvmfs_talk proxy info
 
 ## Other Installation Methods
```

### Comparing `shoal-client-1.0.3/shoal_client/config.py` & `shoal-client-1.0.4/shoal_client/config.py`

 * *Files identical despite different names*

### Comparing `shoal-client-1.0.3/setup.py` & `shoal-client-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `shoal-client-1.0.3/PKG-INFO` & `shoal-client-1.0.4/shoal_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: shoal-client
-Version: 1.0.3
+Version: 1.0.4
 Summary: A squid cache publishing and advertising tool designed to work in fast changing environments
 Home-page: http://github.com/hep-gc/shoal
 Author: Mike Chester, Colson Drimiel, Ian Gable, Alex Lam, Rob Prior, Ryan Taylor, Steve Traylen, Marcus Ebert, Da Meng
 Author-email: heprc-shoal@uvic.ca
 License: 'GPL3' or 'Apache 2'
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Shoal Client README
-# Version: v1.0.1
 
 shoal-client will configure cvmfs to use the closest squid server to you by contacting the shoal server
 and using cvmfs-talk to update the active proxy configuration.
 
 shoal-client is a simple python script typically configured to run with cron to check for new squids 
 periodically. Before setting the cronjob in place make sure that shoal-client is
 configured correctly (see Usage below).
@@ -29,15 +28,15 @@
 **Note**: Requires Python 2.4+
 
 **Note**: Shoal config files will be located either at `~/.shoal/` or `/etc/shoal/` if installed 
 root permissions.
 
 ### Recommended Instalation Method: Use pip
 
-1. `pip install shoal-client`
+1. `sudo python3 -m pip install shoal-client` or, if using an old python2 version of pip: `pip install shoal-client`
 2. Copy the configuration file to proper location
     ```
     # For python3
     cp /usr/local/share/shoal-client/shoal_client.conf /etc/shoal/
     
     # For python2
     cp /usr/share/shoal-client/shoal_client.conf /etc/shoal/
@@ -65,16 +64,17 @@
     (serverurl=http://PresetServer.ca:3128)(proxyurl=http://PROXY.FROM.SHOAL.1:3128)(proxyurl=http://PROXY.FROM.SHOAL.2:3128)
 
 ### Flags and Options
 | Option | Description |
 | --- | --- |
 | -d or --dump | Print closest proxies to terminal for testing or debugging. |
 | -s `hostname` or --server `hostname`| Specifies URL of the desired shoal-server to contact. Takes precedence over the option in config file. |
-| -n `int` or --squids `int` | Specifies the number of squids to retrieve from the shoal-server |
-| -f or --frontier| Outputs a string appropriate for use as the frontier proxy enviroment variable instead of using cvmfs-talk to update the active proxy configuration|
+| -n `int` or --squids `int` | Specifies the number of squids to retrieve from the shoal-server. |
+| -f or --frontier | Outputs a string appropriate for use as the frontier proxy enviroment variable instead of using cvmfs-talk to update the active proxy configuration. |
+| -k or --skip-broadcast | Skips waiting to hear from a shoal-agent on the local network and goes directly to the shoal server for a squid. Only reccomended when you know there is no squid//agent on the local network. |
 
 Shoal client now uses the cvmfs_talk protocol. To view the list of returned squids issue:
 
      cvmfs_talk proxy info
 
 ## Other Installation Methods
```

### Comparing `shoal-client-1.0.3/conf/shoal_client.conf` & `shoal-client-1.0.4/conf/shoal_client.conf`

 * *Files identical despite different names*

### Comparing `shoal-client-1.0.3/shoal-client` & `shoal-client-1.0.4/shoal-client`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 skip_broadcast = False
 best_http_proxy = ''
 env_proxy = ''
 unicode = str
 broadcast_timeout = 90
 shoal_server_timeout = 30
 paths = config.paths
+force_server = False
 
 def get_local_squid(q, t):
     PORT = 50000
     BROADCAST_ID = "fna349fn" #to make sure we don't confuse or get confused by other programs
 
     from socket import socket, AF_INET, SOCK_DGRAM
     
@@ -74,14 +75,15 @@
         gets server and dump variables from command line arguments
     """
     global server
     global dump
     global frontier
     global numsquids
     global skip_broadcast
+    global force_server
 
     p = OptionParser()
     p.add_option("-s", "--server", action="store", type="string", dest="server",
                  help="Also needs string for specifying the shoal server to use. " +
                  "Takes precedence over the option in config file.")
     p.add_option("-d", "--dump", action="store_true", dest="dump",
                  help="Print closest proxies to terminal for debugging "+
@@ -91,26 +93,31 @@
                  "instead of executing a cvfms-talk command to update the active configuration.")
     p.add_option("-n", "--squids", action="store", type="int", dest="numsquids",
                  help="Specifies the number of squids to retrieve" +
                  "from the shoal-server (default is 2).")
     p.add_option("-k", "--skip-broadcast", action="store_true",  dest="skip_broadcast",
                  help="Tells the shoal client to skip waiting for a local squid broadcast" +
                  "signal to avoid a fruitless timeout.")
+    p.add_option("-o", "--force-server", action="store_true",  dest="force_server",
+                 help="Forces the shoal client to contact the shoal server for additional squids" +
+                 "even if a local one is found via broadcast.")
     (options, args) = p.parse_args()
 
     if options.server:
         server = options.server
     if options.dump:
         dump = True
     if options.frontier:
         frontier = True
     if options.numsquids:
         numsquids = options.numsquids
     if options.skip_broadcast:
         skip_broadcast = True
+    if options.force_server:
+        force_server = True
 
 def convertServerData(val):
     """
         converts val to digits if it's not already or else return None
     """
     if val.isdigit():
         return int(val)
@@ -308,53 +315,60 @@
         "Enviroment Variable located, adding: %s as default proxy" % env_proxy)
     if env_proxy != "":
         env_proxy += ";"
 
 except KeyError as e:
     syslog.syslog(syslog.LOG_ERR, "No HTTP_PROXY enviroment variable found")
 
-## read server data (if it can be read) into a dictionary called data
-try:
-    #if there is a bad proxy set we will never reach shoal-server
-    #this goes direct to avoid any bad configuration
-    proxy_handler = UrlRequest.ProxyHandler({})
-    opener = UrlRequest.build_opener(proxy_handler)
-    if server[-1] == "/":
-        server_url = server + "%s/" % (numsquids + 5)
-    else:
-        server_url = server + "/%s/" % (numsquids + 5)
-    f = opener.open(server_url, timeout=shoal_server_timeout)
-    # data = json.loads(f.read())
-    data = parseServerData(f.read())
-    syslog.syslog(syslog.LOG_DEBUG, "Got data from %s" % server)
-except (UrlError, ValueError, socket.timeout) as e:
-    # This is where the client now exits if it can't reach shoal, might be worth
-    # refactoring instead of injecting code here to reuse the proceeding code.
-    #checkEnvVariable()
-    #checkConfig()
-    syslog.syslog(syslog.LOG_ERR, "Unable to reach shoal-server, reverting to defaults")
-    #sys.exit(1)
-except Exception as ex:
-    syslog.syslog(syslog.LOG_ERR, "Encountered unknown exception during request to shoal-server:")
-    syslog.syslog(syslog.LOG_ERR, "%s" % ex)
-    syslog.syslog(syslog.LOG_ERR, "Continuing with defaults...")    
-
-
-if not frontier and not skip_broadcast:
+# Listen on local network for a local squid agent broadcast
+if not skip_broadcast:
     q = Queue()
     p = Process(target=get_local_squid, args=(q,broadcast_timeout))
     p.start()
     try:
        local_squid = q.get(block=True, timeout=broadcast_timeout)
     except Q.Empty:
        #continue
        #print("queue timeout !")
        pass
     p.join()
 
+
+## read server data (if it can be read) into a dictionary called data
+# by default the server is only contacted if the force server flag is set or
+# no squid was found via local broadcast
+if local_squid is None or force_server:
+    try:
+        #if there is a bad proxy set we will never reach shoal-server
+        #this goes direct to avoid any bad configuration
+        proxy_handler = UrlRequest.ProxyHandler({})
+        opener = UrlRequest.build_opener(proxy_handler)
+        if server[-1] == "/":
+            server_url = server + "%s/" % (numsquids + 5)
+        else:
+            server_url = server + "/%s/" % (numsquids + 5)
+        f = opener.open(server_url, timeout=shoal_server_timeout)
+        # data = json.loads(f.read())
+        data = parseServerData(f.read())
+        syslog.syslog(syslog.LOG_DEBUG, "Got data from %s" % server)
+    except (UrlError, ValueError, socket.timeout) as e:
+        # This is where the client now exits if it can't reach shoal, might be worth
+        # refactoring instead of injecting code here to reuse the proceeding code.
+        #checkEnvVariable()
+        #checkConfig()
+        syslog.syslog(syslog.LOG_ERR, "Unable to reach shoal-server, reverting to defaults")
+        #sys.exit(1)
+    except Exception as ex:
+        syslog.syslog(syslog.LOG_ERR, "Encountered unknown exception during request to shoal-server:")
+        syslog.syslog(syslog.LOG_ERR, "%s" % ex)
+        syslog.syslog(syslog.LOG_ERR, "Continuing with defaults...")    
+
+
+
+
 # If the shoal_server was reachable
 ## iterate through the data dict and use all hostname and squid_port keys
 ## to create addresses for squids in best_http_proxy
 # syslog.syslog(syslog.LOG_INFO, "Received data from server, processing.")
 
 if data:
     for squid_key in list(data):
@@ -396,27 +410,33 @@
 default_http_proxy = temp_default_http
 
 #need to reformat default string for frontier nodes
 if frontier:
     new_defaults = ''
     tmpproxies = default_http_proxy.split(';')
     for proxy in tmpproxies:
-        if proxy != 'DIRECT':
+        if proxy != 'DIRECT' and proxy != "":
             new_defaults += '(proxyurl=%s)' % proxy
     default_http_proxy = new_defaults
 
 if local_squid:
-    best_http_proxy = "http://" + local_squid + ";" + best_http_proxy
+    if frontier:
+        best_http_proxy = "(proxyurl=http://" + local_squid + ")" + best_http_proxy
+    else:
+        best_http_proxy = "http://" + local_squid + ";" + best_http_proxy
+
 cvmfs_http_proxy = "\"" + best_http_proxy + default_http_proxy + "\""
 syslog.syslog(syslog.LOG_DEBUG, "Data parsing complete.")
 
 if dump:
     if not frontier:
         cvmfs_http_proxy = "\"" + best_http_proxy + env_proxy + default_http_proxy + "\""
     syslog.syslog(syslog.LOG_INFO, "Dumping proxy string")
+    if cvmfs_http_proxy[-2] == ";":
+        cvmfs_http_proxy = cvmfs_http_proxy[0:-2] + '"'
     print(cvmfs_http_proxy)
 
 elif frontier:
     #retrieve frontier env variable and insert new squids
     try:
         frontier_var = os.getenv("FRONTIER_SERVER", "")
     except:
@@ -431,14 +451,17 @@
     if replacements == 0:
         frontier_output = frontier_output + best_http_proxy + default_http_proxy
     print(frontier_output)
 
 else:
     # include the case that the client is unable to connect to the shoal_server
     cvmfs_http_proxy = best_http_proxy + env_proxy + default_http_proxy
+    # check for trailing semicolon
+    if cvmfs_http_proxy[-2] == ";":
+        cvmfs_http_proxy = cvmfs_http_proxy[0:-2] + '"'
     syslog.syslog(syslog.LOG_DEBUG, "Data parsing complete.")
     syslog.syslog(syslog.LOG_INFO, "Setting %s as proxy" % cvmfs_http_proxy)
 
     syslog.syslog(syslog.LOG_DEBUG, "Executing 'cvmfs_talk proxy set %s'" % cvmfs_http_proxy)
     try:
         p = Popen(["cvmfs_talk", "proxy", "set", cvmfs_http_proxy], stdout=PIPE, stderr=PIPE)
         output, errors = p.communicate()
```

### Comparing `shoal-client-1.0.3/README.md` & `shoal-client-1.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Shoal Client README
-# Version: v1.0.1
 
 shoal-client will configure cvmfs to use the closest squid server to you by contacting the shoal server
 and using cvmfs-talk to update the active proxy configuration.
 
 shoal-client is a simple python script typically configured to run with cron to check for new squids 
 periodically. Before setting the cronjob in place make sure that shoal-client is
 configured correctly (see Usage below).
@@ -18,15 +17,15 @@
 **Note**: Requires Python 2.4+
 
 **Note**: Shoal config files will be located either at `~/.shoal/` or `/etc/shoal/` if installed 
 root permissions.
 
 ### Recommended Instalation Method: Use pip
 
-1. `pip install shoal-client`
+1. `sudo python3 -m pip install shoal-client` or, if using an old python2 version of pip: `pip install shoal-client`
 2. Copy the configuration file to proper location
     ```
     # For python3
     cp /usr/local/share/shoal-client/shoal_client.conf /etc/shoal/
     
     # For python2
     cp /usr/share/shoal-client/shoal_client.conf /etc/shoal/
@@ -54,16 +53,17 @@
     (serverurl=http://PresetServer.ca:3128)(proxyurl=http://PROXY.FROM.SHOAL.1:3128)(proxyurl=http://PROXY.FROM.SHOAL.2:3128)
 
 ### Flags and Options
 | Option | Description |
 | --- | --- |
 | -d or --dump | Print closest proxies to terminal for testing or debugging. |
 | -s `hostname` or --server `hostname`| Specifies URL of the desired shoal-server to contact. Takes precedence over the option in config file. |
-| -n `int` or --squids `int` | Specifies the number of squids to retrieve from the shoal-server |
-| -f or --frontier| Outputs a string appropriate for use as the frontier proxy enviroment variable instead of using cvmfs-talk to update the active proxy configuration|
+| -n `int` or --squids `int` | Specifies the number of squids to retrieve from the shoal-server. |
+| -f or --frontier | Outputs a string appropriate for use as the frontier proxy enviroment variable instead of using cvmfs-talk to update the active proxy configuration. |
+| -k or --skip-broadcast | Skips waiting to hear from a shoal-agent on the local network and goes directly to the shoal server for a squid. Only reccomended when you know there is no squid//agent on the local network. |
 
 Shoal client now uses the cvmfs_talk protocol. To view the list of returned squids issue:
 
      cvmfs_talk proxy info
 
 ## Other Installation Methods
```

