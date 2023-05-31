# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.902.tar", last modified: Tue May 30 00:20:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.903.tar", last modified: Wed May 31 02:09:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.902.tar` & `tencentcloud-sdk-python-cynosdb-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)    99466 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)    10242 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)   341152 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:20:49.000000 tencentcloud-sdk-python-cynosdb-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)   107865 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    11040 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   370619 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:09:03.000000 tencentcloud-sdk-python-cynosdb-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.902/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def BindClusterResourcePackages(self, request):
+        """为集群绑定资源包
+
+        :param request: Request instance for BindClusterResourcePackages.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.BindClusterResourcePackagesRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.BindClusterResourcePackagesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("BindClusterResourcePackages", params, headers=headers)
+            response = json.loads(body)
+            model = models.BindClusterResourcePackagesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CloseAuditService(self, request):
         """TDSQL-C for MySQL实例关闭审计服务
 
         :param request: Request instance for CloseAuditService.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CloseAuditServiceRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.CloseAuditServiceResponse`
 
@@ -367,14 +390,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateResourcePackage(self, request):
+        """新购资源包
+
+        :param request: Request instance for CreateResourcePackage.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateResourcePackageRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.CreateResourcePackageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateResourcePackage", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateResourcePackageResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteAccounts(self, request):
         """删除账号
 
         :param request: Request instance for DeleteAccounts.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DeleteAccountsRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DeleteAccountsResponse`
 
@@ -1241,14 +1287,83 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeResourcePackageDetail(self, request):
+        """查询资源包使用详情
+
+        :param request: Request instance for DescribeResourcePackageDetail.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcePackageDetailRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcePackageDetailResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeResourcePackageDetail", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeResourcePackageDetailResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeResourcePackageList(self, request):
+        """查询资源包列表
+
+        :param request: Request instance for DescribeResourcePackageList.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcePackageListRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcePackageListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeResourcePackageList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeResourcePackageListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeResourcePackageSaleSpec(self, request):
+        """查询资源包规格
+
+        :param request: Request instance for DescribeResourcePackageSaleSpec.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcePackageSaleSpecRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcePackageSaleSpecResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeResourcePackageSaleSpec", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeResourcePackageSaleSpecResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeResourcesByDealName(self, request):
         """根据计费订单id查询资源列表
 
         :param request: Request instance for DescribeResourcesByDealName.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcesByDealNameRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcesByDealNameResponse`
 
@@ -1977,14 +2092,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyResourcePackageClusters(self, request):
+        """给资源包绑定集群
+
+        :param request: Request instance for ModifyResourcePackageClusters.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyResourcePackageClustersRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.ModifyResourcePackageClustersResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyResourcePackageClusters", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyResourcePackageClustersResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyResourcePackageName(self, request):
+        """修改资源包名称
+
+        :param request: Request instance for ModifyResourcePackageName.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyResourcePackageNameRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.ModifyResourcePackageNameResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyResourcePackageName", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyResourcePackageNameResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyVipVport(self, request):
         """修改实例组ip，端口
 
         :param request: Request instance for ModifyVipVport.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyVipVportRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.ModifyVipVportResponse`
 
@@ -2161,14 +2322,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def RefundResourcePackage(self, request):
+        """退款资源包
+
+        :param request: Request instance for RefundResourcePackage.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.RefundResourcePackageRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.RefundResourcePackageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RefundResourcePackage", params, headers=headers)
+            response = json.loads(body)
+            model = models.RefundResourcePackageResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def RemoveClusterSlaveZone(self, request):
         """删除从可用区
 
         :param request: Request instance for RemoveClusterSlaveZone.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.RemoveClusterSlaveZoneRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.RemoveClusterSlaveZoneResponse`
 
@@ -2435,14 +2619,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UnbindClusterResourcePackages(self, request):
+        """cynos解绑资源包
+
+        :param request: Request instance for UnbindClusterResourcePackages.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.UnbindClusterResourcePackagesRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.UnbindClusterResourcePackagesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UnbindClusterResourcePackages", params, headers=headers)
+            response = json.loads(body)
+            model = models.UnbindClusterResourcePackagesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpgradeClusterVersion(self, request):
         """更新集群Cynos内核版本
 
         :param request: Request instance for UpgradeClusterVersion.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.UpgradeClusterVersionRequest`
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,29 @@
 
 # CAM签名/鉴权错误。
 AUTHFAILURE = 'AuthFailure'
 
 # 批量查询失败。
 FAILEDOPERATION_BATCHGETINSTANCEERROR = 'FailedOperation.BatchGetInstanceError'
 
+# 绑定资源包失败
+FAILEDOPERATION_BINDSOURCEPACKAGEERROR = 'FailedOperation.BindSourcePackageError'
+
 # 获取权限失败，请稍后重试。如果持续不成功，请联系客服进行处理。
 FAILEDOPERATION_CAMCHECKRESOURCEERROR = 'FailedOperation.CamCheckResourceError'
 
 # 鉴权失败，请稍后重试。如果持续不成功，请联系客服进行处理。
 FAILEDOPERATION_CAMSIGANDAUTHERROR = 'FailedOperation.CamSigAndAuthError'
 
 # 创建并支付订单失败。
 FAILEDOPERATION_CREATEORDER = 'FailedOperation.CreateOrder'
 
