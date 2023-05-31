# Comparing `tmp/embedbase-1.2.5.tar.gz` & `tmp/embedbase-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.2.5.tar", max compression
+gzip compressed data, was "embedbase-1.2.6.tar", max compression
```

## Comparing `embedbase-1.2.5.tar` & `embedbase-1.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-30 12:49:44.775864 embedbase-1.2.5/LICENSE
--rw-r--r--   0        0        0     4931 2023-05-30 12:49:44.775864 embedbase-1.2.5/README.md
--rw-r--r--   0        0        0      121 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/__main__.py
--rw-r--r--   0        0        0      416 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/api.py
--rw-r--r--   0        0        0    21232 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3920 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/database/base.py
--rw-r--r--   0        0        0     6962 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/database/memory_db.py
--rw-r--r--   0        0        0    11071 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     9430 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/logging_utils.py
--rw-r--r--   0        0        0     1313 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/models.py
--rw-r--r--   0        0        0     1245 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/utils.py
--rw-r--r--   0        0        0     3730 2023-05-30 12:49:44.915866 embedbase-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 embedbase-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-31 07:36:24.872705 embedbase-1.2.6/LICENSE
+-rw-r--r--   0        0        0     4931 2023-05-31 07:36:24.872705 embedbase-1.2.6/README.md
+-rw-r--r--   0        0        0      121 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/__main__.py
+-rw-r--r--   0        0        0      416 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/api.py
+-rw-r--r--   0        0        0    21232 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3920 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/database/base.py
+-rw-r--r--   0        0        0     6962 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0    11071 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     9883 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/logging_utils.py
+-rw-r--r--   0        0        0     1459 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/models.py
+-rw-r--r--   0        0        0     1245 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-31 07:36:25.008709 embedbase-1.2.6/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-31 07:36:25.012709 embedbase-1.2.6/embedbase/utils.py
+-rw-r--r--   0        0        0     3730 2023-05-31 07:36:25.012709 embedbase-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 embedbase-1.2.6/PKG-INFO
```

### Comparing `embedbase-1.2.5/LICENSE` & `embedbase-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/README.md` & `embedbase-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/__main__.py` & `embedbase-1.2.6/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/app.py` & `embedbase-1.2.6/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/database/base.py` & `embedbase-1.2.6/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/database/memory_db.py` & `embedbase-1.2.6/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/database/postgres_db.py` & `embedbase-1.2.6/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/database/supabase_db.py` & `embedbase-1.2.6/embedbase/database/supabase_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 import asyncio
 import itertools
 
 import pandas as pd
 from pandas import DataFrame, Series
 
 from embedbase.database import VectorDatabase
