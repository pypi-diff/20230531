# Comparing `tmp/didas-3.0.0.tar.gz` & `tmp/didas-3.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/didas/didas/dist/.tmp-5xestc5n/didas-3.0.0.tar", last modified: Tue Nov 29 21:29:58 2022, max compression
+gzip compressed data, was "/home/runner/work/didas/didas/dist/.tmp-vogca9pe/didas-3.0.1rc1.tar", last modified: Wed May 31 16:37:37 2023, max compression
```

## Comparing `didas-3.0.0.tar` & `didas-3.0.1rc1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 21:29:58.000000 didas-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 21:29:58.000000 didas-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 21:29:58.000000 didas-3.0.0/.github/linters/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-11-29 21:29:49.000000 didas-3.0.0/.github/linters/.flake8
--rw-r--r--   0 runner    (1001) docker     (116)       31 2022-11-29 21:29:49.000000 didas-3.0.0/.github/linters/.python-black
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 21:29:58.000000 didas-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1294 2022-11-29 21:29:49.000000 didas-3.0.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1799 2022-11-29 21:29:49.000000 didas-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1090 2022-11-29 21:29:58.000000 didas-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      221 2022-11-29 21:29:49.000000 didas-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 21:29:58.000000 didas-3.0.0/didas/
--rw-r--r--   0 runner    (1001) docker     (116)      412 2022-11-29 21:29:49.000000 didas-3.0.0/didas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2022-11-29 21:29:58.000000 didas-3.0.0/didas/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     1465 2022-11-29 21:29:49.000000 didas-3.0.0/didas/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (116)     9877 2022-11-29 21:29:49.000000 didas-3.0.0/didas/oracle.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 21:29:58.000000 didas-3.0.0/didas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1090 2022-11-29 21:29:58.000000 didas-3.0.0/didas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      342 2022-11-29 21:29:58.000000 didas-3.0.0/didas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-29 21:29:58.000000 didas-3.0.0/didas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      120 2022-11-29 21:29:58.000000 didas-3.0.0/didas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2022-11-29 21:29:58.000000 didas-3.0.0/didas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1264 2022-11-29 21:29:49.000000 didas-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       41 2022-11-29 21:29:49.000000 didas-3.0.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-29 21:29:58.000000 didas-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:37:37.000000 didas-3.0.1rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:37:37.000000 didas-3.0.1rc1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-31 16:37:21.000000 didas-3.0.1rc1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:37:37.000000 didas-3.0.1rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:37:37.000000 didas-3.0.1rc1/.github/linters/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 16:37:21.000000 didas-3.0.1rc1/.github/linters/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-31 16:37:21.000000 didas-3.0.1rc1/.github/linters/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 16:37:21.000000 didas-3.0.1rc1/.github/linters/.python-black
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:37:37.000000 didas-3.0.1rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-31 16:37:21.000000 didas-3.0.1rc1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-31 16:37:21.000000 didas-3.0.1rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-31 16:37:37.000000 didas-3.0.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-31 16:37:21.000000 didas-3.0.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:37:37.000000 didas-3.0.1rc1/didas/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-31 16:37:21.000000 didas-3.0.1rc1/didas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-31 16:37:36.000000 didas-3.0.1rc1/didas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-31 16:37:21.000000 didas-3.0.1rc1/didas/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-31 16:37:21.000000 didas-3.0.1rc1/didas/oracle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:37:37.000000 didas-3.0.1rc1/didas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-31 16:37:37.000000 didas-3.0.1rc1/didas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-31 16:37:37.000000 didas-3.0.1rc1/didas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:37:37.000000 didas-3.0.1rc1/didas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-31 16:37:37.000000 didas-3.0.1rc1/didas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 16:37:37.000000 didas-3.0.1rc1/didas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-31 16:37:21.000000 didas-3.0.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 16:37:21.000000 didas-3.0.1rc1/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 16:37:37.000000 didas-3.0.1rc1/setup.cfg
```

### Comparing `didas-3.0.0/.github/workflows/pypi.yml` & `didas-3.0.1rc1/.github/workflows/pypi.yml`

 * *Files 7% similar despite different names*

```diff
@@ -6,27 +6,26 @@
   push:
     tags:
       - '*'
 
 jobs:
   linter:
     name: Lint Code Base
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Lint Code Base
-        uses: docker://ghcr.io/github/super-linter:slim-v4
+        uses: super-linter/super-linter@v5
         env:
-          DEFAULT_BRANCH: main
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
   build-n-publish:
     needs: linter
     name: Build and publish Python 🐍 distributions 📦 to PyPI and TestPyPI
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: '0'
       - name: Set up Python 3.7
         uses: actions/setup-python@v4
         with:
