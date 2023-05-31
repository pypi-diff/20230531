# Comparing `tmp/tiledb_jupyter_bioimg-0.1.1a6.tar.gz` & `tmp/tiledb_jupyter_bioimg-0.1.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb_jupyter_bioimg-0.1.1a6.tar", last modified: Tue May 30 15:54:14 2023, max compression
+gzip compressed data, was "tiledb_jupyter_bioimg-0.1.1a7.tar", last modified: Wed May 31 09:40:02 2023, max compression
```

## Comparing `tiledb_jupyter_bioimg-0.1.1a6.tar` & `tiledb_jupyter_bioimg-0.1.1a7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:54:14.676667 tiledb_jupyter_bioimg-0.1.1a6/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 15:54:14.676667 tiledb_jupyter_bioimg-0.1.1a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-30 15:51:33.000000 tiledb_jupyter_bioimg-0.1.1a6/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:54:14.676667 tiledb_jupyter_bioimg-0.1.1a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:54:14.668667 tiledb_jupyter_bioimg-0.1.1a6/src/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/src/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:54:14.668667 tiledb_jupyter_bioimg-0.1.1a6/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:54:14.672667 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:54:14.672667 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:54:14.676667 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14610 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
--rw-r--r--   0 runner    (1001) docker     (123)   725916 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js
--rw-r--r--   0 runner    (1001) docker     (123)   516691 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   172313 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/744.29f5fc192fc8171f023f.js
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/remoteEntry.7d8ec031bffcf5f758ea.js
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 15:53:39.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    90733 2023-05-30 15:54:13.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:54:14.672667 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 15:54:14.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-30 15:54:14.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:54:14.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:52:46.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 15:54:14.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 15:54:14.000000 tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-30 15:49:05.000000 tiledb_jupyter_bioimg-0.1.1a6/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:02.418595 tiledb_jupyter_bioimg-0.1.1a7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-31 09:40:02.418595 tiledb_jupyter_bioimg-0.1.1a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-31 09:37:17.000000 tiledb_jupyter_bioimg-0.1.1a7/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:40:02.418595 tiledb_jupyter_bioimg-0.1.1a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:02.410595 tiledb_jupyter_bioimg-0.1.1a7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/src/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:02.410595 tiledb_jupyter_bioimg-0.1.1a7/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:02.410595 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:02.414595 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:02.418595 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14610 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)   725916 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/633.1125117a0017a3fcb647.js
+-rw-r--r--   0 runner    (1001) docker     (123)   516691 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/635.812cb387a85b4a4dd127.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/635.812cb387a85b4a4dd127.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   172313 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/744.ca2ab2033fd1289054ea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/remoteEntry.5cdbd27cab7657a97979.js
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-31 09:39:29.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    90733 2023-05-31 09:40:00.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:02.414595 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-31 09:40:02.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-31 09:40:02.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:40:02.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:38:33.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 09:40:02.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 09:40:02.000000 tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-31 09:34:48.000000 tiledb_jupyter_bioimg-0.1.1a7/tsconfig.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/LICENSE` & `tiledb_jupyter_bioimg-0.1.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.1a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb_jupyter_bioimg
-Version: 0.1.1a6
+Version: 0.1.1a7
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/README.md` & `tiledb_jupyter_bioimg-0.1.1a7/README.md`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/package.json` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.91875%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.5cdbd27cab7657a97979.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'resolutions'": "OrderedDict([('@luma.gl/constants', '^8.5.16'), ('@deck.gl/aggregation-layers', "*

 * *                  "'^8.8.12'), ('@deck.gl/core', '^8.8.12'), ('@deck.gl/carto', '^8.8.12'), "*

 * *                  "('@deck.gl/extensions', '^8.8.12'), ('@deck.gl/geo-layers', '^8.8.12'), "*

 * *                  "('@deck.gl/google-maps', '^8.8. […]*

```diff
@@ -25,14 +25,19 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.5cdbd27cab7657a97979.js",
+            "style": "./style"
+        },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -41,14 +46,28 @@
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@tiledb-inc/jupyter-bioimage-viewer",
     "repository": {
         "type": "git",
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"
     },
+    "resolutions": {
+        "@deck.gl/aggregation-layers": "^8.8.12",
+        "@deck.gl/carto": "^8.8.12",
+        "@deck.gl/core": "^8.8.12",
+        "@deck.gl/extensions": "^8.8.12",
+        "@deck.gl/geo-layers": "^8.8.12",
+        "@deck.gl/google-maps": "^8.8.12",
+        "@deck.gl/json": "^8.8.12",
+        "@deck.gl/layers": "^8.8.12",
+        "@deck.gl/mapbox": "^8.8.12",
+        "@deck.gl/mesh-layers": "^8.8.12",
+        "@deck.gl/react": "^8.8.12",
+        "@luma.gl/constants": "^8.5.16"
+    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
@@ -67,9 +86,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1-alpha.6"
+    "version": "0.1.1-alpha.7"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/setup.py` & `tiledb_jupyter_bioimg-0.1.1a7/setup.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/src/index.ts` & `tiledb_jupyter_bioimg-0.1.1a7/src/index.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/src/version.ts` & `tiledb_jupyter_bioimg-0.1.1a7/src/version.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/src/widget.ts` & `tiledb_jupyter_bioimg-0.1.1a7/src/widget.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/_version.py` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/_version.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/package.json` & `tiledb_jupyter_bioimg-0.1.1a7/package.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.91875%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}",*

 * * "'resolutions'": "OrderedDict([('@luma.gl/constants', '^8.5.16'), ('@deck.gl/aggregation-layers', "*

 * *                  "'^8.8.12'), ('@deck.gl/core', '^8.8.12'), ('@deck.gl/carto', '^8.8.12'), "*

 * *                  "('@deck.gl/extensions', '^8.8.12'), ('@deck.gl/geo-layers', '^8.8.12'), "*

 * *                  "('@deck.gl/google-maps', '^8.8.12'), ('@deck.gl/mapbox', '^8.8.12'), "*

 * *                  "('@deck.gl/json', '^8.8.12'), ('@deck.gl/layers', '^8.8.12'), "*

 * *           […]*

```diff
@@ -25,19 +25,14 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.7d8ec031bffcf5f758ea.js",
-            "style": "./style"
-        },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -46,14 +41,28 @@
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@tiledb-inc/jupyter-bioimage-viewer",
     "repository": {
         "type": "git",
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"
     },
+    "resolutions": {
+        "@deck.gl/aggregation-layers": "^8.8.12",
+        "@deck.gl/carto": "^8.8.12",
+        "@deck.gl/core": "^8.8.12",
+        "@deck.gl/extensions": "^8.8.12",
+        "@deck.gl/geo-layers": "^8.8.12",
+        "@deck.gl/google-maps": "^8.8.12",
+        "@deck.gl/json": "^8.8.12",
+        "@deck.gl/layers": "^8.8.12",
+        "@deck.gl/mapbox": "^8.8.12",
+        "@deck.gl/mesh-layers": "^8.8.12",
+        "@deck.gl/react": "^8.8.12",
+        "@luma.gl/constants": "^8.5.16"
+    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
@@ -72,9 +81,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1-alpha.6"
+    "version": "0.1.1-alpha.7"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/633.1125117a0017a3fcb647.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -37,47 +37,47 @@
                             basePath: e.data.basePath
                         },
                         r = new(n())(t),
                         a = e.data.downsample,
                         i = e.data.index.x,
                         s = e.data.index.y,
                         l = e.data.tileSize,
-                        f = e.data.format,
-                        c = e.data.axes.indexOf("X"),
+                        c = e.data.format,
+                        f = e.data.axes.indexOf("X"),
                         u = e.data.axes.indexOf("Y"),
                         p = e.data.axes.indexOf("C"),
                         d = new Array(3);
-                    d[c] = [i * l * a, Math.min((i + 1) * l * a, e.data.levelWidth) - 1], d[u] = [s * l * a, Math.min((s + 1) * l * a, e.data.levelHeight) - 1], d[p] = e.data.channelRanges;
-                    const y = (d[c][1] - d[c][0] + 1) / a,
+                    d[f] = [i * l * a, Math.min((i + 1) * l * a, e.data.levelWidth) - 1], d[u] = [s * l * a, Math.min((s + 1) * l * a, e.data.levelHeight) - 1], d[p] = e.data.channelRanges;
+                    const y = (d[f][1] - d[f][0] + 1) / a,
                         h = (d[u][1] - d[u][0] + 1) / a;
                     let b = 0;
                     if ("number" == typeof d[p][0]) b = d[p][1] - d[p][0] + 1;
                     else
                         for (const e of d[p]) b += e[1] - e[0] + 1;
                     const v = {
                             layout: "row-major",
                             ranges: d,
-                            bufferSize: Math.pow(l * a, 2) * b * o[f].bytes,
+                            bufferSize: Math.pow(l * a, 2) * b * o[c].bytes,
                             attributes: ["intensity"],
                             returnRawBuffers: !0
                         },
                         m = r.query.ReadQuery(e.data.namespace, e.data.levelUri, v),
-                        g = o[f].create(await m.next().then((e => e.value.intensity))),
-                        w = o[f].create(y * h * b),
+                        g = o[c].create(await m.next().then((e => e.value.intensity))),
+                        w = o[c].create(y * h * b),
                         E = new Array(3);
                     for (let e = 0; e < d.length; ++e) E[e] = d[e][1] - d[e][0] + 1;
                     1 === a ? self.postMessage({
                         data: g,
                         width: y,
                         height: h,
                         channels: b
                     }, [g.buffer]) : (g.forEach(((e, t) => {
                         const r = new Array(3);
                         r[0] = ~~(t / (E[1] * E[2])), r[1] = ~~(t % (E[1] * E[2]) / E[2]), r[2] = t % E[2];
-                        const n = (r[p] * h + ~~(r[u] / a)) * y + ~~(r[c] / a);
+                        const n = (r[p] * h + ~~(r[u] / a)) * y + ~~(r[f] / a);
                         w[n] = e
                     })), self.postMessage({
                         data: w,
                         width: y,
                         height: h,
                         channels: b
                     }, [w.buffer]))
@@ -98,38 +98,38 @@
     }
     n.m = r, n.c = a, n.x = () => {
         var e = n.O(void 0, [635], (() => n(9936)));
         return n.O(e)
     }, e = [], n.O = (t, r, a, i) => {
         if (!r) {
             var o = 1 / 0;
-            for (c = 0; c < e.length; c++) {
-                for (var [r, a, i] = e[c], s = !0, l = 0; l < r.length; l++)(!1 & i || o >= i) && Object.keys(n.O).every((e => n.O[e](r[l]))) ? r.splice(l--, 1) : (s = !1, i < o && (o = i));
+            for (f = 0; f < e.length; f++) {
+                for (var [r, a, i] = e[f], s = !0, l = 0; l < r.length; l++)(!1 & i || o >= i) && Object.keys(n.O).every((e => n.O[e](r[l]))) ? r.splice(l--, 1) : (s = !1, i < o && (o = i));
                 if (s) {
-                    e.splice(c--, 1);
-                    var f = a();
-                    void 0 !== f && (t = f)
+                    e.splice(f--, 1);
+                    var c = a();
+                    void 0 !== c && (t = c)
                 }
             }
             return t
         }
         i = i || 0;
-        for (var c = e.length; c > 0 && e[c - 1][2] > i; c--) e[c] = e[c - 1];
-        e[c] = [r, a, i]
+        for (var f = e.length; f > 0 && e[f - 1][2] > i; f--) e[f] = e[f - 1];
+        e[f] = [r, a, i]
     }, n.n = e => {
         var t = e && e.__esModule ? () => e.default : () => e;
         return n.d(t, {
             a: t
         }), t
     }, n.d = (e, t) => {
         for (var r in t) n.o(t, r) && !n.o(e, r) && Object.defineProperty(e, r, {
             enumerable: !0,
             get: t[r]
         })
-    }, n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, r) => (n.f[r](e, t), t)), [])), n.u = e => e + ".024275f22a135fe53126.js?v=024275f22a135fe53126", n.g = function() {
+    }, n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, r) => (n.f[r](e, t), t)), [])), n.u = e => e + ".812cb387a85b4a4dd127.js?v=812cb387a85b4a4dd127", n.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), n.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), n.r = e => {
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/635.812cb387a85b4a4dd127.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 635.024275f22a135fe53126.js.LICENSE.txt */
+/*! For license information please see 635.812cb387a85b4a4dd127.js.LICENSE.txt */
 (self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || []).push([
     [635], {
         9757: (t, e, r) => {
             "use strict";
             r.d(e, {
                 Z: () => i
             });
@@ -12180,15 +12180,15 @@
             }
         },
         9669: (t, e, r) => {
             t.exports = r(1609)
         },
         5448: (t, e, r) => {
             "use strict";
-            var i = r(4867),
+            var i = r(3837),
                 s = r(6026),
                 n = r(4372),
                 a = r(5327),
                 o = r(4097),
                 c = r(4109),
                 u = r(7985),
                 p = r(5061);
@@ -12239,15 +12239,15 @@
                         g && (g.abort(), r(t), g = null)
                     })), d || (d = null), g.send(d)
                 }))
             }
         },
         1609: (t, e, r) => {
             "use strict";
-            var i = r(4867),
+            var i = r(3837),
                 s = r(1849),
                 n = r(321),
                 a = r(7185);
 
             function o(t) {
                 var e = new n(t),
                     r = s(n.prototype.request, e);
@@ -12301,15 +12301,15 @@
             "use strict";
             t.exports = function(t) {
                 return !(!t || !t.__CANCEL__)
             }
         },
         321: (t, e, r) => {
             "use strict";
-            var i = r(4867),
+            var i = r(3837),
                 s = r(5327),
                 n = r(782),
                 a = r(3572),
                 o = r(7185),
                 c = r(4875),
                 u = c.validators;
 
@@ -12375,15 +12375,15 @@
                         data: r
                     }))
                 }
             })), t.exports = p
         },
         782: (t, e, r) => {
             "use strict";
-            var i = r(4867);
+            var i = r(3837);
 
             function s() {
                 this.handlers = []
             }
             s.prototype.use = function(t, e, r) {
                 return this.handlers.push({
                     fulfilled: t,
@@ -12413,15 +12413,15 @@
             t.exports = function(t, e, r, s, n) {
                 var a = new Error(t);
                 return i(a, e, r, s, n)
             }
         },
         3572: (t, e, r) => {
             "use strict";
-            var i = r(4867),
+            var i = r(3837),
                 s = r(8527),
                 n = r(6502),
                 a = r(5655);
 
             function o(t) {
                 t.cancelToken && t.cancelToken.throwIfRequested()
             }
@@ -12452,15 +12452,15 @@
                         code: this.code
                     }
                 }, t
             }
         },
         7185: (t, e, r) => {
             "use strict";
-            var i = r(4867);
+            var i = r(3837);
             t.exports = function(t, e) {
                 e = e || {};
                 var r = {},
                     s = ["url", "method", "data"],
                     n = ["headers", "auth", "proxy", "params"],
                     a = ["baseURL", "transformRequest", "transformResponse", "paramsSerializer", "timeout", "timeoutMessage", "withCredentials", "adapter", "responseType", "xsrfCookieName", "xsrfHeaderName", "onUploadProgress", "onDownloadProgress", "decompress", "maxContentLength", "maxBodyLength", "maxRedirects", "transport", "httpAgent", "httpsAgent", "cancelToken", "socketPath", "responseEncoding"],
                     o = ["validateStatus"];
@@ -12492,27 +12492,27 @@
             t.exports = function(t, e, r) {
                 var s = r.config.validateStatus;
                 r.status && s && !s(r.status) ? e(i("Request failed with status code " + r.status, r.config, null, r.request, r)) : t(r)
             }
         },
         8527: (t, e, r) => {
             "use strict";
-            var i = r(4867),
+            var i = r(3837),
                 s = r(5655);
             t.exports = function(t, e, r) {
                 var n = this || s;
                 return i.forEach(r, (function(r) {
                     t = r.call(n, t, e)
                 })), t
             }
         },
         5655: (t, e, r) => {
             "use strict";
             var i = r(4155),
-                s = r(4867),
+                s = r(3837),
                 n = r(6016),
                 a = r(481),
                 o = {
                     "Content-Type": "application/x-www-form-urlencoded"
                 };
 
             function c(t, e) {
@@ -12577,15 +12577,15 @@
                     for (var r = new Array(arguments.length), i = 0; i < r.length; i++) r[i] = arguments[i];
                     return t.apply(e, r)
                 }
             }
         },
         5327: (t, e, r) => {
             "use strict";
-            var i = r(4867);
+            var i = r(3837);
 
             function s(t) {
                 return encodeURIComponent(t).replace(/%3A/gi, ":").replace(/%24/g, "$").replace(/%2C/gi, ",").replace(/%20/g, "+").replace(/%5B/gi, "[").replace(/%5D/gi, "]")
             }
             t.exports = function(t, e, r) {
                 if (!e) return t;
                 var n;
@@ -12609,15 +12609,15 @@
             "use strict";
             t.exports = function(t, e) {
                 return e ? t.replace(/\/+$/, "") + "/" + e.replace(/^\/+/, "") : t
             }
         },
         4372: (t, e, r) => {
             "use strict";
-            var i = r(4867);
+            var i = r(3837);
             t.exports = i.isStandardBrowserEnv() ? {
                 write: function(t, e, r, s, n, a) {
                     var o = [];
                     o.push(t + "=" + encodeURIComponent(e)), i.isNumber(r) && o.push("expires=" + new Date(r).toGMTString()), i.isString(s) && o.push("path=" + s), i.isString(n) && o.push("domain=" + n), !0 === a && o.push("secure"), document.cookie = o.join("; ")
                 },
                 read: function(t) {
                     var e = document.cookie.match(new RegExp("(^|;\\s*)(" + t + ")=([^;]*)"));
@@ -12644,15 +12644,15 @@
             "use strict";
             t.exports = function(t) {
                 return "object" == typeof t && !0 === t.isAxiosError
             }
         },
         7985: (t, e, r) => {
             "use strict";
-            var i = r(4867);
+            var i = r(3837);
             t.exports = i.isStandardBrowserEnv() ? function() {
                 var t, e = /(msie|trident)/i.test(navigator.userAgent),
                     r = document.createElement("a");
 
                 function s(t) {
                     var i = t;
                     return e && (r.setAttribute("href", i), i = r.href), r.setAttribute("href", i), {
@@ -12673,24 +12673,24 @@
                     }
             }() : function() {
                 return !0
             }
         },
         6016: (t, e, r) => {
             "use strict";
-            var i = r(4867);
+            var i = r(3837);
             t.exports = function(t, e) {
                 i.forEach(t, (function(r, i) {
                     i !== e && i.toUpperCase() === e.toUpperCase() && (t[e] = r, delete t[i])
                 }))
             }
         },
         4109: (t, e, r) => {
             "use strict";
-            var i = r(4867),
+            var i = r(3837),
                 s = ["age", "authorization", "content-length", "content-type", "etag", "expires", "from", "host", "if-modified-since", "if-unmodified-since", "last-modified", "location", "max-forwards", "proxy-authorization", "referer", "retry-after", "user-agent"];
             t.exports = function(t) {
                 var e, r, n, a = {};
                 return t ? (i.forEach(t.split("\n"), (function(t) {
                     if (n = t.indexOf(":"), e = i.trim(t.substr(0, n)).toLowerCase(), r = i.trim(t.substr(n + 1)), e) {
                         if (a[e] && s.indexOf(e) >= 0) return;
                         a[e] = "set-cookie" === e ? (a[e] ? a[e] : []).concat([r]) : a[e] ? a[e] + ", " + r : r
@@ -12748,15 +12748,15 @@
                             if (!0 !== c) throw new TypeError("option " + n + " must be " + c)
                         } else if (!0 !== r) throw Error("Unknown option " + n)
                     }
                 },
                 validators: s
             }
         },
-        4867: (t, e, r) => {
+        3837: (t, e, r) => {
             "use strict";
             var i = r(1849),
                 s = Object.prototype.toString;
 
             function n(t) {
                 return "[object Array]" === s.call(t)
             }
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/635.812cb387a85b4a4dd127.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/744.29f5fc192fc8171f023f.js` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/744.ca2ab2033fd1289054ea.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,65 +1,65 @@
 "use strict";
 (self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || []).push([
     [744], {
         1744: (e, i, t) => {
             t.r(i), t.d(i, {
                 MODULE_NAME: () => o,
                 MODULE_VERSION: () => r,
-                default: () => m
+                default: () => c
             });
             var l = {};
             t.r(l), t.d(l, {
-                BioImageViewerModel: () => d,
+                BioImageViewerModel: () => u,
                 BioImageViewerView: () => p
             });
             var s = t(8233);
             const n = t(4147),
                 r = n.version,
                 o = n.name;
             var a = t(2832),
-                u = t.n(a);
-            class d extends s.DOMWidgetModel {
+                d = t.n(a);
+            class u extends s.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: d.model_name,
-                        _model_module: d.model_module,
-                        _model_module_version: d.model_module_version,
-                        _view_name: d.view_name,
-                        _view_module: d.view_module,
-                        _view_module_version: d.view_module_version
+                        _model_name: u.model_name,
+                        _model_module: u.model_module,
+                        _model_module_version: u.model_module_version,
+                        _view_name: u.view_name,
+                        _view_module: u.view_module,
+                        _view_module_version: u.view_module_version
                     })
                 }
             }
-            d.model_module = o, d.model_module_version = r, d.view_module = o, d.view_module_version = r, d.serializers = Object.assign({}, s.DOMWidgetModel.serializers), d.model_name = "BioImageViewerModel", d.view_name = "BioImageViewerView";
+            u.model_module = o, u.model_module_version = r, u.view_module = o, u.view_module_version = r, u.serializers = Object.assign({}, s.DOMWidgetModel.serializers), u.model_name = "BioImageViewerModel", u.view_name = "BioImageViewerView";
             class p extends s.DOMWidgetView {
                 constructor() {
                     super(...arguments), this.values = this.model.get("value")
                 }
                 render() {
                     const e = document.createElement("div");
-                    this.el.appendChild(e), u()({
+                    this.el.appendChild(e), d()({
                         rootElement: e,
                         apiKey: this.values.token,
                         groupID: this.values.groupID,
                         namespace: this.values.namespace
                     })
                 }
             }
-            const m = {
+            const c = {
                 id: "@tiledb-inc/jupyter-bioimage-viewer",
                 autoStart: !0,
                 requires: [s.IJupyterWidgetRegistry],
                 activate: function(e, i) {
                     i.registerWidget({
                         name: o,
                         version: r,
                         exports: l
                     })
                 }
             }
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.1-alpha.6","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.0-alpha.7"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js"}}')
+            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.1-alpha.7","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.0-alpha.7"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"resolutions":{"@luma.gl/constants":"^8.5.16","@deck.gl/aggregation-layers":"^8.8.12","@deck.gl/core":"^8.8.12","@deck.gl/carto":"^8.8.12","@deck.gl/extensions":"^8.8.12","@deck.gl/geo-layers":"^8.8.12","@deck.gl/google-maps":"^8.8.12","@deck.gl/mapbox":"^8.8.12","@deck.gl/json":"^8.8.12","@deck.gl/layers":"^8.8.12","@deck.gl/mesh-layers":"^8.8.12","@deck.gl/react":"^8.8.12"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js"}}')
         }
     }
 ]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/remoteEntry.7d8ec031bffcf5f758ea.js` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/remoteEntry.5cdbd27cab7657a97979.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, i, o, d, l, u, s, f, c, p, h, b, v, m, g, y = {
+    var e, r, t, a, n, i, o, d, l, u, s, c, f, p, h, b, v, m, g, y = {
             5290: (e, r, t) => {
                 var a = {
                         "./index": () => t.e(744).then((() => () => t(1744))),
                         "./extension": () => t.e(744).then((() => () => t(1744))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -48,28 +48,28 @@
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         38: "06c00f555d53e8ae5aa5",
         172: "6267f3dd3063477e34ed",
         344: "8db93920a8ca0f0600d9",
         446: "3bf34f45c93ace9c0f28",
-        633: "770b26571c8b948a69e3",
-        635: "024275f22a135fe53126",
+        633: "1125117a0017a3fcb647",
+        635: "812cb387a85b4a4dd127",
         713: "44bebcfa12a45c30ff83",
-        744: "29f5fc192fc8171f023f",
+        744: "ca2ab2033fd1289054ea",
         747: "433530952542f03ebc71"
     } [e] + ".js?v=" + {
         38: "06c00f555d53e8ae5aa5",
         172: "6267f3dd3063477e34ed",
         344: "8db93920a8ca0f0600d9",
         446: "3bf34f45c93ace9c0f28",
-        633: "770b26571c8b948a69e3",
-        635: "024275f22a135fe53126",
+        633: "1125117a0017a3fcb647",
+        635: "812cb387a85b4a4dd127",
         713: "44bebcfa12a45c30ff83",
-        744: "29f5fc192fc8171f023f",
+        744: "ca2ab2033fd1289054ea",
         747: "433530952542f03ebc71"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -88,24 +88,24 @@
                     var s = l[u];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
                         o = s;
                         break
                     }
                 }
             o || (d = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, j.nc && o.setAttribute("nonce", j.nc), o.setAttribute("data-webpack", r + n), o.src = t), e[t] = [a];
-            var f = (r, a) => {
-                    o.onerror = o.onload = null, clearTimeout(c);
+            var c = (r, a) => {
+                    o.onerror = o.onload = null, clearTimeout(f);
                     var n = e[t];
                     if (delete e[t], o.parentNode && o.parentNode.removeChild(o), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                f = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: o
                 }), 12e4);
-            o.onerror = f.bind(null, o.onerror), o.onload = f.bind(null, o.onload), d && document.head.appendChild(o)
+            o.onerror = c.bind(null, o.onerror), o.onload = c.bind(null, o.onload), d && document.head.appendChild(o)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -127,15 +127,15 @@
                         (!d || !d.loaded && (!a != !d.eager ? a : o > d.from)) && (n[r] = {
                             get: t,
                             from: o,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (d("@jupyter-widgets/base", "4.1.1", (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))), d("@tiledb-inc/bioimage-viewer", "0.1.0-alpha.7", (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.1-alpha.6", (() => j.e(744).then((() => () => j(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@jupyter-widgets/base", "4.1.1", (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))), d("@tiledb-inc/bioimage-viewer", "0.1.0-alpha.7", (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.1-alpha.7", (() => j.e(744).then((() => () => j(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -185,63 +185,63 @@
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var o = 0, d = 1, l = !0;; d++, o++) {
-                var u, s, f = d < e.length ? (typeof e[d])[0] : "";
-                if (o >= r.length || "o" == (s = (typeof(u = r[o]))[0])) return !l || ("u" == f ? d > a && !n : "" == f != n);
+                var u, s, c = d < e.length ? (typeof e[d])[0] : "";
+                if (o >= r.length || "o" == (s = (typeof(u = r[o]))[0])) return !l || ("u" == c ? d > a && !n : "" == c != n);
                 if ("u" == s) {
-                    if (!l || "u" != f) return !1
+                    if (!l || "u" != c) return !1
                 } else if (l)
-                    if (f == s)
+                    if (c == s)
                         if (d <= a) {
                             if (u != e[d]) return !1
                         } else {
                             if (n ? u > e[d] : u < e[d]) return !1;
                             u != e[d] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != c && "n" != c) {
                     if (n || d <= a) return !1;
                     l = !1, d--
                 } else {
-                    if (d <= a || s < f != n) return !1;
+                    if (d <= a || s < c != n) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, d--)
+                } else "s" != c && "n" != c && (l = !1, d--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var f = [],
+            p = f.pop.bind(f);
         for (o = 1; o < e.length; o++) {
             var h = e[o];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
+            f.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
         }
         return !!p()
     }, o = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", u = (e, r, t, a) => {
         var n = d(e, t);
-        return i(a, n) || f(l(e, t, n, a)), c(e[t][n])
+        return i(a, n) || c(l(e, t, n, a)), f(e[t][n])
     }, s = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !i(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, f = e => {
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
+    }, f = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
         var i = j.I(r);
         return i && i.then ? i.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
     })(((e, r, t, a) => (o(e, t), u(r, 0, t, a)))), b = p(((e, r, t, a, n) => {
         var i = r && j.o(r, t) && s(r, t, a);
-        return i ? c(i) : n()
+        return i ? f(i) : n()
     })), v = {}, m = {
         2832: () => b("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 0, , "alpha", 7], (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))),
         8233: () => b("default", "@jupyter-widgets/base", [, [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1
         ], (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))),
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg/render.py` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg/render.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg.egg-info/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-jupyter-bioimg
-Version: 0.1.1a6
+Version: 0.1.1a7
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tiledb_jupyter_bioimg.egg-info/SOURCES.txt` & `tiledb_jupyter_bioimg-0.1.1a7/tiledb_jupyter_bioimg.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 tiledb_jupyter_bioimg.egg-info/top_level.txt
 tiledb_jupyter_bioimg/labextension/package.json
 tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
 tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
 tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js
 tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
-tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js
-tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js
-tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt
+tiledb_jupyter_bioimg/labextension/static/633.1125117a0017a3fcb647.js
+tiledb_jupyter_bioimg/labextension/static/635.812cb387a85b4a4dd127.js
+tiledb_jupyter_bioimg/labextension/static/635.812cb387a85b4a4dd127.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
 tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/744.29f5fc192fc8171f023f.js
+tiledb_jupyter_bioimg/labextension/static/744.ca2ab2033fd1289054ea.js
 tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
-tiledb_jupyter_bioimg/labextension/static/remoteEntry.7d8ec031bffcf5f758ea.js
+tiledb_jupyter_bioimg/labextension/static/remoteEntry.5cdbd27cab7657a97979.js
 tiledb_jupyter_bioimg/labextension/static/style.js
 tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a6/tsconfig.json` & `tiledb_jupyter_bioimg-0.1.1a7/tsconfig.json`

 * *Files identical despite different names*

