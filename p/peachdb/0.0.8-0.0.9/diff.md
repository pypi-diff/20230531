# Comparing `tmp/peachdb-0.0.8.tar.gz` & `tmp/peachdb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peachdb-0.0.8.tar", last modified: Tue May 30 17:00:39 2023, max compression
+gzip compressed data, was "peachdb-0.0.9.tar", last modified: Tue May 30 17:36:35 2023, max compression
```

## Comparing `peachdb-0.0.8.tar` & `peachdb-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2023-05-29 20:30:02.000000 peachdb-0.0.8/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       25 2023-05-30 16:35:10.000000 peachdb-0.0.8/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 17:00:39.543553 peachdb-0.0.8/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6051 2023-05-30 16:38:49.000000 peachdb-0.0.8/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/peachdb/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7855 2023-05-30 10:56:06.000000 peachdb-0.0.8/peachdb/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/peachdb/backends/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      923 2023-05-29 16:37:03.000000 peachdb-0.0.8/peachdb/backends/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3161 2023-05-30 10:57:00.000000 peachdb-0.0.8/peachdb/backends/backend_base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2056 2023-05-30 11:29:19.000000 peachdb-0.0.8/peachdb/backends/hnsw_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2669 2023-05-29 16:37:03.000000 peachdb-0.0.8/peachdb/backends/numpy_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3894 2023-05-29 20:30:02.000000 peachdb-0.0.8/peachdb/backends/torch_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      223 2023-05-29 16:37:03.000000 peachdb-0.0.8/peachdb/constants.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/peachdb/embedder/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4936 2023-05-30 11:00:29.000000 peachdb-0.0.8/peachdb/embedder/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/peachdb/embedder/containers/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:50:04.000000 peachdb-0.0.8/peachdb/embedder/containers/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1671 2023-05-29 20:30:02.000000 peachdb-0.0.8/peachdb/embedder/containers/base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1568 2023-05-29 20:32:06.000000 peachdb-0.0.8/peachdb/embedder/containers/sentence_transformer.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/peachdb/embedder/models/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:49:59.000000 peachdb-0.0.8/peachdb/embedder/models/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      288 2023-05-26 16:27:29.000000 peachdb-0.0.8/peachdb/embedder/models/base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      598 2023-05-29 10:12:31.000000 peachdb-0.0.8/peachdb/embedder/models/sentence_transformer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2718 2023-05-30 10:47:11.000000 peachdb-0.0.8/peachdb/embedder/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/peachdb.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 17:00:39.000000 peachdb-0.0.8/peachdb.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      727 2023-05-30 17:00:39.000000 peachdb-0.0.8/peachdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-05-30 17:00:39.000000 peachdb-0.0.8/peachdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      138 2023-05-30 17:00:39.000000 peachdb-0.0.8/peachdb.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-30 17:00:39.000000 peachdb-0.0.8/peachdb.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       64 2023-05-30 16:30:14.000000 peachdb-0.0.8/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      138 2023-05-30 16:44:43.000000 peachdb-0.0.8/requirements.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-30 17:00:39.543553 peachdb-0.0.8/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      852 2023-05-30 17:00:09.000000 peachdb-0.0.8/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2023-05-29 20:30:02.000000 peachdb-0.0.9/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       25 2023-05-30 16:35:10.000000 peachdb-0.0.9/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 17:36:35.331771 peachdb-0.0.9/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6051 2023-05-30 16:38:49.000000 peachdb-0.0.9/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/peachdb/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7855 2023-05-30 10:56:06.000000 peachdb-0.0.9/peachdb/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/peachdb/backends/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      923 2023-05-29 16:37:03.000000 peachdb-0.0.9/peachdb/backends/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3161 2023-05-30 10:57:00.000000 peachdb-0.0.9/peachdb/backends/backend_base.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2056 2023-05-30 11:29:19.000000 peachdb-0.0.9/peachdb/backends/hnsw_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2669 2023-05-29 16:37:03.000000 peachdb-0.0.9/peachdb/backends/numpy_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3894 2023-05-29 20:30:02.000000 peachdb-0.0.9/peachdb/backends/torch_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      388 2023-05-30 17:33:07.000000 peachdb-0.0.9/peachdb/constants.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/peachdb/embedder/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4936 2023-05-30 11:00:29.000000 peachdb-0.0.9/peachdb/embedder/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/peachdb/embedder/containers/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:50:04.000000 peachdb-0.0.9/peachdb/embedder/containers/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2169 2023-05-30 17:33:37.000000 peachdb-0.0.9/peachdb/embedder/containers/base.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1568 2023-05-29 20:32:06.000000 peachdb-0.0.9/peachdb/embedder/containers/sentence_transformer.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/peachdb/embedder/models/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:49:59.000000 peachdb-0.0.9/peachdb/embedder/models/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      288 2023-05-26 16:27:29.000000 peachdb-0.0.9/peachdb/embedder/models/base.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      598 2023-05-29 10:12:31.000000 peachdb-0.0.9/peachdb/embedder/models/sentence_transformer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2718 2023-05-30 10:47:11.000000 peachdb-0.0.9/peachdb/embedder/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/peachdb.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 17:36:35.000000 peachdb-0.0.9/peachdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      727 2023-05-30 17:36:35.000000 peachdb-0.0.9/peachdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-05-30 17:36:35.000000 peachdb-0.0.9/peachdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      151 2023-05-30 17:36:35.000000 peachdb-0.0.9/peachdb.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-30 17:36:35.000000 peachdb-0.0.9/peachdb.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       64 2023-05-30 16:30:14.000000 peachdb-0.0.9/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      151 2023-05-30 17:08:02.000000 peachdb-0.0.9/requirements.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-30 17:36:35.331771 peachdb-0.0.9/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      852 2023-05-30 17:17:02.000000 peachdb-0.0.9/setup.py
```

### Comparing `peachdb-0.0.8/LICENSE` & `peachdb-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/PKG-INFO` & `peachdb-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peachdb
-Version: 0.0.8
+Version: 0.0.9
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/peach-db/peachdb
 Project-URL: Documentation, https://github.com/peach-db/peachdb/blob/master/README.md
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `peachdb-0.0.8/README.md` & `peachdb-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/peachdb/__init__.py` & `peachdb-0.0.9/peachdb/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/peachdb/backends/__init__.py` & `peachdb-0.0.9/peachdb/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/peachdb/backends/backend_base.py` & `peachdb-0.0.9/peachdb/backends/backend_base.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/peachdb/backends/hnsw_backend.py` & `peachdb-0.0.9/peachdb/backends/hnsw_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/peachdb/backends/numpy_backend.py` & `peachdb-0.0.9/peachdb/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/peachdb/backends/torch_backend.py` & `peachdb-0.0.9/peachdb/backends/torch_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/peachdb/embedder/__init__.py` & `peachdb-0.0.9/peachdb/embedder/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/peachdb/embedder/containers/base.py` & `peachdb-0.0.9/peachdb/embedder/containers/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,46 @@
 import os
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Optional
 
 import modal
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
+import requests
 
+from peachdb.constants import CACHED_REQUIREMENTS_TXT, GIT_REQUIREMENTS_TXT
 from peachdb.embedder.utils import is_s3_uri
 
+# Logic to get a requirements.txt file for the base image when package is on PyPI.
+dev_requirements_path = Path(__file__).parents[3] / "requirements.txt"
+if os.path.exists(dev_requirements_path):
+    requirements_path = dev_requirements_path
+else:
+    response = requests.get(GIT_REQUIREMENTS_TXT)
+
+    response.raise_for_status()
+
+    with open(CACHED_REQUIREMENTS_TXT, "w") as f:
+        f.write(response.text)
+
+    requirements_path = CACHED_REQUIREMENTS_TXT
+
 # Requirements for the base image of models we want to serve.
 # We don't add the requirements.txt here as that contains requirements across ALL our models.
 base_container_image = (
     modal.Image.debian_slim()
     .apt_install("curl", "zip", "git")
     .run_commands(
         "curl https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip -o awscliv2.zip",
         "unzip awscliv2.zip",
         "./aws/install",
         "rm -rf awscliv2.zip aws",
     )
-    .pip_install_from_requirements(Path(__file__).parents[3] / "requirements.txt")
+    .pip_install_from_requirements(requirements_path)
 )
 
 modal_compute_spec_decorator = lambda stub, image: stub.cls(
     image=image,
     gpu="T4",
     timeout=400,
     secret=modal.Secret.from_dotenv(Path(__file__).parents[3] / ".env"),
```

### Comparing `peachdb-0.0.8/peachdb/embedder/containers/sentence_transformer.py` & `peachdb-0.0.9/peachdb/embedder/containers/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/peachdb/embedder/models/sentence_transformer.py` & `peachdb-0.0.9/peachdb/embedder/models/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/peachdb/embedder/utils.py` & `peachdb-0.0.9/peachdb/embedder/utils.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/peachdb.egg-info/PKG-INFO` & `peachdb-0.0.9/peachdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peachdb
-Version: 0.0.8
+Version: 0.0.9
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/peach-db/peachdb
 Project-URL: Documentation, https://github.com/peach-db/peachdb/blob/master/README.md
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `peachdb-0.0.8/peachdb.egg-info/SOURCES.txt` & `peachdb-0.0.9/peachdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.8/setup.py` & `peachdb-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # read the contents README
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="peachdb",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     install_requires=requirements,
     dependency_links=["https://download.pytorch.org/whl/cu113"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     project_urls={
```