```

### Comparing `didas-3.0.0/.gitignore` & `didas-3.0.1rc1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -123,7 +123,9 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+*/_version.py
```

### Comparing `didas-3.0.0/PKG-INFO` & `didas-3.0.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: didas
-Version: 3.0.0
+Version: 3.0.1rc1
 Summary: Python Commons for Didas
 Author-email: Georg Wendorf <georgfriedrich.wendorf@freenet.ag>
 Maintainer-email: Georg Wendorf <georgfriedrich.wendorf@freenet.ag>
 Project-URL: Homepage, https://github.com/freenet-group/didas
 Project-URL: Documentation, https://github.com/freenet-group/didas/blob/main/README.md
 Project-URL: Repository, https://github.com/freenet-group/didas
 Project-URL: Changelog, https://github.com/freenet-group/didas/releases
```

### Comparing `didas-3.0.0/didas/mlflow.py` & `didas-3.0.1rc1/didas/mlflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import google.auth.transport.requests
 import google.oauth2.id_token
 import mlflow.tracking
 import pandas as pd
 
 
-def set_google_tracking_token(tracking_uri=None, tracking_token=None):
+def set_google_tracking_token(tracking_uri=None, tracking_token=None, google_application_credentials=None):
+    if google_application_credentials is not None:
+        os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = google_application_credentials
     if tracking_uri is not None:
         os.environ["MLFLOW_TRACKING_URI"] = tracking_uri
     if tracking_token is None:
         os.environ["MLFLOW_TRACKING_TOKEN"] = google.oauth2.id_token.fetch_id_token(
             request=google.auth.transport.requests.Request(),
             audience=os.environ["MLFLOW_TRACKING_URI"],
         )
```

### Comparing `didas-3.0.0/didas/oracle.py` & `didas-3.0.1rc1/didas/oracle.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from sqlalchemy import String, create_engine
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import DatabaseError
 from tqdm import tqdm
 
 
 def get_engine(
-    oracle_username: str = None,
-    oracle_password: str = None,
+    oracle_username: str = "",
+    oracle_password: str = "",
     oracle_hosts: set = set(),
-    oracle_port: int = None,
-    oracle_servicename: str = None,
+    oracle_port: int = -1,
+    oracle_servicename: str = "",
 ) -> Engine:
-    oracle_username = oracle_username or os.environ["ORACLE_USER"]
-    oracle_password = oracle_password or os.environ["ORACLE_PASS"]
+    oracle_username = oracle_username if oracle_username != "" else os.environ["ORACLE_USER"]
+    oracle_password = oracle_password if oracle_password != "" else os.environ["ORACLE_PASS"]
     oracle_hosts |= {v for k, v in os.environ.items() if k.startswith("ORACLE_HOST")}
-    oracle_port = oracle_port or int(os.environ["ORACLE_PORT"])
-    oracle_servicename = oracle_servicename or os.environ["ORACLE_SERVICE_NAME"]
+    oracle_port = oracle_port if oracle_port != -1 else int(os.getenv("ORACLE_PORT", "1521"))
+    oracle_servicename = oracle_servicename if oracle_servicename != "" else os.environ["ORACLE_SERVICE_NAME"]
     assert len(oracle_hosts) > 0
     excs = dict()
     for oracle_host in oracle_hosts:
-        engine = create_engine(f"oracle+cx_oracle://{oracle_username}:{oracle_password}@{oracle_host}:{oracle_port}/?service_name={oracle_servicename}", max_identifier_length=128)
+        engine = create_engine(f"oracle+oracledb://{oracle_username}:{oracle_password}@{oracle_host}:{oracle_port}/?service_name={oracle_servicename}")
         try:
             with engine.begin():
                 return engine
         except DatabaseError as e:
             excs[oracle_host] = e
     assert False, excs
```

### Comparing `didas-3.0.0/didas.egg-info/PKG-INFO` & `didas-3.0.1rc1/didas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: didas
-Version: 3.0.0
+Version: 3.0.1rc1
 Summary: Python Commons for Didas
 Author-email: Georg Wendorf <georgfriedrich.wendorf@freenet.ag>
 Maintainer-email: Georg Wendorf <georgfriedrich.wendorf@freenet.ag>
 Project-URL: Homepage, https://github.com/freenet-group/didas
 Project-URL: Documentation, https://github.com/freenet-group/didas/blob/main/README.md
 Project-URL: Repository, https://github.com/freenet-group/didas
 Project-URL: Changelog, https://github.com/freenet-group/didas/releases
```

### Comparing `didas-3.0.0/pyproject.toml` & `didas-3.0.1rc1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     "pytest"
 ]
 dev = [
     "black",
     "flake8"
 ]
 oracle = [
-    "cx-Oracle",
-    "SQLAlchemy",
+    "oracledb",
+    "SQLAlchemy>=2",
     "tqdm",
     "numpy"
 ]
 mlflow = [
     "pandas",
     "mlflow-skinny",
     "google-auth"
```

