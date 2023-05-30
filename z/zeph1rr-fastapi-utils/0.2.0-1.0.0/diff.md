# Comparing `tmp/zeph1rr_fastapi_utils-0.2.0.tar.gz` & `tmp/zeph1rr_fastapi_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeph1rr_fastapi_utils-0.2.0.tar", max compression
+gzip compressed data, was "zeph1rr_fastapi_utils-1.0.0.tar", max compression
```

## Comparing `zeph1rr_fastapi_utils-0.2.0.tar` & `zeph1rr_fastapi_utils-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      527 2023-05-30 22:34:12.518584 zeph1rr_fastapi_utils-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 20:54:40.889819 zeph1rr_fastapi_utils-0.2.0/README.md
--rw-r--r--   0        0        0      158 2023-05-28 20:57:48.425054 zeph1rr_fastapi_utils-0.2.0/zeph1rr_fastapi_utils/__init__.py
--rw-r--r--   0        0        0     1852 2023-05-28 21:03:01.524784 zeph1rr_fastapi_utils-0.2.0/zeph1rr_fastapi_utils/logger.py
--rw-r--r--   0        0        0     2204 2023-05-30 22:34:26.738186 zeph1rr_fastapi_utils-0.2.0/zeph1rr_fastapi_utils/utils.py
--rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 zeph1rr_fastapi_utils-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      527 2023-05-30 22:47:33.985842 zeph1rr_fastapi_utils-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 20:54:40.889819 zeph1rr_fastapi_utils-1.0.0/README.md
+-rw-r--r--   0        0        0      158 2023-05-28 20:57:48.425054 zeph1rr_fastapi_utils-1.0.0/zeph1rr_fastapi_utils/__init__.py
+-rw-r--r--   0        0        0     1852 2023-05-28 21:03:01.524784 zeph1rr_fastapi_utils-1.0.0/zeph1rr_fastapi_utils/logger.py
+-rw-r--r--   0        0        0     2234 2023-05-30 22:47:23.232714 zeph1rr_fastapi_utils-1.0.0/zeph1rr_fastapi_utils/utils.py
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 zeph1rr_fastapi_utils-1.0.0/PKG-INFO
```

### Comparing `zeph1rr_fastapi_utils-0.2.0/pyproject.toml` & `zeph1rr_fastapi_utils-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeph1rr-fastapi-utils"
-version = "0.2.0"
+version = "1.0.0"
 description = "Package for unificate functions in fastapi"
 authors = ["Zeph1rr <grianton535@gmail.com>"]
 readme = "README.md"
 packages = [{include = "zeph1rr_fastapi_utils"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `zeph1rr_fastapi_utils-0.2.0/zeph1rr_fastapi_utils/logger.py` & `zeph1rr_fastapi_utils-1.0.0/zeph1rr_fastapi_utils/logger.py`

 * *Files identical despite different names*

### Comparing `zeph1rr_fastapi_utils-0.2.0/zeph1rr_fastapi_utils/utils.py` & `zeph1rr_fastapi_utils-1.0.0/zeph1rr_fastapi_utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,18 +52,18 @@
         to_encode.update({"exp": expire})
         encoded_jwt = jwt.encode(
             to_encode, self.jwt_secret, algorithm="HS256"
         )
         return encoded_jwt
 
 
-def _get_project_meta():
+def get_project_meta(project_path: str = pathlib.Path(__name__).parent.parent.parent):
     pyproject_path = pathlib.Path(
-        pathlib.Path(__file__).parent.parent.parent, "pyproject.toml"
+        project_path, "pyproject.toml"
     )
     with open(pyproject_path, mode="rb") as pyproject:
         return tomli.load(pyproject)["tool"]["poetry"]
 
 
 def get_project_data() -> tuple:
-    project_meta = _get_project_meta()
+    project_meta = get_project_meta()
     return project_meta["name"], project_meta["version"]
```

### Comparing `zeph1rr_fastapi_utils-0.2.0/PKG-INFO` & `zeph1rr_fastapi_utils-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeph1rr-fastapi-utils
-Version: 0.2.0
+Version: 1.0.0
 Summary: Package for unificate functions in fastapi
 Author: Zeph1rr
 Author-email: grianton535@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
```

