# Comparing `tmp/calitp_map_utils-2023.5.24.tar.gz` & `tmp/calitp_map_utils-2023.5.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_map_utils-2023.5.24.tar", max compression
+gzip compressed data, was "calitp_map_utils-2023.5.31.tar", max compression
```

## Comparing `calitp_map_utils-2023.5.24.tar` & `calitp_map_utils-2023.5.31.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      944 2023-05-23 18:00:10.633586 calitp_map_utils-2023.5.24/README.md
--rw-r--r--   0        0        0     4290 2023-05-24 15:33:39.118930 calitp_map_utils-2023.5.24/calitp_map_utils/__init__.py
--rw-r--r--   0        0        0       44 2023-05-23 18:00:10.635825 calitp_map_utils-2023.5.24/calitp_map_utils/__main__.py
--rw-r--r--   0        0        0     1409 2023-05-24 15:28:37.116341 calitp_map_utils-2023.5.24/calitp_map_utils/cli.py
--rw-r--r--   0        0        0      626 2023-05-24 18:37:37.869199 calitp_map_utils-2023.5.24/pyproject.toml
--rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 calitp_map_utils-2023.5.24/PKG-INFO
+-rw-r--r--   0        0        0      944 2023-05-31 19:48:46.649796 calitp_map_utils-2023.5.31/README.md
+-rw-r--r--   0        0        0     4963 2023-05-31 19:48:46.650512 calitp_map_utils-2023.5.31/calitp_map_utils/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-31 19:48:46.650988 calitp_map_utils-2023.5.31/calitp_map_utils/__main__.py
+-rw-r--r--   0        0        0     1441 2023-05-31 19:48:46.651582 calitp_map_utils-2023.5.31/calitp_map_utils/cli.py
+-rw-r--r--   0        0        0      646 2023-05-31 19:48:54.451038 calitp_map_utils-2023.5.31/pyproject.toml
+-rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 calitp_map_utils-2023.5.31/PKG-INFO
```

### Comparing `calitp_map_utils-2023.5.24/README.md` & `calitp_map_utils-2023.5.31/README.md`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.5.24/calitp_map_utils/cli.py` & `calitp_map_utils-2023.5.31/calitp_map_utils/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 import gzip
 import json
 import sys
 from typing import Optional
 
 import typer
 
-from . import Analysis, State
+from . import LayerType, State
 from . import validate_geojson as validate_geojson_func
 
 app = typer.Typer()
 
 
 @app.command()
-def validate_geojson(path: str, analysis: Optional[Analysis] = None):
-    collection = validate_geojson_func(path, analysis, verbose=True)
+def validate_geojson(path: str, kind: Optional[LayerType] = None):
+    collection = validate_geojson_func(path, kind, verbose=True)
 
     typer.secho(
         f"Success! Validated {len(collection.features)} features.",
         fg=typer.colors.GREEN,
     )
 
 
 @app.command()
 def validate_state(
     infile: Optional[str] = None,
     base64url: bool = False,
     compressed: bool = False,
     data: bool = False,
     verbose: bool = False,
+    host: Optional[str] = None,
 ):
     if infile:
         typer.secho(f"Reading {infile}.")
         with open(infile) as f:
             contents = f.read()
     else:
         typer.secho("Reading from stdin...")
@@ -48,8 +49,8 @@
 
         contents = byts.decode()
 
     state = State(**json.loads(contents))
     state.validate_layers(verbose=verbose, data=data)
     typer.secho("Validation successful!", fg=typer.colors.GREEN)
     typer.secho(f"Creating URL from state {state.json()}...")
-    typer.secho(f"URL: {state.iframe_url}")
+    typer.secho(f"URL: {state.iframe_url(host)}")
```

### Comparing `calitp_map_utils-2023.5.24/pyproject.toml` & `calitp_map_utils-2023.5.31/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calitp_map_utils"
-version = "2023.5.24"
+version = "2023.5.31"
 description = ""
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.9"
 pyyaml = "^6.0"
@@ -20,11 +20,12 @@
 [tool.poetry.group.dev.dependencies]
 pydantic-to-typescript = "^1.0.10"
 mypy = "^1.3.0"
 types-tqdm = "^4.65.0.1"
 types-requests = "^2.30.0.0"
 pytest = "^7.3.1"
 pytest-spec = "^3.2.0"
+erdantic = "^0.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `calitp_map_utils-2023.5.24/PKG-INFO` & `calitp_map_utils-2023.5.31/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calitp-map-utils
-Version: 2023.5.24
+Version: 2023.5.31
 Summary: 
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: calitp-data (==2023.2.13.1)
```

