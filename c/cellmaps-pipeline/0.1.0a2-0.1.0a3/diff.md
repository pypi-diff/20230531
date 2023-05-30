# Comparing `tmp/cellmaps_pipeline-0.1.0a2.tar.gz` & `tmp/cellmaps_pipeline-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a2.tar", last modified: Wed May 24 17:17:41 2023, max compression
+gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a3.tar", last modified: Tue May 30 23:33:24 2023, max compression
```

## Comparing `cellmaps_pipeline-0.1.0a2.tar` & `cellmaps_pipeline-0.1.0a3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.609582 cellmaps_pipeline-0.1.0a2/
--rw-r--r--   0 churas     (504) staff       (20)      160 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a2/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3641 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a2/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-22 23:49:21.000000 cellmaps_pipeline-0.1.0a2/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a2/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a2/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6043 2023-05-24 17:17:41.609813 cellmaps_pipeline-0.1.0a2/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4019 2023-05-22 23:49:10.000000 cellmaps_pipeline-0.1.0a2/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.600173 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/
--rw-r--r--   0 churas     (504) staff       (20)      277 2023-05-23 23:25:11.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     7654 2023-05-23 16:27:52.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      132 2023-04-04 23:01:54.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    11405 2023-05-23 23:24:07.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.601735 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6043 2023-05-24 17:17:41.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1024 2023-05-24 17:17:41.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-24 17:17:41.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-24 17:17:41.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)      169 2023-05-24 17:17:41.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       18 2023-05-24 17:17:41.000000 cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.606531 cellmaps_pipeline-0.1.0a2/docs/
--rw-r--r--   0 churas     (504) staff       (20)      618 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.595415 cellmaps_pipeline-0.1.0a2/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.595483 cellmaps_pipeline-0.1.0a2/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.607412 cellmaps_pipeline-0.1.0a2/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a2/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a2/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a2/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)      744 2023-05-22 23:59:43.000000 cellmaps_pipeline-0.1.0a2/docs/cellmaps_pipeline.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6035 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      285 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      934 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1189 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      451 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      815 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       76 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4340 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      787 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      687 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      400 2023-05-24 17:17:41.610332 cellmaps_pipeline-0.1.0a2/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2386 2023-05-19 23:36:32.000000 cellmaps_pipeline-0.1.0a2/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 17:17:41.609273 cellmaps_pipeline-0.1.0a2/tests/
--rw-r--r--   0 churas     (504) staff       (20)       72 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a2/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     2554 2023-04-04 23:02:59.000000 cellmaps_pipeline-0.1.0a2/tests/test_cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      896 2023-05-19 22:06:11.000000 cellmaps_pipeline-0.1.0a2/tests/test_cellmapspipeline.py
--rw-r--r--   0 churas     (504) staff       (20)      772 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a2/tests/test_integration_cellmaps_pipeline.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.178800 cellmaps_pipeline-0.1.0a3/
+-rw-r--r--   0 churas     (504) staff       (20)      160 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a3/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3641 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a3/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-22 23:49:21.000000 cellmaps_pipeline-0.1.0a3/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a3/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a3/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6043 2023-05-30 23:33:24.178917 cellmaps_pipeline-0.1.0a3/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4019 2023-05-22 23:49:10.000000 cellmaps_pipeline-0.1.0a3/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.170785 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/
+-rw-r--r--   0 churas     (504) staff       (20)      277 2023-05-30 21:24:11.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     7654 2023-05-23 16:27:52.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      132 2023-04-04 23:01:54.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    11415 2023-05-30 21:24:11.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.172042 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6043 2023-05-30 23:33:24.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1024 2023-05-30 23:33:24.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-30 23:33:24.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-30 23:33:24.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)      169 2023-05-30 23:33:24.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       18 2023-05-30 23:33:24.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.176629 cellmaps_pipeline-0.1.0a3/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      618 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.167907 cellmaps_pipeline-0.1.0a3/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.167972 cellmaps_pipeline-0.1.0a3/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.177730 cellmaps_pipeline-0.1.0a3/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a3/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a3/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a3/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      744 2023-05-22 23:59:43.000000 cellmaps_pipeline-0.1.0a3/docs/cellmaps_pipeline.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6035 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      285 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      934 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1189 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      451 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      815 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       76 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4340 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      787 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      687 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      400 2023-05-30 23:33:24.179349 cellmaps_pipeline-0.1.0a3/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2386 2023-05-19 23:36:32.000000 cellmaps_pipeline-0.1.0a3/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.178627 cellmaps_pipeline-0.1.0a3/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       72 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1296 2023-05-30 21:25:35.000000 cellmaps_pipeline-0.1.0a3/tests/test_cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      896 2023-05-30 21:25:54.000000 cellmaps_pipeline-0.1.0a3/tests/test_cellmapspipeline.py
+-rw-r--r--   0 churas     (504) staff       (20)      772 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a3/tests/test_integration_cellmaps_pipeline.py
```

### Comparing `cellmaps_pipeline-0.1.0a2/CONTRIBUTING.rst` & `cellmaps_pipeline-0.1.0a3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/LICENSE` & `cellmaps_pipeline-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/PKG-INFO` & `cellmaps_pipeline-0.1.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_pipeline
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Runs full Cellmaps CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
 Author: Christopher Churas
 Author-email: cchuras@ucsd.edu
 License: MIT license
 Description: ==============
         CM4AI Pipeline
