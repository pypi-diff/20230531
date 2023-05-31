# Comparing `tmp/countess-0.0.28.tar.gz` & `tmp/countess-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.28.tar", last modified: Fri May 26 07:10:38 2023, max compression
+gzip compressed data, was "countess-0.0.29.tar", last modified: Wed May 31 04:03:08 2023, max compression
```

## Comparing `countess-0.0.28.tar` & `countess-0.0.29.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.627911 countess-0.0.28/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.28/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       26 2023-05-25 01:44:18.000000 countess-0.0.28/MANIFEST.in
--rw-rw-r--   0 nick      (1000) nick      (1000)     3477 2023-05-26 07:10:38.627911 countess-0.0.28/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-05-26 07:08:39.000000 countess-0.0.28/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.623911 countess-0.0.28/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-05-26 07:08:45.000000 countess-0.0.28/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.623911 countess-0.0.28/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.28/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      415 2023-05-25 01:44:18.000000 countess-0.0.28/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4157 2023-05-25 01:44:18.000000 countess-0.0.28/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1910 2023-05-25 01:44:18.000000 countess-0.0.28/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    16461 2023-05-26 07:02:31.000000 countess-0.0.28/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5938 2023-05-26 07:05:39.000000 countess-0.0.28/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13181 2023-05-26 07:05:55.000000 countess-0.0.28/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.623911 countess-0.0.28/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.28/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    18762 2023-05-26 07:05:55.000000 countess-0.0.28/countess/gui/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-05-25 01:44:18.000000 countess-0.0.28/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    34169 2023-05-26 07:05:56.000000 countess-0.0.28/countess/gui/main.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    12797 2023-05-26 06:50:03.000000 countess-0.0.28/countess/gui/tabular.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.627911 countess-0.0.28/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5969 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3711 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/data_table.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1236 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/expression.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2160 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4385 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/hdf5.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3051 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/log_score.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2562 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/mutagenize.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5520 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1477 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/python.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6784 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2039 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/sequence.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2496 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/variant.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.28/countess/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.627911 countess-0.0.28/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.28/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    12859 2023-05-25 01:44:18.000000 countess-0.0.28/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.623911 countess-0.0.28/countess.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     3477 2023-05-26 07:10:38.000000 countess-0.0.28/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1068 2023-05-26 07:10:38.000000 countess-0.0.28/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-26 07:10:38.000000 countess-0.0.28/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      997 2023-05-26 07:10:38.000000 countess-0.0.28/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      201 2023-05-26 07:10:38.000000 countess-0.0.28/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-05-26 07:10:38.000000 countess-0.0.28/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     2809 2023-05-26 06:01:26.000000 countess-0.0.28/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-26 07:10:38.627911 countess-0.0.28/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.28/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.627911 countess-0.0.28/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      480 2023-05-25 01:44:18.000000 countess-0.0.28/tests/test_gui.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.934222 countess-0.0.29/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.29/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       26 2023-05-25 01:44:18.000000 countess-0.0.29/MANIFEST.in
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3477 2023-05-31 04:03:08.934222 countess-0.0.29/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-05-31 04:01:08.000000 countess-0.0.29/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.926222 countess-0.0.29/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-05-31 04:00:59.000000 countess-0.0.29/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.930222 countess-0.0.29/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.29/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      415 2023-05-25 01:44:18.000000 countess-0.0.29/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4157 2023-05-25 01:44:18.000000 countess-0.0.29/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1910 2023-05-25 01:44:18.000000 countess-0.0.29/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    16561 2023-05-31 03:55:05.000000 countess-0.0.29/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5938 2023-05-26 07:05:39.000000 countess-0.0.29/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13419 2023-05-31 03:55:05.000000 countess-0.0.29/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.930222 countess-0.0.29/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.29/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18816 2023-05-31 03:55:05.000000 countess-0.0.29/countess/gui/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-05-25 01:44:18.000000 countess-0.0.29/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    14766 2023-05-31 03:55:05.000000 countess-0.0.29/countess/gui/main.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13294 2023-05-30 06:54:25.000000 countess-0.0.29/countess/gui/tabular.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19791 2023-05-30 01:24:26.000000 countess-0.0.29/countess/gui/tree.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.934222 countess-0.0.29/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.29/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5969 2023-05-31 03:55:05.000000 countess-0.0.29/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3711 2023-05-31 03:55:05.000000 countess-0.0.29/countess/plugins/data_table.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1236 2023-05-25 01:44:18.000000 countess-0.0.29/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2160 2023-05-25 01:44:18.000000 countess-0.0.29/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4699 2023-05-31 03:57:07.000000 countess-0.0.29/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-05-25 01:44:18.000000 countess-0.0.29/countess/plugins/hdf5.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3051 2023-05-31 03:55:05.000000 countess-0.0.29/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-05-25 01:44:18.000000 countess-0.0.29/countess/plugins/log_score.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2562 2023-05-25 01:44:18.000000 countess-0.0.29/countess/plugins/mutagenize.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5520 2023-05-31 03:55:05.000000 countess-0.0.29/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1560 2023-05-31 03:55:05.000000 countess-0.0.29/countess/plugins/python.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6280 2023-05-31 03:57:59.000000 countess-0.0.29/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2194 2023-05-31 03:55:05.000000 countess-0.0.29/countess/plugins/sequence.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2238 2023-05-31 03:58:42.000000 countess-0.0.29/countess/plugins/variant.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.29/countess/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.934222 countess-0.0.29/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.29/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    12859 2023-05-25 01:44:18.000000 countess-0.0.29/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.926222 countess-0.0.29/countess.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3477 2023-05-31 04:03:08.000000 countess-0.0.29/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1089 2023-05-31 04:03:08.000000 countess-0.0.29/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-31 04:03:08.000000 countess-0.0.29/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      997 2023-05-31 04:03:08.000000 countess-0.0.29/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      201 2023-05-31 04:03:08.000000 countess-0.0.29/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-05-31 04:03:08.000000 countess-0.0.29/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2809 2023-05-26 06:01:26.000000 countess-0.0.29/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-31 04:03:08.934222 countess-0.0.29/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.29/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:03:08.934222 countess-0.0.29/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      480 2023-05-25 01:44:18.000000 countess-0.0.29/tests/test_gui.py
```

### Comparing `countess-0.0.28/LICENSE.txt` & `countess-0.0.29/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/PKG-INFO` & `countess-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.28
+Version: 0.0.29
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -12,15 +12,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.28
+# CountESS 0.0.29
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.28/README.md` & `countess-0.0.29/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.28
+# CountESS 0.0.29
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.28/countess/core/config.py` & `countess-0.0.29/countess/core/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess/core/logger.py` & `countess-0.0.29/countess/core/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess/core/parameters.py` & `countess-0.0.29/countess/core/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,23 +323,23 @@
 class ColumnChoiceParam(ChoiceParam):
     """A ChoiceParam which DaskTransformPlugin knows
     it should automatically update with a list of columns"""
 
     def set_column_choices(self, choices):
         self.set_choices(list(choices))
 
