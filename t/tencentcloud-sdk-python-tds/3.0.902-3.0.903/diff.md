# Comparing `tmp/tencentcloud-sdk-python-tds-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-tds-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tds-3.0.902.tar", last modified: Tue May 30 00:33:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tds-3.0.903.tar", last modified: Wed May 31 02:22:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tds-3.0.902.tar` & `tencentcloud-sdk-python-tds-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud/tds/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud/tds/v20220801/
--rw-r--r--   0 root         (0) root         (0)     4532 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud/tds/v20220801/tds_client.py
--rw-r--r--   0 root         (0) root         (0)      717 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud/tds/v20220801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud/tds/v20220801/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15921 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud/tds/v20220801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud/tds/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud_sdk_python_tds.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud_sdk_python_tds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud_sdk_python_tds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud_sdk_python_tds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/tencentcloud_sdk_python_tds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:33:54.000000 tencentcloud-sdk-python-tds-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:22:28.000000 tencentcloud-sdk-python-tds-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:22:27.000000 tencentcloud-sdk-python-tds-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:22:28.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:22:28.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud/tds/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:22:28.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud/tds/v20220801/
+-rw-r--r--   0 root         (0) root         (0)     4532 2023-05-31 02:22:27.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud/tds/v20220801/tds_client.py
+-rw-r--r--   0 root         (0) root         (0)      717 2023-05-31 02:22:27.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud/tds/v20220801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:22:27.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud/tds/v20220801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15921 2023-05-31 02:22:27.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud/tds/v20220801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:22:27.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud/tds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:22:27.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:22:28.000000 tencentcloud-sdk-python-tds-3.0.903/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:22:28.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud_sdk_python_tds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:22:28.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud_sdk_python_tds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-31 02:22:28.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud_sdk_python_tds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:22:28.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud_sdk_python_tds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:22:28.000000 tencentcloud-sdk-python-tds-3.0.903/tencentcloud_sdk_python_tds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:22:27.000000 tencentcloud-sdk-python-tds-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:22:28.000000 tencentcloud-sdk-python-tds-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tds-3.0.902/README.rst` & `tencentcloud-sdk-python-tds-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tds-3.0.902/tencentcloud/tds/v20220801/tds_client.py` & `tencentcloud-sdk-python-tds-3.0.903/tencentcloud/tds/v20220801/tds_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tds-3.0.902/tencentcloud/tds/v20220801/errorcodes.py` & `tencentcloud-sdk-python-tds-3.0.903/tencentcloud/tds/v20220801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tds-3.0.902/tencentcloud/tds/v20220801/models.py` & `tencentcloud-sdk-python-tds-3.0.903/tencentcloud/tds/v20220801/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tds-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tds-3.0.903/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.902'
+__version__ = '3.0.903'
```

### Comparing `tencentcloud-sdk-python-tds-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-tds-3.0.903/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tds
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Tds SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tds-3.0.902/tencentcloud_sdk_python_tds.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tds-3.0.903/tencentcloud_sdk_python_tds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tds
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Tds SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tds-3.0.902/setup.py` & `tencentcloud-sdk-python-tds-3.0.903/setup.py`

 * *Files identical despite different names*