+# 创建资源包失败
+FAILEDOPERATION_CREATESOURCEPACKAGEERROR = 'FailedOperation.CreateSourcePackageError'
+
 # 数据库访问失败，请稍后重试。如果持续不成功，请联系客服进行处理。
 FAILEDOPERATION_DATABASEACCESSERROR = 'FailedOperation.DatabaseAccessError'
 
 # 创建流程失败，请稍后重试。如果持续不成功，请联系客服进行处理。
 FAILEDOPERATION_FLOWCREATEERROR = 'FailedOperation.FlowCreateError'
 
 # Flow不存在。
@@ -49,20 +55,32 @@
 
 # 账号余额不足。
 FAILEDOPERATION_INSUFFICIENTBALANCE = 'FailedOperation.InsufficientBalance'
 
 # 操作失败，请稍后重试。如果持续不成功，请联系客服进行处理。
 FAILEDOPERATION_OPERATIONFAILEDERROR = 'FailedOperation.OperationFailedError'
 
+# 查询资源包消耗明细失败
+FAILEDOPERATION_QUERYSOURCEPACKAGEDETAILERROR = 'FailedOperation.QuerySourcePackageDetailError'
+
+# 查询资源包失败
+FAILEDOPERATION_QUERYSOURCEPACKAGEERROR = 'FailedOperation.QuerySourcePackageError'
+
 # 规格信息查询失败。
 FAILEDOPERATION_QUERYSPECBYSPECCODEERROR = 'FailedOperation.QuerySpecBySpecCodeError'
 
+# 资源包退款失败
+FAILEDOPERATION_REFUNDSOURCEPACKAGEERROR = 'FailedOperation.RefundSourcePackageError'
+
 # 创建并支付订单失败，请稍后重试。如果持续不成功，请联系客服进行处理。
 FAILEDOPERATION_TRADECREATEORDERERROR = 'FailedOperation.TradeCreateOrderError'
 
+# 解绑资源包失败
+FAILEDOPERATION_UNBINDSOURCEPACKAGEERROR = 'FailedOperation.UnBindSourcePackageError'
+
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 查询数据库失败。
 INTERNALERROR_DBOPERATIONFAILED = 'InternalError.DbOperationFailed'
 
 # 获取安全组信息失败。
@@ -238,14 +256,17 @@
 
 # serverless实例当前状态不允许该操作。
 OPERATIONDENIED_SERVERLESSINSTANCESTATUSDENIED = 'OperationDenied.ServerlessInstanceStatusDenied'
 
 # 任务冲突检查不通过。
 OPERATIONDENIED_TASKCONFLICTERROR = 'OperationDenied.TaskConflictError'
 
