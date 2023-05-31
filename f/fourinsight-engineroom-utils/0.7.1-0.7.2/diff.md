# Comparing `tmp/fourinsight_engineroom_utils-0.7.1-py3-none-any.whl.zip` & `tmp/fourinsight_engineroom_utils-0.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13988 bytes, number of entries: 10
--rw-r--r--  2.0 unx      777 b- defN 23-Feb-14 09:22 fourinsight/engineroom/utils/__init__.py
--rw-r--r--  2.0 unx    16145 b- defN 23-Feb-14 09:22 fourinsight/engineroom/utils/_core.py
--rw-r--r--  2.0 unx    26506 b- defN 23-Feb-14 09:22 fourinsight/engineroom/utils/_datamanage.py
--rw-r--r--  2.0 unx       62 b- defN 23-Feb-14 09:22 fourinsight/engineroom/utils/iter_index/__init__.py
--rw-r--r--  2.0 unx     1183 b- defN 23-Feb-14 09:22 fourinsight/engineroom/utils/iter_index/_iter_index.py
--rw-r--r--  2.0 unx     1064 b- defN 23-Feb-14 09:23 fourinsight_engineroom_utils-0.7.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      763 b- defN 23-Feb-14 09:23 fourinsight_engineroom_utils-0.7.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-14 09:23 fourinsight_engineroom_utils-0.7.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Feb-14 09:23 fourinsight_engineroom_utils-0.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      999 b- defN 23-Feb-14 09:23 fourinsight_engineroom_utils-0.7.1.dist-info/RECORD
-10 files, 47603 bytes uncompressed, 12228 bytes compressed:  74.3%
+Zip file size: 14260 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      777 b- defN 23-May-31 09:09 fourinsight/engineroom/utils/__init__.py
+-rw-r--r--  2.0 unx    17091 b- defN 23-May-31 09:08 fourinsight/engineroom/utils/_core.py
+-rw-r--r--  2.0 unx    26506 b- defN 23-May-31 09:08 fourinsight/engineroom/utils/_datamanage.py
+-rw-r--r--  2.0 unx       62 b- defN 23-May-31 09:08 fourinsight/engineroom/utils/iter_index/__init__.py
+-rw-r--r--  2.0 unx     1239 b- defN 23-May-31 09:08 fourinsight/engineroom/utils/iter_index/_iter_index.py
+-rw-r--r--  2.0 unx     1064 b- defN 23-May-31 09:09 fourinsight_engineroom_utils-0.7.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      763 b- defN 23-May-31 09:09 fourinsight_engineroom_utils-0.7.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 09:09 fourinsight_engineroom_utils-0.7.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-31 09:09 fourinsight_engineroom_utils-0.7.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      999 b- defN 23-May-31 09:09 fourinsight_engineroom_utils-0.7.2.dist-info/RECORD
+10 files, 48605 bytes uncompressed, 12500 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: fourinsight/engineroom/utils/iter_index/__init__.py
 Comment: 
 
 Filename: fourinsight/engineroom/utils/iter_index/_iter_index.py
 Comment: 
 
-Filename: fourinsight_engineroom_utils-0.7.1.dist-info/LICENSE
+Filename: fourinsight_engineroom_utils-0.7.2.dist-info/LICENSE
 Comment: 
 
-Filename: fourinsight_engineroom_utils-0.7.1.dist-info/METADATA
+Filename: fourinsight_engineroom_utils-0.7.2.dist-info/METADATA
 Comment: 
 
-Filename: fourinsight_engineroom_utils-0.7.1.dist-info/WHEEL
+Filename: fourinsight_engineroom_utils-0.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: fourinsight_engineroom_utils-0.7.1.dist-info/top_level.txt
+Filename: fourinsight_engineroom_utils-0.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: fourinsight_engineroom_utils-0.7.1.dist-info/RECORD
+Filename: fourinsight_engineroom_utils-0.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fourinsight/engineroom/utils/__init__.py

