# Comparing `tmp/venv-modulefile-0.1.1.tar.gz` & `tmp/venv-modulefile-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/venv-modulefile/dist/tmpf2iq8d1m/venv-modulefile-0.1.1.tar", last modified: Tue May 23 15:19:45 2023, max compression
+gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/venv-modulefile/dist/tmpwc0d4fos/venv-modulefile-0.1.2.tar", last modified: Wed May 31 15:21:01 2023, max compression
```

## Comparing `venv-modulefile-0.1.1.tar` & `venv-modulefile-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4047 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-05-04 08:19:39.000000 venv-modulefile-0.1.1/pyproject.toml
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/setup.cfg
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-04-19 16:42:18.000000 venv-modulefile-0.1.1/MANIFEST.in
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      959 2023-05-22 14:55:50.000000 venv-modulefile-0.1.1/README.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9608 2023-05-22 10:27:41.000000 venv-modulefile-0.1.1/setup.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venvmod/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-05-23 15:19:14.000000 venv-modulefile-0.1.1/src/venvmod/VERSION
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      247 2023-05-23 10:47:49.000000 venv-modulefile-0.1.1/src/venvmod/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2984 2023-05-23 12:42:56.000000 venv-modulefile-0.1.1/src/venvmod/tools.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venvmod/commands/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1713 2023-05-23 14:21:45.000000 venv-modulefile-0.1.1/src/venvmod/commands/test_imports.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3467 2023-05-23 14:58:07.000000 venv-modulefile-0.1.1/src/venvmod/commands/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     5185 2023-05-23 14:00:38.000000 venv-modulefile-0.1.1/src/venvmod/commands/create_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10056 2023-05-23 14:58:12.000000 venv-modulefile-0.1.1/src/venvmod/commands/append_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    12965 2023-05-23 14:57:37.000000 venv-modulefile-0.1.1/src/venvmod/modulefile.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2903 2023-05-23 15:18:04.000000 venv-modulefile-0.1.1/src/README.md
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      809 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/entry_points.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/top_level.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      567 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/SOURCES.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4047 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/dependency_links.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      241 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/requires.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-05-04 08:19:39.000000 venv-modulefile-0.1.1/LICENSE.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-05-24 12:42:33.000000 venv-modulefile-0.1.2/pyproject.toml
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/setup.cfg
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-04-19 16:42:18.000000 venv-modulefile-0.1.2/MANIFEST.in
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      959 2023-05-22 14:55:50.000000 venv-modulefile-0.1.2/README.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9606 2023-05-24 11:56:17.000000 venv-modulefile-0.1.2/setup.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venvmod/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-05-31 15:18:02.000000 venv-modulefile-0.1.2/src/venvmod/VERSION
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      247 2023-05-23 10:47:49.000000 venv-modulefile-0.1.2/src/venvmod/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1624 2023-05-24 15:09:55.000000 venv-modulefile-0.1.2/src/venvmod/tools.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venvmod/commands/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1715 2023-05-24 14:50:10.000000 venv-modulefile-0.1.2/src/venvmod/commands/test_imports.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3825 2023-05-24 16:12:10.000000 venv-modulefile-0.1.2/src/venvmod/commands/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     5049 2023-05-24 16:11:24.000000 venv-modulefile-0.1.2/src/venvmod/commands/create_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    11077 2023-05-24 16:13:07.000000 venv-modulefile-0.1.2/src/venvmod/commands/append_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10550 2023-05-24 17:54:10.000000 venv-modulefile-0.1.2/src/venvmod/modulefile.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2899 2023-05-24 11:55:46.000000 venv-modulefile-0.1.2/src/README.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      807 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/entry_points.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/top_level.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      567 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/SOURCES.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/dependency_links.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      241 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/requires.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-05-04 08:19:39.000000 venv-modulefile-0.1.2/LICENSE.md
```

### Comparing `venv-modulefile-0.1.1/PKG-INFO` & `venv-modulefile-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/roland-lenain/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/roland-lenain/venv-modulefile/issues
 Project-URL: Doc, https://venv-modulefile.readthedocs.io/en/latest/index.html
@@ -68,24 +68,24 @@
 
 - The following commands modify the modulefile of the virtual environment:
   - `venvmod-cmd-append-path` / `venvmod-cmd-prepend-path`: modifies an environment variable
   - `venvmod-cmd-module-load`: loads a modulefile
   - `venvmod-cmd-module-use`: adds a search path for modulefile
   - `venvmod-cmd-remove-path`: removes path from environment variable
   - `venvmod-cmd-setenv`: defines an environment variable
-  - `venvmod-cmd-set-aliases`: defines an alias
+  - `venvmod-cmd-set-alias`: defines an alias
   - `venvmod-cmd-source-sh`: sources a script
 
 - `venvmod-cmd-read-env`: reads modifications to do from environment variable:
   - `[NAME]_LD_LIBRARY_PATH`, `[NAME]_PYTHONPATH`, `[NAME]_PATH`: ``prepend`` for each element separated by ':'
   - `[NAME]_MODULE_USE`: ``module use`` for each element 'module' separated by ' '
   - `[NAME]_MODULEFILES`: ``module load`` for each element '/path/' separated by ' '
   - `[NAME]_SOURCEFILES`: ``source-sh`` for each element 'shell script [args...]' separated by ';'
   - `[NAME]_EXPORTS`: ``setenv`` for each element 'var=value' separated by ' '
