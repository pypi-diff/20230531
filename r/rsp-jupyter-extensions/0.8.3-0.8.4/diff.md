# Comparing `tmp/rsp_jupyter_extensions-0.8.3.tar.gz` & `tmp/rsp_jupyter_extensions-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsp_jupyter_extensions-0.8.3.tar", last modified: Fri May 26 22:44:57 2023, max compression
+gzip compressed data, was "rsp_jupyter_extensions-0.8.4.tar", last modified: Tue May 30 22:31:38 2023, max compression
```

## Comparing `rsp_jupyter_extensions-0.8.3.tar` & `rsp_jupyter_extensions-0.8.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.054662 rsp_jupyter_extensions-0.8.3/
--rw-r--r--   0 adam       (501) staff       (20)     1068 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)      480 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)     3949 2023-05-26 22:44:57.054331 rsp_jupyter_extensions-0.8.3/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     3072 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/README.md
--rw-r--r--   0 adam       (501) staff       (20)     1146 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/RELEASE.md
--rw-r--r--   0 adam       (501) staff       (20)      205 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/install.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.029961 rsp_jupyter_extensions-0.8.3/jupyter-config/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.037867 rsp_jupyter_extensions-0.8.3/jupyter-config/nb-config/
--rw-r--r--   0 adam       (501) staff       (20)       99 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/jupyter-config/nb-config/rsp_jupyter_extensions.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.038308 rsp_jupyter_extensions-0.8.3/jupyter-config/server-config/
--rw-r--r--   0 adam       (501) staff       (20)       97 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/jupyter-config/server-config/rsp_jupyter_extensions.json
--rw-r--r--   0 adam       (501) staff       (20)     3052 2023-05-26 22:31:06.000000 rsp_jupyter_extensions-0.8.3/package.json
--rw-r--r--   0 adam       (501) staff       (20)      915 2023-05-26 21:43:44.000000 rsp_jupyter_extensions-0.8.3/pyproject.toml
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.041835 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/
--rw-r--r--   0 adam       (501) staff       (20)      699 2021-09-15 20:02:14.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     2218 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/environment.py
--rw-r--r--   0 adam       (501) staff       (20)     2311 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/execution.py
--rw-r--r--   0 adam       (501) staff       (20)      916 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/handlers.py
--rw-r--r--   0 adam       (501) staff       (20)     1573 2021-09-15 20:02:14.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/hub.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.044893 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/
--rw-r--r--   0 adam       (501) staff       (20)     3194 2023-05-26 21:53:39.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/package.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.048391 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/
--rw-r--r--   0 adam       (501) staff       (20)     6154 2023-05-26 21:53:39.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/360.fc403a4ceb567571372e.js
--rw-r--r--   0 adam       (501) staff       (20)     3377 2023-05-26 21:53:39.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/747.b57adabf32495ac79fb2.js
--rw-r--r--   0 adam       (501) staff       (20)     6866 2023-05-26 21:53:39.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/remoteEntry.ba7b3ca42c9aa9705c93.js
--rw-r--r--   0 adam       (501) staff       (20)      165 2023-05-26 21:53:38.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/style.js
--rw-r--r--   0 adam       (501) staff       (20)     2452 2023-05-26 21:53:39.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/third-party-licenses.json
--rw-r--r--   0 adam       (501) staff       (20)     3298 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/query.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.048897 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/templates/
--rw-r--r--   0 adam       (501) staff       (20)     2735 2022-09-16 20:51:36.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/templates/portal_query.ipynb.template
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.044528 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     3949 2023-05-26 22:44:56.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     1306 2023-05-26 22:44:56.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-05-26 22:44:56.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2021-09-22 18:31:11.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)       41 2023-05-26 22:44:56.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       23 2023-05-26 22:44:56.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-05-26 22:44:57.054752 rsp_jupyter_extensions-0.8.3/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     3120 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/setup.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.052634 rsp_jupyter_extensions-0.8.3/src/
--rw-r--r--   0 adam       (501) staff       (20)     1577 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/src/DisplayLabVersion.tsx
--rw-r--r--   0 adam       (501) staff       (20)     4015 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.3/src/displayversion.ts
--rw-r--r--   0 adam       (501) staff       (20)     1420 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/src/index.ts
--rw-r--r--   0 adam       (501) staff       (20)     5503 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/src/query.ts
--rw-r--r--   0 adam       (501) staff       (20)     4737 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/src/savequit.ts
--rw-r--r--   0 adam       (501) staff       (20)      304 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/src/tokens.ts
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.053831 rsp_jupyter_extensions-0.8.3/style/
--rw-r--r--   0 adam       (501) staff       (20)        0 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/style/base.css
--rw-r--r--   0 adam       (501) staff       (20)       25 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/style/index.css
--rw-r--r--   0 adam       (501) staff       (20)       21 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/style/index.js
--rw-r--r--   0 adam       (501) staff       (20)      580 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.3/tsconfig.json
--rw-r--r--   0 adam       (501) staff       (20)   203643 2023-05-26 21:35:08.000000 rsp_jupyter_extensions-0.8.3/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:31:38.035110 rsp_jupyter_extensions-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-30 22:31:38.035110 rsp_jupyter_extensions-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:31:38.027110 rsp_jupyter_extensions-0.8.4/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:31:38.031110 rsp_jupyter_extensions-0.8.4/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/jupyter-config/nb-config/rsp_jupyter_extensions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:31:38.031110 rsp_jupyter_extensions-0.8.4/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/jupyter-config/server-config/rsp_jupyter_extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:31:38.031110 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:31:38.031110 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-30 22:31:37.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:31:38.031110 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-30 22:31:37.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/static/360.fc403a4ceb567571372e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-30 22:31:37.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/static/747.b57adabf32495ac79fb2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-30 22:31:37.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/static/remoteEntry.2387dea3163aed71b036.js
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-30 22:31:36.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-30 22:31:37.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:31:38.031110 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/templates/portal_query.ipynb.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:31:38.031110 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-30 22:31:37.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-30 22:31:38.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:31:37.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:30:53.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-30 22:31:37.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 22:31:37.000000 rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:31:38.035110 rsp_jupyter_extensions-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:31:38.035110 rsp_jupyter_extensions-0.8.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/src/DisplayLabVersion.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/src/displayversion.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/src/query.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/src/savequit.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/src/tokens.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:31:38.035110 rsp_jupyter_extensions-0.8.4/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-30 22:30:17.000000 rsp_jupyter_extensions-0.8.4/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)   203645 2023-05-30 22:31:26.000000 rsp_jupyter_extensions-0.8.4/yarn.lock
```

### Comparing `rsp_jupyter_extensions-0.8.3/LICENSE` & `rsp_jupyter_extensions-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/PKG-INFO` & `rsp_jupyter_extensions-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsp_jupyter_extensions
-Version: 0.8.3
+Version: 0.8.4
 Summary: Jupyter Extensions for the RSP
 Home-page: https://github.com/lsst-sqre/rsp-jupyter-extensions
 Author: Adam Thornton
 Author-email: athornton@lsst.org
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `rsp_jupyter_extensions-0.8.3/README.md` & `rsp_jupyter_extensions-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/RELEASE.md` & `rsp_jupyter_extensions-0.8.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/package.json` & `rsp_jupyter_extensions-0.8.4/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.8.4'"}*

```diff
@@ -97,9 +97,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.3"
+    "version": "0.8.4"
 }