```diff
@@ -14,15 +14,15 @@
     CompositeDataSource,
     DatetimeIndexConverter,
     DrioDataSource,
     FloatIndexConverter,
     IntegerIndexConverter,
 )
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 
 __all__ = [
     "AzureBlobHandler",
     "BaseDataSource",
     "BaseHandler",
     "BaseIndexConverter",
     "CompositeDataSource",
```

## fourinsight/engineroom/utils/_core.py

```diff
@@ -393,15 +393,18 @@
         """
         if not set(self._headers.keys()).issuperset(results):
             raise KeyError("Keyword must be in headers.")
 
         current_index = self._dataframe.index[-1]
 
         try:
-            row_update = pd.DataFrame(data=results, index=[current_index],).astype(
+            row_update = pd.DataFrame(
+                data=results,
+                index=[current_index],
+            ).astype(
                 {
                     header: dtype_
                     for header, dtype_ in self._headers.items()
                     if header in results
                 }
             )
         except ValueError:
@@ -429,58 +432,74 @@
 
         for row_i, result_i in dataframe.to_dict(orient="index").items():
             if self._indexing_mode == "auto":
                 row_i = None
             self.new_row(row_i)
             self.collect(**result_i)
 
-    def pull(self, raise_on_missing=True):
+    def pull(self, raise_on_missing=True, strict=True):
         """
         Pull results from source. Remote source overwrites existing values.
 
         Parameters
         ----------
         raise_on_missing : bool
             Raise exception if results can not be pulled from source.
+        strict : bool
+            Whether to be strict with respect to headers in the source or not. Setting
+            `strict=True` (default) will require that the source has the exact same
+            headers as the `ResultCollector`. Setting `strict=False` will allow pulling
+            of partial results (i.e., headers that does not have results in source,
+            will be populated with `None` values).
         """
 
         self._handler.pull(raise_on_missing=raise_on_missing)
         if not self._handler.getvalue():
             return
 
         self._handler.seek(0)
-        df = pd.read_csv(
+        df_source = pd.read_csv(
             self._handler, index_col=0, parse_dates=True, dtype=self._headers
         )
 
-        if not (set(df.columns) == set(self._headers.keys())):
+        if strict and set(df_source.columns) != set(self._headers.keys()):
             raise ValueError("Header is not valid.")
 
         if (
-            not df.index.empty
+            not df_source.index.empty
             and (self._indexing_mode == "auto")
-            and not (df.index.dtype == "int64")
+            and not (df_source.index.dtype == "int64")
         ):
             raise ValueError("Index dtype must be 'int64'.")
         elif (
-            not df.index.empty
+            not df_source.index.empty
             and (self._indexing_mode == "timestamp")
-            and not (isinstance(df.index, pd.DatetimeIndex))
+            and not (isinstance(df_source.index, pd.DatetimeIndex))
         ):
             raise ValueError("Index must be 'DatetimeIndex'.")
 
-        self._dataframe = df
+        columns_missing = self.dataframe.columns.difference(df_source.columns)
+        df_source[columns_missing] = None
+
+        self._dataframe = df_source[self._headers.keys()].astype(self._headers)
 
     def push(self):
         """
         Push results to source.
         """
         self._handler.seek(0)
         self._handler.truncate()
-        self._dataframe.to_csv(self._handler, sep=",", index=True, line_terminator="\n")
+        try:
+            self._dataframe.to_csv(
+                self._handler, sep=",", index=True, lineterminator="\n"
+            )
+        except TypeError:  # for backward compatibility (remove after 2024-06-01)
+            self._dataframe.to_csv(
+                self._handler, sep=",", index=True, line_terminator="\n"
+            )
         self._handler.push()
 
     @property
     def dataframe(self):
         """Return a (deep) copy of the internal dataframe"""
         return self._dataframe.copy(deep=True)
```

## fourinsight/engineroom/utils/iter_index/_iter_index.py

