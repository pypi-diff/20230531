# Comparing `tmp/tencentcloud-sdk-python-thpc-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-thpc-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.902.tar", last modified: Tue May 30 00:34:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.903.tar", last modified: Wed May 31 02:22:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-thpc-3.0.902.tar` & `tencentcloud-sdk-python-thpc-3.0.903.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20220401/
--rw-r--r--   0 root         (0) root         (0)     4733 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20220401/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20220401/__init__.py
--rw-r--r--   0 root         (0) root         (0)    97393 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20220401/models.py
--rw-r--r--   0 root         (0) root         (0)    16733 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20220401/thpc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20211109/
--rw-r--r--   0 root         (0) root         (0)     2035 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20211109/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20211109/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43727 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20211109/models.py
--rw-r--r--   0 root         (0) root         (0)     4612 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20211109/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20230321/
--rw-r--r--   0 root         (0) root         (0)     4248 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20230321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20230321/__init__.py
--rw-r--r--   0 root         (0) root         (0)   105526 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20230321/models.py
--rw-r--r--   0 root         (0) root         (0)    17699 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20230321/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud_sdk_python_thpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      781 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-30 00:34:15.000000 tencentcloud-sdk-python-thpc-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:34:16.000000 tencentcloud-sdk-python-thpc-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20220401/
+-rw-r--r--   0 root         (0) root         (0)     4733 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20220401/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20220401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    97393 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20220401/models.py
+-rw-r--r--   0 root         (0) root         (0)    16733 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20220401/thpc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20211109/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20211109/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20211109/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43727 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20211109/models.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20211109/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20230321/
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20230321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20230321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   107151 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20230321/models.py
+-rw-r--r--   0 root         (0) root         (0)    17699 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20230321/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud_sdk_python_thpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      781 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-31 02:22:49.000000 tencentcloud-sdk-python-thpc-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:22:50.000000 tencentcloud-sdk-python-thpc-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/README.rst` & `tencentcloud-sdk-python-thpc-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20220401/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20220401/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20220401/models.py` & `tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20220401/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20220401/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20220401/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20211109/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20211109/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20211109/models.py` & `tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20211109/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20211109/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20211109/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20230321/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20230321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20230321/models.py` & `tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20230321/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,16 @@
 true：发送检查请求，不会创建实例。检查项包括是否填写了必需参数，请求格式，业务限制和云服务器库存。
 如果检查不通过，则返回对应错误码；
 如果检查通过，则返回RequestId.
 false（默认）：发送正常请求，通过检查后直接创建实例
         :type DryRun: bool
         :param NodeType: 添加节点类型。默认取值：STATIC。<li>STATIC：静态节点，不会参与弹性伸缩流程。<li>DYNAMIC：弹性节点，会被弹性缩容的节点。管控节点和登录节点不支持此参数。
         :type NodeType: str
