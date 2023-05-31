# Comparing `tmp/netdevice-1.2.6.tar.gz` & `tmp/netdevice-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netdevice-1.2.6.tar", last modified: Tue Sep  6 03:25:03 2022, max compression
+gzip compressed data, was "netdevice-1.2.7.tar", last modified: Wed May 31 09:06:44 2023, max compression
```

## Comparing `netdevice-1.2.6.tar` & `netdevice-1.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2022-09-06 03:25:03.251786 netdevice-1.2.6/
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       39 2022-08-17 08:17:30.000000 netdevice-1.2.6/MANIFEST.in
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    28158 2022-09-06 03:25:03.251786 netdevice-1.2.6/PKG-INFO
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    27872 2022-09-06 03:24:48.000000 netdevice-1.2.6/README.rst
-drwxr-xr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2022-09-06 03:25:03.229784 netdevice-1.2.6/demo/
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)     1988 2022-08-17 08:17:30.000000 netdevice-1.2.6/demo/demo.py
-drwxr-xr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2022-09-06 03:25:03.241783 netdevice-1.2.6/netdevice/
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      447 2022-08-17 08:17:30.000000 netdevice-1.2.6/netdevice/__init__.py
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      385 2022-08-17 08:17:30.000000 netdevice-1.2.6/netdevice/cisco.py
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    35106 2022-08-17 08:17:30.000000 netdevice-1.2.6/netdevice/junos.py
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    51940 2022-09-06 03:19:04.000000 netdevice-1.2.6/netdevice/linux.py
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    27847 2022-08-17 08:17:30.000000 netdevice-1.2.6/netdevice/ovn.py
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    24965 2022-08-17 08:17:30.000000 netdevice-1.2.6/netdevice/ovs.py
-drwxr-xr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2022-09-06 03:25:03.249785 netdevice-1.2.6/netdevice.egg-info/
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    28158 2022-09-06 03:25:03.000000 netdevice-1.2.6/netdevice.egg-info/PKG-INFO
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      331 2022-09-06 03:25:03.000000 netdevice-1.2.6/netdevice.egg-info/SOURCES.txt
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)        1 2022-09-06 03:25:03.000000 netdevice-1.2.6/netdevice.egg-info/dependency_links.txt
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       53 2022-09-06 03:25:03.000000 netdevice-1.2.6/netdevice.egg-info/requires.txt
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       10 2022-09-06 03:25:03.000000 netdevice-1.2.6/netdevice.egg-info/top_level.txt
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       38 2022-09-06 03:25:03.252785 netdevice-1.2.6/setup.cfg
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      570 2022-09-06 03:23:13.000000 netdevice-1.2.6/setup.py
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-05-31 09:06:44.413310 netdevice-1.2.7/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       39 2022-08-17 08:17:30.000000 netdevice-1.2.7/MANIFEST.in
+-rw-rw-r--   0 ypguo    (19391612) Domain Users (1049089)    28180 2023-05-31 09:06:44.414310 netdevice-1.2.7/PKG-INFO
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    27914 2023-05-31 09:06:12.000000 netdevice-1.2.7/README.rst
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-05-31 09:06:44.376318 netdevice-1.2.7/demo/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)     1988 2022-08-17 08:17:30.000000 netdevice-1.2.7/demo/demo.py
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-05-31 09:06:44.394312 netdevice-1.2.7/netdevice/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      447 2022-08-17 08:17:30.000000 netdevice-1.2.7/netdevice/__init__.py
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      385 2022-08-17 08:17:30.000000 netdevice-1.2.7/netdevice/cisco.py
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    35106 2022-08-17 08:17:30.000000 netdevice-1.2.7/netdevice/junos.py
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    51892 2023-05-31 09:05:20.000000 netdevice-1.2.7/netdevice/linux.py
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    27847 2022-08-17 08:17:30.000000 netdevice-1.2.7/netdevice/ovn.py
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    24965 2022-08-17 08:17:30.000000 netdevice-1.2.7/netdevice/ovs.py
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-05-31 09:06:44.411319 netdevice-1.2.7/netdevice.egg-info/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    28180 2023-05-31 09:06:44.000000 netdevice-1.2.7/netdevice.egg-info/PKG-INFO
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      331 2023-05-31 09:06:44.000000 netdevice-1.2.7/netdevice.egg-info/SOURCES.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)        1 2023-05-31 09:06:44.000000 netdevice-1.2.7/netdevice.egg-info/dependency_links.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       53 2023-05-31 09:06:44.000000 netdevice-1.2.7/netdevice.egg-info/requires.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       10 2023-05-31 09:06:44.000000 netdevice-1.2.7/netdevice.egg-info/top_level.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       38 2023-05-31 09:06:44.415313 netdevice-1.2.7/setup.cfg
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      570 2023-05-31 09:05:55.000000 netdevice-1.2.7/setup.py
```

### Comparing `netdevice-1.2.6/PKG-INFO` & `netdevice-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: netdevice
-Version: 1.2.6
+Version: 1.2.7
 Summary: Python modules to execute command on remote network device based on pexpect.
 Home-page: https://github.com/guoyoooping/networkdevice
 Author: Yongping Guo
 Author-email: guoyoooping@163.com
 License: GPLv3
