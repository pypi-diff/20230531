# Comparing `tmp/mlflow_aws_rds_iam-0.2.0.tar.gz` & `tmp/mlflow_aws_rds_iam-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_aws_rds_iam-0.2.0.tar", max compression
+gzip compressed data, was "mlflow_aws_rds_iam-0.2.1.tar", max compression
```

## Comparing `mlflow_aws_rds_iam-0.2.0.tar` & `mlflow_aws_rds_iam-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1085 2023-05-20 10:38:40.387615 mlflow_aws_rds_iam-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     1555 2023-05-20 10:38:40.387615 mlflow_aws_rds_iam-0.2.0/README.md
--rw-r--r--   0        0        0      227 2023-05-20 10:38:40.387615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/__init__.py
--rw-r--r--   0        0        0   174184 2023-05-20 10:38:40.388615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/certs/global-bundle.pem
--rw-r--r--   0        0        0      947 2023-05-20 10:38:40.388615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/listeners.py
--rw-r--r--   0        0        0     2441 2023-05-20 10:38:40.388615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/model_registry.py
--rw-r--r--   0        0        0      808 2023-05-20 10:38:40.388615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/ssl.py
--rw-r--r--   0        0        0     2585 2023-05-20 10:38:40.388615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/tracking.py
--rw-r--r--   0        0        0      537 2023-05-20 10:38:40.388615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/utils.py
--rw-r--r--   0        0        0     1548 2023-05-20 10:38:40.389615 mlflow_aws_rds_iam-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 mlflow_aws_rds_iam-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-30 23:11:56.508940 mlflow_aws_rds_iam-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     1555 2023-05-30 23:11:56.508940 mlflow_aws_rds_iam-0.2.1/README.md
+-rw-r--r--   0        0        0      227 2023-05-30 23:11:56.508940 mlflow_aws_rds_iam-0.2.1/mlflow_aws_rds_iam/__init__.py
+-rw-r--r--   0        0        0   174184 2023-05-30 23:11:56.509940 mlflow_aws_rds_iam-0.2.1/mlflow_aws_rds_iam/certs/global-bundle.pem
+-rw-r--r--   0        0        0     1078 2023-05-30 23:11:56.509940 mlflow_aws_rds_iam-0.2.1/mlflow_aws_rds_iam/listeners.py
+-rw-r--r--   0        0        0     2322 2023-05-30 23:11:56.509940 mlflow_aws_rds_iam-0.2.1/mlflow_aws_rds_iam/model_registry.py
+-rw-r--r--   0        0        0      983 2023-05-30 23:11:56.509940 mlflow_aws_rds_iam-0.2.1/mlflow_aws_rds_iam/ssl.py
+-rw-r--r--   0        0        0     2460 2023-05-30 23:11:56.509940 mlflow_aws_rds_iam-0.2.1/mlflow_aws_rds_iam/tracking.py
+-rw-r--r--   0        0        0     1050 2023-05-30 23:11:56.509940 mlflow_aws_rds_iam-0.2.1/mlflow_aws_rds_iam/utils.py
+-rw-r--r--   0        0        0     1664 2023-05-30 23:11:56.510940 mlflow_aws_rds_iam-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 mlflow_aws_rds_iam-0.2.1/PKG-INFO
```

### Comparing `mlflow_aws_rds_iam-0.2.0/LICENSE.md` & `mlflow_aws_rds_iam-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlflow_aws_rds_iam-0.2.0/README.md` & `mlflow_aws_rds_iam-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/certs/global-bundle.pem` & `mlflow_aws_rds_iam-0.2.1/mlflow_aws_rds_iam/certs/global-bundle.pem`

 * *Files identical despite different names*

### Comparing `mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/listeners.py` & `mlflow_aws_rds_iam-0.2.1/mlflow_aws_rds_iam/listeners.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""SQLAlchemy Engine event listeners module."""
 import logging
 from typing import Callable
 
 from mypy_boto3_rds.client import RDSClient
 from sqlalchemy import Dialect
 from sqlalchemy.pool import ConnectionPoolEntry
 
@@ -9,14 +10,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 def make_token_provider(
     rds_client: RDSClient,
 ) -> Callable[[Dialect, ConnectionPoolEntry, dict[str, str], dict[str, str]], None]:
+    """Make a SQLAlchemy Engine event listener that injects tokens into conns."""
+
     def provide_token(
         dialect: Dialect,
         conn_rec: ConnectionPoolEntry,
         cargs: dict[str, str],
         cparams: dict[str, str],
     ) -> None:
         logger.debug("Renewing token for '%s'.", cparams["host"])
```

### Comparing `mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/model_registry.py` & `mlflow_aws_rds_iam-0.2.1/mlflow_aws_rds_iam/tracking.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,49 @@
+"""MLflow Tracking plugin module."""
 import logging
 import os
 from urllib.parse import quote_plus
 
 import boto3
-from mlflow.store.model_registry.sqlalchemy_store import SqlAlchemyStore
+from mlflow.store.tracking.sqlalchemy_store import SqlAlchemyStore
 from sqlalchemy import event, make_url
 
 from .listeners import make_token_provider
 from .ssl import IS_SSL_DISABLED_ENV_VAR, set_ssl_params
-from .utils import DatabaseType, get_db_default_port, get_db_type
+from .utils import get_db_default_port
 
 logger = logging.getLogger(__name__)
 
 
 class RDSIAMStore(SqlAlchemyStore):  # type: ignore[misc]
+    """MLflow Tracking SQLAlchemy store with AWS RDS IAM auth support."""
+
     engine = None
 
-    def __init__(self, store_uri: str):
-        logger.debug("Using MLflow RDS IAM auth model registry store plugin.")
+    def __init__(self, store_uri: str, artifact_uri: str):
+        logger.debug("Using MLflow RDS IAM auth tracking store plugin.")
 
         db_uri = make_url(store_uri)
 
-        if not get_db_type(db_uri) in DatabaseType:
-            raise ValueError(
-                "RDS IAM auth plugin for MLflow Model Registry only supports "
-                "Postgresql and MySQL."
-            )
-
         # Use SSL database connection with CA verification unless explicitly disabled
         if not os.getenv(IS_SSL_DISABLED_ENV_VAR, "False").lower() in ("true", "1"):
             db_uri = set_ssl_params(db_uri)
         else:
-            logger.warning("SSL model registry strore database connection is disabled.")
+            logger.warning("SSL tracking store database connection is disabled.")
 
         # Do not use RDS IAM tokens if a password is defined
         if db_uri.password:
-            logger.debug("SSL database connection is disabled.")
-            super().__init__(db_uri.render_as_string(hide_password=False))
+            logger.debug("Using tracking store database password auth.")
+            super().__init__(
+                db_uri.render_as_string(hide_password=False),
+                default_artifact_root=artifact_uri,
+            )
             return
 
-        logger.debug("Using model registry store RDS IAM token auth.")
+        logger.debug("Using tracking store RDS IAM token auth.")
         if not db_uri.host or not db_uri.username:
             raise ValueError(
                 "RDS IAM authentication requires a URI with a host and user."
             )
 
         rds = boto3.client("rds")
 
@@ -54,15 +54,18 @@
                     DBHostname=db_uri.host,
                     Port=db_uri.port or get_db_default_port(db_uri),
                     DBUsername=db_uri.username,
                 )
             )
         )
         logger.debug(
-            "Model registry store bootstrap database URI: %s", db_uri.render_as_string()
+            "Tracking store bootstrap database URI: %s", db_uri.render_as_string()
         )
 
         # Let MLflow's own SqlAlchemyStore initialize the SA engine
-        super().__init__(db_uri.render_as_string(hide_password=False))
+        super().__init__(
+            db_uri.render_as_string(hide_password=False),
+            default_artifact_root=artifact_uri,
+        )
 
         # Add token rotation listener to the engine
         event.listen(self.engine, "do_connect", make_token_provider(rds))
```

### Comparing `mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/tracking.py` & `mlflow_aws_rds_iam-0.2.1/mlflow_aws_rds_iam/model_registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,46 @@
+"""MLflow Model Registry plugin module."""
 import logging
 import os
 from urllib.parse import quote_plus
 
 import boto3
-from mlflow.store.tracking.sqlalchemy_store import SqlAlchemyStore
+from mlflow.store.model_registry.sqlalchemy_store import SqlAlchemyStore
 from sqlalchemy import event, make_url
 
 from .listeners import make_token_provider
 from .ssl import IS_SSL_DISABLED_ENV_VAR, set_ssl_params
-from .utils import DatabaseType, get_db_default_port, get_db_type
+from .utils import get_db_default_port
 
 logger = logging.getLogger(__name__)
 
 
 class RDSIAMStore(SqlAlchemyStore):  # type: ignore[misc]
+    """MLflow Model Registry SQLAlchemy store with AWS RDS IAM auth support."""
+
     engine = None
 
-    def __init__(self, store_uri: str, artifact_uri: str):
-        logger.debug("Using MLflow RDS IAM auth tracking store plugin.")
+    def __init__(self, store_uri: str):
+        logger.debug("Using MLflow RDS IAM auth model registry store plugin.")
 
         db_uri = make_url(store_uri)
 
-        if not get_db_type(db_uri) in DatabaseType:
-            raise ValueError(
-                "RDS IAM auth plugin for MLflow tracking only supports "
-                "Postgresql and MySQL."
-            )
-
         # Use SSL database connection with CA verification unless explicitly disabled
         if not os.getenv(IS_SSL_DISABLED_ENV_VAR, "False").lower() in ("true", "1"):
             db_uri = set_ssl_params(db_uri)
         else:
-            logger.warning("SSL tracking store database connection is disabled.")
+            logger.warning("SSL model registry strore database connection is disabled.")
 
         # Do not use RDS IAM tokens if a password is defined
         if db_uri.password:
-            logger.debug("Using tracking store database password auth.")
-            super().__init__(
-                db_uri.render_as_string(hide_password=False),
-                default_artifact_root=artifact_uri,
-            )
+            logger.debug("SSL database connection is disabled.")
+            super().__init__(db_uri.render_as_string(hide_password=False))
             return
 
-        logger.debug("Using tracking store RDS IAM token auth.")
+        logger.debug("Using model registry store RDS IAM token auth.")
         if not db_uri.host or not db_uri.username:
             raise ValueError(
                 "RDS IAM authentication requires a URI with a host and user."
             )
 
         rds = boto3.client("rds")
 
@@ -57,18 +51,15 @@
                     DBHostname=db_uri.host,
                     Port=db_uri.port or get_db_default_port(db_uri),
                     DBUsername=db_uri.username,
                 )
             )
         )
         logger.debug(
-            "Tracking store bootstrap database URI: %s", db_uri.render_as_string()
+            "Model registry store bootstrap database URI: %s", db_uri.render_as_string()
         )
 
         # Let MLflow's own SqlAlchemyStore initialize the SA engine
-        super().__init__(
-            db_uri.render_as_string(hide_password=False),
-            default_artifact_root=artifact_uri,
-        )
+        super().__init__(db_uri.render_as_string(hide_password=False))
 
         # Add token rotation listener to the engine
         event.listen(self.engine, "do_connect", make_token_provider(rds))
```

### Comparing `mlflow_aws_rds_iam-0.2.0/pyproject.toml` & `mlflow_aws_rds_iam-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlflow-aws-rds-iam"
-version = "0.2.0"
+version = "0.2.1"
 description = "MLflow plugins adding AWS RDS IAM auth for tracking and model registry stores"
 authors = ["Loris Zinsou <lzinsou@protonmail.com>"]
 readme = "README.md"
 keywords = ["mlflow", "plugin", "mlops", "aws", "rds", "iam", "postgresql", "mysql"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Plugins",
@@ -20,28 +20,34 @@
 [tool.poetry.plugins."mlflow.model_registry_store"]
 postgresql = "mlflow_aws_rds_iam.model_registry:RDSIAMStore"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 mlflow = "~2"
 sqlalchemy = "~2"
-boto3 = ">=1.26.134,<2"
+boto3 = ">=1.26,<2"
 StrEnum = { version = ">=0.4", allow-prereleases = true, python = "<3.11" }
-boto3-stubs = {extras = ["rds"], version = ">=1.26.134,<2"}
+boto3-stubs = {extras = ["rds"], version = ">=1.26,<2"}
 
 [tool.poetry.dev-dependencies]
 flake8 = "^6.0.0"
 mypy = "^1.2.0"
 isort = "^5.12.0"
 black = "^23.3.0"
 pytest = "^7.3.1"
 
+[tool.poetry.group.dev.dependencies]
+pytest-cov = "^4.0.0"
+
 [tool.isort]
 profile = "black"
 
+[tool.pytest.ini_options]
+addopts = "--cov=mlflow_aws_rds_iam"
+
 [tool.mypy]
 strict = true
 exclude = "tests"
 
 [[tool.mypy.overrides]]
 module = "mlflow.store.model_registry.sqlalchemy_store"
 ignore_missing_imports = true
```

### Comparing `mlflow_aws_rds_iam-0.2.0/PKG-INFO` & `mlflow_aws_rds_iam-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mlflow-aws-rds-iam
-Version: 0.2.0
+Version: 0.2.1
 Summary: MLflow plugins adding AWS RDS IAM auth for tracking and model registry stores
 Home-page: https://gitlab.com/lzinsou/mlflow-aws-rds-iam
 Keywords: mlflow,plugin,mlops,aws,rds,iam,postgresql,mysql
 Author: Loris Zinsou
 Author-email: lzinsou@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: StrEnum (>=0.4) ; python_version < "3.11"
-Requires-Dist: boto3 (>=1.26.134,<2)
-Requires-Dist: boto3-stubs[rds] (>=1.26.134,<2)
+Requires-Dist: boto3 (>=1.26,<2)
+Requires-Dist: boto3-stubs[rds] (>=1.26,<2)
 Requires-Dist: mlflow (>=2,<3)
 Requires-Dist: sqlalchemy (>=2,<3)
 Project-URL: Repository, https://gitlab.com/lzinsou/mlflow-aws-rds-iam
 Description-Content-Type: text/markdown
 
 MLflow AWS RDS IAM Auth Plugins
 ===============================
```

