# Comparing `tmp/viledatools-1.0.8.tar.gz` & `tmp/viledatools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\viledatools-1.0.8.tar", last modified: Fri Feb 26 09:35:29 2021, max compression
+gzip compressed data, was "dist\viledatools-1.0.9.tar", last modified: Fri Mar 26 15:49:25 2021, max compression
```

## Comparing `viledatools-1.0.8.tar` & `viledatools-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2021-02-26 09:35:29.835702 viledatools-1.0.8/
--rw-rw-rw-   0        0        0      681 2021-02-26 09:35:29.834701 viledatools-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      163 2021-02-16 17:20:08.000000 viledatools-1.0.8/README.rst
--rw-rw-rw-   0        0        0       42 2021-02-26 09:35:29.835702 viledatools-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1022 2021-02-26 09:35:19.000000 viledatools-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-02-26 09:35:29.824702 viledatools-1.0.8/viledatools/
--rw-rw-rw-   0        0        0     1036 2021-02-26 09:33:57.000000 viledatools-1.0.8/viledatools/__init__.py
--rw-rw-rw-   0        0        0    32291 2021-02-26 09:33:22.000000 viledatools-1.0.8/viledatools/apiutils.py
--rw-rw-rw-   0        0        0     6369 2021-02-16 17:20:08.000000 viledatools-1.0.8/viledatools/diagonaltablewalk.py
--rw-rw-rw-   0        0        0    10144 2021-02-16 17:20:08.000000 viledatools-1.0.8/viledatools/fatask.py
--rw-rw-rw-   0        0        0    21622 2021-02-25 19:10:08.000000 viledatools-1.0.8/viledatools/importcellparser.py
--rw-rw-rw-   0        0        0     6681 2021-02-25 18:50:46.000000 viledatools-1.0.8/viledatools/importsheetparser.py
--rw-rw-rw-   0        0        0      471 2021-02-16 17:20:08.000000 viledatools-1.0.8/viledatools/viledaexceptions.py
--rw-rw-rw-   0        0        0     4284 2021-02-25 19:09:48.000000 viledatools-1.0.8/viledatools/viledautils.py
-drwxrwxrwx   0        0        0        0 2021-02-26 09:35:29.833720 viledatools-1.0.8/viledatools.egg-info/
--rw-rw-rw-   0        0        0      681 2021-02-26 09:35:29.000000 viledatools-1.0.8/viledatools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2021-02-26 09:35:29.000000 viledatools-1.0.8/viledatools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-26 09:35:29.000000 viledatools-1.0.8/viledatools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-02-16 18:01:17.000000 viledatools-1.0.8/viledatools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2021-02-26 09:35:29.000000 viledatools-1.0.8/viledatools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-02-26 09:35:29.000000 viledatools-1.0.8/viledatools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-03-26 15:49:25.543812 viledatools-1.0.9/
+-rw-rw-rw-   0        0        0      681 2021-03-26 15:49:25.543812 viledatools-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2021-02-16 17:20:08.000000 viledatools-1.0.9/README.rst
+-rw-rw-rw-   0        0        0       42 2021-03-26 15:49:25.543812 viledatools-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2021-03-26 15:35:50.000000 viledatools-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-03-26 15:49:25.532810 viledatools-1.0.9/viledatools/
+-rw-rw-rw-   0        0        0     1036 2021-03-26 15:35:40.000000 viledatools-1.0.9/viledatools/__init__.py
+-rw-rw-rw-   0        0        0    32293 2021-03-17 08:45:02.000000 viledatools-1.0.9/viledatools/apiutils.py
+-rw-rw-rw-   0        0        0     6369 2021-02-16 17:20:08.000000 viledatools-1.0.9/viledatools/diagonaltablewalk.py
+-rw-rw-rw-   0        0        0    10144 2021-02-16 17:20:08.000000 viledatools-1.0.9/viledatools/fatask.py
+-rw-rw-rw-   0        0        0    24208 2021-03-26 15:47:46.000000 viledatools-1.0.9/viledatools/importcellparser.py
+-rw-rw-rw-   0        0        0     6681 2021-02-25 18:50:46.000000 viledatools-1.0.9/viledatools/importsheetparser.py
+-rw-rw-rw-   0        0        0      471 2021-02-16 17:20:08.000000 viledatools-1.0.9/viledatools/viledaexceptions.py
+-rw-rw-rw-   0        0        0     4704 2021-03-26 15:40:05.000000 viledatools-1.0.9/viledatools/viledautils.py
+drwxrwxrwx   0        0        0        0 2021-03-26 15:49:25.541810 viledatools-1.0.9/viledatools.egg-info/
+-rw-rw-rw-   0        0        0      681 2021-03-26 15:49:24.000000 viledatools-1.0.9/viledatools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2021-03-26 15:49:25.000000 viledatools-1.0.9/viledatools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-03-26 15:49:24.000000 viledatools-1.0.9/viledatools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-02-16 18:01:17.000000 viledatools-1.0.9/viledatools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2021-03-26 15:49:24.000000 viledatools-1.0.9/viledatools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2021-03-26 15:49:24.000000 viledatools-1.0.9/viledatools.egg-info/top_level.txt
```

### Comparing `viledatools-1.0.8/PKG-INFO` & `viledatools-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: viledatools
-Version: 1.0.8
+Version: 1.0.9
 Summary: Classes and functions to use for development of intregration software
 Home-page: https://www.vileda-professional.com/
 Author: FHCS GmbH
 Author-email: support@fhcs.zendesk.com
 License: Creative Commons Attribution 4.0 International
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `viledatools-1.0.8/setup.py` & `viledatools-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 py setup.py sdist bdist_wheel
 twine upload --repository pypi dist/*
 """
 
 from setuptools import setup
 
 setup(name='viledatools',
-      version='1.0.8',
+      version='1.0.9',
       packages=['viledatools'],
       url='https://www.vileda-professional.com/',
       license='Creative Commons Attribution 4.0 International',
       author='FHCS GmbH',
       author_email='support@fhcs.zendesk.com',
       description='Classes and functions to use for development of intregration software',
       install_requires=['aiohttp>=3.7.3', 'openpyxl>=3.0.6'],
```

