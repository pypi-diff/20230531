# Comparing `tmp/tencentcloud-sdk-python-wedata-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-wedata-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.902.tar", last modified: Tue May 30 00:37:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.903.tar", last modified: Wed May 31 02:26:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wedata-3.0.902.tar` & `tencentcloud-sdk-python-wedata-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:31.000000 tencentcloud-sdk-python-wedata-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-30 00:37:30.000000 tencentcloud-sdk-python-wedata-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:31.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:31.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/wedata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:37:30.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:31.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/wedata/v20210820/
--rw-r--r--   0 root         (0) root         (0)     3323 2023-05-30 00:37:30.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:37:30.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)   184325 2023-05-30 00:37:30.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 root         (0) root         (0)   699593 2023-05-30 00:37:30.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:37:30.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:31.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud_sdk_python_wedata.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:37:31.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-30 00:37:31.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-30 00:37:31.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:37:31.000000 tencentcloud-sdk-python-wedata-3.0.902/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-30 00:37:31.000000 tencentcloud-sdk-python-wedata-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-05-30 00:37:30.000000 tencentcloud-sdk-python-wedata-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:37:31.000000 tencentcloud-sdk-python-wedata-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/wedata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)     3323 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   184325 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)   703148 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud_sdk_python_wedata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:26:17.000000 tencentcloud-sdk-python-wedata-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.902/README.rst` & `tencentcloud-sdk-python-wedata-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/wedata/v20210820/errorcodes.py` & `tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/wedata/v20210820/wedata_client.py` & `tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/wedata/v20210820/models.py` & `tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/wedata/v20210820/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7219,14 +7219,24 @@
         :type TaskTypeIdList: str
         :param StatusList: 任务状态字符串，多个任务状态之间以英文字符逗号分隔
         :type StatusList: str
         :param TaskCycleUnitList: 任务周期类型字符串，多个任务周期之间以英文字符逗号分隔
         :type TaskCycleUnitList: str
         :param ProductNameList: 任务所属产品类型
         :type ProductNameList: str
+        :param SourceServiceId: 数据源id或（仅针对离线同步任务）来源数据源id
+        :type SourceServiceId: str
+        :param SourceServiceType: 数据源类型或（仅针对离线同步任务）来源数据源类型
+        :type SourceServiceType: str
+        :param TargetServiceId: （仅针对离线同步任务）目标数据源id
+        :type TargetServiceId: str
+        :param TargetServiceType: （仅针对离线同步任务）目标数据源类型
+        :type TargetServiceType: str
+        :param AlarmType: 告警类型，多个类型以逗号分隔
+        :type AlarmType: str
         """
         self.ProjectId = None
         self.FolderIdList = None
         self.WorkFlowIdList = None
         self.WorkFlowNameList = None
         self.TaskNameList = None
         self.TaskIdList = None
@@ -7235,14 +7245,19 @@
         self.SortItem = None
         self.SortType = None
         self.InChargeList = None
         self.TaskTypeIdList = None
         self.StatusList = None
         self.TaskCycleUnitList = None
         self.ProductNameList = None
+        self.SourceServiceId = None
+        self.SourceServiceType = None
+        self.TargetServiceId = None
+        self.TargetServiceType = None
+        self.AlarmType = None
 
 
     def _deserialize(self, params):
         self.ProjectId = params.get("ProjectId")
         self.FolderIdList = params.get("FolderIdList")
         self.WorkFlowIdList = params.get("WorkFlowIdList")
         self.WorkFlowNameList = params.get("WorkFlowNameList")
@@ -7253,14 +7268,19 @@
         self.SortItem = params.get("SortItem")
         self.SortType = params.get("SortType")
         self.InChargeList = params.get("InChargeList")
         self.TaskTypeIdList = params.get("TaskTypeIdList")
         self.StatusList = params.get("StatusList")
         self.TaskCycleUnitList = params.get("TaskCycleUnitList")
         self.ProductNameList = params.get("ProductNameList")
+        self.SourceServiceId = params.get("SourceServiceId")
+        self.SourceServiceType = params.get("SourceServiceType")
+        self.TargetServiceId = params.get("TargetServiceId")
+        self.TargetServiceType = params.get("TargetServiceType")
+        self.AlarmType = params.get("AlarmType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -19116,14 +19136,41 @@
         :type VirtualFlag: bool
         :param TaskAction: 弹性周期配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type TaskAction: str
         :param DelayTime: 延迟时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type DelayTime: int
+        :param ExecutionStartTime: 执行开始时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutionStartTime: str
+        :param ExecutionEndTime: 执行结束时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutionEndTime: str
+        :param Layer: 层级
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Layer: str
+        :param SourceServiceId: 来源数据源ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SourceServiceId: str
+        :param SourceServiceType: 来源数据源类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SourceServiceType: str
+        :param TargetServiceId: 目标数据源ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TargetServiceId: str
+        :param TargetServiceType: 目标数据源类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TargetServiceType: str
+        :param AlarmType: 任务告警类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AlarmType: str
+        :param CreateTime: 任务创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
         """
         self.TaskId = None
         self.TaskName = None
         self.WorkflowId = None
         self.WorkflowName = None
         self.ProjectName = None
         self.ProjectIdent = None