-Platform: UNKNOWN
 
 netdevice
 *********
 
 Python modules to execute command on remote network device.
 
 To install easily::
@@ -734,9 +733,8 @@
 
 1.2: support new device: ovn
 
 1.2.1: 1) LinuxDevice support non server given, then it would run sh command locally.
        2) Support new device: ovn.
 
 1.2.6 fix issue when login by telnet
-
-
+1.2.7 Bug fix: Leading name doesn't work.
```

### Comparing `netdevice-1.2.6/README.rst` & `netdevice-1.2.7/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -724,7 +724,8 @@
 
 1.2: support new device: ovn
 
 1.2.1: 1) LinuxDevice support non server given, then it would run sh command locally.
        2) Support new device: ovn.
 
 1.2.6 fix issue when login by telnet
+1.2.7 Bug fix: Leading name doesn't work.
```

### Comparing `netdevice-1.2.6/demo/demo.py` & `netdevice-1.2.7/demo/demo.py`

 * *Files identical despite different names*

### Comparing `netdevice-1.2.6/netdevice/junos.py` & `netdevice-1.2.7/netdevice/junos.py`

 * *Files identical despite different names*

### Comparing `netdevice-1.2.6/netdevice/linux.py` & `netdevice-1.2.7/netdevice/linux.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,35 +567,35 @@
         #print("level: %d, log_level: %d" %(level, log_level))
         if level > log_level or (not kwargs.get("with_log", True)):
             return
 
         name_color = color_dict.get(self['log_color'], None)
         now = time.strftime('%Y%m%d %H:%M:%S',time.localtime(time.time()))
         l = self['log_time'] and "[%s]" %(now) or ""
+        if leading:
+            logname = leading
+        else:
+            logname = self["name"] and self["name"] or self.name
         #l += "[%s][%s]" %(now, threading.current_thread().name)
         l2 = l + "[%s%s%s]" %(name_color and name_color or "",
-                self["name"] and self["name"] or self.name,
-                name_color and "\033[0m" or "")
-        l3 = l + "[%s]" %(self["name"] and self["name"] or self.name)
+                logname, name_color and "\033[0m" or "")
 
         f = StringIO(message)
         for i in f.readlines():
             # remove the trailing '\n' and readd later.
             i = i.strip('[\r\n]')
             if self.fd:
                 self.fd.write("%s: %s\n" %(l2, i))
                 self.fd.flush()
 
             if color != "no_color" or bg_color != "no_color":
                 i = "%s%s%s%s" %(color_dict.get(color, 'no_color'),
                         bg_color_dict.get(bg_color, 'no_color'),
                         i,
                         color_dict['no_color'])
-            if leading:
-                i = leading + i
             sys.stdout.write("%s: %s\n" %(l2, i))
         f.close()
 
     def sleep (self, timeout, total = 50, char = '>', description = "sleep"):
         '''
         Sleep with progress bar, the granularity is 0.1 second. something like
         that:
```

### Comparing `netdevice-1.2.6/netdevice/ovn.py` & `netdevice-1.2.7/netdevice/ovn.py`

 * *Files identical despite different names*

### Comparing `netdevice-1.2.6/netdevice/ovs.py` & `netdevice-1.2.7/netdevice/ovs.py`

 * *Files identical despite different names*

### Comparing `netdevice-1.2.6/netdevice.egg-info/PKG-INFO` & `netdevice-1.2.7/netdevice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: netdevice
-Version: 1.2.6
+Version: 1.2.7
 Summary: Python modules to execute command on remote network device based on pexpect.
 Home-page: https://github.com/guoyoooping/networkdevice
 Author: Yongping Guo
 Author-email: guoyoooping@163.com
 License: GPLv3
-Platform: UNKNOWN
 
 netdevice
 *********
 
 Python modules to execute command on remote network device.
 
 To install easily::
@@ -734,9 +733,8 @@
 
 1.2: support new device: ovn
 
 1.2.1: 1) LinuxDevice support non server given, then it would run sh command locally.
        2) Support new device: ovn.
 
 1.2.6 fix issue when login by telnet
-
-
+1.2.7 Bug fix: Leading name doesn't work.
```

### Comparing `netdevice-1.2.6/setup.py` & `netdevice-1.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='netdevice',
-      version='1.2.6',
+      version='1.2.7',
       author='Yongping Guo',
       author_email='guoyoooping@163.com',
       description='Python modules to execute command on remote network device based on pexpect.',
       long_description=open('README.rst').read(),
       install_requires = ["ipaddress", "pexpect", "lxml", "IPy", "xmltodict", "dpkt", "simplejson"],
       url='https://github.com/guoyoooping/networkdevice',
       license="GPLv3",
```

