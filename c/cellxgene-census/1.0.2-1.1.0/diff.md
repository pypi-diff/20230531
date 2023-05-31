# Comparing `tmp/cellxgene_census-1.0.2.tar.gz` & `tmp/cellxgene_census-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_census-1.0.2.tar", last modified: Tue May 23 01:31:00 2023, max compression
+gzip compressed data, was "cellxgene_census-1.1.0.tar", last modified: Wed May 31 14:56:32 2023, max compression
```

## Comparing `cellxgene_census-1.0.2.tar` & `cellxgene_census-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:31:00.621107 cellxgene_census-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-23 01:31:00.621107 cellxgene_census-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/release_process.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:31:00.613107 cellxgene_census-1.0.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:31:00.621107 cellxgene_census-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:31:00.613107 cellxgene_census-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:31:00.617107 cellxgene_census-1.0.2/src/cellxgene_census/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/_presence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/_release_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:31:00.617107 cellxgene_census-1.0.2/src/cellxgene_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-23 01:31:00.000000 cellxgene_census-1.0.2/src/cellxgene_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-23 01:31:00.000000 cellxgene_census-1.0.2/src/cellxgene_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:31:00.000000 cellxgene_census-1.0.2/src/cellxgene_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 01:31:00.000000 cellxgene_census-1.0.2/src/cellxgene_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 01:31:00.000000 cellxgene_census-1.0.2/src/cellxgene_census.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:31:00.621107 cellxgene_census-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25092 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/test_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/test_get_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/release_process.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.612868 cellxgene_census-1.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.612868 cellxgene_census-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.612868 cellxgene_census-1.1.0/src/cellxgene_census/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/_presence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/_release_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/src/cellxgene_census/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/src/cellxgene_census/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/experimental/ml/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/src/cellxgene_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 14:56:32.000000 cellxgene_census-1.1.0/src/cellxgene_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-31 14:56:32.000000 cellxgene_census-1.1.0/src/cellxgene_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:56:32.000000 cellxgene_census-1.1.0/src/cellxgene_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 14:56:32.000000 cellxgene_census-1.1.0/src/cellxgene_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 14:56:32.000000 cellxgene_census-1.1.0/src/cellxgene_census.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25438 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/tests/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/experimental/ml/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/test_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/test_get_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/test_util.py
```

### Comparing `cellxgene_census-1.0.2/LICENSE` & `cellxgene_census-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.2/PKG-INFO` & `cellxgene_census-1.1.0/src/cellxgene_census.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cellxgene_census
-Version: 1.0.2
+Name: cellxgene-census
+Version: 1.1.0
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: experimental
 License-File: LICENSE
 
 # CZ CELLxGENE Discover Census
 
 The `cellxgene_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/).
```

### Comparing `cellxgene_census-1.0.2/README.md` & `cellxgene_census-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.2/pyproject.toml` & `cellxgene_census-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,32 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies= [
     # NOTE: the tiledbsoma version must be >= to the version used in the Census builder, to
     # ensure that the assets are readable (tiledbsoma supports backward compatible reading).
     # Make sure this version does not fall behind the builder's tiledbsoma version.
-    "tiledbsoma==1.2.4",
+    "tiledbsoma==1.2.5",
     "anndata",
     "numpy>=1.21,<1.24",  # numpy is constrained by numba and the old pip solver
     "requests",
     "typing_extensions",
     "s3fs",
     "scipy",
     # Temporary fix for Mac OSX, to be removed by https://github.com/chanzuckerberg/cellxgene-census/issues/415
     "certifi",
 ]
 
+[project.optional-dependencies]
+experimental = [
+    "torch==2.0.1",
+    "torchdata==0.6.1",
+    "scikit-learn==1.2.2",
+]
+
 [project.urls]
 homepage = "https://github.com/chanzuckerberg/cellxgene-census"
 repository = "https://github.com/chanzuckerberg/cellxgene-census"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["cellxgene_census*"]  # package names should match these glob patterns (["*"] by default)
@@ -65,14 +72,15 @@
 strict = true
 plugins = "numpy.typing.mypy_plugin"
 
 [tool.pytest.ini_options]
 markers = [
     "live_corpus: runs on the live CELLxGENE Census data corpus and small enough to run in CI",
     "expensive: too expensive to run regularly or in CI",
+    "experimental: tests for the `experimental` package",
 ]
 
 [tool.ruff]
 select = ["E", "F", "B", "I"]
 ignore = ["E501", "E402", "C408", ]
 line-length = 120
 target-version = "py39"
