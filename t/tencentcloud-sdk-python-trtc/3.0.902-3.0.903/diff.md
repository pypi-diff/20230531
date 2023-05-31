# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.902.tar", last modified: Tue May 30 00:36:07 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.903.tar", last modified: Wed May 31 02:24:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.902.tar` & `tencentcloud-sdk-python-trtc-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)     9679 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)   198994 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)    58535 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:36:07.000000 tencentcloud-sdk-python-trtc-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   199184 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)    58535 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:24:52.000000 tencentcloud-sdk-python-trtc-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.902/README.rst` & `tencentcloud-sdk-python-trtc-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/trtc/v20190722/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,16 +208,18 @@
 0：腾讯云存储 COS，暂不支持其他家。
         :type Vendor: int
         :param Region: 第三方云存储的地域信息。
         :type Region: str
         :param Bucket: 第三方存储桶信息。
         :type Bucket: str
         :param AccessKey: 第三方存储的access_key账号信息。
+若存储至腾讯云COS，请前往https://console.cloud.tencent.com/cam/capi 查看或创建
         :type AccessKey: str
         :param SecretKey: 第三方存储的secret_key账号信息。
+若存储至腾讯云COS，请前往https://console.cloud.tencent.com/cam/capi 查看或创建
         :type SecretKey: str
         :param FileNamePrefix: 第三方云存储bucket 的指定位置，由字符串数组组成。合法的字符串范围a~z,A~Z,0~9,'_'和'-'，举个例子，录制文件xxx.m3u8在 ["prefix1", "prefix2"]作用下，会变成prefix1/prefix2/TaskId/xxx.m3u8。
         :type FileNamePrefix: list of str
         """
         self.Vendor = None
         self.Region = None
         self.Bucket = None
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.902/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.903/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.903/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.902/setup.py` & `tencentcloud-sdk-python-trtc-3.0.903/setup.py`

 * *Files identical despite different names*

