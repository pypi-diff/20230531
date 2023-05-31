# Comparing `tmp/tencentcloud-sdk-python-facefusion-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-facefusion-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-facefusion-3.0.902.tar", last modified: Tue May 30 00:23:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-facefusion-3.0.903.tar", last modified: Wed May 31 02:11:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-facefusion-3.0.902.tar` & `tencentcloud-sdk-python-facefusion-3.0.903.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      758 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20181201/
--rw-r--r--   0 root         (0) root         (0)     5769 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20181201/facefusion_client.py
--rw-r--r--   0 root         (0) root         (0)     6738 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20181201/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20181201/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22519 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20181201/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20220927/
--rw-r--r--   0 root         (0) root         (0)     3386 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20220927/facefusion_client.py
--rw-r--r--   0 root         (0) root         (0)     5459 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20220927/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20220927/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13479 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20220927/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud_sdk_python_facefusion.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud_sdk_python_facefusion.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      708 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud_sdk_python_facefusion.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:23:27.000000 tencentcloud-sdk-python-facefusion-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20181201/
+-rw-r--r--   0 root         (0) root         (0)     5769 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20181201/facefusion_client.py
+-rw-r--r--   0 root         (0) root         (0)     6738 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20181201/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20181201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22519 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20181201/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20220927/
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20220927/facefusion_client.py
+-rw-r--r--   0 root         (0) root         (0)     5459 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20220927/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20220927/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13702 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20220927/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud_sdk_python_facefusion.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud_sdk_python_facefusion.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      708 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud_sdk_python_facefusion.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:11:42.000000 tencentcloud-sdk-python-facefusion-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.902/README.rst` & `tencentcloud-sdk-python-facefusion-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20181201/facefusion_client.py` & `tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20181201/facefusion_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20181201/errorcodes.py` & `tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20181201/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20181201/models.py` & `tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20181201/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20220927/facefusion_client.py` & `tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20220927/facefusion_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20220927/errorcodes.py` & `tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20220927/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud/facefusion/v20220927/models.py` & `tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud/facefusion/v20220927/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,35 +360,40 @@
         :type CreateTime: str
         :param UpdateTime: 修改时间
         :type UpdateTime: str
         :param MaterialFaceList: 人脸信息
         :type MaterialFaceList: list of MaterialFaces
         :param MaterialName: 素材名
         :type MaterialName: str
+        :param AuditResult: 审核原因
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AuditResult: str
         """
         self.MaterialId = None
         self.MaterialStatus = None
         self.CreateTime = None
         self.UpdateTime = None
         self.MaterialFaceList = None
         self.MaterialName = None
+        self.AuditResult = None
 
 
     def _deserialize(self, params):
         self.MaterialId = params.get("MaterialId")
         self.MaterialStatus = params.get("MaterialStatus")
         self.CreateTime = params.get("CreateTime")
         self.UpdateTime = params.get("UpdateTime")
         if params.get("MaterialFaceList") is not None:
             self.MaterialFaceList = []
             for item in params.get("MaterialFaceList"):
                 obj = MaterialFaces()
                 obj._deserialize(item)
                 self.MaterialFaceList.append(obj)
         self.MaterialName = params.get("MaterialName")
+        self.AuditResult = params.get("AuditResult")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.902/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO` & `tencentcloud-sdk-python-facefusion-3.0.903/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-facefusion
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Facefusion SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-facefusion-3.0.903/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-facefusion
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Facefusion SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.902/setup.py` & `tencentcloud-sdk-python-facefusion-3.0.903/setup.py`

 * *Files identical despite different names*

