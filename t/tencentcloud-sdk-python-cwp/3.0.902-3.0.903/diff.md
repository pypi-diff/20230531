# Comparing `tmp/tencentcloud-sdk-python-cwp-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-cwp-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.902.tar", last modified: Tue May 30 00:20:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.903.tar", last modified: Wed May 31 02:08:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cwp-3.0.902.tar` & `tencentcloud-sdk-python-cwp-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/cwp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/cwp/v20180228/
--rw-r--r--   0 root         (0) root         (0)     3900 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/cwp/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   253271 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/cwp/v20180228/cwp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/cwp/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)   910717 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/cwp/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/cwp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud_sdk_python_cwp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:20:35.000000 tencentcloud-sdk-python-cwp-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/cwp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/cwp/v20180228/
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/cwp/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   253287 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/cwp/v20180228/cwp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/cwp/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   911322 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/cwp/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/cwp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud_sdk_python_cwp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:08:50.000000 tencentcloud-sdk-python-cwp-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.902/README.rst` & `tencentcloud-sdk-python-cwp-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/cwp/v20180228/errorcodes.py` & `tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/cwp/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/cwp/v20180228/cwp_client.py` & `tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/cwp/v20180228/cwp_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3890,15 +3890,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeSaveOrUpdateWarnings(self, request):
-        """更新或者插入用户告警设置(该接口废弃,请调用 ModifyWarningSetting )
+        """下线
+
+        更新或者插入用户告警设置(该接口废弃,请调用 ModifyWarningSetting )
 
         :param request: Request instance for DescribeSaveOrUpdateWarnings.
         :type request: :class:`tencentcloud.cwp.v20180228.models.DescribeSaveOrUpdateWarningsRequest`
         :rtype: :class:`tencentcloud.cwp.v20180228.models.DescribeSaveOrUpdateWarningsResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/cwp/v20180228/models.py` & `tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/cwp/v20180228/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1852,40 +1852,54 @@
         :param UpdateTime: 数据更新时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type UpdateTime: str
         :param FirstTime: 首次采集时间
         :type FirstTime: str
         :param IsNew: 是否新增[0:否|1:是]
         :type IsNew: int
+        :param MachineExtraInfo: 附加信息
+        :type MachineExtraInfo: :class:`tencentcloud.cwp.v20180228.models.MachineExtraInfo`
+        :param Quuid: 主机Id
+        :type Quuid: str
+        :param Uuid: Agent Id
+        :type Uuid: str
         """
         self.Name = None
         self.Desc = None
         self.Version = None
         self.InstallTime = None
         self.Type = None
         self.MachineName = None
         self.MachineIp = None
         self.OsInfo = None
         self.UpdateTime = None
         self.FirstTime = None
         self.IsNew = None
+        self.MachineExtraInfo = None
+        self.Quuid = None
+        self.Uuid = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.Desc = params.get("Desc")
         self.Version = params.get("Version")
         self.InstallTime = params.get("InstallTime")
         self.Type = params.get("Type")
         self.MachineName = params.get("MachineName")
         self.MachineIp = params.get("MachineIp")
         self.OsInfo = params.get("OsInfo")
         self.UpdateTime = params.get("UpdateTime")
         self.FirstTime = params.get("FirstTime")
         self.IsNew = params.get("IsNew")
+        if params.get("MachineExtraInfo") is not None:
+            self.MachineExtraInfo = MachineExtraInfo()
+            self.MachineExtraInfo._deserialize(params.get("MachineExtraInfo"))
+        self.Quuid = params.get("Quuid")
+        self.Uuid = params.get("Uuid")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cwp-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cwp-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.903/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.902/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.903/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.902/setup.py` & `tencentcloud-sdk-python-cwp-3.0.903/setup.py`

 * *Files identical despite different names*

