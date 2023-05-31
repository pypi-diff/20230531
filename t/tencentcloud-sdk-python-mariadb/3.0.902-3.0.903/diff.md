# Comparing `tmp/tencentcloud-sdk-python-mariadb-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-mariadb-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mariadb-3.0.902.tar", last modified: Tue May 30 00:27:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mariadb-3.0.903.tar", last modified: Wed May 31 02:15:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mariadb-3.0.902.tar` & `tencentcloud-sdk-python-mariadb-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud_sdk_python_mariadb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud_sdk_python_mariadb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud_sdk_python_mariadb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud_sdk_python_mariadb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/mariadb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/mariadb/v20170312/
--rw-r--r--   0 root         (0) root         (0)    70802 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/mariadb/v20170312/mariadb_client.py
--rw-r--r--   0 root         (0) root         (0)    14808 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/mariadb/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/mariadb/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   217944 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/mariadb/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/mariadb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:27:16.000000 tencentcloud-sdk-python-mariadb-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud_sdk_python_mariadb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud_sdk_python_mariadb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud_sdk_python_mariadb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud_sdk_python_mariadb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/mariadb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/mariadb/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    70802 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/mariadb/v20170312/mariadb_client.py
+-rw-r--r--   0 root         (0) root         (0)    14808 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/mariadb/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/mariadb/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   217944 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/mariadb/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/mariadb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:15:18.000000 tencentcloud-sdk-python-mariadb-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mariadb
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Mariadb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.902/README.rst` & `tencentcloud-sdk-python-mariadb-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/mariadb/v20170312/mariadb_client.py` & `tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/mariadb/v20170312/mariadb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/mariadb/v20170312/errorcodes.py` & `tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/mariadb/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.902/tencentcloud/mariadb/v20170312/models.py` & `tencentcloud-sdk-python-mariadb-3.0.903/tencentcloud/mariadb/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-mariadb-3.0.903/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mariadb
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Mariadb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.902/setup.py` & `tencentcloud-sdk-python-mariadb-3.0.903/setup.py`

 * *Files identical despite different names*