```diff
@@ -2,15 +2,15 @@
 
 
 def date_range(
     start=None,
     end=None,
     periods=None,
     freq=None,
-    inclusive=None,
+    inclusive="both",
     **kwargs,
 ):
     """
     Return lists of start/end pairs. Wrapper around ``pandas.date_range``.
 
     Parameters
     ----------
@@ -33,11 +33,14 @@
         Sequence of start values as `pandas.Timestamp`.
     end : list
         Sequence of end values as `pandas.Timestamp`.
     """
     if periods:
         periods += 1
 
+    if inclusive is None:
+        inclusive = "both"
+
     start_end = pd.date_range(
         start=start, end=end, periods=periods, freq=freq, inclusive=inclusive, **kwargs
     )
     return list(start_end[:-1]), list(start_end[1:])
```

## Comparing `fourinsight_engineroom_utils-0.7.1.dist-info/LICENSE` & `fourinsight_engineroom_utils-0.7.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fourinsight_engineroom_utils-0.7.1.dist-info/METADATA` & `fourinsight_engineroom_utils-0.7.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fourinsight-engineroom-utils
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python boilerplate and utilites for 4Insight EngineRoom app development.
 Home-page: https://4insight.io/
 Author: 4Subsea
 Author-email: support@4subsea.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `fourinsight_engineroom_utils-0.7.1.dist-info/RECORD` & `fourinsight_engineroom_utils-0.7.2.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-fourinsight/engineroom/utils/__init__.py,sha256=_n0E1h3XJRVlayR66LOTtLM4IZrUSOZI7ILulriZ0sU,777
-fourinsight/engineroom/utils/_core.py,sha256=txVwED4kQHRStHzYoQ6fWbhVz72CDnIMlnz5a6gGkRE,16145
+fourinsight/engineroom/utils/__init__.py,sha256=6Gu7obWxJVmnyYx8lgOOcTIVq0El4voIhu_gNKWXATY,777
+fourinsight/engineroom/utils/_core.py,sha256=ZdmWPmbygkYyMEFmvqC4-uSn7w1bO3UjtCBcB0RA4cs,17091
 fourinsight/engineroom/utils/_datamanage.py,sha256=NmZGRpYbPYy7kQd1drkAgPlmyoN8tC6imz_7wHmyYdc,26506
 fourinsight/engineroom/utils/iter_index/__init__.py,sha256=FYA92_ljg6GJnWMo-szKMLfF7vaMF46NAoFIc4OeTms,62
-fourinsight/engineroom/utils/iter_index/_iter_index.py,sha256=OtfIQRJ307weBzGq60QpULzpTdWxKTrOVSeSaU6zFfY,1183
-fourinsight_engineroom_utils-0.7.1.dist-info/LICENSE,sha256=0fAIvOa0aSEFA9-tPJGRuqMa6SMxWBfDah5S9szI8TM,1064
-fourinsight_engineroom_utils-0.7.1.dist-info/METADATA,sha256=fuX1Y4Kq0_8wDm7gYsujtbQuw4BFIT9yxz9os6AD5AQ,763
-fourinsight_engineroom_utils-0.7.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-fourinsight_engineroom_utils-0.7.1.dist-info/top_level.txt,sha256=oxGWrcBg2Biv0bKrBHd9Clg_bel4Tqr0lNxMFgxOMrk,12
-fourinsight_engineroom_utils-0.7.1.dist-info/RECORD,,
+fourinsight/engineroom/utils/iter_index/_iter_index.py,sha256=rNxtO1dmCYCG4q9DUU9sD9Fohid7FMX8G5b_KX1-MOU,1239
+fourinsight_engineroom_utils-0.7.2.dist-info/LICENSE,sha256=0fAIvOa0aSEFA9-tPJGRuqMa6SMxWBfDah5S9szI8TM,1064
+fourinsight_engineroom_utils-0.7.2.dist-info/METADATA,sha256=BhKDBQBXSiq5ulo2wqw2GXjxwXOxxvt0O1hhgE3X_-o,763
+fourinsight_engineroom_utils-0.7.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fourinsight_engineroom_utils-0.7.2.dist-info/top_level.txt,sha256=oxGWrcBg2Biv0bKrBHd9Clg_bel4Tqr0lNxMFgxOMrk,12
+fourinsight_engineroom_utils-0.7.2.dist-info/RECORD,,
```