```

### Comparing `cellxgene_census-1.0.2/release_process.md` & `cellxgene_census-1.1.0/release_process.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.2/src/cellxgene_census/__init__.py` & `cellxgene_census-1.1.0/src/cellxgene_census/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 """
-An API to facilitate use of the CZI Science CELLxGENE Census. The Census is a versioned container of single-cell data hosted at [CELLxGENE Discover](https://cellxgene.cziscience.com/).
+An API to facilitate use of the CZI Science CELLxGENE Census. The Census is a versioned container of single-cell data hosted at `CELLxGENE Discover`_.
 
 The API is built on the `tiledbsoma` SOMA API, and provides a number of helper functions including:
 
     * Open a named version of the Census, for use with the SOMA API
     * Get a list of available Census versions, and for each version, a description
     * Get a slice of the Census as an AnnData, for use with ScanPy
     * Get the URI for, or directly download, underlying data in H5AD format
 
-For more information on the API, visit the [cellxgene_census repo](https://github.com/chanzuckerberg/cellxgene-census/). For more information on SOMA, see the [tiledbsoma repo](https://github.com/single-cell-data/TileDB-SOMA).
+For more information on the API, visit the `cellxgene_census repo`_. For more information on SOMA, see the `tiledbsoma repo`_.
+
+.. _CELLxGENE Discover:
+    https://cellxgene.cziscience.com/
+
+.. _cellxgene_census repo:
+    https://github.com/chanzuckerberg/cellxgene-census/
+
+.. _tiledbsoma repo:
+    https://github.com/single-cell-data/TileDB-SOMA
 """
 
 try:
     from importlib import metadata
 except ImportError:
     # for python <=3.7
     import importlib_metadata as metadata  # type: ignore[no-redef]
```

### Comparing `cellxgene_census-1.0.2/src/cellxgene_census/_experiment.py` & `cellxgene_census-1.1.0/src/cellxgene_census/_experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Returns:
         A soma.Experiment object with the requested experiment.
 
     Raises:
         ValueError: if unable to find the specified organism.
 
     Lifecycle:
-        Experimental.
+        maturing
 
     Examples:
 
         >>> human = get_experiment(census, 'homo sapiens')
 
         >>> human = get_experiment(census, 'Homo sapiens')
```

### Comparing `cellxgene_census-1.0.2/src/cellxgene_census/_get_anndata.py` & `cellxgene_census-1.1.0/src/cellxgene_census/_get_anndata.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         column_names:
             Columns to fetch for ``obs`` and ``var`` dataframes.
 
     Returns:
         An :class:`anndata.AnnData` object containing the census slice.
 
     Lifecycle:
-        Experimental.
+        maturing
 
     Examples:
         >>> get_anndata(census, "Mus musculus", obs_value_filter="tissue_general in ['brain', 'lung']")
 
         >>> get_anndata(census, "Homo sapiens", column_names={"obs": ["tissue"]})
 
         >>> get_anndata(census, "Homo sapiens", obs_coords=slice(0, 1000))
```

### Comparing `cellxgene_census-1.0.2/src/cellxgene_census/_open.py` & `cellxgene_census-1.1.0/src/cellxgene_census/_open.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,25 @@
 api_logger = logging.getLogger("cellxgene_census")
 api_logger.setLevel(logging.INFO)
 api_logger.addHandler(logging.StreamHandler())
 
 
 def _open_soma(locator: CensusLocator, context: Optional[soma.options.SOMATileDBContext] = None) -> soma.Collection:
     """Private. Merge config defaults and return open census as a soma Collection/context."""
-    s3_region = locator.get("s3_region")
+    context = _build_soma_tiledb_context(locator.get("s3_region"), context)
+    return soma.open(locator["uri"], mode="r", soma_type=soma.Collection, context=context)
+
+
+def _build_soma_tiledb_context(
+    s3_region: Optional[str] = None, context: Optional[soma.options.SOMATileDBContext] = None
+) -> soma.options.SOMATileDBContext:
+    """
+    Private. Build a SOMATileDBContext with sensible defaults. If user-defined context is provided, only update the
+    `vfs.s3.region` only.
+    """
 
     if not context:
         # if no user-defined context, cellxgene_census defaults take precedence over SOMA defaults
         context = soma.options.SOMATileDBContext()
         tiledb_config = {**DEFAULT_TILEDB_CONFIGURATION}
         if s3_region is not None:
             tiledb_config["vfs.s3.region"] = s3_region
