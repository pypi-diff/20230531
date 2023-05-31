# Comparing `tmp/aws_parquet-0.1.0.tar.gz` & `tmp/aws_parquet-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_parquet-0.1.0.tar", max compression
+gzip compressed data, was "aws_parquet-0.2.0.tar", max compression
```

## Comparing `aws_parquet-0.1.0.tar` & `aws_parquet-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1155 2023-05-29 14:21:15.510299 aws_parquet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-27 12:44:13.337430 aws_parquet-0.1.0/src/aws_parquet/__init__.py
--rw-r--r--   0        0        0      315 2023-05-29 14:23:51.668665 aws_parquet-0.1.0/src/aws_parquet/_types.py
--rw-r--r--   0        0        0    14354 2023-05-29 14:26:28.370482 aws_parquet-0.1.0/src/aws_parquet/dataset.py
--rw-r--r--   0        0        0     2473 2023-05-29 14:23:51.710022 aws_parquet-0.1.0/src/aws_parquet/interface.py
--rw-r--r--   0        0        0        0 2023-05-27 12:44:13.338464 aws_parquet-0.1.0/src/aws_parquet/py.typed
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 aws_parquet-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1176 2023-05-31 17:58:47.653187 aws_parquet-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-05-31 17:25:56.938752 aws_parquet-0.2.0/src/aws_parquet/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-29 14:23:51.668665 aws_parquet-0.2.0/src/aws_parquet/_types.py
+-rw-r--r--   0        0        0    15941 2023-05-31 17:53:36.675601 aws_parquet-0.2.0/src/aws_parquet/dataset.py
+-rw-r--r--   0        0        0     2473 2023-05-29 14:23:51.710022 aws_parquet-0.2.0/src/aws_parquet/interface.py
+-rw-r--r--   0        0        0        0 2023-05-27 12:44:13.338464 aws_parquet-0.2.0/src/aws_parquet/py.typed
+-rw-r--r--   0        0        0      527 1970-01-01 00:00:00.000000 aws_parquet-0.2.0/PKG-INFO
```

### Comparing `aws_parquet-0.1.0/pyproject.toml` & `aws_parquet-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "aws_parquet"
-version = "0.1.0"
+version = "0.2.0"
 description = "An object-oriented interface for defining parquet datasets for AWS built on top of awswrangler and pandera"
 packages = [{ include = "aws_parquet", from = "src" }]
 authors = []
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 awswrangler = "^3.1.1"
 pandera = "^0.15.1"
+pydantic = "^1.10.8"
 
 [tool.poetry.dev-dependencies]
 # type hints
 mypy = "1.3.0"
 # formatting
 black = "23.3.0"
 # linting
```

### Comparing `aws_parquet-0.1.0/src/aws_parquet/dataset.py` & `aws_parquet-0.2.0/src/aws_parquet/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Optional,
     Union,
     cast,
     overload,
 )
 import pandas as pd
 import pandera as pa
-from abc import abstractmethod
+from pydantic import BaseModel
 from typeguard import typechecked
 
 from aws_parquet._types import PartitionLike, DataFrameOrIteratorT
 from aws_parquet.interface import ParquetDatasetInterface
 
 
 @typechecked
@@ -53,109 +53,125 @@
                 if not partitions_types:
                     partitions_types = p_types
                 if p_values:
                     partitions_types = p_types
                     partitions_values[path_wo_filename] = p_values
                 elif p_types != partitions_types:
                     raise ValueError(
-                        f"At least two different partitions schema detected: "
+                        f"At least two different partitions pandera_schema detected: "
                         f"{partitions_types} and {p_types}"
                     )
     if not partitions_types:
         return None, None
     return partitions_types, partitions_values
 
 
-@typechecked
-class ParquetDataset(ParquetDatasetInterface):
-    """Dataset for Parquet files in S3."""
+class FrozenBaseModel(BaseModel):
+    """Base model with frozen fields."""
 
-    @property
-    @abstractmethod
-    def partition_cols(self) -> List[str]:
-        """Return the partition columns."""
-        ...
+    class Config:
+        """Model config."""
 
-    @property
-    @abstractmethod
-    def database(self) -> str:
-        """Return the name of the database."""
-        ...
+        frozen = True
+        extras = "forbid"
 
-    @property
-    @abstractmethod
-    def table(self) -> str:
-        """Return the name of the dataset."""
-        ...
 
-    @property
-    @abstractmethod
-    def path(self) -> str:
-        """Return the path of the dataset."""
-        ...
+@typechecked
+class ParquetDataset(ParquetDatasetInterface, FrozenBaseModel):
+    """Dataset for Parquet files in S3."""
 
