# Comparing `tmp/morastrja-0.8.8.tar.gz` & `tmp/morastrja-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\morastrja-0.8.8.tar", last modified: Mon Apr 24 11:24:43 2023, max compression
+gzip compressed data, was "dist\morastrja-0.8.9.tar", last modified: Wed May 31 13:06:23 2023, max compression
```

## Comparing `morastrja-0.8.8.tar` & `morastrja-0.8.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 11:24:43.353839 morastrja-0.8.8/
--rw-rw-rw-   0        0        0      911 2023-04-24 11:24:43.348845 morastrja-0.8.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 11:24:43.187943 morastrja-0.8.8/ext/
--rw-rw-rw-   0        0        0   144565 2023-04-23 09:36:42.000000 morastrja-0.8.8/ext/cmorastr.c
--rw-rw-rw-   0        0        0     7449 2023-04-22 08:30:35.000000 morastrja-0.8.8/ext/cmorastr_bitap.h
--rw-rw-rw-   0        0        0     6123 2023-04-22 08:33:16.000000 morastrja-0.8.8/ext/cmorastr_pre.h
--rw-rw-rw-   0        0        0    13611 2023-04-22 08:35:20.000000 morastrja-0.8.8/ext/cmorastr_twoway.c
--rw-rw-rw-   0        0        0      958 2023-04-03 21:48:24.000000 morastrja-0.8.8/ext/cmorastr_twoway.h
-drwxrwxrwx   0        0        0        0 2023-04-24 11:24:43.269879 morastrja-0.8.8/morastrja/
--rw-rw-rw-   0        0        0      851 2023-04-21 04:23:48.000000 morastrja-0.8.8/morastrja/__init__.py
--rw-rw-rw-   0        0        0     6557 2023-04-24 07:47:26.000000 morastrja-0.8.8/morastrja/__init__.pyi
--rw-rw-rw-   0        0        0     1297 2023-04-21 00:44:26.000000 morastrja-0.8.8/morastrja/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 11:24:43.342843 morastrja-0.8.8/morastrja/data/
--rw-rw-rw-   0        0        0        0 2022-12-01 03:09:37.000000 morastrja-0.8.8/morastrja/data/__init__.py
--rw-rw-rw-   0        0        0     1407 2023-01-06 11:34:21.000000 morastrja-0.8.8/morastrja/data/table.bak
--rw-rw-rw-   0        0        0     1407 2023-01-17 12:13:16.000000 morastrja-0.8.8/morastrja/data/table.py
--rw-rw-rw-   0        0        0        0 2023-04-24 04:38:52.000000 morastrja-0.8.8/morastrja/py.typed
--rw-rw-rw-   0        0        0       54 2023-04-21 04:20:44.000000 morastrja-0.8.8/morastrja/utils.py
--rw-rw-rw-   0        0        0     1058 2023-04-21 04:19:11.000000 morastrja-0.8.8/morastrja/utils.pyi
-drwxrwxrwx   0        0        0        0 2023-04-24 11:24:43.320710 morastrja-0.8.8/morastrja.egg-info/
--rw-rw-rw-   0        0        0      911 2023-04-24 11:24:42.000000 morastrja-0.8.8/morastrja.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-04-24 11:24:42.000000 morastrja-0.8.8/morastrja.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 11:24:42.000000 morastrja-0.8.8/morastrja.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-24 11:24:42.000000 morastrja-0.8.8/morastrja.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 11:24:43.353839 morastrja-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0     1544 2023-04-24 11:23:08.000000 morastrja-0.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:06:23.929051 morastrja-0.8.9/
+-rw-rw-rw-   0        0        0      911 2023-05-31 13:06:23.928053 morastrja-0.8.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 13:06:23.781577 morastrja-0.8.9/ext/
+-rw-rw-rw-   0        0        0   144565 2023-05-02 21:47:38.000000 morastrja-0.8.9/ext/cmorastr.c
+-rw-rw-rw-   0        0        0     7449 2023-04-22 08:30:35.000000 morastrja-0.8.9/ext/cmorastr_bitap.h
+-rw-rw-rw-   0        0        0     6123 2023-04-22 08:33:16.000000 morastrja-0.8.9/ext/cmorastr_pre.h
+-rw-rw-rw-   0        0        0    13611 2023-04-22 08:35:20.000000 morastrja-0.8.9/ext/cmorastr_twoway.c
+-rw-rw-rw-   0        0        0      958 2023-04-03 21:48:24.000000 morastrja-0.8.9/ext/cmorastr_twoway.h
+drwxrwxrwx   0        0        0        0 2023-05-31 13:06:23.863562 morastrja-0.8.9/morastrja/
+-rw-rw-rw-   0        0        0      851 2023-04-21 04:23:48.000000 morastrja-0.8.9/morastrja/__init__.py
+-rw-rw-rw-   0        0        0     6642 2023-05-30 18:22:58.000000 morastrja-0.8.9/morastrja/__init__.pyi
+-rw-rw-rw-   0        0        0     1297 2023-04-21 00:44:26.000000 morastrja-0.8.9/morastrja/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:06:23.924053 morastrja-0.8.9/morastrja/data/
+-rw-rw-rw-   0        0        0        0 2022-12-01 03:09:37.000000 morastrja-0.8.9/morastrja/data/__init__.py
+-rw-rw-rw-   0        0        0     1407 2023-01-06 11:34:21.000000 morastrja-0.8.9/morastrja/data/table.bak
+-rw-rw-rw-   0        0        0     1407 2023-01-17 12:13:16.000000 morastrja-0.8.9/morastrja/data/table.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 04:38:52.000000 morastrja-0.8.9/morastrja/py.typed
+-rw-rw-rw-   0        0        0       54 2023-04-21 04:20:44.000000 morastrja-0.8.9/morastrja/utils.py
+-rw-rw-rw-   0        0        0     1080 2023-05-30 18:24:35.000000 morastrja-0.8.9/morastrja/utils.pyi
+drwxrwxrwx   0        0        0        0 2023-05-31 13:06:23.901069 morastrja-0.8.9/morastrja.egg-info/
+-rw-rw-rw-   0        0        0      911 2023-05-31 13:06:22.000000 morastrja-0.8.9/morastrja.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-31 13:06:23.000000 morastrja-0.8.9/morastrja.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 13:06:22.000000 morastrja-0.8.9/morastrja.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-31 13:06:22.000000 morastrja-0.8.9/morastrja.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 13:06:23.930050 morastrja-0.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2023-05-31 13:03:26.000000 morastrja-0.8.9/setup.py
```

### Comparing `morastrja-0.8.8/PKG-INFO` & `morastrja-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: morastrja
-Version: 0.8.8
+Version: 0.8.9
 Summary: Mora String for the Japanese Language
 Home-page: https://github.com/Hizuru3/morastrja
 Author: Hizuru
 License: MIT
 Description: 
         This module provides a class that counts morae, based on Japanese syllabaries.
