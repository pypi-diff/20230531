# Comparing `tmp/countess-minimap2-0.0.5.tar.gz` & `tmp/countess-minimap2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-minimap2-0.0.5.tar", last modified: Mon May 15 02:52:20 2023, max compression
+gzip compressed data, was "countess-minimap2-0.0.6.tar", last modified: Wed May 31 04:07:35 2023, max compression
```

## Comparing `countess-minimap2-0.0.5.tar` & `countess-minimap2-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 02:52:20.119832 countess-minimap2-0.0.5/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2023-04-13 01:52:34.000000 countess-minimap2-0.0.5/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     2082 2023-05-15 02:52:20.119832 countess-minimap2-0.0.5/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1509 2023-05-15 02:51:43.000000 countess-minimap2-0.0.5/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 02:52:20.119832 countess-minimap2-0.0.5/countess_minimap2.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     2082 2023-05-15 02:52:20.000000 countess-minimap2-0.0.5/countess_minimap2.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      314 2023-05-15 02:52:20.000000 countess-minimap2-0.0.5/countess_minimap2.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-15 02:52:20.000000 countess-minimap2-0.0.5/countess_minimap2.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       63 2023-05-15 02:52:20.000000 countess-minimap2-0.0.5/countess_minimap2.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       68 2023-05-15 02:52:20.000000 countess-minimap2-0.0.5/countess_minimap2.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       18 2023-05-15 02:52:20.000000 countess-minimap2-0.0.5/countess_minimap2.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     4278 2023-05-15 02:51:34.000000 countess-minimap2-0.0.5/countess_minimap2.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1086 2023-05-15 00:56:31.000000 countess-minimap2-0.0.5/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-15 02:52:20.119832 countess-minimap2-0.0.5/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-15 00:46:44.000000 countess-minimap2-0.0.5/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:07:35.216711 countess-minimap2-0.0.6/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2023-04-13 01:52:34.000000 countess-minimap2-0.0.6/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2082 2023-05-31 04:07:35.216711 countess-minimap2-0.0.6/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1509 2023-05-31 04:06:44.000000 countess-minimap2-0.0.6/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:07:35.216711 countess-minimap2-0.0.6/countess_minimap2.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2082 2023-05-31 04:07:35.000000 countess-minimap2-0.0.6/countess_minimap2.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      314 2023-05-31 04:07:35.000000 countess-minimap2-0.0.6/countess_minimap2.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-31 04:07:35.000000 countess-minimap2-0.0.6/countess_minimap2.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       63 2023-05-31 04:07:35.000000 countess-minimap2-0.0.6/countess_minimap2.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       68 2023-05-31 04:07:35.000000 countess-minimap2-0.0.6/countess_minimap2.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       18 2023-05-31 04:07:35.000000 countess-minimap2-0.0.6/countess_minimap2.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4217 2023-05-31 04:06:17.000000 countess-minimap2-0.0.6/countess_minimap2.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1086 2023-05-31 04:01:45.000000 countess-minimap2-0.0.6/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-31 04:07:35.216711 countess-minimap2-0.0.6/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-15 00:46:44.000000 countess-minimap2-0.0.6/setup.py
```

### Comparing `countess-minimap2-0.0.5/LICENSE.txt` & `countess-minimap2-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-minimap2-0.0.5/PKG-INFO` & `countess-minimap2-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: countess-minimap2
-Version: 0.0.5
+Version: 0.0.6
 Summary: CountESS Minimap2 Plugin
 Author-email: Nick Moore <nick@zoic.org>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# CountESS MiniMap2 Plugin v0.0.5
