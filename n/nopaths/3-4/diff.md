# Comparing `tmp/nopaths-3.tar.gz` & `tmp/nopaths-4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopaths-3.tar", last modified: Tue May 30 02:01:08 2023, max compression
+gzip compressed data, was "nopaths-4.tar", last modified: Wed May 31 09:18:13 2023, max compression
```

## Comparing `nopaths-3.tar` & `nopaths-4.tar`

### file list

```diff
@@ -1,61 +1,58 @@
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 02:01:08.749209 nopaths-3/
--rw-r--r--   0 nop       (1000) nop       (1000)     4445 2023-05-30 02:01:08.749209 nopaths-3/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)     2835 2023-05-29 12:59:16.000000 nopaths-3/README.rst
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 02:01:08.745209 nopaths-3/bin/
--rwxr-xr-x   0 nop       (1000) nop       (1000)     2374 2023-05-30 00:51:00.000000 nopaths-3/bin/nopaths
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 02:01:08.745209 nopaths-3/nopaths/
--rw-r--r--   0 nop       (1000) nop       (1000)      527 2023-05-29 13:03:22.000000 nopaths-3/nopaths/clients.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1050 2023-05-29 13:03:22.000000 nopaths-3/nopaths/clocked.py
--rw-r--r--   0 nop       (1000) nop       (1000)      923 2023-05-29 13:03:22.000000 nopaths-3/nopaths/command.py
--rw-r--r--   0 nop       (1000) nop       (1000)      127 2023-05-29 13:34:01.000000 nopaths-3/nopaths/configs.py
--rw-r--r--   0 nop       (1000) nop       (1000)      760 2023-05-29 13:03:22.000000 nopaths-3/nopaths/decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      341 2023-05-29 13:03:22.000000 nopaths-3/nopaths/default.py
--rw-r--r--   0 nop       (1000) nop       (1000)      203 2023-05-29 13:31:30.000000 nopaths-3/nopaths/defines.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1149 2023-05-29 13:03:22.000000 nopaths-3/nopaths/encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      368 2023-05-29 13:03:22.000000 nopaths-3/nopaths/errored.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1913 2023-05-29 13:03:22.000000 nopaths-3/nopaths/handler.py
--rw-r--r--   0 nop       (1000) nop       (1000)      903 2023-05-29 13:03:22.000000 nopaths-3/nopaths/listens.py
--rw-r--r--   0 nop       (1000) nop       (1000)      400 2023-05-29 13:03:22.000000 nopaths-3/nopaths/logging.py
--rw-r--r--   0 nop       (1000) nop       (1000)      929 2023-05-29 13:03:22.000000 nopaths-3/nopaths/message.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 02:01:08.749209 nopaths-3/nopaths/modules/
--rw-r--r--   0 nop       (1000) nop       (1000)      520 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/__init__.py
--rw-r--r--   0 nop       (1000) nop       (1000)      561 2023-05-29 13:30:51.000000 nopaths-3/nopaths/modules/cfg.py
--rw-r--r--   0 nop       (1000) nop       (1000)      158 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/cmd.py
--rw-r--r--   0 nop       (1000) nop       (1000)      365 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/err.py
--rw-r--r--   0 nop       (1000) nop       (1000)      402 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/flt.py
--rw-r--r--   0 nop       (1000) nop       (1000)      948 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/fnd.py
--rw-r--r--   0 nop       (1000) nop       (1000)    19809 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/irc.py
--rw-r--r--   0 nop       (1000) nop       (1000)      668 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/log.py
--rw-r--r--   0 nop       (1000) nop       (1000)    17771 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/mdl.py
--rw-r--r--   0 nop       (1000) nop       (1000)      136 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/mod.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2385 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/req.py
--rw-r--r--   0 nop       (1000) nop       (1000)     7638 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/rss.py
--rw-r--r--   0 nop       (1000) nop       (1000)      458 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/slg.py
--rw-r--r--   0 nop       (1000) nop       (1000)      295 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/sts.py
--rw-r--r--   0 nop       (1000) nop       (1000)      892 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/tdo.py
--rw-r--r--   0 nop       (1000) nop       (1000)      989 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/thr.py
--rw-r--r--   0 nop       (1000) nop       (1000)      202 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/upt.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2727 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/usr.py
--rw-r--r--   0 nop       (1000) nop       (1000)      157 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/ver.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1640 2023-05-29 13:03:22.000000 nopaths-3/nopaths/objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2057 2023-05-29 13:03:22.000000 nopaths-3/nopaths/objfunc.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1756 2023-05-29 13:03:22.000000 nopaths-3/nopaths/parsers.py
--rw-r--r--   0 nop       (1000) nop       (1000)     3985 2023-05-29 13:03:22.000000 nopaths-3/nopaths/persist.py
--rw-r--r--   0 nop       (1000) nop       (1000)      325 2023-05-29 13:03:22.000000 nopaths-3/nopaths/repeats.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2425 2023-05-30 00:56:36.000000 nopaths-3/nopaths/runtime.py
--rw-r--r--   0 nop       (1000) nop       (1000)      878 2023-05-29 13:03:22.000000 nopaths-3/nopaths/threads.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2891 2023-05-29 13:03:22.000000 nopaths-3/nopaths/utility.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 02:01:08.749209 nopaths-3/nopaths.egg-info/
--rw-r--r--   0 nop       (1000) nop       (1000)     4445 2023-05-30 02:01:08.000000 nopaths-3/nopaths.egg-info/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)     1127 2023-05-30 02:01:08.000000 nopaths-3/nopaths.egg-info/SOURCES.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-30 02:01:08.000000 nopaths-3/nopaths.egg-info/dependency_links.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        8 2023-05-30 02:01:08.000000 nopaths-3/nopaths.egg-info/top_level.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-30 02:01:08.000000 nopaths-3/nopaths.egg-info/zip-safe
--rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-05-30 02:01:08.749209 nopaths-3/setup.cfg
--rw-r--r--   0 nop       (1000) nop       (1000)      816 2023-05-30 02:00:11.000000 nopaths-3/setup.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 02:01:08.749209 nopaths-3/test/
--rw-r--r--   0 nop       (1000) nop       (1000)      483 2023-05-29 12:59:16.000000 nopaths-3/test/test_decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      377 2023-05-29 12:59:16.000000 nopaths-3/test/test_encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      887 2023-05-29 12:59:16.000000 nopaths-3/test/test_inherit.py
--rw-r--r--   0 nop       (1000) nop       (1000)     4580 2023-05-29 12:59:16.000000 nopaths-3/test/test_objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1051 2023-05-29 12:59:16.000000 nopaths-3/test/test_storage.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-31 09:18:13.138167 nopaths-4/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4524 2023-05-31 09:18:13.138167 nopaths-4/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)     2890 2023-05-30 21:25:56.000000 nopaths-4/README.rst
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-31 09:18:13.134167 nopaths-4/nopaths/
+-rw-r--r--   0 nop       (1000) nop       (1000)     1253 2023-05-30 22:47:54.000000 nopaths-4/nopaths/__init__.py
+-rwxr-xr-x   0 nop       (1000) nop       (1000)     2205 2023-05-30 20:37:42.000000 nopaths-4/nopaths/__main__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      527 2023-05-29 13:03:22.000000 nopaths-4/nopaths/clients.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1050 2023-05-29 13:03:22.000000 nopaths-4/nopaths/clocked.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2484 2023-05-31 09:08:04.000000 nopaths-4/nopaths/command.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      127 2023-05-29 13:34:01.000000 nopaths-4/nopaths/configs.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      760 2023-05-29 13:03:22.000000 nopaths-4/nopaths/decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      341 2023-05-29 13:03:22.000000 nopaths-4/nopaths/default.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      226 2023-05-30 08:05:54.000000 nopaths-4/nopaths/defines.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1156 2023-05-30 20:10:02.000000 nopaths-4/nopaths/encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      311 2023-05-30 08:03:46.000000 nopaths-4/nopaths/errored.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1913 2023-05-29 13:03:22.000000 nopaths-4/nopaths/handler.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      903 2023-05-29 13:03:22.000000 nopaths-4/nopaths/listens.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      410 2023-05-30 13:33:23.000000 nopaths-4/nopaths/logging.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      929 2023-05-29 13:03:22.000000 nopaths-4/nopaths/message.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-31 09:18:13.138167 nopaths-4/nopaths/modules/
+-rw-r--r--   0 nop       (1000) nop       (1000)     1746 2023-05-30 22:54:09.000000 nopaths-4/nopaths/modules/__init__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      537 2023-05-30 17:33:08.000000 nopaths-4/nopaths/modules/cfg.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      195 2023-05-30 18:18:56.000000 nopaths-4/nopaths/modules/cmd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      365 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/err.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      402 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/flt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      948 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/fnd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)    19811 2023-05-30 11:53:49.000000 nopaths-4/nopaths/modules/irc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      668 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/log.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      136 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/mod.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     7638 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/rss.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      295 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/sts.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      892 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/tdo.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      989 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/thr.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      202 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/upt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      157 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/ver.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1638 2023-05-30 19:25:22.000000 nopaths-4/nopaths/objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2082 2023-05-30 19:02:10.000000 nopaths-4/nopaths/objfunc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1756 2023-05-29 13:03:22.000000 nopaths-4/nopaths/parsers.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     4149 2023-05-30 19:27:37.000000 nopaths-4/nopaths/persist.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      325 2023-05-29 13:03:22.000000 nopaths-4/nopaths/repeats.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2439 2023-05-30 13:31:53.000000 nopaths-4/nopaths/runtime.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      878 2023-05-29 13:03:22.000000 nopaths-4/nopaths/threads.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2891 2023-05-29 13:03:22.000000 nopaths-4/nopaths/utility.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-31 09:18:13.138167 nopaths-4/nopaths.egg-info/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4524 2023-05-31 09:18:13.000000 nopaths-4/nopaths.egg-info/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)     1086 2023-05-31 09:18:13.000000 nopaths-4/nopaths.egg-info/SOURCES.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-31 09:18:13.000000 nopaths-4/nopaths.egg-info/dependency_links.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        8 2023-05-31 09:18:13.000000 nopaths-4/nopaths.egg-info/top_level.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-31 09:18:13.000000 nopaths-4/nopaths.egg-info/zip-safe
+-rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-05-31 09:18:13.138167 nopaths-4/setup.cfg
+-rw-r--r--   0 nop       (1000) nop       (1000)      787 2023-05-30 21:34:37.000000 nopaths-4/setup.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-31 09:18:13.138167 nopaths-4/test/
+-rw-r--r--   0 nop       (1000) nop       (1000)      661 2023-05-31 09:17:18.000000 nopaths-4/test/test_composite.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      483 2023-05-29 12:59:16.000000 nopaths-4/test/test_decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      377 2023-05-29 12:59:16.000000 nopaths-4/test/test_encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      887 2023-05-29 12:59:16.000000 nopaths-4/test/test_inherit.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     4580 2023-05-29 12:59:16.000000 nopaths-4/test/test_objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1051 2023-05-29 12:59:16.000000 nopaths-4/test/test_storage.py
```

### Comparing `nopaths-3/PKG-INFO` & `nopaths-4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopaths
-Version: 3
+Version: 4
 Summary: there are no paths
 Home-page: http://github.com/nopaths/nopaths
 Author: No Paths <nopaths@proton.me>
 Author-email: nopaths@proton.me
 License: Public Domain
 Description: **NAME**
         