-
-class ColumnOrIndexChoiceParam(ColumnChoiceParam):
-    INDEX_VALUE = "— INDEX —"
-
-    def set_choices(self, choices: Iterable[str]):
-        super().set_choices([self.INDEX_VALUE] + list(choices))
-
-    def is_index(self):
-        return self.value == self.INDEX_VALUE
+    def get_column(self, df):
+        if self.value in df.columns:
+            return df[self.value]
+        elif self.value == df.index.name:
+            return df.index
+        elif hasattr(df.index, "names") and self.value in df.index.names:
+            return df.index.to_frame()[self.value]
+        else:
+            raise ValueError(f"Column {self.value} not found")
 
 
 class ColumnOrNoneChoiceParam(ColumnChoiceParam):
     NONE_VALUE = "— NONE —"
 
     def set_choices(self, choices: Iterable[str]):
         super().set_choices([self.NONE_VALUE] + list(choices))
```

### Comparing `countess-0.0.28/countess/core/pipeline.py` & `countess-0.0.29/countess/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess/core/plugins.py` & `countess-0.0.29/countess/core/plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,15 +209,20 @@
 
 
 class PandasTransformPlugin(PandasBasePlugin):
     input_columns: list[str] = []
 
     def prepare_df(self, df: pd.DataFrame, logger: Logger):
         assert isinstance(df, pd.DataFrame)