### Comparing `viledatools-1.0.8/viledatools/__init__.py` & `viledatools-1.0.9/viledatools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding=utf-8
 """
 viledatools
 """
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 from typing import Tuple
 
 from .apiutils import (FARequests as FARequests, fagetrefs as fagetrefs, getcookieval as getcookieval, gettag as gettag)
 from .diagonaltablewalk import DiagonalTableWalk as DiagonalTableWalk
 from .fatask import FATask as FATask
 from .importcellparser import ImportCellParser as ImportCellParser
```

### Comparing `viledatools-1.0.8/viledatools/apiutils.py` & `viledatools-1.0.9/viledatools/apiutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     for _i in _orig:
         if _i in _ALLOWED:
             _pre += _i
         else:
             _pre += chr(0x0020)
     return _pre.upper().split()
 
+
 def getcookieval(httpsession: aiohttp.ClientSession, cname: str) -> Optional[str]:
     """
     Extract required cookie from aiohttp.CookieJar instance from aiohttp session.
 
     :param httpsession: Active aiohttp session to use
     :param cname: String name of cookie to extract
     :return: Value of cookie or None if no cookie existing
```

### Comparing `viledatools-1.0.8/viledatools/diagonaltablewalk.py` & `viledatools-1.0.9/viledatools/diagonaltablewalk.py`

 * *Files identical despite different names*

### Comparing `viledatools-1.0.8/viledatools/fatask.py` & `viledatools-1.0.9/viledatools/fatask.py`

 * *Files identical despite different names*

### Comparing `viledatools-1.0.8/viledatools/importcellparser.py` & `viledatools-1.0.9/viledatools/importcellparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,46 @@
         :return: True if cell value is parsed as yes, False otherwise
         """
         # Trim, uppercase and compare
         if str(cellobject.value).upper().strip() in ["ДА", "АГА", "Д", "YES", "YEP", "Y", "YEAH", "JA", "J"]:
             return True
         return False
 
