# Comparing `tmp/ohmytmp-0.0.5.tar.gz` & `tmp/ohmytmp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmytmp-0.0.5.tar", last modified: Mon May 29 10:41:54 2023, max compression
+gzip compressed data, was "ohmytmp-0.0.6.tar", last modified: Wed May 31 07:12:45 2023, max compression
```

## Comparing `ohmytmp-0.0.5.tar` & `ohmytmp-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 10:41:54.433860 ohmytmp-0.0.5/
--rw-rw-rw-   0        0        0     1064 2023-05-28 04:17:27.000000 ohmytmp-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1891 2023-05-29 10:41:54.433341 ohmytmp-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-05-29 10:32:35.000000 ohmytmp-0.0.5/README.md
--rw-rw-rw-   0        0        0      705 2023-05-29 10:33:20.000000 ohmytmp-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 10:41:54.433860 ohmytmp-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 10:41:54.416126 ohmytmp-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 10:41:54.423422 ohmytmp-0.0.5/src/ohmytmp/
--rw-rw-rw-   0        0        0      149 2023-05-29 10:31:50.000000 ohmytmp-0.0.5/src/ohmytmp/__init__.py
--rw-rw-rw-   0        0        0     1752 2023-05-28 14:19:38.000000 ohmytmp-0.0.5/src/ohmytmp/constant.py
--rw-rw-rw-   0        0        0     1071 2023-05-29 10:36:21.000000 ohmytmp-0.0.5/src/ohmytmp/core.py
--rw-rw-rw-   0        0        0     2100 2023-05-29 10:31:02.000000 ohmytmp-0.0.5/src/ohmytmp/guesstype.py
--rw-rw-rw-   0        0        0      745 2023-05-29 10:35:50.000000 ohmytmp-0.0.5/src/ohmytmp/plugin.py
-drwxrwxrwx   0        0        0        0 2023-05-29 10:41:54.432304 ohmytmp-0.0.5/src/ohmytmp.egg-info/
--rw-rw-rw-   0        0        0     1891 2023-05-29 10:41:54.000000 ohmytmp-0.0.5/src/ohmytmp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-29 10:41:54.000000 ohmytmp-0.0.5/src/ohmytmp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 10:41:54.000000 ohmytmp-0.0.5/src/ohmytmp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-29 10:41:54.000000 ohmytmp-0.0.5/src/ohmytmp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 07:12:45.102855 ohmytmp-0.0.6/
+-rw-rw-rw-   0        0        0     1064 2023-05-28 04:17:27.000000 ohmytmp-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1891 2023-05-31 07:12:45.102855 ohmytmp-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-05-30 01:31:43.000000 ohmytmp-0.0.6/README.md
+-rw-rw-rw-   0        0        0      705 2023-05-31 07:12:29.000000 ohmytmp-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:12:45.102855 ohmytmp-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 07:12:45.089854 ohmytmp-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:12:45.097854 ohmytmp-0.0.6/src/ohmytmp/
+-rw-rw-rw-   0        0        0     1876 2023-05-30 15:15:40.000000 ohmytmp-0.0.6/src/ohmytmp/__constant.py
+-rw-rw-rw-   0        0        0     1818 2023-05-31 07:03:57.000000 ohmytmp-0.0.6/src/ohmytmp/__core.py
+-rw-rw-rw-   0        0        0     2132 2023-05-30 15:15:43.000000 ohmytmp-0.0.6/src/ohmytmp/__guesstype.py
+-rw-rw-rw-   0        0        0      138 2023-05-30 15:22:50.000000 ohmytmp-0.0.6/src/ohmytmp/__init__.py
+-rw-rw-rw-   0        0        0     1915 2023-05-30 15:15:34.000000 ohmytmp-0.0.6/src/ohmytmp/__plugin.py
+-rw-rw-rw-   0        0        0      155 2023-05-30 15:22:56.000000 ohmytmp-0.0.6/src/ohmytmp/plugin.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:12:45.101856 ohmytmp-0.0.6/src/ohmytmp.egg-info/
+-rw-rw-rw-   0        0        0     1891 2023-05-31 07:12:45.000000 ohmytmp-0.0.6/src/ohmytmp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-05-31 07:12:45.000000 ohmytmp-0.0.6/src/ohmytmp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:12:45.000000 ohmytmp-0.0.6/src/ohmytmp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 07:12:45.000000 ohmytmp-0.0.6/src/ohmytmp.egg-info/top_level.txt
```

### Comparing `ohmytmp-0.0.5/LICENSE` & `ohmytmp-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmytmp-0.0.5/PKG-INFO` & `ohmytmp-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmytmp
-Version: 0.0.5
+Version: 0.0.6
 Summary: ohmytmp-core
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
```

### Comparing `ohmytmp-0.0.5/pyproject.toml` & `ohmytmp-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ohmytmp"
-version = "0.0.5"
+version = "0.0.6"
 description = "ohmytmp-core"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["file"]
 
 authors = [
```

### Comparing `ohmytmp-0.0.5/src/ohmytmp/constant.py` & `ohmytmp-0.0.6/src/ohmytmp/__constant.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,19 @@
                 ans[i] = eval('self.%s' % i)
         return ans
 
 
 class __func(Const):
     def __init__(self) -> None:
         super().__init__()
-        self.ANALYSIS = 'analysis'
-        self.AFTER = 'after'
+        self.GUESSTYPE = 0x08
+        self.ANALYSIS = 0x18
+        self.ADDTAGS = 0x28
+        self.DESTINATION = 0x38
+        self.AFTER = 0x48
 
 
 FUNC = __func()
 
 
 class __type(Const):
     def __init__(self) -> None:
@@ -63,7 +66,10 @@
     def to_taglist(self, addlist: list = ['EXT', 'TYPE']) -> list:
         ans = self.TAGS.copy()
         d = self.to_dict()
         for i in addlist:
             if i in d and isinstance(d[i], str):
                 ans.append('%s_%s' % (i, d[i]))
         return ans
+
+
+__all__ = ('FUNC', 'TYPE', 'Info')
```

### Comparing `ohmytmp-0.0.5/src/ohmytmp/guesstype.py` & `ohmytmp-0.0.6/src/ohmytmp/__guesstype.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import mimetypes
 
-from .constant import TYPE, Info
+from .__constant import TYPE, Info
 
 
 def get_ext(p: str) -> str:
     return os.path.splitext(p)[1][1:]
 
 
 def guess_mime(p: str) -> str:
@@ -67,7 +67,10 @@
     return ext_re.get(e, TYPE.UNKNOWN)
 
 
 def guesstype(info: Info) -> None:
     info.TYPE = guess_ext(info.EXT)
     if info.TYPE == TYPE.UNKNOWN:
         info.TYPE = guess_mime(info.SRC)
+
+
+__all__ = ('guesstype',)
```

### Comparing `ohmytmp-0.0.5/src/ohmytmp.egg-info/PKG-INFO` & `ohmytmp-0.0.6/src/ohmytmp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmytmp
-Version: 0.0.5
+Version: 0.0.6
 Summary: ohmytmp-core
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
```