```

### Comparing `morastrja-0.8.8/ext/cmorastr.c` & `morastrja-0.8.9/ext/cmorastr.c`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.8/ext/cmorastr_bitap.h` & `morastrja-0.8.9/ext/cmorastr_bitap.h`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.8/ext/cmorastr_pre.h` & `morastrja-0.8.9/ext/cmorastr_pre.h`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.8/ext/cmorastr_twoway.c` & `morastrja-0.8.9/ext/cmorastr_twoway.c`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.8/ext/cmorastr_twoway.h` & `morastrja-0.8.9/ext/cmorastr_twoway.h`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.8/morastrja/__init__.py` & `morastrja-0.8.9/morastrja/__init__.py`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.8/morastrja/__init__.pyi` & `morastrja-0.8.9/morastrja/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,22 +45,22 @@
             Katakana or hiragana. (Full-width katakana are preferred)
         ignore : bool, optional
             Whether to skip invalid characters or not. Default is False.
         """
 
     def __add__(self: Self, __other: MoraStr | str) -> Self: ...
 
-    def __contains__(self, __sub_morastr: str | MoraStr) -> bool: ...
+    def __contains__(self, __sub_morastr: str | MoraStr) -> bool: ...   # type: ignore[override]
 
     def __eq__(self, __other: object) -> bool: ...
 
     @overload
-    def __getitem__(self: Self, __index: slice) -> Self: ...
-    @overload
     def __getitem__(self, __index: int | SupportsIndex) -> str: ...
+    @overload
+    def __getitem__(self: Self, __index: slice) -> Self: ...
 
     def __getnewargs__(self) -> tuple[str]: ...
 
     def __hash__(self) -> int: ...
 
     def __iter__(self) -> Iterator[str]: ...
 
@@ -90,30 +90,32 @@
     @overload
     def find(self, __sub_morastr: str | MoraStr,
              __start: int | SupportsIndex | None = 0,
              __end: int | SupportsIndex | None = ...) -> int: ...
     @overload
     def find(self, __sub_morastr: str | MoraStr,
              *, charwise: bool = False) -> int: ...
+    @overload
     def find(self, *args, **kwargs):
         "Return the 1st index " \
         "where sub_morastr is found within self[start:end]."
 
     def finditer(self, __sub_morastr: str | MoraStr,
-                 *, charwise: bool = False) -> Iterator[int]: ...
-        "Return an iterator that yields indices of sub_morastr "
+                 *, charwise: bool = False) -> Iterator[int]:
+        "Return an iterator that yields indices of sub_morastr " \
         "found in self."
 
     @overload
     def index(self, __sub_morastr: str | MoraStr,
               __start: int | SupportsIndex | None = 0,
               __end: int | SupportsIndex | None = ...) -> int: ...
     @overload
     def index(self, __sub_morastr: str | MoraStr,
               *, charwise: bool = False) -> int: ...
+    @overload
     def index(self, *args, **kwargs):
         "Like MoraStr.find(), but raises an error " \
         "when sub_morastr is not found."
 
     def removeprefix(self, __prefix: str | MoraStr) -> MoraStr:
         "Return self[len(prefix):] if self starts w/ prefix, " \
         "or a copy of self."
@@ -130,25 +132,27 @@
     @overload
     def rfind(self, __sub_morastr: str | MoraStr,
               __start: int | SupportsIndex | None = 0,
               __end: int | SupportsIndex | None = ...) -> int: ...
     @overload
     def rfind(self, __sub_morastr: str | MoraStr,
               *, charwise: bool = False) -> int: ...
+    @overload
     def rfind(self, *args, **kwargs):
         "Return the last index " \
         "where sub_morastr is found within self[start:end]."
 
     @overload
     def rindex(self, __sub_morastr: str | MoraStr,
                __start: int | SupportsIndex | None = 0,
                __end: int | SupportsIndex | None = ...) -> int: ...
     @overload
     def rindex(self, __sub_morastr: str | MoraStr,
                *, charwise: bool = False) -> int: ...
+    @overload
     def rindex(self, *args, **kwargs):
         "Like MoraStr.rfind(), but raise an error " \
         "when sub_morastr is not found."
 
     def startswith(self, __prefix: str | MoraStr | tuple[str | MoraStr],
                    __start: int | SupportsIndex | None = 0,
                    __end: int | SupportsIndex | None = ...) -> bool:
```

### Comparing `morastrja-0.8.8/morastrja/__main__.py` & `morastrja-0.8.9/morastrja/__main__.py`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.8/morastrja/data/table.bak` & `morastrja-0.8.9/morastrja/data/table.bak`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.8/morastrja/data/table.py` & `morastrja-0.8.9/morastrja/data/table.py`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.8/morastrja/utils.pyi` & `morastrja-0.8.9/morastrja/utils.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,23 @@
                    ou: bool = False, ei: bool = False,
                    nn: bool = True) -> str: ...
 @overload
 def vowel_to_choon(__kana_string: MoraStr, maxrep: int = 1,
                    *, clean: bool = False,
                    ou: bool = False, ei: bool = False,
                    nn: bool = True) -> MoraStr: ...
+@overload
 def vowel_to_choon(self, *args, **kwargs):
     "convert consecutive vowels in kana_string to choonpu"
 
 
 @overload
 def choon_to_vowel(__kana_string: str,
                    *, strict: bool = True,
                    clean: bool = False) -> str: ...
 @overload
 def choon_to_vowel(__kana_string: MoraStr,
                    *, strict: bool = True,
                    clean: bool = False) -> MoraStr: ...
+@overload
 def choon_to_vowel(self, *args, **kwargs):
     "convert choonpu in kana_string to vowel characters"
```

### Comparing `morastrja-0.8.8/morastrja.egg-info/PKG-INFO` & `morastrja-0.8.9/morastrja.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: morastrja
-Version: 0.8.8
+Version: 0.8.9
 Summary: Mora String for the Japanese Language
 Home-page: https://github.com/Hizuru3/morastrja
 Author: Hizuru
 License: MIT
 Description: 
         This module provides a class that counts morae, based on Japanese syllabaries.
```

### Comparing `morastrja-0.8.8/setup.py` & `morastrja-0.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 ext = Extension('morastrja._morastr',
                 sources = ['ext/cmorastr.c'],
                 depends = ['*.h', 'cmorastr_twoway.c'],
                 extra_compile_args=['-O2'])
 
 setup (name = 'morastrja',
-       version = '0.8.8',
+       version = '0.8.9',
        description = 'Mora String for the Japanese Language',
        author = 'Hizuru',
        url = 'https://github.com/Hizuru3/morastrja',
        license = 'MIT',
        long_description = '''
 This module provides a class that counts morae, based on Japanese syllabaries.
 ''',
```