-from embedbase.database.base import Dataset, SearchResponse, SelectResponse, WhereResponse
+from embedbase.database.base import (
+    Dataset,
+    SearchResponse,
+    SelectResponse,
+    WhereResponse,
+)
 from embedbase.models import Document
 from embedbase.utils import BatchGenerator
 
 
 class Supabase(VectorDatabase):
     """
     Implements a vector database using supabase
@@ -102,14 +107,28 @@
         user_id: Optional[str] = None,
         batch_size: Optional[int] = 100,
         store_data: bool = True,
     ):
         df_batcher = BatchGenerator(batch_size)
         batches = [batch_df for batch_df in df_batcher(df)]
 
+        # create dataset in datasets table if not exist
+
+        q = self.supabase.table("datasets").select("*").eq("name", dataset_id)
+        if user_id:
+            q = q.eq("owner", user_id)
+        data = q.execute().data
+        if not data:
+            self.supabase.table("datasets").insert(
+                {
+                    "name": dataset_id,
+                    "owner": user_id,
+                }
+            ).execute()
+
         async def _insert(batch_df: DataFrame):
             def _d(row: Series):
                 data = {
                     "id": row.id,
                     "embedding": row.embedding,
                     "hash": row.hash,
                     "dataset_id": dataset_id,
@@ -185,46 +204,46 @@
 
     async def clear(self, dataset_id: str, user_id: Optional[str] = None):
         req = self.supabase.table("documents").delete().eq("dataset_id", dataset_id)
         if user_id:
             req = req.eq("user_id", user_id)
         req.execute()
 
-    async def get_datasets(self, user_id: Optional[str] = None):
-        req = self.supabase.table("distinct_datasets").select(
-            "dataset_id", "documents_count"
-        )
-        if user_id:
-            req = req.eq("user_id", user_id)
-        data = req.execute().data
-        return [
-            Dataset(
-                dataset_id=row["dataset_id"],
-                documents_count=row["documents_count"],
-            )
-            for row in data
-        ]
-    
-    # TODO: above old, below new, temporary hack
     # async def get_datasets(self, user_id: Optional[str] = None):
-    #     req = self.supabase.table("datasets").select(
-    #         "name", "documents_count", "created_at"
+    #     req = self.supabase.table("distinct_datasets").select(
+    #         "dataset_id", "documents_count"
     #     )
     #     if user_id:
-    #         req = req.eq("owner", user_id)
+    #         req = req.eq("user_id", user_id)
     #     data = req.execute().data
     #     return [
     #         Dataset(
-    #             dataset_id=row["name"],
+    #             dataset_id=row["dataset_id"],
     #             documents_count=row["documents_count"],
-    #             created_at=row["created_at"],
     #         )
     #         for row in data
     #     ]
 
+    # TODO: above old, below new, temporary hack
+    async def get_datasets(self, user_id: Optional[str] = None):
+        req = self.supabase.table("datasets").select(
+            "name", "documents_count", "created_at"
+        )
+        if user_id:
+            req = req.eq("owner", user_id)
+        data = req.execute().data
+        return [
+            Dataset(
+                dataset_id=row["name"],
+                documents_count=row["documents_count"],
+                created_at=row["created_at"],
+            )
+            for row in data
+        ]
+
     async def list(
         self,
         dataset_id: str,
         user_id: Optional[str] = None,
         offset: int = 0,
         limit: int = 100,
     ) -> List[Document]:
@@ -241,15 +260,14 @@
                 hash=row["hash"],
                 metadata=row["metadata"],
                 dataset_ids=[row["dataset_id"]],
             )
             for row in data
         ]
 
-
     async def where(
         self,
         dataset_id: Optional[str] = None,
         user_id: Optional[str] = None,
         where: Optional[Union[dict, List[dict]]] = None,
     ) -> List[WhereResponse]:
         """
```

### Comparing `embedbase-1.2.5/embedbase/embedding/base.py` & `embedbase-1.2.6/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/embedding/cohere.py` & `embedbase-1.2.6/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/embedding/openai.py` & `embedbase-1.2.6/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/firebase_auth.py` & `embedbase-1.2.6/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/logging_utils.py` & `embedbase-1.2.6/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/models.py` & `embedbase-1.2.6/embedbase/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -44,18 +44,20 @@
 class DeleteRequest(BaseModel):
     ids: List[str]
 
 
 class SearchRequest(BaseModel):
     query: str
     top_k: int = 6
+    # todo add validation on metdata (create Metdata class as in sdk-py)
     where: Optional[Union[dict, List[dict]]] = None
 
 
 class ReplaceDocument(BaseModel):
     data: str = None
     metadata: Optional[dict] = None
 
 
 class ReplaceRequest(BaseModel):
     documents: List[ReplaceDocument]
+    # todo add validation on metdata (create Metdata class as in sdk-py)
     where: Optional[Union[dict, List[dict]]] = None
```

### Comparing `embedbase-1.2.5/embedbase/settings.py` & `embedbase-1.2.6/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/strings.py` & `embedbase-1.2.6/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/embedbase/utils.py` & `embedbase-1.2.6/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.5/pyproject.toml` & `embedbase-1.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "embedbase"
-version = "1.2.5"
+version = "1.2.6"
 description = "Open-source API & SDK to integrate your data and easily hook them up to LLMs."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence", "llm"]
```

### Comparing `embedbase-1.2.5/PKG-INFO` & `embedbase-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.2.5
+Version: 1.2.6
 Summary: Open-source API & SDK to integrate your data and easily hook them up to LLMs.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

