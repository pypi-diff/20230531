# Comparing `tmp/quiltplus-0.8.1.tar.gz` & `tmp/quiltplus-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltplus-0.8.1.tar", max compression
+gzip compressed data, was "quiltplus-0.9.0.tar", max compression
```

## Comparing `quiltplus-0.8.1.tar` & `quiltplus-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-03-01 19:37:11.440551 quiltplus-0.8.1/LICENSE.md
--rw-r--r--   0        0        0     1183 2023-03-02 00:44:34.769534 quiltplus-0.8.1/README.md
--rw-r--r--   0        0        0      842 2023-05-19 20:33:53.562381 quiltplus-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      821 2023-05-19 20:32:18.927042 quiltplus-0.8.1/quiltplus/__init__.py
--rw-r--r--   0        0        0     3258 2023-03-01 19:37:11.442886 quiltplus-0.8.1/quiltplus/cache.py
--rw-r--r--   0        0        0       36 2023-03-01 19:37:11.443193 quiltplus-0.8.1/quiltplus/cli/__init__.py
--rw-r--r--   0        0        0      612 2023-03-01 19:37:11.443370 quiltplus-0.8.1/quiltplus/cli/catalog.py
--rw-r--r--   0        0        0      237 2023-03-01 19:37:11.443620 quiltplus-0.8.1/quiltplus/cli/context.py
--rw-r--r--   0        0        0      927 2023-03-01 19:37:11.443833 quiltplus-0.8.1/quiltplus/cli/depend.py
--rw-r--r--   0        0        0     1168 2023-03-01 19:37:11.444170 quiltplus-0.8.1/quiltplus/cli/group.py
--rw-r--r--   0        0        0      665 2023-03-01 19:37:11.444406 quiltplus-0.8.1/quiltplus/cli/pkg.py
--rwxr-xr-x   0        0        0      127 2023-02-27 04:37:56.107220 quiltplus-0.8.1/quiltplus/cli/qp.py
--rw-r--r--   0        0        0     1009 2023-03-01 19:37:11.444736 quiltplus-0.8.1/quiltplus/cli/stage.py
--rw-r--r--   0        0        0     5712 2023-03-01 19:37:11.445107 quiltplus-0.8.1/quiltplus/config.py
--rw-r--r--   0        0        0     3227 2023-05-19 18:59:56.847388 quiltplus-0.8.1/quiltplus/id.py
--rw-r--r--   0        0        0      716 2023-03-01 19:37:11.446051 quiltplus-0.8.1/quiltplus/ignore.py
--rw-r--r--   0        0        0     5025 2023-05-19 18:59:56.848083 quiltplus-0.8.1/quiltplus/package.py
--rw-r--r--   0        0        0     1867 2023-05-19 18:59:56.848713 quiltplus-0.8.1/quiltplus/parse.py
--rw-r--r--   0        0        0      696 2023-05-19 18:59:56.848983 quiltplus-0.8.1/quiltplus/registry.py
--rw-r--r--   0        0        0      524 2023-05-19 20:33:14.589232 quiltplus-0.8.1/quiltplus/resource.py
--rw-r--r--   0        0        0      467 2023-05-19 18:59:56.849553 quiltplus-0.8.1/quiltplus/types.py
--rw-r--r--   0        0        0     1375 2023-05-19 17:22:44.235928 quiltplus-0.8.1/quiltplus/unparse.py
--rw-r--r--   0        0        0      779 2023-05-19 18:59:56.850051 quiltplus-0.8.1/quiltplus/versions.py
--rw-r--r--   0        0        0     2052 1970-01-01 00:00:00.000000 quiltplus-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-01 19:37:11.440551 quiltplus-0.9.0/LICENSE.md
+-rw-r--r--   0        0        0      668 2023-05-31 14:03:42.566191 quiltplus-0.9.0/README.md
+-rw-r--r--   0        0        0      837 2023-05-31 14:03:42.570360 quiltplus-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      631 2023-05-31 14:03:42.572187 quiltplus-0.9.0/quiltplus/__init__.py
+-rw-r--r--   0        0        0      716 2023-03-01 19:37:11.446051 quiltplus-0.9.0/quiltplus/ignore.py
+-rw-r--r--   0        0        0     2059 2023-05-31 14:03:42.573471 quiltplus-0.9.0/quiltplus/local.py
+-rw-r--r--   0        0        0     3805 2023-05-31 14:03:42.575123 quiltplus-0.9.0/quiltplus/package.py
+-rw-r--r--   0        0        0      457 2023-05-31 14:03:42.576091 quiltplus-0.9.0/quiltplus/path.py
+-rw-r--r--   0        0        0       80 2023-05-31 14:03:42.576780 quiltplus-0.9.0/quiltplus/property.py
+-rw-r--r--   0        0        0      593 2023-05-31 14:03:42.577524 quiltplus-0.9.0/quiltplus/registry.py
+-rw-r--r--   0        0        0      606 2023-05-31 14:03:42.578377 quiltplus-0.9.0/quiltplus/resource.py
+-rw-r--r--   0        0        0      366 2023-05-31 14:03:42.579049 quiltplus-0.9.0/quiltplus/root.py
+-rw-r--r--   0        0        0     1176 2023-05-31 14:03:42.579492 quiltplus-0.9.0/quiltplus/type.py
+-rw-r--r--   0        0        0     1483 2023-05-31 14:03:42.579909 quiltplus-0.9.0/quiltplus/uri.py
+-rw-r--r--   0        0        0      573 2023-05-31 14:03:42.580666 quiltplus-0.9.0/quiltplus/versions.py
+-rw-r--r--   0        0        0     1588 1970-01-01 00:00:00.000000 quiltplus-0.9.0/PKG-INFO
```

### Comparing `quiltplus-0.8.1/LICENSE.md` & `quiltplus-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quiltplus-0.8.1/pyproject.toml` & `quiltplus-0.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "quiltplus"
-version = "0.8.1"
+version = "0.9.0"
 description = "Resource-oriented Python API/CLI for Quilt's decentralized social knowledge platform"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["yaml", "api", "resource", "quilt"]
 packages = [
    { include = "quiltplus" }
 ]
 