-  - `[NAME]_ALIASES`: ``set-aliases`` for each element 'var="value"' separated by ' '
+  - `[NAME]_ALIASES`: ``set-alias`` for each element 'var="value"' separated by ' '
   - `[NAME]_REMOVE_PATHS`: ``remove-path`` for each element 'var=value' separated by ' '
   where `[NAME]` is the name of the environment module (case insensitive, "-" and "." are replaced by "_").
 
 - `venvmod-add-appli` allows to create sub modulefile. `--appli` option of the above commands
   permit to modify these modulefiles.
 
 - `venvmod-test-import`: tests the import of modules given as argument
```

### Comparing `venv-modulefile-0.1.1/README.md` & `venv-modulefile-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.1/setup.py` & `venv-modulefile-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             "venvmod-cmd-module-use=venvmod.commands.append_module:module_use",
             "venvmod-cmd-module-load=venvmod.commands.append_module:module_load",
             "venvmod-cmd-source-sh=venvmod.commands.append_module:source_sh",
             "venvmod-cmd-prepend-path=venvmod.commands.append_module:prepend_path",
             "venvmod-cmd-append-path=venvmod.commands.append_module:append_path",
             "venvmod-cmd-setenv=venvmod.commands.append_module:setenv",
             "venvmod-cmd-remove-path=venvmod.commands.append_module:remove_path",
-            "venvmod-cmd-set-aliases=venvmod.commands.append_module:set_aliases",
+            "venvmod-cmd-set-alias=venvmod.commands.append_module:set_aliases",
             "venvmod-test-import=venvmod.commands.test_imports:test_imports",
         ],
     },
     # List additional URLs that are relevant to your project as a dict.
     #
     # This field corresponds to the "Project-URL" metadata fields:
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
```

### Comparing `venv-modulefile-0.1.1/src/venvmod/commands/test_imports.py` & `venv-modulefile-0.1.2/src/venvmod/commands/test_imports.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         error = err
 
     if verbose:
         print(f">>> import {module_name}:")
         if error:
             print(f"  FAILED {error}")
         else:
-            if hasattr(module,"__file__"):
+            if hasattr(module, "__file__"):
                 print(f"  {module.__file__}")
-            elif hasattr(module,"__name__"):
+            elif hasattr(module, "__name__"):
                 print(f"  {module.__name__}")
     return error
 
 
 def test_imports(arguments: List[str] = None) -> int:
     """Test import modules
```

### Comparing `venv-modulefile-0.1.1/src/venvmod/commands/__init__.py` & `venv-modulefile-0.1.2/src/venvmod/commands/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 import argparse
 import logging
 from pathlib import Path
 from typing import Any, List, Tuple
 
 from ..modulefile import get_module_file_directory
-from ..tools import logger, get_std_name
+from ..tools import check_raise, logger, get_std_name
 
 
 def get_parser(  # name: str,  # pylint: disable=too-many-arguments
                description: str,  # pylint: disable=too-many-arguments
                positionals: List[Tuple[str, Any, str, Any]] = None,
                with_appli: bool = False,
                options: List[Tuple[str, Any, str]] = None,
@@ -52,32 +52,38 @@
                                 metavar=positional[0].replace("-", "_"),
                                 default=positional[1],
                                 help=positional[2],
                                 nargs=positional[3])
 
     if options:
         for option in options:
-            parser.add_argument(f"--{option[0]}",
-                                metavar=option[0].replace("-", "_"),
-                                default=option[1],
-                                help=option[2])
+            if isinstance(option[1], bool):
+                parser.add_argument(f"--{option[0]}",
+                                    action='store_true' if not option[1] else 'store_false',
+                                    default=option[1],
+                                    help=option[2])
+            else:
+                parser.add_argument(f"--{option[0]}",
+                                    metavar=option[0].replace("-", "_"),
+                                    default=option[1],
+                                    help=option[2])
 
     parsered = parser.parse_args(args)
     if parsered.verbose:
         logger.setLevel(logging.DEBUG)
     else:
         logger.setLevel(logging.INFO)
 
-    if not Path(parsered.virtual_env).absolute().is_dir():
-        raise FileNotFoundError(f"virtual environment '{parsered.virtual_env}' does not exist.")
+    check_raise(not Path(parsered.virtual_env).absolute().is_dir(),
+                FileNotFoundError, f"virtual environment '{parsered.virtual_env}' does not exist.")
 
     return parsered
 
 
-def get_module_filepath(virtual_env: Path, appli_name: str = None) -> str:
+def get_module_filepath(virtual_env: Path, appli_name: str = None) -> Path:
     """_summary_
 
     Parameters
     ----------
     virtual_env : pathlib.Path
         name or path to the virtual env
     appli_name : str, optional