-    @property
-    @abstractmethod
-    def schema(self) -> pa.DataFrameSchema:
-        """Return the schema of the dataset."""
+    database: str
+    table: str
+    path: str
+    pandera_schema: pa.DataFrameSchema
+    partition_cols: List[str] = []
+    compression: Literal["snappy", "gzip", "zstd", None] = "snappy"
 
-    @property
-    def compression(self) -> Literal["snappy", "gzip", None]:
-        """Return the compression of the dataset."""
-        return "snappy"
+    # TODO - check that the pandera schema is compatible for parquet serde
 
     @property
     def categorical_columns(self) -> List[str]:
         """Return the categorical columns of the dataset."""
         return [
             col_name
-            for col_name, col_schema in self.schema.columns.items()
-            if str(col_schema.dtype) == "category"
+            for col_name, col_pandera_schema in self.pandera_schema.columns.items()
+            if str(col_pandera_schema.dtype) == "category"
+        ]
+
+    @property
+    def open_ended_categorical_columns(self) -> List[str]:
+        """Return the categorical columns of the dataset with no categories defined."""
+        return [
+            col_name
+            for col_name, col_pandera_schema in self.pandera_schema.columns.items()
+            if (
+                str(col_pandera_schema.dtype) == "category"
+                and (col_pandera_schema.dtype.type.categories is None)
+            )
         ]
 
     @property
     def columns(self) -> List[str]:
         """Return the columns of the dataset."""
-        return list(self.schema.columns.keys())
+        return list(self.pandera_schema.columns.keys())
 
