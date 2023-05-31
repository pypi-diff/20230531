# Comparing `tmp/ascend_io_cli-1.0.6.tar.gz` & `tmp/ascend_io_cli-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascend_io_cli-1.0.6.tar", max compression
+gzip compressed data, was "ascend_io_cli-1.0.8.tar", max compression
```

## Comparing `ascend_io_cli-1.0.6.tar` & `ascend_io_cli-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    11357 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/LICENSE
--rw-r--r--   0        0        0     1210 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/README.rst
--rw-r--r--   0        0        0      573 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/ascend_io_cli/__init__.py
--rwxr-xr-x   0        0        0     1202 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/ascend_io_cli/cli.py
--rw-r--r--   0        0        0        0 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/ascend_io_cli/commands/__init__.py
--rw-r--r--   0        0        0     6467 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/ascend_io_cli/commands/apply.py
--rw-r--r--   0        0        0     8089 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/ascend_io_cli/commands/clone.py
--rw-r--r--   0        0        0     1877 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/ascend_io_cli/commands/config.py
--rw-r--r--   0        0        0     2170 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/ascend_io_cli/commands/delete.py
--rw-r--r--   0        0        0     1426 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/ascend_io_cli/commands/describe.py
--rw-r--r--   0        0        0     7085 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/ascend_io_cli/commands/download.py
--rw-r--r--   0        0        0     3822 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/ascend_io_cli/commands/list.py
--rw-r--r--   0        0        0     2500 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/ascend_io_cli/commands/pause.py
--rw-r--r--   0        0        0     3951 2022-12-23 18:45:24.071849 ascend_io_cli-1.0.6/ascend_io_cli/commands/reset.py
--rw-r--r--   0        0        0      986 2022-12-23 18:45:24.075849 ascend_io_cli-1.0.6/ascend_io_cli/commands/resume.py
--rw-r--r--   0        0        0      312 2022-12-23 18:45:24.075849 ascend_io_cli-1.0.6/ascend_io_cli/commands/version.py
--rw-r--r--   0        0        0     5283 2022-12-23 18:45:24.075849 ascend_io_cli-1.0.6/ascend_io_cli/support.py
--rw-r--r--   0        0        0     1232 2022-12-23 18:45:24.075849 ascend_io_cli-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 ascend_io_cli-1.0.6/setup.py
--rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 ascend_io_cli-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/LICENSE
+-rw-r--r--   0        0        0     1210 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/README.rst
+-rw-r--r--   0        0        0      573 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/__init__.py
+-rwxr-xr-x   0        0        0     1344 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/cli.py
+-rw-r--r--   0        0        0        0 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/__init__.py
+-rw-r--r--   0        0        0     6467 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/apply.py
+-rw-r--r--   0        0        0     8108 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/clone.py
+-rw-r--r--   0        0        0     1877 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/config.py
+-rw-r--r--   0        0        0      950 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/create.py
+-rw-r--r--   0        0        0     2170 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/delete.py
+-rw-r--r--   0        0        0     1426 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/describe.py
+-rw-r--r--   0        0        0     8430 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/download.py
+-rw-r--r--   0        0        0     3822 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/list.py
+-rw-r--r--   0        0        0     2500 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/pause.py
+-rw-r--r--   0        0        0     3951 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/reset.py
+-rw-r--r--   0        0        0      986 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/resume.py
+-rw-r--r--   0        0        0      312 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/commands/version.py
+-rw-r--r--   0        0        0     5652 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/ascend_io_cli/support.py
+-rw-r--r--   0        0        0     1232 2023-03-06 16:32:14.889472 ascend_io_cli-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 ascend_io_cli-1.0.8/setup.py
+-rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 ascend_io_cli-1.0.8/PKG-INFO
```

### Comparing `ascend_io_cli-1.0.6/LICENSE` & `ascend_io_cli-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ascend_io_cli-1.0.6/README.rst` & `ascend_io_cli-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/__init__.py` & `ascend_io_cli-1.0.8/ascend_io_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/cli.py` & `ascend_io_cli-1.0.8/ascend_io_cli/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 import glob
 import importlib
 import os
 
 import typer
 