```

### Comparing `rsp_jupyter_extensions-0.8.3/pyproject.toml` & `rsp_jupyter_extensions-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/__init__.py` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/environment.py` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/environment.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/execution.py` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/execution.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/handlers.py` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/handlers.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/hub.py` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/hub.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/package.json` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9757936507936508%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.2387dea3163aed71b036.js'}}",*

 * * "'version'": "'0.8.4'"}*

```diff
@@ -47,15 +47,15 @@
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ba7b3ca42c9aa9705c93.js",
+            "load": "static/remoteEntry.2387dea3163aed71b036.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/statusbar-extension:mode-switch"
         ],
         "discovery": {
             "server": {
@@ -102,9 +102,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.1"
+    "version": "0.8.4"
 }
```

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/360.fc403a4ceb567571372e.js` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/static/360.fc403a4ceb567571372e.js`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/747.b57adabf32495ac79fb2.js` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/static/747.b57adabf32495ac79fb2.js`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/remoteEntry.ba7b3ca42c9aa9705c93.js` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/static/remoteEntry.2387dea3163aed71b036.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, b = {
-            309: (e, r, t) => {
+            287: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(360).then((() => () => t(360))),
                         "./extension": () => t.e(360).then((() => () => t(360))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => m.e(360).then((() => () => m(360))),
                         from: i,
                         eager: !1
                     })
-                })("rsp-jupyter-extensions", "0.8.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("rsp-jupyter-extensions", "0.8.4"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -273,10 +273,10 @@
                     u && u(m)
                 }
                 for (r && r(t); l < a.length; l++) o = a[l], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkrsp_jupyter_extensions = self.webpackChunkrsp_jupyter_extensions || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), m.nc = void 0;
-    var y = m(309);
+    var y = m(287);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["rsp-jupyter-extensions"] = y
 })();
```

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/third-party-licenses.json` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/query.py` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/query.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/templates/portal_query.ipynb.template` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions/templates/portal_query.ipynb.template`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/PKG-INFO` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsp-jupyter-extensions
-Version: 0.8.3
+Version: 0.8.4
 Summary: Jupyter Extensions for the RSP
 Home-page: https://github.com/lsst-sqre/rsp-jupyter-extensions
 Author: Adam Thornton
 Author-email: athornton@lsst.org
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/SOURCES.txt` & `rsp_jupyter_extensions-0.8.4/rsp_jupyter_extensions.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 rsp_jupyter_extensions.egg-info/dependency_links.txt
 rsp_jupyter_extensions.egg-info/not-zip-safe
 rsp_jupyter_extensions.egg-info/requires.txt
 rsp_jupyter_extensions.egg-info/top_level.txt
 rsp_jupyter_extensions/labextension/package.json
 rsp_jupyter_extensions/labextension/static/360.fc403a4ceb567571372e.js
 rsp_jupyter_extensions/labextension/static/747.b57adabf32495ac79fb2.js
-rsp_jupyter_extensions/labextension/static/remoteEntry.ba7b3ca42c9aa9705c93.js
+rsp_jupyter_extensions/labextension/static/remoteEntry.2387dea3163aed71b036.js
 rsp_jupyter_extensions/labextension/static/style.js
 rsp_jupyter_extensions/labextension/static/third-party-licenses.json
 rsp_jupyter_extensions/templates/portal_query.ipynb.template
 src/DisplayLabVersion.tsx
 src/displayversion.ts
 src/index.ts
 src/query.ts
```