-        self.input_columns = list(df.columns)
+        if hasattr(df.index, "names"):
+            self.input_columns = [n for n in df.index.names if n] + list(df.columns)
+        elif df.index.name:
+            self.input_columns = [df.index.name] + list(df.columns)
+        else:
+            self.input_columns = list(df.columns)
 
         for p in self.parameters.values():
             p.set_column_choices(self.input_columns)
 
     # XXX prepare and run handle multiple inputs differntly?
 
     def prepare(
```

### Comparing `countess-0.0.28/countess/gui/config.py` & `countess-0.0.29/countess/gui/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,15 @@
                     else tk.NORMAL
                 )
         elif isinstance(self.parameter, MultiParam):
             self.update_subwrappers(self.parameter.params.values(), None)
         elif isinstance(self.parameter, ChoiceParam):
             self.entry.destroy()
             choices = self.parameter.choices or [""]
+            self.var.set(self.parameter.value)
             self.entry = tk.OptionMenu(self.tk_parent, self.var, *choices)
             self.entry.grid(sticky=tk.EW, padx=10, pady=5)
         elif isinstance(self.parameter, BooleanParam):
             self.set_checkbox_value()
         elif isinstance(self.parameter, TextParam):
             if self.parameter.read_only:
                 self.entry["state"] = "normal"
@@ -373,15 +374,15 @@
         if self.callback is not None:
             self.callback(self.parameter)
 
     def change_file_callback(self, *_):
         file_types = self.parameter.file_types
         filename = filedialog.askopenfilename(filetypes=file_types)
         self.parameter.value = filename
-        self.var.set(self.parameter.value)
+        self.entry["text"] = self.parameter.value
         self.callback(self.parameter)
 
     def set_value(self, value):
         # self.parameter.value is a property, and some cleaning may occur, so we just
         # check before and after to see if it has changed.
         old_parameter_value = self.parameter.value
         self.parameter.value = value
```

### Comparing `countess-0.0.28/countess/gui/logger.py` & `countess-0.0.29/countess/gui/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess/gui/tabular.py` & `countess-0.0.29/countess/gui/tabular.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
 import tkinter as tk
 from functools import partial
-from math import ceil, floor
+from math import ceil, floor, isnan
 from tkinter import ttk
 
 from pandas.api.types import is_integer_dtype, is_numeric_dtype
 
 # XXX columns should automatically resize based on information
 # from __column_xscrollcommand which can tell if they're
 # overflowing.  Or maybe use
@@ -13,24 +13,35 @@
 # etc etc.
 
 
 def column_format_for(df_column):
     if is_numeric_dtype(df_column.dtype):
         # Work out the maximum width required to represent the integer part in this
         # column, so we can pad values to that width.
-        width = max(len(str(floor(df_column.min()))), len(str(ceil(df_column.max()))))
+        column_min = df_column.min()
+        if type(column_min) is float and isnan(column_min):
+            column_min = 0
+        column_max = df_column.max()
+        if type(column_max) is float and isnan(column_max):
+            column_max = 0
+        width = max(len(str(floor(column_min))), len(str(ceil(column_max))))
         if is_integer_dtype(df_column.dtype):
             return f"%{width}d"
         else:
-            return f"%{width+12}.12f"
+            # leave room for the point and 12 decimals.
+            # format_value will remove trailing 0s.
+            return f"%{width+13}.12f"
     else:
         return "%s"
 
 
 def format_value(value, column_format):
+    if value is None or (type(value) is float and isnan(value)):
+        return "—"
+
     # remove trailing 0's from floats (%g doesn't align correctly)
     try:
         if column_format.endswith("f"):
             return (column_format % value).rstrip("0")
         else:
             return column_format % value
     except TypeError:
@@ -75,14 +86,15 @@
             # MultiIndex case
             column_names = list(self.dataframe.index.names) + list(self.dataframe.columns)
             column_dtypes = list(self.dataframe.index.dtypes) + list(self.dataframe.dtypes)
             index_frame = self.dataframe.index.to_frame()
             self.column_formats = [
                 column_format_for(index_frame[name]) for name in dataframe.index.names
             ] + [column_format_for(dataframe[name]) for name in dataframe.columns]