@@ -12,16 +12,16 @@
         
             nopaths - there are no paths
         
         **SYNOPSIS**
         
         ::
         
-            python3 -m nopaths <cmd> [key=val] [key==val]
-            python3 -m nopaths [-c] [-d] [-v]
+            nopaths <cmd> [key=val] [key==val]
+            nopaths [-c] [-d] [-v]
         
         **DESCRIPTION**
         
         ``nopaths`` is a python3 bot, it connects to irc and provides a select sets of
         commands. It doesn't use os.popen, does no external imports, can be run in client
         or daemon mode and has batteries included. 
         
@@ -52,67 +52,68 @@
         
         or download the tarball from https://github.com/nopaths/nopaths/releases/
         
         **USAGE**
         
         use an alias for easier typing::
         
-            $ alias np="python3 -m nopaths"
+            $ alias nopaths="python3 -m nopaths"
         
         list of commands::
         
-            $ np cmd
+            $ nopaths cmd
             cmd,err,flt,sts,thr,upt
         
         start a console::
         
-            $ np -c
+            $ nopaths -c
             >
         
         start additional modules::
         
-            $ np mod=<mod1,mod2> -c
+            $ nopaths mod=<mod1,mod2> -c
             >
         
         list of modules::
         
-            $ np mod
+            $ nopaths mod
             cmd,err,flt,fnd,irc,log,mod,rss,sts,tdo,thr,upt
         
         start as daemon::
         
