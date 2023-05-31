# Comparing `tmp/mech_client-0.1.4.tar.gz` & `tmp/mech_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mech_client-0.1.4.tar", max compression
+gzip compressed data, was "mech_client-0.1.5.tar", max compression
```

## Comparing `mech_client-0.1.4.tar` & `mech_client-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11339 2023-05-27 20:23:22.952168 mech_client-0.1.4/LICENSE
--rw-r--r--   0        0        0     2037 2023-05-30 10:09:38.116752 mech_client-0.1.4/README.md
--rw-r--r--   0        0        0       22 2023-05-30 20:37:48.076470 mech_client-0.1.4/mech_client/__init__.py
--rw-r--r--   0        0        0     1147 2023-05-30 08:36:18.724247 mech_client-0.1.4/mech_client/cli.py
--rw-r--r--   0        0        0     7414 2023-05-30 20:39:00.456129 mech_client-0.1.4/mech_client/interact.py
--rw-r--r--   0        0        0     1790 2023-05-27 19:55:10.151934 mech_client-0.1.4/mech_client/prompt_to_ipfs.py
--rw-r--r--   0        0        0     1670 2023-05-27 20:02:06.617746 mech_client-0.1.4/mech_client/push_to_ipfs.py
--rw-r--r--   0        0        0      558 2023-05-30 20:37:50.024123 mech_client-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 mech_client-0.1.4/setup.py
--rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 mech_client-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-05-27 20:23:22.952168 mech_client-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2037 2023-05-30 10:09:38.116752 mech_client-0.1.5/README.md
+-rw-r--r--   0        0        0       22 2023-05-31 14:34:24.312320 mech_client-0.1.5/mech_client/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-30 08:36:18.724247 mech_client-0.1.5/mech_client/cli.py
+-rw-r--r--   0        0        0     7403 2023-05-31 14:33:42.501031 mech_client-0.1.5/mech_client/interact.py
+-rw-r--r--   0        0        0     1779 2023-05-31 14:33:42.502514 mech_client-0.1.5/mech_client/prompt_to_ipfs.py
+-rw-r--r--   0        0        0     1659 2023-05-31 14:33:42.503191 mech_client-0.1.5/mech_client/push_to_ipfs.py
+-rw-r--r--   0        0        0      558 2023-05-31 14:34:19.506035 mech_client-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 mech_client-0.1.5/setup.py
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 mech_client-0.1.5/PKG-INFO
```

### Comparing `mech_client-0.1.4/LICENSE` & `mech_client-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.4/README.md` & `mech_client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.4/mech_client/cli.py` & `mech_client-0.1.5/mech_client/cli.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.4/mech_client/interact.py` & `mech_client-0.1.5/mech_client/interact.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 Usage:
 
 python client.py <prompt> <tool>
 """
 
 import json
 import os
-import sys
 import time
 import warnings
 from typing import Any, Dict, Optional
 
 import requests
 import websocket
 from aea.contracts.base import Contract
```

### Comparing `mech_client-0.1.4/mech_client/prompt_to_ipfs.py` & `mech_client-0.1.5/mech_client/prompt_to_ipfs.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 Usage:
 
 python push_to_ipfs.py <prompt> <tool>
 """
 
 import json
 import shutil
-import sys
 import tempfile
 import uuid
 from typing import Tuple
 
 from mech_client.push_to_ipfs import push_to_ipfs