-from ascend_io_cli.support import (OutputFormat, hostname_callback, max_workers_callback, output_callback, verbosity_callback)
+from ascend_io_cli.support import (OutputFormat, hostname_callback, max_workers_callback, output_callback, verbosity_callback, verify_ssl_callback)
 
 # Loop through all commands and add them as sub-commands here.
 app = typer.Typer(name='ascend')
 for path in glob.glob(os.path.join(os.path.dirname(__file__), 'commands', '*.py')):
   name = os.path.basename(path)[:-3]
   if name != '__init__':
     module = importlib.import_module(f'ascend_io_cli.commands.{name}')
@@ -24,13 +24,14 @@
         None,
         show_default=False,
         callback=hostname_callback,
         help='Hostname to use',
         is_eager=True,
     ),
     max_workers: int = typer.Option(10, callback=max_workers_callback, help='Maximum threads to use', is_eager=True),
+    verify_ssl: bool = typer.Option(True, callback=verify_ssl_callback, is_eager=True, hidden=True, show_default=False),
 ):
   pass
 
 
 if __name__ == "__main__":
   app()
```

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/commands/apply.py` & `ascend_io_cli-1.0.8/ascend_io_cli/commands/apply.py`

 * *Files identical despite different names*

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/commands/clone.py` & `ascend_io_cli-1.0.8/ascend_io_cli/commands/clone.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,39 +77,39 @@
   )
 
 
 def _hydrate_component(data_service_id: str, dataflow_id: str, component_id: str, base_dir: str):
   v2_name = Path(base_dir).resolve().joinpath(f'{component_id}.py')
   file = next(filter(lambda x: os.path.exists(x), [v2_name]), None)
   if not file:
-    raise Exception(f"component file for {data_service_id}.{dataflow_id}.{component_id} not found in {base_dir}")
+    raise Exception(f"component file for {data_service_id}.{dataflow_id}.{component_id} not found at {base_dir}")
   logging.debug(f'Loading at {file}')
   spec = importlib.util.spec_from_file_location("local", file)
   module_d = importlib.util.module_from_spec(spec)
   spec.loader.exec_module(module_d)
   return vars(module_d)['component']
 
 
 def _hydrate_dataflow(data_service_id: str, dataflow_id: str, new_data_service_id, new_dataflow_id: str, base_dir: str):
   v2_name = Path(base_dir).resolve().joinpath(f'{dataflow_id}.py')
   file = next(filter(lambda x: os.path.exists(x), [v2_name]), None)
   if not file:
-    raise Exception(f"dataflow file for {data_service_id} not found in {v2_name}")
+    raise Exception(f"dataflow file for {data_service_id}.{dataflow_id} not found at {v2_name}")
   logging.debug(f'Loading at {file}')
   spec = importlib.util.spec_from_file_location("local", file)
   module_d = importlib.util.module_from_spec(spec)
   spec.loader.exec_module(module_d)
   return vars(module_d)['construct_dataflow'](new_data_service_id, new_dataflow_id)
 
 
 def _hydrate_data_service(data_service_id: str, new_data_service_id: str, base_dir: str):
   v2_name = Path(base_dir).resolve().joinpath(f'{data_service_id}.py')
   file = next(filter(lambda x: os.path.exists(x), [v2_name]), None)
   if not file:
-    raise Exception(f"dataservice file for {data_service_id} not found in {base_dir}")
+    raise Exception(f"dataservice file for {data_service_id} not found at {base_dir}")
   logging.debug(f'Loading at {file}')
   spec = importlib.util.spec_from_file_location("local", file)
   module_d = importlib.util.module_from_spec(spec)
   spec.loader.exec_module(module_d)
   return vars(module_d)['construct_data_service'](new_data_service_id)
 
 