### Comparing `rsp_jupyter_extensions-0.8.3/setup.py` & `rsp_jupyter_extensions-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/src/DisplayLabVersion.tsx` & `rsp_jupyter_extensions-0.8.4/src/DisplayLabVersion.tsx`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/src/displayversion.ts` & `rsp_jupyter_extensions-0.8.4/src/displayversion.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/src/index.ts` & `rsp_jupyter_extensions-0.8.4/src/index.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/src/query.ts` & `rsp_jupyter_extensions-0.8.4/src/query.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/src/savequit.ts` & `rsp_jupyter_extensions-0.8.4/src/savequit.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/tsconfig.json` & `rsp_jupyter_extensions-0.8.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.3/yarn.lock` & `rsp_jupyter_extensions-0.8.4/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
   integrity sha512-u7stbOuYjaPezCuLj29hNW1v64M2Md2qupEKP1fHc7WdOA3DgLh37suiSrZYY7haUB7iBeQZ9P1uiRF359do3g==
   dependencies:
     "@babel/helper-validator-identifier" "^7.18.6"
     chalk "^2.0.0"
     js-tokens "^4.0.0"
 
 "@babel/runtime@^7.1.2":
-  version "7.22.0"
-  resolved "https://registry.yarnpkg.com/@babel/runtime/-/runtime-7.22.0.tgz#b7ca53ae391c404037540724186038afd83e26f9"
-  integrity sha512-TT6NB0oszYQ4oxLNUdG+FNHIc3MohXVCKA2BeyQ4WeM2VCSC6wBZ6P0Yfkdzxv+87D8Xk0LJyHeCKlWMvpZt0g==
+  version "7.22.3"
+  resolved "https://registry.yarnpkg.com/@babel/runtime/-/runtime-7.22.3.tgz#0a7fce51d43adbf0f7b517a71f4c3aaca92ebcbb"
+  integrity sha512-XsDuspWKLUsxwCp6r7EhsExHtYfbe5oAGQ19kqngTdCPUoPQzOPdUbD/pB9PJiwb2ptYKQDjSJT3R6dC+EPqfQ==
   dependencies:
     regenerator-runtime "^0.13.11"
 
 "@blueprintjs/colors@^4.0.0-alpha.3":
   version "4.2.1"
   resolved "https://registry.yarnpkg.com/@blueprintjs/colors/-/colors-4.2.1.tgz#603b2512caee84feddcb3dbd536534c140b9a1f3"
   integrity sha512-Cx7J2YnUuxn+fi+y5XtXnBB7+cFHN4xBrRkaAetp78i3VTCXjUk+d1omrOr8TqbRucUXTdrhbZOUHpzRLFcJpQ==
