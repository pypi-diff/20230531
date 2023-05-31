# Comparing `tmp/bmsdna_lakeapi-0.4.7.tar.gz` & `tmp/bmsdna_lakeapi-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.4.7.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.5.1.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.4.7.tar` & `bmsdna_lakeapi-0.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1081 2023-05-25 15:16:53.787064 bmsdna_lakeapi-0.4.7/LICENSE
--rw-r--r--   0        0        0     8431 2023-05-25 15:16:53.787064 bmsdna_lakeapi-0.4.7/README.md
--rw-r--r--   0        0        0      271 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1074 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      926 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     5989 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     4072 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_datafusion.py
--rw-r--r--   0        0        0     8573 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6390 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11432 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    11558 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    19758 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6836 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     7822 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4497 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3151 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2367 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      326 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1842 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     9725 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-31 08:32:18.764371 bmsdna_lakeapi-0.5.1/LICENSE
+-rw-r--r--   0        0        0     8929 2023-05-31 08:32:18.764371 bmsdna_lakeapi-0.5.1/README.md
+-rw-r--r--   0        0        0      337 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      670 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     6355 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     9131 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6039 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11357 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    11904 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    18925 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6754 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1177 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6512 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4253 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3109 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2478 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-05-31 08:32:18.780371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1998 2023-05-31 08:32:18.780371 bmsdna_lakeapi-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.5.1/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.4.7/LICENSE` & `bmsdna_lakeapi-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.7/README.md` & `bmsdna_lakeapi-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,26 +36,28 @@
 [![PyPI version](https://badge.fury.io/py/bmsdna-lakeapi.svg)](https://pypi.org/project/bmsdna-lakeapi/)
 
 Pypi Package `bmsdna-lakeapi` can be installed like any python package : `pip install bmsdna-lakeapi`
 
 ## Basic Idea
 
 Based on a `YAML` configuration and the data source, LakeAPI will automatically generate GET and/or POST endpoints.
-Calling the endpoint turns the query into an SQL statement that can be executed with the engine of your choice (duckdb, datafusion or polars).
+Calling the endpoint turns the query into an SQL statement that can be executed with the engine of your choice (duckdb or polars).
 The result is then seralised into the requested format (Json, CSV, Arrow etc).
 
+This makes it super easy to distribute your data lake data to other systems. We use it internally to feed data to MS SQL Server, SQLite, Streamlit and Web Apps. You can host it wherever you want, we use Azure Websites which works fine even for very large data amounts.
+
 ## OpenAPI
 
 Of course everything works with `OpenAPI` and `FastAPI`. This means you can add other FastAPI routes, you can use the /docs and /redoc endpoints.
 
 So everything will be fully documented automatically, which is really cool. 🔥🔥
 
 ## Engine
 
-`DuckDB` is the default query engine. `Polars` and `Datafusion` are also supported, but lack some features. The query engine can be specified at the route level and at the query level with the hidden parameter $engine="duckdb|datafusion|polars". If you want polars or datafusion, add the required extra.
+`DuckDB` is the default query engine. `Polars` is also supported, but lack some features. The query engine can be specified at the route level and at the query level with the hidden parameter $engine="duckdb|polars". If you want polars, add the required extra.
 
 At the moment, DuckDB seems to have an advantage and performs the best. Also features like full text search are only available with `DuckDB`.
 
 ## Default Security
 
 By Default, Basic Authentication is enabled. To add a user, simply run `add_lakeapi_user YOURUSERNAME --yaml-file config.yml`. This will add the user to your config yaml (argon2 encrypted).
 The generated Password is printed. If you do not want this logic, you can overwrite the username_retriver of the Default Config
@@ -218,11 +220,16 @@
 - Metadata endpoints to retrieve data types, string lengths and more
 - Easily expose entire folders by using a "\*" wildcard in both the name and the datasource.uri config, see example in the config above
 - Good test coverage
 
 ## Work in progress
 
 Please note that this is a work in progress, changes will be made and things may break. Especially at this early stage.
+We recommend only using the export from `bmsdna.lakeapi` for now and not to use the submodules.
+
+## Limitations
+
+- You can currently only serve local files. We might add support for `fsspec` later on. You can still mount your data if you use Linux, which is what we do in production
 
 ## Contribution
 
 Feel free to contribute, report bugs or request enhancements.
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/api/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 import os
 
 
 @dataclass(frozen=True)
 class LakeApiStartInfo:
     start_config: BasicConfig
     config: Configs
-    get_username: Callable[[Request], Awaitable]
 
 
 def init_lakeapi(
-    app: FastAPI, start_config: BasicConfig | None = None, config: Configs | str | None = None
+    app: FastAPI, use_basic_auth: bool, start_config: BasicConfig | None = None, config: Configs | str | None = None
 ) -> LakeApiStartInfo:
     start_config = start_config or get_default_config()
     real_config: Configs
     if config is None:
         real_config = Configs.from_yamls(start_config, os.getenv("CONFIG_PATH", "config.yml"))
     elif isinstance(config, str):
         real_config = Configs.from_yamls(start_config, config)
     else:
         real_config = config
-    router, get_username = init_routes(real_config, start_config)
+    router = init_routes(real_config, start_config)
+    if use_basic_auth:
+        from bmsdna.lakeapi.core.uservalidation import add_user_middlware
+
+        add_user_middlware(app, start_config, real_config.users)
     app.include_router(router)
-    return LakeApiStartInfo(start_config, real_config, get_username)
+    return LakeApiStartInfo(start_config, real_config)
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 from bmsdna.lakeapi.core.types import Engines
 from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 from bmsdna.lakeapi.context.df_polars import PolarsExecutionContext
-from bmsdna.lakeapi.context.df_datafusion import DatafusionDbExecutionContext
 
 
 def get_context_by_engine(engine: Engines):
     match engine.lower():
         case "duckdb":
             from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 
             ExecutionContext = DuckDbExecutionContext
         case "polars":
             from bmsdna.lakeapi.context.df_polars import PolarsExecutionContext
 
             ExecutionContext = PolarsExecutionContext
-        case "datafusion":
-            from bmsdna.lakeapi.context.df_datafusion import DatafusionDbExecutionContext
-
-            ExecutionContext = DatafusionDbExecutionContext
         case _:
             raise Exception(f"Unknown engine {engine}")
     return ExecutionContext
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/df_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -106,17 +106,28 @@
         self.modified_dates: dict[str, datetime] = {}
 
     def get_pyarrow_dataset(
         self,
         uri: str,
         file_type: FileTypes,
         partitions: Optional[List[Tuple[str, str, Any]]],
-    ) -> Optional[pa.dataset.Dataset]:
+    ) -> Optional[pa.dataset.Dataset | pa.Table]:
         if file_type in ["parquet", "ipc", "arrow", "feather", "csv", "orc"]:
             ds = pa.dataset.dataset(uri, format=file_type)
+        elif file_type in ["ndjson", "json"]:
+            import pandas
+
+            pd = pandas.read_json(uri, orient="records", lines=file_type == "ndjson")
+
+            return pyarrow.Table.from_pandas(pd)
+        elif file_type == "avro":
+            import polars as pl
+
+            pd = pl.read_avro(uri).to_arrow()
+            return pd
         elif file_type == "delta":
             dt = DeltaTable(
                 uri,
             )
 
             ds = dt.to_pyarrow_dataset(partitions=partitions)
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -197,14 +197,25 @@
             search_con.execute(f"PRAGMA create_fts_index('{persistence_name}', '{pk_name}', {scc})")
             search_con.close()
             if os.path.exists(persistance_file_name):
                 os.remove(persistance_file_name)
             os.rename(persistance_file_name_temp, persistance_file_name)
         self.persistance_file_name = persistance_file_name
 
+    def register_dataframe(
+        self, name: str, uri: str, file_type: FileTypes, partitions: List[Tuple[str, str, Any]] | None
+    ):
+        if file_type == "json":
+            self.con.execute(f"CREATE VIEW {name} as SELECT *FROM read_json_auto('{uri}', format='array')")
+            return
+        if file_type == "ndjson":
+            self.con.execute(f"CREATE VIEW {name} as SELECT *FROM read_json_auto('{uri}', format='newline_delimited')")
+            return
+        return super().register_dataframe(name, uri, file_type, partitions)
+
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         if self.res_con:
             self.res_con.__exit__(*args)
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/df_polars.py`

 * *Files 8% similar despite different names*

```diff
@@ -142,16 +142,14 @@
             case "delta":
                 from bmsdna.lakeapi.polars_extensions.delta import scan_delta2
 
                 df = pl.scan_delta2(  # type: ignore
                     uri,
                     pyarrow_options={"partitions": partitions},
                 )
-            case "parquet_withdecimal":  # differentiation no longer needed
-                df = pl.scan_parquet(uri)
             case "parquet":
                 df = pl.scan_parquet(uri)
             case "arrow":
                 df = pl.scan_ipc(uri)
             case "avro":
                 df = cast(pl.LazyFrame, pl.read_avro(uri))
             case "csv":
@@ -179,17 +177,7 @@
         return PolarsResultData(df, self.sql_context)
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         pass
-
-
-local = threading.local()
-local.exec_context = None
-
-
-def get_polars_context() -> ExecutionContext:
-    if local.exec_context is None:
-        local.exec_context = PolarsExecutionContext()
-    return local.exec_context
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,39 +22,36 @@
 from fastapi import APIRouter, Request
 
 import yaml
 from polars.type_aliases import JoinStrategy
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 
 from bmsdna.lakeapi.core.log import get_logger
+from bmsdna.lakeapi.core.partition_utils import _with_implicit_parameters
 from bmsdna.lakeapi.core.types import FileTypes, OperatorType, Param, PolaryTypeFunction, Engines, SearchConfig
 
 logger = get_logger(__name__)
 
 
 @dataclass(frozen=True)
 class BasicConfig:
-    username_retriever: Callable[[Request, "BasicConfig", "Sequence[UserConfig]"], str | Awaitable[str]]
     enable_sql_endpoint: bool
     temp_folder_path: str
     data_path: str
-    token_jwt_secret: str | None  # None disables the token feature
     min_search_length: int
+    default_engine: Engines
 
 
 def get_default_config():
-    from bmsdna.lakeapi.core.uservalidation import get_username
-
     return BasicConfig(
-        username_retriever=get_username,
         enable_sql_endpoint=os.getenv("ENABLE_SQL_ENDPOINT", "0") == "1",
         temp_folder_path=os.getenv("TEMP", "/tmp"),
         data_path=os.environ.get("DATA_PATH", "data"),
-        token_jwt_secret=os.getenv("JWT_SECRET", None),
         min_search_length=3,
+        default_engine="duckdb",
     )
 
 
 @dataclass
 class Filter:
     key: str
     operator: Literal[
@@ -137,20 +134,20 @@
 class Config:
     name: str
     tag: str
     datasource: DatasourceConfig
     version: Optional[int] = 1
     api_method: Union[Literal["get", "post"], List[Literal["get", "post"]]] = "get"
     params: Optional[List[Union[Param, str]]] = None
-    engine: Engines = "duckdb"
     timestamp: Optional[datetime] = None
     cache_expiration_time_seconds: Optional[int] = CACHE_EXPIRATION_TIME_SECONDS
     options: Optional[Union[Option, None]] = None
     allow_get_all_pages: Optional[bool] = False
     search: Optional[List[SearchConfig]] = None
+    engine: Optional[Engines] = None
 
     def __post_init__(self):
         self.version_str = (
             str(self.version) if str(self.version or 1).startswith("v") else "v" + str(self.version or 1)
         )
         self.route = "/api/" + self.version_str + "/" + self.tag + "/" + self.name
 
@@ -165,15 +162,14 @@
     @classmethod
     def from_dict(
         cls, config: Dict, basic_config: BasicConfig, table_names: List[tuple[int, str, str]]
     ) -> List["Config"]:
         name = config["name"]
         tag = config["tag"]
         version = config.get("version", 1)
-        engine = config.get("engine", "duckdb")
         api_method = cast(Literal["post", "get"], config.get("api_method", "get"))
         params = config.get("params")
         datasource = config["datasource"]
         uri = datasource["uri"]
         assert isinstance(uri, str)
         file_type = cast(FileTypes, datasource.get("file_type", "delta") if datasource else "delta")
         columns = datasource.get("columns") if datasource else None
@@ -199,17 +195,14 @@
             sortby = [SortBy(by=s.get("by"), direction=s.get("direction")) for s in sortby]
 
         select = columns if columns else select
 
         if select:
             select = [Column(name=c.get("name"), alias=c.get("alias")) for c in select]
 
-        if not engine:
-            engine = "duckdb"
-
         if name == "*":
             assert uri.endswith("/*")
             folder = uri.rstrip("/*")
             root_folder = os.path.join(basic_config.data_path, folder)
             if not os.path.exists(root_folder):
                 logger.warning("Path not existing: " + root_folder)
                 return []
@@ -225,24 +218,24 @@
                             file_type=file_type,
                             select=select,
                             exclude=exclude,
                             sortby=sortby,
                             filters=None,
                             cache_expiration_time_seconds=cache_expiration_time_seconds,
                         )
-
+                        new_params = _with_implicit_parameters(_params, file_type, basic_config, datasource.uri)
                         ls.append(
                             cls(
                                 name=it.name,
                                 tag=tag,
-                                engine=engine,  # type: ignore
                                 version=version,
+                                engine=config.get("engine", None),
                                 api_method=api_method,
                                 search=search_config,
-                                params=_params,  # type: ignore
+                                params=new_params,  # type: ignore
                                 allow_get_all_pages=config.get("allow_get_all_pages", False),
                                 datasource=datasource,
                                 cache_expiration_time_seconds=cache_expiration_time_seconds,
                             )
                         )
             return ls
         else:
@@ -251,24 +244,25 @@
                 file_type=file_type,
                 select=select,
                 exclude=exclude,
                 sortby=sortby,
                 filters=None,
                 cache_expiration_time_seconds=cache_expiration_time_seconds,
             )
