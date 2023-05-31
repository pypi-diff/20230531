# Comparing `tmp/tencentcloud-sdk-python-ccc-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-ccc-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.902.tar", last modified: Tue May 30 00:17:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.903.tar", last modified: Wed May 31 02:05:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ccc-3.0.902.tar` & `tencentcloud-sdk-python-ccc-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/ccc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/ccc/v20200210/
--rw-r--r--   0 root         (0) root         (0)    36406 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/ccc/v20200210/ccc_client.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/ccc/v20200210/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/ccc/v20200210/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142135 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/ccc/v20200210/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud_sdk_python_ccc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:17:33.000000 tencentcloud-sdk-python-ccc-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:34.000000 tencentcloud-sdk-python-ccc-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:05:33.000000 tencentcloud-sdk-python-ccc-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:34.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:34.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/ccc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:34.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/ccc/v20200210/
+-rw-r--r--   0 root         (0) root         (0)    36406 2023-05-31 02:05:33.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/ccc/v20200210/ccc_client.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-05-31 02:05:33.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/ccc/v20200210/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:05:33.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/ccc/v20200210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142129 2023-05-31 02:05:33.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/ccc/v20200210/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:05:33.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:05:33.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:05:34.000000 tencentcloud-sdk-python-ccc-3.0.903/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:34.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud_sdk_python_ccc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:05:34.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-31 02:05:34.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:05:34.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:05:34.000000 tencentcloud-sdk-python-ccc-3.0.903/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:05:33.000000 tencentcloud-sdk-python-ccc-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:05:34.000000 tencentcloud-sdk-python-ccc-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.902/README.rst` & `tencentcloud-sdk-python-ccc-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/ccc/v20200210/ccc_client.py` & `tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/ccc/v20200210/ccc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/ccc/v20200210/errorcodes.py` & `tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/ccc/v20200210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/ccc/v20200210/models.py` & `tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/ccc/v20200210/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,15 +797,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param SdkAppId: 应用 ID（必填），可以查看 https://console.cloud.tencent.com/ccc
         :type SdkAppId: int
-        :param SeatUserId: 坐席账号。
+        :param SeatUserId: 座席账号。
         :type SeatUserId: str
         """
         self.SdkAppId = None
         self.SeatUserId = None
 
 
     def _deserialize(self, params):
@@ -2462,15 +2462,15 @@
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
 class ErrStaffItem(AbstractModel):
-    """批量添加客服时，返回出错客服的像个信息
+    """批量添加客服时，返回出错客服的信息
 
     """
 
     def __init__(self):
         r"""
         :param StaffEmail: 坐席邮箱地址
         :type StaffEmail: str
@@ -2899,21 +2899,21 @@
 
     """
 
     def __init__(self):
         r"""
         :param SdkAppId: 应用ID
         :type SdkAppId: int
-        :param Email: 坐席账户
+        :param Email: 座席账户
         :type Email: str
-        :param Name: 坐席名称
+        :param Name: 座席名称
         :type Name: str
-        :param Phone: 坐席手机号（带0086前缀,示例：008618011111111）
+        :param Phone: 座席手机号（带0086前缀,示例：008618011111111）
         :type Phone: str
-        :param Nick: 坐席昵称
+        :param Nick: 座席昵称
         :type Nick: str
         :param SkillGroupIds: 绑定技能组ID列表
         :type SkillGroupIds: list of int
         :param UseMobileCallOut: 是否开启手机外呼开关
         :type UseMobileCallOut: bool
         :param UseMobileAccept: 手机接听模式 0 - 关闭 | 1 - 仅离线 | 2 - 始终
         :type UseMobileAccept: int
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ccc-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ccc-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.903/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.902/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.903/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.902/setup.py` & `tencentcloud-sdk-python-ccc-3.0.903/setup.py`

 * *Files identical despite different names*