-[tool.poetry.scripts]
-qp = "quiltplus.cli.qp:cli"
-
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
+urllib3 = "<2"
 quilt3 = "^5.1.0"
 trio = "^0.22.0"
 isort = "^5.12.0"
 asyncclick = "^8.1.3.4"
 pytest-cov = "^4.0.0"
-# anyio = "^3.6.1"
-# anyio = {git = "https://github.com/agronholm/anyio.git"}
-anyio = "^3.6.2"
+anyio = "^3.7.0"
 typing-extensions = "^4.5.0"
+un-yaml = ">0.0.0"
+# udc = {git = "https://github.com/data-yaml/udc.git", rev = "main"}
+tzlocal = "^5.0.1"
+
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 pytest-trio = "^0.8.0"
 pytest-watcher = "^0.2.6"
 
 [build-system]
```

### Comparing `quiltplus-0.8.1/quiltplus/__init__.py` & `quiltplus-0.9.0/quiltplus/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import yaml
 
-from .cache import QuiltIdCache  # NOQA F401
-from .cli import cli  # NOQA F401
-from .config import QuiltConfig  # NOQA F401
-from .id import QuiltID  # NOQA F401
 from .ignore import GitIgnore  # NOQA F401
+from .local import QuiltLocal  # NOQA F401
 from .package import QuiltPackage  # NOQA F401
-from .parse import (K_BKT, K_HSH, K_PKG, K_PRP, K_PTH,  # NOQA F401
-                             K_STR, K_VER, QuiltParse)
-from .resource import QuiltResource  # NOQA F401
 from .registry import QuiltRegistry  # NOQA F401
-from .unparse import QuiltUnparse  # NOQA F401
+from .resource import QuiltResource, QuiltResourceURI  # NOQA F401
+from .type import QuiltType  # NOQA F401
+from .uri import QuiltUri  # NOQA F401
 from .versions import QuiltVersions  # NOQA F401
 
 
 def default_representer(dumper, data):
     # Alternatively, use repr() instead of str():
     return dumper.represent_scalar("tag:yaml.org,2002:str", str(data))
```

### Comparing `quiltplus-0.8.1/quiltplus/ignore.py` & `quiltplus-0.9.0/quiltplus/ignore.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.8.1/quiltplus/registry.py` & `quiltplus-0.9.0/quiltplus/registry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from quilt3 import list_packages
-from typing_extensions import Self
 
-from .id import QuiltID
+from .root import QuiltRoot
 
 
-class QuiltRegistry:
+class QuiltRegistry(QuiltRoot):
     """Creates registry object from QuiltID."""
 
-    def __init__(self, id: QuiltID):
-        self.id = id
-        self.registry = id.registry()
+    def __init__(self, attrs: dict):
+        super().__init__(attrs)
+        self.attrs = attrs
 
     def __repr__(self):
         return f"QuiltRegistry({self.registry})"
 
-    def __eq__(self, other: Self):
-        return self.registry == other.registry
-
     def url(self, pkg: str):
         """Convert package name to URL."""
-        return self.id.quilt_uri() + f"#package={pkg}:latest"
+        return self.pkg_uri(pkg) + ":latest"
 
-    async def list(self):
+    async def list(self, opts: dict = {}):
         """List package URIs in registry."""
         return [self.url(pkg) for pkg in list_packages(self.registry)]
```

