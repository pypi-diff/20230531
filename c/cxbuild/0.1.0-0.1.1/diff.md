# Comparing `tmp/cxbuild-0.1.0.tar.gz` & `tmp/cxbuild-0.1.1.tar.gz`

## Comparing `cxbuild-0.1.0.tar` & `cxbuild-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cxbuild-0.1.0/.gitmodules
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 cxbuild-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 cxbuild-0.1.0/CMakeLists.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cxbuild-0.1.0/requirements.txt
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cxbuild-0.1.0/.github/workflows/build_wheels.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cxbuild-0.1.0/.procure/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/__about__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/__init__.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/cmake_extension.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/cmake_tool.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/copyutils.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/cxbuild.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/extension_builder.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/project.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/project_base.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/pyproject.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/setup_tool.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/solution.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/tool.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/build_hooks/__init__.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 cxbuild-0.1.0/cxbuild/cli/__init__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 cxbuild-0.1.0/pkg/cxb_simple/CMakeLists.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cxbuild-0.1.0/pkg/cxb_simple/README.md
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 cxbuild-0.1.0/pkg/cxb_simple/pyproject.toml
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 cxbuild-0.1.0/pkg/cxb_simple/setup.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 cxbuild-0.1.0/pkg/cxb_simple/cxb_simple/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 cxbuild-0.1.0/pkg/cxb_simple/cxb_simple/__main__.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 cxbuild-0.1.0/pkg/cxb_simple/src/main.cpp
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cxbuild-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cxbuild-0.1.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 cxbuild-0.1.0/LICENSE
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cxbuild-0.1.0/README.md
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 cxbuild-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 cxbuild-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cxbuild-0.1.1/.gitmodules
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 cxbuild-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 cxbuild-0.1.1/CMakeLists.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cxbuild-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cxbuild-0.1.1/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cxbuild-0.1.1/.procure/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/__about__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/__init__.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/activity.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/backend.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/build_tool.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/cmake_extension.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/cmake_tool.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/copyutils.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/cxbuild.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/extension_builder.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/pip_tool.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/project.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/project_base.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/pyproject.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/setup_tool.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/solution.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/tool.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/cli/__init__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/README.md
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/pyproject.toml
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/setup.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/cxb_simple/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/cxb_simple/__main__.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/src/main.cpp
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cxbuild-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 cxbuild-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 cxbuild-0.1.1/LICENSE
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cxbuild-0.1.1/README.md
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 cxbuild-0.1.1/PKG-INFO
```

### Comparing `cxbuild-0.1.0/CMakeLists.txt` & `cxbuild-0.1.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.0/.github/workflows/build_wheels.yml` & `cxbuild-0.1.1/.github/workflows/build_wheels.yml`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.0/cxbuild/cmake_tool.py` & `cxbuild-0.1.1/cxbuild/cmake_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import dataclasses
 import sys, os
 import shutil
 from pathlib import Path
-import site
 
 from .tool import Tool
 
 
 class CMakeConfigError(Exception):
     """
     Something is misconfigured.
@@ -58,17 +57,16 @@
         if self.config.generator is not None:
             configure_args += [f'-G "{self.config.generator}"']
 
             if self.config.generator == "Ninja":
                 configure_args += [f"-DCMAKE_MAKE_PROGRAM={shutil.which('ninja')}"]
 
         # CMake configure arguments
-        cmake_install_prefix = Path.cwd() / '_cxinstall'
+        cmake_install_prefix = Path.cwd() / '_cxbuild/artifacts'
 
-        #cmake_prefix_path = ';'.join(self.config.prefix_dirs)
         cmake_prefix_path = join_posix_paths(self.config.prefix_dirs)
         print('cmake_prefix_path: ', cmake_prefix_path)
 
         configure_args += [
             f"-DCMAKE_BUILD_TYPE={self.config.build_type}",
             f"-DCMAKE_INSTALL_PREFIX:PATH={cmake_install_prefix}",
             #f"-DCMAKE_MODULE_PATH:PATH={cmake_module_path}",
```

### Comparing `cxbuild-0.1.0/cxbuild/copyutils.py` & `cxbuild-0.1.1/cxbuild/copyutils.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.0/cxbuild/cxbuild.py` & `cxbuild-0.1.1/cxbuild/cxbuild.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 from pathlib import Path
 
 from .solution import Solution
 
+import socket
+from loguru import logger
+
+HOST, PORT = 'localhost', 5005
+
+sock = socket.socket(socket.AF_INET, # Internet
+                     socket.SOCK_DGRAM) # UDP
+
+def logudp(message: str):
+    sock.sendto(bytes(message, 'utf-8'), (HOST, PORT))
+
+logger.add(logudp)
 
 class CxBuild:
     def __init__(self) -> None:
         self.solution = Solution(Path.cwd())
 
     def configure(self):
         print('configure')
