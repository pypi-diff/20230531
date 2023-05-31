# Comparing `tmp/policyuniverse-1.5.1.20230526.tar.gz` & `tmp/policyuniverse-1.5.1.20230531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyuniverse-1.5.1.20230526.tar", last modified: Fri May 26 15:39:15 2023, max compression
+gzip compressed data, was "policyuniverse-1.5.1.20230531.tar", last modified: Wed May 31 17:21:54 2023, max compression
```

## Comparing `policyuniverse-1.5.1.20230526.tar` & `policyuniverse-1.5.1.20230531.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:15.496235 policyuniverse-1.5.1.20230526/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-26 15:39:15.496235 policyuniverse-1.5.1.20230526/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:15.496235 policyuniverse-1.5.1.20230526/policyuniverse/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/action_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/arn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/common.py
--rw-r--r--   0 runner    (1001) docker     (123)  7791087 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/data.json
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/expander_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:15.496235 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-26 15:39:15.000000 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-26 15:39:15.000000 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:39:15.000000 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:39:15.000000 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-26 15:39:15.000000 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 15:39:15.000000 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-26 15:39:15.496235 policyuniverse-1.5.1.20230526/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:21:54.715176 policyuniverse-1.5.1.20230531/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-31 17:21:54.715176 policyuniverse-1.5.1.20230531/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:21:54.711176 policyuniverse-1.5.1.20230531/policyuniverse/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/action_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/arn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7793680 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/expander_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:21:54.715176 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-31 17:21:54.000000 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-31 17:21:54.000000 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:21:54.000000 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:21:54.000000 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-31 17:21:54.000000 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 17:21:54.000000 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-31 17:21:54.715176 policyuniverse-1.5.1.20230531/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/setup.py
```

### Comparing `policyuniverse-1.5.1.20230526/LICENSE` & `policyuniverse-1.5.1.20230531/LICENSE`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230526/PKG-INFO` & `policyuniverse-1.5.1.20230531/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyuniverse
-Version: 1.5.1.20230526
+Version: 1.5.1.20230531
 Summary: Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.
 Home-page: https://github.com/Netflix-Skunkworks/policyuniverse
 Author: Patrick Kelley
 Author-email: patrickbarrettkelley@gmail.com
 Keywords: iam,arn,action_groups,condition,policy,statement,wildcard
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
```

### Comparing `policyuniverse-1.5.1.20230526/README.md` & `policyuniverse-1.5.1.20230531/README.md`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230526/policyuniverse/__init__.py` & `policyuniverse-1.5.1.20230531/policyuniverse/__init__.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230526/policyuniverse/action.py` & `policyuniverse-1.5.1.20230531/policyuniverse/action.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230526/policyuniverse/action_categories.py` & `policyuniverse-1.5.1.20230531/policyuniverse/action_categories.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230526/policyuniverse/arn.py` & `policyuniverse-1.5.1.20230531/policyuniverse/arn.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230526/policyuniverse/common.py` & `policyuniverse-1.5.1.20230531/policyuniverse/common.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230526/policyuniverse/data.json` & `policyuniverse-1.5.1.20230531/policyuniverse/data.json`

 * *Files 0% similar despite different names*