-            $ np mod=cmd,irc,rss -d
+            $ nopaths mod=cmd,irc,rss -d
             $ 
         
         **CONFIGURATION**
         
         *irc*
         
         
         ::
         
-            $ np cfg server=<server>
-            $ np cfg channel=<channel>
-            $ np cfg nick=<nick>
+            $ nopaths cfg server=<server>
+            $ nopaths cfg channel=<channel>
+            $ nopaths cfg nick=<nick>
         
         *sasl*
         
         ::
         
-            $ np pwd <nsvnick> <nspass>
-            $ np cfg password=<frompwd>
+            $ nopaths pwd <nsnick> <nspass>
+            $ nopaths cfg password=<frompwd>
         
         *rss*
         
         ::
         
-            $ np rss <url>
-            $ np dpl <str_in_url> <i1,i2>
-            $ np rem <str_in_url>
-            $ np nme <str_in_url< <name>
+            $ nopaths rss <url>
+            $ nopaths dpl <str_in_url> <i1,i2>
+            $ nopaths rem <str_in_url>
+            $ nopaths nme <str_in_url> <name>
+        
         
         **COMMANDS**
         
         ::
         
             cmd - commands
             cfg - irc configuration
@@ -131,20 +132,22 @@
             rem - removes a rss feed
             req - reconsider
             rss - add a feed
             slg - slogan
             thr - show the running threads
             tpc - genocide stats into topic
         