+# 不支持该类型规格售卖
+OPERATIONDENIED_UNSUPPORTSALESPECERROR = 'OperationDenied.UnSupportSaleSpecError'
+
 # 用户未进行实名认证，请先进行实名认证才可购买。
 OPERATIONDENIED_USERNOTAUTHENTICATEDERROR = 'OperationDenied.UserNotAuthenticatedError'
 
 # Serverless不支持该版本。
 OPERATIONDENIED_VERSIONNOTSUPPORTERROR = 'OperationDenied.VersionNotSupportError'
 
 # 集群不存在。
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/cynosdb/v20190107/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -802,14 +802,94 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class BindClusterResourcePackagesRequest(AbstractModel):
+    """BindClusterResourcePackages请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PackageIds: 资源包唯一ID
+        :type PackageIds: list of str
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        """
+        self.PackageIds = None
+        self.ClusterId = None
+
+
+    def _deserialize(self, params):
+        self.PackageIds = params.get("PackageIds")
+        self.ClusterId = params.get("ClusterId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class BindClusterResourcePackagesResponse(AbstractModel):
+    """BindClusterResourcePackages返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class BindInstanceInfo(AbstractModel):
+    """资源包绑定的实例信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 绑定的实例ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceId: str
+        :param InstanceRegion: 绑定的实例所在的地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceRegion: str
+        :param InstanceType: 绑定的实例类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceType: str
+        """
+        self.InstanceId = None
+        self.InstanceRegion = None
+        self.InstanceType = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.InstanceRegion = params.get("InstanceRegion")
+        self.InstanceType = params.get("InstanceType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class BinlogItem(AbstractModel):
     """Binlog描述
 
     """
 
     def __init__(self):
         r"""
@@ -1773,14 +1853,95 @@
 
 
     def _deserialize(self, params):
         self.TemplateId = params.get("TemplateId")
         self.RequestId = params.get("RequestId")
 
 
+class CreateResourcePackageRequest(AbstractModel):
+    """CreateResourcePackage请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceType: 实例类型
+        :type InstanceType: str
+        :param PackageRegion: 资源包使用地域
+china-中国内地通用，overseas-港澳台及海外通用
+        :type PackageRegion: str
+        :param PackageType: 资源包类型
+
+资源包类型：CCU-计算资源包，DISK-存储资源包
+        :type PackageType: str
+        :param PackageVersion: 资源包版本
+base-基础版本，common-通用版本，enterprise-企业版本
+        :type PackageVersion: str
+        :param PackageSpec: 资源包大小，计算资源单位：万个；存储资源：GB
+        :type PackageSpec: float
+        :param ExpireDay: 资源包有效期，单位:天
+        :type ExpireDay: int
+        :param PackageCount: 购买资源包个数
+        :type PackageCount: int
+        :param PackageName: 资源包名称
+        :type PackageName: str
+        """
+        self.InstanceType = None
+        self.PackageRegion = None
+        self.PackageType = None
+        self.PackageVersion = None
+        self.PackageSpec = None
+        self.ExpireDay = None
+        self.PackageCount = None
+        self.PackageName = None
+
+
+    def _deserialize(self, params):
+        self.InstanceType = params.get("InstanceType")
+        self.PackageRegion = params.get("PackageRegion")
+        self.PackageType = params.get("PackageType")
+        self.PackageVersion = params.get("PackageVersion")
+        self.PackageSpec = params.get("PackageSpec")
+        self.ExpireDay = params.get("ExpireDay")
+        self.PackageCount = params.get("PackageCount")
+        self.PackageName = params.get("PackageName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateResourcePackageResponse(AbstractModel):
+    """CreateResourcePackage返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BigDealIds: 付费总订单号
+        :type BigDealIds: list of str
+        :param DealNames: 每个物品对应一个dealName，业务需要根据dealName保证发货接口幂等
+        :type DealNames: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.BigDealIds = None
+        self.DealNames = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.BigDealIds = params.get("BigDealIds")
+        self.DealNames = params.get("DealNames")
+        self.RequestId = params.get("RequestId")
+
+
 class CynosdbCluster(AbstractModel):
     """集群信息
 
     """
 
     def __init__(self):
         r"""
@@ -1909,14 +2070,17 @@
         :type IsFreeze: str
         :param OrderSource: 订单来源
 注意：此字段可能返回 null，表示取不到有效值。
         :type OrderSource: str
         :param Ability: 能力
 注意：此字段可能返回 null，表示取不到有效值。
         :type Ability: :class:`tencentcloud.cynosdb.v20190107.models.Ability`
+        :param ResourcePackages: 实例绑定资源包信息（此处只返回存储资源包，即packageType=DISK）	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourcePackages: list of ResourcePackage
         """
         self.Status = None
         self.UpdateTime = None
         self.Zone = None
         self.ClusterName = None
         self.Region = None
         self.DbVersion = None
@@ -1952,14 +2116,15 @@
         self.MasterZone = None
         self.HasSlaveZone = None
         self.SlaveZones = None
         self.BusinessType = None
         self.IsFreeze = None
         self.OrderSource = None
         self.Ability = None
+        self.ResourcePackages = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.UpdateTime = params.get("UpdateTime")
         self.Zone = params.get("Zone")
         self.ClusterName = params.get("ClusterName")
@@ -2014,14 +2179,20 @@
         self.SlaveZones = params.get("SlaveZones")
         self.BusinessType = params.get("BusinessType")
         self.IsFreeze = params.get("IsFreeze")
         self.OrderSource = params.get("OrderSource")
         if params.get("Ability") is not None:
             self.Ability = Ability()
             self.Ability._deserialize(params.get("Ability"))
+        if params.get("ResourcePackages") is not None:
+            self.ResourcePackages = []
+            for item in params.get("ResourcePackages"):
+                obj = ResourcePackage()
+                obj._deserialize(item)
+                self.ResourcePackages.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2036,69 +2207,29 @@
         r"""
         :param ClusterId: 集群ID
         :type ClusterId: str
         :param ClusterName: 集群名称
         :type ClusterName: str
         :param Region: 地域
         :type Region: str
+        :param Zone: 可用区
+        :type Zone: str
+        :param PhysicalZone: 物理可用区
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PhysicalZone: str
         :param Status: 状态
         :type Status: str
         :param StatusDesc: 状态描述
         :type StatusDesc: str
-        :param VpcName: VPC名称
-        :type VpcName: str
-        :param VpcId: vpc唯一id
-        :type VpcId: str
-        :param SubnetName: 子网名称
-        :type SubnetName: str
-        :param SubnetId: 子网ID
-        :type SubnetId: str
-        :param Charset: 字符集
-        :type Charset: str
-        :param CreateTime: 创建时间
-        :type CreateTime: str
-        :param DbType: 数据库类型
-        :type DbType: str
-        :param DbVersion: 数据库版本
-        :type DbVersion: str
-        :param UsedStorage: 使用容量
-        :type UsedStorage: int
-        :param RoAddr: 读写分离Vport
-        :type RoAddr: list of Addr
-        :param InstanceSet: 实例信息
-        :type InstanceSet: list of ClusterInstanceDetail
-        :param PayMode: 付费模式
-        :type PayMode: int
-        :param PeriodEndTime: 到期时间
-        :type PeriodEndTime: str
-        :param Vip: vip地址
-        :type Vip: str
-        :param Vport: vport端口
-        :type Vport: int
-        :param ProjectID: 项目id
-        :type ProjectID: int
-        :param Zone: 可用区
-        :type Zone: str
-        :param ResourceTags: 实例绑定的tag数组信息
-        :type ResourceTags: list of Tag
         :param ServerlessStatus: 当Db类型为SERVERLESS时，serverless集群状态，可选值:
 resume
 resuming
 pause
 pausing
         :type ServerlessStatus: str
-        :param LogBin: binlog开关，可选值：ON, OFF
-注意：此字段可能返回 null，表示取不到有效值。
-        :type LogBin: str
-        :param PitrType: pitr类型，可选值：normal, redo_pitr
-注意：此字段可能返回 null，表示取不到有效值。
-        :type PitrType: str
-        :param PhysicalZone: 物理可用区
-注意：此字段可能返回 null，表示取不到有效值。
-        :type PhysicalZone: str
         :param StorageId: 存储Id
 注意：此字段可能返回 null，表示取不到有效值。
         :type StorageId: str
         :param Storage: 存储大小，单位为G
 注意：此字段可能返回 null，表示取不到有效值。
         :type Storage: int
         :param MaxStorageSize: 最大存储规格，单位为G
@@ -2106,20 +2237,44 @@
         :type MaxStorageSize: int
         :param MinStorageSize: 最小存储规格，单位为G
 注意：此字段可能返回 null，表示取不到有效值。
         :type MinStorageSize: int
         :param StoragePayMode: 存储付费类型，1为包年包月，0为按量计费
 注意：此字段可能返回 null，表示取不到有效值。
         :type StoragePayMode: int
+        :param VpcName: VPC名称
+        :type VpcName: str
+        :param VpcId: vpc唯一id
+        :type VpcId: str
+        :param SubnetName: 子网名称
+        :type SubnetName: str
+        :param SubnetId: 子网ID
+        :type SubnetId: str
+        :param Charset: 字符集
+        :type Charset: str
+        :param CreateTime: 创建时间
+        :type CreateTime: str
+        :param DbType: 数据库类型
+        :type DbType: str
         :param DbMode: 数据库类型，normal，serverless
 注意：此字段可能返回 null，表示取不到有效值。
         :type DbMode: str
+        :param DbVersion: 数据库版本
+        :type DbVersion: str
         :param StorageLimit: 存储空间上限
 注意：此字段可能返回 null，表示取不到有效值。
         :type StorageLimit: int
+        :param UsedStorage: 使用容量
+        :type UsedStorage: int
+        :param Vip: vip地址
+        :type Vip: str
+        :param Vport: vport端口
+        :type Vport: int
+        :param RoAddr: 读写分离Vport
+        :type RoAddr: list of Addr
         :param Ability: 集群支持的功能
 注意：此字段可能返回 null，表示取不到有效值。
         :type Ability: :class:`tencentcloud.cynosdb.v20190107.models.Ability`
         :param CynosVersion: cynos版本
 注意：此字段可能返回 null，表示取不到有效值。
         :type CynosVersion: str
         :param BusinessType: 商业类型
@@ -2136,125 +2291,128 @@
         :type Tasks: list of ObjectTask
         :param MasterZone: 主可用区
 注意：此字段可能返回 null，表示取不到有效值。
         :type MasterZone: str
         :param SlaveZones: 从可用区列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type SlaveZones: list of str
+        :param InstanceSet: 实例信息
+        :type InstanceSet: list of ClusterInstanceDetail
+        :param PayMode: 付费模式
+        :type PayMode: int
+        :param PeriodEndTime: 到期时间
+        :type PeriodEndTime: str
+        :param ProjectID: 项目id
+        :type ProjectID: int
+        :param ResourceTags: 实例绑定的tag数组信息
+        :type ResourceTags: list of Tag
         :param ProxyStatus: Proxy状态
 注意：此字段可能返回 null，表示取不到有效值。
         :type ProxyStatus: str
+        :param LogBin: binlog开关，可选值：ON, OFF
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogBin: str
         :param IsSkipTrade: 是否跳过交易
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsSkipTrade: str
+        :param PitrType: pitr类型，可选值：normal, redo_pitr
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PitrType: str
         :param IsOpenPasswordComplexity: 是否打开密码复杂度
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsOpenPasswordComplexity: str
         :param NetworkStatus: 网络类型
 注意：此字段可能返回 null，表示取不到有效值。
         :type NetworkStatus: str
+        :param ResourcePackages: 集群绑定的资源包信息	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourcePackages: list of ResourcePackage
         """
         self.ClusterId = None
         self.ClusterName = None
         self.Region = None
+        self.Zone = None
+        self.PhysicalZone = None
         self.Status = None
         self.StatusDesc = None
+        self.ServerlessStatus = None
+        self.StorageId = None
+        self.Storage = None
+        self.MaxStorageSize = None
+        self.MinStorageSize = None
+        self.StoragePayMode = None
         self.VpcName = None
         self.VpcId = None
         self.SubnetName = None
         self.SubnetId = None
         self.Charset = None
         self.CreateTime = None
         self.DbType = None
+        self.DbMode = None
         self.DbVersion = None
+        self.StorageLimit = None
         self.UsedStorage = None
-        self.RoAddr = None
-        self.InstanceSet = None
-        self.PayMode = None
-        self.PeriodEndTime = None
         self.Vip = None
         self.Vport = None
-        self.ProjectID = None
-        self.Zone = None
-        self.ResourceTags = None
-        self.ServerlessStatus = None
-        self.LogBin = None
-        self.PitrType = None
-        self.PhysicalZone = None
-        self.StorageId = None
-        self.Storage = None
-        self.MaxStorageSize = None
-        self.MinStorageSize = None
-        self.StoragePayMode = None
-        self.DbMode = None
-        self.StorageLimit = None
+        self.RoAddr = None
         self.Ability = None
         self.CynosVersion = None
         self.BusinessType = None
         self.HasSlaveZone = None
         self.IsFreeze = None
         self.Tasks = None
         self.MasterZone = None
         self.SlaveZones = None
+        self.InstanceSet = None
+        self.PayMode = None
+        self.PeriodEndTime = None
+        self.ProjectID = None
+        self.ResourceTags = None
         self.ProxyStatus = None
+        self.LogBin = None
         self.IsSkipTrade = None
+        self.PitrType = None
         self.IsOpenPasswordComplexity = None
         self.NetworkStatus = None
+        self.ResourcePackages = None
 
 
     def _deserialize(self, params):
         self.ClusterId = params.get("ClusterId")
         self.ClusterName = params.get("ClusterName")
         self.Region = params.get("Region")
+        self.Zone = params.get("Zone")
+        self.PhysicalZone = params.get("PhysicalZone")
         self.Status = params.get("Status")
         self.StatusDesc = params.get("StatusDesc")
+        self.ServerlessStatus = params.get("ServerlessStatus")
+        self.StorageId = params.get("StorageId")
+        self.Storage = params.get("Storage")
+        self.MaxStorageSize = params.get("MaxStorageSize")
+        self.MinStorageSize = params.get("MinStorageSize")
+        self.StoragePayMode = params.get("StoragePayMode")
         self.VpcName = params.get("VpcName")
         self.VpcId = params.get("VpcId")
         self.SubnetName = params.get("SubnetName")
         self.SubnetId = params.get("SubnetId")
         self.Charset = params.get("Charset")
         self.CreateTime = params.get("CreateTime")
         self.DbType = params.get("DbType")
+        self.DbMode = params.get("DbMode")
         self.DbVersion = params.get("DbVersion")
+        self.StorageLimit = params.get("StorageLimit")
         self.UsedStorage = params.get("UsedStorage")
+        self.Vip = params.get("Vip")
+        self.Vport = params.get("Vport")
         if params.get("RoAddr") is not None:
             self.RoAddr = []
             for item in params.get("RoAddr"):
                 obj = Addr()
                 obj._deserialize(item)
                 self.RoAddr.append(obj)
-        if params.get("InstanceSet") is not None:
-            self.InstanceSet = []
-            for item in params.get("InstanceSet"):
-                obj = ClusterInstanceDetail()
-                obj._deserialize(item)
-                self.InstanceSet.append(obj)
-        self.PayMode = params.get("PayMode")
-        self.PeriodEndTime = params.get("PeriodEndTime")
-        self.Vip = params.get("Vip")
-        self.Vport = params.get("Vport")
-        self.ProjectID = params.get("ProjectID")
-        self.Zone = params.get("Zone")
-        if params.get("ResourceTags") is not None:
-            self.ResourceTags = []
-            for item in params.get("ResourceTags"):
-                obj = Tag()
-                obj._deserialize(item)
-                self.ResourceTags.append(obj)
-        self.ServerlessStatus = params.get("ServerlessStatus")
-        self.LogBin = params.get("LogBin")
-        self.PitrType = params.get("PitrType")
-        self.PhysicalZone = params.get("PhysicalZone")
-        self.StorageId = params.get("StorageId")
-        self.Storage = params.get("Storage")
-        self.MaxStorageSize = params.get("MaxStorageSize")
-        self.MinStorageSize = params.get("MinStorageSize")
-        self.StoragePayMode = params.get("StoragePayMode")
-        self.DbMode = params.get("DbMode")
-        self.StorageLimit = params.get("StorageLimit")
         if params.get("Ability") is not None:
             self.Ability = Ability()
             self.Ability._deserialize(params.get("Ability"))
         self.CynosVersion = params.get("CynosVersion")
         self.BusinessType = params.get("BusinessType")
         self.HasSlaveZone = params.get("HasSlaveZone")
         self.IsFreeze = params.get("IsFreeze")
@@ -2262,18 +2420,41 @@
             self.Tasks = []
             for item in params.get("Tasks"):
                 obj = ObjectTask()
                 obj._deserialize(item)
                 self.Tasks.append(obj)
         self.MasterZone = params.get("MasterZone")
         self.SlaveZones = params.get("SlaveZones")
+        if params.get("InstanceSet") is not None:
+            self.InstanceSet = []
+            for item in params.get("InstanceSet"):
+                obj = ClusterInstanceDetail()
+                obj._deserialize(item)
+                self.InstanceSet.append(obj)
+        self.PayMode = params.get("PayMode")
+        self.PeriodEndTime = params.get("PeriodEndTime")
+        self.ProjectID = params.get("ProjectID")
+        if params.get("ResourceTags") is not None:
+            self.ResourceTags = []
+            for item in params.get("ResourceTags"):
+                obj = Tag()
+                obj._deserialize(item)
+                self.ResourceTags.append(obj)
         self.ProxyStatus = params.get("ProxyStatus")
+        self.LogBin = params.get("LogBin")
         self.IsSkipTrade = params.get("IsSkipTrade")
+        self.PitrType = params.get("PitrType")
         self.IsOpenPasswordComplexity = params.get("IsOpenPasswordComplexity")
         self.NetworkStatus = params.get("NetworkStatus")
+        if params.get("ResourcePackages") is not None:
+            self.ResourcePackages = []
+            for item in params.get("ResourcePackages"):
+                obj = ResourcePackage()
+                obj._deserialize(item)
+                self.ResourcePackages.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2339,14 +2520,16 @@
         :type Region: str
         :param Zone: 可用区
         :type Zone: str
         :param Status: 实例状态
         :type Status: str
         :param StatusDesc: 实例状态中文描述
         :type StatusDesc: str
+        :param DbMode: 实例形态，是否为serverless实例
+        :type DbMode: str
         :param DbType: 数据库类型
         :type DbType: str
         :param DbVersion: 数据库版本
         :type DbVersion: str
         :param Cpu: Cpu，单位：核
         :type Cpu: int
         :param Memory: 内存，单位：GB
@@ -2427,26 +2610,30 @@
         :type MasterZone: str
         :param SlaveZones: 备可用区
 注意：此字段可能返回 null，表示取不到有效值。
         :type SlaveZones: list of str
         :param InstanceNetInfo: 实例网络信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceNetInfo: list of InstanceNetInfo
+        :param ResourcePackages: 实例绑定资源包信息（此处只返回计算资源包，即packageType=CCU）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourcePackages: list of ResourcePackage
         """
         self.Uin = None
         self.AppId = None
         self.ClusterId = None
         self.ClusterName = None
         self.InstanceId = None
         self.InstanceName = None
         self.ProjectId = None
         self.Region = None
         self.Zone = None
         self.Status = None
         self.StatusDesc = None
+        self.DbMode = None
         self.DbType = None
         self.DbVersion = None
         self.Cpu = None
         self.Memory = None
         self.Storage = None
         self.InstanceType = None
         self.InstanceRole = None
@@ -2478,28 +2665,30 @@
         self.BusinessType = None
         self.Tasks = None
         self.IsFreeze = None
         self.ResourceTags = None
         self.MasterZone = None
         self.SlaveZones = None
         self.InstanceNetInfo = None
+        self.ResourcePackages = None
 
 
     def _deserialize(self, params):
         self.Uin = params.get("Uin")
         self.AppId = params.get("AppId")
         self.ClusterId = params.get("ClusterId")
         self.ClusterName = params.get("ClusterName")
         self.InstanceId = params.get("InstanceId")
         self.InstanceName = params.get("InstanceName")
         self.ProjectId = params.get("ProjectId")
         self.Region = params.get("Region")
         self.Zone = params.get("Zone")
         self.Status = params.get("Status")
         self.StatusDesc = params.get("StatusDesc")
+        self.DbMode = params.get("DbMode")
         self.DbType = params.get("DbType")
         self.DbVersion = params.get("DbVersion")
         self.Cpu = params.get("Cpu")
         self.Memory = params.get("Memory")
         self.Storage = params.get("Storage")
         self.InstanceType = params.get("InstanceType")
         self.InstanceRole = params.get("InstanceRole")
@@ -2546,14 +2735,20 @@
         self.SlaveZones = params.get("SlaveZones")
         if params.get("InstanceNetInfo") is not None:
             self.InstanceNetInfo = []
             for item in params.get("InstanceNetInfo"):
                 obj = InstanceNetInfo()
                 obj._deserialize(item)
                 self.InstanceNetInfo.append(obj)
+        if params.get("ResourcePackages") is not None:
+            self.ResourcePackages = []
+            for item in params.get("ResourcePackages"):
+                obj = ResourcePackage()
+                obj._deserialize(item)
+                self.ResourcePackages.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5431,14 +5626,259 @@
                 obj = SecurityGroup()
                 obj._deserialize(item)
                 self.Groups.append(obj)
         self.Total = params.get("Total")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeResourcePackageDetailRequest(AbstractModel):
+    """DescribeResourcePackageDetail请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PackageId: 资源包唯一ID
+        :type PackageId: str
+        :param ClusterIds: 实例ID
+        :type ClusterIds: list of str
+        :param StartTime: 开始时间
+        :type StartTime: str
+        :param EndTime: 结束时间
+        :type EndTime: str
+        :param Offset: 偏移量
+        :type Offset: str
+        :param Limit: 限制
+        :type Limit: str
+        """
+        self.PackageId = None
+        self.ClusterIds = None
+        self.StartTime = None
+        self.EndTime = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.PackageId = params.get("PackageId")
+        self.ClusterIds = params.get("ClusterIds")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeResourcePackageDetailResponse(AbstractModel):
+    """DescribeResourcePackageDetail返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Total: 总使用明细数
+        :type Total: int
+        :param Detail: 资源包明细说明
+        :type Detail: list of PackageDetail
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Total = None
+        self.Detail = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Total = params.get("Total")
+        if params.get("Detail") is not None:
+            self.Detail = []
+            for item in params.get("Detail"):
+                obj = PackageDetail()
+                obj._deserialize(item)
+                self.Detail.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeResourcePackageListRequest(AbstractModel):
+    """DescribeResourcePackageList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PackageId: 资源包唯一ID
+        :type PackageId: list of str
+        :param PackageName: 资源包名称
+        :type PackageName: list of str
+        :param PackageType: 资源包类型
+CCU-计算资源包，DISK-存储资源包
+        :type PackageType: list of str
+        :param PackageRegion: 资源包使用地域
+china-中国内地通用，overseas-港澳台及海外通用
+        :type PackageRegion: list of str
+        :param Status: 资源包状态
+creating-创建中；
+using-使用中；
+expired-已过期；
+normal_finish-使用完；
+apply_refund-申请退费中；
+refund-已退费。
+        :type Status: list of str
+        :param OrderBy: 排序条件，支持排序条件:startTime-生效时间，
+expireTime-过期时间，packageUsedSpec-使用容量，packageTotalSpec-总存储量。
+按照数组顺序排列；
+        :type OrderBy: list of str
+        :param OrderDirection: 排序方式，DESC-降序，ASC-升序
+        :type OrderDirection: str
+        :param Offset: 偏移量
+        :type Offset: int
+        :param Limit: 限制
+        :type Limit: int
+        """
+        self.PackageId = None
+        self.PackageName = None
+        self.PackageType = None
+        self.PackageRegion = None
+        self.Status = None
+        self.OrderBy = None
+        self.OrderDirection = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.PackageId = params.get("PackageId")
+        self.PackageName = params.get("PackageName")
+        self.PackageType = params.get("PackageType")
+        self.PackageRegion = params.get("PackageRegion")
+        self.Status = params.get("Status")
+        self.OrderBy = params.get("OrderBy")
+        self.OrderDirection = params.get("OrderDirection")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeResourcePackageListResponse(AbstractModel):
+    """DescribeResourcePackageList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Total: 总配置数
+        :type Total: int
+        :param Detail: 资源包明细
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Detail: list of Package
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Total = None
+        self.Detail = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Total = params.get("Total")
+        if params.get("Detail") is not None:
+            self.Detail = []
+            for item in params.get("Detail"):
+                obj = Package()
+                obj._deserialize(item)
+                self.Detail.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeResourcePackageSaleSpecRequest(AbstractModel):
+    """DescribeResourcePackageSaleSpec请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceType: 实例类型
+        :type InstanceType: str
+        :param PackageRegion: 资源包使用地域
+china-中国内地通用，overseas-港澳台及海外通用
+        :type PackageRegion: str
+        :param PackageType: 资源包类型
+CCU-计算资源包
+DISK-存储资源包
+        :type PackageType: str
+        :param Offset: 偏移量
+        :type Offset: int
+        :param Limit: 限制
+        :type Limit: int
+        """
+        self.InstanceType = None
+        self.PackageRegion = None
+        self.PackageType = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.InstanceType = params.get("InstanceType")
+        self.PackageRegion = params.get("PackageRegion")
+        self.PackageType = params.get("PackageType")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeResourcePackageSaleSpecResponse(AbstractModel):
+    """DescribeResourcePackageSaleSpec返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Total: 可售卖资源包规格总数
+        :type Total: int
+        :param Detail: 资源包明细说明
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Detail: list of SalePackageSpec
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Total = None
+        self.Detail = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Total = params.get("Total")
+        if params.get("Detail") is not None:
+            self.Detail = []
+            for item in params.get("Detail"):
+                obj = SalePackageSpec()
+                obj._deserialize(item)
+                self.Detail.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeResourcesByDealNameRequest(AbstractModel):
     """DescribeResourcesByDealName请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7709,14 +8149,108 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifyResourcePackageClustersRequest(AbstractModel):
+    """ModifyResourcePackageClusters请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PackageId: 资源包唯一ID
+        :type PackageId: str
+        :param BindClusterIds: 需要建立绑定关系的集群ID
+        :type BindClusterIds: list of str
+        :param UnbindClusterIds: 需要解除绑定关系的集群ID
+        :type UnbindClusterIds: list of str
+        """
+        self.PackageId = None
+        self.BindClusterIds = None
+        self.UnbindClusterIds = None
+
+
+    def _deserialize(self, params):
+        self.PackageId = params.get("PackageId")
+        self.BindClusterIds = params.get("BindClusterIds")
+        self.UnbindClusterIds = params.get("UnbindClusterIds")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyResourcePackageClustersResponse(AbstractModel):
+    """ModifyResourcePackageClusters返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class ModifyResourcePackageNameRequest(AbstractModel):
+    """ModifyResourcePackageName请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PackageId: 资源包唯一ID
+        :type PackageId: str
+        :param PackageName: 自定义的资源包名称，最长支持120个字符
+        :type PackageName: str
+        """
+        self.PackageId = None
+        self.PackageName = None
+
+
+    def _deserialize(self, params):
+        self.PackageId = params.get("PackageId")
+        self.PackageName = params.get("PackageName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyResourcePackageNameResponse(AbstractModel):
+    """ModifyResourcePackageName返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyVipVportRequest(AbstractModel):
     """ModifyVipVport请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8333,14 +8867,167 @@
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         self.RequestId = params.get("RequestId")
 
 
+class Package(AbstractModel):
+    """资源包
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AppId: AppID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppId: int
+        :param PackageId: 资源包唯一ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageId: str
+        :param PackageName: 资源包名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageName: str
+        :param PackageType: 资源包类型
+CCU-计算资源包，DISK-存储资源包
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageType: str
+        :param PackageRegion: 资源包使用地域
+china-中国内地通用，overseas-港澳台及海外通用
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageRegion: str
+        :param Status: 资源包状态
+creating-创建中；
+using-使用中；
+expired-已过期；
+normal_finish-使用完；
+apply_refund-申请退费中；
+refund-已退费。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: str
+        :param PackageTotalSpec: 资源包总量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageTotalSpec: float
+        :param PackageUsedSpec: 资源包已使用量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageUsedSpec: float
+        :param HasQuota: 资源包已使用量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HasQuota: bool
+        :param BindInstanceInfos: 绑定实例信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BindInstanceInfos: list of BindInstanceInfo
+        :param StartTime: 生效时间：2022-07-01 00:00:00
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StartTime: str
+        :param ExpireTime: 失效时间：2022-08-01 00:00:00
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExpireTime: str
+        """
+        self.AppId = None
+        self.PackageId = None
+        self.PackageName = None
+        self.PackageType = None
+        self.PackageRegion = None
+        self.Status = None
+        self.PackageTotalSpec = None
+        self.PackageUsedSpec = None
+        self.HasQuota = None
+        self.BindInstanceInfos = None
+        self.StartTime = None
+        self.ExpireTime = None
+
+
+    def _deserialize(self, params):
+        self.AppId = params.get("AppId")
+        self.PackageId = params.get("PackageId")
+        self.PackageName = params.get("PackageName")
+        self.PackageType = params.get("PackageType")
+        self.PackageRegion = params.get("PackageRegion")
+        self.Status = params.get("Status")
+        self.PackageTotalSpec = params.get("PackageTotalSpec")
+        self.PackageUsedSpec = params.get("PackageUsedSpec")
+        self.HasQuota = params.get("HasQuota")
+        if params.get("BindInstanceInfos") is not None:
+            self.BindInstanceInfos = []
+            for item in params.get("BindInstanceInfos"):
+                obj = BindInstanceInfo()
+                obj._deserialize(item)
+                self.BindInstanceInfos.append(obj)
+        self.StartTime = params.get("StartTime")
+        self.ExpireTime = params.get("ExpireTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class PackageDetail(AbstractModel):
+    """资源包明细说明
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AppId: AppId账户ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppId: int
+        :param PackageId: 资源包唯一ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageId: str
+        :param InstanceId: 实例ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceId: str
+        :param SuccessDeductSpec: 成功抵扣容量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SuccessDeductSpec: float
+        :param PackageTotalUsedSpec: 截止当前，资源包已使用的容量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageTotalUsedSpec: float
+        :param StartTime: 抵扣开始时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StartTime: str
+        :param EndTime: 抵扣结束时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EndTime: str
+        :param ExtendInfo: 扩展信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExtendInfo: str
+        """
+        self.AppId = None
+        self.PackageId = None
+        self.InstanceId = None
+        self.SuccessDeductSpec = None
+        self.PackageTotalUsedSpec = None
+        self.StartTime = None
+        self.EndTime = None
+        self.ExtendInfo = None
+
+
+    def _deserialize(self, params):
+        self.AppId = params.get("AppId")
+        self.PackageId = params.get("PackageId")
+        self.InstanceId = params.get("InstanceId")
+        self.SuccessDeductSpec = params.get("SuccessDeductSpec")
+        self.PackageTotalUsedSpec = params.get("PackageTotalUsedSpec")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.ExtendInfo = params.get("ExtendInfo")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ParamDetail(AbstractModel):
     """实例参数详细描述
 
     """
 
     def __init__(self):
         r"""
@@ -8803,14 +9490,59 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RefundResourcePackageRequest(AbstractModel):
+    """RefundResourcePackage请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PackageId: 资源包唯一ID
+        :type PackageId: str
+        """
+        self.PackageId = None
+
+
+    def _deserialize(self, params):
+        self.PackageId = params.get("PackageId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RefundResourcePackageResponse(AbstractModel):
+    """RefundResourcePackage返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DealNames: 每个物品对应一个dealName，业务需要根据dealName保证发货接口幂等
+        :type DealNames: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DealNames = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.DealNames = params.get("DealNames")
+        self.RequestId = params.get("RequestId")
+
+
 class RemoveClusterSlaveZoneRequest(AbstractModel):
     """RemoveClusterSlaveZone请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8905,14 +9637,45 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ResourcePackage(AbstractModel):
+    """资源包信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PackageId: 资源包的唯一ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageId: str
+        :param PackageType: 资源包类型：CCU：计算资源包
+DISK：存储资源包
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageType: str
+        """
+        self.PackageId = None
+        self.PackageType = None
+
+
+    def _deserialize(self, params):
+        self.PackageId = params.get("PackageId")
+        self.PackageType = params.get("PackageType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class RestartInstanceRequest(AbstractModel):
     """RestartInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9287,14 +10050,67 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class SalePackageSpec(AbstractModel):
+    """资源包明细说明
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PackageRegion: 资源包使用地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageRegion: str
+        :param PackageType: 资源包类型
+CCU-计算资源包
+DISK-存储资源包
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageType: str
+        :param PackageVersion: 资源包版本
+base-基础版本，common-通用版本，enterprise-企业版本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageVersion: str
+        :param MinPackageSpec: 当前版本资源包最小资源数，计算资源单位：个；存储资源：GB
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MinPackageSpec: float
+        :param MaxPackageSpec: 当前版本资源包最大资源数，计算资源单位：个；存储资源：GB
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MaxPackageSpec: float
+        :param ExpireDay: 资源包有效期，单位:天
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExpireDay: int
+        """
+        self.PackageRegion = None
+        self.PackageType = None
+        self.PackageVersion = None
+        self.MinPackageSpec = None
+        self.MaxPackageSpec = None
+        self.ExpireDay = None
+
+
+    def _deserialize(self, params):
+        self.PackageRegion = params.get("PackageRegion")
+        self.PackageType = params.get("PackageType")
+        self.PackageVersion = params.get("PackageVersion")
+        self.MinPackageSpec = params.get("MinPackageSpec")
+        self.MaxPackageSpec = params.get("MaxPackageSpec")
+        self.ExpireDay = params.get("ExpireDay")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class SaleRegion(AbstractModel):
     """售卖地域信息
 
     """
 
     def __init__(self):
         r"""
@@ -10033,14 +10849,59 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class UnbindClusterResourcePackagesRequest(AbstractModel):
+    """UnbindClusterResourcePackages请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param PackageIds: 资源包唯一ID,如果不传，解绑该实例绑定的所有资源包
+        :type PackageIds: list of str
+        """
+        self.ClusterId = None
+        self.PackageIds = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.PackageIds = params.get("PackageIds")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UnbindClusterResourcePackagesResponse(AbstractModel):
+    """UnbindClusterResourcePackages返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class UpgradeClusterVersionRequest(AbstractModel):
     """UpgradeClusterVersion请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.902/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.903/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.903/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.902/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.903/setup.py`

 * *Files identical despite different names*