```

### Comparing `cxbuild-0.1.0/cxbuild/extension_builder.py` & `cxbuild-0.1.1/cxbuild/extension_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,18 +23,9 @@
             raise ValueError("No CMakeExtension objects found")
 
         for ext in cmake_extensions:
             self.build_extension(ext)
 
     def build_extension(self, ext: CMakeExtension) -> None:
         ext_path = self.get_ext_fullpath(ext.name)
-        print('ext_path: ', ext_path)
         ext_dir = Path(ext_path).parent.absolute()
-        print('ext_dir: ', ext_dir)
-
-        CX_INSTALL_DIR = Path(os.environ.get('CX_INSTALL_DIR'))
-        print('CX_INSTALL_DIR: ', CX_INSTALL_DIR)
-        install_from = CX_INSTALL_DIR / ext.install_from
-        print('install_from: ', install_from)
-        install_to = ext_dir
-        print('install_to: ', install_to)
-        copy_directory_contents(install_from, install_to)
+        ext.build(ext_path, ext_dir)
```

### Comparing `cxbuild-0.1.0/cxbuild/pyproject.py` & `cxbuild-0.1.1/cxbuild/pyproject.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.0/cxbuild/setup_tool.py` & `cxbuild-0.1.1/cxbuild/setup_tool.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.0/cxbuild/solution.py` & `cxbuild-0.1.1/cxbuild/solution.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import site
 import importlib
 from pathlib import Path
 
 from .cmake_tool import CMakeConfig, CMakeTool
 
+from .activity import BuildActivity, DevelopActivity
 from .project_base import ProjectBase
 from .project import Project
 
 def is_glob(s):
     return any(char in s for char in '*?[]')
 
 class Solution(ProjectBase):
@@ -50,15 +51,15 @@
                 plugin_module = importlib.import_module(plugin)
                 print('plugin_module: ', plugin_module)
                 plugin_prefix = Path(plugin_module.__file__).parent.parent
                 print('plugin_prefix: ', plugin_prefix)
                 prefix_dirs.append(plugin_prefix)
                 
         print('prefix_dirs: ', prefix_dirs)
-        config = CMakeConfig(source_dir=Path('.'), build_dir=Path('_cxbuild'), build_type='Release', generator=None, prefix_dirs=prefix_dirs)
+        config = CMakeConfig(source_dir=Path('.'), build_dir=Path('_cxbuild/build'), build_type='Release', generator=None, prefix_dirs=prefix_dirs)
         return config
     
     def configure(self):
         print('configure')
         config = self.create_config()
         tool = CMakeTool(config)
         tool.configure()
@@ -66,32 +67,31 @@
     def develop(self):
         print('develop')
         config = self.create_config()
         tool = CMakeTool(config)
         tool.build()
         tool.install()
 
-        env = os.environ.copy()
-        env["CX_INSTALL_DIR"] = str(self.path / '_cxinstall')
+        activity = DevelopActivity()
+        activity.commit()
 
         for project in self.projects:
-            project.develop(env)
+            project.develop(activity.make_environ())
 
     def build(self):
         print('build')
         config = self.create_config()
         tool = CMakeTool(config)
         tool.build()
         tool.install()
-        
-        env = os.environ.copy()
-        env["ROOT_DIR"] = str(self.path)
-        env["CX_INSTALL_DIR"] = str(self.path / '_cxinstall')
+
+        activity = BuildActivity()
+        activity.commit()
 
         for project in self.projects:
-            project.build(env)
+            project.build(activity.make_environ())
 
     def install(self):
         print('install')
         config = self.create_config()
         tool = CMakeTool(config)
         tool.install()
```

### Comparing `cxbuild-0.1.0/cxbuild/build_hooks/__init__.py` & `cxbuild-0.1.1/cxbuild/backend.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,98 @@
 """
 PEP 517 build hooks
 """
 
 
 from __future__ import annotations
-
+from typing import Mapping, Any
+import os
 import setuptools.build_meta as build_meta
+
 __all__ = [
+    "_supported_features",
     "build_sdist",
     "build_wheel",
+    "build_editable",
     "get_requires_for_build_sdist",
     "get_requires_for_build_wheel",
+    "get_requires_for_build_editable",
     "prepare_metadata_for_build_wheel",
+    "prepare_metadata_for_build_editable",
 ]
 
+from pathlib import Path
+from loguru import logger
+
+from .project import Project
+
+
+def _supported_features():
+    return ["build_editable"]
+
+
 def build_sdist(
     sdist_directory: str,
     config_settings: dict[str, list[str] | str] | None = None,
 ) -> str:
+    logger.debug("Build hook: build_sdist")
     return build_meta.build_sdist(sdist_directory, config_settings)
 
+
 def build_wheel(
     wheel_directory: str,
     config_settings: dict[str, list[str] | str] | None = None,
     metadata_directory: str | None = None,
 ) -> str:
-    return build_meta.build_wheel(wheel_directory, config_settings, metadata_directory)
+    logger.debug("Build hook: build_wheel")
+    logger.debug(f"wheel_directory: {wheel_directory}")
+    project = Project(Path.cwd())
+    return project.build_wheel(wheel_directory, config_settings, metadata_directory)
+
+
+def build_editable(
+    wheel_directory: str,
+    config_settings: dict[str, list[str] | str] | None = None,
+    metadata_directory: str | None = None,
+) -> str:
+    logger.debug("Build hook: build_editable")
+    logger.debug(f"wheel_directory: {wheel_directory}")
+    # If not invoked indirectly by cxbuild itself do the default action
+    if not os.environ.get('CBX_ACTIVITY'):
+        return build_meta.build_wheel(wheel_directory, config_settings, metadata_directory)
+    return build_wheel(wheel_directory, config_settings, metadata_directory)
+
 
 def get_requires_for_build_sdist(
     config_settings: dict[str, str | list[str]] | None = None  # noqa: ARG001
 ) -> list[str]:
-    #return ["pathspec", "pyproject_metadata"]
+    logger.debug("Build hook: get_requires_for_build_sdist")
     return build_meta.get_requires_for_build_sdist(config_settings)
 
+
 def get_requires_for_build_wheel(
-    config_settings: dict[str, str | list[str]] | None = None,
+    config_settings: Mapping[str, Any] | None = None
 ) -> list[str]:
-    return build_meta.get_requires_for_build_wheel(config_settings)
+    logger.debug("Build hook: get_requires_for_build_wheel")
+    return []
+
+
+def get_requires_for_build_editable(self, config_settings=None):
+    logger.debug("Build hook: get_requires_for_build_editable")
+    return get_requires_for_build_wheel(config_settings)
+
 
 def prepare_metadata_for_build_wheel(
     metadata_directory: str,
     config_settings: dict[str, list[str] | str] | None = None,
 ) -> str:
-    return build_meta.prepare_metadata_for_build_wheel(metadata_directory, config_settings)
+    logger.debug("Build hook: prepare_metadata_for_build_wheel")
+    return build_meta.prepare_metadata_for_build_wheel(
+        metadata_directory, config_settings
+    )
+
+
+def prepare_metadata_for_build_editable(metadata_directory, config_settings=None):
+    logger.debug("Build hook: build_editable")
+    return build_meta.prepare_metadata_for_build_wheel(
+        metadata_directory, config_settings
+    )
```

### Comparing `cxbuild-0.1.0/cxbuild/cli/__init__.py` & `cxbuild-0.1.1/cxbuild/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.0/pkg/cxb_simple/CMakeLists.txt` & `cxbuild-0.1.1/pkg/cxb_simple/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.0/pkg/cxb_simple/pyproject.toml` & `cxbuild-0.1.1/pkg/cxb_simple/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.0/pkg/cxb_simple/src/main.cpp` & `cxbuild-0.1.1/pkg/cxb_simple/src/main.cpp`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.0/.gitignore` & `cxbuild-0.1.1/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -72,12 +72,11 @@
 .python-version
 
 # envrc
 .envrc
 
 # CxBuild
 _cxbuild
-_cxinstall
 
 depot
 tmp
 temp
```

### Comparing `cxbuild-0.1.0/LICENSE` & `cxbuild-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.0/pyproject.toml` & `cxbuild-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cxbuild"
-version = "0.1.0"
+version = "0.1.1"
 description = 'CMake Extension Builder'
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = []
 authors = [{ name = "Kurtis Fields", email = "kurtisfields@gmail.com" }]
 classifiers = [
@@ -17,16 +17,18 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "click ==8.1.3",
-    "tomli ==2.0.1"
+    "pydantic >=1.10.8",
+    "click >=8.1.3",
+    "tomli >=2.0.1",
+    "loguru >=0.7.0"
 ]
 
 #dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black ~=22.12.0"]
 test = ["pytest ~=7.2.1"]
```

### Comparing `cxbuild-0.1.0/PKG-INFO` & `cxbuild-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxbuild
-Version: 0.1.0
+Version: 0.1.1
 Summary: CMake Extension Builder
 Project-URL: homepage, https://github.com/crungelab/cxbuild
 Project-URL: documentation, https://crungelab.github.io/cxbuild/
 Project-URL: repository, https://github.com/crungelab/cxbuild
 Project-URL: changelog, https://github.com/crungelab/cxbuild/blob/main/CHANGELOG.md
 Author-email: Kurtis Fields <kurtisfields@gmail.com>
 License: MIT License
@@ -33,16 +33,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: click==8.1.3
-Requires-Dist: tomli==2.0.1
+Requires-Dist: click>=8.1.3
+Requires-Dist: loguru>=0.7.0
+Requires-Dist: pydantic>=1.10.8
+Requires-Dist: tomli>=2.0.1
 Provides-Extra: dev
 Requires-Dist: black~=22.12.0; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest~=7.2.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 # CxBuild :bricks:
```