+        
         **AUTHOR**
         
         ::
         
             No Paths <nopaths@proton.me>
         
+        
         **COPYRIGHT**
         
         ::
         
             nopaths is placed in the Public Domain.
         
 Platform: UNKNOWN
```

### Comparing `nopaths-3/README.rst` & `nopaths-4/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
     nopaths - there are no paths
 
 **SYNOPSIS**
 
 ::
 
-    python3 -m nopaths <cmd> [key=val] [key==val]
-    python3 -m nopaths [-c] [-d] [-v]
+    nopaths <cmd> [key=val] [key==val]
+    nopaths [-c] [-d] [-v]
 
 **DESCRIPTION**
 
 ``nopaths`` is a python3 bot, it connects to irc and provides a select sets of
 commands. It doesn't use os.popen, does no external imports, can be run in client
 or daemon mode and has batteries included. 
 
@@ -44,67 +44,68 @@
 
 or download the tarball from https://github.com/nopaths/nopaths/releases/
 
 **USAGE**
 
 use an alias for easier typing::
 
-    $ alias np="python3 -m nopaths"
+    $ alias nopaths="python3 -m nopaths"
 
 list of commands::
 
-    $ np cmd
+    $ nopaths cmd
     cmd,err,flt,sts,thr,upt
 
 start a console::
 
-    $ np -c
+    $ nopaths -c
     >
 
 start additional modules::
 