```

### Comparing `venv-modulefile-0.1.1/src/venvmod/commands/create_module.py` & `venv-modulefile-0.1.2/src/venvmod/commands/create_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from packaging import version
 
 from ..tools import get_std_name
 from . import get_parser
 from .append_module import module_load, read_env as read_env_vars
 from ..modulefile import (get_version, ModuleInstaller, upgrade_modulefile, create_modulefile,
-                          upgrade_venv)
+                          upgrade_venv, test_if_already_init)
 
 from ..tools import PACKAGE_NAME, check_raise, remove_duplicates
 
 
 def initialize(virtual_env: Path = None,
                version_or_path: str = "5.2.0",
                read_env: bool = False) -> int:
@@ -47,45 +47,41 @@
                      ("activate-log", "", "Log message when the module is loaded."),
                      ("read-env", False, "Read environment variables. 'See cmd-read-env'")])
         virtual_env = Path(options.virtual_env).absolute()
         if options.modulefile_version:
             version_or_path = options.modulefile_version
         read_env = options.read_env
 
+    test_if_already_init(virtual_env=virtual_env)
+
     if version.parse(get_version()) < version.parse("14.6"):
 
         install_prefix = virtual_env / "opt" / "modulefiles"
         if not (install_prefix / "init").exists():
-            code = ModuleInstaller(install_prefix=install_prefix,
-                                   version_or_path=version_or_path,
-                                   cache_directory=virtual_env / ".cache").run(
-                                       verbose=options.verbose, do_raise=True)
-            if code:
-                return code
-
-        code = upgrade_modulefile(virtual_env=virtual_env, module_prefix=install_prefix)
-        if code:
-            return code
-
-    code = create_modulefile(virtual_env=virtual_env,
-                             module_name=get_std_name(virtual_env.name),
-                             module_category=PACKAGE_NAME,
-                             log_load=options.activate_log)
-    if code:
-        return code
+            ModuleInstaller(install_prefix=install_prefix,
+                            version_or_path=version_or_path,
+                            cache_directory=virtual_env / ".cache").run(
+                                verbose=options.verbose)
+
+        upgrade_modulefile(virtual_env=virtual_env, module_prefix=install_prefix)
+
+    create_modulefile(virtual_env=virtual_env,
+                      module_name=get_std_name(virtual_env.name),
+                      module_category=PACKAGE_NAME,
+                      log_load=options.activate_log)
 
     if read_env:
         read_env_vars(arguments=(virtual_env, get_std_name(virtual_env.name)))
 
     return upgrade_venv(virtual_env=virtual_env)
 
 
 def add_appli(virtual_env: Path = None,
               applis: List[str] = None,
-              read_env: bool = False):
+              read_env: bool = False) -> int:
     """Add application modulefiles to the environment.
 
     This call also use the :func:`venvmod.commands.append_module.read_env` function for each appli.
 
     Parameters
     ----------
     virtual_env : Path, optional
@@ -110,20 +106,20 @@
         virtual_env_name = get_std_name(virtual_env.name)
         read_env = options.read_env
 
     fails = []
     for appli in remove_duplicates(options.APPLI + (applis if applis else [])):
         appli_name = get_std_name(appli)
         module_name = f"{virtual_env_name}-{appli_name}"
-        code = create_modulefile(virtual_env=virtual_env,
-                                 module_name=module_name,
-                                 module_category=f"{PACKAGE_NAME}-{appli_name}")
-        if code:
+        if create_modulefile(virtual_env=virtual_env,
+                             module_name=module_name,
+                             module_category=f"{PACKAGE_NAME}-{appli_name}"):
             fails.append(appli)
 
         if read_env:
             read_env_vars(arguments=(virtual_env, appli_name))
         module_load(arguments=(virtual_env, "", module_name))
 
     check_raise(condition=len(fails) > 0,
                 exception_type=RuntimeError,
                 message=f"The installation of the folowing appli failed : {fails}")
+    return 0
```

### Comparing `venv-modulefile-0.1.1/src/venvmod/commands/append_module.py` & `venv-modulefile-0.1.2/src/venvmod/commands/append_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 To append instructions in modulefile.
 """
 import os
 from pathlib import Path
 from typing import Any, List, Tuple
 
 from venvmod.tools import get_std_name, logger
-from venvmod.modulefile import add_command
 
 from . import get_module_filepath, get_parser
+from ..tools import check_raise
 
 
 def append_command(arguments: Tuple[str, str, str],
                    description: str,
                    positionals: List[Tuple[str, Any, str, Any]],
                    command: str):
     """Append a command to a modulefile.
@@ -43,15 +43,21 @@
             logger.debug("append_command positional '%s': '%s'", positional, values)
             arguments += " " + " ".join(values)
     else:
         virtual_env, appli, arguments = arguments
 
     filepath = get_module_filepath(virtual_env=Path(virtual_env).absolute(), appli_name=appli)
 
-    add_command(filename=filepath, line=f"{command} {arguments}")
+    check_raise(not filepath.exists(), FileNotFoundError,
+                f"You can't add command to non exsting modulefile {filepath}."
+                f" You may need to run 'venvmod-initialize {virtual_env}'"
+                f" or 'venvmod-add-appli {virtual_env} {filepath.name}' first.")
+
+    with filepath.open(mode='a', encoding='utf-8') as modulefile:
+        modulefile.write(f"{command} {arguments}\n")
 
 
 def module_use(arguments: Tuple[str, str, str] = None):
     """Add a 'module use' command to a modulefile.
 
     Paths to use are given as str in the last value of ``arguments``.
 