```diff
@@ -54658,16 +54658,16 @@
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/deepracer/latest/developerguide/deepracer-choose-race-type.html"
         }
       }
     },
-    "arn_format": "arn:aws:deepracer:${Region}:${Account}:${ResourceType}/${ResourceName}",
-    "arn_regex": "^arn:aws:deepracer:.+",
+    "arn_format": "arn:${Partition}:deepracer:${Region}:${Account}:${ResourceType}/${ResourceName}",
+    "arn_regex": "^arn:${Partition}:deepracer:.+",
     "description": "AWS DeepRacer",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/deepracer/latest/developerguide/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/deepracer/latest/developerguide/what-is-deepracer.html",
       "authz_doc_page": "https://docs.aws.amazon.com/deepracer/latest/developerguide/deepracer-understand-required-permissions-and-iam-roles.html",
@@ -81146,15 +81146,15 @@
       "api_reference_doc_page": "https://docs.aws.amazon.com/scheduler/latest/APIReference/Welcome.html",
       "authz_doc_page": "https://docs.aws.amazon.com/scheduler/latest/UserGuide/security-iam.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/scheduler/latest/UserGuide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html"
     },
     "prefix": "scheduler"
   },
-  "EventBridgeSchemas": {
+  "EventBridge Schemas": {
     "actions": {
       "CreateDiscoverer": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
@@ -81587,23 +81587,23 @@
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/eventbridge/latest/schema-reference/v1-registries-name-registryname-schemas-name-schemaname.html#UpdateSchema"
         }
       }
     },
-    "arn_format": "arn:aws:schemas:${Region}:${Account}:${ResourceType}/${ResourceName}",
+    "arn_format": "arn:${Partition}:schemas:${Region}:${Account}:${ResourceType}/${ResourceName}",
     "arn_regex": "^arn:${Partition}:schemas:.+:.+:.+",
     "description": "Amazon EventBridge Schemas",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/eventbridge/latest/schema-reference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/eventbridge/latest/schema-reference/",
-      "authz_doc_page": "https://docs.aws.amazon.com/eventbridge/latest/userguide/auth-and-access-control-eventbridge.html",
+      "authz_doc_page": "https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-security.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/eventbridge/latest/userguide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/eventbridge/latest/userguide/"
     },
     "prefix": "schemas"
   },
   "ExecuteAPI": {
     "actions": {
@@ -100282,14 +100282,28 @@
         "description": "Grants permission to delete an existing attachment",
         "docs": {
           "api_doc": "",
           "doc_page": "https://aws.amazon.com/iq/",
           "doc_page_rel": "https://aws.amazon.com/iq/"
         }
       },
+      "DownloadAttachment": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to download existing attachment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "https://aws.amazon.com/iq/",
+          "doc_page_rel": "https://aws.amazon.com/iq/"
+        }
+      },
       "EndCall": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to end a voice/video call",
@@ -100463,14 +100477,28 @@
         "description": "Grants permission to read a proposal",
         "docs": {
           "api_doc": "",
           "doc_page": "https://aws.amazon.com/iq/",
           "doc_page_rel": "https://aws.amazon.com/iq/"
         }
       },
+      "GetRequest": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get a created request",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "https://aws.amazon.com/iq/",
+          "doc_page_rel": "https://aws.amazon.com/iq/"
+        }
+      },
       "GetReview": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -100503,14 +100531,29 @@
         "description": "Grants permission to start a voice/video call",
         "docs": {
           "api_doc": "",
           "doc_page": "https://aws.amazon.com/iq/",
           "doc_page_rel": "https://aws.amazon.com/iq/"
         }
       },
+      "ListAttachments": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list existing attachments",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "https://aws.amazon.com/iq/",
+          "doc_page_rel": "https://aws.amazon.com/iq/"
+        }
+      },
       "ListConversations": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -100791,17 +100834,17 @@
     "arn_regex": "^arn:${Partition}:iq:.+",
     "description": "AWS IQ",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/aws-iq/latest/user-guide/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/aws-iq/latest/user-guide/",
-      "authz_doc_page": "https://docs.aws.amazon.com/aws-iq/latest/user-guide/security.html",
+      "authz_doc_page": "https://docs.aws.amazon.com/aws-iq/latest/experts-user-guide/set-up-expert-account-permissions-to-use-aws-iq.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/aws-iq/",
-      "context_keys_doc_root": "https://docs.aws.amazon.com/aws-iq/latest/user-guide/"
+      "context_keys_doc_root": "https://docs.aws.amazon.com/aws-iq/latest/experts-user-guide/"
     },
     "prefix": "iq"
   },
   "IQ Permission": {
     "actions": {
       "ApproveAccessGrant": {
         "aws_action_groups": [
@@ -100910,21 +100953,21 @@
         }
       }
     },
     "arn_format": "arn:${Partition}:iq-permission:${Region}:${Account}:${ResourceType}/${ResourceName}",
     "arn_regex": "^arn:${Partition}:iq-permission:.+",
     "description": "AWS IQ Permissions",
     "docs": {
-      "actions_doc_root": "https://docs.aws.amazon.com/aws-iq/latest/user-guide/",
+      "actions_doc_root": "https://docs.aws.amazon.com/aws-iq/latest/experts-user-guide/",
       "api_detail_root": "",
       "api_doc_root": "",
-      "api_reference_doc_page": "https://docs.aws.amazon.com/aws-iq/latest/user-guide/",
-      "authz_doc_page": "https://docs.aws.amazon.com/aws-iq/latest/user-guide/security.html",
+      "api_reference_doc_page": "https://docs.aws.amazon.com/aws-iq/latest/experts-user-guide/",
+      "authz_doc_page": "https://docs.aws.amazon.com/aws-iq/latest/experts-user-guide/set-up-expert-account-permissions-to-use-aws-iq.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/aws-iq/",
-      "context_keys_doc_root": "https://docs.aws.amazon.com/aws-iq/latest/user-guide/"
+      "context_keys_doc_root": "https://docs.aws.amazon.com/aws-iq/latest/experts-user-guide/"
     },
     "prefix": "iq-permission"
   },
   "Identity Store": {
     "actions": {
       "CreateGroup": {
         "aws_action_groups": [
@@ -110471,15 +110514,16 @@
       "CreateCampaign": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
-          "aws:TagKeys"
+          "aws:TagKeys",
+          "iotfleetwise:DestinationArn"
         ],
         "description": "Grants permission to create a campaign",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/iot-fleetwise/latest/APIReference/API_CreateCampaign.html"
         }
@@ -160563,14 +160607,42 @@
         "description": "Grants permission to describe permissions for an analysis",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/APIReference/API_DescribeAnalysisPermissions.html"
         }
       },
+      "DescribeAssetBundleExportJob": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to describe an asset bundle export job",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/APIReference/API_DescribeAssetBundleExportJob.html"
+        }
+      },
+      "DescribeAssetBundleImportJob": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to describe an asset bundle import job",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/APIReference/API_DescribeAssetBundleImportJob.html"
+        }
+      },
       "DescribeCustomPermissions": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to describe a custom permissions resource in a QuickSight account",
@@ -161137,14 +161209,44 @@
         "description": "Grants permission to list all analyses in an account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/APIReference/API_ListAnalyses.html"
         }
       },
+      "ListAssetBundleExportJobs": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list all asset bundle export jobs",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/APIReference/API_ListAssetBundleExportJobs.html"
+        }
+      },
+      "ListAssetBundleImportJobs": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list all asset bundle import jobs",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/APIReference/API_ListAssetBundleImportJobs.html"
+        }
+      },
       "ListCustomPermissions": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to list custom permissions resources in QuickSight account",
@@ -161741,14 +161843,40 @@
         "description": "Grants permission to use Amazon QuickSight, in Enterprise edition, to display your Microsoft Active Directory directory groups so that you can choose which ones to map to roles in Amazon QuickSight",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}iam-actions.html",
           "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/user/iam-actions.html"
         }
       },
+      "StartAssetBundleExportJob": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start an asset bundle export job",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/APIReference/API_StartAssetBundleExportJob.html"
+        }
+      },
+      "StartAssetBundleImportJob": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start an asset bundle import job",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/APIReference/API_StartAssetBundleImportJob.html"
+        }
+      },
       "Subscribe": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "quicksight:DirectoryType",
@@ -191308,436 +191436,396 @@
     "actions": {
       "CreateAwsLogSource": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to enable any source type in any region for accounts that are either part of a trusted organization or standalone accounts",
+        "description": "Grants permission to enable any source type in any region for accounts that are either part of a trusted organization or standalone account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateAwsLogSource.html"
         }
       },
       "CreateCustomLogSource": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to add a custom source name",
+        "description": "Grants permission to add a custom source",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateCustomLogSource.html"
         }
       },
-      "CreateDatalake": {
+      "CreateDataLake": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to create a new Security Data Lake",
+        "description": "Grants permission to create a new security data lake",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateDatalake.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateDataLake.html"
         }
       },
-      "CreateDatalakeAutoEnable": {
+      "CreateDataLakeExceptionSubscription": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to add to the configuration for automatically enabling Amazon Security Lake access for new organization accounts",
+        "description": "Grants permission to get instant notifications about exceptions. Subscribes to the SNS topics for exception notifications",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateDatalakeAutoEnable.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateDataLakeExceptionSubscription.html"
         }
       },
-      "CreateDatalakeDelegatedAdmin": {
+      "CreateDataLakeOrganizationConfiguration": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to designate the Amazon Security Lake administrator account for the organization",
+        "description": "Grants permission to automatically enable Amazon Security Lake for new member accounts in your organization",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateDatalakeDelegatedAdmin.html"
-        }
-      },
-      "CreateDatalakeExceptionsSubscription": {
-        "aws_action_groups": [
-          "ReadWrite"
-        ],
-        "calculated_action_group": "Write",
-        "condition_keys": [],
-        "description": "Grants permission to get instant notifications about exceptions by subscribing to the SNS topics for exception notifications",
-        "docs": {
-          "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateDatalakeExceptionsSubscription.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateDataLakeOrganizationConfiguration.html"
         }
       },
       "CreateSubscriber": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to create a subscription permission for accounts that are already enabled",
+        "description": "Grants permission to create a subscriber",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateSubscriber.html"
         }
       },
-      "CreateSubscriptionNotificationConfiguration": {
+      "CreateSubscriberNotification": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to create a webhook invocation to notify a client when there is new data in the Data Lake",
+        "description": "Grants permission to create a webhook invocation to notify a client when there is new data in the data lake",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateSubscriptionNotificationConfiguration.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateSubscriberNotification.html"
         }
       },
       "DeleteAwsLogSource": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to disable any source type in any region for accounts that are either part of a trusted organization or standalone accounts",
+        "description": "Grants permission to disable any source type in any region for accounts that are part of a trusted organization or standalone accounts",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeleteAwsLogSource.html"
         }
       },
       "DeleteCustomLogSource": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to remove a custom source name",
+        "description": "Grants permission to remove a custom source",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeleteCustomLogSource.html"
         }
       },
-      "DeleteDatalake": {
+      "DeleteDataLake": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to delete all Security Data Lakes",
+        "description": "Grants permission to delete security data lake",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeleteDatalake.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeleteDataLake.html"
         }
       },
-      "DeleteDatalakeAutoEnable": {
+      "DeleteDataLakeExceptionSubscription": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to remove from the existing configuration the automatic enabling of Amazon Security Lake access for new organization accounts",
+        "description": "Grants permission to unsubscribe from SNS topics for exception notifications. Removes exception notifications for the SNS topic",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeleteDatalakeAutoEnable.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeleteDataLakeExceptionSubscription.html"
         }
       },
-      "DeleteDatalakeDelegatedAdmin": {
+      "DeleteDataLakeOrganizationConfiguration": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to remove the Delegated Administrator account and disable Amazon Security Lake as a service for this organization",
+        "description": "Grants permission to remove the automatic enablement of Amazon Security Lake access for new organization accounts",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeleteDatalakeDelegatedAdmin.html"
-        }
-      },
-      "DeleteDatalakeExceptionsSubscription": {
-        "aws_action_groups": [
-          "ReadWrite"
-        ],
-        "calculated_action_group": "Write",
-        "condition_keys": [],
-        "description": "Grants permission to unsubscribe from SNS topics for exception notifications. Also, removes the SNS exception notifications topic",
-        "docs": {
-          "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeleteDatalakeExceptionsSubscription.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeleteDataLakeOrganizationConfiguration.html"
         }
       },
       "DeleteSubscriber": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to delete the specified subscription permissions for accounts that are already enabled",
+        "description": "Grants permission to delete the specified subscriber",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeleteSubscriber.html"
         }
       },
-      "DeleteSubscriptionNotificationConfiguration": {
+      "DeleteSubscriberNotification": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to remove a webhook invocation to notify a client when there is new data in the Data Lake",
+        "description": "Grants permission to remove a webhook invocation to notify a client when there is new data in the data lake",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeleteSubscriptionNotificationConfiguration.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeleteSubscriberNotification.html"
         }
       },
-      "GetDatalake": {
+      "DeregisterDataLakeDelegatedAdministrator": {
         "aws_action_groups": [
-          "ReadOnly",
           "ReadWrite"
         ],
-        "calculated_action_group": "Read",
-        "condition_keys": [],
-        "description": "Grants permission to get information on the Security Data Lake",
-        "docs": {
-          "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_GetDatalake.html"
-        }
-      },
-      "GetDatalakeAutoEnable": {
-        "aws_action_groups": [
-          "ReadOnly",
-          "ReadWrite"
-        ],
-        "calculated_action_group": "Read",
+        "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to get an organization\ufffd\ufffd\ufffds configuration setting for the automatic enabling of Amazon Security Lake access for new organization accounts",
+        "description": "Grants permission to remove the Delegated Administrator account and disable Amazon Security Lake as a service for this organization",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_GetDatalakeAutoEnable.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_DeregisterDataLakeDelegatedAdministrator.html"
         }
       },
-      "GetDatalakeExceptionsExpiry": {
+      "GetDataLakeExceptionSubscription": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Grants permission to allow user to query what was set as the expiration period for the exception message",
+        "description": "Grants permission to query the protocol and endpoint that were provided when subscribing to SNS topics for exception notifications",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_GetDatalakeExceptionsExpiry.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_GetDataLakeExceptionSubscription.html"
         }
       },
-      "GetDatalakeExceptionsSubscription": {
+      "GetDataLakeOrganizationConfiguration": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Grants permission to query the protocol and endpoint that were supplied when subscribing to the SNS topics for exception notifications",
+        "description": "Grants permission to get an organization\ufffd\ufffd\ufffds configuration setting for automatically enabling Amazon Security Lake access for new organization accounts",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_GetDatalakeExceptionsSubscription.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_GetDataLakeOrganizationConfiguration.html"
         }
       },
-      "GetDatalakeStatus": {
+      "GetDataLakeSources": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Grants permission to get a static snapshot of the Security Data Lake in the current region, including enabled accounts and log sources",
+        "description": "Grants permission to get a static snapshot of the security data lake in the current region. The snapshot includes enabled accounts and log sources",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_GetDatalakeStatus.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_GetDataLakeSources.html"
         }
       },
       "GetSubscriber": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Grants permission to get subscription information for a subscription permission for accounts that are already enabled",
+        "description": "Grants permission to get information about subscriber that is already created",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_GetSubscriber.html"
         }
       },
-      "GetSubscriptionNotificationConfiguration": {
+      "ListDataLakeExceptions": {
         "aws_action_groups": [
+          "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
-        "calculated_action_group": "Read",
+        "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Grants permission to get information for a webhook invocation to notify a client when there is new data in the Data Lake",
+        "description": "Grants permission to get the list of all non-retryable failures",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_GetSubscriptionNotificationConfiguration.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_ListDataLakeExceptions.html"
         }
       },
-      "ListDatalakeExceptions": {
+      "ListDataLakes": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Grants permission to get the list of all non-retry-able failures",
+        "description": "Grants permission to list information about the security data lakes",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_ListDatalakeExceptions.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_ListDataLakes.html"
         }
       },
       "ListLogSources": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Grants permission to show the estate view of enabled accounts with the enabled sources in the enabled regions",
+        "description": "Grants permission to view the enabled accounts. You can view the enabled sources in the enabled regions",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_ListLogSources.html"
         }
       },
       "ListSubscribers": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Grants permission to list all subscription permissions for accounts that are already enabled",
+        "description": "Grants permission to list all subscribers",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_ListSubscribers.html"
         }
       },
-      "UpdateDatalake": {
+      "RegisterDataLakeDelegatedAdministrator": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to update a Security Data Lake",
+        "description": "Grants permission to designate an account as the Amazon Security Lake administrator account for the organization",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_UpdateDatalake.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_RegisterDataLakeDelegatedAdministrator.html"
         }
       },
-      "UpdateDatalakeExceptionsExpiry": {
+      "UpdateDataLake": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to control the time-to-live (TTL) for the exception message to remain in service cache",
+        "description": "Grants permission to update a security data lake",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_UpdateDatalakeExceptionsExpiry.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_UpdateDataLake.html"
         }
       },
-      "UpdateDatalakeExceptionsSubscription": {
+      "UpdateDataLakeExceptionSubscription": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update subscriptions to the SNS topics for exception notifications",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_UpdateDatalakeExceptionsSubscription.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_UpdateDataLakeExceptionSubscription.html"
         }
       },
       "UpdateSubscriber": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to update subscription information for a subscription permission for accounts that are already enabled",
+        "description": "Grants permission to update subscriber",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_UpdateSubscriber.html"
         }
       },
-      "UpdateSubscriptionNotificationConfiguration": {
+      "UpdateSubscriberNotification": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to update a webhook invocation to notify a client when there is new data in the Data Lake",
+        "description": "Grants permission to update a webhook invocation to notify a client when there is new data in the data lake",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_UpdateSubscriptionNotificationConfiguration.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_UpdateSubscriberNotification.html"
         }
       }
     },
-    "arn_format": "",
-    "arn_regex": "",
+    "arn_format": "arn:${Partition}:securitylake:${Region}:${Account}:${ResourceType}/${ResourcePath}",
+    "arn_regex": "^arn:${Partition}:securitylake:.+:.+:.+",
     "description": "Amazon Security Lake",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/security-lake/latest/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/security-lake/latest/APIReference/",
-      "authz_doc_page": "https://docs.aws.amazon.com/security-lake/latest/userguide/access_policies.html",
-      "concepts_doc_root": "https://docs.aws.amazon.com/security-lake/latest/userguide/",
-      "context_keys_doc_root": "https://docs.aws.amazon.com/IAM/latest/UserGuide/"
+      "authz_doc_page": "https://docs.aws.amazon.com/AmazonSecurityLake/latest/access_policies.html",
+      "concepts_doc_root": "https://docs.aws.amazon.com/AmazonSecurityLake/latest/",
+      "context_keys_doc_root": "https://docs.aws.amazon.com/AmazonSecurityLake/latest/"
     },
     "prefix": "securitylake"
   },
   "ServerMigrationService": {
     "actions": {
       "CreateApp": {
         "aws_action_groups": [
```