-    def _build_coercible_schema_given_columns(
+    def _build_coercible_pandera_schema_given_columns(
         self, columns: Optional[List[str]] = None
     ) -> pa.DataFrameSchema:
-        """Build the schema given a list of columns."""
+        """Build the pandera_schema given a list of columns."""
         if columns is None:
-            schema = self.schema
-            schema.coerce = True
-            return schema
+            pandera_schema = self.pandera_schema
+            pandera_schema.coerce = True
+            return pandera_schema
 
-        schema = pa.DataFrameSchema(
+        pandera_schema = pa.DataFrameSchema(
             columns={
-                col_name: col_schema
-                for col_name, col_schema in self.schema.columns.items()
+                col_name: col_pandera_schema
+                for col_name, col_pandera_schema in self.pandera_schema.columns.items()
                 if col_name in columns
             }
         )
-        schema.coerce = True
-        return schema
+        pandera_schema.coerce = True
+        return pandera_schema
 
-    def _build_coercible_schema_given_partition(
+    def _build_coercible_pandera_schema_given_partition(
         self, partition: PartitionLike
     ) -> pa.DataFrameSchema:
-        """Build the schema of the partition."""
-        return self._build_coercible_schema_given_columns(
+        """Build the pandera_schema of the partition."""
+        return self._build_coercible_pandera_schema_given_columns(
             columns=list(partition.keys())
         )
 
     def _get_sample_df(self) -> pd.DataFrame:
-        """Return a sample dataframe with the dataset schema."""
+        """Return a sample dataframe with the dataset pandera_schema."""
         cols = []
-        for col, pa_col in self.schema.columns.items():
-            s = pd.Series([], dtype=pa_col.dtype.type, name=col)
+        for col, pa_col in self.pandera_schema.columns.items():
+            if str(pa_col.dtype.type) == "category":
+                s = self._get_sample_categorical_series(col, pa_col)
+
+            else:
+                s = pd.Series([], dtype=pa_col.dtype.type, name=col)
+
             cols.append(s)
+
         return pd.concat(cols, axis=1)
 
+    def _get_sample_categorical_series(self, col, pa_col):
+        if pa_col.dtype.type.categories is None:
+            # if no categories are provided then assume the values are strings
+            sample_string = "sample"
+            s = pd.Series(
+                [],
+                dtype=pd.CategoricalDtype(categories=[sample_string], ordered=False),
+                name=col,
+            )
+        else:
+            s = pd.Series([], dtype=pa_col.dtype.type, name=col)
+        return s
+
     def _get_athena_columns_types(self) -> Dict[str, str]:
         """Return the columns types for Athena."""
         df = self._get_sample_df()
         col_types, _ = wr._data_types.athena_types_from_pandas_partitioned(
             df=df,
             index=False,
             partition_cols=self.partition_cols,
@@ -184,14 +200,16 @@
 
     def create(
         self,
         if_exists: Literal["ignore", "warn", "raise"] = "ignore",
         sync: bool = True,
     ) -> None:
         """Create the dataset."""
+        wr.catalog.create_database(name=self.database, exist_ok=True)
+
         table_exists_in_catalog = wr.catalog.does_table_exist(
             database=self.database, table=self.table
         )
         if table_exists_in_catalog:
             if if_exists == "warn":
                 warnings.warn(
                     message=(
@@ -245,47 +263,60 @@
         """Build a partition filter function."""
 
         def compare_partition(partition: PartitionLike) -> bool:
             """Compare the partition."""
             partition_df = pd.DataFrame(
                 {k: [v] for k, v in partition.items() if k in partition_values.keys()}
             )
-            partition_schema = self._build_coercible_schema_given_partition(
-                partition_values
+            partition_pandera_schema = (
+                self._build_coercible_pandera_schema_given_partition(partition_values)
             )
-            partition_df_coerced = partition_schema(partition_df)
+            partition_df_coerced = partition_pandera_schema(partition_df)
 
             partition_values_df = pd.DataFrame(
                 {k: [v] for k, v in partition_values.items()}
             )
-            partition_values_coerced = partition_schema(partition_values_df)
+            partition_values_coerced = partition_pandera_schema(partition_values_df)
             return cast(bool, partition_df_coerced.equals(partition_values_coerced))
 
         return compare_partition
 
-    def _apply_schema(
-        self, df: pd.DataFrame, schema: pa.DataFrameSchema
+    def _apply_pandera_schema(
+        self, df: pd.DataFrame, pandera_schema: pa.DataFrameSchema
     ) -> pd.DataFrame:
-        out = schema(df)
+        out = pandera_schema(df)
+
+        for col in self.categorical_columns:
+            out[col] = out[col].cat.rename_categories(lambda x: str(x))
+
+        for col in self.open_ended_categorical_columns:
+            out[col] = out[col].cat.remove_unused_categories()
+
         return out[self.columns]
 
-    def _coerce_and_check_schema(
+    def _coerce_and_check_pandera_schema(
         self,
         df: DataFrameOrIteratorT,
         columns: Optional[List[str]],
     ) -> DataFrameOrIteratorT:
-        """Coerce the schema and check the schema."""
-        schema = self._build_coercible_schema_given_columns(columns)
+        """Coerce the pandera_schema and check the pandera_schema."""
+        pandera_schema = self._build_coercible_pandera_schema_given_columns(columns)
         if isinstance(df, pd.DataFrame):
-            return cast(DataFrameOrIteratorT, self._apply_schema(df=df, schema=schema))
+            return cast(
+                DataFrameOrIteratorT,
+                self._apply_pandera_schema(df=df, pandera_schema=pandera_schema),
+            )
 
         elif isinstance(df, Iterator):
             return cast(
                 DataFrameOrIteratorT,
-                (self._apply_schema(df=sub_df, schema=schema) for sub_df in df),
+                (
+                    self._apply_pandera_schema(df=sub_df, pandera_schema=pandera_schema)
+                    for sub_df in df
+                ),
             )
 
         else:
             raise TypeError("df must be a DataFrame or an Iterator of DataFrames.")
 
     @overload
     def read(
@@ -324,15 +355,15 @@
             dataset=True,
             chunked=chunked,
             partition_filter=partition_filter,
             columns=columns,
             use_threads=use_threads,
         )
 
-        return self._coerce_and_check_schema(out, columns=columns)
+        return self._coerce_and_check_pandera_schema(out, columns=columns)
 
     @overload
     def query(
         self,
         sql: str,
         *,
         workgroup: Optional[str] = None,
@@ -376,31 +407,33 @@
             use_threads=use_threads,
             workgroup=workgroup,
             **kwargs,
         )
 
     def update(self, data: pd.DataFrame, overwrite: bool = False) -> None:
         """Update the dataset."""
-        schema = self._build_coercible_schema_given_columns()
-        input_df = schema(data)
+        pandera_schema = self._build_coercible_pandera_schema_given_columns()
+        input_df = pandera_schema(data)
         wr.s3.to_parquet(
             df=input_df,
             path=self.path,
             dataset=True,
             mode="overwrite_partitions" if overwrite else "append",
             partition_cols=self.partition_cols,
             database=self.database,
             table=self.table,
         )
 
     def _get_partition_record(self, partition: PartitionLike) -> Dict[str, str]:
         """Get the partition record."""
         partition_df = pd.DataFrame({k: [v] for k, v in partition.items()})
-        partition_schema = self._build_coercible_schema_given_partition(partition)
-        partition_df_coerced = partition_schema(partition_df)
+        partition_pandera_schema = self._build_coercible_pandera_schema_given_partition(
+            partition
+        )
+        partition_df_coerced = partition_pandera_schema(partition_df)
         partition_record = partition_df_coerced.to_dict(orient="records")[0]
         return {k: str(v) for k, v in partition_record.items()}
 
     def _build_path(self, partition_record: PartitionLike) -> str:
         """Build the path pattern for a given partition."""
         path = self.path
         for col in self.partition_cols:
```

### Comparing `aws_parquet-0.1.0/src/aws_parquet/interface.py` & `aws_parquet-0.2.0/src/aws_parquet/interface.py`

 * *Files identical despite different names*