@@ -165,42 +171,42 @@
                    description="Remove value from environment variable.",
                    positionals=[("VARIABLE", [], "Environment variable to modify", 1),
                                 ("PATH", [], "Path to remove from variable", 1)],
                    command="remove-path")
 
 
 def set_aliases(arguments: Tuple[str, str, str] = None):
-    """Add a 'set-aliases' command to a modulefile.
+    """Add a 'set-alias' command to a modulefile.
 
     Alias to define are given as str in the last value of ``arguments``.
 
     Parameters
     ----------
     arguments : Tuple[str, str, str], optional
         See ``append_command`` function, by default None
     """
     append_command(arguments,
                    description="Define aliases.",
                    positionals=[("ALIAS", [], "Alias name", 1),
                                 ("VALUE", [], "Alias value", 1)],
-                   command="set-aliases")
+                   command="set-alias")
 
 
 def read_env(arguments: Tuple[str, str] = None):  # pylint: disable=too-many-branches
     """Add commands to a modulefile from environment variables.
 
     Parse ``os.environ`` to look at variable starting with 'appli' (case insensitive) name.
 
     For thoses variables, append commands for the following suffixes:
      - "LD_LIBRARY_PATH", "PYTHONPATH", "PATH": ``prepend``
      - "MODULE_USE": ``module use``
      - "MODULEFILES": ``module load``
      - "SOURCEFILES": ``source-sh`` for each element 'shell script [args...]' separated by ';'
      - "EXPORTS": ``setenv`` for each element 'var=value' separated by ' '
-     - "ALIASES": ``set-aliases`` for each element 'var=value' separated by ' '
+     - "ALIASES": ``set-alias`` for each element 'var=value' separated by ' '
      - "REMOVE_PATHS": ``remove-path`` for each element 'var=value' separated by ' '
 
     Examples
     --------
     The following ::
 
         $ export MY_APPLI_LD_LIBRARY_PATH="/path/to/lib1:/path/to/lib2"
@@ -227,39 +233,57 @@
     appli_env_vars = {envvar: value for envvar, value in os.environ.items()
                       if get_std_name(envvar).startswith(appli.replace('.', '_'))}
 
     logger.debug("read_env: os.environ = '%s'", os.environ)
     logger.debug("read_env: appli_env_vars = '%s'", appli_env_vars)
 
     # Source file in first
-    for envvar, value in appli_env_vars.items():
+    _read_src_files(virtual_env, appli_env_vars, appli)
+    # modules
+    _read_modules(virtual_env, appli_env_vars, appli)
+    # prepend
+    _read_prepend(virtual_env, appli_env_vars, appli)
+    # other, remove is at the end
+    _read_others(virtual_env, appli_env_vars, appli)
+
+
+def _read_src_files(virtual_env, appli_env_vars, appli):
+    for envvar, value in appli_env_vars.copy().items():
         if envvar.endswith("SOURCEFILES"):
             for var in value.split(";"):
                 if var:
                     source_sh(arguments=(virtual_env, appli, var))
             appli_env_vars.pop(envvar)
             break
 
-    path_to_prepend = ["LD_LIBRARY_PATH", "PYTHONPATH", "PATH"]
-    for envvar, value in appli_env_vars.items():
 
-        for var_path in path_to_prepend:
+def _read_modules(virtual_env, appli_env_vars, appli):
+    for suffix, function in {
+            "MODULE_USE": module_use,
+            "MODULEFILES": module_load}.items():
+        for envvar, value in appli_env_vars.copy().items():
+            if envvar.endswith(suffix):
+                function(arguments=(virtual_env, appli, value))
+                appli_env_vars.pop(envvar)
+
+
+def _read_prepend(virtual_env, appli_env_vars, appli):
+    for var_path in ["LD_LIBRARY_PATH", "PYTHONPATH", "PATH"]:
+        for envvar, value in appli_env_vars.copy().items():
             if envvar.endswith(var_path):
                 for var in reversed(value.split(":")):
                     if var:
                         prepend_path(arguments=(virtual_env, appli, f"{var_path} {var}"))
-                break
+                appli_env_vars.pop(envvar)
 
-        for suffix, function in {
-                "MODULE_USE": module_use,
-                "MODULEFILES": module_load}.items():
-            if envvar.endswith(suffix):
-                function(arguments=(virtual_env, appli, value))
 
