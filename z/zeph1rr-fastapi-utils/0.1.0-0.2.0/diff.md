# Comparing `tmp/zeph1rr_fastapi_utils-0.1.0.tar.gz` & `tmp/zeph1rr_fastapi_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeph1rr_fastapi_utils-0.1.0.tar", max compression
+gzip compressed data, was "zeph1rr_fastapi_utils-0.2.0.tar", max compression
```

## Comparing `zeph1rr_fastapi_utils-0.1.0.tar` & `zeph1rr_fastapi_utils-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      509 2023-05-28 20:58:04.887803 zeph1rr_fastapi_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 20:54:40.889819 zeph1rr_fastapi_utils-0.1.0/README.md
--rw-r--r--   0        0        0      158 2023-05-28 20:57:48.425054 zeph1rr_fastapi_utils-0.1.0/zeph1rr_fastapi_utils/__init__.py
--rw-r--r--   0        0        0     1852 2023-05-28 21:03:01.524784 zeph1rr_fastapi_utils-0.1.0/zeph1rr_fastapi_utils/logger.py
--rw-r--r--   0        0        0     1784 2023-05-28 21:02:48.731880 zeph1rr_fastapi_utils-0.1.0/zeph1rr_fastapi_utils/utils.py
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 zeph1rr_fastapi_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      527 2023-05-30 22:34:12.518584 zeph1rr_fastapi_utils-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 20:54:40.889819 zeph1rr_fastapi_utils-0.2.0/README.md
+-rw-r--r--   0        0        0      158 2023-05-28 20:57:48.425054 zeph1rr_fastapi_utils-0.2.0/zeph1rr_fastapi_utils/__init__.py
+-rw-r--r--   0        0        0     1852 2023-05-28 21:03:01.524784 zeph1rr_fastapi_utils-0.2.0/zeph1rr_fastapi_utils/logger.py
+-rw-r--r--   0        0        0     2204 2023-05-30 22:34:26.738186 zeph1rr_fastapi_utils-0.2.0/zeph1rr_fastapi_utils/utils.py
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 zeph1rr_fastapi_utils-0.2.0/PKG-INFO
```

### Comparing `zeph1rr_fastapi_utils-0.1.0/zeph1rr_fastapi_utils/logger.py` & `zeph1rr_fastapi_utils-0.2.0/zeph1rr_fastapi_utils/logger.py`

 * *Files identical despite different names*

### Comparing `zeph1rr_fastapi_utils-0.1.0/zeph1rr_fastapi_utils/utils.py` & `zeph1rr_fastapi_utils-0.2.0/zeph1rr_fastapi_utils/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import json
+import pathlib
+import tomli
 from uuid import UUID
 from datetime import datetime
 from datetime import timedelta
 
 from jose import jwt
 from passlib.context import CryptContext
 from fastapi import HTTPException
@@ -48,7 +50,20 @@
         to_encode = data.copy()
         expire = datetime.utcnow() + self.expire
         to_encode.update({"exp": expire})
         encoded_jwt = jwt.encode(
             to_encode, self.jwt_secret, algorithm="HS256"
         )
         return encoded_jwt
+
+
+def _get_project_meta():
+    pyproject_path = pathlib.Path(
+        pathlib.Path(__file__).parent.parent.parent, "pyproject.toml"
+    )
+    with open(pyproject_path, mode="rb") as pyproject:
+        return tomli.load(pyproject)["tool"]["poetry"]
+
+
+def get_project_data() -> tuple:
+    project_meta = _get_project_meta()
+    return project_meta["name"], project_meta["version"]
```

### Comparing `zeph1rr_fastapi_utils-0.1.0/PKG-INFO` & `zeph1rr_fastapi_utils-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: zeph1rr-fastapi-utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: Package for unificate functions in fastapi
 Author: Zeph1rr
 Author-email: grianton535@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
 Requires-Dist: fastapi (>=0.95.2,<0.96.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
```

