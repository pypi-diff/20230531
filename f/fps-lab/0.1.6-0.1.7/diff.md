# Comparing `tmp/fps_lab-0.1.6.tar.gz` & `tmp/fps_lab-0.1.7.tar.gz`

## Comparing `fps_lab-0.1.6.tar` & `fps_lab-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_lab-0.1.6/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_lab-0.1.6/fps_lab/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fps_lab-0.1.6/fps_lab/main.py
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 fps_lab-0.1.6/fps_lab/routes.py
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 fps_lab-0.1.6/fps_lab/static/favicon.ico
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_lab-0.1.6/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_lab-0.1.6/COPYING.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fps_lab-0.1.6/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 fps_lab-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fps_lab-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_lab-0.1.7/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_lab-0.1.7/fps_lab/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fps_lab-0.1.7/fps_lab/main.py
+-rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 fps_lab-0.1.7/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 fps_lab-0.1.7/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_lab-0.1.7/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_lab-0.1.7/COPYING.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fps_lab-0.1.7/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 fps_lab-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fps_lab-0.1.7/PKG-INFO
```

### Comparing `fps_lab-0.1.6/fps_lab/main.py` & `fps_lab-0.1.7/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `fps_lab-0.1.6/fps_lab/routes.py` & `fps_lab-0.1.7/fps_lab/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -154,39 +154,47 @@
     ):
         settings = json.loads(user.settings)
         settings[f"{name0}:{name1}"] = await request.json()
         await user_update({"settings": json.dumps(settings)})
         return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
     async def get_settings(self, user: User):
-        with open(self.jlab_dir / "static" / "package.json") as f:
-            package = json.load(f)
         if user:
             user_settings = json.loads(user.settings)
         else:
             user_settings = {}
         settings = []
-        for path in (self.jlab_dir / "schemas" / "@jupyterlab").glob("*/*.json"):
-            with open(path) as f:
-                schema = json.load(f)
-            key = f"{path.parent.name}:{path.stem}"
-            setting = {
-                "id": f"@jupyterlab/{key}",
-                "schema": schema,
-                "version": package["version"],
-                "raw": "{}",
-                "settings": {},
-                "warning": None,
-                "last_modified": None,
-                "created": None,
-            }
-            if key in user_settings:
-                setting.update(user_settings[key])
-                setting["settings"] = json5.loads(user_settings[key]["raw"])
-            settings.append(setting)
+        schemas = [self.jlab_dir / "schemas"]
+        for d1 in self.labextensions_dir.iterdir():
+            if (d1 / "schemas").exists():
+                schemas.append(d1 / "schemas")
+            for d2 in d1.iterdir():
+                if (d2 / "schemas").exists():
+                    schemas.append(d2 / "schemas")
+        for s in schemas:
+            for d1 in s.iterdir():
+                for d2 in d1.iterdir():
+                    package = json.loads((d2 / "package.json.orig").read_text())
+                    for path in [p for p in d2.iterdir() if p.suffix == ".json"]:
+                        schema = json.loads(path.read_text())
+                        key = f"{path.parent.name}:{path.stem}"
+                        setting = {
+                            "id": f"{d1.name}/{key}",
+                            "schema": schema,
+                            "version": package["version"],
+                            "raw": "{}",
+                            "settings": {},
+                            "warning": None,
+                            "last_modified": None,
+                            "created": None,
+                        }
+                        if key in user_settings:
+                            setting.update(user_settings[key])
+                            setting["settings"] = json5.loads(user_settings[key]["raw"])
+                        settings.append(setting)
         return {"settings": settings}
 
     def get_federated_extensions(self, extensions_dir: Path) -> Tuple[List, List]:
         federated_extensions = []
         disabled_extensions = []
 
         for path in glob(os.path.join(extensions_dir, "**", "package.json"), recursive=True):
```

### Comparing `fps_lab-0.1.6/fps_lab/static/favicon.ico` & `fps_lab-0.1.7/fps_lab/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `fps_lab-0.1.6/.gitignore` & `fps_lab-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_lab-0.1.6/COPYING.md` & `fps_lab-0.1.7/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_lab-0.1.6/pyproject.toml` & `fps_lab-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_lab-0.1.6/PKG-INFO` & `fps_lab-0.1.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_lab
-Version: 0.1.6
+Version: 0.1.7
 Summary: An FPS plugin for the JupyterLab/RetroLab API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

