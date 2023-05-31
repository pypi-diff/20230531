# Comparing `tmp/stac-asset-0.0.2.tar.gz` & `tmp/stac-asset-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-asset-0.0.2.tar", last modified: Thu May 25 12:58:39 2023, max compression
+gzip compressed data, was "stac-asset-0.0.3.tar", last modified: Wed May 31 21:50:05 2023, max compression
```

## Comparing `stac-asset-0.0.2.tar` & `stac-asset-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-25 12:58:39.684466 stac-asset-0.0.2/
--rw-r--r--   0 gadomski   (501) staff       (20)    11357 2023-05-23 19:38:34.000000 stac-asset-0.0.2/LICENSE
--rw-r--r--   0 gadomski   (501) staff       (20)     5673 2023-05-25 12:58:39.684062 stac-asset-0.0.2/PKG-INFO
--rw-r--r--   0 gadomski   (501) staff       (20)     5077 2023-05-25 12:54:26.000000 stac-asset-0.0.2/README.md
--rw-r--r--   0 gadomski   (501) staff       (20)     1041 2023-05-25 12:56:18.000000 stac-asset-0.0.2/pyproject.toml
--rw-r--r--   0 gadomski   (501) staff       (20)       38 2023-05-25 12:58:39.684572 stac-asset-0.0.2/setup.cfg
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-25 12:58:39.664889 stac-asset-0.0.2/src/
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-25 12:58:39.673429 stac-asset-0.0.2/src/stac_asset/
--rw-r--r--   0 gadomski   (501) staff       (20)     6030 2023-05-25 12:54:26.000000 stac-asset-0.0.2/src/stac_asset/__init__.py
--rw-r--r--   0 gadomski   (501) staff       (20)      393 2023-05-25 12:54:26.000000 stac-asset-0.0.2/src/stac_asset/__main__.py
--rw-r--r--   0 gadomski   (501) staff       (20)     5726 2023-05-25 12:54:26.000000 stac-asset-0.0.2/src/stac_asset/client.py
--rw-r--r--   0 gadomski   (501) staff       (20)      116 2023-05-24 12:12:03.000000 stac-asset-0.0.2/src/stac_asset/constants.py
--rw-r--r--   0 gadomski   (501) staff       (20)     1016 2023-05-25 12:54:26.000000 stac-asset-0.0.2/src/stac_asset/filesystem_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)     1453 2023-05-25 12:54:26.000000 stac-asset-0.0.2/src/stac_asset/http_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)     3601 2023-05-25 12:54:26.000000 stac-asset-0.0.2/src/stac_asset/planetary_computer_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)     2013 2023-05-25 12:54:26.000000 stac-asset-0.0.2/src/stac_asset/s3_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)      666 2023-05-24 12:09:09.000000 stac-asset-0.0.2/src/stac_asset/types.py
--rw-r--r--   0 gadomski   (501) staff       (20)     2596 2023-05-25 12:54:26.000000 stac-asset-0.0.2/src/stac_asset/usgs_eros_client.py
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-25 12:58:39.677840 stac-asset-0.0.2/src/stac_asset.egg-info/
--rw-r--r--   0 gadomski   (501) staff       (20)     5673 2023-05-25 12:58:39.000000 stac-asset-0.0.2/src/stac_asset.egg-info/PKG-INFO
--rw-r--r--   0 gadomski   (501) staff       (20)      694 2023-05-25 12:58:39.000000 stac-asset-0.0.2/src/stac_asset.egg-info/SOURCES.txt
--rw-r--r--   0 gadomski   (501) staff       (20)        1 2023-05-25 12:58:39.000000 stac-asset-0.0.2/src/stac_asset.egg-info/dependency_links.txt
--rw-r--r--   0 gadomski   (501) staff       (20)      236 2023-05-25 12:58:39.000000 stac-asset-0.0.2/src/stac_asset.egg-info/requires.txt
--rw-r--r--   0 gadomski   (501) staff       (20)       11 2023-05-25 12:58:39.000000 stac-asset-0.0.2/src/stac_asset.egg-info/top_level.txt
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-25 12:58:39.683166 stac-asset-0.0.2/tests/
--rw-r--r--   0 gadomski   (501) staff       (20)      864 2023-05-24 18:24:31.000000 stac-asset-0.0.2/tests/test_download.py
--rw-r--r--   0 gadomski   (501) staff       (20)      986 2023-05-25 12:54:26.000000 stac-asset-0.0.2/tests/test_filesystem_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)      813 2023-05-24 18:24:31.000000 stac-asset-0.0.2/tests/test_open.py
--rw-r--r--   0 gadomski   (501) staff       (20)      704 2023-05-25 12:54:26.000000 stac-asset-0.0.2/tests/test_planetary_computer_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)     1070 2023-05-25 12:54:26.000000 stac-asset-0.0.2/tests/test_s3_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)      869 2023-05-25 12:54:26.000000 stac-asset-0.0.2/tests/test_usgs_eros_client.py
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-31 21:50:05.937831 stac-asset-0.0.3/
+-rw-r--r--   0 gadomski   (501) staff       (20)    11357 2023-05-23 19:38:34.000000 stac-asset-0.0.3/LICENSE
+-rw-r--r--   0 gadomski   (501) staff       (20)     6706 2023-05-31 21:50:05.937168 stac-asset-0.0.3/PKG-INFO
+-rw-r--r--   0 gadomski   (501) staff       (20)     6110 2023-05-26 20:55:38.000000 stac-asset-0.0.3/README.md
+-rw-r--r--   0 gadomski   (501) staff       (20)     1041 2023-05-31 21:48:19.000000 stac-asset-0.0.3/pyproject.toml
+-rw-r--r--   0 gadomski   (501) staff       (20)       38 2023-05-31 21:50:05.938099 stac-asset-0.0.3/setup.cfg
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-31 21:50:05.912603 stac-asset-0.0.3/src/
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-31 21:50:05.924307 stac-asset-0.0.3/src/stac_asset/
+-rw-r--r--   0 gadomski   (501) staff       (20)     1233 2023-05-26 20:55:38.000000 stac-asset-0.0.3/src/stac_asset/__init__.py
+-rw-r--r--   0 gadomski   (501) staff       (20)      393 2023-05-25 12:54:26.000000 stac-asset-0.0.3/src/stac_asset/__main__.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     6420 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/client.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     1178 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/earthdata_client.py
+-rw-r--r--   0 gadomski   (501) staff       (20)      615 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/errors.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     1022 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/filesystem_client.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     4389 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/functions.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     1459 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/http_client.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     3749 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/planetary_computer_client.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     2129 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/s3_client.py
+-rw-r--r--   0 gadomski   (501) staff       (20)      370 2023-05-26 20:10:27.000000 stac-asset-0.0.3/src/stac_asset/strategy.py
+-rw-r--r--   0 gadomski   (501) staff       (20)      780 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/types.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     2602 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/usgs_eros_client.py
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-31 21:50:05.930077 stac-asset-0.0.3/src/stac_asset.egg-info/
+-rw-r--r--   0 gadomski   (501) staff       (20)     6706 2023-05-31 21:50:05.000000 stac-asset-0.0.3/src/stac_asset.egg-info/PKG-INFO
+-rw-r--r--   0 gadomski   (501) staff       (20)      812 2023-05-31 21:50:05.000000 stac-asset-0.0.3/src/stac_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 gadomski   (501) staff       (20)        1 2023-05-31 21:50:05.000000 stac-asset-0.0.3/src/stac_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 gadomski   (501) staff       (20)      236 2023-05-31 21:50:05.000000 stac-asset-0.0.3/src/stac_asset.egg-info/requires.txt
+-rw-r--r--   0 gadomski   (501) staff       (20)       11 2023-05-31 21:50:05.000000 stac-asset-0.0.3/src/stac_asset.egg-info/top_level.txt
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-31 21:50:05.936149 stac-asset-0.0.3/tests/
+-rw-r--r--   0 gadomski   (501) staff       (20)      353 2023-05-31 21:36:43.000000 stac-asset-0.0.3/tests/test_download.py
+-rw-r--r--   0 gadomski   (501) staff       (20)      707 2023-05-26 20:58:46.000000 stac-asset-0.0.3/tests/test_earthdata_client.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     2156 2023-05-26 20:29:22.000000 stac-asset-0.0.3/tests/test_filesystem_client.py
+-rw-r--r--   0 gadomski   (501) staff       (20)      416 2023-05-25 20:46:44.000000 stac-asset-0.0.3/tests/test_open.py
+-rw-r--r--   0 gadomski   (501) staff       (20)      704 2023-05-25 19:53:19.000000 stac-asset-0.0.3/tests/test_planetary_computer_client.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     1187 2023-05-26 13:07:26.000000 stac-asset-0.0.3/tests/test_s3_client.py
+-rw-r--r--   0 gadomski   (501) staff       (20)      869 2023-05-25 12:54:26.000000 stac-asset-0.0.3/tests/test_usgs_eros_client.py
```

### Comparing `stac-asset-0.0.2/LICENSE` & `stac-asset-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.2/PKG-INFO` & `stac-asset-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.0.2
+Version: 0.0.3
 Summary: Read, download, and write STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: repository, https://github.com/gadomski/stac-asset
 Project-URL: changelog, https://github.com/gadomski/stac-asset/blob/main/CHANGELOG.md
 Keywords: stac,async
 Classifier: Programming Language :: Python :: 3
