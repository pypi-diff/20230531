# Comparing `tmp/tencentcloud-sdk-python-tcr-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-tcr-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcr-3.0.902.tar", last modified: Tue May 30 00:33:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcr-3.0.903.tar", last modified: Wed May 31 02:21:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcr-3.0.902.tar` & `tencentcloud-sdk-python-tcr-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/tcr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/tcr/v20190924/
--rw-r--r--   0 root         (0) root         (0)    99022 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/tcr/v20190924/tcr_client.py
--rw-r--r--   0 root         (0) root         (0)     8446 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/tcr/v20190924/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/tcr/v20190924/__init__.py
--rw-r--r--   0 root         (0) root         (0)   259743 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/tcr/v20190924/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/tcr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud_sdk_python_tcr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud_sdk_python_tcr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud_sdk_python_tcr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/tencentcloud_sdk_python_tcr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:33:21.000000 tencentcloud-sdk-python-tcr-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/tcr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/tcr/v20190924/
+-rw-r--r--   0 root         (0) root         (0)    99109 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/tcr/v20190924/tcr_client.py
+-rw-r--r--   0 root         (0) root         (0)     8446 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/tcr/v20190924/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/tcr/v20190924/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   259897 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/tcr/v20190924/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/tcr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud_sdk_python_tcr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud_sdk_python_tcr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud_sdk_python_tcr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/tencentcloud_sdk_python_tcr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:21:44.000000 tencentcloud-sdk-python-tcr-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:21:45.000000 tencentcloud-sdk-python-tcr-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.902/README.rst` & `tencentcloud-sdk-python-tcr-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/tcr/v20190924/tcr_client.py` & `tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/tcr/v20190924/tcr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1018,14 +1018,16 @@
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteSecurityPolicy(self, request):
         """删除实例公网访问白名单策略
 
+        注意：当PolicyIndex和CidrBlock同时存在时，CidrBlock优先级更高
+
         :param request: Request instance for DeleteSecurityPolicy.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteSecurityPolicyRequest`
         :rtype: :class:`tencentcloud.tcr.v20190924.models.DeleteSecurityPolicyResponse`
 
         """
         try:
             params = request._serialize()
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/tcr/v20190924/errorcodes.py` & `tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/tcr/v20190924/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/tcr/v20190924/models.py` & `tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/tcr/v20190924/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2419,24 +2419,28 @@
         r"""
         :param RegistryId: 实例Id
         :type RegistryId: str
         :param PolicyIndex: 白名单Id
         :type PolicyIndex: int
         :param PolicyVersion: 白名单版本
         :type PolicyVersion: str
+        :param CidrBlock: 网段或IP(互斥)
+        :type CidrBlock: str
         """
         self.RegistryId = None
         self.PolicyIndex = None
         self.PolicyVersion = None
+        self.CidrBlock = None
 
 
     def _deserialize(self, params):
         self.RegistryId = params.get("RegistryId")
         self.PolicyIndex = params.get("PolicyIndex")
         self.PolicyVersion = params.get("PolicyVersion")
+        self.CidrBlock = params.get("CidrBlock")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcr-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcr-3.0.902/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcr-3.0.903/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcr
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Tcr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-tcr-3.0.903/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcr
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Tcr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.902/setup.py` & `tencentcloud-sdk-python-tcr-3.0.903/setup.py`

 * *Files identical despite different names*

