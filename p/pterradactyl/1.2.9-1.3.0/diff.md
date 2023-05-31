# Comparing `tmp/pterradactyl-1.2.9.tar.gz` & `tmp/pterradactyl-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pterradactyl-1.2.9.tar", max compression
+gzip compressed data, was "pterradactyl-1.3.0.tar", max compression
```

## Comparing `pterradactyl-1.2.9.tar` & `pterradactyl-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0    10346 2021-12-21 15:25:54.034711 pterradactyl-1.2.9/LICENSE.md
--rw-r--r--   0        0        0     8039 2021-12-21 15:25:54.034711 pterradactyl-1.2.9/README.md
--rw-r--r--   0        0        0       85 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/__init__.py
--rw-r--r--   0        0        0      188 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/__main__.py
--rw-r--r--   0        0        0     1104 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/cli.py
--rw-r--r--   0        0        0        0 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/commands/__init__.py
--rw-r--r--   0        0        0      261 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/commands/base.py
--rw-r--r--   0        0        0      858 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/commands/dump.py
--rw-r--r--   0        0        0      129 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/commands/env.py
--rw-r--r--   0        0        0     2486 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/commands/lookup.py
--rw-r--r--   0        0        0     1418 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/commands/manifest.py
--rw-r--r--   0        0        0      140 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/commands/state.py
--rw-r--r--   0        0        0     4291 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/config.py
--rw-r--r--   0        0        0      938 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/facter/__init__.py
--rw-r--r--   0        0        0     1776 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/facter/arguments.py
--rw-r--r--   0        0        0      151 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/facter/base.py
--rw-r--r--   0        0        0      233 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/facter/environment.py
--rw-r--r--   0        0        0      362 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/facter/jinja.py
--rw-r--r--   0        0        0     1247 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/facter/regex.py
--rw-r--r--   0        0        0      987 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/facter/shell.py
--rw-r--r--   0        0        0     2000 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/facter/woops/manifest_path.py
--rw-r--r--   0        0        0        0 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/terraform/__init__.py
--rw-r--r--   0        0        0     3430 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/terraform/config.py
--rw-r--r--   0        0        0     9078 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/terraform/terraform.py
--rw-r--r--   0        0        0      699 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/util/__init__.py
--rw-r--r--   0        0        0     2016 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/util/download.py
--rw-r--r--   0        0        0     2721 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/util/filesystem.py
--rw-r--r--   0        0        0      125 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/util/package.py
--rw-r--r--   0        0        0      873 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/validator/__init__.py
--rw-r--r--   0        0        0      169 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/validator/base.py
--rw-r--r--   0        0        0      764 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pterradactyl/validator/version.py
--rw-r--r--   0        0        0     2825 2021-12-21 15:25:54.038711 pterradactyl-1.2.9/pyproject.toml
--rw-r--r--   0        0        0    13011 2021-12-21 15:26:02.271846 pterradactyl-1.2.9/setup.py
--rw-r--r--   0        0        0     9126 2021-12-21 15:26:02.272714 pterradactyl-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0    10346 2023-05-31 15:12:27.938916 pterradactyl-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     8039 2023-05-31 15:12:27.938916 pterradactyl-1.3.0/README.md
+-rw-r--r--   0        0        0       69 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/__init__.py
+-rw-r--r--   0        0        0      188 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/__main__.py
+-rw-r--r--   0        0        0     1082 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/cli.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/__init__.py
+-rw-r--r--   0        0        0      261 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/base.py
+-rw-r--r--   0        0        0      814 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/dump.py
+-rw-r--r--   0        0        0      129 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/env.py
+-rw-r--r--   0        0        0     2307 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/lookup.py
+-rw-r--r--   0        0        0     1407 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/manifest.py
+-rw-r--r--   0        0        0      140 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/state.py
+-rw-r--r--   0        0        0     4292 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/config.py
+-rw-r--r--   0        0        0      918 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/arguments.py
+-rw-r--r--   0        0        0      151 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/base.py
+-rw-r--r--   0        0        0      254 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/environment.py
+-rw-r--r--   0        0        0      384 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/jinja.py
+-rw-r--r--   0        0        0     1269 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/regex.py
+-rw-r--r--   0        0        0     1225 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/shell.py
+-rw-r--r--   0        0        0     2028 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/woops/manifest_path.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/terraform/__init__.py
+-rw-r--r--   0        0        0     3406 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/terraform/config.py
+-rw-r--r--   0        0        0     9344 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/terraform/terraform.py
+-rw-r--r--   0        0        0      699 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/util/__init__.py
+-rw-r--r--   0        0        0     2016 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/util/download.py
+-rw-r--r--   0        0        0     2721 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/util/filesystem.py
+-rw-r--r--   0        0        0      121 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/util/package.py
+-rw-r--r--   0        0        0      794 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/validator/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/validator/base.py
+-rw-r--r--   0        0        0      764 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/validator/version.py
+-rw-r--r--   0        0        0     2773 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9017 1970-01-01 00:00:00.000000 pterradactyl-1.3.0/PKG-INFO
```

### Comparing `pterradactyl-1.2.9/LICENSE.md` & `pterradactyl-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.2.9/README.md` & `pterradactyl-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.2.9/pterradactyl/cli.py` & `pterradactyl-1.3.0/pterradactyl/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import argparse
-import pkg_resources
 import os
 
 import pterradactyl
