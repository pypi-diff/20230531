# Comparing `tmp/iam_actions-1.2.20230530.tar.gz` & `tmp/iam_actions-1.2.20230531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230530.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230531.tar", max compression
```

## Comparing `iam_actions-1.2.20230530.tar` & `iam_actions-1.2.20230531.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/README.md
--rw-r--r--   0        0        0      228 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/__init__.py
--rw-r--r--   0        0        0  4275737 2023-05-30 02:34:44.736123 iam_actions-1.2.20230530/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/services.py
--rw-r--r--   0        0        0   549706 2023-05-30 02:34:44.736123 iam_actions-1.2.20230530/iam_actions/policies.json
--rw-r--r--   0        0        0   194779 2023-05-30 02:34:44.736123 iam_actions-1.2.20230530/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   533245 2023-05-30 02:34:44.736123 iam_actions-1.2.20230530/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-30 02:34:45.508125 iam_actions-1.2.20230530/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230530/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230530/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/README.md
+-rw-r--r--   0        0        0      228 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4280299 2023-05-31 02:49:49.509393 iam_actions-1.2.20230531/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-31 02:48:07.461038 iam_actions-1.2.20230531/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   549782 2023-05-31 02:49:49.513393 iam_actions-1.2.20230531/iam_actions/policies.json
+-rw-r--r--   0        0        0   195033 2023-05-31 02:49:49.509393 iam_actions-1.2.20230531/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   533302 2023-05-31 02:49:49.509393 iam_actions-1.2.20230531/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-31 02:49:50.577393 iam_actions-1.2.20230531/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230531/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230531/PKG-INFO
```

### Comparing `iam_actions-1.2.20230530/LICENSE` & `iam_actions-1.2.20230531/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230530/README.md` & `iam_actions-1.2.20230531/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230530/iam_actions/actions.json` & `iam_actions-1.2.20230531/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994748391246139%*

 * *Differences: {"'iq'": "{'ListAttachments': {'access_level': 'List', 'description': 'Grants permission to list "*

 * *         "existing attachments', 'resources': ['attachment']}, 'DownloadAttachment': "*

 * *         "{'access_level': 'Read', 'description': 'Grants permission to download existing "*

 * *         "attachment', 'resources': ['attachment']}, 'GetRequest': {'access_level': 'Read', "*

 * *         "'description': 'Grants permission to get a created request', 'resources': ['request']}}",*

 * * "'quicksight'": "{'DescribeAssetBundleI […]*

```diff
@@ -81058,20 +81058,22 @@
             "description": "Grants permission to delete an existing attachment",
             "orphan": false,
             "resources": [
                 "attachment"
             ]
         },
         "DownloadAttachment": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DownloadAttachment",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to download existing attachment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "attachment"
+            ]
         },
         "EndCall": {
             "access_level": "Write",
             "action": "EndCall",
             "condition_keys": [],
             "description": "Grants permission to end a voice/video call",
             "orphan": false,
@@ -81196,20 +81198,22 @@
             "description": "Grants permission to read a proposal",
             "orphan": false,
             "resources": [
                 "proposal"
             ]
         },
         "GetRequest": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetRequest",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get a created request",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "request"
+            ]
         },
         "GetReview": {
             "access_level": "Read",
             "action": "GetReview",
             "condition_keys": [],
             "description": "Grants permission to read a review for an expert",
             "orphan": false,
@@ -81232,20 +81236,22 @@
             "action": "InitiateCall",
             "condition_keys": [],
             "description": "Grants permission to start a voice/video call",
             "orphan": false,
             "resources": []
         },
         "ListAttachments": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListAttachments",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list existing attachments",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "attachment"
+            ]
         },
         "ListConversations": {
             "access_level": "Read",
             "action": "ListConversations",
             "condition_keys": [],
             "description": "Grants permission to list existing conversations",
             "orphan": false,
@@ -109606,28 +109612,32 @@
             "description": "Grants permission to describe permissions for an analysis",
             "orphan": false,
             "resources": [
                 "analysis"
             ]
         },
         "DescribeAssetBundleExportJob": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeAssetBundleExportJob",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe an asset bundle export job",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "assetBundleExportJob"
+            ]
         },
         "DescribeAssetBundleImportJob": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeAssetBundleImportJob",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe an asset bundle import job",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "assetBundleImportJob"
+            ]
         },
         "DescribeCustomPermissions": {
             "access_level": "Write",
             "action": "DescribeCustomPermissions",
             "condition_keys": [],
             "description": "Grants permission to describe a custom permissions resource in a QuickSight account",
             "orphan": false,
@@ -110039,28 +110049,32 @@
             "description": "Grants permission to list all analyses in an account",
             "orphan": false,
             "resources": [
                 "analysis"
             ]
         },
         "ListAssetBundleExportJobs": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListAssetBundleExportJobs",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all asset bundle export jobs",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "assetBundleExportJob"
+            ]
         },
         "ListAssetBundleImportJobs": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListAssetBundleImportJobs",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all asset bundle import jobs",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "assetBundleImportJob"
+            ]
         },
         "ListCustomPermissions": {
             "access_level": "Write",
             "action": "ListCustomPermissions",
             "condition_keys": [],
             "description": "Grants permission to list custom permissions resources in QuickSight account",
             "orphan": false,
@@ -110460,28 +110474,32 @@
             "action": "SetGroupMapping",
             "condition_keys": [],
             "description": "Grants permission to use Amazon QuickSight, in Enterprise edition, to display your Microsoft Active Directory directory groups so that you can choose which ones to map to roles in Amazon QuickSight",
             "orphan": false,
             "resources": []
         },
         "StartAssetBundleExportJob": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartAssetBundleExportJob",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to start an asset bundle export job",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "assetBundleExportJob"
+            ]
         },
         "StartAssetBundleImportJob": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartAssetBundleImportJob",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to start an asset bundle import job",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "assetBundleImportJob"
+            ]
         },
         "Subscribe": {
             "access_level": "Write",
             "action": "Subscribe",
             "condition_keys": [
                 "quicksight:DirectoryType",
                 "quicksight:Edition"
@@ -129913,14 +129931,38 @@
             "access_level": "Write",
             "action": "CreateCustomLogSource",
             "condition_keys": [],
             "description": "Grants permission to add a custom source name",
             "orphan": false,
             "resources": []
         },
+        "CreateDataLake": {
+            "access_level": "Undocumented",
+            "action": "CreateDataLake",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateDataLakeExceptionSubscription": {
+            "access_level": "Undocumented",
+            "action": "CreateDataLakeExceptionSubscription",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateDataLakeOrganizationConfiguration": {
+            "access_level": "Undocumented",
+            "action": "CreateDataLakeOrganizationConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateDatalake": {
             "access_level": "Write",
             "action": "CreateDatalake",
             "condition_keys": [],
             "description": "Grants permission to create a new Security Data Lake",
             "orphan": false,
             "resources": []
@@ -129953,14 +129995,22 @@
             "access_level": "Write",
             "action": "CreateSubscriber",
             "condition_keys": [],
             "description": "Grants permission to create a subscription permission for accounts that are already enabled",
             "orphan": false,
             "resources": []
         },
+        "CreateSubscriberNotification": {
+            "access_level": "Undocumented",
+            "action": "CreateSubscriberNotification",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateSubscriptionNotificationConfiguration": {
             "access_level": "Write",
             "action": "CreateSubscriptionNotificationConfiguration",
             "condition_keys": [],
             "description": "Grants permission to create a webhook invocation to notify a client when there is new data in the Data Lake",
             "orphan": false,
             "resources": []
@@ -129977,14 +130027,38 @@
             "access_level": "Write",
             "action": "DeleteCustomLogSource",
             "condition_keys": [],
             "description": "Grants permission to remove a custom source name",
             "orphan": false,
             "resources": []
         },
+        "DeleteDataLake": {
+            "access_level": "Undocumented",
+            "action": "DeleteDataLake",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteDataLakeExceptionSubscription": {
+            "access_level": "Undocumented",
+            "action": "DeleteDataLakeExceptionSubscription",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteDataLakeOrganizationConfiguration": {
+            "access_level": "Undocumented",
+            "action": "DeleteDataLakeOrganizationConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteDatalake": {
             "access_level": "Write",
             "action": "DeleteDatalake",
             "condition_keys": [],
             "description": "Grants permission to delete all Security Data Lakes",
             "orphan": false,
             "resources": []
@@ -130017,22 +130091,62 @@
             "access_level": "Write",
             "action": "DeleteSubscriber",
             "condition_keys": [],
             "description": "Grants permission to delete the specified subscription permissions for accounts that are already enabled",
             "orphan": false,
             "resources": []
         },
+        "DeleteSubscriberNotification": {
+            "access_level": "Undocumented",
+            "action": "DeleteSubscriberNotification",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteSubscriptionNotificationConfiguration": {
             "access_level": "Write",
             "action": "DeleteSubscriptionNotificationConfiguration",
             "condition_keys": [],
             "description": "Grants permission to remove a webhook invocation to notify a client when there is new data in the Data Lake",
             "orphan": false,
             "resources": []
         },
+        "DeregisterDataLakeDelegatedAdministrator": {
+            "access_level": "Undocumented",
+            "action": "DeregisterDataLakeDelegatedAdministrator",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetDataLakeExceptionSubscription": {
+            "access_level": "Undocumented",
+            "action": "GetDataLakeExceptionSubscription",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetDataLakeOrganizationConfiguration": {
+            "access_level": "Undocumented",
+            "action": "GetDataLakeOrganizationConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetDataLakeSources": {
+            "access_level": "Undocumented",
+            "action": "GetDataLakeSources",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetDatalake": {
             "access_level": "Read",
             "action": "GetDatalake",
             "condition_keys": [],
             "description": "Grants permission to get information on the Security Data Lake",
             "orphan": false,
             "resources": []
@@ -130081,14 +130195,30 @@
             "access_level": "Read",
             "action": "GetSubscriptionNotificationConfiguration",
             "condition_keys": [],
             "description": "Grants permission to get information for a webhook invocation to notify a client when there is new data in the Data Lake",
             "orphan": false,
             "resources": []
         },
+        "ListDataLakeExceptions": {
+            "access_level": "Undocumented",
+            "action": "ListDataLakeExceptions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListDataLakes": {
+            "access_level": "Undocumented",
+            "action": "ListDataLakes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListDatalakeExceptions": {
             "access_level": "List",
             "action": "ListDatalakeExceptions",
             "condition_keys": [],
             "description": "Grants permission to get the list of all non-retry-able failures",
             "orphan": false,
             "resources": []
@@ -130105,14 +130235,38 @@
             "access_level": "List",
             "action": "ListSubscribers",
             "condition_keys": [],
             "description": "Grants permission to list all subscription permissions for accounts that are already enabled",
             "orphan": false,
             "resources": []
         },
+        "RegisterDataLakeDelegatedAdministrator": {
+            "access_level": "Undocumented",
+            "action": "RegisterDataLakeDelegatedAdministrator",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateDataLake": {
+            "access_level": "Undocumented",
+            "action": "UpdateDataLake",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateDataLakeExceptionSubscription": {
+            "access_level": "Undocumented",
+            "action": "UpdateDataLakeExceptionSubscription",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateDatalake": {
             "access_level": "Write",
             "action": "UpdateDatalake",
             "condition_keys": [],
             "description": "Grants permission to update a Security Data Lake",
             "orphan": false,
             "resources": []
@@ -130137,14 +130291,22 @@
             "access_level": "Write",
             "action": "UpdateSubscriber",
             "condition_keys": [],
             "description": "Grants permission to update subscription information for a subscription permission for accounts that are already enabled",
             "orphan": false,
             "resources": []
         },
+        "UpdateSubscriberNotification": {
+            "access_level": "Undocumented",
+            "action": "UpdateSubscriberNotification",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateSubscriptionNotificationConfiguration": {
             "access_level": "Write",
             "action": "UpdateSubscriptionNotificationConfiguration",
             "condition_keys": [],
             "description": "Grants permission to update a webhook invocation to notify a client when there is new data in the Data Lake",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20230530/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230531/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230530/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230531/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230530/iam_actions/generate/generate.py` & `iam_actions-1.2.20230531/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230530/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230531/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230530/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230531/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230530/iam_actions/generate/services.py` & `iam_actions-1.2.20230531/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230530/iam_actions/policies.json` & `iam_actions-1.2.20230531/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999212890284319%*

 * *Differences: {"'serviceMap'": "{'Amazon Security Lake': {'Actions': {insert: [(2, 'CreateDataLake'), (3, "*

 * *                 "'CreateDataLakeExceptionSubscription'), (4, "*

 * *                 "'CreateDataLakeOrganizationConfiguration'), (6, 'CreateSubscriberNotification'), "*

 * *                 "(9, 'DeleteDataLake'), (10, 'DeleteDataLakeExceptionSubscription'), (11, "*

 * *                 "'DeleteDataLakeOrganizationConfiguration'), (13, "*

 * *                 "'DeleteSubscriberNotification'), (14, "*

 * *                 "'DeregisterData […]*

```diff
@@ -5443,14 +5443,15 @@
             ],
             "HasResource": true,
             "StringPrefix": "iotfleetwise",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
