# Comparing `tmp/py-cone-1.0.8.tar.gz` & `tmp/py-cone-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-cone-1.0.8.tar", last modified: Wed Mar 15 08:06:54 2023, max compression
+gzip compressed data, was "py-cone-1.0.9.tar", last modified: Wed May 31 09:37:26 2023, max compression
```

## Comparing `py-cone-1.0.8.tar` & `py-cone-1.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 08:06:54.395524 py-cone-1.0.8/
--rw-rw-rw-   0        0        0     1085 2023-02-21 05:25:29.000000 py-cone-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      220 2023-03-15 08:06:54.394017 py-cone-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-02-21 05:25:29.000000 py-cone-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-15 08:06:54.198377 py-cone-1.0.8/cone/
--rw-rw-rw-   0        0        0      105 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-15 08:06:54.215679 py-cone-1.0.8/cone/communication/
--rw-rw-rw-   0        0        0      141 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/communication/__init__.py
--rw-rw-rw-   0        0        0     1584 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/communication/ding_talk.py
--rw-rw-rw-   0        0        0       99 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/communication/mail.py
-drwxrwxrwx   0        0        0        0 2023-03-15 08:06:54.233167 py-cone-1.0.8/cone/crypto/
--rw-rw-rw-   0        0        0      123 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/crypto/__init__.py
--rw-rw-rw-   0        0        0     1196 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/crypto/aes.py
--rw-rw-rw-   0        0        0      238 2023-03-13 01:28:44.000000 py-cone-1.0.8/cone/crypto/md5.py
--rw-rw-rw-   0        0        0       99 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/crypto/rsa.py
-drwxrwxrwx   0        0        0        0 2023-03-15 08:06:54.258482 py-cone-1.0.8/cone/hooks/
--rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/hooks/__init__.py
--rw-rw-rw-   0        0        0      364 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/hooks/exception.py
--rw-rw-rw-   0        0        0     1643 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/hooks/lib.py
--rw-rw-rw-   0        0        0      234 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/hooks/signal.py
-drwxrwxrwx   0        0        0        0 2023-03-15 08:06:54.277483 py-cone-1.0.8/cone/patterns/
--rw-rw-rw-   0        0        0      201 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/patterns/__init__.py
--rw-rw-rw-   0        0        0      393 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/patterns/instance.py
--rw-rw-rw-   0        0        0      767 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/patterns/singleton.py
-drwxrwxrwx   0        0        0        0 2023-03-15 08:06:54.323336 py-cone-1.0.8/cone/utils/
--rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/utils/__init__.py
--rw-rw-rw-   0        0        0     6590 2023-03-15 08:06:02.000000 py-cone-1.0.8/cone/utils/classes.py
--rw-rw-rw-   0        0        0     4520 2023-02-21 08:39:35.000000 py-cone-1.0.8/cone/utils/config.py
--rw-rw-rw-   0        0        0     2704 2023-03-10 01:39:26.000000 py-cone-1.0.8/cone/utils/db_utils.py
--rw-rw-rw-   0        0        0    14807 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/utils/functional.py
--rw-rw-rw-   0        0        0     2310 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/utils/log.py
-drwxrwxrwx   0        0        0        0 2023-03-15 08:06:54.338360 py-cone-1.0.8/cone/utils/network/
--rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/utils/network/__init__.py
--rw-rw-rw-   0        0        0     3327 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/utils/network/curl.py
--rw-rw-rw-   0        0        0      814 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/utils/network/url.py
--rw-rw-rw-   0        0        0     1003 2023-02-21 05:25:29.000000 py-cone-1.0.8/cone/utils/os.py
-drwxrwxrwx   0        0        0        0 2023-03-15 08:06:54.350748 py-cone-1.0.8/py_cone.egg-info/
--rw-rw-rw-   0        0        0      220 2023-03-15 08:06:54.000000 py-cone-1.0.8/py_cone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      880 2023-03-15 08:06:54.000000 py-cone-1.0.8/py_cone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 08:06:54.000000 py-cone-1.0.8/py_cone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-03-15 08:06:54.000000 py-cone-1.0.8/py_cone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 08:06:54.395524 py-cone-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      305 2023-03-15 08:06:02.000000 py-cone-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-15 08:06:54.394017 py-cone-1.0.8/tests/
--rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0      608 2023-02-21 05:25:29.000000 py-cone-1.0.8/tests/communication.py
--rw-rw-rw-   0        0        0     2051 2023-02-21 05:25:29.000000 py-cone-1.0.8/tests/curl.py
--rw-rw-rw-   0        0        0      499 2023-02-21 05:25:29.000000 py-cone-1.0.8/tests/exception.py
--rw-rw-rw-   0        0        0     1114 2023-02-21 05:25:29.000000 py-cone-1.0.8/tests/functional.py
--rw-rw-rw-   0        0        0      923 2023-02-21 05:25:29.000000 py-cone-1.0.8/tests/hook.py
--rw-rw-rw-   0        0        0      476 2023-02-21 05:25:29.000000 py-cone-1.0.8/tests/interrupt.py
--rw-rw-rw-   0        0        0      996 2023-02-21 05:25:29.000000 py-cone-1.0.8/tests/pattern.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.304181 py-cone-1.0.9/
+-rw-rw-rw-   0        0        0     1085 2023-02-21 05:25:29.000000 py-cone-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      220 2023-05-31 09:37:26.303677 py-cone-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-02-21 05:25:29.000000 py-cone-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.178447 py-cone-1.0.9/cone/
+-rw-rw-rw-   0        0        0      105 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.196213 py-cone-1.0.9/cone/communication/
+-rw-rw-rw-   0        0        0      141 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/communication/__init__.py
+-rw-rw-rw-   0        0        0     1584 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/communication/ding_talk.py
+-rw-rw-rw-   0        0        0       99 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/communication/mail.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.199216 py-cone-1.0.9/cone/crypto/
+-rw-rw-rw-   0        0        0      123 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1196 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/crypto/aes.py
+-rw-rw-rw-   0        0        0      238 2023-03-13 01:28:44.000000 py-cone-1.0.9/cone/crypto/md5.py
+-rw-rw-rw-   0        0        0       99 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/crypto/rsa.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.202829 py-cone-1.0.9/cone/hooks/
+-rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/hooks/__init__.py
+-rw-rw-rw-   0        0        0      364 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/hooks/exception.py
+-rw-rw-rw-   0        0        0     1643 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/hooks/lib.py
+-rw-rw-rw-   0        0        0      234 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/hooks/signal.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.214168 py-cone-1.0.9/cone/patterns/
+-rw-rw-rw-   0        0        0      201 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/patterns/__init__.py
+-rw-rw-rw-   0        0        0      393 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/patterns/instance.py
+-rw-rw-rw-   0        0        0      767 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/patterns/singleton.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.237456 py-cone-1.0.9/cone/utils/
+-rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/utils/__init__.py
+-rw-rw-rw-   0        0        0     6590 2023-03-15 08:06:02.000000 py-cone-1.0.9/cone/utils/classes.py
+-rw-rw-rw-   0        0        0     4520 2023-02-21 08:39:35.000000 py-cone-1.0.9/cone/utils/config.py
+-rw-rw-rw-   0        0        0     2704 2023-03-10 01:39:26.000000 py-cone-1.0.9/cone/utils/db_utils.py
+-rw-rw-rw-   0        0        0    15011 2023-05-31 09:36:43.000000 py-cone-1.0.9/cone/utils/functional.py
+-rw-rw-rw-   0        0        0     2310 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/utils/log.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.245093 py-cone-1.0.9/cone/utils/network/
+-rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/utils/network/__init__.py
+-rw-rw-rw-   0        0        0     3327 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/utils/network/curl.py
+-rw-rw-rw-   0        0        0      814 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/utils/network/url.py
+-rw-rw-rw-   0        0        0     1003 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/utils/os.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.254597 py-cone-1.0.9/py_cone.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-05-31 09:37:26.000000 py-cone-1.0.9/py_cone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2023-05-31 09:37:26.000000 py-cone-1.0.9/py_cone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 09:37:26.000000 py-cone-1.0.9/py_cone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 09:37:26.000000 py-cone-1.0.9/py_cone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 09:37:26.304181 py-cone-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      293 2023-05-31 09:36:24.000000 py-cone-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.302360 py-cone-1.0.9/tests/
+-rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      608 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/communication.py
+-rw-rw-rw-   0        0        0     2051 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/curl.py
+-rw-rw-rw-   0        0        0      499 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/exception.py
+-rw-rw-rw-   0        0        0     1114 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/functional.py
+-rw-rw-rw-   0        0        0      923 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/hook.py
+-rw-rw-rw-   0        0        0      476 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/interrupt.py
+-rw-rw-rw-   0        0        0      996 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/pattern.py
```

### Comparing `py-cone-1.0.8/LICENSE` & `py-cone-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/cone/communication/ding_talk.py` & `py-cone-1.0.9/cone/communication/ding_talk.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/cone/crypto/aes.py` & `py-cone-1.0.9/cone/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/cone/hooks/lib.py` & `py-cone-1.0.9/cone/hooks/lib.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/cone/patterns/singleton.py` & `py-cone-1.0.9/cone/patterns/singleton.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/cone/utils/classes.py` & `py-cone-1.0.9/cone/utils/classes.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/cone/utils/config.py` & `py-cone-1.0.9/cone/utils/config.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/cone/utils/db_utils.py` & `py-cone-1.0.9/cone/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/cone/utils/functional.py` & `py-cone-1.0.9/cone/utils/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,24 +51,33 @@
 
 
 class classproperty:
     """
     Decorator that converts a method with a single cls argument into a property
     that can be accessed directly from the class.
     """