-        for suffix, function in {
+def _read_others(virtual_env, appli_env_vars, appli):
+    for suffix, function in {
                 "EXPORTS": setenv,
                 "ALIASES": set_aliases,
                 "REMOVE_PATHS": remove_path}.items():
+        for envvar, value in appli_env_vars.copy().items():
             if envvar.endswith(suffix):
                 for var in value.split():
                     if var:
                         function(arguments=(virtual_env, appli, var.replace("=", " ")))
+                appli_env_vars.pop(envvar)
```

### Comparing `venv-modulefile-0.1.1/src/venvmod/modulefile.py` & `venv-modulefile-0.1.2/src/venvmod/modulefile.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Environment module modification/installation."""
 
 import os
 import shutil
 from pathlib import Path
 import pathlib
+import subprocess
 import tarfile
-from typing import List
 
 from packaging import version
 import requests
 
-from venvmod.tools import (get_std_name, get_process_result, run_process, check_raise,
+from venvmod.tools import (get_std_name, get_shell_command, check_raise,
                            get_shell_name, PACKAGE_NAME, logger)
 
 
 def get_module_file_directory(virtual_env: Path) -> Path:
     """Gets the modulefiles directory
 
     Parameters
@@ -26,69 +26,49 @@
     -------
     Path
         virtual_env path + "/etc/modulefiles"
     """
     return virtual_env.absolute() / "etc" / "modulefiles"
 
 
-def add_command(filename: Path, line: str):
-    """Appends a command to a modulefile
+ACTIVATE_HEADER_LINE = (f"# This file is generated from {PACKAGE_NAME}"
+                        " from regular venv or virtualenv file.")
+
+
+def test_if_already_init(virtual_env: Path):
+    """checks if venv-modulefile is already initialized.
 
     Parameters
     ----------
-    filename : Path
-        File to modify
-    line : str
-        Line to append
-
-    Raises
-    ------
-    FileNotFoundError
-        If filename is not found
+    virtual_env : Path
+        Path to virtual env
     """
-    if not filename.exists():
-        raise FileNotFoundError(f"Can't add command to non exsting file {filename}.")
-    with open(filename, mode='a', encoding='utf-8') as modulefile:
-        modulefile.write(line + "\n")
+    with (virtual_env / "bin" / "activate").open(mode="r", encoding='utf-8') as src_file:
+        check_raise(ACTIVATE_HEADER_LINE in src_file.read(), AssertionError,
+                    f"{virtual_env} is already a venv-modulefile environment.")
 
 
 def get_version() -> str:
     """Gets modulefile version
 
     Returns
     -------
     str
         version as 'x.y.z', '0.0.0' if not found
     """
-    result = get_process_result(command="module --version", capture_output=True)
-    logger.debug(f"get_version: {result}")
-    logger.debug(f"get_version: {result.stderr.decode()}")
-    logger.debug(f"get_version: {result.stdout.decode()}")
-    if 'VERSION=' in result.stderr.decode().split()[0]: # version < 4.0
-        return result.stderr.decode().split()[0].split("=")[1]
-    if 'Modules' == result.stderr.decode().split()[0]:
-        return result.stderr.decode().split()[2]
-    return "0.0.0"
-
+    result = subprocess.run([get_shell_command(), '-c', "module --version"],
+                            stderr=subprocess.PIPE, stdout=subprocess.PIPE, check=False)
 
-def get_version_list(index: int = 0) -> List[int] or int:
-    """Gets version as list
-
-    Parameters
-    ----------
-    index : int, optional
-        index in version, by default 0
-
-    Returns
-    -------
-    List[int] or int
-        version numbers or version number if index > 0
-    """
-    version_list = [int(id) for id in get_version().split(".")]
-    return version_list[index-1] if index else version_list
+    logger.debug("get_version: %s\n%s\n%s", result, result.stderr.decode(), result.stdout.decode())
+    if result.returncode == 0:
+        if 'VERSION=' in result.stderr.decode().split()[0]:  # version < 4.0
+            return result.stderr.decode().split()[0].split("=")[1]
+        if 'Modules' == result.stderr.decode().split()[0]:
+            return result.stderr.decode().split()[2]
+    return "0.0.0"
 
 
 class ModuleInstaller:  # pylint: disable=too-few-public-methods
     """Class to install Environment Module.
     """
 
     def __init__(self,
@@ -96,28 +76,21 @@
                  install_prefix: str or Path,
                  cache_directory: str or Path) -> None:
 
         self._version_or_path: str = version_or_path
         self._install_prefix: Path = Path(install_prefix)
         self._cache_directory: Path = Path(cache_directory)
 
-    def run(self, verbose: bool = False, do_raise: bool = True) -> int:
+    def run(self, verbose: bool = False):
         """run installer
 
         Parameters
         ----------
         verbose : bool, optional
             True to enable verbosity, by default False
-        do_raise : bool, optional
-            True to raise if fails, by default True
-
-        Returns
-        -------
-        int
-            return code
         """
 
         self._cache_directory.mkdir(parents=True, exist_ok=True)
         if Path(self._version_or_path).exists():
             src_directory = Path(self._version_or_path)
             build_directory = self._cache_directory / src_directory.name
         else:
@@ -130,53 +103,47 @@
                 cwd = os.getcwd()
                 os.chdir(self._cache_directory)
                 try:
                     file = tarfile.open(  # pylint: disable=consider-using-with
                         fileobj=requests.get(
                             url="https://github.com/cea-hpc/modules/releases/download/"
                                 f"v{self._version_or_path}/modules-{self._version_or_path}.tar.gz",
-                            stream=True).raw,
+                            stream=True,
+                            timeout=120.0).raw,
                         mode="r|gz")
                     try:
                         file.extractall()
                     finally:
                         file.close()
                 finally:
                     os.chdir(cwd)
             build_directory = src_directory
 
         build_directory.mkdir(parents=True, exist_ok=True)
-        code = run_process(command=f"{src_directory}/configure --prefix={self._install_prefix}"
-                                   " --with-python=$(which python3)",
-                           verbose=verbose,
-                           cwd=build_directory,
-                           do_raise=do_raise)
-        if code:
-            return code
-
-        return run_process(command="make clean && make && make install",
-                           verbose=verbose,
-                           cwd=build_directory,
-                           do_raise=do_raise)
 