@@ -421,17 +421,17 @@
     "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/widgets" "^1.37.2"
 
 "@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15":
-  version "4.0.0"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-4.0.0.tgz#0a22a286fbf9cb7b981aa848091caa1305fc5169"
-  integrity sha512-9jqM4MqKcEoLoXZkMBJOPNco0mmmV3IsKYtrQkFRMm6eeYd7xdBsfKCkfvN8msOfyJUgfxXw1RrQA5sLII7g7w==
+  version "4.0.1"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-4.0.1.tgz#c6ef43c50e27deca7e7e86e4324ff1a552877944"
+  integrity sha512-uQHr54cBXhQgDMhYD39+xErZNr04xCOk936reXPiLBmJL9B855+nNRN0ls8Lmach3czWYNJ3XP+lZG+xUZ/uPw==
   dependencies:
     "@lumino/coreutils" "^2.1.1"
 
 "@jupyterlab/nbformat@^3.6.3":
   version "3.6.3"
   resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.3.tgz#8520338e3679cbe8ce2ea8eb5a9b816f8b774ad3"
   integrity sha512-0qJLa4dtOmu9EmHFeM7gaZi4qheovIPc9ZrgGGRuG0obajs4YYlvh4MQvCSgpVhme4AuBfGlcfzhlx+Gbzr5Xw==
@@ -446,17 +446,17 @@
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
 
 "@jupyterlab/rendermime-interfaces@^3.6.3":
-  version "3.8.0"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.8.0.tgz#5e8a8f558df5a66325f14a568a2ebedb9095410a"
-  integrity sha512-a+5AABK99DxunPBDIEPWFO2cXT3UqghQ75/k7+9QV0Bf3pqGMzHe5fSk2ZBDeQ+gvTT88yYlL7oxzjzbGzU0Lw==
+  version "3.8.1"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.8.1.tgz#7a4305802f66c2b41cfd0560977b0e21b73d376e"
+  integrity sha512-n5XN9UWIgJM9xt4Sua8atG3wPyZTtauDZ50PgemXD3z6YQcflXONkGh0g1Uykd3X1WoBhHoFcxTId1BtBxgVLQ==
   dependencies:
     "@lumino/coreutils" "^2.1.1"
     "@lumino/widgets" "^2.1.1"
 
 "@jupyterlab/rendermime@^3.6.3":
   version "3.6.3"
   resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.6.3.tgz#48d83c70493b0356d4dac6d89a863d8a5a84f68e"
@@ -1327,22 +1327,22 @@
   version "3.0.2"
   resolved "https://registry.yarnpkg.com/braces/-/braces-3.0.2.tgz#3454e1a462ee8d599e236df336cd9ea4f8afe107"
   integrity sha512-b8um+L1RzM3WDSzvhm6gIz1yfTbBt6YTlcEKAvsmqCZZFw46z626lVj9j1yEPW33H5H+lBQpZMP1k8l+78Ha0A==
   dependencies:
     fill-range "^7.0.1"
 
 browserslist@^4.14.5:
-  version "4.21.5"
-  resolved "https://registry.yarnpkg.com/browserslist/-/browserslist-4.21.5.tgz#75c5dae60063ee641f977e00edd3cfb2fb7af6a7"
-  integrity sha512-tUkiguQGW7S3IhB7N+c2MV/HZPSCPAAiYBZXLsBhFB/PCy6ZKKsZrmBayHV9fdGV/ARIfJ14NkxKzRDjvp7L6w==
-  dependencies:
-    caniuse-lite "^1.0.30001449"
-    electron-to-chromium "^1.4.284"
-    node-releases "^2.0.8"
-    update-browserslist-db "^1.0.10"
+  version "4.21.7"
+  resolved "https://registry.yarnpkg.com/browserslist/-/browserslist-4.21.7.tgz#e2b420947e5fb0a58e8f4668ae6e23488127e551"
+  integrity sha512-BauCXrQ7I2ftSqd2mvKHGo85XR0u7Ru3C/Hxsy/0TkfCtjrmAbPdzLGasmoiBxplpDXlPvdjX9u7srIMfgasNA==
+  dependencies:
+    caniuse-lite "^1.0.30001489"
+    electron-to-chromium "^1.4.411"
+    node-releases "^2.0.12"
+    update-browserslist-db "^1.0.11"
 
 buffer-from@^1.0.0:
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/buffer-from/-/buffer-from-1.1.2.tgz#2b146a6fd72e80b4f55d255f35ed59a3a9a41bd5"
   integrity sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==
 
 buffer@^5.5.0, buffer@^5.6.0:
@@ -1386,18 +1386,18 @@
     get-intrinsic "^1.0.2"
 
 callsites@^3.0.0:
   version "3.1.0"
   resolved "https://registry.yarnpkg.com/callsites/-/callsites-3.1.0.tgz#b3630abd8943432f54b3f0519238e33cd7df2f73"
   integrity sha512-P8BjAsXvZS+VIDUI11hHCQEv74YT67YUi5JJFNWIqL235sBmjX4+qx9Muvls5ivyNENctx46xQLQ3aTuE7ssaQ==
 
-caniuse-lite@^1.0.30001449:
-  version "1.0.30001489"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001489.tgz#ca82ee2d4e4dbf2bd2589c9360d3fcc2c7ba3bd8"
-  integrity sha512-x1mgZEXK8jHIfAxm+xgdpHpk50IN3z3q3zP261/WS+uvePxW8izXuCu6AHz0lkuYTlATDehiZ/tNyYBdSQsOUQ==
+caniuse-lite@^1.0.30001489:
+  version "1.0.30001491"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001491.tgz#eab0e0f392de6f7411751d148de9b5bd6b203e46"
+  integrity sha512-17EYIi4TLnPiTzVKMveIxU5ETlxbSO3B6iPvMbprqnKh4qJsQGk5Nh1Lp4jIMAE0XfrujsJuWZAM3oJdMHaKBA==
 
 chalk@^2.0.0, chalk@^2.3.0, chalk@^2.4.1:
   version "2.4.2"
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
   integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
   dependencies:
     ansi-styles "^3.2.1"
@@ -1701,18 +1701,18 @@
     semver "^5.4.1"
 
 eastasianwidth@^0.2.0:
   version "0.2.0"
   resolved "https://registry.yarnpkg.com/eastasianwidth/-/eastasianwidth-0.2.0.tgz#696ce2ec0aa0e6ea93a397ffcf24aa7840c827cb"
   integrity sha512-I88TYZWc9XiYHRQ4/3c5rjjfgkjhLyW2luGIheGERbNQ6OY7yTybanSpDXZa8y7VUP9YmDcYa+eyq4ca7iLqWA==
 