-    $ np mod=<mod1,mod2> -c
+    $ nopaths mod=<mod1,mod2> -c
     >
 
 list of modules::
 
-    $ np mod
+    $ nopaths mod
     cmd,err,flt,fnd,irc,log,mod,rss,sts,tdo,thr,upt
 
 start as daemon::
 
-    $ np mod=cmd,irc,rss -d
+    $ nopaths mod=cmd,irc,rss -d
     $ 
 
 **CONFIGURATION**
 
 *irc*
 
 
 ::
 
-    $ np cfg server=<server>
-    $ np cfg channel=<channel>
-    $ np cfg nick=<nick>
+    $ nopaths cfg server=<server>
+    $ nopaths cfg channel=<channel>
+    $ nopaths cfg nick=<nick>
 
 *sasl*
 
 ::
 
-    $ np pwd <nsvnick> <nspass>
-    $ np cfg password=<frompwd>
+    $ nopaths pwd <nsnick> <nspass>
+    $ nopaths cfg password=<frompwd>
 
 *rss*
 
 ::
 
-    $ np rss <url>
-    $ np dpl <str_in_url> <i1,i2>
-    $ np rem <str_in_url>
-    $ np nme <str_in_url< <name>
+    $ nopaths rss <url>
+    $ nopaths dpl <str_in_url> <i1,i2>
+    $ nopaths rem <str_in_url>
+    $ nopaths nme <str_in_url> <name>
+
 
 **COMMANDS**
 
 ::
 
     cmd - commands
     cfg - irc configuration
@@ -123,18 +124,20 @@
     rem - removes a rss feed
     req - reconsider
     rss - add a feed
     slg - slogan
     thr - show the running threads
     tpc - genocide stats into topic
 
+
 **AUTHOR**
 
 ::
 
     No Paths <nopaths@proton.me>
 
+
 **COPYRIGHT**
 
 ::
 
     nopaths is placed in the Public Domain.
```

### Comparing `nopaths-3/bin/nopaths` & `nopaths-4/nopaths/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-#!/usr/bin/env python3
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R
+# pylint: disable=C,I,R,E0401,W0212,W0611
 
 
 "there are no paths"
 
 
 import os
 import readline
 import sys
 import termios
 import time
-import traceback
 
 
 sys.path.insert(0, os.getcwd())
 
 
 from nopaths.clients import Client
 from nopaths.command import Commands
-from nopaths.errored import Errors
 from nopaths.logging import Logging
-from nopaths.objects import update
-from nopaths.persist import Persist, write
-from nopaths.runtime import DATE, Cfg, banner, command, launch, parse_cli
+from nopaths.persist import Persist
+from nopaths.runtime import Cfg, banner, command, parse_cli
 from nopaths.runtime import scanstr, waiter
-from nopaths.utility import spl
 
 
 import nopaths.modules
 
 
+Commands.modules = nopaths.modules
 Persist.workdir = os.path.expanduser(f"~/.{Cfg.name}")
 
 
 class CLI(Client):
 
     def announce(self, txt):
         pass
@@ -88,15 +84,14 @@
     parse_cli(' '.join(sys.argv[1:]))
     if "v" in Cfg.opts and "d" not in Cfg.opts:
         Logging.verbose = True
         Logging.raw = print
         banner()
     dowait = False
     if Cfg.txt:
-        scanstr(nopaths.modules, Cfg.mod, "a" in Cfg.opts)
         cli = CLI()
         command(cli, Cfg.otxt)
     elif 'd' in Cfg.opts:
         daemon()
         dowait = True
     if "c" in Cfg.opts:
         dowait = True
```

### Comparing `nopaths-3/nopaths/clients.py` & `nopaths-4/nopaths/clients.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/clocked.py` & `nopaths-4/nopaths/clocked.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/decoder.py` & `nopaths-4/nopaths/decoder.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/encoder.py` & `nopaths-4/nopaths/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is placed in the Public Domain.
 
 
 import json
 
 