+        pipe = subprocess.PIPE if not verbose else None
+        for command in [[f"{src_directory}/configure",
+                         f"--prefix={self._install_prefix}",
+                         "--with-python=$(which python3)"],
+                        ["make", "clean"],
+                        ["make"],
+                        ["make", "install"]]:
+            subprocess.run([get_shell_command(), "-c", " ".join(command)],
+                           stderr=pipe, stdout=pipe, cwd=build_directory, check=True)
 
-def upgrade_modulefile(virtual_env: Path, module_prefix: Path) -> int:
+
+def upgrade_modulefile(virtual_env: Path, module_prefix: Path):
     """Upgrade modulefile in venv
 
     Parameters
     ----------
     virtual_env : Path
         Path to virtual env
     module_prefix : Path
         Modulefile install prefix
-
-    Returns
-    -------
-    int
-        return code
     """
 
     activate_src = virtual_env / "bin" / "activate"
     check_raise(not activate_src.is_file(), AssertionError,
                 f'"activate" file {activate_src} not found.')
 
     with open(activate_src, "r", encoding='utf-8') as src_file:
@@ -196,16 +163,14 @@
     with open(activate_tmp, "w", encoding='utf-8') as tmp_file:
         for line in src_lines:
             tmp_file.write(line)
             if "you cannot run it directly" in line:
                 tmp_file.write("\n"f". {init_file_path}{os.sep}$(ps -ocomm= -q $$)\n")
     pathlib.Path.replace(activate_tmp, activate_src)
 
-    return 0
-
 
 MODULE_TEMPLATES = {"TCL": """#%Module -*- tcl -*-
 ##
 ## modulefile for __name__
 ##
 #Global infos
 set              category             __category__
@@ -218,22 +183,21 @@
 module-whatis "adds $name to your environment"
 
 __log_load__
 
 #conflicts, prereq
 conflict $category
 
-""",
-    }
+"""}
 
 
 def create_modulefile(virtual_env: Path,
                       module_name: str = PACKAGE_NAME,
                       module_category: str = None,
-                      log_load: str = "") -> int:
+                      log_load: str = ""):
     """Creates a modulefile.
 
     Parameters
     ----------
     module_name : str
         Name of the module to create
     module_directory : Path
@@ -253,146 +217,114 @@
     module_file = module_file.replace("__category__", module_category)
 
     to_replace = ""
     if log_load:
         log_load = log_load.replace('[', r'\[').replace(']', r'\]')
         to_replace = ('if { [ module-info mode load ] } {\n'
                       f'    puts stderr "{log_load}"\n'
-                       '}')
+                      '}')
     module_file = module_file.replace("__log_load__", to_replace)
 
     with open(module_file_name, "w", encoding='utf-8') as mod_file:
         mod_file.write(module_file)
-        return 0
 
-    return 1
 
+SHELL_TEST_DEACTIVATE_STATUS = """
+function _test_deactivate_status(){
+    module_status=( $module_unuse_status $module_unload_status )
+    unset module_unuse_status
+    unset module_unload_status
+    unset -f _test_deactivate_status
+    for return_code in $module_status ; do
+        if (( $return_code > 0 )); then return $return_code; fi
+    done
+}
 
-USE_MODULE_TEMPLATE = """module use "__module_dir__"
-module_use_status=( $module_use_status $? )
 """
-LOAD_MODULE_TEMPLATE = """module load '__module_name__'
-module_load_status=( $module_load_status $? )
+
+UNLOAD_MODULES = """
+    # Unload non-Python dependencies
+    module unload '{}'
+    module_unload_status=$?
+    module unuse '{}'
+    module_unuse_status=$?
+
 """
 
-UNLOAD_MODULE_TEMPLATE = """    module unload '__module_name__'
-    module_unload_status=( $module_unload_status $? )
+LOAD_MODULES = """
+# Load non-Python dependencies
+module use '{}'
+module_use_status=$?
+module load '{}'
+module_load_status=$?
 """
-UNUSE_MODULE_TEMPLATE = """    module unuse "__module_dir__"
-    module_unuse_status=( $module_unuse_status $? )
+
+SHELL_TEST_ACTIVATE_STATUS = """
+function _test_activate_status(){
+    module_status=( $module_use_status $module_load_status )
+    unset module_use_status
+    unset module_load_status
+    unset -f _test_activate_status
+    for return_code in $module_status ; do
+       if (( $return_code > 0 )); then return $return_code; fi
+    done
+}
+_test_activate_status
 """
 
 
-def upgrade_venv(virtual_env: Path):  # pylint: disable=too-many-branches,too-many-locals,too-many-statements
+def upgrade_venv(virtual_env: Path):
     """Ugrade virtual env with modulefile at activate and deactivate.
 
     Parameters
     ----------
     env_prefix : Path
         Path to environment.
 
     Raises
     ------
     AssertionError
         If the activate script is not found.
     AssertionError
         If the module is already loaded frome the script but from another modulefile directory.
     """
-    bin_dir = virtual_env / "bin"
 
