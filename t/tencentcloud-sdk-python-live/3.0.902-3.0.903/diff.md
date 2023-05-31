# Comparing `tmp/tencentcloud-sdk-python-live-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.902.tar", last modified: Tue May 30 00:26:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.903.tar", last modified: Wed May 31 02:15:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.902.tar` & `tencentcloud-sdk-python-live-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   137451 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    18117 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   433012 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:15:00.000000 tencentcloud-sdk-python-live-3.0.903/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:15:00.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:15:00.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-31 02:15:00.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-31 02:15:00.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:15:00.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-31 02:14:59.000000 tencentcloud-sdk-python-live-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:15:00.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:15:00.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:15:00.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   137451 2023-05-31 02:14:59.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    18117 2023-05-31 02:14:59.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:14:59.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   433012 2023-05-31 02:14:59.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:14:59.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:14:59.000000 tencentcloud-sdk-python-live-3.0.903/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-31 02:15:00.000000 tencentcloud-sdk-python-live-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-31 02:14:59.000000 tencentcloud-sdk-python-live-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:15:00.000000 tencentcloud-sdk-python-live-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-live-3.0.902/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.903/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.902/README.rst` & `tencentcloud-sdk-python-live-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.903/tencentcloud/live/v20180801/live_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.903/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.903/tencentcloud/live/v20180801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2183,18 +2183,18 @@
 极速高清目标码率=VideoBitrate * (1-AdaptBitratePercent)
 
 取值范围：0.0到0.5
         :type AdaptBitratePercent: float
         :param ShortEdgeAsHeight: 是否以短边作为高度，0：否，1：是。默认0。
         :type ShortEdgeAsHeight: int
         :param DRMType: DRM 加密类型，可选值：fairplay、normalaes、widevine。
-不传递或着为空字符串，清空之前的DRM配置。
+不传递或者为空字符串，清空之前的DRM配置。
         :type DRMType: str
         :param DRMTracks: DRM 加密项，可选值：AUDIO、SD、HD、UHD1、UHD2，后四个为一组，同组中的内容只能选一个。
-不传递或着为空字符串，清空之前的DRM配置。
+不传递或者为空字符串，清空之前的DRM配置。
         :type DRMTracks: str
         """
         self.TemplateName = None
         self.VideoBitrate = None
         self.Acodec = None
         self.AudioBitrate = None
         self.Vcodec = None
@@ -9691,18 +9691,18 @@
 极速高清目标码率=VideoBitrate * (1-AdaptBitratePercent)
 
 取值范围：0.0到0.5
         :type AdaptBitratePercent: float
         :param ShortEdgeAsHeight: 是否以短边作为高度，0：否，1：是。默认0。
         :type ShortEdgeAsHeight: int
         :param DRMType: DRM 加密类型，可选值：fairplay、normalaes、widevine。
-不传递或着为空字符串，清空之前的DRM配置。
+不传递或者为空字符串，清空之前的DRM配置。
         :type DRMType: str
         :param DRMTracks: DRM 加密项，可选值：AUDIO、SD、HD、UHD1、UHD2，后四个为一组，同组中的内容只能选一个。
-不传递或着为空字符串，清空之前的DRM配置。
+不传递或者为空字符串，清空之前的DRM配置。
         :type DRMTracks: str
         """
         self.TemplateId = None
         self.Vcodec = None
         self.Acodec = None
         self.AudioBitrate = None
         self.Description = None
```

### Comparing `tencentcloud-sdk-python-live-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.903/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.902/setup.py` & `tencentcloud-sdk-python-live-3.0.903/setup.py`

 * *Files identical despite different names*

