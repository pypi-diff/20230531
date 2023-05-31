# Comparing `tmp/jupyverse_api-0.1.6.tar.gz` & `tmp/jupyverse_api-0.1.7.tar.gz`

## Comparing `jupyverse_api-0.1.6.tar` & `jupyverse_api-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/cli.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/README.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 jupyverse_api-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/README.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 jupyverse_api-0.1.7/PKG-INFO
```

### Comparing `jupyverse_api-0.1.6/jupyverse_api/cli.py` & `jupyverse_api-0.1.7/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/jupyverse_api/app/__init__.py` & `jupyverse_api-0.1.7/jupyverse_api/app/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,7 +45,10 @@
             if path in _paths:
                 raise RuntimeError(
                     f"{_type } mounts a path that is already defined in {_router}: {path}"
                 )
         self._router_paths[_type].append(path)
         logger.debug("%s mounted path: %s", _type, path)
         self._app.mount(path, *args, **kwargs)
+
+    def add_middleware(self, middleware, *args, **kwargs) -> None:
+        self._app.add_middleware(middleware, *args, **kwargs)
```

### Comparing `jupyverse_api-0.1.6/jupyverse_api/auth/__init__.py` & `jupyverse_api-0.1.7/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/jupyverse_api/contents/__init__.py` & `jupyverse_api-0.1.7/jupyverse_api/contents/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,20 @@
     async def get_path(self, file_id: str) -> str:
         ...
 
     @abstractmethod
     async def get_id(self, file_path: str) -> str:
         ...
 
+    def watch(self, path: str):
+        ...
+
+    def unwatch(self, path: str, watcher):
+        ...
+
 
 class Contents(Router, ABC):
     def __init__(self, app: App, auth: Auth):
         super().__init__(app=app)
 
         router = APIRouter()
```

### Comparing `jupyverse_api-0.1.6/jupyverse_api/contents/models.py` & `jupyverse_api-0.1.7/jupyverse_api/contents/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class Content(BaseModel):
     name: str
     path: str
     last_modified: Optional[str]
     created: Optional[str]
-    content: Optional[Union[str, Dict, List[Dict]]]
+    content: Optional[Union[List[Dict], str, Dict]]
     format: Optional[str]
     mimetype: Optional[str]
     size: Optional[int]
     writable: bool
     type: str
```

### Comparing `jupyverse_api-0.1.6/jupyverse_api/jupyterlab/__init__.py` & `jupyverse_api-0.1.7/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/jupyverse_api/kernels/__init__.py` & `jupyverse_api-0.1.7/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/jupyverse_api/kernels/models.py` & `jupyverse_api-0.1.7/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/jupyverse_api/lab/__init__.py` & `jupyverse_api-0.1.7/jupyverse_api/lab/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ..auth import Auth, User
 from ..app import App
 
 
 class Lab(Router, ABC):
     prefix_dir: Path
     jlab_dir: Path
+    labextensions_dir: Path
     extensions_dir: Path
     redirect_after_root: str
 
     def __init__(self, app: App, auth: Auth, jupyterlab_config: Optional[JupyterLabConfig]):
         super().__init__(app)
 
         self.prefix_dir = Path(sys.prefix)
@@ -32,14 +33,15 @@
             jlab_dev_mode = jupyterlab_config.dev_mode
         else:
             jlab_dev_mode = False
         if jlab_dev_mode:
             self.jlab_dir = Path(jupyterlab_module.__file__).parents[1] / "dev_mode"
         else:
             self.jlab_dir = self.prefix_dir / "share" / "jupyter" / "lab"
+        self.labextensions_dir = self.prefix_dir / "share" / "jupyter" / "labextensions"
         for ext in self.federated_extensions:
             name = ext["name"]
             self.mount(
                 f"/lab/extensions/{name}/static",
                 StaticFiles(directory=self.extensions_dir / name / "static"),
                 name=name,
             )
```

### Comparing `jupyverse_api-0.1.6/jupyverse_api/main/__init__.py` & `jupyverse_api-0.1.7/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/jupyverse_api/nbconvert/__init__.py` & `jupyverse_api-0.1.7/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/jupyverse_api/resource_usage/__init__.py` & `jupyverse_api-0.1.7/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/jupyverse_api/retrolab/__init__.py` & `jupyverse_api-0.1.7/jupyverse_api/retrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/jupyverse_api/terminals/__init__.py` & `jupyverse_api-0.1.7/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/.gitignore` & `jupyverse_api-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/COPYING.md` & `jupyverse_api-0.1.7/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/pyproject.toml` & `jupyverse_api-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.6/PKG-INFO` & `jupyverse_api-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyverse_api
-Version: 0.1.6
+Version: 0.1.7
 Summary: The public API for Jupyverse
 Project-URL: Source, https://github.com/jupyter-server/jupyverse/jupyverse_api
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: api,jupyverse
 Classifier: Development Status :: 4 - Beta
```

