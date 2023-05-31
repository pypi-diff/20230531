# Comparing `tmp/OBP_devops-0.0.2.tar.gz` & `tmp/OBP_devops-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_devops-0.0.2.tar", last modified: Fri Jan 27 07:01:26 2023, max compression
+gzip compressed data, was "OBP_devops-0.1.0.tar", last modified: Wed May 31 12:35:06 2023, max compression
```

## Comparing `OBP_devops-0.0.2.tar` & `OBP_devops-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-01-27 07:01:26.615946 OBP_devops-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-01-27 07:01:26.584685 OBP_devops-0.0.2/OBP_devops/
--rw-rw-rw-   0        0        0     7041 2023-01-27 07:00:54.000000 OBP_devops-0.0.2/OBP_devops/__init__.py
--rw-rw-rw-   0        0        0     2600 2023-01-27 06:22:26.000000 OBP_devops-0.0.2/OBP_devops/cloudformation.py
--rw-rw-rw-   0        0        0     9072 2023-01-27 06:22:26.000000 OBP_devops-0.0.2/OBP_devops/codebuild.py
--rw-rw-rw-   0        0        0     2630 2023-01-27 06:22:26.000000 OBP_devops-0.0.2/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py
--rw-rw-rw-   0        0        0     2993 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py
--rw-rw-rw-   0        0        0     2457 2023-01-27 06:57:47.000000 OBP_devops-0.0.2/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py
--rw-rw-rw-   0        0        0     2365 2023-01-27 05:16:17.000000 OBP_devops-0.0.2/OBP_devops/codepipeline.py
--rw-rw-rw-   0        0        0     4336 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/ecr.py
--rw-rw-rw-   0        0        0     1883 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/ecr_private_tag_immutability_enabled.py
--rw-rw-rw-   0        0        0     1826 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/ecs_container_insights_enabled.py
--rw-rw-rw-   0        0        0     2158 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/ecs_containers_non_privileged.py
--rw-rw-rw-   0        0        0     2232 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/ecs_containers_read_only_access.py
--rw-rw-rw-   0        0        0     2035 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/ecs_fargate_latest_platform_version.py
--rw-rw-rw-   0        0        0     2175 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/ecs_task_definition_memory_hard_limit.py
--rw-rw-rw-   0        0        0     2302 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/ecs_task_definition_nonroot_user.py
--rw-rw-rw-   0        0        0     2169 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/ecs_task_definition_pid_mode_check.py
--rw-rw-rw-   0        0        0     2376 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/ecs_task_definition_user_for_host_mode_check.py
--rw-rw-rw-   0        0        0     4711 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/eks.py
--rw-rw-rw-   0        0        0     3314 2023-01-27 06:22:27.000000 OBP_devops-0.0.2/OBP_devops/elastic_beanstalk.py
--rw-rw-rw-   0        0        0     5941 2023-01-27 05:16:17.000000 OBP_devops-0.0.2/OBP_devops/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-27 07:01:26.600308 OBP_devops-0.0.2/OBP_devops.egg-info/
--rw-rw-rw-   0        0        0      369 2023-01-27 07:01:26.000000 OBP_devops-0.0.2/OBP_devops.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      976 2023-01-27 07:01:26.000000 OBP_devops-0.0.2/OBP_devops.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-27 07:01:26.000000 OBP_devops-0.0.2/OBP_devops.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-01-27 07:01:26.000000 OBP_devops-0.0.2/OBP_devops.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      369 2023-01-27 07:01:26.615946 OBP_devops-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_devops-0.0.2/README.md
--rw-rw-rw-   0        0        0      550 2023-01-27 06:59:16.000000 OBP_devops-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-27 07:01:26.615946 OBP_devops-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:06.479433 OBP_devops-0.1.0/
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:06.463791 OBP_devops-0.1.0/OBP_devops/
+-rw-rw-rw-   0        0        0     7180 2023-05-31 12:31:35.000000 OBP_devops-0.1.0/OBP_devops/__init__.py
+-rw-rw-rw-   0        0        0     2600 2023-01-27 06:22:26.000000 OBP_devops-0.1.0/OBP_devops/cloudformation.py
+-rw-rw-rw-   0        0        0     9072 2023-01-27 06:22:26.000000 OBP_devops-0.1.0/OBP_devops/codebuild.py
+-rw-rw-rw-   0        0        0     2632 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py
+-rw-rw-rw-   0        0        0     3016 2023-05-31 12:31:35.000000 OBP_devops-0.1.0/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py
+-rw-rw-rw-   0        0        0     2480 2023-05-31 12:31:35.000000 OBP_devops-0.1.0/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py
+-rw-rw-rw-   0        0        0     2365 2023-01-27 05:16:17.000000 OBP_devops-0.1.0/OBP_devops/codepipeline.py
+-rw-rw-rw-   0        0        0     4336 2023-01-27 06:22:27.000000 OBP_devops-0.1.0/OBP_devops/ecr.py
+-rw-rw-rw-   0        0        0     1906 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/ecr_private_tag_immutability_enabled.py
+-rw-rw-rw-   0        0        0     1849 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/ecs_container_insights_enabled.py
+-rw-rw-rw-   0        0        0     1861 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/ecs_containers_non_privileged.py
+-rw-rw-rw-   0        0        0     1935 2023-05-31 12:31:35.000000 OBP_devops-0.1.0/OBP_devops/ecs_containers_read_only_access.py
+-rw-rw-rw-   0        0        0     2058 2023-05-31 12:31:35.000000 OBP_devops-0.1.0/OBP_devops/ecs_fargate_latest_platform_version.py
+-rw-rw-rw-   0        0        0     1886 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/ecs_task_definition_memory_hard_limit.py
+-rw-rw-rw-   0        0        0     1995 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/ecs_task_definition_nonroot_user.py
+-rw-rw-rw-   0        0        0     1892 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/ecs_task_definition_pid_mode_check.py
+-rw-rw-rw-   0        0        0     2091 2023-05-31 12:31:35.000000 OBP_devops-0.1.0/OBP_devops/ecs_task_definition_user_for_host_mode_check.py
+-rw-rw-rw-   0        0        0     4711 2023-01-27 06:22:27.000000 OBP_devops-0.1.0/OBP_devops/eks.py
+-rw-rw-rw-   0        0        0     3326 2023-01-30 07:27:29.000000 OBP_devops-0.1.0/OBP_devops/elastic_beanstalk.py
+-rw-rw-rw-   0        0        0     6477 2023-05-31 12:13:47.000000 OBP_devops-0.1.0/OBP_devops/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:06.479433 OBP_devops-0.1.0/OBP_devops.egg-info/
+-rw-rw-rw-   0        0        0      369 2023-05-31 12:35:06.000000 OBP_devops-0.1.0/OBP_devops.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2023-05-31 12:35:06.000000 OBP_devops-0.1.0/OBP_devops.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 12:35:06.000000 OBP_devops-0.1.0/OBP_devops.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 12:35:06.000000 OBP_devops-0.1.0/OBP_devops.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      369 2023-05-31 12:35:06.479433 OBP_devops-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_devops-0.1.0/README.md
+-rw-rw-rw-   0        0        0      550 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 12:35:06.479433 OBP_devops-0.1.0/setup.cfg
```

### Comparing `OBP_devops-0.0.2/OBP_devops/__init__.py` & `OBP_devops-0.1.0/OBP_devops/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 
 from botocore.exceptions import ClientError
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Klera DevOps'
-__version__ = '0.0.2'
+__version__ = '0.1.0'
 
 
 class aws_client:
     def __init__(self, **kwargs):
         if 'aws_access_key_id' in kwargs.keys() and 'aws_secret_access_key' in kwargs.keys():
             self.session = session.Session(
                 aws_access_key_id=kwargs['aws_access_key_id'],
                 aws_secret_access_key=kwargs['aws_secret_access_key'],
             )
         elif 'profile_name' in kwargs.keys():
             self.session = session.Session(profile_name=kwargs['profile_name'])
 
     from .utils import get_regions, list_elastic_beanstalk_envs, list_eks_clusters, list_ecr_repositories, \