-
 from pterradactyl.config import Config
 from pterradactyl.util import package
 
 SKIP_PTERRA_YAML_ENC = os.environ.get("SKIP_PTERRA_YAML_ENC", False)
 
 
 def dispatch(argv):
```

### Comparing `pterradactyl-1.2.9/pterradactyl/commands/dump.py` & `pterradactyl-1.3.0/pterradactyl/commands/dump.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import os
 import yaml
 
 from pterradactyl.config import Config
 from pterradactyl.facter import Facter
-from pterradactyl.terraform.terraform import Terraform
 from pterradactyl.terraform.config import TerraformConfig
 
-from .base import AbstractBaseCommand
+from pterradactyl.commands.base import AbstractBaseCommand
 
 
 class AbstractDumpCommand(AbstractBaseCommand):
 
     def __init__(self, config, parser):
         super().__init__(config, parser)
```

### Comparing `pterradactyl-1.2.9/pterradactyl/commands/lookup.py` & `pterradactyl-1.3.0/pterradactyl/commands/lookup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-import os
-import yaml
-import phiera
 import logging
+import os
 
+import phiera
+import yaml
 from yaml.representer import SafeRepresenter
 
 from pterradactyl.config import Config
-from pterradactyl.facter import Facter
-from pterradactyl.validator import Validator
-from pterradactyl.terraform.terraform import Terraform
-from pterradactyl.terraform.config import TerraformConfig
 
-from .base import AbstractBaseCommand
+from pterradactyl.commands.base import AbstractBaseCommand
 
 log = logging.getLogger(__name__)
 
 
 class LookupCommand(AbstractBaseCommand):
     """ Performs a hiera lookup and dumps result as yaml"""
     subcommands = []
@@ -60,8 +56,8 @@
                     exit(1)
                 facts[key] = value
 
         context = {**facts, **{'facts': facts}}
         hiera = phiera.Hiera(config.get('hiera'), context=facts, base_path=config.dir)
         data = hiera.get(lookups[0], {}, merge=dict, merge_deep=True)
         yaml.add_representer(phiera.util.LookupDict, SafeRepresenter.represent_dict)
-        log.info(yaml.dump(dict(data), explicit_start=True))
+        print(yaml.dump(dict(data), explicit_start=True))
```

### Comparing `pterradactyl-1.2.9/pterradactyl/commands/manifest.py` & `pterradactyl-1.3.0/pterradactyl/commands/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import os
-
 from pterradactyl.config import Config
 from pterradactyl.facter import Facter
-from pterradactyl.validator import Validator
-from pterradactyl.terraform.terraform import Terraform
 from pterradactyl.terraform.config import TerraformConfig
+from pterradactyl.terraform.terraform import Terraform
+from pterradactyl.validator import Validator
 
 from .base import AbstractBaseCommand
 
 
 class ManifestCommand(AbstractBaseCommand):
     subcommands = []