```

### Comparing `mech_client-0.1.4/mech_client/push_to_ipfs.py` & `mech_client-0.1.5/mech_client/push_to_ipfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 This script allows pushing a file directly to IPFS.
 
 Usage:
 
 python push_to_ipfs.py <file_path>
 """
 
-import sys
 from typing import Tuple
 
 import multibase
 import multicodec
 from aea.helpers.cid import to_v1
 from aea_cli_ipfs.ipfs_utils import IPFSTool
```

### Comparing `mech_client-0.1.4/pyproject.toml` & `mech_client-0.1.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "mech-client"
-version = "0.1.4"
+version = "0.1.5"
 description = "Basic client to interact with a mech"
 authors = ["David Minarsch <david.minarsch@googlemail.com>"]
 readme = "README.md"
 packages = [{include = "mech_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-open-aea = {version = "1.33.0", extras = ["cli"]}
-open-aea-ledger-ethereum = "1.33.0"
-open-aea-cli-ipfs = "1.33.0"
+open-aea = {version = "1.34.0", extras = ["cli"]}
+open-aea-ledger-ethereum = "1.34.0"
+open-aea-cli-ipfs = "1.34.0"
 websocket-client = ">=0.32.0,<1"
 
 [tool.poetry.scripts]
 mechx = "mech_client.cli:cli"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `mech_client-0.1.4/setup.py` & `mech_client-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['mech_client']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['open-aea-cli-ipfs==1.33.0',
- 'open-aea-ledger-ethereum==1.33.0',
- 'open-aea[cli]==1.33.0',
+['open-aea-cli-ipfs==1.34.0',
+ 'open-aea-ledger-ethereum==1.34.0',
+ 'open-aea[cli]==1.34.0',
  'websocket-client>=0.32.0,<1']
 
 entry_points = \
 {'console_scripts': ['mechx = mech_client.cli:cli']}
 
 setup_kwargs = {
     'name': 'mech-client',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Basic client to interact with a mech',
     'long_description': '# mech-client\nBasic client to interact with a mech\n\n> **Warning**<br />\n> **This is a hacky alpha version of the client - don\'t rely on it as production software.**\n\n## Installation\n\n```bash\npip install mech-client\n```\n\nThen, set a websocket endpoint for Gnosis RPC like so:\n\n```bash\nexport WEBSOCKET_ENDPOINT=<YOUR ENDPOINT>\n```\n\n## CLI:\n\n```bash\nUsage: mechx [OPTIONS] COMMAND [ARGS]...\n\n  Command-line tool for interacting with mechs.\n\nOptions:\n  --version  Show the version and exit.\n  --help     Show this message and exit.\n\nCommands:\n  interact        Interact with a mech specifying a prompt and tool.\n  prompt-to-ipfs  Upload a prompt and tool to IPFS as metadata.\n  push-to-ipfs    Upload a file to IPFS.\n ```\n\n## Usage:\n\nFirst, create a private key in file `ethereum_private_key.txt` with this command:\n\n```bash\naea generate-key ethereum\n```\n\nEnsure the private key carries funds on Gnosis Chain.\n\nSecond, run the following command to instruct the mech with `<prompt>` and `<tool>`:\n\n```bash\nmechx interact <prompt> <tool>\n```\n\nExample output:\n```bash\nmechx interact "write a short poem" "openai-text-davinci-003"\nPrompt uploaded: https://gateway.autonolas.tech/ipfs/f01701220ad9e2d5698fbd6c3a4ce61f329590e68a23181772669e543e69decdae316423b\nTransaction sent: https://gnosisscan.io/tx/0xb3a17ef90da6cc7a86e008a3a91bd367d573b406eae53405a4aa981001a5eaf3\nRequest on-chain with id: 15263135923206312300456917202469137903009897852865973093832667165921851537677\nData arrived: https://gateway.autonolas.tech/ipfs/f017012205053a4ae3ef0cf4ed7eff0c2d74dbaf3479fbdeb292472560e7bfaa4cfecfcdc\nData: {\'requestId\': 15263135923206312300456917202469137903009897852865973093832667165921851537677, \'result\': "\\n\\nA sun-filled sky,\\nA soft breeze blowing by,\\nWhere the trees sway in the wind,\\nA peaceful moment I can\'t rewind."}\n```\n\n## Release guide:\n\nFinish edits, bump versions in `pyproject.toml` and `mech_client/__init__.py`, then `poetry lock`, then `rm -rf dist`, then `poetry publish --build --username=<username> --password=<password>`.',
     'author': 'David Minarsch',
     'author_email': 'david.minarsch@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mech_client-0.1.4/PKG-INFO` & `mech_client-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mech-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: Basic client to interact with a mech
 Author: David Minarsch
 Author-email: david.minarsch@googlemail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: open-aea-cli-ipfs (==1.33.0)
-Requires-Dist: open-aea-ledger-ethereum (==1.33.0)
-Requires-Dist: open-aea[cli] (==1.33.0)
+Requires-Dist: open-aea-cli-ipfs (==1.34.0)
+Requires-Dist: open-aea-ledger-ethereum (==1.34.0)
+Requires-Dist: open-aea[cli] (==1.34.0)
 Requires-Dist: websocket-client (>=0.32.0,<1)
 Description-Content-Type: text/markdown
 
 # mech-client
 Basic client to interact with a mech
 
 > **Warning**<br />
```