-    activate_src = bin_dir / "activate"
+    activate_src = virtual_env / "bin" / "activate"
     check_raise(not activate_src.is_file(), AssertionError,
-                f'"activate" file is expected in {bin_dir}.')
-
-    header_line = f"# This file is generated from {PACKAGE_NAME}"\
-                  " from regular venv or virtualenv file."
+                f'{activate_src} file not found.')
 
     modulefile_name = get_std_name(virtual_env.name)
     module_directory = get_module_file_directory(virtual_env=virtual_env)
-    unuse_module = UNUSE_MODULE_TEMPLATE.replace("__module_dir__", str(module_directory))
-    unload_module = UNLOAD_MODULE_TEMPLATE.replace("__module_name__", modulefile_name)
-
-    load_module = LOAD_MODULE_TEMPLATE.replace("__module_name__", modulefile_name)
-    use_module = USE_MODULE_TEMPLATE.replace("__module_dir__", str(module_directory))
 
-    with open(activate_src, "r", encoding='utf-8') as src_file:
-        file_read = src_file.read()
-        check_raise(header_line in file_read, AssertionError,
-                    f"{virtual_env} is already a venv-modulefile environment.")
+    test_if_already_init(virtual_env=virtual_env)
 
     with open(activate_src, "r", encoding='utf-8') as src_file:
         src_lines = src_file.readlines()
 
     tmp_path = virtual_env / "tmp" / PACKAGE_NAME
     tmp_path.mkdir(exist_ok=True, parents=True)
 
     activate_tmp = tmp_path / "activate"
 
-    with open(activate_tmp, "w", encoding='utf-8') as tmp_file:
-
-        def _write_in_file(tmp_file, line, to_write):
-            if to_write:
-                if to_write[0] == -1:
-                    tmp_file.write(to_write[1])
-                    tmp_file.write(line)
-                elif to_write[0] == 1:
-                    tmp_file.write(line)
-                    tmp_file.write(to_write[1])
-                elif to_write[0] == 0:
-                    tmp_file.write(line)
+    with activate_tmp.open("w", encoding='utf-8') as tmp_file:
 
-        reset_is_done = 0
-        deactivate_nondestructive = 0
         for count, line in enumerate(src_lines):
-            to_write = None
+            to_write = ()
             if count == 2:
-                to_write = (-1, f"{header_line}\n")
+                to_write = (0, f"{ACTIVATE_HEADER_LINE}\n")
             elif "deactivate () {" in line:
-                to_write = (-1, """
-function _test_deactivate_status(){
-module_status=( $module_unuse_status $module_unload_status )
-unset module_unuse_status
-unset module_unload_status
-unset -f _test_deactivate_status
-for return_code in $module_status ; do
-    if (( $return_code > 0 )); then return $return_code; fi
-done
-}\n\n""")
+                to_write = (0, SHELL_TEST_DEACTIVATE_STATUS)
             elif "unset -f deactivate" in line:
                 to_write = (1, "        _test_deactivate_status\n        return $?\n")
             elif "reset old environment variables" in line:
-                to_write = (-1, "\n    # Unload non-Python dependencies\n"
-                           + unload_module + unuse_module + "\n")
-                reset_is_done += 1
+                to_write = (0, UNLOAD_MODULES.format(modulefile_name, str(module_directory)))
             elif "deactivate nondestructive" in line:
-                to_write = (1, "\n# Load non-Python dependencies\n" + use_module + load_module)
-                deactivate_nondestructive += 1
+                to_write = (1, LOAD_MODULES.format(str(module_directory), modulefile_name))
             else:
                 to_write = (0, "")
 
-            _write_in_file(tmp_file, line, to_write)
+            tmp_file.write(line + to_write[1] if to_write[0] else to_write[1] + line)
 
-        if reset_is_done != 1:
-            logger.error(
-                "'reset old environment variables' has been found %s"
-                " times in activate script. It is expectet to be 1 time.", reset_is_done)
-        if deactivate_nondestructive != 1:
-            logger.error(
-                "'deactivate nondestructive' has been found %s"
-                " times in activate script. It is expectet to be 1 time.",
-                deactivate_nondestructive)
-
-        tmp_file.write("""
-function _test_activate_status(){
-    module_status=( $module_use_status $module_load_status )
-    unset module_use_status
-    unset module_load_status
-    unset -f _test_activate_status
-    for return_code in $module_status ; do
-       if (( $return_code > 0 )); then return $return_code; fi
-    done
-}
-_test_activate_status
-""")
+        tmp_file.write(SHELL_TEST_ACTIVATE_STATUS)
 
     shutil.copyfile(activate_tmp, activate_src)
     shutil.rmtree(tmp_path)
```

### Comparing `venv-modulefile-0.1.1/src/README.md` & `venv-modulefile-0.1.2/src/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,24 +39,24 @@
 
 - The following commands modify the modulefile of the virtual environment:
   - `venvmod-cmd-append-path` / `venvmod-cmd-prepend-path`: modifies an environment variable
   - `venvmod-cmd-module-load`: loads a modulefile
   - `venvmod-cmd-module-use`: adds a search path for modulefile
   - `venvmod-cmd-remove-path`: removes path from environment variable
   - `venvmod-cmd-setenv`: defines an environment variable
