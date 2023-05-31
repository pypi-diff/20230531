# Comparing `tmp/fgo_api_types-2023.5.31.14.13.56.tar.gz` & `tmp/fgo_api_types-2023.5.31.14.20.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.5.31.14.13.56.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.5.31.14.20.7.tar", max compression
```

## Comparing `fgo_api_types-2023.5.31.14.13.56.tar` & `fgo_api_types-2023.5.31.14.20.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-05-31 14:13:34.878216 fgo_api_types-2023.5.31.14.13.56/LICENSE
--rw-r--r--   0        0        0      449 2023-05-31 14:13:34.878216 fgo_api_types-2023.5.31.14.13.56/README.md
--rw-r--r--   0        0        0        0 2023-05-31 14:13:56.230111 fgo_api_types-2023.5.31.14.13.56/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-05-31 14:13:56.230111 fgo_api_types-2023.5.31.14.13.56/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-05-31 14:13:56.230111 fgo_api_types-2023.5.31.14.13.56/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-05-31 14:13:56.230111 fgo_api_types-2023.5.31.14.13.56/fgo_api_types/common.py
--rw-r--r--   0        0        0    38038 2023-05-31 14:13:56.230111 fgo_api_types-2023.5.31.14.13.56/fgo_api_types/enums.py
--rw-r--r--   0        0        0   157892 2023-05-31 14:13:56.230111 fgo_api_types-2023.5.31.14.13.56/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    75728 2023-05-31 14:13:56.234111 fgo_api_types-2023.5.31.14.13.56/fgo_api_types/nice.py
--rw-r--r--   0        0        0    50619 2023-05-31 14:13:56.234111 fgo_api_types-2023.5.31.14.13.56/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-05-31 14:13:56.234111 fgo_api_types-2023.5.31.14.13.56/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18670 2023-05-31 14:13:56.234111 fgo_api_types-2023.5.31.14.13.56/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-05-31 14:13:56.558110 fgo_api_types-2023.5.31.14.13.56/pyproject.toml
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 fgo_api_types-2023.5.31.14.13.56/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-31 14:19:45.134564 fgo_api_types-2023.5.31.14.20.7/LICENSE
+-rw-r--r--   0        0        0      449 2023-05-31 14:19:45.134564 fgo_api_types-2023.5.31.14.20.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/common.py
+-rw-r--r--   0        0        0    38038 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   157892 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    75688 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    50619 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18670 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-05-31 14:20:07.631875 fgo_api_types-2023.5.31.14.20.7/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.5.31.14.20.7/PKG-INFO
```

### Comparing `fgo_api_types-2023.5.31.14.13.56/LICENSE` & `fgo_api_types-2023.5.31.14.20.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.13.56/fgo_api_types/basic.py` & `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.13.56/fgo_api_types/common.py` & `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.13.56/fgo_api_types/enums.py` & `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.13.56/fgo_api_types/gameenums.py` & `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.13.56/fgo_api_types/nice.py` & `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -2318,15 +2318,14 @@
 class NiceQuestPhaseExtraDetail(BaseModelORJson):
     questSelect: list[int] | None = None
     singleForceSvtId: int | None = None
     hintTitle: str | None = None
     hintMessage: str | None = None
     aiNpc: NiceQuestPhaseAiNpc | None = None
     aiMultiNpc: list[NiceQuestPhaseAiNpc] | None = None
-    singleForceSvtId: int | None = None
     overwriteEquipSkills: dict | None = None
 
 
 class NiceRestriction(BaseModelORJson):
     id: int
     name: str
     type: NiceRestrictionType
```

### Comparing `fgo_api_types-2023.5.31.14.13.56/fgo_api_types/raw.py` & `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.13.56/fgo_api_types/rayshift.py` & `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.13.56/fgo_api_types/search.py` & `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.13.56/pyproject.toml` & `fgo_api_types-2023.5.31.14.20.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.05.31.14.13.56"
+version = "2023.05.31.14.20.07"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.5.31.14.13.56/PKG-INFO` & `fgo_api_types-2023.5.31.14.20.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.5.31.14.13.56
+Version: 2023.5.31.14.20.7
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