+            new_params = _with_implicit_parameters(_params, file_type, basic_config, datasource.uri)
 
             return [
                 cls(
                     name=name,
                     tag=tag,
                     version=version,
                     search=search_config,
-                    engine=engine,  # type: ignore
                     api_method=api_method,
-                    params=_params,  # type: ignore
+                    engine=config.get("engine", None),
+                    params=new_params,  # type: ignore
                     allow_get_all_pages=config.get("allow_get_all_pages", False),
                     datasource=datasource,
                     cache_expiration_time_seconds=cache_expiration_time_seconds,
                 )
             ]
 
     async def to_dict(self) -> dict:
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/dataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import pyarrow.parquet
 from aiocache import Cache, cached
 from aiocache.serializers import PickleSerializer
 
 from bmsdna.lakeapi.core.config import BasicConfig, DatasourceConfig, GroupByConfig, GroupByExpConfig, Param
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 from bmsdna.lakeapi.core.log import get_logger
-from bmsdna.lakeapi.core.model import get_param_def, should_hide_colname
+from bmsdna.lakeapi.core.model import get_param_def
 from bmsdna.lakeapi.core.types import DeltaOperatorTypes, FileTypes
 from bmsdna.lakeapi.context.df_base import ResultData, ExecutionContext
 import pypika
 from pypika.queries import QueryBuilder
 import pypika.queries as fn
 import duckdb
 