-from .objects import Object
+from .objects import Object, items
 
 
 def __dir__():
     return (
             'ObjectEncoder',
             'dump',
             'dumps'
```

### Comparing `nopaths-3/nopaths/handler.py` & `nopaths-4/nopaths/handler.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/listens.py` & `nopaths-4/nopaths/listens.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/message.py` & `nopaths-4/nopaths/message.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/modules/cfg.py` & `nopaths-4/nopaths/modules/cfg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R
 
 
 from ..objects import edit, keys, prt
 from ..persist import last, write
 from ..runtime import Cfg
```

### Comparing `nopaths-3/nopaths/modules/fnd.py` & `nopaths-4/nopaths/modules/fnd.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/modules/irc.py` & `nopaths-4/nopaths/modules/irc.py`

 * *Files 1% similar despite different names*

```diff
@@ -481,15 +481,15 @@
                 event.txt = event.txt[1:]
             elif event.txt.startswith('%s:' % self.cfg.nick):
                 event.txt = event.txt[len(self.cfg.nick)+1:]
             else:
                 return
             if self.cfg.users and not Users.allowed(event.origin, 'USER'):
                 return
-            Logging.debug(f"command from {event.orig}: {event.txt}")
+            Logging.debug(f"command from {event.origin}: {event.txt}")
             msg = Message()
             copy(msg, event)
             msg.type = 'command'
             msg.parse(event.txt)
             self.handle(msg)
 
     def quit(self, event):
```

### Comparing `nopaths-3/nopaths/modules/log.py` & `nopaths-4/nopaths/modules/log.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/modules/rss.py` & `nopaths-4/nopaths/modules/rss.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/modules/tdo.py` & `nopaths-4/nopaths/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/modules/thr.py` & `nopaths-4/nopaths/modules/thr.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/objects.py` & `nopaths-4/nopaths/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 import uuid
 
 
 def __dir__():
     return (
             'Object',
             'copy',
-            'indet',
+            'ident',
             'items',
             'keys',
             'kind',
             'update',
             'values'
            )
 
 
 class Object:
 
     __slots__ = ('__dict__', '__oid__')
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self):
         self.__oid__ = ident(self)
 
     def __iter__(self):
         return iter(self.__dict__)
 
     def __len__(self):
         return len(self.__dict__)
@@ -41,14 +41,15 @@
         update(obj, dict(val))
     elif isinstance(val, zip):
         update(obj, dict(val))
     elif isinstance(val, dict):
         update(obj, val)
     elif isinstance(val, Object):
         update(obj, vars(val))
