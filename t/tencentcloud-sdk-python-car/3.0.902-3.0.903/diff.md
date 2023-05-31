# Comparing `tmp/tencentcloud-sdk-python-car-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-car-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-car-3.0.902.tar", last modified: Tue May 30 00:17:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-car-3.0.903.tar", last modified: Wed May 31 02:05:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-car-3.0.902.tar` & `tencentcloud-sdk-python-car-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud/car/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud/car/v20220110/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud/car/v20220110/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud/car/v20220110/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5256 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud/car/v20220110/car_client.py
--rw-r--r--   0 root         (0) root         (0)     9309 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud/car/v20220110/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud/car/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud_sdk_python_car.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud_sdk_python_car.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud_sdk_python_car.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud_sdk_python_car.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:17:12.000000 tencentcloud-sdk-python-car-3.0.902/tencentcloud_sdk_python_car.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud/car/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud/car/v20220110/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud/car/v20220110/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud/car/v20220110/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud/car/v20220110/car_client.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud/car/v20220110/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud/car/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud_sdk_python_car.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud_sdk_python_car.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud_sdk_python_car.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud_sdk_python_car.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:05:08.000000 tencentcloud-sdk-python-car-3.0.903/tencentcloud_sdk_python_car.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-car-3.0.902/README.rst` & `tencentcloud-sdk-python-car-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.902/tencentcloud/car/v20220110/errorcodes.py` & `tencentcloud-sdk-python-car-3.0.903/tencentcloud/car/v20220110/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.902/tencentcloud/car/v20220110/car_client.py` & `tencentcloud-sdk-python-car-3.0.903/tencentcloud/car/v20220110/car_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.902/tencentcloud/car/v20220110/models.py` & `tencentcloud-sdk-python-car-3.0.903/tencentcloud/car/v20220110/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,36 +88,43 @@
         :type UserIp: str
         :param ClientSession: 客户端session信息，从SDK请求中获得。特殊的，当 RunMode 参数为 RunWithoutClient 时，该字段可以为空
         :type ClientSession: str
         :param RunMode: 云端运行模式。
 RunWithoutClient：允许无客户端连接的情况下仍保持云端 App 运行
 默认值（空）：要求必须有客户端连接才会保持云端 App 运行。
         :type RunMode: str
+        :param ApplicationParameters: 应用启动参数。
+如果请求的是多应用共享项目，此参数生效；
+如果请求的是关闭预启动的单应用独享项目，此参数生效；
+如果请求的是开启预启动的单应用独享项目，此参数失效。
+        :type ApplicationParameters: str
         :param HostUserId: 【多人互动】房主用户ID，在多人互动模式下为必填字段。
 如果该用户是房主，HostUserId需要和UserId保持一致；
 如果该用户非房主，HostUserId需要填写房主的HostUserId。
         :type HostUserId: str
         :param Role: 【多人互动】角色。
 Player：玩家（可通过键鼠等操作应用）
 Viewer：观察者（只能观看，无法操作）
         :type Role: str
         """
         self.UserId = None
         self.UserIp = None
         self.ClientSession = None
         self.RunMode = None
+        self.ApplicationParameters = None
         self.HostUserId = None
         self.Role = None
 
 
     def _deserialize(self, params):
         self.UserId = params.get("UserId")
         self.UserIp = params.get("UserIp")
         self.ClientSession = params.get("ClientSession")
         self.RunMode = params.get("RunMode")
+        self.ApplicationParameters = params.get("ApplicationParameters")
         self.HostUserId = params.get("HostUserId")
         self.Role = params.get("Role")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
```

### Comparing `tencentcloud-sdk-python-car-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-car-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-car-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-car-3.0.903/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-car
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Car SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-car-3.0.902/setup.py` & `tencentcloud-sdk-python-car-3.0.903/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.902/tencentcloud_sdk_python_car.egg-info/PKG-INFO` & `tencentcloud-sdk-python-car-3.0.903/tencentcloud_sdk_python_car.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-car
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Car SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