@@ -291,32 +291,40 @@
                 case "<>":
                     exprs.append(fn.Field(colname) != value if value is not None else fn.Field(colname).isnotnull())
                 case "==":
                     exprs.append(fn.Field(colname) == value if value is not None else fn.Field(colname).isnull())
                 case "=":
                     exprs.append(fn.Field(colname) == value if value is not None else fn.Field(colname).isnull())
                 case "not contains":
-                    exprs.append(fn.Field(colname).not_like.contains("%" + value + "%"))
+                    exprs.append(fn.Field(colname).not_like("%" + value + "%"))
                 case "contains":
                     exprs.append(fn.Field(colname).like("%" + value + "%"))
                 case "in":
                     lsv = cast(list[str], value)
                     if len(lsv) > 0:
                         exprs.append(fn.Field(colname).isin(lsv))
                 case "not in":
                     lsv = cast(list[str], value)
                     if len(lsv) > 0:
                         exprs.append(~fn.Field(colname).isin(lsv))
                 case "between":
                     lsv = cast(list[str], value)
                     if len(lsv) == 2:
                         exprs.append(fn.Field(colname).between(lsv[0], lsv[1]))
+                    else:
+                        from fastapi import HTTPException
+
+                        raise HTTPException(400, "Must have an array with 2 elements for between")
                 case "not between":
                     lsv = cast(list[str], value)
                     if len(lsv) == 2:
                         exprs.append(~fn.Field(colname).between(lsv[0], lsv[1]))