@@ -131,15 +131,15 @@
     logging.warning(f"Dataflow '{to_data_service}.{new_dataflow_id}' already exists")
     raise typer.Exit(101)
 
   with tempfile.TemporaryDirectory() as temp_dir:
     write_dir = Path(temp_dir).resolve().joinpath(f'{from_service}', f'{from_dataflow}')
     write_dir.mkdir(parents=True, exist_ok=True)
     download_dataflow(client, data_service_id=from_service, dataflow_id=from_dataflow, resource_base_path=str(write_dir), template_dir=template_dir)
-    hydrated = _hydrate_dataflow(from_service, from_dataflow, data_service_id, new_dataflow_id, write_dir)
+    hydrated = _hydrate_dataflow(from_service, from_dataflow, to_data_service, new_dataflow_id, str(write_dir))
     DataflowApplier(client).apply(data_service_id=to_data_service, dataflow=hydrated, delete=True, dry_run=False)
     print_response(ctx, hydrated)
 
 
 @app.command(name='data-service', help='Clone an existing data service')
 def clone_data_service(
     ctx: typer.Context,
```

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/commands/config.py` & `ascend_io_cli-1.0.8/ascend_io_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/commands/delete.py` & `ascend_io_cli-1.0.8/ascend_io_cli/commands/delete.py`

 * *Files identical despite different names*

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/commands/describe.py` & `ascend_io_cli-1.0.8/ascend_io_cli/commands/describe.py`

 * *Files identical despite different names*

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/commands/download.py` & `ascend_io_cli-1.0.8/ascend_io_cli/commands/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import concurrent
+import fnmatch
 import logging
 import os
 import shutil
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from pathlib import Path
+from typing import List
 
 import typer
 from ascend.sdk.render import TEMPLATES_V2, download_component, download_data_service, download_dataflow
 from google.protobuf.json_format import MessageToDict
 
 from ascend_io_cli.support import get_client, print_response
 
@@ -18,28 +20,68 @@
 def _configure_write_dir(write_dir: Path, unique: bool) -> Path:
   write_dir = write_dir.resolve().joinpath(f'{datetime.now().strftime("%Y%m%d%H%M%S") if unique else ""}')
   if not os.path.exists(write_dir):
     os.makedirs(write_dir, exist_ok=True)
   return write_dir
 
 
+def _load_ignore_matches(write_dir: Path) -> List[str]:
+  ignore = []
+  ignore_file = write_dir.joinpath('.ascendignore')
+  if ignore_file.exists():
+    with ignore_file.open('r', encoding='UTF-8') as file:
+      while line := file.readline():
+        line = line.strip()
+        if line:
+          ignore.append(line)
+  if '.git' not in ignore:
+    ignore.append('.git')
+  if '.ascendignore' not in ignore:
+    ignore.append('.ascendignore')
+  return ignore
+
+
+def _files_accepted(matches: List[str], base_dir: Path) -> List[str]:
+  """Identify the files that should be accepted for cleanup.
+  Ignores files that should be kept/preserved."""
+  accepted_files = []
+
+  for root, dirnames, filenames in os.walk(base_dir, topdown=True):
+    for dirname in dirnames:
+      for ignore in matches:
+        if fnmatch.fnmatch(dirname, ignore) or fnmatch.fnmatch(dirname + '/', ignore):
+          dirnames.remove(dirname) # remove any ignored directories from further consideration in os.walk
+
+    for filename in filenames:
+      full_file_path = os.path.join(root, filename)
+      keep_file = True
+      for ignore in matches:
+        if fnmatch.fnmatch(full_file_path, ignore) or fnmatch.fnmatch(filename, ignore) or filename == ignore:
+          keep_file = False
+          break
+      if keep_file:
+        accepted_files.append(full_file_path)
+
+  return accepted_files
+
+
 def _clean_write_dir(write_dir: Path, purge: bool):
-  """The purge option will also remove the .git folder"""
+  """The purge option will remove everything"""
   if write_dir and write_dir.exists():
+    assert write_dir != '/' # never remove root protection
+
     if purge:
       shutil.rmtree(write_dir)
     else:
-      for ls_dir in filter((lambda d: d != '.git'), os.listdir(write_dir)):
-        target = write_dir.joinpath(str(ls_dir))
-        if target.is_dir():
-          shutil.rmtree(target)
-        elif target.is_file():
-          os.remove(target)
-        else:
-          logging.debug(f'clean target was neither a file or a directory: {target}')
+      # assume .ascendignore in current working directory
+      ignore_files = _load_ignore_matches(Path('.'))
+      files = _files_accepted(ignore_files, write_dir)
+      files.reverse()
+      for f in files:
+        os.remove(f)
 
 
 @app.command()
 def data_service(
     ctx: typer.Context,
     data_service: str = typer.Argument(None, help='Data Service id to download', show_default=False),
     base_dir: str = typer.Option('./ascend', help='Base directory to write the service and flows'),
```

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/commands/list.py` & `ascend_io_cli-1.0.8/ascend_io_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/commands/pause.py` & `ascend_io_cli-1.0.8/ascend_io_cli/commands/pause.py`

 * *Files identical despite different names*

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/commands/reset.py` & `ascend_io_cli-1.0.8/ascend_io_cli/commands/reset.py`

 * *Files identical despite different names*

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/commands/resume.py` & `ascend_io_cli-1.0.8/ascend_io_cli/commands/resume.py`

 * *Files identical despite different names*

### Comparing `ascend_io_cli-1.0.6/ascend_io_cli/support.py` & `ascend_io_cli-1.0.8/ascend_io_cli/support.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,21 @@
 class CliOptions:
   def __init__(
       self,
       hostname: str = None,
       indent: int = None,
       output: str = None,
       workers: int = None,
+      verify_ssl: bool = True,
   ):
     self.indent = indent
     self.hostname = hostname
     self.output = output
     self.workers = workers
+    self.verify_ssl = verify_ssl
 
 
 def re_matcher(s: str, is_regex: bool):
   # if the expression is not a regex, treat it like a 'string contains' regular expression
   return re.compile(s if is_regex else ".*" + re.escape(s) + ".*", re.IGNORECASE) if not_blank(s) else None
 
 
@@ -173,14 +175,18 @@
     logger = logging.getLogger()
     logger.setLevel(verbosity)
     glog.setLevel(verbosity)
     logger.info(f'Logging verbosity changed to {verbosity}')
   return verbosity
 
 
+def verify_ssl_callback(ctx: typer.Context, value: bool):
+  _get_cli_options(ctx).verify_ssl = value
+
+
 def param_callback(
     ctx: typer.Context,
     param,
     value: any,
 ):
   _load_default_map(ctx)
   return value if value else ctx.default_map.get(param.name, None)
@@ -196,8 +202,12 @@
   opts = _get_cli_options(ctx)
   opts.hostname = final_value
   logging.debug(f'Using SDK host: {final_value}')
   return final_value
 
 
 def get_client(ctx: typer.Context):
-  return Client(_get_cli_options(ctx).hostname)
+  verify_ssl = _get_cli_options(ctx).verify_ssl
+  logging.debug(f'SSL Verification: {verify_ssl}')
+  if not verify_ssl:
+    logging.warning('SSL Verification Disabled!')
+  return Client(hostname=_get_cli_options(ctx).hostname, verify_ssl=verify_ssl)
```

### Comparing `ascend_io_cli-1.0.6/pyproject.toml` & `ascend_io_cli-1.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ascend-io-cli"
-version = "1.0.6"
+version = "1.0.8"
 description = "The Ascend CLI"
 license = "Apache-2.0"
 authors = ["Ascend.io Engineering <support@ascend.io>"]
 maintainers = ["Ascend.io Engineering <support@ascend.io>"]
 readme = "README.rst"
 homepage = "https://www.ascend.io"
 documentation = "https://developer.ascend.io"
@@ -17,21 +17,21 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 ascend-io-sdk = "^0.2.52"
 typer = { extras = ["all"], version = "^0.7.0" }
 tabulate = "^0.9.0"
-rich = "^12.5.0"
+rich = "^12.6.0"
 tomlkit = "^0.11.4"
 pipdeptree = "^2.3.1"
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
+pytest = "^7.2.1"
 twine = "^4.0.0"
 
 [tool.poetry.scripts]
 ascend = "ascend_io_cli.cli:app"
 
 [tool.poetry.urls]
 "Ascend.io" = "https://www.ascend.io"
```

### Comparing `ascend_io_cli-1.0.6/setup.py` & `ascend_io_cli-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'ascend-io-sdk>=0.2.52,<0.3.0',
  'pipdeptree>=2.3.1,<3.0.0',
- 'rich>=12.5.0,<13.0.0',
+ 'rich>=12.6.0,<13.0.0',
  'tabulate>=0.9.0,<0.10.0',
  'tomlkit>=0.11.4,<0.12.0',
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['ascend = ascend_io_cli.cli:app']}
 
 setup_kwargs = {
     'name': 'ascend-io-cli',
-    'version': '1.0.6',
+    'version': '1.0.8',
     'description': 'The Ascend CLI',
     'long_description': '=====================\nAscend.io CLI\n=====================\n\nThis package contains the `Ascend CLI <https://developer.ascend.io/docs/python-sdk>`_. The\nCLI is designed to make working with the Ascend.io platform simple and easy. This CLI\nwraps the `Ascend Python SDK <https://developer.ascend.io/docs/python-sdk>`_.\n\nGet help by passing ``--help`` into any command for a rundown of the syntax for each command.::\n\n ascend --help\n\nMake sure you are running the most current version::\n\n ascend version\n\nThe CLI can save default values for certain parameters. For example, to set a default hostname::\n\n ascend config set hostname my-ascendhost.company.io\n\nRemoving a default is as simple as::\n\n ascend config unset hostname\n\n---------------\nAuthentication\n---------------\nYou will want to download your API key from the Ascend UI. [Here is some documentation](https://developer.ascend.io/docs/python-sdk#getting-started)\nthat shows you how to get your key. Please keep your key secure!\n\n\n---------------\nRead the Docs\n---------------\n* `Ascend.io Python SDK Documentation <https://developer.ascend.io/docs/python-sdk>`_\n* `Ascend Developer Hub <https://developer.ascend.io>`_\n* `Ascend.io <https://www.ascend.io>`_\n',
     'author': 'Ascend.io Engineering',
     'author_email': 'support@ascend.io',
     'maintainer': 'Ascend.io Engineering',
     'maintainer_email': 'support@ascend.io',
     'url': 'https://www.ascend.io',
```

### Comparing `ascend_io_cli-1.0.6/PKG-INFO` & `ascend_io_cli-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascend-io-cli
-Version: 1.0.6
+Version: 1.0.8
 Summary: The Ascend CLI
 Home-page: https://www.ascend.io
 License: Apache-2.0
 Keywords: ascend,pipeline,data,automation,platform
 Author: Ascend.io Engineering
 Author-email: support@ascend.io
 Maintainer: Ascend.io Engineering
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: ascend-io-sdk (>=0.2.52,<0.3.0)
 Requires-Dist: pipdeptree (>=2.3.1,<3.0.0)
-Requires-Dist: rich (>=12.5.0,<13.0.0)
+Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tomlkit (>=0.11.4,<0.12.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: Ascend.io, https://www.ascend.io
 Project-URL: Ascend Developer Hub, https://developer.ascend.io
 Project-URL: Documentation, https://developer.ascend.io
 Description-Content-Type: text/x-rst
```