+# CountESS MiniMap2 Plugin v0.0.6
 
 This is a plugin to allow [MiniMap2](https://github.com/lh3/minimap2) 
 to be used from within [CountESS](https://github.com/CountESS-Project/CountESS/)
 
 This might be useful, but it also stands as a handy example of how to write
 a CountESS plugin which wraps an external Python library.
```

### Comparing `countess-minimap2-0.0.5/README.md` & `countess-minimap2-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS MiniMap2 Plugin v0.0.5
+# CountESS MiniMap2 Plugin v0.0.6
 
 This is a plugin to allow [MiniMap2](https://github.com/lh3/minimap2) 
 to be used from within [CountESS](https://github.com/CountESS-Project/CountESS/)
 
 This might be useful, but it also stands as a handy example of how to write
 a CountESS plugin which wraps an external Python library.
```

### Comparing `countess-minimap2-0.0.5/countess_minimap2.egg-info/PKG-INFO` & `countess-minimap2-0.0.6/countess_minimap2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: countess-minimap2
-Version: 0.0.5
+Version: 0.0.6
 Summary: CountESS Minimap2 Plugin
 Author-email: Nick Moore <nick@zoic.org>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# CountESS MiniMap2 Plugin v0.0.5
+# CountESS MiniMap2 Plugin v0.0.6
 
 This is a plugin to allow [MiniMap2](https://github.com/lh3/minimap2) 
 to be used from within [CountESS](https://github.com/CountESS-Project/CountESS/)
 
 This might be useful, but it also stands as a handy example of how to write
 a CountESS plugin which wraps an external Python library.
```

### Comparing `countess-minimap2-0.0.5/countess_minimap2.py` & `countess-minimap2-0.0.6/countess_minimap2.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 import mappy  # type: ignore
 
 from countess.core.logger import Logger
 from countess.core.parameters import (
     BooleanParam,
     ChoiceParam,
-    ColumnOrIndexChoiceParam,
+    ColumnChoiceParam,
     IntegerParam,
     StringParam,
     FileParam,
 )
 from countess.core.plugins import PandasTransformPlugin
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 CS_STRING_RE = r"(=[ACTGTN]+|:[0-9]+|(?:\*[ACGTN][ACGTN])+|\+[ACGTN]+|-[ACGTN]+)"
 MM2_PRESET_CHOICES = ["sr", "map-pb", "map-ont", "asm5", "asm10", "splice"]
 
 
 def cs_to_hgvs(cs_string: str, offset: int=1) -> str:
     """Turn the Minimap2 "difference string" into a HGVS string"""
@@ -65,67 +65,64 @@
     """
     version = VERSION
     link = "https://github.com/nickzoic/countess-minimap2#readme"
 
     FILE_TYPES = [("MMI", "*.mmi"), ("FASTA", "*.fa(sta)?")]
 
     parameters = {
-        "column": ColumnOrIndexChoiceParam("Input Column", "sequence"),
+        "column": ColumnChoiceParam("Input Column", "sequence"),
         "prefix": StringParam("Output Column Prefix", "mm"),
         "ref": FileParam("Ref FA / Ref MMI", file_types = FILE_TYPES),
         "preset": ChoiceParam("Preset", "sr", choices=MM2_PRESET_CHOICES),
         "min_length": IntegerParam("Minimum Match Length", 0),
         "drop": BooleanParam("Drop Unmatched", False),
     }
 
     def run_df(self, df: pd.DataFrame, logger: Logger) -> pd.DataFrame:
 
-        assert isinstance(self.parameters['column'], ColumnOrIndexChoiceParam)
+        assert isinstance(self.parameters['column'], ColumnChoiceParam)
 
+        column = self.parameters['column'].get_column(df)
         prefix = self.parameters["prefix"].value
 
         aligner = mappy.Aligner(
             self.parameters["ref"].value, preset=self.parameters["preset"].value
         )
 
         if not aligner:
             logger.error("ERROR: failed to load/build index file")
             return pd.DataFrame()
 
-        df = df.copy()
-
-        if self.parameters["column"].is_index():
-            df["__index"] = df.index
-            column_name = "__index"
-        else:
-            column_name = self.parameters["column"].value
-
         prefix = self.parameters["prefix"].value
         min_length = self.parameters["min_length"].value
 
-        def process(row: Mapping[str, Any]) -> tuple[Optional[str], int, int, int, Optional[str], Optional[str], Optional[str]]:
+        def process(value: str) -> pd.Series:
             # XXX only returns first match
-            x = aligner.map(row[column_name], cs=True)
+            x = aligner.map(value, cs=True)
             for z in x:
                 if z.r_en - z.r_st >= min_length:
-                    return (z.ctg, z.r_st, z.r_en, z.strand, z.cigar_str, z.cs, \
-                            cs_to_hgvs(z.cs, z.r_st+1))
-            return (None, 0, 0, 0, None, None, None)
-
-        column_names = [
-            prefix + "_ctg",
-            prefix + "_r_st",
-            prefix + "_r_en",
-            prefix + "_r_strand",
-            prefix + "_cigar",
-            prefix + "_cs",
-            prefix + "_hgvs",
-        ]
-        df[column_names] = df.apply(process, axis=1, result_type="expand")
+                    return pd.Series({
+                        prefix + "_ctg": z.ctg,
+                        prefix + "_r_st": z.r_st,
+                        prefix + "_r_en": z.r_en,
+                        prefix + "_strand": z.strand,
+                        prefix + "_cigar": z.cigar_str,
+                        prefix + "_cs": z.cs,
+                        prefix + "_hgvs": cs_to_hgvs(z.cs, z.r_st+1),
+                    })
+            return pd.Series({
+                prefix + "_ctg": None,
+                prefix + "_r_st": 0,
+                prefix + "_r_en": 0,
+                prefix + "_strand": 0,
+                prefix + "_cigar": "",
+                prefix + "_cs": "",
+                prefix + "_hgvs": "",
+            })
+
 
-        if self.parameters["column"].is_index():
-            df.drop(columns=["__index"])
+        df = df.join(column.apply(process, convert_dtype=True))
 
         if self.parameters["drop"].value:
-            df = df.query("mm_ctg.notnull()")
+            df = df.dropna(subset=[prefix + "_ctg"])
 
         return df
```

### Comparing `countess-minimap2-0.0.5/pyproject.toml` & `countess-minimap2-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 dependencies = [
     "countess>=0.0.26,<0.1",
     "mappy~=2.24",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "countess[dev]>=0.0.26,<0.1",
+    "countess[dev]>=0.0.29,<0.1",
 ]
 
 [project.entry-points.countess_plugins]
 minimap2 = "countess_minimap2:MiniMap2Plugin"
 
 [tool.setuptools.dynamic]
 version = { attr = "countess_minimap2.VERSION" }
```