```

### Comparing `pterradactyl-1.2.9/pterradactyl/config.py` & `pterradactyl-1.3.0/pterradactyl/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import os
-import yaml
 import logging
+import os
 import subprocess
+
+import yaml
 from appdirs import AppDirs
 from phiera import Merge
 
 log = logging.getLogger(__name__)
 
 """
 TODO - proper doc
```

### Comparing `pterradactyl-1.2.9/pterradactyl/facter/__init__.py` & `pterradactyl-1.3.0/pterradactyl/facter/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pterradactyl.config import Config
-from pterradactyl.util import lookup, package, merge_dict
+from pterradactyl.util import package
 
 
 class Facter(object):
     config = {}
     facts = {}
 
     def __init__(self):
```

### Comparing `pterradactyl-1.2.9/pterradactyl/facter/arguments.py` & `pterradactyl-1.3.0/pterradactyl/facter/arguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import os
-import re
 from argparse import Action
 
-from .base import BaseFacter
-from pterradactyl.config import Config
 from pterradactyl.util import as_list, lookup
 
+from pterradactyl.facter.base import BaseFacter
+
+
 class ArgumentsFacter(BaseFacter):
 
   def __init__(self, config):
     self.arg_specs = config
     self.actions = {}
 
   def parser_setup(self, parser):
```

### Comparing `pterradactyl-1.2.9/pterradactyl/facter/regex.py` & `pterradactyl-1.3.0/pterradactyl/facter/regex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import re
+
 import phiera
 from jinja2 import Environment
-from .base import BaseFacter
+
 from pterradactyl.config import Config
 
+from pterradactyl.facter.base import BaseFacter
+
 
 class RegexFacter(BaseFacter):
 
     def __init__(self, config):
         # XXX - todo config syntax check
         self.config = Config()
         self.source = config['source']
```

### Comparing `pterradactyl-1.2.9/pterradactyl/facter/woops/manifest_path.py` & `pterradactyl-1.3.0/pterradactyl/facter/woops/manifest_path.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # uncompyle6 version 3.3.4
 # Python bytecode 3.7 (3394)
 # Decompiled from: Python 3.7.3 (default, Mar 27 2019, 09:23:15) 
 # [Clang 10.0.1 (clang-1001.0.46.3)]
 # Embedded file name: /Users/rmk/Projects/pterra/pterradactyl/pterradactyl/facter/manifest_path.py
 # Size of source mod 2**32: 1517 bytes
-import os, re
+import os
+import re
 from argparse import Action
-from .base import BaseFacter
+
 from pterradactyl.config import Config
 
+from pterradactyl.facter.base import BaseFacter
+
+
 class ManifestPathFacter(BaseFacter):
 
     def __init__(self, config):
         self.path_specs = config
 
     def parser_setup(self, parser):
         self.action = PathFactActionFactory(Config().dir, self.path_specs)
```

### Comparing `pterradactyl-1.2.9/pterradactyl/terraform/config.py` & `pterradactyl-1.3.0/pterradactyl/terraform/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
+import json
 import os
 import re
-import json
-import yaml
+
 import phiera
 
 from pterradactyl.config import Config
-from pterradactyl.util import merge_dict, lookup
-
+from pterradactyl.util import lookup
 
 # XXX - this class is too "clever" for its own good. it's hard to follow.
 
 class TerraformConfig(object):
     alias_syntax = re.compile(r'(\S+) as (\S+)')
     properties = ['resource', 'provider', 'variable', 'output',
                   'local', 'module', 'data', 'terraform']
```

### Comparing `pterradactyl-1.2.9/pterradactyl/terraform/terraform.py` & `pterradactyl-1.3.0/pterradactyl/terraform/terraform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-import platform
+import glob
+import json
+import logging
 import os
+import platform
 import re
 import subprocess
 import sys
-import json
-import glob
-import requests
-import logging
-
 from pathlib import Path
+
+import requests
 from semantic_version import SimpleSpec, Version
+
 from pterradactyl.config import Config
 from pterradactyl.util import memoize
 from pterradactyl.util.download import download
-from pterradactyl.util.filesystem import ensure_executable, ensure_directory, sync_local_tf_plugins, check_stderr
-
-logging.basicConfig(level=logging.INFO, encoding='utf-8', format=None)
+from pterradactyl.util.filesystem import (check_stderr, ensure_directory,
+                                          ensure_executable,
+                                          sync_local_tf_plugins)
+
+LOG_FORMAT = '[%(asctime)s] [%(levelname)s] [%(process)s] [%(name)s] ' \
+             '[%(filename)s/%(funcName)s:%(lineno)d]: %(message)s'
+logging.basicConfig(level=logging.INFO, format=LOG_FORMAT)
 log = logging.getLogger(__name__)
 
 
 class Terraform(object):
     RELEASE_URL_PATTERN = 'https://releases.hashicorp.com/terraform/{version}/terraform_{version}_{os}_{arch}.zip'
     GITHUB_RELEASES_URL_PATTERN = 'https://api.{domain}/repos/{owner}/{repo}/releases'
 
@@ -122,15 +127,15 @@
     def ensure_plugins(self):
         for plugin in self.plugins:
             self.ensure_plugin(**plugin)
 
     def ensure_plugin(self, repo, owner, version, domain="github.com"):
         for plugin_bin in os.listdir(self.bin_dir):
             if plugin_bin.startswith(repo):
-                found_version = re.search('v(\d+.\d+.\d+)', plugin_bin)
+                found_version = re.search(r'v(\d+.\d+.\d+)', plugin_bin)
                 if found_version and \
                         Version(found_version.groups()[0]) in SimpleSpec(version):
                     break
                 else:
                     self.deprecate_plugin(plugin_bin)
 
         else:
@@ -167,15 +172,15 @@
         latest_release = ['0.0.0', '']
         releases_res = requests.get(self.GITHUB_RELEASES_URL_PATTERN.format(
             domain=domain,
             owner=owner,
             repo=repo
         ), headers=self.auth_headers.get(domain)).json()
         for r in releases_res:
-            version = r.get('tag_name').split('v')[1]
+            version = r.get("tag_name")[1:] if r.get("tag_name").startswith("v") else r.get("tag_name")
             if Version(version) in spec and Version(version) > Version(latest_release[0]):
                 for a in r['assets']:
                     asset_url = a['browser_download_url']
                     if platform.system().lower() in asset_url and \
                             self.__architecture_type() in asset_url:
                         latest_release[0] = version
                         latest_release[1] = a['url']
```

### Comparing `pterradactyl-1.2.9/pterradactyl/util/__init__.py` & `pterradactyl-1.3.0/pterradactyl/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.2.9/pterradactyl/util/download.py` & `pterradactyl-1.3.0/pterradactyl/util/download.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
-import tempfile
 import tarfile
-
+import tempfile
 from io import BytesIO
 from zipfile import ZipFile
+
 import requests
 
 
 def extract_from_zip(path, filename):
     archive = ZipFile(path)
 
     for member in archive.namelist():
```

### Comparing `pterradactyl-1.2.9/pterradactyl/util/filesystem.py` & `pterradactyl-1.3.0/pterradactyl/util/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import os
-import stat
 import json
 import logging
-
+import os
+import stat
 from pathlib import Path
 from shutil import copy
 
 log = logging.getLogger(__name__)
 
 def ensure_executable(path):
   st = os.stat(path)
@@ -62,8 +61,8 @@
         log.error(std_err.decode('utf-8'))
     except:
         log.error("Could not parse facts.json file at location: {}.\n Returning default error message.".format(facts_file))
         log.error(std_err.decode('utf-8'))
 
 def get_json(path):
     with open(path, "r") as stream:
-        return json.load(stream)
+        return json.load(stream)
```

### Comparing `pterradactyl-1.2.9/pterradactyl/validator/__init__.py` & `pterradactyl-1.3.0/pterradactyl/validator/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import os
-import re
+from pterradactyl.util import package
 
-from pterradactyl.config import Config
-from pterradactyl.util import lookup, package, merge_dict
 
 class Validator(object):
 
   def __init__(self, root_module, facts):
     self.facts = facts
     self.root_module = root_module
     self.validators = package.entry_points('pterradactyl.validators')
```

### Comparing `pterradactyl-1.2.9/pterradactyl/validator/version.py` & `pterradactyl-1.3.0/pterradactyl/validator/version.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
-import pterradactyl
 
 from semantic_version import SimpleSpec, Version
 
+import pterradactyl
 from pterradactyl.config import Config
 from pterradactyl.validator.base import BaseValidator
 
 log = logging.getLogger(__name__)
 
 class VersionValidator(BaseValidator):
```

### Comparing `pterradactyl-1.2.9/pyproject.toml` & `pterradactyl-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pterradactyl"
-version = "1.2.9"
+version = "1.3.0"
 description = "hiera-inspired terraform wrapper"
 authors = ["Rob King <rob.king@nike.com>",
            "Vincent Liu <vincent.liu@nike.com>"
 ]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
@@ -14,31 +14,25 @@
 ]
 packages = [
     { include = "pterradactyl" },
 ]
 repository = "https://github.com/Nike-Inc/pterradactyl"
 
 [tool.poetry.dependencies]
-python = "^3.7 || ^3.8"
+python = "^3.10.10"
 python-interface = "^1.5.3"
-pyyaml = "^5.3.1"
+pyyaml = "^6.0.0"
 jinja2 = "^2.11.1"
+MarkupSafe = "2.0.1"
 appdirs = "^1.4.3"
 jsonpath-ng = "^1.5.1"
 semantic_version = "^2.8.4"
-phiera = "^2.0.13"
+phiera = "^2.1.0"
 requests = "^2.24.0"
 
-[tool.poetry.dev-dependencies]
-pytest = { version = ">=4.6.9" }
-pytest-cov = { version = ">=3.0.0"}
-mock = { version = ">=3.0.4" }
-responses = { version = "^0.4.0" }
-testfixtures = { version = "6.18.3"}
-
 [tool.poetry.scripts]
 pt = "pterradactyl.__main__:main"
 
 [tool.poetry.plugins."pterradactyl.registered_commands"]
 apply = "pterradactyl.commands.manifest:ManifestCommand"
 console = "pterradactyl.commands.manifest:ManifestCommand"
 destroy = "pterradactyl.commands.manifest:ManifestCommand"
@@ -70,10 +64,17 @@
 environment = "pterradactyl.facter.environment:EnvironmentFacter"
 regex = "pterradactyl.facter.regex:RegexFacter"
 
 
 [tool.poetry.plugins."pterradactyl.validators"]
 version = "pterradactyl.validator.version:VersionValidator"
 
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+pytest-cov = "^4.1.0"
+testfixtures = "^7.1.0"
+responses = "^0.23.1"
+
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pterradactyl-1.2.9/PKG-INFO` & `pterradactyl-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: pterradactyl
-Version: 1.2.9
+Version: 1.3.0
 Summary: hiera-inspired terraform wrapper
 Home-page: https://github.com/Nike-Inc/pterradactyl
 License: Apache-2.0
 Author: Rob King
 Author-email: rob.king@nike.com
 Maintainer: Mohamed Abdul Huq Ismail
 Maintainer-email: Abdul.Ismail@nike.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.10.10,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: MarkupSafe (==2.0.1)
 Requires-Dist: appdirs (>=1.4.3,<2.0.0)
 Requires-Dist: jinja2 (>=2.11.1,<3.0.0)
 Requires-Dist: jsonpath-ng (>=1.5.1,<2.0.0)
-Requires-Dist: phiera (>=2.0.13,<3.0.0)
+Requires-Dist: phiera (>=2.1.0,<3.0.0)
 Requires-Dist: python-interface (>=1.5.3,<2.0.0)
-Requires-Dist: pyyaml (>=5.3.1,<6.0.0)
+Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
 Requires-Dist: requests (>=2.24.0,<3.0.0)
 Requires-Dist: semantic_version (>=2.8.4,<3.0.0)
 Project-URL: Repository, https://github.com/Nike-Inc/pterradactyl
 Description-Content-Type: text/markdown
 
 Pterradactyl
 ---
```