@@ -19139,14 +19186,23 @@
         self.InCharge = None
         self.CycleUnit = None
         self.LeftCoordinate = None
         self.TopCoordinate = None
         self.VirtualFlag = None
         self.TaskAction = None
         self.DelayTime = None
+        self.ExecutionStartTime = None
+        self.ExecutionEndTime = None
+        self.Layer = None
+        self.SourceServiceId = None
+        self.SourceServiceType = None
+        self.TargetServiceId = None
+        self.TargetServiceType = None
+        self.AlarmType = None
+        self.CreateTime = None
 
 
     def _deserialize(self, params):
         self.TaskId = params.get("TaskId")
         self.TaskName = params.get("TaskName")
         self.WorkflowId = params.get("WorkflowId")
         self.WorkflowName = params.get("WorkflowName")
@@ -19164,14 +19220,23 @@
         self.InCharge = params.get("InCharge")
         self.CycleUnit = params.get("CycleUnit")
         self.LeftCoordinate = params.get("LeftCoordinate")
         self.TopCoordinate = params.get("TopCoordinate")
         self.VirtualFlag = params.get("VirtualFlag")
         self.TaskAction = params.get("TaskAction")
         self.DelayTime = params.get("DelayTime")
+        self.ExecutionStartTime = params.get("ExecutionStartTime")
+        self.ExecutionEndTime = params.get("ExecutionEndTime")
+        self.Layer = params.get("Layer")
+        self.SourceServiceId = params.get("SourceServiceId")
+        self.SourceServiceType = params.get("SourceServiceType")
+        self.TargetServiceId = params.get("TargetServiceId")
+        self.TargetServiceType = params.get("TargetServiceType")
+        self.AlarmType = params.get("AlarmType")
+        self.CreateTime = params.get("CreateTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -19572,31 +19637,39 @@
         :type PageNumber: int
         :param PageSize: 页大小
         :type PageSize: int
         :param Items: 工作流列表信息
         :type Items: list of TaskCanvasInfo
         :param TotalPage: 总页数
         :type TotalPage: int
+        :param PageCount: 页数
+        :type PageCount: int
+        :param TotalCount: 总条数
+        :type TotalCount: int
         """
         self.PageNumber = None
         self.PageSize = None
         self.Items = None
         self.TotalPage = None
+        self.PageCount = None
+        self.TotalCount = None
 
 
     def _deserialize(self, params):
         self.PageNumber = params.get("PageNumber")
         self.PageSize = params.get("PageSize")
         if params.get("Items") is not None:
             self.Items = []
             for item in params.get("Items"):
                 obj = TaskCanvasInfo()
                 obj._deserialize(item)
                 self.Items.append(obj)
         self.TotalPage = params.get("TotalPage")
+        self.PageCount = params.get("PageCount")
+        self.TotalCount = params.get("TotalCount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wedata-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wedata-3.0.902/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.903/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.903/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.902/setup.py` & `tencentcloud-sdk-python-wedata-3.0.903/setup.py`

 * *Files identical despite different names*