@@ -22,60 +22,79 @@
 [![PyPI](https://img.shields.io/pypi/v/stac-asset?style=for-the-badge)](https://pypi.org/project/stac-asset)
 
 Download STAC Assets using a variety of authentication schemes.
 
 ## Installation
 
 ```shell
-pip install git+https://github.com/gadomski/stac-async
+pip install stac-asset
 ```
 
 ## Usage
 
-Download a STAC [Item](https://github.com/radiantearth/stac-spec/blob/master/item-spec/item-spec.md) and all of its assets to a local directory.
-Each Asset's href will be updated to point to the local file.
+Here's how to download a STAC [Item](https://github.com/radiantearth/stac-spec/blob/master/item-spec/item-spec.md) and all of its assets to a local directory using the top-level function.
+The correct [client](#clients) will be guessed from the assets' href.
+Each asset's href will be updated to point to the local file.
 
 ```python
-import stac_async
+import stac_asset
 
 href = "https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json"
-await stac_async.download_item_from_href(href, ".")
+await stac_asset.download_item_from_href(href, ".")
 ```
 
 To download an item using the command line:
 
 ```python
 python -m stac_asset https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json .
 ```
 
+See [the documentation](https://stac-asset.readthedocs.io/en/stable/index.html) for more examples and complete API documentation.
+
 ### Clients
 
 This library comes with several clients, each tailored for a specific data provider model and authentication scheme.
 Some clients require some setup before use; they are called out in this table, and the details are provided below.
 
 | Name | Description | Notes |
 | -- | -- | -- |
 | `HttpClient` | Simple HTTP client without any authentication | |
 | `S3Client` | Simple S3 client | Use `requester_pays=True` in the client initializer to enable access to requester pays buckets, e.g. USGS landsat's public AWS archive |
 | `FilesystemClient` | Moves files from place to place on a local filesystem | Mostly used for testing |
 | `PlanetaryComputerClient` | Signs urls with the [Planetary Computer Authentication API](https://planetarycomputer.microsoft.com/docs/reference/sas/) | No additional setup required, works out of the box |
 | `UsgsErosClient` | Uses a token-based authentication workflow to download data, e.g. landsat, from USGS EROS | Requires creation of a personal access token, see section below |
+| `EarthdataClient` | Uses a token-based authentication to download data, from _some_ Earthdata providers, e.g. DAACs | Requires creation of a personal access token, see section below |
+
+### S3Client
+
+To use the `requester_pays` option, you need to configure your AWS credentials.
+See [the AWS documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html) for instructions.
 
 #### USGS EROS
 
 The USGS EROS system, which hosts landsat data, requires a personal access token to download assets.
 Here's how to create and use your personal access token with **stac-asset**:
 
 1. [Create a new personal access token](https://ers.cr.usgs.gov/password/appgenerate)
 2. Set two environment variables:
     - `USGS_EROS_USERNAME` to your username (found in the top right of the web UI)
     - `USGS_EROS_PAT` to your personal access token
-3. Use `UsgsErosClient.login()` to create a new client.
+3. Use `UsgsErosClient.default()` to create a new client.
+
+You can also provide your username and password to the `UsgsErosClient.login` method.
+
+#### Earthdata
+
+You'll need a personal access token.
+
+1. Create a new personal access token by going to <https://urs.earthdata.nasa.gov/profile> and then clicking "Generate Token" (you'll need to log in).
+2. Set an enviornment variable named `EARTHDATA_PAT` to your token.
+3. Use `EarthdataClient.default()` to create a new client.
 
-You can also provide your username and password to the `login` method.
+You can also provide your token directly to `EarthdataClient.login()`.
 
 ## Design goals
 
 As determined during a meeting at the Element 84 offices (formerly Azavea offices) on 2023-05-24.
 
 - [x] `async`-first
 - [ ] Allow range requests
@@ -101,39 +120,39 @@
 - [ ] CLI
 
 ## Contributing
 
 Use Github [issues](https://github.com/gadomski/stac-asset/issues) to report bugs and request new features.
 Use Github [pull requests](https://github.com/gadomski/stac-asset/pulls) to fix bugs and propose new features.
 
-### Developing
+## Developing
 
 Clone, install with the dev dependencies, and install **pre-commit**:
 
 ```shell
 git clone git@github.com:gadomski/stac-asset.git
 cd stac-asset
 pip install '.[dev]'
 pre-commit install
 ```
 
-#### Testing
+### Testing
 
 All network-touching tests are disabled by default, because we can't use [pytest-vcr](https://pytest-vcr.readthedocs.io/en/latest/) (<https://github.com/kevin1024/vcrpy/issues/597>), and repeatedly hitting the network during testing and CI is bad behavior.
 To enable network-touching tests:
 
 ```shell
 pytest --network-access
 ```
 
 Some tests are client-specific and need your environment to be configured correctly.
 See [each client's documentation](#clients) for instructions on setting up your environment for each client.
 If your environment is not configured for a certain client, that client's tests are skipped.
 
-#### Docs
+### Docs
 
 Install the documentation dependencies:
 
 ```shell
 pip install -e '.[docs]'
 ```
```

### Comparing `stac-asset-0.0.2/README.md` & `stac-asset-0.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -5,60 +5,79 @@
 [![PyPI](https://img.shields.io/pypi/v/stac-asset?style=for-the-badge)](https://pypi.org/project/stac-asset)
 
 Download STAC Assets using a variety of authentication schemes.
 
 ## Installation
 
 ```shell
-pip install git+https://github.com/gadomski/stac-async
+pip install stac-asset
 ```
 
 ## Usage
 
-Download a STAC [Item](https://github.com/radiantearth/stac-spec/blob/master/item-spec/item-spec.md) and all of its assets to a local directory.
-Each Asset's href will be updated to point to the local file.
+Here's how to download a STAC [Item](https://github.com/radiantearth/stac-spec/blob/master/item-spec/item-spec.md) and all of its assets to a local directory using the top-level function.
+The correct [client](#clients) will be guessed from the assets' href.
+Each asset's href will be updated to point to the local file.
 
 ```python
-import stac_async
+import stac_asset
 
 href = "https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json"
-await stac_async.download_item_from_href(href, ".")
+await stac_asset.download_item_from_href(href, ".")
 ```
 
 To download an item using the command line:
 
 ```python
 python -m stac_asset https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json .
 ```
 
+See [the documentation](https://stac-asset.readthedocs.io/en/stable/index.html) for more examples and complete API documentation.
+
 ### Clients
 
 This library comes with several clients, each tailored for a specific data provider model and authentication scheme.
 Some clients require some setup before use; they are called out in this table, and the details are provided below.
 
 | Name | Description | Notes |
 | -- | -- | -- |
 | `HttpClient` | Simple HTTP client without any authentication | |
 | `S3Client` | Simple S3 client | Use `requester_pays=True` in the client initializer to enable access to requester pays buckets, e.g. USGS landsat's public AWS archive |
 | `FilesystemClient` | Moves files from place to place on a local filesystem | Mostly used for testing |
 | `PlanetaryComputerClient` | Signs urls with the [Planetary Computer Authentication API](https://planetarycomputer.microsoft.com/docs/reference/sas/) | No additional setup required, works out of the box |
 | `UsgsErosClient` | Uses a token-based authentication workflow to download data, e.g. landsat, from USGS EROS | Requires creation of a personal access token, see section below |
+| `EarthdataClient` | Uses a token-based authentication to download data, from _some_ Earthdata providers, e.g. DAACs | Requires creation of a personal access token, see section below |
+
+### S3Client
+
+To use the `requester_pays` option, you need to configure your AWS credentials.
+See [the AWS documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html) for instructions.
 
 #### USGS EROS
 
 The USGS EROS system, which hosts landsat data, requires a personal access token to download assets.
 Here's how to create and use your personal access token with **stac-asset**:
 
 1. [Create a new personal access token](https://ers.cr.usgs.gov/password/appgenerate)
 2. Set two environment variables:
     - `USGS_EROS_USERNAME` to your username (found in the top right of the web UI)
     - `USGS_EROS_PAT` to your personal access token
-3. Use `UsgsErosClient.login()` to create a new client.
+3. Use `UsgsErosClient.default()` to create a new client.
+
+You can also provide your username and password to the `UsgsErosClient.login` method.
+
+#### Earthdata
+
+You'll need a personal access token.
+
+1. Create a new personal access token by going to <https://urs.earthdata.nasa.gov/profile> and then clicking "Generate Token" (you'll need to log in).
+2. Set an enviornment variable named `EARTHDATA_PAT` to your token.
+3. Use `EarthdataClient.default()` to create a new client.
 
-You can also provide your username and password to the `login` method.
+You can also provide your token directly to `EarthdataClient.login()`.
 
 ## Design goals
 
 As determined during a meeting at the Element 84 offices (formerly Azavea offices) on 2023-05-24.
 
 - [x] `async`-first
 - [ ] Allow range requests
@@ -84,39 +103,39 @@
 - [ ] CLI
 
 ## Contributing
 
 Use Github [issues](https://github.com/gadomski/stac-asset/issues) to report bugs and request new features.
 Use Github [pull requests](https://github.com/gadomski/stac-asset/pulls) to fix bugs and propose new features.
 
-### Developing
+## Developing
 
 Clone, install with the dev dependencies, and install **pre-commit**:
 
 ```shell
 git clone git@github.com:gadomski/stac-asset.git
 cd stac-asset
 pip install '.[dev]'
 pre-commit install
 ```
 
-#### Testing
+### Testing
 
 All network-touching tests are disabled by default, because we can't use [pytest-vcr](https://pytest-vcr.readthedocs.io/en/latest/) (<https://github.com/kevin1024/vcrpy/issues/597>), and repeatedly hitting the network during testing and CI is bad behavior.
 To enable network-touching tests:
 
 ```shell
 pytest --network-access
 ```
 
 Some tests are client-specific and need your environment to be configured correctly.
 See [each client's documentation](#clients) for instructions on setting up your environment for each client.
 If your environment is not configured for a certain client, that client's tests are skipped.
 
-#### Docs
+### Docs
 
 Install the documentation dependencies:
 
 ```shell
 pip install -e '.[docs]'
 ```
```

### Comparing `stac-asset-0.0.2/pyproject.toml` & `stac-asset-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stac-asset"
-version = "0.0.2"
+version = "0.0.3"
 description = "Read, download, and write STAC assets across platforms and providers"
 authors = [
     {name = "Pete Gadomski", email = "pete.gadomski@gmail.com"}
 ]
 readme = "README.md"
 keywords = ["stac", "async"]
 classifiers = [
@@ -24,15 +24,15 @@
 [project.optional-dependencies]
 dev = [
     "black~=23.3",
     "mypy~=1.3",
     "pre-commit~=3.3",
     "pytest~=7.3",
     "pytest-asyncio~=0.21",
-    "ruff==0.0.269",
+    "ruff==0.0.270",
     "types-aiofiles~=23.1",
 ]
 docs = [
     "pydata-sphinx-theme~=0.13",
     "sphinx~=7.0",
 ]
```

### Comparing `stac-asset-0.0.2/src/stac_asset/__init__.py` & `stac-asset-0.0.3/src/stac_asset/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-"""Get STAC Assets from various platforms and using different authentication schemes.
-
-The core class is :py:class:`Client`, which defines a common interface.
-Other clients inherit from :py:class:`Client` to implement any custom behavior.
-"""
-
 import json
-from typing import AsyncIterator, Optional
+from typing import AsyncIterator, Optional, Type
 
-from pystac import Asset, Item
+from pystac import Item
 from yarl import URL
 
 from .client import Client
-from .constants import DEFAULT_ASSET_FILE_NAME
 from .filesystem_client import FilesystemClient
 from .http_client import HttpClient
 from .planetary_computer_client import PlanetaryComputerClient
 from .s3_client import S3Client
 from .types import PathLikeObject
 from .usgs_eros_client import UsgsErosClient
 
@@ -30,84 +23,51 @@
         AsyncIterator[bytes]: An iterator over the file's bytes.
     """
     async with await guess_client(href) as client:
         async for chunk in client.open_href(href):
             yield chunk
 
 
-async def open_asset(asset: Asset) -> AsyncIterator[bytes]:
-    """Open a STAC Asset.
-
-    Args:
-        asset: The Asset to open.
-
-    Returns:
-        AsyncIterator[bytes]: An iterator over the Asset's bytes.
-    """
-    async with await guess_client(asset.href) as client:
-        async for chunk in client.open_href(asset.href):
-            yield chunk
-
-
 async def download_href(href: str, path: PathLikeObject) -> None:
     """Download a file to the given path.
 
     The path's directory must exist.
 
     Args:
         href: The href to download.
         path: The location of the downloaded file.
     """
     async with await guess_client(href) as client:
         await client.download_href(href, path)
 
 
-async def download_asset(
-    asset: Asset,
-    directory: PathLikeObject,
-    make_directory: bool = False,
-    asset_file_name: str = DEFAULT_ASSET_FILE_NAME,
-) -> None:
-    """Download a STAC Asset into the given directory.
-
-    The file at the asset's href is downloaded into the directory. The asset is
-    also downloaded into the directory, and its href is updated to point to the
-    local file.
-
-    Args:
-        asset: The Asset to download.
-        directory: The location of the downloaded file and Asset.
-        make_directory: If true, create the directory (with exists_ok=True)
-            before downloading.
-    """
-    async with await guess_client(asset.href) as client:
-        await client.download_asset(asset, directory, make_directory, asset_file_name)
-
-
 async def download_item(
     item: Item,
     directory: PathLikeObject,
     make_directory: bool = False,
     item_file_name: Optional[str] = None,
     include_self_link: bool = True,
-) -> None:
+) -> Item:
     """Downloads an item to the local filesystem.
 
     Args:
         item: The :py:class:`pystac.Item`.
         directory: The output directory that will hold the items and assets.
         make_directory: Whether to create the directory if it doesn't exist.
         item_file_name: The file name of the output item. If not provided, will
             default to the item's id with a .json extension.
         include_self_link: Whether to include a self link in the output item.
+
+    Returns:
+        Item: The `~pystac.Item`, with the updated asset hrefs.
     """
     if not item.assets:
         raise ValueError("cannot guess a client if an item does not have any assets")
     async with await guess_client(next(iter(item.assets.values())).href) as client:
-        await client.download_item(
+        return await client.download_item(
             item, directory, make_directory, item_file_name, include_self_link
         )
 
 
 async def download_item_from_href(
     href: str,
     directory: PathLikeObject,
@@ -161,36 +121,19 @@
         href: The input href.
 
     Yields:
         Client: The most appropriate client for the href, maybe.
     """
     url = URL(href)
     if not url.host:
-        client_type: type[Client] = FilesystemClient
+        client_type: Type[Client] = FilesystemClient
     elif url.host.endswith("blob.core.windows.net"):
         client_type = PlanetaryComputerClient
     elif url.host == "https://landsatlook.usgs.gov":
         client_type = UsgsErosClient
     elif url.scheme == "http" or url.scheme == "https":
         client_type = HttpClient
     elif url.scheme == "s3":
         client_type = S3Client
     else:
         client_type = FilesystemClient
     return await client_type.default()
-
-
-__all__ = [
-    "FilesystemClient",
-    "HttpClient",
-    "PlanetaryComputerClient",
-    "S3Client",
-    "UsgsErosClient",
-    "download_asset",
-    "download_href",
-    "download_item",
-    "download_item_from_href",
-    "guess_client",
-    "open_asset",
-    "open_href",
-    "read_file",
-]
```

### Comparing `stac-asset-0.0.2/src/stac_asset/client.py` & `stac-asset-0.0.3/src/stac_asset/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from __future__ import annotations
 
-import json
+import asyncio
 import os.path
+import warnings
 from abc import ABC, abstractmethod
-from asyncio import TaskGroup
+from asyncio import Task
 from pathlib import Path
 from types import TracebackType
-from typing import AsyncIterator, Optional, TypeVar
+from typing import Any, AsyncIterator, Dict, List, Optional, Type, TypeVar
 
 import aiofiles
 import pystac.utils
-from pystac import Asset, Item
+from pystac import Item
 from yarl import URL
 
-from .constants import DEFAULT_ASSET_FILE_NAME
+from .errors import (
+    AssetDownloadException,
+    AssetDownloadWarning,
+    AssetOverwriteException,
+)
+from .strategy import FileNameStrategy
 from .types import PathLikeObject
 
 T = TypeVar("T", bound="Client")
 
 
 class Client(ABC):
     """An abstract base class for all clients."""
 
     @classmethod
-    async def default(cls: type[T]) -> T:
+    async def default(cls: Type[T]) -> T:
         """Creates the default version of this client.
 
         We can't just use the initializer, because some clients need to do
         asynchronous actions during their setup.
 
         Returns:
             T: The default version of this Client.
@@ -56,110 +62,130 @@
 
         Yields:
             AsyncIterator[bytes]: An iterator over chunks of the read file
         """
         async for chunk in self.open_url(URL(href)):
             yield chunk
 
-    async def open_asset(self, asset: Asset) -> AsyncIterator[bytes]:
-        """Opens an asset and yields an iterator over its bytes.
-
-        Args:
-            asset: The input asset
-
-        Yields:
-            AsyncIterator[bytes]: An iterator over chunks of the read file
-        """
-        async for chunk in self.open_href(asset.href):
-            yield chunk
-
-    async def download_href(self, href: str, path: PathLikeObject) -> None:
+    async def download_href(
+        self, href: str, path: PathLikeObject, clean: bool = True
+    ) -> None:
         """Downloads a file to the local filesystem.
 
         Args:
             href: The input href
             path: The ouput file path
+            clean: If an error occurs, delete the output file
         """
-        async with aiofiles.open(path, mode="wb") as f:
-            async for chunk in self.open_href(href):
-                await f.write(chunk)
-
-    async def download_asset(
-        self,
-        asset: Asset,
-        directory: PathLikeObject,
-        make_directory: bool = False,
-        asset_file_name: str = DEFAULT_ASSET_FILE_NAME,
-    ) -> None:
-        """Downloads a STAC Asset into the given directory.
-
-        The file at the asset's href is downloaded into the directory. The asset is
-        also downloaded into the directory, and its href is updated to point to the
-        local file.
-
-        Args:
-            asset: The Asset to download.
-            directory: The location of the downloaded file and Asset.
-            make_directory: If true, create the directory (with exists_ok=True)
-                before downloading.
-            asset_file_name: The name of the Asset json file in the directory.
-        """
-        directory_as_path = Path(directory)
-        if make_directory:
-            directory_as_path.mkdir(exist_ok=True)
-        path = directory_as_path / os.path.basename(asset.href)
-        await self.download_href(asset.href, path)
-        asset.href = str(path)
-        asset_as_str = json.dumps(asset.to_dict())
-        async with aiofiles.open(directory_as_path / asset_file_name, "w") as f:
-            await f.write(asset_as_str)
+        try:
+            async with aiofiles.open(path, mode="wb") as f:
+                async for chunk in self.open_href(href):
+                    await f.write(chunk)
+        except Exception as err:
+            path_as_path = Path(path)
+            if clean and path_as_path.exists():
+                try:
+                    path_as_path.unlink()
+                except Exception:
+                    pass
+            raise err
 
     async def download_item(
         self,
         item: Item,
         directory: PathLikeObject,
         make_directory: bool = False,
         item_file_name: Optional[str] = None,
         include_self_link: bool = True,
-    ) -> None:
+        asset_file_name_strategy: FileNameStrategy = FileNameStrategy.FILE_NAME,
+    ) -> Item:
         """Downloads all Assets in an item into the given directory.
 
         Args:
             item: The Item to download, along with its assets.
             directory: The location of the downloaded file and Asset.
             make_directory: If true, create the directory (with exists_ok=True)
                 before downloading.
             item_file_name: The name of the Item json file in the directory.
             include_self_link: Whether to include a self link on the item.
+
+        Returns:
+            Item: The `~pystac.Item`, with the updated asset hrefs.
         """
         directory_as_path = Path(directory)
         if make_directory:
             directory_as_path.mkdir(exist_ok=True)
+        elif not directory_as_path.exists():
+            raise FileNotFoundError(f"output directory does not exist: {directory}")
+
         if item_file_name is None:
             item_file_name = f"{item.id}.json"
         item_path = directory_as_path / item_file_name
-        async with TaskGroup() as task_group:
-            for key, asset in item.assets.items():
-                # TODO allow different layout schemes
-                path = directory_as_path / os.path.basename(asset.href)
-                absolute_href = asset.get_absolute_href()
-                if absolute_href is None:
-                    raise ValueError(f"asset '{key}' does not have an absolute href")
-                task_group.create_task(self.download_href(absolute_href, path))
+
+        tasks: List[Task[Any]] = list()
+        keys_to_delete = list()
+        file_names: Dict[str, str] = dict()
+        for key, asset in item.assets.items():
+            if asset_file_name_strategy == FileNameStrategy.FILE_NAME:
+                file_name = os.path.basename(URL(asset.href).path)
+            elif asset_file_name_strategy == FileNameStrategy.KEY:
+                file_name = key + Path(asset.href).suffix
+            path = directory_as_path / file_name
+            if file_name in file_names:
+                for task in tasks:
+                    task.cancel()
+                raise AssetOverwriteException(list(file_names.values()))
+            else:
+                file_names[file_name] = str(path)
+
+            absolute_href = asset.get_absolute_href()
+            if absolute_href is None:
+                warnings.warn(
+                    f"asset '{key}' does not have an absolute href",
+                    AssetDownloadWarning,
+                )
+                keys_to_delete.append(key)
+            else:
+                tasks.append(
+                    asyncio.create_task(self._download_asset(key, absolute_href, path))
+                )
                 item.assets[key].href = pystac.utils.make_relative_href(
                     str(path), str(item_path)
                 )
+        for key in keys_to_delete:
+            del item.assets[key]
+
+        results = await asyncio.gather(*tasks, return_exceptions=True)
+        for result in results:
+            if isinstance(result, AssetDownloadException):
+                warnings.warn(str(result), AssetDownloadWarning)
+                del item.assets[result.key]
+
+        new_links = list()
         for link in item.links:
-            if link.is_hierarchical():
+            link_href = link.get_href(transform_href=False)
+            if link_href and not pystac.utils.is_absolute_href(link_href):
                 link.target = pystac.utils.make_absolute_href(link.href, item.self_href)
-        item.save_object(include_self_link=include_self_link, dest_href=str(item_path))
+                new_links.append(link)
+        item.links = new_links
+
+        item.set_self_href(str(item_path))
+        item.save_object(include_self_link=include_self_link)
+
+        return item
+
+    async def _download_asset(self, key: str, href: str, path: Path) -> None:
+        try:
+            await self.download_href(href, path)
+        except Exception as e:
+            raise AssetDownloadException(key, href, e)
 
     async def __aenter__(self) -> Client:
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[type[BaseException]],
+        exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Optional[bool]:
         return None
```

### Comparing `stac-asset-0.0.2/src/stac_asset/filesystem_client.py` & `stac-asset-0.0.3/src/stac_asset/filesystem_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from types import TracebackType
-from typing import AsyncIterator, Optional
+from typing import AsyncIterator, Optional, Type
 
 import aiofiles
 from yarl import URL
 
 from .client import Client
 
 
@@ -26,12 +26,12 @@
                 yield chunk
 
     async def __aenter__(self) -> FilesystemClient:
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[type[BaseException]],
+        exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Optional[bool]:
         return None
```

### Comparing `stac-asset-0.0.2/src/stac_asset/http_client.py` & `stac-asset-0.0.3/src/stac_asset/http_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from types import TracebackType
-from typing import AsyncIterator, Optional, TypeVar
+from typing import AsyncIterator, Optional, Type, TypeVar
 
 from aiohttp import ClientSession
 from yarl import URL
 
 from .client import Client
 
 T = TypeVar("T", bound="HttpClient")
@@ -18,15 +18,15 @@
     Configure the session to customize its behavior.
     """
 
     session: ClientSession
     """A atiohttp session that will be used for all requests."""
 
     @classmethod
-    async def default(cls: type[T]) -> T:
+    async def default(cls: Type[T]) -> T:
         """Creates the default http client with a vanilla session object."""
         session = ClientSession()
         return cls(session)
 
     def __init__(self, session: ClientSession) -> None:
         super().__init__()
         self.session = session
@@ -38,13 +38,13 @@
                 yield chunk
 
     async def __aenter__(self) -> HttpClient:
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[type[BaseException]],
+        exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Optional[bool]:
         await self.session.close()
         return await super().__aexit__(exc_type, exc_val, exc_tb)
```

### Comparing `stac-asset-0.0.2/src/stac_asset/planetary_computer_client.py` & `stac-asset-0.0.3/src/stac_asset/planetary_computer_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 https://github.com/microsoft/planetary-computer-sdk-for-python/blob/main/planetary_computer/sas.py,
 thanks Tom Augspurger!
 """
 
 from __future__ import annotations
 
 import datetime
+from asyncio import Lock
 from datetime import timezone
 from types import TracebackType
-from typing import Any, AsyncIterator, Dict, Optional
+from typing import Any, AsyncIterator, Dict, Optional, Type
 
 from aiohttp import ClientSession
 from yarl import URL
 
 from .http_client import HttpClient
 
 DEFAULT_SAS_TOKEN_ENDPOINT = "https://planetarycomputer.microsoft.com/api/sas/v1/token"
 
 
 class _Token:
     expiry: datetime.datetime
     token: str
 
     @classmethod
-    def from_dict(cls, data: dict[str, Any]) -> _Token:
+    def from_dict(cls, data: Dict[str, Any]) -> _Token:
         try:
             expiry = datetime.datetime.fromisoformat(data["msft:expiry"])
         except KeyError:
             raise ValueError(f"missing 'msft:expiry' key in dict: {data}")
 
         try:
             token = data["token"]
@@ -47,23 +48,25 @@
 
     def __str__(self) -> str:
         return self.token
 
 
 class PlanetaryComputerClient(HttpClient):
     _cache: Dict[URL, _Token]
+    _cache_lock: Lock
     token_request_url: URL
 
     def __init__(
         self,
         session: ClientSession,
         sas_token_endpoint: str = DEFAULT_SAS_TOKEN_ENDPOINT,
     ) -> None:
         super().__init__(session)
         self._cache = dict()
+        self._cache_lock = Lock()
         self.sas_token_endpoint = URL(sas_token_endpoint)
 
     async def open_url(self, url: URL) -> AsyncIterator[bytes]:
         # We only need to modify the url if:
         #
         # - The url is in Azure blob storage
         # - The url is not in the public thumbnail storage account
@@ -84,26 +87,27 @@
         account_name = url.host.split(".")[0]
         container_name = url.path.split("/", 2)[1]
         token = await self._get_token(account_name, container_name)
         return URL(str(url.with_query(None)) + "?" + token, encoded=False)
 
     async def _get_token(self, account_name: str, container_name: str) -> str:
         url = self.sas_token_endpoint.joinpath(account_name, container_name)
-        token = self._cache.get(url)
-        if token is None or token.ttl() < 60:
-            response = await self.session.get(url)
-            response.raise_for_status()
-            token = _Token.from_dict(await response.json())
-            self._cache[url] = token
+        async with self._cache_lock:
+            token = self._cache.get(url)
+            if token is None or token.ttl() < 60:
+                response = await self.session.get(url)
+                response.raise_for_status()
+                token = _Token.from_dict(await response.json())
+                self._cache[url] = token
         return str(token)
 
     async def __aenter__(self) -> PlanetaryComputerClient:
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[type[BaseException]],
+        exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Optional[bool]:
         await self.session.close()
         return await super().__aexit__(exc_type, exc_val, exc_tb)
```

### Comparing `stac-asset-0.0.2/src/stac_asset/s3_client.py` & `stac-asset-0.0.3/src/stac_asset/s3_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from types import TracebackType
-from typing import AsyncIterator, Optional
+from typing import AsyncIterator, Optional, Type
 
 import aiobotocore.session
 from aiobotocore.session import AioSession
 from botocore import UNSIGNED
 from botocore.config import Config
 from yarl import URL
 
@@ -52,17 +52,20 @@
             }
             if self.requester_pays:
                 params["RequestPayer"] = "requester"
             response = await client.get_object(**params)
             async for chunk in response["Body"]:
                 yield chunk
 
+    async def has_credentials(self) -> bool:
+        return await self.session.get_credentials() is not None
+
     async def __aenter__(self) -> S3Client:
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[type[BaseException]],
+        exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Optional[bool]:
         return None
```

### Comparing `stac-asset-0.0.2/src/stac_asset/usgs_eros_client.py` & `stac-asset-0.0.3/src/stac_asset/usgs_eros_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import json
 import os
 from types import TracebackType
-from typing import Optional
+from typing import Optional, Type
 
 from aiohttp import ClientSession
 
 from .http_client import HttpClient
 
 
 class UsgsErosClient(HttpClient):
@@ -68,13 +68,13 @@
         )
 
     async def __aenter__(self) -> UsgsErosClient:
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[type[BaseException]],
+        exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Optional[bool]:
         await self.session.close()
         return await super().__aexit__(exc_type, exc_val, exc_tb)
```

### Comparing `stac-asset-0.0.2/src/stac_asset.egg-info/PKG-INFO` & `stac-asset-0.0.3/src/stac_asset.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.0.2
+Version: 0.0.3
 Summary: Read, download, and write STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: repository, https://github.com/gadomski/stac-asset
 Project-URL: changelog, https://github.com/gadomski/stac-asset/blob/main/CHANGELOG.md
 Keywords: stac,async
 Classifier: Programming Language :: Python :: 3
@@ -22,60 +22,79 @@
 [![PyPI](https://img.shields.io/pypi/v/stac-asset?style=for-the-badge)](https://pypi.org/project/stac-asset)
 
 Download STAC Assets using a variety of authentication schemes.
 
 ## Installation
 
 ```shell
-pip install git+https://github.com/gadomski/stac-async
+pip install stac-asset
 ```
 
 ## Usage
 
-Download a STAC [Item](https://github.com/radiantearth/stac-spec/blob/master/item-spec/item-spec.md) and all of its assets to a local directory.
-Each Asset's href will be updated to point to the local file.
+Here's how to download a STAC [Item](https://github.com/radiantearth/stac-spec/blob/master/item-spec/item-spec.md) and all of its assets to a local directory using the top-level function.
+The correct [client](#clients) will be guessed from the assets' href.
+Each asset's href will be updated to point to the local file.
 
 ```python
-import stac_async
+import stac_asset
 
 href = "https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json"
-await stac_async.download_item_from_href(href, ".")
+await stac_asset.download_item_from_href(href, ".")
 ```
 
 To download an item using the command line:
 
 ```python
 python -m stac_asset https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json .
 ```
 
+See [the documentation](https://stac-asset.readthedocs.io/en/stable/index.html) for more examples and complete API documentation.
+
 ### Clients
 
 This library comes with several clients, each tailored for a specific data provider model and authentication scheme.
 Some clients require some setup before use; they are called out in this table, and the details are provided below.
 
 | Name | Description | Notes |
 | -- | -- | -- |
 | `HttpClient` | Simple HTTP client without any authentication | |
 | `S3Client` | Simple S3 client | Use `requester_pays=True` in the client initializer to enable access to requester pays buckets, e.g. USGS landsat's public AWS archive |
 | `FilesystemClient` | Moves files from place to place on a local filesystem | Mostly used for testing |
 | `PlanetaryComputerClient` | Signs urls with the [Planetary Computer Authentication API](https://planetarycomputer.microsoft.com/docs/reference/sas/) | No additional setup required, works out of the box |
 | `UsgsErosClient` | Uses a token-based authentication workflow to download data, e.g. landsat, from USGS EROS | Requires creation of a personal access token, see section below |
+| `EarthdataClient` | Uses a token-based authentication to download data, from _some_ Earthdata providers, e.g. DAACs | Requires creation of a personal access token, see section below |
+
+### S3Client
+
+To use the `requester_pays` option, you need to configure your AWS credentials.
+See [the AWS documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html) for instructions.
 
 #### USGS EROS
 
 The USGS EROS system, which hosts landsat data, requires a personal access token to download assets.
 Here's how to create and use your personal access token with **stac-asset**:
 
 1. [Create a new personal access token](https://ers.cr.usgs.gov/password/appgenerate)
 2. Set two environment variables:
     - `USGS_EROS_USERNAME` to your username (found in the top right of the web UI)
     - `USGS_EROS_PAT` to your personal access token
-3. Use `UsgsErosClient.login()` to create a new client.
+3. Use `UsgsErosClient.default()` to create a new client.
+
+You can also provide your username and password to the `UsgsErosClient.login` method.
+
+#### Earthdata
+
+You'll need a personal access token.
+
+1. Create a new personal access token by going to <https://urs.earthdata.nasa.gov/profile> and then clicking "Generate Token" (you'll need to log in).
+2. Set an enviornment variable named `EARTHDATA_PAT` to your token.
+3. Use `EarthdataClient.default()` to create a new client.
 
-You can also provide your username and password to the `login` method.
+You can also provide your token directly to `EarthdataClient.login()`.
 
 ## Design goals
 
 As determined during a meeting at the Element 84 offices (formerly Azavea offices) on 2023-05-24.
 
 - [x] `async`-first
 - [ ] Allow range requests
@@ -101,39 +120,39 @@
 - [ ] CLI
 
 ## Contributing
 
 Use Github [issues](https://github.com/gadomski/stac-asset/issues) to report bugs and request new features.
 Use Github [pull requests](https://github.com/gadomski/stac-asset/pulls) to fix bugs and propose new features.
 
-### Developing
+## Developing
 
 Clone, install with the dev dependencies, and install **pre-commit**:
 
 ```shell
 git clone git@github.com:gadomski/stac-asset.git
 cd stac-asset
 pip install '.[dev]'
 pre-commit install
 ```
 
-#### Testing
+### Testing
 
 All network-touching tests are disabled by default, because we can't use [pytest-vcr](https://pytest-vcr.readthedocs.io/en/latest/) (<https://github.com/kevin1024/vcrpy/issues/597>), and repeatedly hitting the network during testing and CI is bad behavior.
 To enable network-touching tests:
 
 ```shell
 pytest --network-access
 ```
 
 Some tests are client-specific and need your environment to be configured correctly.
 See [each client's documentation](#clients) for instructions on setting up your environment for each client.
 If your environment is not configured for a certain client, that client's tests are skipped.
 
-#### Docs
+### Docs
 
 Install the documentation dependencies:
 
 ```shell
 pip install -e '.[docs]'
 ```
```

### Comparing `stac-asset-0.0.2/src/stac_asset.egg-info/SOURCES.txt` & `stac-asset-0.0.3/src/stac_asset.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
 src/stac_asset/__init__.py
 src/stac_asset/__main__.py
 src/stac_asset/client.py
-src/stac_asset/constants.py
+src/stac_asset/earthdata_client.py
+src/stac_asset/errors.py
 src/stac_asset/filesystem_client.py
+src/stac_asset/functions.py
 src/stac_asset/http_client.py
 src/stac_asset/planetary_computer_client.py
 src/stac_asset/s3_client.py
+src/stac_asset/strategy.py
 src/stac_asset/types.py
 src/stac_asset/usgs_eros_client.py
 src/stac_asset.egg-info/PKG-INFO
 src/stac_asset.egg-info/SOURCES.txt
 src/stac_asset.egg-info/dependency_links.txt
 src/stac_asset.egg-info/requires.txt
 src/stac_asset.egg-info/top_level.txt
 tests/test_download.py
+tests/test_earthdata_client.py
 tests/test_filesystem_client.py
 tests/test_open.py
 tests/test_planetary_computer_client.py
 tests/test_s3_client.py
 tests/test_usgs_eros_client.py
```

### Comparing `stac-asset-0.0.2/tests/test_planetary_computer_client.py` & `stac-asset-0.0.3/tests/test_planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.2/tests/test_s3_client.py` & `stac-asset-0.0.3/tests/test_s3_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,9 +26,11 @@
         assert os.path.getsize(tmp_path / "out.jpg") == 6060
 
 
 async def test_download_requester_pays(
     tmp_path: Path, requester_pays_href: str
 ) -> None:
     async with S3Client(requester_pays=True) as client:
+        if not await client.has_credentials():
+            pytest.skip("aws credentials are invalid or not present")
         await client.download_href(requester_pays_href, tmp_path / "out.jpg")
         assert os.path.getsize(tmp_path / "out.jpg") == 6114
```

### Comparing `stac-asset-0.0.2/tests/test_usgs_eros_client.py` & `stac-asset-0.0.3/tests/test_usgs_eros_client.py`

 * *Files identical despite different names*

