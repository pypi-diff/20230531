# Comparing `tmp/pilot_platform_object_storage-1.1.0.tar.gz` & `tmp/pilot_platform_object_storage-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot_platform_object_storage-1.1.0.tar", max compression
+gzip compressed data, was "pilot_platform_object_storage-1.1.1.tar", max compression
```

## Comparing `pilot_platform_object_storage-1.1.0.tar` & `pilot_platform_object_storage-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3325 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/README.md
--rw-r--r--   0        0        0      120 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/__init__.py
--rw-r--r--   0        0        0      324 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/clients/__init__.py
--rw-r--r--   0        0        0     4506 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/clients/azure_blob_client.py
--rw-r--r--   0        0        0     5162 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/clients/azure_container_client.py
--rw-r--r--   0        0        0     2143 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/clients/base_container_client.py
--rw-r--r--   0        0        0     2051 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/clients/base_file_client.py
--rw-r--r--   0        0        0     1902 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/factories.py
--rw-r--r--   0        0        0      239 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/managers/__init__.py
--rw-r--r--   0        0        0     3751 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/managers/azure_blob_manager.py
--rw-r--r--   0        0        0      727 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/managers/base_manager.py
--rw-r--r--   0        0        0      196 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/providers/__init__.py
--rw-r--r--   0        0        0     4902 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/providers/azure.py
--rw-r--r--   0        0        0      444 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/providers/enum.py
--rw-r--r--   0        0        0     1009 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4265 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.1.0/setup.py
--rw-r--r--   0        0        0     3903 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3336 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/README.md
+-rw-r--r--   0        0        0      120 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/__init__.py
+-rw-r--r--   0        0        0      324 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/clients/__init__.py
+-rw-r--r--   0        0        0     4506 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/clients/azure_blob_client.py
+-rw-r--r--   0        0        0     5162 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/clients/azure_container_client.py
+-rw-r--r--   0        0        0     2143 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/clients/base_container_client.py
+-rw-r--r--   0        0        0     2051 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/clients/base_file_client.py
+-rw-r--r--   0        0        0     1902 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/factories.py
+-rw-r--r--   0        0        0      239 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/managers/__init__.py
+-rw-r--r--   0        0        0     3762 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/managers/azure_blob_manager.py
+-rw-r--r--   0        0        0      727 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/managers/base_manager.py
+-rw-r--r--   0        0        0      196 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/providers/__init__.py
+-rw-r--r--   0        0        0     4902 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/providers/azure.py
+-rw-r--r--   0        0        0      444 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/providers/enum.py
+-rw-r--r--   0        0        0     1009 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.1.1/setup.py
+-rw-r--r--   0        0        0     3914 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.1.1/PKG-INFO
```

### Comparing `pilot_platform_object_storage-1.1.0/README.md` & `pilot_platform_object_storage-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ```python
 import asyncio
 from object_storage.factories import get_manager
 
 connection_string = 'DefaultEndpointsProtocol=https;AccountName=pilot;AccountKey=any;EndpointSuffix=core.windows.net'
 azr_manager = get_manager('azure', connection_string)
 
-account_sas = asyncio.run(azr_manager.get_account_sas())
+account_sas = asyncio.run(azr_manager.get_container_sas('test'))
 print(blob_sas)
 > 'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature'
 
 
 blob_sas = asyncio.run(azr_manager.get_blob_sas('test', 'small.txt'))
 
 print(blob_sas)
@@ -38,26 +38,26 @@
 
 ### File Client
 ```python
 import asyncio
 from object_storage.factories import get_file_client
 
 blob_sas_url = 'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature'
-azr_account_client = get_file_client('azure', blob_sas_url)
-asyncio.run(azr_account_client.upload_file('./small.txt'))
+azr_file_client = get_file_client('azure', blob_sas_url)
+asyncio.run(azr_file_client.upload_file('./small.txt'))
 ```
 
 ### Container Client
 ```python
 import asyncio
 from object_storage.factories import get_container_client
 
 container_sas_url = 'https://pilot.blob.core.windows.net/test?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature'
-azr_account_client = get_file_client('azure', container_sas_url)
-asyncio.run(azr_account_client.upload_file('small.txt', './small.txt'))
+azr_container_client = get_container_client('azure', container_sas_url)
+asyncio.run(azr_container_client.upload_file('small.txt', './small.txt'))
 
 ```
 
 
 ## Installation & Quick Start
 The latest version of the object-storage package is available on [PyPi](https://pypi.org/project/pilot-platform-object-storage/) and can be installed into another service via Pip.
```