+    return obj
 
 
 def ident(obj) -> str:
     return os.path.join(
                         kind(obj),
                         str(uuid.uuid4().hex),
                         os.sep.join(str(datetime.datetime.now()).split())
```

### Comparing `nopaths-3/nopaths/objfunc.py` & `nopaths-4/nopaths/objfunc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is placed in the Public Domain.
 
 
-from .objects import Object, items, keys
+from .objects import Object, copy, items, keys
 
 
 def __dir__():
     return (
             'edit',
             'prt',
             'search'
@@ -73,15 +73,16 @@
         res.append(txt)
     txt = " ".join(res)
     return txt.strip()
 
 
 def search(obj, selector) -> bool:
     res = False
-    select = Object(selector)
+    select = Object()
+    copy(select, selector)
     for key, value in items(select):
         try:
             val = getattr(obj, key)
         except AttributeError:
             continue
         if str(value) in str(val):
             res = True
```

### Comparing `nopaths-3/nopaths/parsers.py` & `nopaths-4/nopaths/parsers.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/persist.py` & `nopaths-4/nopaths/persist.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import time
 import _thread
 
 
 from .decoder import ObjectDecoder, load
 from .default import Default
 from .encoder import dump
-from .objects import Object, kind, update
+from .objects import Object, ident, kind, update
 from .objfunc import search
 from .utility import cdir, fnclass, fntime, strip
 
 
 def __dir__():
     return (
             'Persist',
@@ -119,14 +119,17 @@
         delattr(Persist.cls, f"{clz.__module__}.{clz.__name__}")
 
     @staticmethod
     def storedir() -> str:
         return os.path.join(Persist.workdir, "store")
 
 
+## FUNCTIONS
+
+
 def last(obj, selector=None) -> None:
     if selector is None:
         selector = {}
     result = sorted(
                     Persist.find(kind(obj), selector),
                     key=lambda x: fntime(x.__oid__)
                    )
@@ -144,13 +147,23 @@
             data = load(ofile)
             update(obj, data)
     obj.__oid__ = strip(pth)
     return obj.__oid__
 
 
 def write(obj) -> str:
-    pth = Persist.path(obj.__oid__)
+    try:
+        pth = Persist.path(obj.__oid__)
+    except TypeError:
+        pth = Persist.path(ident(obj))
     cdir(pth)
     with disklock:
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile)
     return strip(pth)
+
+"""
+def recursive(obj):
+    
+    for k, v in items(obj):
+"""
+
```

### Comparing `nopaths-3/nopaths/runtime.py` & `nopaths-4/nopaths/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 import functools
 import io
 import time
 import traceback
 
 
+from .default import Default
+from .objects import Object, kind, update
+from .logging import Logging
 from .command import Commands
 from .configs import Cfg
-from .default import Default
 from .errored import Errors
-from .logging import Logging
 from .message import Message
-from .objects import Object, kind, update
 from .persist import Persist
 from .threads import Thread
 from .utility import fntime, spl
 
 
 def __dir__():
     return (
@@ -33,19 +33,22 @@
 
 
 DATE = time.ctime(time.time()).replace("  ", " ")
 STARTTIME = time.time()
 
 
 Cfg.debug = False
-Cfg.mod = "cmd,err,flt,mod,,sts,thr,upt,ver"
+Cfg.mod = "cmd,err,flt,mod,sts,thr,upt,ver"
 Cfg.name = "nopaths"
 Cfg.skip = "PING,PONG,PRIVMSG"
 Cfg.threaded = False
-Cfg.version = "1"
+Cfg.version = "4"
+
+
+## FUNCTIONS
 
 
 def banner():
     Logging.debug(f"{Cfg.name.upper()} started at {DATE}")
 
 
 def command(cli, txt) -> Message:
```

### Comparing `nopaths-3/nopaths/threads.py` & `nopaths-4/nopaths/threads.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths/utility.py` & `nopaths-4/nopaths/utility.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/nopaths.egg-info/PKG-INFO` & `nopaths-4/nopaths.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopaths
-Version: 3
+Version: 4
 Summary: there are no paths
 Home-page: http://github.com/nopaths/nopaths
 Author: No Paths <nopaths@proton.me>
 Author-email: nopaths@proton.me
 License: Public Domain
 Description: **NAME**
         
@@ -12,16 +12,16 @@
         
             nopaths - there are no paths
         
         **SYNOPSIS**
         
         ::
         
-            python3 -m nopaths <cmd> [key=val] [key==val]
-            python3 -m nopaths [-c] [-d] [-v]
+            nopaths <cmd> [key=val] [key==val]
+            nopaths [-c] [-d] [-v]
         
         **DESCRIPTION**
         
         ``nopaths`` is a python3 bot, it connects to irc and provides a select sets of
         commands. It doesn't use os.popen, does no external imports, can be run in client
         or daemon mode and has batteries included. 
         
@@ -52,67 +52,68 @@
         
         or download the tarball from https://github.com/nopaths/nopaths/releases/
         
         **USAGE**
         
         use an alias for easier typing::
         
-            $ alias np="python3 -m nopaths"
+            $ alias nopaths="python3 -m nopaths"
         
         list of commands::
         
-            $ np cmd
+            $ nopaths cmd
             cmd,err,flt,sts,thr,upt
         
         start a console::
         
-            $ np -c
+            $ nopaths -c
             >
         
         start additional modules::
         
-            $ np mod=<mod1,mod2> -c
+            $ nopaths mod=<mod1,mod2> -c
             >
         
         list of modules::
         
-            $ np mod
+            $ nopaths mod
             cmd,err,flt,fnd,irc,log,mod,rss,sts,tdo,thr,upt
         
         start as daemon::
         
-            $ np mod=cmd,irc,rss -d
+            $ nopaths mod=cmd,irc,rss -d
             $ 
         
         **CONFIGURATION**
         
         *irc*
         
         
         ::
         
-            $ np cfg server=<server>
-            $ np cfg channel=<channel>
-            $ np cfg nick=<nick>
+            $ nopaths cfg server=<server>
+            $ nopaths cfg channel=<channel>
+            $ nopaths cfg nick=<nick>
         
         *sasl*
         
         ::
         
-            $ np pwd <nsvnick> <nspass>
-            $ np cfg password=<frompwd>
+            $ nopaths pwd <nsnick> <nspass>
+            $ nopaths cfg password=<frompwd>
         
         *rss*
         
         ::
         
-            $ np rss <url>
-            $ np dpl <str_in_url> <i1,i2>
-            $ np rem <str_in_url>
-            $ np nme <str_in_url< <name>
+            $ nopaths rss <url>
+            $ nopaths dpl <str_in_url> <i1,i2>
+            $ nopaths rem <str_in_url>
+            $ nopaths nme <str_in_url> <name>
+        
         
         **COMMANDS**
         
         ::
         
             cmd - commands
             cfg - irc configuration
@@ -131,20 +132,22 @@
             rem - removes a rss feed
             req - reconsider
             rss - add a feed
             slg - slogan
             thr - show the running threads
             tpc - genocide stats into topic
         
+        
         **AUTHOR**
         
         ::
         
             No Paths <nopaths@proton.me>
         
+        
         **COPYRIGHT**
         
         ::
         
             nopaths is placed in the Public Domain.
         
 Platform: UNKNOWN
```

### Comparing `nopaths-3/nopaths.egg-info/SOURCES.txt` & `nopaths-4/nopaths.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.rst
 setup.py
-bin/nopaths
+nopaths/__init__.py
+nopaths/__main__.py
 nopaths/clients.py
 nopaths/clocked.py
 nopaths/command.py
 nopaths/configs.py
 nopaths/decoder.py
 nopaths/default.py
 nopaths/defines.py
@@ -31,23 +32,20 @@
 nopaths/modules/cfg.py
 nopaths/modules/cmd.py
 nopaths/modules/err.py
 nopaths/modules/flt.py
 nopaths/modules/fnd.py
 nopaths/modules/irc.py
 nopaths/modules/log.py
-nopaths/modules/mdl.py
 nopaths/modules/mod.py
-nopaths/modules/req.py
 nopaths/modules/rss.py
-nopaths/modules/slg.py
 nopaths/modules/sts.py
 nopaths/modules/tdo.py
 nopaths/modules/thr.py
 nopaths/modules/upt.py
-nopaths/modules/usr.py
 nopaths/modules/ver.py
+test/test_composite.py
 test/test_decoder.py
 test/test_encoder.py
 test/test_inherit.py
 test/test_objects.py
 test/test_storage.py
```

### Comparing `nopaths-3/setup.py` & `nopaths-4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,27 @@
 
 def read():
     return open("README.rst", "r").read()
 
 
 setup(
     name="nopaths",
-    version="3",
+    version="4",
     author="No Paths <nopaths@proton.me>",
     author_email="nopaths@proton.me",
     url="http://github.com/nopaths/nopaths",
     zip_safe=True,
     description="there are no paths",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
     packages=[
               "nopaths",
               'nopaths.modules'
              ],
-    scripts=["bin/nopaths"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: Public Domain",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Software Development :: Libraries :: Python Modules",
      ],
 )
```

### Comparing `nopaths-3/test/test_inherit.py` & `nopaths-4/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/test/test_objects.py` & `nopaths-4/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `nopaths-3/test/test_storage.py` & `nopaths-4/test/test_storage.py`

 * *Files identical despite different names*