+                "iotfleetwise:DestinationArn",
                 "iotfleetwise:UpdateToDecoderManifestArn",
                 "iotfleetwise:UpdateToModelManifestArn"
             ]
         },
         "AWS IoT Greengrass": {
             "ARNFormat": "arn:aws:greengrass:${Region}:${Account}:/greengrass/${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:greengrass:.+:[0-9]+:.+",
@@ -18680,48 +18681,47 @@
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
         "Amazon Security Lake": {
+            "ARNFormat": "arn:aws:securitylake:${Region}:${Account}:${ResourceType}/${ResourcePath}",
+            "ARNRegex": "^arn:aws:securitylake:.+:.+:.+",
             "Actions": [
                 "CreateAwsLogSource",
                 "CreateCustomLogSource",
-                "CreateDatalake",
-                "CreateDatalakeAutoEnable",
-                "CreateDatalakeDelegatedAdmin",
-                "CreateDatalakeExceptionsSubscription",
+                "CreateDataLake",
+                "CreateDataLakeExceptionSubscription",
+                "CreateDataLakeOrganizationConfiguration",
                 "CreateSubscriber",
-                "CreateSubscriptionNotificationConfiguration",
+                "CreateSubscriberNotification",
                 "DeleteAwsLogSource",
                 "DeleteCustomLogSource",
-                "DeleteDatalake",
-                "DeleteDatalakeAutoEnable",
-                "DeleteDatalakeDelegatedAdmin",
-                "DeleteDatalakeExceptionsSubscription",
+                "DeleteDataLake",
+                "DeleteDataLakeExceptionSubscription",
+                "DeleteDataLakeOrganizationConfiguration",
                 "DeleteSubscriber",
-                "DeleteSubscriptionNotificationConfiguration",
-                "GetDatalake",
-                "GetDatalakeAutoEnable",
-                "GetDatalakeExceptionsExpiry",
-                "GetDatalakeExceptionsSubscription",
-                "GetDatalakeStatus",
+                "DeleteSubscriberNotification",
+                "DeregisterDataLakeDelegatedAdministrator",
+                "GetDataLakeExceptionSubscription",
+                "GetDataLakeOrganizationConfiguration",
+                "GetDataLakeSources",
                 "GetSubscriber",
-                "GetSubscriptionNotificationConfiguration",
-                "ListDatalakeExceptions",
+                "ListDataLakeExceptions",
+                "ListDataLakes",
                 "ListLogSources",
                 "ListSubscribers",
-                "UpdateDatalake",
-                "UpdateDatalakeExceptionsExpiry",
-                "UpdateDatalakeExceptionsSubscription",
+                "RegisterDataLakeDelegatedAdministrator",
+                "UpdateDataLake",
+                "UpdateDataLakeExceptionSubscription",
                 "UpdateSubscriber",
-                "UpdateSubscriptionNotificationConfiguration"
+                "UpdateSubscriberNotification"
             ],
-            "HasResource": false,
+            "HasResource": true,
             "StringPrefix": "securitylake"
         },
         "Amazon Session Manager Message Gateway Service": {
             "Actions": [
                 "CreateControlChannel",
                 "CreateDataChannel",
                 "OpenControlChannel",
```

### Comparing `iam_actions-1.2.20230530/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230531/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998611111111111%*

 * *Differences: {"'quicksight'": "{'assetBundleExportJob': OrderedDict([('arn_pattern', "*

 * *                 "'arn:*:quicksight:*:*:asset-bundle-export-job/*'), ('condition_keys', None)]), "*

 * *                 "'assetBundleImportJob': OrderedDict([('arn_pattern', "*

 * *                 "'arn:*:quicksight:*:*:asset-bundle-import-job/*'), ('condition_keys', None)])}"}*

```diff
@@ -4893,14 +4893,22 @@
             "arn_pattern": "arn:*:quicksight:*:*:account/*",
             "condition_keys": null
         },
         "analysis": {
             "arn_pattern": "arn:*:quicksight:*:*:analysis/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "assetBundleExportJob": {
+            "arn_pattern": "arn:*:quicksight:*:*:asset-bundle-export-job/*",
+            "condition_keys": null
+        },
+        "assetBundleImportJob": {
+            "arn_pattern": "arn:*:quicksight:*:*:asset-bundle-import-job/*",
+            "condition_keys": null
+        },
         "assignment": {
             "arn_pattern": "arn:*:quicksight::*:assignment/*",
             "condition_keys": null
         },
         "customization": {
             "arn_pattern": "arn:*:quicksight:*:*:customization/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20230530/iam_actions/services.json` & `iam_actions-1.2.20230531/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999541367472915%*

 * *Differences: {"'iotfleetwise'": "{'ConditionKeys': {insert: [(3, 'iotfleetwise:DestinationArn')]}}",*

 * * "'securitylake'": "{'Actions': {insert: [(2, 'CreateDataLake'), (3, "*

 * *                   "'CreateDataLakeExceptionSubscription'), (4, "*

 * *                   "'CreateDataLakeOrganizationConfiguration'), (6, "*

 * *                   "'CreateSubscriberNotification'), (9, 'DeleteDataLake'), (10, "*

 * *                   "'DeleteDataLakeExceptionSubscription'), (11, "*

 * *                   "'DeleteDataLakeOrganizationConfiguration'), (13 […]*

```diff
@@ -10839,14 +10839,15 @@
             "UpdateSignalCatalog",
             "UpdateVehicle"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys",
+            "iotfleetwise:DestinationArn",
             "iotfleetwise:UpdateToDecoderManifestArn",
             "iotfleetwise:UpdateToModelManifestArn"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS IoT FleetWise"
         ]
@@ -18020,51 +18021,52 @@
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Security Hub"
         ]
     },
     "securitylake": {
-        "ARNFormats": [],
-        "ARNRegexes": [],
+        "ARNFormats": [
+            "arn:aws:securitylake:${Region}:${Account}:${ResourceType}/${ResourcePath}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:securitylake:.+:.+:.+"
+        ],
         "Actions": [
             "CreateAwsLogSource",
             "CreateCustomLogSource",
-            "CreateDatalake",
-            "CreateDatalakeAutoEnable",
-            "CreateDatalakeDelegatedAdmin",
-            "CreateDatalakeExceptionsSubscription",
+            "CreateDataLake",
+            "CreateDataLakeExceptionSubscription",
+            "CreateDataLakeOrganizationConfiguration",
             "CreateSubscriber",
-            "CreateSubscriptionNotificationConfiguration",
+            "CreateSubscriberNotification",
             "DeleteAwsLogSource",
             "DeleteCustomLogSource",
-            "DeleteDatalake",
-            "DeleteDatalakeAutoEnable",
-            "DeleteDatalakeDelegatedAdmin",
-            "DeleteDatalakeExceptionsSubscription",
+            "DeleteDataLake",
+            "DeleteDataLakeExceptionSubscription",
+            "DeleteDataLakeOrganizationConfiguration",
             "DeleteSubscriber",
-            "DeleteSubscriptionNotificationConfiguration",
-            "GetDatalake",
-            "GetDatalakeAutoEnable",
-            "GetDatalakeExceptionsExpiry",
-            "GetDatalakeExceptionsSubscription",
-            "GetDatalakeStatus",
+            "DeleteSubscriberNotification",
+            "DeregisterDataLakeDelegatedAdministrator",
+            "GetDataLakeExceptionSubscription",
+            "GetDataLakeOrganizationConfiguration",
+            "GetDataLakeSources",
             "GetSubscriber",
-            "GetSubscriptionNotificationConfiguration",
-            "ListDatalakeExceptions",
+            "ListDataLakeExceptions",
+            "ListDataLakes",
             "ListLogSources",
             "ListSubscribers",
-            "UpdateDatalake",
-            "UpdateDatalakeExceptionsExpiry",
-            "UpdateDatalakeExceptionsSubscription",
+            "RegisterDataLakeDelegatedAdministrator",
+            "UpdateDataLake",
+            "UpdateDataLakeExceptionSubscription",
             "UpdateSubscriber",
-            "UpdateSubscriptionNotificationConfiguration"
+            "UpdateSubscriberNotification"
         ],
         "ConditionKeys": [],
-        "HasResource": false,
+        "HasResource": true,
         "ServiceNames": [
             "Amazon Security Lake"
         ]
     },
     "serverlessrepo": {
         "ARNFormats": [
             "arn:aws:serverlessrepo:${Region}:${Account}:${ResourceType}/${ResourceId}"
```

### Comparing `iam_actions-1.2.20230530/pyproject.toml` & `iam_actions-1.2.20230531/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230530"
+version = "1.2.20230531"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230530/setup.py` & `iam_actions-1.2.20230531/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230530',
+    'version': '1.2.20230531',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230530/PKG-INFO` & `iam_actions-1.2.20230531/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230530
+Version: 1.2.20230531
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