### Comparing `pilot_platform_object_storage-1.1.0/object_storage/clients/azure_blob_client.py` & `pilot_platform_object_storage-1.1.1/object_storage/clients/azure_blob_client.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.1.0/object_storage/clients/azure_container_client.py` & `pilot_platform_object_storage-1.1.1/object_storage/clients/azure_container_client.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.1.0/object_storage/clients/base_container_client.py` & `pilot_platform_object_storage-1.1.1/object_storage/clients/base_container_client.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.1.0/object_storage/clients/base_file_client.py` & `pilot_platform_object_storage-1.1.1/object_storage/clients/base_file_client.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.1.0/object_storage/factories.py` & `pilot_platform_object_storage-1.1.1/object_storage/factories.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.1.0/object_storage/managers/azure_blob_manager.py` & `pilot_platform_object_storage-1.1.1/object_storage/managers/azure_blob_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,8 +82,8 @@
                 account_name=service.account_name,
                 account_key=service.credential.account_key,
                 container_name=container,
                 permission=AccountSasPermissions(read=read, write=write, list=list, delete=delete),
                 start=datetime.utcnow(),
                 expiry=datetime.utcnow() + timedelta(hours=1),
             )
-        return f'{service.url}?{sas_token}'
+        return f'{service.url}{container}?{sas_token}'
```

### Comparing `pilot_platform_object_storage-1.1.0/object_storage/managers/base_manager.py` & `pilot_platform_object_storage-1.1.1/object_storage/managers/base_manager.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.1.0/object_storage/providers/azure.py` & `pilot_platform_object_storage-1.1.1/object_storage/providers/azure.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.1.0/pyproject.toml` & `pilot_platform_object_storage-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pilot-platform-object-storage"
-version = "1.1.0"
+version = "1.1.1"
 description = "Python library for interacting with multiple object storage APIs."
 authors = ["Indoc Research"]
 readme = "README.md"
 packages = [{include = "object_storage"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pilot_platform_object_storage-1.1.0/setup.py` & `pilot_platform_object_storage-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 install_requires = \
 ['aiofiles>=23.1.0,<24.0.0',
  'aiohttp>=3.8.4,<4.0.0',
  'azure-storage-blob>=12.16.0,<13.0.0']
 
 setup_kwargs = {
     'name': 'pilot-platform-object-storage',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'Python library for interacting with multiple object storage APIs.',
-    'long_description': '# Pilot Platform Storage Manager\n\n[![Run Tests](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml/badge.svg?branch=develop)](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml)\n[![Python](https://img.shields.io/badge/python-3.9-brightgreen.svg)](https://www.python.org/)\n[![PyPI](https://img.shields.io/pypi/v/pilot-platform-object-storage.svg)](https://pypi.org/project/pilot-platform-object-storage/)\n\nProvides a simple and flexible Python library for efficient and reliable object storage solutions. Enables direct interaction with multiple object storage APIs, starting with Azure Blob API and with plans to add more in the future\n\n\n## Getting Started\n\n### Manager\n```python\nimport asyncio\nfrom object_storage.factories import get_manager\n\nconnection_string = \'DefaultEndpointsProtocol=https;AccountName=pilot;AccountKey=any;EndpointSuffix=core.windows.net\'\nazr_manager = get_manager(\'azure\', connection_string)\n\naccount_sas = asyncio.run(azr_manager.get_account_sas())\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\n\n\nblob_sas = asyncio.run(azr_manager.get_blob_sas(\'test\', \'small.txt\'))\n\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=blob_signature\'\n\n\nblobs_list = asyncio.run(azr_manager.list_objects(\'test\'))\nprint(blobs_list)\n> [<class \'azure.storage.blob._models.BlobProperties\'>, ...]\n\n\nblobs_list = asyncio.run(azr_manager.create_container(\'test\'))\n```\n\n### File Client\n```python\nimport asyncio\nfrom object_storage.factories import get_file_client\n\nblob_sas_url = \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_account_client = get_file_client(\'azure\', blob_sas_url)\nasyncio.run(azr_account_client.upload_file(\'./small.txt\'))\n```\n\n### Container Client\n```python\nimport asyncio\nfrom object_storage.factories import get_container_client\n\ncontainer_sas_url = \'https://pilot.blob.core.windows.net/test?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_account_client = get_file_client(\'azure\', container_sas_url)\nasyncio.run(azr_account_client.upload_file(\'small.txt\', \'./small.txt\'))\n\n```\n\n\n## Installation & Quick Start\nThe latest version of the object-storage package is available on [PyPi](https://pypi.org/project/pilot-platform-object-storage/) and can be installed into another service via Pip.\n\nPip install from PyPi:\n```\npip install pilot-platform-object-storage\n```\n\nIn `pyproject.toml`:\n```\npilot-platform-object-storage = "^<VERSION>"\n```\n\nPip install from a local `.whl` file:\n```\npip install pilot_platform_object_storage-<VERSION>-py3-none-any.whl\n```\n\n## Contribution\n\nYou can contribute the project in following ways:\n\n* Report a bug.\n* Suggest a feature.\n* Open a pull request for fixing issues or adding functionality. Please consider using [pre-commit](https://pre-commit.com) in this case.\n* For general guidelines on how to contribute to the project, please take a look at the [contribution guide](CONTRIBUTING.md).\n',
+    'long_description': '# Pilot Platform Storage Manager\n\n[![Run Tests](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml/badge.svg?branch=develop)](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml)\n[![Python](https://img.shields.io/badge/python-3.9-brightgreen.svg)](https://www.python.org/)\n[![PyPI](https://img.shields.io/pypi/v/pilot-platform-object-storage.svg)](https://pypi.org/project/pilot-platform-object-storage/)\n\nProvides a simple and flexible Python library for efficient and reliable object storage solutions. Enables direct interaction with multiple object storage APIs, starting with Azure Blob API and with plans to add more in the future\n\n\n## Getting Started\n\n### Manager\n```python\nimport asyncio\nfrom object_storage.factories import get_manager\n\nconnection_string = \'DefaultEndpointsProtocol=https;AccountName=pilot;AccountKey=any;EndpointSuffix=core.windows.net\'\nazr_manager = get_manager(\'azure\', connection_string)\n\naccount_sas = asyncio.run(azr_manager.get_container_sas(\'test\'))\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\n\n\nblob_sas = asyncio.run(azr_manager.get_blob_sas(\'test\', \'small.txt\'))\n\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=blob_signature\'\n\n\nblobs_list = asyncio.run(azr_manager.list_objects(\'test\'))\nprint(blobs_list)\n> [<class \'azure.storage.blob._models.BlobProperties\'>, ...]\n\n\nblobs_list = asyncio.run(azr_manager.create_container(\'test\'))\n```\n\n### File Client\n```python\nimport asyncio\nfrom object_storage.factories import get_file_client\n\nblob_sas_url = \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_file_client = get_file_client(\'azure\', blob_sas_url)\nasyncio.run(azr_file_client.upload_file(\'./small.txt\'))\n```\n\n### Container Client\n```python\nimport asyncio\nfrom object_storage.factories import get_container_client\n\ncontainer_sas_url = \'https://pilot.blob.core.windows.net/test?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_container_client = get_container_client(\'azure\', container_sas_url)\nasyncio.run(azr_container_client.upload_file(\'small.txt\', \'./small.txt\'))\n\n```\n\n\n## Installation & Quick Start\nThe latest version of the object-storage package is available on [PyPi](https://pypi.org/project/pilot-platform-object-storage/) and can be installed into another service via Pip.\n\nPip install from PyPi:\n```\npip install pilot-platform-object-storage\n```\n\nIn `pyproject.toml`:\n```\npilot-platform-object-storage = "^<VERSION>"\n```\n\nPip install from a local `.whl` file:\n```\npip install pilot_platform_object_storage-<VERSION>-py3-none-any.whl\n```\n\n## Contribution\n\nYou can contribute the project in following ways:\n\n* Report a bug.\n* Suggest a feature.\n* Open a pull request for fixing issues or adding functionality. Please consider using [pre-commit](https://pre-commit.com) in this case.\n* For general guidelines on how to contribute to the project, please take a look at the [contribution guide](CONTRIBUTING.md).\n',
     'author': 'Indoc Research',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pilot_platform_object_storage-1.1.0/PKG-INFO` & `pilot_platform_object_storage-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-object-storage
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library for interacting with multiple object storage APIs.
 Author: Indoc Research
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -28,15 +28,15 @@
 ```python
 import asyncio
 from object_storage.factories import get_manager
 
 connection_string = 'DefaultEndpointsProtocol=https;AccountName=pilot;AccountKey=any;EndpointSuffix=core.windows.net'
 azr_manager = get_manager('azure', connection_string)
 
-account_sas = asyncio.run(azr_manager.get_account_sas())
+account_sas = asyncio.run(azr_manager.get_container_sas('test'))
 print(blob_sas)
 > 'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature'
 
 
 blob_sas = asyncio.run(azr_manager.get_blob_sas('test', 'small.txt'))
 
 print(blob_sas)
@@ -53,26 +53,26 @@
 
 ### File Client
 ```python
 import asyncio
 from object_storage.factories import get_file_client
 
 blob_sas_url = 'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature'
-azr_account_client = get_file_client('azure', blob_sas_url)
-asyncio.run(azr_account_client.upload_file('./small.txt'))
+azr_file_client = get_file_client('azure', blob_sas_url)
+asyncio.run(azr_file_client.upload_file('./small.txt'))
 ```
 
 ### Container Client
 ```python
 import asyncio
 from object_storage.factories import get_container_client
 
 container_sas_url = 'https://pilot.blob.core.windows.net/test?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature'
-azr_account_client = get_file_client('azure', container_sas_url)
-asyncio.run(azr_account_client.upload_file('small.txt', './small.txt'))
+azr_container_client = get_container_client('azure', container_sas_url)
+asyncio.run(azr_container_client.upload_file('small.txt', './small.txt'))
 
 ```
 
 
 ## Installation & Quick Start
 The latest version of the object-storage package is available on [PyPi](https://pypi.org/project/pilot-platform-object-storage/) and can be installed into another service via Pip.
```