-        list_codebuild_projects, list_code_pipelines
+        list_codebuild_projects, list_code_pipelines, list_task_definitions
     from .elastic_beanstalk import enhanced_health_reporting_enabled, managed_updates_enabled
     from .cloudformation import stack_notification_check
     from .eks import eks_secrets_encrypted, eks_endpoint_no_public_access
     from .ecr import ecr_private_image_scanning_enabled, ecr_private_lifecycle_policy_configured
     from .codebuild import project_artifact_encryption_enabled, project_environment_privileged_check, \
         project_logging_enabled, project_s3_logs_encrypted
     from .codepipeline import codepipeline_deployment_count_check
@@ -45,32 +45,32 @@
     def get_compliance(self) -> list:
         """
         :return:
         """
         regions = self.get_regions()
         eb_envs = self.list_elastic_beanstalk_envs(regions=regions)
         # print("eb envs" + str(eb_envs))
+        task_definitions = self.list_task_definitions(regions)
 
         compliance = [
             # self.enhanced_health_reporting_enabled(eb_envs),
             self.managed_updates_enabled(environments=eb_envs),
             self.stack_notification_check(regions),
             self.ecr_private_tag_immutability_enabled(regions),
             self.ecs_container_insights_enabled(regions),
-            self.ecs_containers_non_privileged(regions),
-            self.ecs_containers_read_only_access(regions),
-            self.ecs_task_definition_nonroot_user(regions),
-            self.ecs_task_definition_pid_mode_check(regions),
-            self.ecs_task_definition_user_for_host_mode_check(regions),
-            self.ecs_task_definition_memory_hard_limit(regions),
+            self.ecs_containers_non_privileged(task_definitions),
+            self.ecs_containers_read_only_access(task_definitions),
+            self.ecs_task_definition_nonroot_user(task_definitions),
+            self.ecs_task_definition_pid_mode_check(task_definitions),
+            self.ecs_task_definition_user_for_host_mode_check(task_definitions),
+            self.ecs_task_definition_memory_hard_limit(task_definitions),
             self.ecs_fargate_latest_platform_version(regions),
             self.codedeploy_auto_rollback_monitor_enabled(regions),
             self.codedeploy_ec2_minimum_healthy_hosts_configured(regions),
             self.codedeploy_lambda_allatonce_traffic_shift_disabled(regions)
-
         ]
 
         # calling the compliance methods for eks
         try:
             eks_clusters = self.list_eks_clusters(regions)
             # print("eks clusters" + str(eks_clusters))
         except ClientError as e:
```

### Comparing `OBP_devops-0.0.2/OBP_devops/cloudformation.py` & `OBP_devops-0.1.0/OBP_devops/cloudformation.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.0.2/OBP_devops/codebuild.py` & `OBP_devops-0.1.0/OBP_devops/codebuild.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.0.2/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py` & `OBP_devops-0.1.0/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     control_id = 'Id44.3'
     compliance_type = "codedeploy_auto_rollback_monitor_enabled"
     description = "Checks if the deployment group is configured with automatic deployment rollback and deployment " \
                   "monitoring with alarms attached."
     resource_type = "AWS ECS"
     risk_level = 'High'
 
-    regions = self.session.get_available_regions('codedeploy')
+    # regions = self.session.get_available_regions('codedeploy')
 
     for region in regions:
         try:
             client = self.session.client('codedeploy', region_name=region)
 
             applications = client.list_applications()['applications']
             for application in applications:
```

### Comparing `OBP_devops-0.0.2/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py` & `OBP_devops-0.1.0/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 def codedeploy_ec2_minimum_healthy_hosts_configured(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: codedeploy_ec2_minimum_healthy_hosts_configured()")
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id44.4'
     compliance_type = "codedeploy_ec2_minimum_healthy_hosts_configured"
     description = "Checks if the deployment group for EC2/On-Premises Compute Platform is configured with a minimum healthy hosts fleet percentage or host count is greater than or equal to the input threshold. Default:: (minimumHealthyHostsFleetPercent=66) and (minimumHealthyHostsHostCount=1)"
     resource_type = "AWS CodeDeploy"
     risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('codedeploy')
+    # regions = self.session.get_available_regions('codedeploy')
 
     for region in regions:
         try:
             client = self.session.client('codedeploy', region_name=region)
             default_minimumHealthyHostsHostCount = 1
             default_minimumHealthyHostsFleetPercent = 66
```

### Comparing `OBP_devops-0.0.2/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py` & `OBP_devops-0.1.0/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 def codedeploy_lambda_allatonce_traffic_shift_disabled(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: codedeploy_lambda_allatonce_traffic_shift_disabled()")
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id44.5'
     compliance_type = "codedeploy_lambda_allatonce_traffic_shift_disabled"
     description = "Checks if the deployment group for Lambda Compute Platform is not using the default deployment configuration."
     resource_type = "AWS CodeDeploy"
     risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('codedeploy')
+    # regions = self.session.get_available_regions('codedeploy')
 
     for region in regions:
         try:
             client = self.session.client('codedeploy', region_name=region)
 
             applications = client.list_applications()['applications']
             for application in applications:
```

### Comparing `OBP_devops-0.0.2/OBP_devops/codepipeline.py` & `OBP_devops-0.1.0/OBP_devops/codepipeline.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.0.2/OBP_devops/ecr.py` & `OBP_devops-0.1.0/OBP_devops/ecr.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.0.2/OBP_devops/ecr_private_tag_immutability_enabled.py` & `OBP_devops-0.1.0/OBP_devops/ecr_private_tag_immutability_enabled.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 def ecr_private_tag_immutability_enabled(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecr_private_tag_immutability_enabled()")
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id44.9'
     compliance_type = "ecr_private_tag_immutability_enabled"
     description = "Checks if a private Amazon Elastic Container Registry (ECR) repository has tag immutability enabled."
     resource_type = "AWS ECR"
     risk_level = 'High'
 
-    regions = self.session.get_available_regions('ecr')
+    # regions = self.session.get_available_regions('ecr')
 
     for region in regions:
         try:
             client = self.session.client('ecr', region_name=region)
 
             resp = client.describe_repositories()
             repositories = resp['repositories']
```

### Comparing `OBP_devops-0.0.2/OBP_devops/ecs_container_insights_enabled.py` & `OBP_devops-0.1.0/OBP_devops/ecs_container_insights_enabled.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 def ecs_container_insights_enabled(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_container_insights_enabled()")
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.1'
     compliance_type = "ecs_container_insights_enabled"
     description = "Checks if Amazon Elastic Container Service clusters have container insights enabled."
     resource_type = "AWS ECS"
     risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('ecs')
+    # regions = self.session.get_available_regions('ecs')
 
     for region in regions:
         try:
             client = self.session.client('ecs', region_name=region)
 
             resp = client.describe_clusters()
             clusters = resp['clusters']
```

### Comparing `OBP_devops-0.0.2/OBP_devops/ecs_containers_non_privileged.py` & `OBP_devops-0.1.0/OBP_devops/ecs_containers_non_privileged.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,54 +4,49 @@
 
 from OBP_devops.utils import get_regions
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def ecs_containers_non_privileged(self, regions) -> dict:
+def ecs_containers_non_privileged(self, task_definitions) -> dict:
     """
+    :param task_definitions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_containers_non_privileged()")
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.2'
     compliance_type = "ecs_containers_non_privileged"
     description = "Checks if the privileged parameter in the container definition of ECSTaskDefinitions is set to ‘true’. "
     resource_type = "AWS ECS TaskDefinition"
     risk_level = 'High'
 
-    regions = self.session.get_available_regions('ecs')
+    # regions = self.session.get_available_regions('ecs')
+
+    for region, definitions in task_definitions.items():
+        for task_definition in definitions:
+            resp = client.describe_task_definition(taskDefinition=task_definition)
+            container_definitions = resp['taskDefinition']['containerDefinitions']
+            for definition in container_definitions:
+
+                try:
+                    if definition['privileged'] == 'False':
+                        raise KeyError
+
+                except KeyError:
+                    result = False
+                    offenders.append(definition['name'])
+                    failReason = "The privileged parameter in the container definition of ECSTaskDefinitions is set to False"
+                    continue
 
-    for region in regions:
-        try:
-            client = self.session.client('ecs', region_name=region)
-            task_definitions = client.list_task_definitions()['taskDefinitionArns']
-            for task_definition in task_definitions:
-                resp = client.describe_task_definition(taskDefinition=task_definition)
-                container_definitions = resp['taskDefinition']['containerDefinitions']
-                for definition in container_definitions:
-
-                    try:
-                        if definition['privileged'] == 'False':
-                            raise KeyError
-
-                    except KeyError:
-                        result = False
-                        offenders.append(definition['name'])
-                        failReason = "The privileged parameter in the container definition of ECSTaskDefinitions is set to False"
-                        continue
-        
-        except ClientError as e:
-            logger.error("Something went wrong with the region {}: {}".format(region, e))
-            
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
         'Description': description,
```

### Comparing `OBP_devops-0.0.2/OBP_devops/ecs_containers_read_only_access.py` & `OBP_devops-0.1.0/OBP_devops/ecs_containers_read_only_access.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 from OBP_devops.utils import get_regions
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def ecs_containers_read_only_access(self, regions) -> dict:
+def ecs_containers_read_only_access(self, task_definitions) -> dict:
     """
+    :param task_definitions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_containers_read_only_access()")
 
     result = True
     failReason = ''
@@ -21,38 +22,32 @@
     control_id = 'Id7.3'
     compliance_type = "ecs_containers_read_only_access"
     description = "Checks if Amazon Elastic Container Service (Amazon ECS) Containers only have read-only access to " \
                   "its root filesystems. ."
     resource_type = "AWS ECS TaskDefinition"
     risk_level = 'High'
 
-    regions = self.session.get_available_regions('ecs')
+    # regions = self.session.get_available_regions('ecs')
+
+    for region, definitions in task_definitions.items():
+        for task_definition in definitions:
+            resp = client.describe_task_definition(taskDefinition=task_definition)
+            container_definitions = resp['taskDefinition']['containerDefinitions']
+            for definition in container_definitions:
+
+                try:
+                    if definition['readonlyRootFilesystem'] == 'False':
+                        raise KeyError
+
+                except KeyError:
+                    result = False
+                    offenders.append(definition['name'])
+                    failReason = "The readonlyRootFilesystem parameter in the container definition of ECSTaskDefinitions is set to ‘false’."
+                    continue
 
-    for region in regions:
-        try:
-            client = self.session.client('ecs', region_name=region)
-            task_definitions = client.list_task_definitions()['taskDefinitionArns']
-            for task_definition in task_definitions:
-                resp = client.describe_task_definition(taskDefinition=task_definition)
-                container_definitions = resp['taskDefinition']['containerDefinitions']
-                for definition in container_definitions:
-
-                    try:
-                        if definition['readonlyRootFilesystem'] == 'False':
-                            raise KeyError
-
-                    except KeyError:
-                        result = False
-                        offenders.append(definition['name'])
-                        failReason = "The readonlyRootFilesystem parameter in the container definition of ECSTaskDefinitions is set to ‘false’."
-                        continue
-        
-        except ClientError as e:
-            logger.error("Something went wrong with the region {}: {}".format(region, e))
-            
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
         'Description': description,
```

### Comparing `OBP_devops-0.0.2/OBP_devops/ecs_fargate_latest_platform_version.py` & `OBP_devops-0.1.0/OBP_devops/ecs_fargate_latest_platform_version.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 def ecs_fargate_latest_platform_version(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_fargate_latest_platform_version()")
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.4'
     compliance_type = "ecs_fargate_latest_platform_version"
     description = "Checks if Amazon Elastic Container Service (ECS) Fargate Services is running on the latest Fargate platform version."
     resource_type = "AWS ECS"
     risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('ecs')
+    # regions = self.session.get_available_regions('ecs')
 
     for region in regions:
         try:
             client = self.session.client('ecs', region_name=region)
             services = client.list_services()['serviceArns']
             for service in services:
                 resp = client.describe_services(services=[service])
```

### Comparing `OBP_devops-0.0.2/OBP_devops/ecs_task_definition_memory_hard_limit.py` & `OBP_devops-0.1.0/OBP_devops/ecs_task_definition_user_for_host_mode_check.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,58 +4,54 @@
 
 from OBP_devops.utils import get_regions
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def ecs_task_definition_memory_hard_limit(self, regions) -> dict:
+def ecs_task_definition_user_for_host_mode_check(self, task_definitions) -> dict:
     """
+    :param task_definitions:
     :param self:
     :return:
     """
-    logger.info(" ---Inside OBP DevOps :: ecs_task_definition_memory_hard_limit()")
+    logger.info(" ---Inside OBP DevOps :: ecs_task_definition_user_for_host_mode_check()")
 
     result = True
     failReason = ''
     offenders = []
-    control_id = 'Id7.6'
-    compliance_type = "ecs_task_definition_memory_hard_limit"
-    description = "Checks if ECS task definitions have a set memory limit for its container definitions. "
+    control_id = 'Id3.38'
+    compliance_type = "ecs_task_definition_user_for_host_mode_check"
+    description = "Checks if an Amazon ECS task definition with host networking mode has 'privileged' or 'user' container definitions. . "
     resource_type = "AWS ECS TaskDefinition"
     risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('ecs')
+    # regions = self.session.get_available_regions('ecs')
 
-    for region in regions:
-        try:
-            client = self.session.client('ecs', region_name=region)
-            task_definitions = client.list_task_definitions()['taskDefinitionArns']
-            for task_definition in task_definitions:
-                resp = client.describe_task_definition(taskDefinition=task_definition)
-                container_definitions = resp['taskDefinition']['containerDefinitions']
-                for definition in container_definitions:
+    for region, definitions in task_definitions.items():
+        for task_definition in definitions:
+
+            try:
 
-                    try:
-                        # print(definition)
-                        if 'memory' not in definition:
+                resp = client.describe_task_definition(taskDefinition=task_definition)
+                if resp['taskDefinition']['networkMode'] == 'host':
+                    for containerdefintion in resp['taskDefinition']['containerDefinitions']:
+                        if containerdefintion['privileged'] == 'False' or '' and containerdefintion['user'] == 'root' or '':
                             raise KeyError
 
-                    except KeyError:
-                        result = False
-                        offenders.append(definition['name'])
-                        failReason = "The ‘memory’ parameter is absent for one container definition."
-                        continue
-        
-        except ClientError as e:
-            logger.error("Something went wrong with the region {}: {}".format(region, e))
+
+            except KeyError:
+                    result = False
+                    offenders.append(resp['taskDefinition']['taskDefinitionArn'])
+                    failReason = "There are ECSTaskDefinitions with host network mode and container definitions of privileged=false or empty and user=root or empty.."
+                    continue
             
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
         'Description': description,
         'Risk Level': risk_level,
         'ControlId': control_id
-    }
+    }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `OBP_devops-0.0.2/OBP_devops/ecs_task_definition_nonroot_user.py` & `OBP_devops-0.1.0/OBP_devops/ecs_task_definition_nonroot_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,60 +4,53 @@
 
 from OBP_devops.utils import get_regions
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def ecs_task_definition_nonroot_user(self, regions) -> dict:
+def ecs_task_definition_nonroot_user(self, task_definitions) -> dict:
     """
+    :param task_definitions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_taskdefinition_nonroot_user()")
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.7'
     compliance_type = "ecs_task_definition_nonroot_user"
     description = "Checks if Amazon Elastic Container Service (Amazon ECS) Containers only have read-only access to its root filesystems. . "
     resource_type = "AWS ECS TaskDefinition"
     risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('ecs')
+    # regions = self.session.get_available_regions('ecs')
+
+    for region, definitions in task_definitions.items():
+        for task_definition in definitions:
+            resp = client.describe_task_definition(taskDefinition=task_definition)
+            container_definitions = resp['taskDefinition']['containerDefinitions']
+            for definition in container_definitions:
+                try:
+                    if 'user' not in definition:
+                        raise KeyError
+                    if definition['user'] == 'root' or definition['user'] == '':
+                        raise KeyError
+
+                except KeyError:
+                    result = False
+                    offenders.append(definition['name'])
+                    failReason = "ECSTaskDefinitions doesn't specify a non root user for EC2 launch type containers to run on"
+                    continue
 
-    for region in regions:
-        try:
-            client = self.session.client('ecs', region_name=region)
-            task_definitions = client.list_task_definitions()['taskDefinitionArns']
-            for task_definition in task_definitions:
-                resp = client.describe_task_definition(taskDefinition=task_definition)
-                container_definitions = resp['taskDefinition']['containerDefinitions']
-                for definition in container_definitions:
-
-                    try:
-
-                        if 'user' not in definition:
-                            raise KeyError
-                        if definition['user'] == 'root' or definition['user'] == '':
-                            raise KeyError
-
-                    except KeyError:
-                        result = False
-                        offenders.append(definition['name'])
-                        failReason = "ECSTaskDefinitions doesn't specify a non root user for EC2 launch type containers to run on"
-                        continue
-        
-        except ClientError as e:
-            logger.error("Something went wrong with the region {}: {}".format(region, e))
-            
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
         'Description': description,
         'Risk Level': risk_level,
         'ControlId': control_id
-    }
+    }
```

### Comparing `OBP_devops-0.0.2/OBP_devops/ecs_task_definition_pid_mode_check.py` & `OBP_devops-0.1.0/OBP_devops/ecs_task_definition_pid_mode_check.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 from OBP_devops.utils import get_regions
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def ecs_task_definition_pid_mode_check(self, regions) -> dict:
+def ecs_task_definition_pid_mode_check(self, task_definitions) -> dict:
     """
+    :param task_definitions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_task_definition_pid_mode_check()")
 
     result = True
     failReason = ''
@@ -22,36 +23,30 @@
     control_id = 'Id7.8'
     compliance_type = "ecs_task_definition_pid_mode_check"
     description = "Checks if ECSTaskDefinitions are configured to share a host’s process namespace with its Amazon " \
                   "Elastic Container Service (Amazon ECS) containers."
     resource_type = "AWS ECS TaskDefinition"
     risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('ecs')
+    # regions = self.session.get_available_regions('ecs')
 
-    for region in regions:
-        try:
-            client = self.session.client('ecs', region_name=region)
-            task_definitions = client.list_task_definitions()['taskDefinitionArns']
-            for task_definition in task_definitions:
-
-                try:
-
-                    resp = client.describe_task_definition(taskDefinition=task_definition)
-                    if resp['taskDefinition']['pidMode'] == 'host':
-                        raise KeyError
-
-                except KeyError:
-                        result = False
-                        offenders.append(resp['taskDefinition']['taskDefinitionArn'])
-                        failReason = "ECSTaskDefinitions are not configured to share a host’s process namespace with its ECS containers as pidMode parameter is set to ‘host’."
-                        continue
-        
-        except ClientError as e:
-            logger.error("Something went wrong with the region {}: {}".format(region, e))
+    for region, definitions in task_definitions.items():
+        for task_definition in definitions:
+
+            try:
+
+                resp = client.describe_task_definition(taskDefinition=task_definition)
+                if resp['taskDefinition']['pidMode'] == 'host':
+                    raise KeyError
+
+            except KeyError:
+                    result = False
+                    offenders.append(resp['taskDefinition']['taskDefinitionArn'])
+                    failReason = "ECSTaskDefinitions are not configured to share a host’s process namespace with its ECS containers as pidMode parameter is set to ‘host’."
+                    continue
             
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
```

### Comparing `OBP_devops-0.0.2/OBP_devops/eks.py` & `OBP_devops-0.1.0/OBP_devops/eks.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.0.2/OBP_devops/elastic_beanstalk.py` & `OBP_devops-0.1.0/OBP_devops/elastic_beanstalk.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     :return:
     """
     logger.info(" ---Inside elastic_beanstalk :: enhanced_health_reporting_enabled()")
 
     result = True
     failReason = ''
     offenders = []
-    control_id = ''
+    control_id = 'Id3.13'
     compliance_type = "Beanstalk Enhanced Health Reporting Enabled"
     description = "Checks if an AWS Elastic Beanstalk environment is configured for enhanced health reporting. The " \
                   "rule is COMPLIANT if the environment is configured for enhanced health reporting."
     resource_type = "Elastic Beanstalk"
     risk_level = 'Medium'
 
     for region, envs in environments.items():
@@ -52,15 +52,15 @@
     :return:
     """
     logger.info(" ---Inside elastic_beanstalk :: managed_updates_enabled()---")
 
     result = True
     failReason = ''
     offenders = []
-    control_id = ''
+    control_id = 'Id3.41'
     compliance_type = 'Elastic Beanstalk managed updates enabled'
     description = 'Checks if managed platform updates in an AWS Elastic Beanstalk environment is enabled'
     resource_type = 'Elastic Beanstalk'
     risk_level = 'Medium'
 
     for region, envs in environments.items():
         client = self.session.client('elasticbeanstalk', region_name=region)
```

### Comparing `OBP_devops-0.0.2/OBP_devops/utils.py` & `OBP_devops-0.1.0/OBP_devops/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -198,7 +198,27 @@
                         break
                 except KeyError:
                     break
         except EndpointConnectionError as e:
             pass
 
     return pipelines
+
+
+# returns the list of task definitions
+def list_task_definitions(self, regions: list) -> dict:
+    """
+    :param self:
+    :param regions:
+    :return:
+    """
+    logger.info(" ---Inside utils :: list_task_definitions()--- ")
+
+    task_definitions = {}
+
+    for region in regions:
+        client = self.session.client('ecs', region_name=region)
+        response = client.list_task_definitions()
+
+        task_definitions.setdefault(region, []).extend(response['taskDefinitionArns'])
+
+    return task_definitions
```

### Comparing `OBP_devops-0.0.2/OBP_devops.egg-info/SOURCES.txt` & `OBP_devops-0.1.0/OBP_devops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.0.2/pyproject.toml` & `OBP_devops-0.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "OBP_devops"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="dheeraj.banodha", email="dheeraj.banodha@impetus.com" },
   { name="ravish.sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
```

