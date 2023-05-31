# Comparing `tmp/tencentcloud-sdk-python-chdfs-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-chdfs-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-chdfs-3.0.902.tar", last modified: Tue May 30 00:18:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-chdfs-3.0.903.tar", last modified: Wed May 31 02:06:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-chdfs-3.0.902.tar` & `tencentcloud-sdk-python-chdfs-3.0.903.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20190718/
--rw-r--r--   0 root         (0) root         (0)     3280 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20190718/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20190718/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51568 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20190718/models.py
--rw-r--r--   0 root         (0) root         (0)    28022 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20190718/chdfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20201112/
--rw-r--r--   0 root         (0) root         (0)     3600 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20201112/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20201112/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60294 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20201112/models.py
--rw-r--r--   0 root         (0) root         (0)    27286 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20201112/chdfs_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud_sdk_python_chdfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud_sdk_python_chdfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud_sdk_python_chdfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:18:30.000000 tencentcloud-sdk-python-chdfs-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20190718/
+-rw-r--r--   0 root         (0) root         (0)     3280 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20190718/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20190718/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51568 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20190718/models.py
+-rw-r--r--   0 root         (0) root         (0)    28022 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20190718/chdfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20201112/
+-rw-r--r--   0 root         (0) root         (0)     3600 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20201112/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20201112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60336 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20201112/models.py
+-rw-r--r--   0 root         (0) root         (0)    27286 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20201112/chdfs_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud_sdk_python_chdfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud_sdk_python_chdfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud_sdk_python_chdfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:06:38.000000 tencentcloud-sdk-python-chdfs-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.902/README.rst` & `tencentcloud-sdk-python-chdfs-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20190718/errorcodes.py` & `tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20190718/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20190718/models.py` & `tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20190718/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20190718/chdfs_client.py` & `tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20190718/chdfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20201112/errorcodes.py` & `tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20201112/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20201112/models.py` & `tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20201112/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1810,30 +1810,30 @@
 class Summary(AbstractModel):
     """生命周期规则当前路径具体存储量信息
 
     """
 
     def __init__(self):
         r"""
-        :param CapacityUsed: 总存储量（单位byte）
+        :param CapacityUsed: 已使用容量（byte）
 注意：此字段可能返回 null，表示取不到有效值。
         :type CapacityUsed: int
-        :param StandardCapacityUsed: 标准存储量（单位byte）
+        :param StandardCapacityUsed: 已使用COS标准存储容量（byte）
 注意：此字段可能返回 null，表示取不到有效值。
         :type StandardCapacityUsed: int
-        :param DegradeCapacityUsed: 低频存储量（单位byte）
+        :param DegradeCapacityUsed: 已使用COS低频存储容量（byte）
 注意：此字段可能返回 null，表示取不到有效值。
         :type DegradeCapacityUsed: int
-        :param ArchiveCapacityUsed: 归档存储量（单位byte）
+        :param ArchiveCapacityUsed: 已使用COS归档存储容量（byte）
 注意：此字段可能返回 null，表示取不到有效值。
         :type ArchiveCapacityUsed: int
-        :param DeepArchiveCapacityUsed: 深度归档存储量（单位byte）
+        :param DeepArchiveCapacityUsed: 已使用COS深度归档存储容量（byte）
 注意：此字段可能返回 null，表示取不到有效值。
         :type DeepArchiveCapacityUsed: int
-        :param IntelligentCapacityUsed: 智能分层存储量（单位byte）
+        :param IntelligentCapacityUsed: 已使用COS智能分层存储容量（byte）
 注意：此字段可能返回 null，表示取不到有效值。
         :type IntelligentCapacityUsed: int
         """
         self.CapacityUsed = None
         self.StandardCapacityUsed = None
         self.DegradeCapacityUsed = None
         self.ArchiveCapacityUsed = None
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/chdfs/v20201112/chdfs_client.py` & `tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/chdfs/v20201112/chdfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.902/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-chdfs-3.0.903/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-chdfs
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Chdfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-chdfs-3.0.903/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-chdfs
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Chdfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.902/setup.py` & `tencentcloud-sdk-python-chdfs-3.0.903/setup.py`

 * *Files identical despite different names*