+            index_cols = len(self.dataframe.index.names)
         elif self.dataframe.index.name:
             # a simple Index, with a name
             column_names = [self.dataframe.index.name] + list(self.dataframe.columns)
             column_dtypes = [self.dataframe.index.dtype] + list(self.dataframe.dtypes)
             self.column_formats = [column_format_for(dataframe.index)] + [
                 column_format_for(dataframe[name]) for name in dataframe.columns
             ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `countess-0.0.28/countess/plugins/csv.py` & `countess-0.0.29/countess/plugins/csv.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess/plugins/data_table.py` & `countess-0.0.29/countess/plugins/data_table.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess/plugins/expression.py` & `countess-0.0.29/countess/plugins/expression.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess/plugins/fastq.py` & `countess-0.0.29/countess/plugins/fastq.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess/plugins/group_by.py` & `countess-0.0.29/countess/plugins/group_by.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import pandas as pd
 from pandas.api.types import is_numeric_dtype
 
 from countess import VERSION
 from countess.core.parameters import (
     BaseParam,
     BooleanParam,
-    ColumnOrIndexChoiceParam,
     PerColumnArrayParam,
     TabularMultiParam,
     TextParam,
 )
 from countess.core.plugins import PandasTransformPlugin
 
 
 def _column_renamer(col):
-    print(f"CR {col}")
     if isinstance(col, tuple):
         if col[-1] == "first":
             return "__".join(col[:-1])
         else:
             return "__".join(col)
     return col
 
@@ -81,22 +79,27 @@
         assert isinstance(self.parameters["columns"], PerColumnArrayParam)
         column_parameters = list(zip(self.input_columns, self.parameters["columns"]))
 
         index_cols = [col for col, col_param in column_parameters if col_param["index"].value]
         agg_ops = dict(
             (
                 col,
-                [k if k != "index" else "first" for k, pp in col_param.params.items() if pp.value],
+                [k for k, pp in col_param.params.items() if pp.value and k != "index"],
             )
             for col, col_param in column_parameters
+            if any(pp.value for k, pp in col_param.params.items() if k != "index")
         )
 
         try:
-            dfo = df.groupby(index_cols or df.index).agg(agg_ops)
-            dfo.columns = [_column_renamer(col) for col in dfo.columns.values]  # type: ignore
+            if agg_ops:
+                dfo = df.groupby(index_cols or df.index).agg(agg_ops)
+                dfo.columns = [_column_renamer(col) for col in dfo.columns.values]  # type: ignore
+            else:
+                # defaults to just a 'count' column.
+                dfo = df.assign(count=1).groupby(index_cols or df.index).count()
         except ValueError as exc:
             logger.exception(exc)
             return pd.DataFrame()
 
         if self.parameters["join"].value:
             return df.merge(dfo, how="left", left_on=index_cols, right_on=index_cols)
         else:
@@ -111,18 +114,22 @@
     version = VERSION
 
     parameters = {
         "groupby": PerColumnArrayParam("Group By", BooleanParam("Index")),
         "expr": TextParam("Expression"),
     }
 
+    # XXX not very useful in its current form.
+    # probably better off making this part of Expression
+    # plugin, or something.
+
     def run_df(self, df: pd.DataFrame, logger) -> pd.DataFrame:
-        assert isinstance(self.parameters["column"], ColumnOrIndexChoiceParam)
-        if self.parameters["column"].is_index():
-            col = df.index
-        else:
-            col = df[self.parameters["column"].value]
-        oper = self.parameters["operation"].value
+        assert isinstance(self.parameters["groupby"], PerColumnArrayParam)
+        cols = [
+            col for col, param in zip(self.input_columns, self.parameters["groupby"]) if param.value
+        ]
+        expr = self.parameters["expr"].value
+
+        if not cols:
+            return df
 
-        df2 = df.groupby(col).agg(oper)
-        assert isinstance(df2, pd.DataFrame)
-        return df2
+        return df.reset_index().groupby(cols).agg(expr.strip())
```

### Comparing `countess-0.0.28/countess/plugins/hdf5.py` & `countess-0.0.29/countess/plugins/hdf5.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess/plugins/join.py` & `countess-0.0.29/countess/plugins/join.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess/plugins/mutagenize.py` & `countess-0.0.29/countess/plugins/mutagenize.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess/plugins/pivot.py` & `countess-0.0.29/countess/plugins/pivot.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess/plugins/python.py` & `countess-0.0.29/countess/plugins/python.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,39 +5,43 @@
 from countess.core.parameters import TextParam
 from countess.core.plugins import PandasTransformPlugin
 
 # XXX pretty sure this is a job for ast.parse rather than just
 # running compile() and exec() but that can wait.
 
 
+# These types will get copied to columns, anything else
+# (eg: classes, methods, functions) won't.
+
+SIMPLE_TYPES = set((bool, int, float, str, tuple, list))
+
+
 class PythonPlugin(PandasTransformPlugin):
     name = "Python Code"
     description = """
-        Apply python code.  Columns are mapped to local variables and back.
+        Apply python code to each row.
+        Columns are mapped to local variables and back.
         "__index" is set to the index value.
-        If you assign to a variable called "__filter", only rows where that
-        value is True will be kept.
+        If you assign to a variable called "__filter",
+        only rows where that value is true will be kept.
     """
 
     version = VERSION
 
     parameters = {"code": TextParam("Python Code")}
 
     def run_df(self, df, logger: Logger) -> pd.DataFrame:
         assert isinstance(self.parameters["code"], TextParam)
         code_object = compile(self.parameters["code"].value, "<PythonPlugin>", mode="exec")
 
         def _process(row):
             row_dict = dict(row)
             exec(code_object, {}, row_dict)  # pylint: disable=exec-used
-            return dict((k, v) for k, v in row_dict.items() if type(v) in (bool, int, float, str))
+            return dict((k, v) for k, v in row_dict.items() if type(v) in SIMPLE_TYPES)
 
         dfo = df.assign(__index=df.index)
         dfo = dfo.apply(_process, axis=1, result_type="expand")
 
-        if "__index" in dfo.columns:
-            dfo = dfo.drop(columns="__index")
-
         if "__filter" in dfo.columns:
             dfo = dfo.query("__filter").drop(columns="__filter")
 
         return dfo
```

### Comparing `countess-0.0.28/countess/plugins/regex.py` & `countess-0.0.29/countess/plugins/regex.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,127 @@
 import re
-from functools import partial
 
 import pandas as pd
 
 from countess import VERSION
 from countess.core.parameters import (
     ArrayParam,
     BooleanParam,
-    ColumnOrIndexChoiceParam,
+    ColumnChoiceParam,
     DataTypeChoiceParam,
+    IntegerParam,
     MultiParam,
     StringParam,
 )
 from countess.core.plugins import PandasInputPlugin, PandasTransformPlugin
 
 
+def _process_row(value: str, compiled_re, output_params, logger) -> pd.Series:
+    match = compiled_re.match(value)
+    if match:
+        return pd.Series(
+            dict(
+                (output_params[n]["name"].value, output_params[n].datatype.cast_value(g))
+                for n, g in enumerate(match.groups())
+            )
+        )
+    else:
+        logger.warning("Didn't Match", detail=repr(value))
+        return pd.Series({})
+
+
+def _process_row_multi(value: str, compiled_re, output_params, logger) -> pd.Series:
+    matches = compiled_re.findall(value)
+    if len(matches) == 0:
+        return pd.Series({})
+    if compiled_re.groups > 1:
+        return pd.Series(
+            dict(
+                (op["name"].value, [op.datatype.cast_value(match[num]) for match in matches])
+                for num, op in enumerate(output_params)
+            )
+        )
+    else:
+        op = output_params[0]
+        return pd.Series({op["name"].value: [op.datatype.cast_value(match) for match in matches]})
+
+
 class RegexToolPlugin(PandasTransformPlugin):
     name = "Regex Tool"
-    description = "Apply regular expressions to column(s) to make new column(s)"
+    description = "Apply regular expressions to a column to make new column(s)"
     link = "https://countess-project.github.io/CountESS/plugins/#regex-tool"
     version = VERSION
 
     parameters = {
-        "regexes": ArrayParam(
-            "Regexes",
+        "column": ColumnChoiceParam("Input Column"),
+        "regex": StringParam("Regular Expression", ".*"),
+        "output": ArrayParam(
+            "Output Columns",
             MultiParam(
-                "Regex",
+                "Col",
                 {
-                    "column": ColumnOrIndexChoiceParam("Input Column"),
-                    "regex": StringParam("Regular Expression", ".*"),
-                    "output": ArrayParam(
-                        "Output Columns",
-                        MultiParam(
-                            "Col",
-                            {
-                                "name": StringParam("Column Name"),
-                                "datatype": DataTypeChoiceParam(
-                                    "Column Type",
-                                    "string",
-                                ),
-                            },
-                        ),
+                    "name": StringParam("Column Name"),
+                    "datatype": DataTypeChoiceParam(
+                        "Column Type",
+                        "string",
                     ),
-                    "drop_column": BooleanParam("Drop Column", False),
-                    "drop_unmatch": BooleanParam("Drop Unmatched Rows", False),
                 },
             ),
         ),
+        "multi": BooleanParam("Multi Match", False),
+        "drop_column": BooleanParam("Drop Column", False),
+        "drop_unmatch": BooleanParam("Drop Unmatched Rows", False),
     }
 
-    def apply_func(self, column_name, compiled_re, output_params, logger, row):
-        value = str(row.get(column_name, ""))
-        match = compiled_re.match(value)
-        if match:
-            return [1] + [
-                output_params[n].datatype.cast_value(g) for n, g in enumerate(match.groups())
-            ]
-        else:
-            logger.warning("Didn't Match", detail=repr(value))
-            return [0] + [None] * compiled_re.groups
-
     def run_df(self, df, logger):
-        # prevent added columns from propagating backwards in
-        # the pipeline!
-        df = df.copy()
-
-        # the index doesn't seem to be available from within the applied function,
-        # which is annoying, so we copy it into a column here.
-        if any(rp["column"].is_index() for rp in self.parameters["regexes"]):
-            df["__index"] = df.index
-
-        # XXX this could be made more efficient by running
-        # multiple regexs in one 'apply' pass.
-
-        for regex_parameter in self.parameters["regexes"]:
-            compiled_re = re.compile(regex_parameter["regex"].value)
+        compiled_re = re.compile(self.parameters["regex"].value)
 
-            while compiled_re.groups > len(regex_parameter["output"].params):
-                regex_parameter["output"].add_row()
+        while compiled_re.groups > len(self.parameters["output"].params):
+            self.parameters["output"].add_row()
 
-            output_params = regex_parameter["output"].params
-            output_names = [pp["name"].value for pp in output_params]
+        output_params = self.parameters["output"].params
+        output_names = [pp["name"].value for pp in output_params]
 
-            if regex_parameter["column"].is_index():
-                column_name = "__index"
-            else:
-                column_name = regex_parameter["column"].value
+        column = self.parameters["column"].get_column(df)
 
-            # XXX not totally happy with this
-            func = partial(self.apply_func, column_name, compiled_re, output_params, logger)
+        if self.parameters["multi"].value:
+            func = _process_row_multi
+        else:
+            func = _process_row
 
-            re_groups_df = df.apply(func, axis=1, result_type="expand")
+        df = df.join(column.apply(func, args=(compiled_re, output_params, logger)))
 
-            for n in range(0, compiled_re.groups):
-                df[output_names[n]] = re_groups_df[n + 1]
+        if self.parameters["drop_unmatch"].value:
+            df = df.dropna(subset=output_names)
 
-            if regex_parameter["drop_unmatch"].value:
-                df["__filter"] = re_groups_df[0]
-                df = df.query("__filter != 0").drop(columns="__filter")
+        if self.parameters["multi"].value:
+            df = df.explode(output_names)
 
-        drop_columns = set(
-            rp["column"].value for rp in self.parameters["regexes"] if rp["drop_column"].value
-        )
-        if "__index" in df:
-            drop_columns.add("__index")
+        if self.parameters["drop_column"].value:
+            column_name = self.parameters["column"].value
+            if column_name not in df.columns:
+                df = df.reset_index()
+            df = df.drop(columns=column_name)
 
-        return df.drop(columns=drop_columns) if drop_columns else df
+        return df
 
 
 class RegexReaderPlugin(PandasInputPlugin):
     name = "Regex Reader"
     description = """Loads arbitrary data from line-delimited files, applying a regular expression
       to each line to extract fields.  If you're trying to read generic CSV or TSV files, use the CSV
       plugin instead as it handles escaping correctly."""
     link = "https://countess-project.github.io/CountESS/plugins/#regex-reader"
     version = VERSION
 
     file_types = [("CSV", "*.csv"), ("TXT", "*.txt")]
 
     parameters = {
-        "regex": StringParam("Regular Expression", ".*"),
-        "skip": BooleanParam("Skip First Row", False),
+        "regex": StringParam("Regular Expression", "(.*)"),
+        "skip": IntegerParam("Skip Lines", 0),
         "output": ArrayParam(
             "Output Columns",
             MultiParam(
                 "Col",
                 {
                     "name": StringParam("Column Name"),
                     "datatype": DataTypeChoiceParam(
@@ -152,15 +149,15 @@
             for n, p in enumerate(output_parameters)
             if p.index.value
         ] or None
 
         records = []
         with open(file_params["filename"].value, "r", encoding="utf-8") as fh:
             for num, line in enumerate(fh):
-                if num == 0 and self.parameters["skip"].value:
+                if num < self.parameters["skip"].value:
                     continue
                 match = compiled_re.match(line)
                 if match:
                     records.append(
                         (
                             output_parameters[n].datatype.cast_value(g)
                             for n, g in enumerate(match.groups())
@@ -176,8 +173,11 @@
                         pd.DataFrame.from_records(records, columns=columns, index=index_columns)
                     )
                     records = []
 
         if len(records) > 0:
             pdfs.append(pd.DataFrame.from_records(records, columns=columns, index=index_columns))
 
-        return pd.concat(pdfs)
+        if len(pdfs) > 0:
+            return pd.concat(pdfs)
+
+        return pd.DataFrame([], columns=columns)
```

### Comparing `countess-0.0.28/countess/plugins/sequence.py` & `countess-0.0.29/countess/plugins/sequence.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
-from countess.core.parameters import (
-    BooleanParam,
-    ColumnOrIndexChoiceParam,
-    IntegerParam,
-    StringParam,
-)
+from countess.core.parameters import BooleanParam, ColumnChoiceParam, IntegerParam, StringParam
 from countess.core.plugins import PandasTransformPlugin
 from countess.utils.variant import invert_dna_sequence
 
 
 class SequencePlugin(PandasTransformPlugin):
     """Manipulate DNA sequences"""
 
     name = "Sequence Tool"
     description = "Manipulate DNA Sequences"
     version = VERSION
     link = "https://countess-project.github.io/CountESS/plugins/#sequence"
 
     parameters = {
-        "column": ColumnOrIndexChoiceParam("Input Column"),
+        "column": ColumnChoiceParam("Input Column"),
         "invert": BooleanParam("Invert", False),
         "offset": IntegerParam("Offset", 0),
         "start": StringParam("Start at ...", ""),
         "stop": StringParam("Stop at ...", ""),
         "length": IntegerParam("Max Length", 150),
         "output": StringParam("Output Column", "sequence"),
     }
@@ -47,10 +42,16 @@
                 offset = seq.find(self.parameters["stop"].value)
                 if offset >= 0:
                     seq = seq[0 : offset + len(self.parameters["stop"].value)]
             if self.parameters["length"].value:
                 seq = seq[0 : self.parameters["length"].value]
             return seq
 
-        dfo = df.copy()
-        dfo[self.parameters["output"].value] = dfo[self.parameters["column"].value].apply(_process)
-        return dfo
+        column_name = self.parameters["column"].value
+        output_column_name = self.parameters["output"].value
+
+        if column_name in df.columns:
+            column = df[column_name]
+        else:
+            column = df.index.to_frame()[column_name]
+
+        return df.assign(**{output_column_name: column.apply(_process)})
```

### Comparing `countess-0.0.28/countess/plugins/variant.py` & `countess-0.0.29/countess/plugins/variant.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,19 @@
+from typing import Optional
+
 import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
-from countess.core.parameters import (
-    BooleanParam,
-    ColumnOrIndexChoiceParam,
-    IntegerParam,
-    StringParam,
-)
+from countess.core.parameters import BooleanParam, ColumnChoiceParam, IntegerParam, StringParam
 from countess.core.plugins import PandasTransformPlugin
 from countess.utils.variant import find_variant_string
 
 
-def process_row(var_seq: str, ref_seq: str, max_mutations: int, logger: Logger):
+def process_row(var_seq: str, ref_seq: str, max_mutations: int, logger: Logger) -> Optional[str]:
     try:
         return find_variant_string("g.", ref_seq, var_seq, max_mutations)
     except ValueError as exc:
         logger.warning(str(exc))
         return None
 
 
@@ -25,47 +22,39 @@
 
     name = "Variant Translator"
     description = "Turns a DNA sequence into a HGVS variant code"
     version = VERSION
     link = "https://countess-project.github.io/CountESS/plugins/#variant"
 
     parameters = {
-        "column": ColumnOrIndexChoiceParam("Input Column"),
+        "column": ColumnChoiceParam("Input Column", "sequence"),
         "sequence": StringParam("Reference Sequence"),
         "auto": BooleanParam("Automatic Reference Sequence?", False),
         "output": StringParam("Output Column", "variant"),
         "max_mutations": IntegerParam("Max Mutations", 10),
         "drop": BooleanParam("Drop unidentified variants", False),
     }
 
     def run_df(self, df: pd.DataFrame, logger: Logger) -> pd.DataFrame:
-        assert isinstance(self.parameters["column"], ColumnOrIndexChoiceParam)
+        assert isinstance(self.parameters["column"], ColumnChoiceParam)
         assert isinstance(self.parameters["sequence"], StringParam)
         assert isinstance(self.parameters["output"], StringParam)
         assert isinstance(self.parameters["max_mutations"], IntegerParam)
 
         dfo = df.copy()
 
+        column = self.parameters["column"].get_column(df)
         output = self.parameters["output"].value
 
-        if self.parameters["column"].is_index():
-            dfo["__index"] = df.index
-            column_name = "__index"
-        else:
-            column_name = self.parameters["column"].value
-
         if self.parameters["auto"].value:
-            value = pd.Series.mode(dfo[column_name])[0]
+            value = pd.Series.mode(column)[0]
             self.parameters["sequence"].value = value
 
         sequence = self.parameters["sequence"].value
         max_mutations = self.parameters["max_mutations"].value
 
-        dfo[output] = dfo[column_name].apply(process_row, args=(sequence, max_mutations, logger))
+        dfo[output] = column.apply(process_row, args=(sequence, max_mutations, logger))
 
         if self.parameters["drop"].value:
             dfo = dfo.query("variant.notnull()")
 
-        if self.parameters["column"].is_index():
-            return dfo.drop(columns=["__index"])
-        else:
-            return dfo
+        return dfo
```

### Comparing `countess-0.0.28/countess/utils/variant.py` & `countess-0.0.29/countess/utils/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/countess.egg-info/PKG-INFO` & `countess-0.0.29/countess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.28
+Version: 0.0.29
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -12,15 +12,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.28
+# CountESS 0.0.29
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.28/countess.egg-info/SOURCES.txt` & `countess-0.0.29/countess.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 countess/core/pipeline.py
 countess/core/plugins.py
 countess/gui/__init__.py
 countess/gui/config.py
 countess/gui/logger.py
 countess/gui/main.py
 countess/gui/tabular.py
+countess/gui/tree.py
 countess/plugins/__init__.py
 countess/plugins/csv.py
 countess/plugins/data_table.py
 countess/plugins/expression.py
 countess/plugins/fastq.py
 countess/plugins/group_by.py
 countess/plugins/hdf5.py
```

### Comparing `countess-0.0.28/countess.egg-info/entry_points.txt` & `countess-0.0.29/countess.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.28/pyproject.toml` & `countess-0.0.29/pyproject.toml`

 * *Files identical despite different names*