-electron-to-chromium@^1.4.284:
-  version "1.4.409"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.409.tgz#33b6d83d83c2e76c3b1c1b90614147e50cc9065f"
-  integrity sha512-+2mRCBG9dR66sprh2dLuO6vr+O1xqHXvhmMglfut3OmfeUVRUho2nZYxxD9pG6G4PLDkZeqhlA/Gk6LpjVSHag==
+electron-to-chromium@^1.4.411:
+  version "1.4.414"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.414.tgz#f9eedb6fb01b50439d8228d8ee3a6fa5e0108437"
+  integrity sha512-RRuCvP6ekngVh2SAJaOKT/hxqc9JAsK+Pe0hP5tGQIfonU2Zy9gMGdJ+mBdyl/vNucMG6gkXYtuM4H/1giws5w==
 
 emoji-regex@^8.0.0:
   version "8.0.0"
   resolved "https://registry.yarnpkg.com/emoji-regex/-/emoji-regex-8.0.0.tgz#e818fd69ce5ccfcb404594f842963bf53164cc37"
   integrity sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==
 
 emoji-regex@^9.2.2:
@@ -2786,17 +2786,17 @@
   resolved "https://registry.yarnpkg.com/levn/-/levn-0.4.1.tgz#ae4562c007473b932a6200d403268dd2fffc6ade"
   integrity sha512-+bT2uH4E5LGE7h/n3evcS/sQlJXCpIp6ym8OWJ5eV6+67Dsql/LaaT7qJBAt2rzfoa/5QBGBhxDix1dMt2kQKQ==
   dependencies:
     prelude-ls "^1.2.1"
     type-check "~0.4.0"
 
 lib0@^0.2.31, lib0@^0.2.42, lib0@^0.2.52, lib0@^0.2.74:
-  version "0.2.76"
-  resolved "https://registry.yarnpkg.com/lib0/-/lib0-0.2.76.tgz#d2b7db3849bb3c4817387a91cf421c4a921d3e0c"
-  integrity sha512-JUJgbBIBQ+SODonRikV/XWpWSPqagwdr7jZ6DXqB8rdP1QQwoKZD0jfC0yqefdvUERFy2i9wVb1v9uR+cvZPuA==
+  version "0.2.78"
+  resolved "https://registry.yarnpkg.com/lib0/-/lib0-0.2.78.tgz#9aa34733075caafb3edf228da6e609d15ada0088"
+  integrity sha512-SV2nU43/6eaYnGH3l0lg2wg1ziB/TH3sAd2E8quXPGwrqo+aX98SNT2ZKucpUr5B8A52jD7ZMjAl+r87Fa/bLQ==
   dependencies:
     isomorphic.js "^0.2.4"
 
 license-webpack-plugin@^2.3.14:
   version "2.3.21"
   resolved "https://registry.yarnpkg.com/license-webpack-plugin/-/license-webpack-plugin-2.3.21.tgz#152f5e82d5f51f8bab78905731f2b8042aa5691b"
   integrity sha512-rVaYU9TddZN3ao8M/0PrRSCdTp2EW6VQymlgsuScld1vef0Ou7fALx3ePe83KLP3xAEDcPK5fkqUVqGBnbz1zQ==
@@ -3062,15 +3062,15 @@
     whatwg-url "^5.0.0"
 
 node-gyp-build@~4.1.0:
   version "4.1.1"
   resolved "https://registry.yarnpkg.com/node-gyp-build/-/node-gyp-build-4.1.1.tgz#d7270b5d86717068d114cc57fff352f96d745feb"
   integrity sha512-dSq1xmcPDKPZ2EED2S6zw/b9NKsqzXRE6dVr8TVQnI3FJOTteUMuqF3Qqs6LZg+mLGYJWqQzMbIjMtJqTv87nQ==
 
-node-releases@^2.0.8:
+node-releases@^2.0.12:
   version "2.0.12"
   resolved "https://registry.yarnpkg.com/node-releases/-/node-releases-2.0.12.tgz#35627cc224a23bfb06fb3380f2b3afaaa7eb1039"
   integrity sha512-QzsYKWhXTWx8h1kIvqfnC++o0pEmpRQA/aenALsL2F4pqNVr7YzcdMlDij5WBnwftRbJCNJL/O7zdKaxKPHqgQ==
 
 normalize-package-data@^2.3.2:
   version "2.5.0"
   resolved "https://registry.yarnpkg.com/normalize-package-data/-/normalize-package-data-2.5.0.tgz#e66db1838b200c1dfc233225d12cb36520e234a8"