```

### Comparing `cellmaps_pipeline-0.1.0a2/README.rst` & `cellmaps_pipeline-0.1.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/cellmaps_pipelinecmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/cellmaps_pipeline/runner.py` & `cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from cellmaps_image_embedding.runner import CellmapsImageEmbedder
 from cellmaps_image_embedding.runner import FakeEmbeddingGenerator
 from cellmaps_image_embedding.runner import DensenetEmbeddingGenerator
 from cellmaps_coembedding.runner import MuseCoEmbeddingGenerator
 from cellmaps_coembedding.runner import FakeCoEmbeddingGenerator
 from cellmaps_coembedding.runner import CellmapsCoEmbedder
 from cellmaps_generate_hierarchy.ppi import CosineSimilarityPPIGenerator
-from cellmaps_generate_hierarchy.hierarchy import CDAPSHierarchyGenerator
+from cellmaps_generate_hierarchy.hierarchy import CDAPSHiDeFHierarchyGenerator
 from cellmaps_generate_hierarchy.runner import CellmapsGenerateHierarchy
 
 import cellmaps_pipeline
 from cellmaps_pipeline.exceptions import CellmapsPipelineError
 
 
 logger = logging.getLogger(__name__)
@@ -129,15 +129,15 @@
         """
         if os.path.isdir(self._hierarchy_dir):
             warnings.warn('Found hierarchy dir, assuming we are good. skipping')
             return 0
 
         ppigen = CosineSimilarityPPIGenerator(embeddingdir=self._coembed_dir)
 
-        hiergen = CDAPSHierarchyGenerator()
+        hiergen = CDAPSHiDeFHierarchyGenerator()
         return CellmapsGenerateHierarchy(outdir=self._hierarchy_dir,
                                          inputdir=self._coembed_dir,
                                          ppigen=ppigen,
                                          hiergen=hiergen,
                                          input_data_dict=self._input_data_dict).run()
 
     def _coembed(self):
```

### Comparing `cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/PKG-INFO` & `cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-pipeline
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Runs full Cellmaps CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
 Author: Christopher Churas
 Author-email: cchuras@ucsd.edu
 License: MIT license
 Description: ==============
         CM4AI Pipeline
```

### Comparing `cellmaps_pipeline-0.1.0a2/cellmaps_pipeline.egg-info/SOURCES.txt` & `cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/docs/Makefile` & `cellmaps_pipeline-0.1.0a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/docs/cellmaps_pipeline.rst` & `cellmaps_pipeline-0.1.0a3/docs/cellmaps_pipeline.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/docs/conf.py` & `cellmaps_pipeline-0.1.0a3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/docs/index.rst` & `cellmaps_pipeline-0.1.0a3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/docs/installation.rst` & `cellmaps_pipeline-0.1.0a3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/docs/make.bat` & `cellmaps_pipeline-0.1.0a3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/docs/newrelease.rst` & `cellmaps_pipeline-0.1.0a3/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/docs/pypircfile.rst` & `cellmaps_pipeline-0.1.0a3/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/docs/usage.rst` & `cellmaps_pipeline-0.1.0a3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/docs/versioningscheme.rst` & `cellmaps_pipeline-0.1.0a3/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/setup.py` & `cellmaps_pipeline-0.1.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a2/tests/test_cellmapspipeline.py` & `cellmaps_pipeline-0.1.0a3/tests/test_cellmapspipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,19 @@
         """Set up test fixtures, if any."""
 
     def tearDown(self):
         """Tear down test fixtures, if any."""
 
     def test_constructor(self):
         """Tests constructor"""
-        myobj = CellmapsPipeline(0)
+        myobj = CellmapsPipeline('foo')
 
         self.assertIsNotNone(myobj)
 
     def test_run_outdir_not_set(self):
         """ Tests run()"""
         try:
             myobj = CellmapsPipeline()
             myobj.run()
             self.fail('expected exception')
         except CellmapsPipelineError as e:
-            self.assertEqual('outdir must be set', str(e))
+            self.assertEqual('outdir is None', str(e))
```

### Comparing `cellmaps_pipeline-0.1.0a2/tests/test_integration_cellmaps_pipeline.py` & `cellmaps_pipeline-0.1.0a3/tests/test_integration_cellmaps_pipeline.py`

 * *Files identical despite different names*