+                    else:
+                        from fastapi import HTTPException
+
+                        raise HTTPException(400, "Must have an array with 2 elements for between")
 
                 case operator:
                     logger.error(f"wrong parameter for filter {operator}")
 
     expr = await concat_expr(exprs)
     return expr
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,19 +27,16 @@
 from bmsdna.lakeapi.core.config import BasicConfig, Config, Configs, Param, SearchConfig
 from bmsdna.lakeapi.core.dataframe import (
     Dataframe,
     filter_df_based_on_params,
     filter_partitions_based_on_params,
 )
 from bmsdna.lakeapi.core.log import get_logger
-from bmsdna.lakeapi.core.model import (
-    create_parameter_model,
-    create_response_model,
-    should_hide_colname,
-)
+from bmsdna.lakeapi.core.model import create_parameter_model, create_response_model
+from bmsdna.lakeapi.core.partition_utils import should_hide_colname
 from bmsdna.lakeapi.core.response import create_response
 from bmsdna.lakeapi.core.types import (
     MetadataDetailResult,
     MetadataSchemaField,
     MetadataSchemaFieldType,
     OutputFileType,
     Engines,
@@ -120,29 +117,22 @@
     metamodel: Optional[ResultData], config: Config, configs: Configs, router: APIRouter, basic_config: BasicConfig
 ):
     route = config.route + "/metadata_detail"
     has_complex = True
     if metamodel is not None:
         has_complex = any((pa.types.is_nested(t) for t in metamodel.arrow_schema().types))
 
-    async def get_username(req: Request):
-        res = basic_config.username_retriever(req, basic_config, configs.users)
-        if inspect.isawaitable(res):
-            res = await res
-        return res
-
     @router.get(
         route,
         tags=["metadata", "metadata:" + config.tag],
         operation_id=config.tag + "_" + config.name,
         name=config.name + "_metadata",
     )
     def get_detailed_metadata(
         req: Request,
-        username=Depends(get_username),
         jsonify_complex: bool = Query(title="jsonify_complex", include_in_schema=has_complex, default=False),
     ) -> MetadataDetailResult:
         import json
 
         req.state.lake_api_basic_config = basic_config
         from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 
@@ -264,20 +254,14 @@
 ):
     route = config.route
 
     query_model = create_parameter_model(
         metamodel, config.tag + "_" + config.name + "_" + apimethod, config.params, config.search, apimethod
     )
 