@@ -46,16 +56,15 @@
         context = context.replace(tiledb_config=tiledb_config)
     else:
         # if specified, the user context takes precedence _except_ for AWS Region in locator
         if s3_region is not None:
             tiledb_config = context.tiledb_ctx.config()
             tiledb_config["vfs.s3.region"] = s3_region
             context = context.replace(tiledb_config=tiledb_config)
-
-    return soma.open(locator["uri"], mode="r", soma_type=soma.Collection, context=context)
+    return context
 
 
 def open_soma(
     *,
     census_version: Optional[str] = "stable",
     uri: Optional[str] = None,
     context: Optional[soma.options.SOMATileDBContext] = None,
@@ -76,15 +85,15 @@
         It can be used as a context manager, which will automatically close upon exit.
 
     Raises:
         ValueError: if the census cannot be found, the URI cannot be opened, or neither a URI
             or a version are specified.
 
     Lifecycle:
-        Experimental.
+        maturing
 
     Examples:
         Open the default Census version, using a context manager which will automatically
         close the Census upon exit of the context.
 
         >>> with cellxgene_census.open_soma() as census:
                 ...
@@ -156,15 +165,15 @@
     Returns:
         A :py:obj:`CensusLocator` object that contains the URI and optional S3 region for the source H5AD.
 
     Raises:
         KeyError: if either `dataset_id` or `census_version` do not exist.
 
     Lifecycle:
-        Experimental.
+        maturing
 
     Examples:
         >>> cellxgene_census.get_source_h5ad_uri("cb5efdb0-f91c-4cbd-9ad4-9d4fa41c572d")
         {'uri': 's3://cellxgene-data-public/cell-census/2022-12-01/h5ads/cb5efdb0-f91c-4cbd-9ad4-9d4fa41c572d.h5ad',
         's3_region': 'us-west-2'}
     """
     description = get_census_version_description(census_version)  # raises
@@ -193,15 +202,15 @@
             The census version name. Defaults to `latest`.
 
     Raises:
         ValueError: if the path already exists (i.e., will not overwrite
             an existing file), or is not a file.
 
     Lifecycle:
-        Experimental.
+        maturing
 
     See Also:
         :func:`get_source_h5ad_uri`: Look up the location of the source H5AD.
 
     Examples:
         >>> download_source_h5ad("8e47ed12-c658-4252-b126-381df8d52a3d", to_path="/tmp/data.h5ad")
     """
```

### Comparing `cellxgene_census-1.0.2/src/cellxgene_census/_presence_matrix.py` & `cellxgene_census-1.1.0/src/cellxgene_census/_presence_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     Returns:
         A :class:`scipy.sparse.csr_array` object containing the presence matrix.
 
     Raises:
         ValueError: if the organism cannot be found.
 
     Lifecycle:
-        Experimental.
+        maturing
 
     Examples:
         >>> get_presence_matrix(census, "Homo sapiens", "RNA")
         <321x60554 sparse array of type '<class 'numpy.uint8'>'
         with 6441269 stored elements in Compressed Sparse Row format>
     """
```

### Comparing `cellxgene_census-1.0.2/src/cellxgene_census/_release_directory.py` & `cellxgene_census-1.1.0/src/cellxgene_census/_release_directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     Returns:
         ``CensusVersionDescription`` - a dictionary containing a description of the release.
 
     Raises:
         KeyError: if unknown census_version value.
 
     Lifecycle:
-        Experimental.
+        maturing
 
     See Also:
         :func:`get_census_version_directory`: returns the entire directory as a dict.
 
     Examples:
         >>> cellxgene_census.get_census_version_description("latest")
         {'release_date': None,
@@ -79,15 +79,15 @@
     """
     Get the directory of Census releases currently available.
 
     Returns:
         A dictionary that contains release names and their corresponding release description.
 
     Lifecycle:
-        Experimental.
+        maturing
 
     See Also:
         :func:`get_census_version_description`: get description by census_version.
 
     Examples:
         >>> cellxgene_census.get_census_version_directory()
         {'latest': {'release_date': None,
```

### Comparing `cellxgene_census-1.0.2/src/cellxgene_census.egg-info/PKG-INFO` & `cellxgene_census-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cellxgene-census
-Version: 1.0.2
+Name: cellxgene_census
+Version: 1.1.0
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: experimental
 License-File: LICENSE
 
 # CZ CELLxGENE Discover Census
 
 The `cellxgene_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/).
```

### Comparing `cellxgene_census-1.0.2/src/cellxgene_census.egg-info/SOURCES.txt` & `cellxgene_census-1.1.0/src/cellxgene_census.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,22 @@
 src/cellxgene_census/_release_directory.py
 src/cellxgene_census/_util.py
 src/cellxgene_census.egg-info/PKG-INFO
 src/cellxgene_census.egg-info/SOURCES.txt
 src/cellxgene_census.egg-info/dependency_links.txt
 src/cellxgene_census.egg-info/requires.txt
 src/cellxgene_census.egg-info/top_level.txt
+src/cellxgene_census/experimental/__init__.py
+src/cellxgene_census/experimental/ml/__init__.py
+src/cellxgene_census/experimental/ml/pytorch.py
 tests/README.md
+tests/__init__.py
 tests/conftest.py
 tests/test_acceptance.py
 tests/test_directory.py
 tests/test_get_anndata.py
 tests/test_get_helpers.py
 tests/test_open.py
-tests/test_util.py
+tests/test_util.py
+tests/experimental/__init__.py
+tests/experimental/ml/__init__.py
+tests/experimental/ml/test_pytorch.py
```

### Comparing `cellxgene_census-1.0.2/tests/README.md` & `cellxgene_census-1.1.0/tests/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,35 @@
 
 Then run the tests:
 
 > pytest ./api/python/cellxgene_census/
 
 ## Pytest Marks
 
-There are two Pytest marks you can use from the command line:
+There are various Pytest marks you can use from the command line:
 
 - live_corpus: tests that directly access the `latest` version of the Census. Enabled by default.
 - expensive: tests that are expensive (ie., cpu, memory, time). Disabled by default - enable with `--expensive`. Some of these tests are _very_ expensive, ie., require a very large memory host to succeed.
+- experimental: tests that are for code in the `experimental` package. Disabled by default - enable with `--experimental`. These tests require installation the optional Python packages installed via pip `pip install -e ./api/python/cellxgene_census/[experimental]`
 
 By default, only relatively cheap & fast tests are run. To enable `expensive` tests:
 
 > pytest --expensive ...
 
+To enable `experimental` tests:
+
+> pytest --experimental ...
+
 To disable `live_corpus` tests:
 
 > pytest -m 'not live_corpus'
 
 You can also combine them, e.g.,
 
-> pytest -m 'not live_corpus' --expensive
+> pytest -m 'not live_corpus' --expensive --experimental
 
 # Acceptance (expensive) tests
 
 These tests are periodically run, and are not part of CI due to their overhead.
 
 When run, please record the results in this file (below) and commit the change to git. Please include the following information:
```

### Comparing `cellxgene_census-1.0.2/tests/test_acceptance.py` & `cellxgene_census-1.1.0/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.2/tests/test_directory.py` & `cellxgene_census-1.1.0/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.2/tests/test_get_anndata.py` & `cellxgene_census-1.1.0/tests/test_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.2/tests/test_get_helpers.py` & `cellxgene_census-1.1.0/tests/test_get_helpers.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.2/tests/test_open.py` & `cellxgene_census-1.1.0/tests/test_open.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,15 @@
     os.environ["AWS_ACCESS_KEY_ID"] = "fake_id"
     os.environ["AWS_SECRET_ACCESS_KEY"] = "fake_key"
     # Passing an empty context
     with pytest.raises(Exception):
         cellxgene_census.open_soma(census_version="latest", context=soma.SOMATileDBContext())
 
 
+@pytest.mark.live_corpus
 def test_can_open_with_anonymous_access() -> None:
     """
     With anonymous access, `open_soma` must be able to access the census even with bogus credentials
     """
     os.environ["AWS_ACCESS_KEY_ID"] = "fake_id"
     os.environ["AWS_SECRET_ACCESS_KEY"] = "fake_key"
     with cellxgene_census.open_soma(census_version="latest") as census:
```

### Comparing `cellxgene_census-1.0.2/tests/test_util.py` & `cellxgene_census-1.1.0/tests/test_util.py`

 * *Files identical despite different names*