-  - `venvmod-cmd-set-aliases`: defines an alias
+  - `venvmod-cmd-set-alias`: defines an alias
   - `venvmod-cmd-source-sh`: sources a script
 
 - `venvmod-cmd-read-env`: reads modifications to do from environment variable:
   - `[NAME]_LD_LIBRARY_PATH`, `[NAME]_PYTHONPATH`, `[NAME]_PATH`: ``prepend`` for each element separated by ':'
   - `[NAME]_MODULE_USE`: ``module use`` for each element 'module' separated by ' '
   - `[NAME]_MODULEFILES`: ``module load`` for each element '/path/' separated by ' '
   - `[NAME]_SOURCEFILES`: ``source-sh`` for each element 'shell script [args...]' separated by ';'
   - `[NAME]_EXPORTS`: ``setenv`` for each element 'var=value' separated by ' '
-  - `[NAME]_ALIASES`: ``set-aliases`` for each element 'var="value"' separated by ' '
+  - `[NAME]_ALIASES`: ``set-alias`` for each element 'var="value"' separated by ' '
   - `[NAME]_REMOVE_PATHS`: ``remove-path`` for each element 'var=value' separated by ' '
   where `[NAME]` is the name of the environment module (case insensitive, "-" and "." are replaced by "_").
 
 - `venvmod-add-appli` allows to create sub modulefile. `--appli` option of the above commands
   permit to modify these modulefiles.
 
 - `venvmod-test-import`: tests the import of modules given as argument
```

### Comparing `venv-modulefile-0.1.1/src/venv_modulefile.egg-info/entry_points.txt` & `venv-modulefile-0.1.2/src/venv_modulefile.egg-info/entry_points.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 venvmod-add-appli = venvmod.commands.create_module:add_appli
 venvmod-cmd-append-path = venvmod.commands.append_module:append_path
 venvmod-cmd-module-load = venvmod.commands.append_module:module_load
 venvmod-cmd-module-use = venvmod.commands.append_module:module_use
 venvmod-cmd-prepend-path = venvmod.commands.append_module:prepend_path
 venvmod-cmd-read-env = venvmod.commands.append_module:read_env
 venvmod-cmd-remove-path = venvmod.commands.append_module:remove_path
-venvmod-cmd-set-aliases = venvmod.commands.append_module:set_aliases
+venvmod-cmd-set-alias = venvmod.commands.append_module:set_aliases
 venvmod-cmd-setenv = venvmod.commands.append_module:setenv
 venvmod-cmd-source-sh = venvmod.commands.append_module:source_sh
 venvmod-initialize = venvmod.commands.create_module:initialize
 venvmod-test-import = venvmod.commands.test_imports:test_imports
```

### Comparing `venv-modulefile-0.1.1/src/venv_modulefile.egg-info/SOURCES.txt` & `venv-modulefile-0.1.2/src/venv_modulefile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.1/src/venv_modulefile.egg-info/PKG-INFO` & `venv-modulefile-0.1.2/src/venv_modulefile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/roland-lenain/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/roland-lenain/venv-modulefile/issues
 Project-URL: Doc, https://venv-modulefile.readthedocs.io/en/latest/index.html
@@ -68,24 +68,24 @@
 
 - The following commands modify the modulefile of the virtual environment:
   - `venvmod-cmd-append-path` / `venvmod-cmd-prepend-path`: modifies an environment variable
   - `venvmod-cmd-module-load`: loads a modulefile
   - `venvmod-cmd-module-use`: adds a search path for modulefile
   - `venvmod-cmd-remove-path`: removes path from environment variable
   - `venvmod-cmd-setenv`: defines an environment variable
-  - `venvmod-cmd-set-aliases`: defines an alias
+  - `venvmod-cmd-set-alias`: defines an alias
   - `venvmod-cmd-source-sh`: sources a script
 
 - `venvmod-cmd-read-env`: reads modifications to do from environment variable:
   - `[NAME]_LD_LIBRARY_PATH`, `[NAME]_PYTHONPATH`, `[NAME]_PATH`: ``prepend`` for each element separated by ':'
   - `[NAME]_MODULE_USE`: ``module use`` for each element 'module' separated by ' '
   - `[NAME]_MODULEFILES`: ``module load`` for each element '/path/' separated by ' '
   - `[NAME]_SOURCEFILES`: ``source-sh`` for each element 'shell script [args...]' separated by ';'
   - `[NAME]_EXPORTS`: ``setenv`` for each element 'var=value' separated by ' '
-  - `[NAME]_ALIASES`: ``set-aliases`` for each element 'var="value"' separated by ' '
+  - `[NAME]_ALIASES`: ``set-alias`` for each element 'var="value"' separated by ' '
   - `[NAME]_REMOVE_PATHS`: ``remove-path`` for each element 'var=value' separated by ' '
   where `[NAME]` is the name of the environment module (case insensitive, "-" and "." are replaced by "_").
 
 - `venvmod-add-appli` allows to create sub modulefile. `--appli` option of the above commands
   permit to modify these modulefiles.
 
 - `venvmod-test-import`: tests the import of modules given as argument
```

### Comparing `venv-modulefile-0.1.1/LICENSE.md` & `venv-modulefile-0.1.2/LICENSE.md`

 * *Files identical despite different names*