-    async def get_username(req: Request):
-        res = basic_config.username_retriever(req, basic_config, configs.users)
-        if inspect.isawaitable(res):
-            res = await res
-        return res
-
     api_method_mapping = {
         "post": router.post(
             route,
             tags=[config.tag],
             response_model=response_model,
             operation_id=config.tag + "_" + config.name + "_" + apimethod,
             name=config.name,
@@ -304,19 +288,18 @@
         limit: Optional[int] = 100,
         offset: Optional[int] = 0,
         select: Union[str, None] = Query(title="$select", alias="$select", default=None, include_in_schema=False),
         distinct: bool = Query(title="$distinct", alias="$distinct", default=False, include_in_schema=False),
         engine: Engines = Query(title="$engine", alias="$engine", default="duckdb", include_in_schema=False),
         format: Optional[OutputFileType] = "json",
         jsonify_complex: bool = Query(title="jsonify_complex", include_in_schema=has_complex, default=False),
-        username=Depends(get_username),
     ):  # type: ignore
         logger.info(f"{params.dict(exclude_unset=True) if params else None}Union[ ,  ]{request.url.path}")
 
-        engine = engine or config.engine
+        engine = engine or basic_config.default_engine
 
         logger.info(f"Engine: {engine}")
 
         ExecutionContext = get_context_by_engine(engine)
 
         with ExecutionContext() as context:
             realdataframe = Dataframe(
@@ -395,15 +378,15 @@
 
             logger.info(f"Query: {get_sql(new_query)}")
 
             df2 = context.execute_sql(new_query)
 
             try:
                 return await create_response(
-                    username, request.url, format or request.headers["Accept"], df2, context, basic_config=basic_config
+                    request.url, format or request.headers["Accept"], df2, context, basic_config=basic_config
                 )
             except Exception as err:
                 logger.error("Error in creating response", exc_info=err)
                 raise HTTPException(status_code=500)
 
 
 duckcon: Optional[duckdb.DuckDBPyConnection] = None
@@ -414,27 +397,20 @@
 
     @router.on_event("shutdown")
     async def shutdown_event():
         global duckcon
         if duckcon is not None:
             duckcon.close()
 
-    async def get_username(req: Request):
-        res = basic_config.username_retriever(req, basic_config, configs.users)
-        if inspect.isawaitable(res):
-            res = await res
-        return res
-
     @router.get("/api/sql/tables", tags=["sql"], operation_id="get_sql_tables")
     async def get_sql_tables(
         request: Request,
         background_tasks: BackgroundTasks,
         Accept: Union[str, None] = Header(default=None),
         format: Optional[OutputFileType] = "json",
-        username=Depends(get_username),
     ):
         try:
             return [table for table in paths]
         except Exception as err:
             raise HTTPException(status_code=500, detail=str(err))
 
     @router.post(
@@ -443,29 +419,28 @@
         operation_id="post_sql_endpoint",
     )
     async def get_sql_post(
         request: Request,
         background_tasks: BackgroundTasks,
         Accept: Union[str, None] = Header(default=None),
         format: Optional[OutputFileType] = "json",
-        username=Depends(get_username),
     ):
         try:
             body = await request.body()
             from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContextBase
 
             global duckcon
             if duckcon is None:
                 duckcon = duckdb.connect()
                 register_duckdb_views(duckcon, paths)
             context = DuckDbExecutionContextBase(duckcon)
             df = context.execute_sql(body.decode("utf-8"))
 
             return await create_response(
-                username, request.url, format or request.headers["Accept"], df, context, basic_config=basic_config
+                request.url, format or request.headers["Accept"], df, context, basic_config=basic_config
             )
         except Exception as err:
             logger.error(err)
             raise HTTPException(status_code=500, detail=str(err))
 
     @router.get(
         "/api/sql",
@@ -474,25 +449,24 @@
     )
     async def get_sql_get(
         request: Request,
         background_tasks: BackgroundTasks,
         sql: str,
         Accept: Union[str, None] = Header(default=None),
         format: Optional[OutputFileType] = "json",
-        username=Depends(get_username),
     ):
         try:
             from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContextBase
 
             global duckcon
             if duckcon is None:
                 duckcon = duckdb.connect()
                 register_duckdb_views(duckcon, paths)
             context = DuckDbExecutionContextBase(duckcon)
 
             df = context.execute_sql(sql)
             return await create_response(
-                username, request.url, format or request.headers["Accept"], df, context, basic_config=basic_config
+                request.url, format or request.headers["Accept"], df, context, basic_config=basic_config
             )
         except Exception as err:
             logger.error(err)
             raise HTTPException(status_code=500, detail=str(err))
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from bmsdna.lakeapi.context.df_base import ResultData
 from aiocache import Cache, cached
 from aiocache.serializers import PickleSerializer
 from fastapi import Query
 from pydantic import BaseModel, create_model
 from bmsdna.lakeapi.context.df_base import ResultData
 from bmsdna.lakeapi.core.config import Param, SearchConfig
+from bmsdna.lakeapi.core.partition_utils import should_hide_colname
 from bmsdna.lakeapi.core.types import OperatorType
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 import pyarrow as pa
 
 cache = cached(ttl=CACHE_EXPIRATION_TIME_SECONDS, cache=Cache.MEMORY, serializer=PickleSerializer())
 
 
@@ -165,18 +166,14 @@
 
 
 class TypeBaseModel(BaseModel):
     class Config:
         orm_mode = True
 
 
-def should_hide_colname(name: str):
-    return name.startswith("_") or "_md5_prefix_" in name or "_xxhash64_prefix_" in name or "_md5_mod_" in name
-
-
 def create_response_model(name: str, frame: ResultData) -> type[BaseModel]:
     schema = frame.arrow_schema()
     props = {
         k: get_schema_for(name, schema.field(k).name, schema.field(k).type)
         for k in schema.names
         if not should_hide_colname(k)
     }
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/response.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from enum import Enum
 from typing import Union
 from uuid import uuid4
 
 import anyio
 import pyarrow as pa
 from fastapi import BackgroundTasks
+from starlette.background import BackgroundTask
 from starlette.datastructures import URL
 from starlette.responses import FileResponse
 
 from bmsdna.lakeapi.context.df_base import ExecutionContext, ResultData
 from bmsdna.lakeapi.core.config import BasicConfig
 from bmsdna.lakeapi.core.log import get_logger
 from bmsdna.lakeapi.core.types import OutputFileType
@@ -29,15 +30,14 @@
     HTML = 4
     ARROW_IPC = 5
     ND_JSON = 6
     PARQUET = 7
     JSON = 8
     XML = 9
     ORC = 10
-    IQY = 13
     ARROW_STREAM = 14
 
 
 def parse_format(accept: Union[str, OutputFileType]) -> tuple[OutputFormats, str]:
     realaccept = accept.split(";")[0].strip().lower()
     if realaccept == "application/avro" or realaccept == "avro":
         return (OutputFormats.AVRO, ".avro")
@@ -51,17 +51,14 @@
         return (OutputFormats.XML, ".xml")
     elif realaccept == "orc":
         return (OutputFormats.ORC, ".orc")
     elif realaccept == mimetypes.guess_type("file.xlsx") or realaccept == "xlsx":
         return (OutputFormats.XLSX, ".xlsx")
     elif realaccept == "text/html" or realaccept == "html":
         return (OutputFormats.HTML, ".html")
-    elif realaccept == "x-application/iqy" or realaccept == "iqy":
-        return (OutputFormats.IQY, ".iqy")
-
     elif realaccept == "application/vnd.apache.arrow.stream" or realaccept == "arrow-stream":
         return (OutputFormats.ARROW_STREAM, "")
 
     elif (
         realaccept == "application/x-arrow"
         or realaccept == "application/x-arrow"
         or realaccept == "application/vnd.apache.arrow.file"
@@ -75,75 +72,38 @@
     elif realaccept == "application/parquet" or realaccept == "parquet":
         return (OutputFormats.PARQUET, ".parquet")
     else:
         return (OutputFormats.JSON, ".json")
 
 
 def write_frame(
-    url: URL, current_user: str, content: ResultData, format: OutputFormats, out: str, basic_config: BasicConfig
-):
-    if format == OutputFormats.IQY:
-        import jwt
-
-        import env
-
-        query = url.query.replace("format=iqy", "").rstrip("&")
-        query = query + ("?" if not query else "&") + "format=json"
-        token = jwt.encode(
-            {"host": url.hostname, "path": url.path, "username": current_user},
-            basic_config.token_jwt_secret,
-            algorithm="HS256",
-        )
-        query += f"&token={token}"
-        host_and_port = (url.hostname or "localhost") + (":" + str(url.port) if url.port and url.port != 443 else "")
-        strdt = f"""WEB
-1
-{url.scheme}://{host_and_port}{url.path}?{query}
-
-Selection=1
-Formatting=None
-PreFormattedTextToColumns=True
-ConsecutiveDelimitersAsOne=False
-SingleBlockTextImport=False
-DisableDateRecognition=False
-DisableRedirections=False"""
-        if isinstance(out, str):
-            with open(out, "w") as f:
-                f.write(strdt)
-        else:
-            out.write(strdt.encode("utf-8"))
-        return
-
+    url: URL, content: ResultData, format: OutputFormats, out: str, basic_config: BasicConfig
+) -> list[str]:
     if format == OutputFormats.AVRO:
         import polars as pl
 
         ds = pl.from_arrow(content.to_arrow_recordbatch())
         assert isinstance(ds, pl.DataFrame)
         ds.write_avro(out)
     elif format == OutputFormats.CSV:
         content.write_csv(out, separator=",")
     elif format == OutputFormats.SEMI_CSV:
         content.write_csv(out, separator=";")
     elif format == OutputFormats.CSV4EXCEL:  # need to write sep=, on first line
-        if isinstance(out, str):
-            content.write_csv(out + "_u8", separator=",")  # type: ignore
-            with open(
-                out, mode="wb"
-            ) as f:  # excel wants utf-16le which polars does not support. therefore we need reencoding
-                f.write(b"sep=,\n")  # add utf-8 bom at beginning
-                with open(out + "_u8", mode="r", encoding="utf-8") as c8:
+        content.write_csv(out + "_u8", separator=",")  # type: ignore
+        with open(
+            out, mode="wb"
+        ) as f:  # excel wants utf-16le which polars does not support. therefore we need reencoding
+            f.write(b"sep=,\n")  # add utf-8 bom at beginning
+            with open(out + "_u8", mode="r", encoding="utf-8") as c8:
+                line = c8.readline()
+                while line != "":
+                    f.write(line.encode("utf-16le"))
                     line = c8.readline()
-                    while line != "":
-                        f.write(line.encode("utf-16le"))
-                        line = c8.readline()
-                os.remove(out + "_u8")
-
-        else:
-            out.write(b"sep=,\r\n")  # not used, and would break special characters
-            content.write_csv(out, separator=",")
+            return [out + "_u8"]
     elif format == OutputFormats.XLSX:
         import polars as pl
 
         ds = pl.from_arrow(content.to_arrow_table())
         assert isinstance(ds, pl.DataFrame)
         ds.write_excel(out, autofit=True)
     elif format == OutputFormats.HTML:
@@ -161,18 +121,25 @@
 
     elif format == OutputFormats.ND_JSON:
         content.write_nd_json(out)
     elif format == OutputFormats.PARQUET:
         content.write_parquet(out)
     else:
         content.write_json(out)
+    return []
+
+
+class FileResponseWCharset(FileResponse):
+    def __init__(self, *args, **kwargs):
+        if "charset" in kwargs:
+            self.charset = kwargs.pop("charset")
+        super().__init__(*args, **kwargs)
 
 
 async def create_response(
-    current_user_name: str,
     url: URL,
     accept: str,
     content: ResultData,
     context: ExecutionContext,
     basic_config: BasicConfig,
 ):
     headers = {}
@@ -188,42 +155,33 @@
         OutputFormats.CSV,
         OutputFormats.SEMI_CSV,
         OutputFormats.CSV4EXCEL,
     ]:
         content_dispositiont_type = "inline"
         filename = None
     path = os.path.join(basic_config.temp_folder_path, str(uuid4()) + extension)
-    media_type = mimetypes.guess_type("file" + extension)[0]
-    write_frame(
-        current_user=current_user_name, url=url, content=content, format=format, out=path, basic_config=basic_config
-    )
+    media_type = "text/csv" if extension == ".csv" else mimetypes.guess_type("file" + extension)[0]
+    additional_files = write_frame(url=url, content=content, format=format, out=path, basic_config=basic_config)
 
-    if media_type is not None and format in [
-        OutputFormats.JSON,
-        OutputFormats.ND_JSON,
-        OutputFormats.CSV,
-        OutputFormats.SEMI_CSV,
-        OutputFormats.CSV4EXCEL,
-        OutputFormats.HTML,
-        OutputFormats.XLSX,
-        OutputFormats.XML,
-    ]:
-        media_type = media_type + ";charset=utf-8"
     tasks = BackgroundTasks()
     import asyncio
 
     async def remove():
         context.close()
         await anyio.sleep(3)
 
         os.remove(path)
+        for f in additional_files:
+            os.remove(f)
 
     tasks.add_task(remove)
 
-    return FileResponse(
+    fr = FileResponseWCharset(
         path=path,
         headers=headers,
         media_type=media_type,
         content_disposition_type=content_dispositiont_type,
         filename=filename,
         background=tasks,
+        charset="utf-16le" if format == OutputFormats.CSV4EXCEL else "utf-8",
     )
+    return fr
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/route.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,20 +20,14 @@
     from bmsdna.lakeapi.core.endpoint import (
         get_response_model,
         create_detailed_meta_endpoint,
         create_config_endpoint,
         create_sql_endpoint,
     )
 
-    async def get_username(req: Request):
-        res = basic_config.username_retriever(req, basic_config, configs.users)
-        if inspect.isawaitable(res):
-            res = await res
-        return res
-
     all_lake_api_routers.append((basic_config, configs))
     router = APIRouter()
     metadata = []
 
     with DuckDbExecutionContext() as context:
         for config in configs:
             methods = (
@@ -87,15 +81,15 @@
                     configs=configs,
                 )
 
         @router.get(
             "/metadata",
             name="metadata",
         )
-        async def get_metadata(username: str = Depends(get_username)):
+        async def get_metadata():
             return metadata
 
         if basic_config.enable_sql_endpoint:
             create_sql_endpoint(
                 router=router,
                 basic_config=basic_config,
                 configs=configs,
@@ -108,11 +102,11 @@
                 if config.search:
                     from bmsdna.lakeapi.core.dataframe import Dataframe
 
                     realdataframe = Dataframe(
                         config.version_str, config.tag, config.name, config.datasource, context, basic_config
                     )
                     if realdataframe.file_exists():
-                        with get_context_by_engine(config.engine)() as ctx:
+                        with get_context_by_engine(basic_config.default_engine)() as ctx:
                             ctx.init_search(realdataframe.tablename, config.search)
 
-        return router, get_username
+        return router
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 from decimal import Decimal
 from typing import Type, Optional, TYPE_CHECKING
 from typing_extensions import TypedDict
 from polars.datatypes.convert import DataTypeMappings
 from pydantic import BaseModel
 
 
-Engines = Literal["duckdb", "polars", "datafusion"]
+Engines = Literal["duckdb", "polars"]
 
 
 FileTypes = Literal[
     "delta",
     "parquet",
     "arrow",
     "arrow-stream",
     "avro",
     "csv",
     "json",
     "ndjson",
-    "parquet_withdecimal",
 ]
 OutputFileType = Literal[
     "json",
     "ndjson",
     "parquet",
     "csv",
     "csv4excel",
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/uservalidation.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 from bmsdna.lakeapi.core.config import BasicConfig, Configs, UserConfig
 from bmsdna.lakeapi.core.yaml import get_yaml
 import inspect
 from aiocache import cached, Cache
 from aiocache.serializers import PickleSerializer
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
+from fastapi import FastAPI, Response
 
 cache = cached(
     ttl=CACHE_EXPIRATION_TIME_SECONDS * 10000,
     cache=Cache.MEMORY,
     serializer=PickleSerializer(),
 )
 
@@ -24,41 +25,43 @@
 async def is_correct(hash: str, pwd_str: str):
     import argon2
 
     ph = argon2.PasswordHasher()
     return ph.verify(hash.encode("utf-8"), pwd_str.encode("utf-8"))
 
 
-async def get_username(req: Request, basic_config: BasicConfig, users: Sequence[UserConfig]):
-    if req.query_params.get("token") and basic_config.token_jwt_secret is not None:
-        import jwt
-
-        token = req.query_params["token"]
-        dt = jwt.decode(token, basic_config.token_jwt_secret, algorithms=["HS256"])
-        if dt["path"] == req.url.path or dt["host"] == req.url.hostname:
-            return dt["username"]
-    credentials = await HTTPBasic(auto_error=True)(req)
-    assert credentials is not None
-    global userhashmap
-    userhashmap = userhashmap or {
-        ud["name"].casefold(): ud["passwordhash"] for ud in users if ud["name"]
-    }  # pay attention not to include an empty user by accident
-
-    if not credentials.username.casefold() in userhashmap.keys():
-        raise HTTPException(
-            status_code=status.HTTP_401_UNAUTHORIZED,
-            detail="Incorrect email or password",
-            headers={"WWW-Authenticate": "Basic"},
-        )
-    pwd_str = credentials.password
-    hash = userhashmap[credentials.username.casefold()]
-
-    is_correct_password = is_correct(hash, pwd_str)
-    if not isinstance(is_correct_password, bool):
-        is_correct_password = await is_correct_password
-    if not is_correct_password:
-        raise HTTPException(
-            status_code=status.HTTP_401_UNAUTHORIZED,
-            detail="Incorrect email or password",
-            headers={"WWW-Authenticate": "Basic"},
-        )
-    return credentials.username
+def add_user_middlware(app: FastAPI, basic_config: BasicConfig, users: Sequence[UserConfig]):
+    @app.middleware("http")
+    async def get_username(request: Request, call_next):
+        import json
+
+        credentials = await HTTPBasic(auto_error=False)(request)
+        if credentials is None:
+            return Response(
+                status_code=401,
+                headers={"WWW-Authenticate": "Basic"},
+                content=json.dumps({"detail": "Not authenticated"}),
+            )
+
+        global userhashmap
+        userhashmap = userhashmap or {
+            ud["name"].casefold(): ud["passwordhash"] for ud in users if ud["name"]
+        }  # pay attention not to include an empty user by accident
+
+        if not credentials.username.casefold() in userhashmap.keys():
+            return Response(
+                status_code=401,
+                headers={"WWW-Authenticate": "Basic"},
+                content=json.dumps({"detail": "Incorrect email or password"}),
+            )
+        pwd_str = credentials.password
+        hash = userhashmap[credentials.username.casefold()]
+
+        is_correct_password = is_correct(hash, pwd_str)
+        if not isinstance(is_correct_password, bool):
+            is_correct_password = await is_correct_password
+        if not is_correct_password:
+            return Response(
+                status_code=401, headers={"WWW-Authenticate": "Basic"}, content="Incorrect email or password"
+            )
+        request.scope["user"] = {"username": credentials.username}
+        return await call_next(request)
```

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.7/pyproject.toml` & `bmsdna_lakeapi-0.5.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.4.7"
+version = "0.5.1"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = "^0.95.1"
 deltalake = "^0.9.0"
 pyyaml = "^6.0"
 aiocache = "^0.12.1"
 pypika = "^0.48.9"
 duckdb = "^0.8.0"
-polars = "^0.17.14"
+polars = "^0.18.0"
 
 # schema stuff
 jsonschema = {version = "^4.17.3", optional=true}
 python2jsonschema = { version ="^0.8", optional=true}
 
 # polars stuff
 xlsx2csv = { version ="^0.8.1", optional = true }
 
 # auth
 argon2-cffi = {version = "^21.3.0", optional=true}
 
-# datafusion
-datafusion = {version = "^24.0.0", optional = true }
 xlsxwriter = "^3.1.0"
 pyjwt = {version = "^2.6.0", optional = true}
 "ruamel.yaml" = {version = "^0.17.26", optional = true}
 
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.308"
@@ -50,14 +48,15 @@
 pytest = "^7.3.1"
 httpx = "^0.24.0"
 pytest-env = "^0.8.1"
 pytest-cov = "^4.0.0"
 pytest-benchmark = "^4.0.0"
 pandas = "^2.0.1"
 pytest-monitor = "^1.6.5"
+coverage = {extras = ["toml"], version = "^7.2.7"}
 
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
@@ -70,13 +69,21 @@
 [tool.black]
 line-length = 119
 
 [tool.poetry.extras]
 schema = ["jsonschema", "python2jsonschema"]
 polars = ["xlsx2csv"]
 auth = ["argon2-cffi", "pyjwt"]
-datafusion= ["datafusion"]
 useradd = ["ruamel.yaml"]
 
 [tool.poetry.scripts]
 validate_lakeapi_schema = { callable = "bmsdna.lakeapi.tools.validateschema:validate_schema_cli", extras = ["schema"] }
-add_lakeapi_user = { callable = "bmsdna.lakeapi.tools.useradd:useradd_cli", extras = ["useradd"] }
+add_lakeapi_user = { callable = "bmsdna.lakeapi.tools.useradd:useradd_cli", extras = ["useradd"] }
+
+[tool.coverage.report]
+exclude_lines =[ "pragma: no cover",
+"if TYPE_CHECKING:",
+"if __name__ == .__main__.:",
+"@(abc.)?abstractmethod",
+"raise AssertionError",
+"raise NotImplementedError"
+]
```

### Comparing `bmsdna_lakeapi-0.4.7/PKG-INFO` & `bmsdna_lakeapi-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.4.7
+Version: 0.5.1
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: auth
-Provides-Extra: datafusion
 Provides-Extra: polars
 Provides-Extra: schema
 Provides-Extra: useradd
 Requires-Dist: aiocache (>=0.12.1,<0.13.0)
 Requires-Dist: argon2-cffi (>=21.3.0,<22.0.0) ; extra == "auth"
-Requires-Dist: datafusion (>=24.0.0,<25.0.0) ; extra == "datafusion"
 Requires-Dist: deltalake (>=0.9.0,<0.10.0)
 Requires-Dist: duckdb (>=0.8.0,<0.9.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0) ; extra == "schema"
-Requires-Dist: polars (>=0.17.14,<0.18.0)
+Requires-Dist: polars (>=0.18.0,<0.19.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0) ; extra == "auth"
 Requires-Dist: pypika (>=0.48.9,<0.49.0)
 Requires-Dist: python2jsonschema (>=0.8,<0.9) ; extra == "schema"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: ruamel.yaml (>=0.17.26,<0.18.0) ; extra == "useradd"
 Requires-Dist: xlsx2csv (>=0.8.1,<0.9.0) ; extra == "polars"
 Requires-Dist: xlsxwriter (>=3.1.0,<4.0.0)
@@ -70,26 +68,28 @@
 [![PyPI version](https://badge.fury.io/py/bmsdna-lakeapi.svg)](https://pypi.org/project/bmsdna-lakeapi/)
 
 Pypi Package `bmsdna-lakeapi` can be installed like any python package : `pip install bmsdna-lakeapi`
 
 ## Basic Idea
 
 Based on a `YAML` configuration and the data source, LakeAPI will automatically generate GET and/or POST endpoints.
-Calling the endpoint turns the query into an SQL statement that can be executed with the engine of your choice (duckdb, datafusion or polars).
+Calling the endpoint turns the query into an SQL statement that can be executed with the engine of your choice (duckdb or polars).
 The result is then seralised into the requested format (Json, CSV, Arrow etc).
 
+This makes it super easy to distribute your data lake data to other systems. We use it internally to feed data to MS SQL Server, SQLite, Streamlit and Web Apps. You can host it wherever you want, we use Azure Websites which works fine even for very large data amounts.
+
 ## OpenAPI
 
 Of course everything works with `OpenAPI` and `FastAPI`. This means you can add other FastAPI routes, you can use the /docs and /redoc endpoints.
 
 So everything will be fully documented automatically, which is really cool. 🔥🔥
 
 ## Engine
 
-`DuckDB` is the default query engine. `Polars` and `Datafusion` are also supported, but lack some features. The query engine can be specified at the route level and at the query level with the hidden parameter $engine="duckdb|datafusion|polars". If you want polars or datafusion, add the required extra.
+`DuckDB` is the default query engine. `Polars` is also supported, but lack some features. The query engine can be specified at the route level and at the query level with the hidden parameter $engine="duckdb|polars". If you want polars, add the required extra.
 
 At the moment, DuckDB seems to have an advantage and performs the best. Also features like full text search are only available with `DuckDB`.
 
 ## Default Security
 
 By Default, Basic Authentication is enabled. To add a user, simply run `add_lakeapi_user YOURUSERNAME --yaml-file config.yml`. This will add the user to your config yaml (argon2 encrypted).
 The generated Password is printed. If you do not want this logic, you can overwrite the username_retriver of the Default Config
@@ -252,12 +252,17 @@
 - Metadata endpoints to retrieve data types, string lengths and more
 - Easily expose entire folders by using a "\*" wildcard in both the name and the datasource.uri config, see example in the config above
 - Good test coverage
 
 ## Work in progress
 
 Please note that this is a work in progress, changes will be made and things may break. Especially at this early stage.
+We recommend only using the export from `bmsdna.lakeapi` for now and not to use the submodules.
+
+## Limitations
+
+- You can currently only serve local files. We might add support for `fsspec` later on. You can still mount your data if you use Linux, which is what we do in production
 
 ## Contribution
 
 Feel free to contribute, report bugs or request enhancements.
```