@@ -3326,17 +3326,17 @@
 
 postcss-value-parser@^4.1.0:
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz#723c09920836ba6d3e5af019f92bc0971c02e514"
   integrity sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==
 
 postcss@^8.2.15, postcss@^8.3.11:
-  version "8.4.23"
-  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.23.tgz#df0aee9ac7c5e53e1075c24a3613496f9e6552ab"
-  integrity sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==
+  version "8.4.24"
+  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.24.tgz#f714dba9b2284be3cc07dbd2fc57ee4dc972d2df"
+  integrity sha512-M0RzbcI0sO/XJNucsGjvWU9ERWxb/ytp1w6dKtxTKgixdtQDq4rmx/g8W1hnaheq9jgwL/oyEdH5Bc4WwJKMqg==
   dependencies:
     nanoid "^3.3.6"
     picocolors "^1.0.0"
     source-map-js "^1.0.2"
 
 prelude-ls@^1.2.1:
   version "1.2.1"
@@ -3869,17 +3869,17 @@
   version "6.0.1"
   resolved "https://registry.yarnpkg.com/strip-ansi/-/strip-ansi-6.0.1.tgz#9e26c63d30f53443e9489495b2105d37b67a85d9"
   integrity sha512-Y38VPSHcqkFrCpFnQ9vuSXmquuv5oXOKpGeT6aGrr3o3Gc9AlVa6JBfUSOCnbxGGZF+/0ooI7KrPuUSztUdU5A==
   dependencies:
     ansi-regex "^5.0.1"
 
 strip-ansi@^7.0.1:
-  version "7.0.1"
-  resolved "https://registry.yarnpkg.com/strip-ansi/-/strip-ansi-7.0.1.tgz#61740a08ce36b61e50e65653f07060d000975fb2"
-  integrity sha512-cXNxvT8dFNRVfhVME3JAe98mkXDYN2O1l7jmcwMnOslDeESg1rF/OZMtK0nRAhiari1unG5cD4jG3rapUAkLbw==
+  version "7.1.0"
+  resolved "https://registry.yarnpkg.com/strip-ansi/-/strip-ansi-7.1.0.tgz#d5b6568ca689d8561370b0707685d22434faff45"
+  integrity sha512-iq6eVVI64nQQTRYq2KtEg2d2uU7LElhTJwsH4YzIHZshxlgZms/wIc4VoDQTlG/IvVIrBKG06CrZnp0qv7hkcQ==
   dependencies:
     ansi-regex "^6.0.1"
 
 strip-bom@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/strip-bom/-/strip-bom-3.0.0.tgz#2334c18e9c759f7bdd56fdef7e9ae3d588e68ed3"
   integrity sha512-vavAMRXOgBVNF6nyEEmL3DBK19iRpDcoIwW+swQ+CbGiu7lju6t+JklA1MHweoWtadgt4ISVUsXLyDq34ddcwA==
@@ -4112,15 +4112,15 @@
     imurmurhash "^0.1.4"
 
 universalify@^2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/universalify/-/universalify-2.0.0.tgz#75a4984efedc4b08975c5aeb73f530d02df25717"
   integrity sha512-hAZsKq7Yy11Zu1DE0OzWjw7nnLZmJZYTDZZyEFHZdUhV8FkH5MCfoU1XMaxXovpyW5nq5scPqq0ZDP9Zyl04oQ==
 
-update-browserslist-db@^1.0.10:
+update-browserslist-db@^1.0.11:
   version "1.0.11"
   resolved "https://registry.yarnpkg.com/update-browserslist-db/-/update-browserslist-db-1.0.11.tgz#9a2a641ad2907ae7b3616506f4b977851db5b940"
   integrity sha512-dCwEFf0/oT85M1fHBg4F0jtLwJrutGoHSQXCh7u4o2t1drG+c0a9Flnqww6XUKSfQMPpJBRjU8d4RXB09qtvaA==
   dependencies:
     escalade "^3.1.1"
     picocolors "^1.0.0"
```