+    def _parseintseq(self, cellobject: openpyxl.cell.cell.Cell, allowedvals: List[int]) -> Union[List[str], None]:
+        """
+        Parse value of cell containing string with semicolon separated integers into a list of stringified integers,
+        values in the MS Excel sheet must be given with ; (semicolon) separator
+
+        :param cellobject: openpyxl cell object to parse
+        :param allowedvals: list of allowed integers, if parsed integer not from this list, exception is raised
+        :return: list of stringified integers parsed from the cell
+        """
+        # Trim and split by semicolons
+        _value_raw_list = cellobject.value.strip().split(";")
+        # Trim each item and filter out empty ones, fill filtered list
+        _value_numbers_set = set()
+        for _item in _value_raw_list:
+            _trimmed_item = _item.strip()
+            if _trimmed_item:
+                try:
+                    _trimmed_item_int = int(_trimmed_item)
+                except Exception:
+                    raise ImportCellParserException((f"_parseintseq(): Wrong value in the cell: "
+                                                     f"{_trimmed_item}, values in the list must be integers divided by "
+                                                     f"semicolons"))
+                if _trimmed_item_int in allowedvals:
+                    _value_numbers_set.add(str(_trimmed_item_int))
+                else:
+                    raise ImportCellParserException((f"_parseintseq(): Wrong value in the cell: "
+                                                     f"{_trimmed_item_int}, integer values in the list must belong to "
+                                                     f"{allowedvals}"))
+        _value_numbers_list = list(_value_numbers_set)
+        _value_numbers_list.sort()
+        return _value_numbers_list
+
     def IQF001SITE(self, cellobject: openpyxl.cell.cell.Cell) -> Union[str, None]:
         """
         Parse site name, normalize with strnorm()
 
         :param cellobject: openpyxl cell object to parse
         :return: normalized site name string parsed from the cell
         """
@@ -276,51 +308,29 @@
         if _value_int < 1:
             raise ImportCellParserException((f"IQF010FREQINTVL: Value in the cell: {_value} out of range, "
                                              f"frequency interval must be greater than 0"))
         return _value_int
 
     def IQF011FREQDAYS(self, cellobject: openpyxl.cell.cell.Cell) -> Union[List[str], None]:
         """
-        Parse task recurrence days as list of stringified integers, where ["1", "2", "3", "4", "5", "6", '7']
+        Parse task recurrence days as list of stringified integers, where ["1", "2", "3", "4", "5", "6", "7"]
         corresponds to [Mon, Tue, Wed, Thu, Fri, Sat, Sun], list values in the MS Excel sheet must
         be given with ; (semicolon) separator
 
         :param cellobject: openpyxl cell object to parse
         :return: list of stringified integers parsed from the cell
         """
         if not isinstance(cellobject, Cell):
             raise TypeError(f"Provided cell object type {type(cellobject)}, type openpyxl.cell.cell.Cell required")
         if cellobject.value is None:
             return None
-        _value = cellobject.value
-        if not isinstance(_value, str):
+        if not isinstance(cellobject.value, str):
             raise ImportCellParserException((f"IQF011FREQDAYS: Cell contents type is {type(cellobject)}, "
                                              f"string type required"))
-        # Trim and split by semicolons
-        _value_raw_list = _value.strip().split(";")
-        # Trim each item and filter out empty ones, fill filtered list
-        _value_numbers_set = set()
-        for _item in _value_raw_list:
-            _trimmed_item = _item.strip()
-            if _trimmed_item:
-                try:
-                    _trimmed_item_int = int(_trimmed_item)
-                except Exception:
-                    raise ImportCellParserException((f"IQF011FREQDAYS: Wrong value in the cell: "
-                                                     f"{_trimmed_item}, values in the list must be integers divided by "
-                                                     f"semicolons"))
-                if _trimmed_item_int in [1, 2, 3, 4, 5, 6, 7]:
-                    _value_numbers_set.add(str(_trimmed_item_int))
-                else:
-                    raise ImportCellParserException((f"IQF011FREQDAYS: Wrong value in the cell: "
-                                                     f"{_trimmed_item_int}, integer values in the list must be from "
-                                                     f"1 to 7"))
-        _value_numbers_list = list(_value_numbers_set)
-        _value_numbers_list.sort()
-        return _value_numbers_list
+        return self._parseintseq(cellobject, [1, 2, 3, 4, 5, 6, 7])
 
     def IQF012ATMID(self, cellobject: openpyxl.cell.cell.Cell) -> Union[int, None]:
         """
         Made for mosklining domain
 
         Parse ATM ID, convert to int
 
@@ -456,7 +466,43 @@
         :return: stringified and trimmed cell value
         """
         if not isinstance(cellobject, Cell):
             raise TypeError(f"Provided cell object type {type(cellobject)}, type openpyxl.cell.cell.Cell required")
         if cellobject.value is None:
             return None
         return str(cellobject.value).strip()