-    def __init__(self, method=None):
-        self.fget = method
+    def __init__(self, getter=None, setter=None):
+        self.fget = getter
+        self.fset = setter
 
     def __get__(self, instance, cls=None):
         return self.fget(cls)
 
+    def __set__(self, instance, value):
+        self.fset(instance, value)
+
     def getter(self, method):
         self.fget = method
         return self
 
+    def setter(self, method):
+        self.fset = method
+        return self
+
+
 class Promise:
     """
     Base class for the proxy class created in the closure of the lazy function.
     It's used to recognize promises in code.
     """
 
     pass
```

### Comparing `py-cone-1.0.8/cone/utils/log.py` & `py-cone-1.0.9/cone/utils/log.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/cone/utils/network/curl.py` & `py-cone-1.0.9/cone/utils/network/curl.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/cone/utils/network/url.py` & `py-cone-1.0.9/cone/utils/network/url.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/cone/utils/os.py` & `py-cone-1.0.9/cone/utils/os.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/py_cone.egg-info/SOURCES.txt` & `py-cone-1.0.9/py_cone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/tests/communication.py` & `py-cone-1.0.9/tests/communication.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/tests/curl.py` & `py-cone-1.0.9/tests/curl.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/tests/functional.py` & `py-cone-1.0.9/tests/functional.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/tests/hook.py` & `py-cone-1.0.9/tests/hook.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.8/tests/pattern.py` & `py-cone-1.0.9/tests/pattern.py`

 * *Files identical despite different names*

