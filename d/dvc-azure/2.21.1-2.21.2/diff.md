# Comparing `tmp/dvc-azure-2.21.1.tar.gz` & `tmp/dvc-azure-2.21.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-azure-2.21.1.tar", last modified: Wed Feb  8 06:32:35 2023, max compression
+gzip compressed data, was "dvc-azure-2.21.2.tar", last modified: Wed May 31 11:02:45 2023, max compression
```

## Comparing `dvc-azure-2.21.1.tar` & `dvc-azure-2.21.2.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-08 06:32:35.184015 dvc-azure-2.21.1/
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-08 06:32:35.180015 dvc-azure-2.21.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-08 06:32:35.184015 dvc-azure-2.21.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1833 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-02-08 06:32:35.184015 dvc-azure-2.21.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-08 06:32:35.184015 dvc-azure-2.21.1/dvc_azure/
--rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/dvc_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-02-08 06:32:35.000000 dvc-azure-2.21.1/dvc_azure/_dvc_azure_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/dvc_azure/path.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/dvc_azure/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-08 06:32:35.184015 dvc-azure-2.21.1/dvc_azure/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/dvc_azure/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/dvc_azure/tests/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/dvc_azure/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/dvc_azure/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/dvc_azure/tests/test_dvc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-08 06:32:35.184015 dvc-azure-2.21.1/dvc_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-02-08 06:32:35.000000 dvc-azure-2.21.1/dvc_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-02-08 06:32:35.000000 dvc-azure-2.21.1/dvc_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-08 06:32:35.000000 dvc-azure-2.21.1/dvc_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-08 06:32:35.000000 dvc-azure-2.21.1/dvc_azure.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-02-08 06:32:35.000000 dvc-azure-2.21.1/dvc_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-02-08 06:32:35.000000 dvc-azure-2.21.1/dvc_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-02-08 06:32:35.184015 dvc-azure-2.21.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-08 06:32:18.000000 dvc-azure-2.21.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:45.939277 dvc-azure-2.21.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:45.935277 dvc-azure-2.21.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:45.935277 dvc-azure-2.21.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1833 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-05-31 11:02:45.939277 dvc-azure-2.21.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:45.935277 dvc-azure-2.21.2/dvc_azure/
+-rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure/_dvc_azure_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:45.935277 dvc-azure-2.21.2/dvc_azure/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/tests/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/tests/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/tests/test_dvc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:45.935277 dvc-azure-2.21.2/dvc_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-05-31 11:02:45.939277 dvc-azure-2.21.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/setup.py
```

### Comparing `dvc-azure-2.21.1/.github/workflows/release.yaml` & `dvc-azure-2.21.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.1/.github/workflows/tests.yaml` & `dvc-azure-2.21.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.1/.github/workflows/update-template.yaml` & `dvc-azure-2.21.2/.github/workflows/update-template.yaml`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.1/.gitignore` & `dvc-azure-2.21.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.1/.pre-commit-config.yaml` & `dvc-azure-2.21.2/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
           - ba,datas,fo,uptodate
     repo: https://github.com/codespell-project/codespell
     rev: v2.1.0
   - hooks:
       - id: isort
         language_version: python3
     repo: https://github.com/timothycrosley/isort
-    rev: 5.9.3
+    rev: 5.12.0
   - hooks:
       - id: flake8
         language_version: python3
         additional_dependencies:
           - flake8-bugbear
           - flake8-comprehensions
           - flake8-debugger
```

### Comparing `dvc-azure-2.21.1/LICENSE` & `dvc-azure-2.21.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.1/PKG-INFO` & `dvc-azure-2.21.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-azure
-Version: 2.21.1
+Version: 2.21.2
 Summary: azure plugin for dvc
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc-azure
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-azure
 Keywords: dvc,azure