+
+    def IQF021FREQMONTHS(self, cellobject: openpyxl.cell.cell.Cell) -> Union[List[str], None]:
+        """
+        Parse task recurrence months as list of stringified integers, where
+        ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11", "12"] corresponds to
+        [Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Oct, Nov, Dec], list values in the MS Excel sheet must
+        be given with ; (semicolon) separator
+
+        :param cellobject: openpyxl cell object to parse
+        :return: list of stringified integers parsed from the cell
+        """
+        if not isinstance(cellobject, Cell):
+            raise TypeError(f"Provided cell object type {type(cellobject)}, type openpyxl.cell.cell.Cell required")
+        if cellobject.value is None:
+            return None
+        if not isinstance(cellobject.value, str):
+            raise ImportCellParserException((f"IQF021FREQMONTHS: Cell contents type is {type(cellobject)}, "
+                                             f"string type required"))
+        return self._parseintseq(cellobject, [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])
+
+    def IQF022SAMEDAYOFWEEK(self, cellobject: openpyxl.cell.cell.Cell) -> Union[bool, None]:
+        """
+        If monthly recurrence is set, then this parameter defines whether task repeats same day of the week, or same
+        date of each month
+
+        If "yes" then task will repeat same day of the same week as first date of the task, if "no" - then task
+        will repeat same date of the month
+
+        :param cellobject: openpyxl cell object to parse
+        :return: True if cell value is parsed as yes, False otherwise
+        """
+        if not isinstance(cellobject, Cell):
+            raise TypeError(f"Provided cell object type {type(cellobject)}, type openpyxl.cell.cell.Cell required")
+        if cellobject.value is None:
+            return None
+        return self._parseyesno(cellobject)
```

### Comparing `viledatools-1.0.8/viledatools/importsheetparser.py` & `viledatools-1.0.9/viledatools/importsheetparser.py`

 * *Files identical despite different names*

### Comparing `viledatools-1.0.8/viledatools/viledautils.py` & `viledatools-1.0.9/viledatools/viledautils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding=utf-8
 """
 (C) FHCS GmbH
 
 Generic ViledaUtils class implementing static methods to use for MS Excel import / export and API communication
 """
 import logging
+from datetime import datetime, timedelta
 from os import walk
 from traceback import format_exc
 from typing import Any, Dict, List
 
 from openpyxl import load_workbook
 
 from .importsheetparser import ImportSheetParser
@@ -86,7 +87,19 @@
         # Log full imported list
         _log_str_reclist = str()
         for _r in reclist:
             _log_str_reclist += str(_r) + "\n"
         tolog.debug(_log_str_reclist)
         # And finally return the list
         return reclist
+
+    @staticmethod
+    def jsondef(obj: Any) -> str:
+        """
+        :param obj: object unknown to json.dump
+        :return: serialized value of object unknown to json.dump
+        """
+        if isinstance(obj, timedelta):
+            return str(obj)
+        elif isinstance(obj, datetime):
+            return obj.strftime("%d.%m.%Y")
+        return repr(obj)
```

### Comparing `viledatools-1.0.8/viledatools.egg-info/PKG-INFO` & `viledatools-1.0.9/viledatools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: viledatools
-Version: 1.0.8
+Version: 1.0.9
 Summary: Classes and functions to use for development of intregration software
 Home-page: https://www.vileda-professional.com/
 Author: FHCS GmbH
 Author-email: support@fhcs.zendesk.com
 License: Creative Commons Attribution 4.0 International
 Description: UNKNOWN
 Platform: UNKNOWN
```