### Comparing `policyuniverse-1.5.1.20230526/policyuniverse/expander_minimizer.py` & `policyuniverse-1.5.1.20230531/policyuniverse/expander_minimizer.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230526/policyuniverse/organization.py` & `policyuniverse-1.5.1.20230531/policyuniverse/organization.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230526/policyuniverse/policy.py` & `policyuniverse-1.5.1.20230531/policyuniverse/policy.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230526/policyuniverse/statement.py` & `policyuniverse-1.5.1.20230531/policyuniverse/statement.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230526/policyuniverse.egg-info/PKG-INFO` & `policyuniverse-1.5.1.20230531/policyuniverse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyuniverse
-Version: 1.5.1.20230526
+Version: 1.5.1.20230531
 Summary: Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.
 Home-page: https://github.com/Netflix-Skunkworks/policyuniverse
 Author: Patrick Kelley
 Author-email: patrickbarrettkelley@gmail.com
 Keywords: iam,arn,action_groups,condition,policy,statement,wildcard
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
```

### Comparing `policyuniverse-1.5.1.20230526/policyuniverse.egg-info/SOURCES.txt` & `policyuniverse-1.5.1.20230531/policyuniverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230526/setup.py` & `policyuniverse-1.5.1.20230531/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ROOT = os.path.realpath(os.path.join(os.path.dirname(__file__)))
 
 tests_require = ["pytest", "coveralls", "bandit"]
 dev_require = ["pre-commit", "black"]
 
 setup(
     name="policyuniverse",
-    version="1.5.1.20230526",
+    version="1.5.1.20230531",
     description="Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.",
     long_description=open(os.path.join(ROOT, "README.md")).read(),
     long_description_content_type="text/markdown",
     author="Patrick Kelley",
     author_email="patrickbarrettkelley@gmail.com",
     url="https://github.com/Netflix-Skunkworks/policyuniverse",
     keywords=[
```