```

### Comparing `dvc-azure-2.21.1/dvc_azure/__init__.py` & `dvc-azure-2.21.2/dvc_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.1/dvc_azure/path.py` & `dvc-azure-2.21.2/dvc_azure/path.py`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.1/dvc_azure/tests/cloud.py` & `dvc-azure-2.21.2/dvc_azure/tests/cloud.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+import uuid
+
 from dvc.testing.cloud import Cloud
 from dvc.testing.path_info import CloudURLInfo
 from funcy import cached_property
 
 
 class Azure(Cloud, CloudURLInfo):
 
@@ -62,7 +65,13 @@
 
     def exists(self):
         raise NotImplementedError
 
     @property
     def config(self):
         return {"url": self.url, **self.opts}
+
+    @staticmethod
+    def get_storagepath():
+        path = os.environ.get("DVC_TEST_AZURE_PATH")
+        assert path
+        return path + "/" + "dvc_test_caches" + "/" + str(uuid.uuid4())
```

### Comparing `dvc-azure-2.21.1/dvc_azure/tests/test_dvc.py` & `dvc-azure-2.21.2/dvc_azure/tests/test_dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.1/dvc_azure.egg-info/PKG-INFO` & `dvc-azure-2.21.2/dvc_azure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-azure
-Version: 2.21.1
+Version: 2.21.2
 Summary: azure plugin for dvc
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc-azure
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-azure
 Keywords: dvc,azure
```

### Comparing `dvc-azure-2.21.1/dvc_azure.egg-info/SOURCES.txt` & `dvc-azure-2.21.2/dvc_azure.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
+.github/workflows/benchmarks.yaml
 .github/workflows/release.yaml
 .github/workflows/tests.yaml
 .github/workflows/update-template.yaml
 dvc_azure/__init__.py
 dvc_azure/_dvc_azure_version.py
 dvc_azure/path.py
 dvc_azure/spec.py
 dvc_azure.egg-info/PKG-INFO
 dvc_azure.egg-info/SOURCES.txt
 dvc_azure.egg-info/dependency_links.txt
 dvc_azure.egg-info/not-zip-safe
 dvc_azure.egg-info/requires.txt
 dvc_azure.egg-info/top_level.txt
 dvc_azure/tests/__init__.py
+dvc_azure/tests/benchmarks.py
 dvc_azure/tests/cloud.py
 dvc_azure/tests/conftest.py
 dvc_azure/tests/fixtures.py
 dvc_azure/tests/test_dvc.py
```

### Comparing `dvc-azure-2.21.1/dvc_azure.egg-info/requires.txt` & `dvc-azure-2.21.2/dvc_azure.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 dvc
-adlfs>=2022.9.0
+adlfs>=2023.4.0
 azure-identity>=1.4.0
 knack
 
 [tests]
 wheel==0.37.0
 dvc[testing]
 pytest==7.2.0
 pytest-cov==3.0.0
 pytest-xdist==2.4.0
 pytest-mock==3.6.1
 pytest-lazy-fixture==0.6.3
 pytest-test-utils==0.0.8
-pytest-servers[azure]==0.1.4
+pytest-servers[azure]==0.2.2
 flaky==3.7.0
 mock==4.0.3
 wget==3.2
 filelock==3.3.2
 crc32c==2.3.post0
 xmltodict==0.12.0
 Pygments==2.10.0
```

### Comparing `dvc-azure-2.21.1/pyproject.toml` & `dvc-azure-2.21.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.1/setup.cfg` & `dvc-azure-2.21.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -25,29 +25,29 @@
 	setuptools_scm[toml]>=6.3.1
 python_requires = >=3.8
 zip_safe = False
 packages = find:
 include_package_data = True
 install_requires = 
 	dvc
-	adlfs>=2022.9.0
+	adlfs>=2023.4.0
 	azure-identity>=1.4.0
 	knack
 
 [options.extras_require]
 tests = 
 	wheel==0.37.0
 	dvc[testing]
 	pytest==7.2.0
 	pytest-cov==3.0.0
 	pytest-xdist==2.4.0
 	pytest-mock==3.6.1
 	pytest-lazy-fixture==0.6.3
 	pytest-test-utils==0.0.8
-	pytest-servers[azure]==0.1.4
+	pytest-servers[azure]==0.2.2
 	flaky==3.7.0
 	mock==4.0.3
 	wget==3.2
 	filelock==3.3.2
 	crc32c==2.3.post0
 	xmltodict==0.12.0
 	Pygments==2.10.0
```

