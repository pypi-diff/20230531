# Comparing `tmp/tencentcloud-sdk-python-gpm-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-gpm-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gpm-3.0.902.tar", last modified: Tue May 30 00:24:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gpm-3.0.903.tar", last modified: Wed May 31 02:12:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gpm-3.0.902.tar` & `tencentcloud-sdk-python-gpm-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:24:10.000000 tencentcloud-sdk-python-gpm-3.0.902/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:24:10.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud_sdk_python_gpm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:24:10.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud_sdk_python_gpm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:24:10.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud_sdk_python_gpm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:24:10.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud_sdk_python_gpm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:24:10.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud_sdk_python_gpm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:24:09.000000 tencentcloud-sdk-python-gpm-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:24:10.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:24:10.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/gpm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:24:10.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/gpm/v20200820/
--rw-r--r--   0 root         (0) root         (0)    18197 2023-05-30 00:24:09.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/gpm/v20200820/gpm_client.py
--rw-r--r--   0 root         (0) root         (0)     5641 2023-05-30 00:24:09.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/gpm/v20200820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:24:09.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/gpm/v20200820/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64177 2023-05-30 00:24:09.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/gpm/v20200820/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:24:09.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/gpm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:24:09.000000 tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:24:10.000000 tencentcloud-sdk-python-gpm-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:24:09.000000 tencentcloud-sdk-python-gpm-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:24:10.000000 tencentcloud-sdk-python-gpm-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud_sdk_python_gpm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud_sdk_python_gpm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud_sdk_python_gpm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud_sdk_python_gpm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud_sdk_python_gpm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/gpm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/gpm/v20200820/
+-rw-r--r--   0 root         (0) root         (0)    18197 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/gpm/v20200820/gpm_client.py
+-rw-r--r--   0 root         (0) root         (0)     5641 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/gpm/v20200820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/gpm/v20200820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64177 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/gpm/v20200820/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/gpm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:12:25.000000 tencentcloud-sdk-python-gpm-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-gpm-3.0.902/tencentcloud_sdk_python_gpm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gpm-3.0.903/tencentcloud_sdk_python_gpm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gpm
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Gpm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gpm-3.0.902/README.rst` & `tencentcloud-sdk-python-gpm-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/gpm/v20200820/gpm_client.py` & `tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/gpm/v20200820/gpm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/gpm/v20200820/errorcodes.py` & `tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/gpm/v20200820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/gpm/v20200820/models.py` & `tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/gpm/v20200820/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gpm-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gpm-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-gpm-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-gpm-3.0.903/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gpm
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Gpm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gpm-3.0.902/setup.py` & `tencentcloud-sdk-python-gpm-3.0.903/setup.py`

 * *Files identical despite different names*