+        :param ProjectId: 实例所属项目ID。该参数可以通过调用 [DescribeProject](https://cloud.tencent.com/document/api/651/78725) 的返回值中的 projectId 字段来获取。不填为默认项目。
+        :type ProjectId: int
         """
         self.Placement = None
         self.ClusterId = None
         self.VirtualPrivateCloud = None
         self.Count = None
         self.ImageId = None
         self.InstanceChargeType = None
@@ -133,14 +135,15 @@
         self.LoginSettings = None
         self.SecurityGroupIds = None
         self.ClientToken = None
         self.QueueName = None
         self.NodeRole = None
         self.DryRun = None
         self.NodeType = None
+        self.ProjectId = None
 
 
     def _deserialize(self, params):
         if params.get("Placement") is not None:
             self.Placement = Placement()
             self.Placement._deserialize(params.get("Placement"))
         self.ClusterId = params.get("ClusterId")
@@ -172,14 +175,15 @@
             self.LoginSettings._deserialize(params.get("LoginSettings"))
         self.SecurityGroupIds = params.get("SecurityGroupIds")
         self.ClientToken = params.get("ClientToken")
         self.QueueName = params.get("QueueName")
         self.NodeRole = params.get("NodeRole")
         self.DryRun = params.get("DryRun")
         self.NodeType = params.get("NodeType")
+        self.ProjectId = params.get("ProjectId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -512,22 +516,25 @@
         :type DataDisks: list of DataDisk
         :param InternetAccessible: 公网带宽相关信息设置。若不指定该参数，则默认公网带宽为0Mbps。
         :type InternetAccessible: :class:`tencentcloud.thpc.v20230321.models.InternetAccessible`
         :param InstanceName: 节点显示名称。<br><li>
 不指定节点显示名称则默认显示‘未命名’。
 最多支持60个字符。
         :type InstanceName: str
+        :param ProjectId: 实例所属项目ID。该参数可以通过调用 [DescribeProject](https://cloud.tencent.com/document/api/651/78725) 的返回值中的 projectId 字段来获取。不填为默认项目。
+        :type ProjectId: int
         """
         self.InstanceChargeType = None
         self.InstanceChargePrepaid = None
         self.InstanceType = None
         self.SystemDisk = None
         self.DataDisks = None
         self.InternetAccessible = None
         self.InstanceName = None
+        self.ProjectId = None
 
 
     def _deserialize(self, params):
         self.InstanceChargeType = params.get("InstanceChargeType")
         if params.get("InstanceChargePrepaid") is not None:
             self.InstanceChargePrepaid = InstanceChargePrepaid()
             self.InstanceChargePrepaid._deserialize(params.get("InstanceChargePrepaid"))
@@ -541,14 +548,15 @@
                 obj = DataDisk()
                 obj._deserialize(item)
                 self.DataDisks.append(obj)
         if params.get("InternetAccessible") is not None:
             self.InternetAccessible = InternetAccessible()
             self.InternetAccessible._deserialize(params.get("InternetAccessible"))
         self.InstanceName = params.get("InstanceName")
+        self.ProjectId = params.get("ProjectId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1367,34 +1375,38 @@
         :param InstanceChargePrepaid: 预付费模式，即包年包月相关参数设置。通过该参数可以指定包年包月节点的购买时长、是否设置自动续费等属性。若指定节点的付费模式为预付费则该参数必传。
         :type InstanceChargePrepaid: :class:`tencentcloud.thpc.v20230321.models.InstanceChargePrepaid`
         :param InstanceType: 节点机型。不同实例机型指定了不同的资源规格。
 <br><li>具体取值可通过调用接口[DescribeInstanceTypeConfigs](https://cloud.tencent.com/document/api/213/15749)来获得最新的规格表或参见[实例规格](https://cloud.tencent.com/document/product/213/11518)描述。
         :type InstanceType: str
         :param VirtualPrivateCloud: 私有网络相关信息配置。
         :type VirtualPrivateCloud: :class:`tencentcloud.thpc.v20230321.models.VirtualPrivateCloud`
+        :param ProjectId: 实例所属项目ID。该参数可以通过调用 [DescribeProject](https://cloud.tencent.com/document/api/651/78725) 的返回值中的 projectId 字段来获取。不填为默认项目。
+        :type ProjectId: int
         """
         self.Placement = None
         self.InstanceChargeType = None
         self.InstanceChargePrepaid = None
         self.InstanceType = None
         self.VirtualPrivateCloud = None
+        self.ProjectId = None
 
 
     def _deserialize(self, params):
         if params.get("Placement") is not None:
             self.Placement = Placement()
             self.Placement._deserialize(params.get("Placement"))
         self.InstanceChargeType = params.get("InstanceChargeType")
         if params.get("InstanceChargePrepaid") is not None:
             self.InstanceChargePrepaid = InstanceChargePrepaid()
             self.InstanceChargePrepaid._deserialize(params.get("InstanceChargePrepaid"))
         self.InstanceType = params.get("InstanceType")
         if params.get("VirtualPrivateCloud") is not None:
             self.VirtualPrivateCloud = VirtualPrivateCloud()
             self.VirtualPrivateCloud._deserialize(params.get("VirtualPrivateCloud"))
+        self.ProjectId = params.get("ProjectId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1722,22 +1734,25 @@
         :type DataDisks: list of DataDisk
         :param InternetAccessible: 公网带宽相关信息设置。若不指定该参数，则默认公网带宽为0Mbps。
         :type InternetAccessible: :class:`tencentcloud.thpc.v20230321.models.InternetAccessible`
         :param InstanceName: 节点显示名称。<br><li>
 不指定节点显示名称则默认显示‘未命名’。
 最多支持60个字符。
         :type InstanceName: str
+        :param ProjectId: 实例所属项目ID。该参数可以通过调用 [DescribeProject](https://cloud.tencent.com/document/api/651/78725) 的返回值中的 projectId 字段来获取。不填为默认项目。
+        :type ProjectId: int
         """
         self.InstanceChargeType = None
         self.InstanceChargePrepaid = None
         self.InstanceType = None
         self.SystemDisk = None
         self.DataDisks = None
         self.InternetAccessible = None
         self.InstanceName = None
+        self.ProjectId = None
 
 
     def _deserialize(self, params):
         self.InstanceChargeType = params.get("InstanceChargeType")
         if params.get("InstanceChargePrepaid") is not None:
             self.InstanceChargePrepaid = InstanceChargePrepaid()
             self.InstanceChargePrepaid._deserialize(params.get("InstanceChargePrepaid"))
@@ -1751,14 +1766,15 @@
                 obj = DataDisk()
                 obj._deserialize(item)
                 self.DataDisks.append(obj)
         if params.get("InternetAccessible") is not None:
             self.InternetAccessible = InternetAccessible()
             self.InternetAccessible._deserialize(params.get("InternetAccessible"))
         self.InstanceName = params.get("InstanceName")
+        self.ProjectId = params.get("ProjectId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1834,22 +1850,25 @@
         :type InternetAccessible: :class:`tencentcloud.thpc.v20230321.models.InternetAccessible`
         :param InstanceName: 节点显示名称。<br><li>
 不指定节点显示名称则默认显示‘未命名’。
 </li><li>购买多个节点，如果指定模式串`{R:x}`，表示生成数字[`[x, x+n-1]`，其中`n`表示购买节点的数量，例如`server_{R:3}`，购买1个时，节点显示名称为`server_3`；购买2个时，节点显示名称分别为`server_3`，`server_4`。支持指定多个模式串`{R:x}`。
 购买多个节点，如果不指定模式串，则在节点显示名称添加后缀`1、2...n`，其中`n`表示购买节点的数量，例如`server_`，购买2个时，节点显示名称分别为`server_1`，`server_2`。</li><li>
 最多支持60个字符（包含模式串）。
         :type InstanceName: str
+        :param ProjectId: 实例所属项目ID。该参数可以通过调用 [DescribeProject](https://cloud.tencent.com/document/api/651/78725) 的返回值中的 projectId 字段来获取。不填为默认项目。
+        :type ProjectId: int
         """
         self.InstanceChargeType = None
         self.InstanceChargePrepaid = None
         self.InstanceType = None
         self.SystemDisk = None
         self.DataDisks = None
         self.InternetAccessible = None
         self.InstanceName = None
+        self.ProjectId = None
 
 
     def _deserialize(self, params):
         self.InstanceChargeType = params.get("InstanceChargeType")
         if params.get("InstanceChargePrepaid") is not None:
             self.InstanceChargePrepaid = InstanceChargePrepaid()
             self.InstanceChargePrepaid._deserialize(params.get("InstanceChargePrepaid"))
@@ -1863,14 +1882,15 @@
                 obj = DataDisk()
                 obj._deserialize(item)
                 self.DataDisks.append(obj)
         if params.get("InternetAccessible") is not None:
             self.InternetAccessible = InternetAccessible()
             self.InternetAccessible._deserialize(params.get("InternetAccessible"))
         self.InstanceName = params.get("InstanceName")
+        self.ProjectId = params.get("ProjectId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/thpc/v20230321/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/thpc/v20230321/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-thpc-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-thpc-3.0.903/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.903/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.903/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.902/setup.py` & `tencentcloud-sdk-python-thpc-3.0.903/setup.py`

 * *Files identical despite different names*

