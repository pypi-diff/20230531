# Comparing `tmp/ibm-cos-sdk-core-2.8.0.tar.gz` & `tmp/ibm-cos-sdk-core-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ibm-cos-sdk-core-2.8.0.tar", last modified: Tue Oct 27 20:35:24 2020, max compression
+gzip compressed data, was "dist/ibm-cos-sdk-core-2.9.0.tar", last modified: Mon Dec 14 21:54:41 2020, max compression
```

## Comparing `ibm-cos-sdk-core-2.8.0.tar` & `ibm-cos-sdk-core-2.9.0.tar`

### file list

```diff
@@ -1,541 +1,539 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_cos_sdk_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)       92 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_cos_sdk_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1868 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_cos_sdk_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20199 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_cos_sdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_cos_sdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_cos_sdk_core.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      178 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1868 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/
--rwxr-xr-x   0 root         (0) root         (0)    17207 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2913 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_waiters.py
--rw-r--r--   0 root         (0) root         (0)     4176 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_kinesis.py
--rw-r--r--   0 root         (0) root         (0)     2774 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_apigateway.py
--rw-r--r--   0 root         (0) root         (0)      566 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3411 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_ec2.py
--rw-r--r--   0 root         (0) root         (0)     1687 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_rds.py
--rw-r--r--   0 root         (0) root         (0)     3045 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_elastictranscoder.py
--rw-r--r--   0 root         (0) root         (0)     2415 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2145 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_session.py
--rw-r--r--   0 root         (0) root         (0)     1208 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_cognito_identity.py
--rw-r--r--   0 root         (0) root         (0)     1947 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_route53.py
--rw-r--r--   0 root         (0) root         (0)     2572 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_loaders.py
--rw-r--r--   0 root         (0) root         (0)     3222 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_glacier.py
--rw-r--r--   0 root         (0) root         (0)      146 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test-credentials
--rw-r--r--   0 root         (0) root         (0)     1970 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_sts.py
--rw-r--r--   0 root         (0) root         (0)     2679 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_emr.py
--rw-r--r--   0 root         (0) root         (0)    14253 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_credentials.py
--rw-r--r--   0 root         (0) root         (0)    12855 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_smoke.py
--rw-r--r--   0 root         (0) root         (0)     7917 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_client_http.py
--rw-r--r--   0 root         (0) root         (0)     7303 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_client.py
--rw-r--r--   0 root         (0) root         (0)     1273 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_cloudformation.py
--rw-r--r--   0 root         (0) root         (0)    53489 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/integration/test_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/
--rw-r--r--   0 root         (0) root         (0)     1691 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/steps/
--rw-r--r--   0 root         (0) root         (0)     3608 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/steps/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/codedeploy/
--rw-r--r--   0 root         (0) root         (0)      443 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/codedeploy/codedeploy.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cognitosync/
--rw-r--r--   0 root         (0) root         (0)      498 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cognitosync/cognitosync.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/support/
--rw-r--r--   0 root         (0) root         (0)      627 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/support/support.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/importexport/
--rw-r--r--   0 root         (0) root         (0)      485 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/importexport/importexport.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/codecommit/
--rw-r--r--   0 root         (0) root         (0)      440 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/codecommit/codecommit.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/efs/
--rw-r--r--   0 root         (0) root         (0)      438 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/efs/efs.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudwatch/
--rw-r--r--   0 root         (0) root         (0)      504 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudwatch/cloudwatch.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/machinelearning/
--rw-r--r--   0 root         (0) root         (0)      487 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/machinelearning/machinelearning.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/storagegateway/
--rw-r--r--   0 root         (0) root         (0)      477 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/storagegateway/storagegateway.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/directconnect/
--rw-r--r--   0 root         (0) root         (0)      454 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/directconnect/directconnect.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/workspaces/
--rw-r--r--   0 root         (0) root         (0)      464 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/workspaces/workspaces.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/route53/
--rw-r--r--   0 root         (0) root         (0)      407 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/route53/route53.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/autoscaling/
--rw-r--r--   0 root         (0) root         (0)      546 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/autoscaling/autoscaling.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/lambda/
--rw-r--r--   0 root         (0) root         (0)      417 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/lambda/lambda.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudhsm/
--rw-r--r--   0 root         (0) root         (0)      407 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudhsm/cloudhsm.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudsearch/
--rw-r--r--   0 root         (0) root         (0)      435 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudsearch/cloudsearch.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/sns/
--rw-r--r--   0 root         (0) root         (0)      443 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/sns/sns.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/glacier/
--rw-r--r--   0 root         (0) root         (0)      414 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/glacier/glacier.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/configservice/
--rw-r--r--   0 root         (0) root         (0)      499 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/configservice/configservice.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/redshift/
--rw-r--r--   0 root         (0) root         (0)      440 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/redshift/redshift.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/sqs/
--rw-r--r--   0 root         (0) root         (0)      437 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/sqs/sqs.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudtrail/
--rw-r--r--   0 root         (0) root         (0)      412 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudtrail/cloudtrail.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/opsworks/
--rw-r--r--   0 root         (0) root         (0)      415 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/opsworks/opsworks.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/es/
--rw-r--r--   0 root         (0) root         (0)      477 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/es/es.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/devicefarm/
--rw-r--r--   0 root         (0) root         (0)      460 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/devicefarm/devicefarm.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/waf/
--rw-r--r--   0 root         (0) root         (0)      490 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/waf/waf.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/elasticache/
--rw-r--r--   0 root         (0) root         (0)      429 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/elasticache/elasticache.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/codepipeline/
--rw-r--r--   0 root         (0) root         (0)      425 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/codepipeline/codepipeline.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/directoryservice/
--rw-r--r--   0 root         (0) root         (0)      471 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/directoryservice/directoryservice.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/dynamodb/
--rw-r--r--   0 root         (0) root         (0)      463 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/dynamodb/dynamodb.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/emr/
--rw-r--r--   0 root         (0) root         (0)      437 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/emr/emr.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/elasticbeanstalk/
--rw-r--r--   0 root         (0) root         (0)      475 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/elasticbeanstalk/elasticbeanstalk.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudfront/
--rw-r--r--   0 root         (0) root         (0)      459 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudfront/cloudfront.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/elasticloadbalancing/
--rw-r--r--   0 root         (0) root         (0)      501 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/elasticloadbalancing/elasticloadbalancing.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/iam/
--rw-r--r--   0 root         (0) root         (0)      406 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/iam/iam.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudwatchlogs/
--rw-r--r--   0 root         (0) root         (0)      483 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudwatchlogs/cloudwatchlogs.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/ecs/
--rw-r--r--   0 root         (0) root         (0)      400 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/ecs/ecs.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/kinesis/
--rw-r--r--   0 root         (0) root         (0)      425 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/kinesis/kinesis.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/ses/
--rw-r--r--   0 root         (0) root         (0)      442 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/ses/ses.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudformation/
--rw-r--r--   0 root         (0) root         (0)      497 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cloudformation/cloudformation.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/rds/
--rw-r--r--   0 root         (0) root         (0)      436 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/rds/rds.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/sts/
--rw-r--r--   0 root         (0) root         (0)      450 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/sts/sts.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/dynamodbstreams/
--rw-r--r--   0 root         (0) root         (0)      505 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/dynamodbstreams/dynamodbstreams.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/kms/
--rw-r--r--   0 root         (0) root         (0)      502 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/kms/kms.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/datapipeline/
--rw-r--r--   0 root         (0) root         (0)      438 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/datapipeline/datapipeline.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/acm/
--rw-r--r--   0 root         (0) root         (0)      444 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/acm/acm.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/ssm/
--rw-r--r--   0 root         (0) root         (0)      409 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/ssm/ssm.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/swf/
--rw-r--r--   0 root         (0) root         (0)      469 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/swf/swf.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/elastictranscoder/
--rw-r--r--   0 root         (0) root         (0)      415 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/elastictranscoder/elastictranscoder.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/route53domains/
--rw-r--r--   0 root         (0) root         (0)      426 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/route53domains/route53domains.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cognitoidentity/
--rw-r--r--   0 root         (0) root         (0)      541 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cognitoidentity/cognitoidentity.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/ec2/
--rw-r--r--   0 root         (0) root         (0)      460 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/ec2/ec2.feature
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)    26334 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_waiters.py
--rw-r--r--   0 root         (0) root         (0)    14368 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_protocols.py
--rw-r--r--   0 root         (0) root         (0)     5621 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_errorfactory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/
--rw-r--r--   0 root         (0) root         (0)      181 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/aws_config_nested
--rw-r--r--   0 root         (0) root         (0)       44 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/boto_config_empty
--rw-r--r--   0 root         (0) root         (0)      176 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/aws_config_other
--rw-r--r--   0 root         (0) root         (0)       36 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/aws_credentials
--rw-r--r--   0 root         (0) root         (0)    51200 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/aws_config_badbytes
--rw-r--r--   0 root         (0) root         (0)       29 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/aws_config_nocreds
--rw-r--r--   0 root         (0) root         (0)      191 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/aws_third_config
--rw-r--r--   0 root         (0) root         (0)      164 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/aws_config
--rw-r--r--   0 root         (0) root         (0)      147 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/aws_config_nested_bad
--rw-r--r--   0 root         (0) root         (0)       66 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/boto_config
--rw-r--r--   0 root         (0) root         (0)      494 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/aws_bad_profile
--rw-r--r--   0 root         (0) root         (0)      154 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/foo_config
--rw-r--r--   0 root         (0) root         (0)      126 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/cfg/aws_config_bad
--rw-r--r--   0 root         (0) root         (0)     1730 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10833 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_http_session.py
--rw-r--r--   0 root         (0) root         (0)    14080 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_eventstream.py
--rw-r--r--   0 root         (0) root         (0)    27532 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_hooks.py
--rw-r--r--   0 root         (0) root         (0)    55239 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_paginate.py
--rw-r--r--   0 root         (0) root         (0)    14270 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_retryhandler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/
--rwxr-xr-x   0 root         (0) root         (0)    13915 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/test_response_parsing.py
--rw-r--r--   0 root         (0) root         (0)      621 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/
--rw-r--r--   0 root         (0) root         (0)      965 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-objects.xml
--rw-r--r--   0 root         (0) root         (0)       64 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-location.json
--rw-r--r--   0 root         (0) root         (0)      153 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-policy.xml
--rw-r--r--   0 root         (0) root         (0)     2733 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-object-versions.xml
--rw-r--r--   0 root         (0) root         (0)     5077 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-buckets.json
--rw-r--r--   0 root         (0) root         (0)     2057 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.json
--rw-r--r--   0 root         (0) root         (0)      353 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.json
--rw-r--r--   0 root         (0) root         (0)     2036 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.xml
--rw-r--r--   0 root         (0) root         (0)      566 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.xml
--rw-r--r--   0 root         (0) root         (0)     4007 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-buckets.xml
--rw-r--r--   0 root         (0) root         (0)      503 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.json
--rw-r--r--   0 root         (0) root         (0)      228 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-policy.json
--rw-r--r--   0 root         (0) root         (0)     2567 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-object-versions.json
--rw-r--r--   0 root         (0) root         (0)      131 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-location.xml
--rw-r--r--   0 root         (0) root         (0)      398 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.json
--rw-r--r--   0 root         (0) root         (0)      937 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-objects.json
--rw-r--r--   0 root         (0) root         (0)      620 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.xml
--rw-r--r--   0 root         (0) root         (0)      568 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/errors/
--rw-r--r--   0 root         (0) root         (0)      245 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/errors/s3-list-objects.xml
--rw-r--r--   0 root         (0) root         (0)      325 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/errors/s3-create-bucket.xml
--rw-r--r--   0 root         (0) root         (0)      237 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/errors/s3-create-bucket.json
--rw-r--r--   0 root         (0) root         (0)      120 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/errors/s3-list-objects.json
--rw-r--r--   0 root         (0) root         (0)     1385 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/README.rst
--rw-r--r--   0 root         (0) root         (0)     6150 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_compat.py
--rw-r--r--   0 root         (0) root         (0)     1097 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_http_client_exception_mapping.py
--rw-r--r--   0 root         (0) root         (0)    37167 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_model.py
--rw-r--r--   0 root         (0) root         (0)    93660 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_utils.py
--rw-r--r--   0 root         (0) root         (0)    44891 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_parsers.py
--rw-r--r--   0 root         (0) root         (0)    36371 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_session.py
--rw-r--r--   0 root         (0) root         (0)     4404 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_translate.py
--rw-r--r--   0 root         (0) root         (0)    16101 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_args.py
--rw-r--r--   0 root         (0) root         (0)       28 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/put_object_data
--rw-r--r--   0 root         (0) root         (0)    34817 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_session_legacy.py
--rw-r--r--   0 root         (0) root         (0)    17699 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_loaders.py
--rw-r--r--   0 root         (0) root         (0)    12096 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_response.py
--rw-r--r--   0 root         (0) root         (0)     8030 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_stub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/data/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/data/aws/s3/
--rw-r--r--   0 root         (0) root         (0)       44 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/data/aws/s3/2006-03-01.normal.json
--rw-r--r--   0 root         (0) root         (0)      213 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/data/non_ascii.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/data/someservice/
--rw-r--r--   0 root         (0) root         (0)       70 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/data/someservice/2013-08-21.normal.json
--rw-r--r--   0 root         (0) root         (0)       69 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/data/someservice/2012-10-01.normal.json
--rw-r--r--   0 root         (0) root         (0)      231 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/data/foo.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/data/sub/
--rw-r--r--   0 root         (0) root         (0)       37 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/data/sub/fie.normal.json
--rw-r--r--   0 root         (0) root         (0)       19 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/data/baz.json
--rw-r--r--   0 root         (0) root         (0)    18826 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_serialize.py
--rw-r--r--   0 root         (0) root         (0)    47335 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_handlers.py
--rw-r--r--   0 root         (0) root         (0)     9749 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_s3_addressing.py
--rw-r--r--   0 root         (0) root         (0)    34014 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)    14224 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_endpoint.py
--rw-r--r--   0 root         (0) root         (0)     6481 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7531 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_configloader.py
--rw-r--r--   0 root         (0) root         (0)   126104 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_credentials.py
--rw-r--r--   0 root         (0) root         (0)    16043 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_validate.py
--rw-r--r--   0 root         (0) root         (0)    29080 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_awsrequest.py
--rw-r--r--   0 root         (0) root         (0)     1541 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_idempotency.py
--rw-r--r--   0 root         (0) root         (0)    19455 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_config_provider.py
--rw-r--r--   0 root         (0) root         (0)    87997 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3189 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_history.py
--rw-r--r--   0 root         (0) root         (0)     9926 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_regions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/
--rw-r--r--   0 root         (0) root         (0)      626 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/
--rw-r--r--   0 root         (0) root         (0)      142 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla.creq
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved.authz
--rw-r--r--   0 root         (0) root         (0)       86 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-key-sort.req
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-relative-relative.sts
--rw-r--r--   0 root         (0) root         (0)      272 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash-pointless-dot.sreq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-key-duplicate.sts
--rw-r--r--   0 root         (0) root         (0)      139 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-unreserved.req
--rw-r--r--   0 root         (0) root         (0)      333 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-unreserved.sreq
--rw-r--r--   0 root         (0) root         (0)      279 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key.sreq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query.sts
--rw-r--r--   0 root         (0) root         (0)      142 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash-dot-slash.creq
--rw-r--r--   0 root         (0) root         (0)      157 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-utf8.creq
--rw-r--r--   0 root         (0) root         (0)       74 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash.req
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-value-trim.sts
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-relative.authz
--rw-r--r--   0 root         (0) root         (0)      142 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-relative-relative.creq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla.sts
--rw-r--r--   0 root         (0) root         (0)      218 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters.creq
--rw-r--r--   0 root         (0) root         (0)      273 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slashes.sreq
--rw-r--r--   0 root         (0) root         (0)       82 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query.req
--rw-r--r--   0 root         (0) root         (0)      146 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slashes.creq
--rw-r--r--   0 root         (0) root         (0)      153 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key.creq
--rw-r--r--   0 root         (0) root         (0)      208 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-unreserved.creq
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-unreserved.authz
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash.authz
--rw-r--r--   0 root         (0) root         (0)      143 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters.req
--rw-r--r--   0 root         (0) root         (0)      181 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-key-duplicate.authz
--rw-r--r--   0 root         (0) root         (0)       78 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash-pointless-dot.req
--rw-r--r--   0 root         (0) root         (0)      268 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash.sreq
--rw-r--r--   0 root         (0) root         (0)       94 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-value-order.req
--rw-r--r--   0 root         (0) root         (0)       85 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value.req
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query.authz
--rw-r--r--   0 root         (0) root         (0)       79 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-relative.req
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query.authz
--rw-r--r--   0 root         (0) root         (0)      336 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded.sreq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value.sts
--rw-r--r--   0 root         (0) root         (0)      276 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query.sreq
--rw-r--r--   0 root         (0) root         (0)      268 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla.sreq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slashes.sts
--rw-r--r--   0 root         (0) root         (0)      150 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query.creq
--rw-r--r--   0 root         (0) root         (0)      143 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-key-case.creq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters.sts
--rw-r--r--   0 root         (0) root         (0)      269 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash-dot-slash.sreq
--rw-r--r--   0 root         (0) root         (0)      143 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla.creq
--rw-r--r--   0 root         (0) root         (0)      276 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value.sreq
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key.authz
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value.sts
--rw-r--r--   0 root         (0) root         (0)      142 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash.creq
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slashes.authz
--rw-r--r--   0 root         (0) root         (0)      124 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-nonunreserved.req
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case.sts
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-utf8.authz
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-space.sts
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash-pointless-dot.sts
--rw-r--r--   0 root         (0) root         (0)      275 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved.creq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash.sts
--rw-r--r--   0 root         (0) root         (0)       89 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case.req
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-relative-relative.authz
--rw-r--r--   0 root         (0) root         (0)      145 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash-pointless-dot.creq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-unreserved.sts
--rw-r--r--   0 root         (0) root         (0)       73 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla.req
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-space.authz
--rw-r--r--   0 root         (0) root         (0)      350 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters.sreq
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla.authz
--rw-r--r--   0 root         (0) root         (0)      151 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-space.creq
--rw-r--r--   0 root         (0) root         (0)      157 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case.creq
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-space.authz
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-nonunreserved.authz
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-key-case.sts
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case.authz
--rw-r--r--   0 root         (0) root         (0)       85 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-value-trim.req
--rw-r--r--   0 root         (0) root         (0)      275 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key.sreq
--rw-r--r--   0 root         (0) root         (0)      279 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value.sreq
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key.authz
--rw-r--r--   0 root         (0) root         (0)       74 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla.req
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-value-order.sts
--rw-r--r--   0 root         (0) root         (0)       81 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-ut8-query.req
--rw-r--r--   0 root         (0) root         (0)      318 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-nonunreserved.sreq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query.sts
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded.sts
--rw-r--r--   0 root         (0) root         (0)       82 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value.req
--rw-r--r--   0 root         (0) root         (0)       85 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key.req
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-space.sts
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash-dot-slash.sts
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved.sts
--rw-r--r--   0 root         (0) root         (0)       74 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-key-case.req
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash-dot-slash.authz
--rw-r--r--   0 root         (0) root         (0)       86 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-relative-relative.req
--rw-r--r--   0 root         (0) root         (0)      154 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-value-trim.creq
--rw-r--r--   0 root         (0) root         (0)      155 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-ut8-query.creq
--rw-r--r--   0 root         (0) root         (0)      209 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-nonunreserved.creq
--rw-r--r--   0 root         (0) root         (0)       80 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-space.req
--rw-r--r--   0 root         (0) root         (0)      179 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-value-order.authz
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-value-case.sts
--rw-r--r--   0 root         (0) root         (0)      142 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query.creq
--rw-r--r--   0 root         (0) root         (0)       73 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query.req
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-nonunreserved.sts
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key.sts
--rw-r--r--   0 root         (0) root         (0)      110 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-key-duplicate.req
--rw-r--r--   0 root         (0) root         (0)      308 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-key-duplicate.sreq
--rw-r--r--   0 root         (0) root         (0)      190 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded.authz
--rw-r--r--   0 root         (0) root         (0)      181 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-value-case.authz
--rw-r--r--   0 root         (0) root         (0)      273 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-relative.sreq
--rw-r--r--   0 root         (0) root         (0)      150 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value.creq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-relative.sts
--rw-r--r--   0 root         (0) root         (0)      284 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-value-case.sreq
--rw-r--r--   0 root         (0) root         (0)      280 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-relative-relative.sreq
--rw-r--r--   0 root         (0) root         (0)      145 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-space.creq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key.sts
--rw-r--r--   0 root         (0) root         (0)      179 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-value-trim.authz
--rw-r--r--   0 root         (0) root         (0)      268 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-key-case.sreq
--rw-r--r--   0 root         (0) root         (0)      290 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-value-order.sreq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-ut8-query.sts
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value.authz
--rw-r--r--   0 root         (0) root         (0)      159 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-value-case.creq
--rw-r--r--   0 root         (0) root         (0)      267 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query.sreq
--rw-r--r--   0 root         (0) root         (0)      401 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved.sreq
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash-pointless-dot.authz
--rw-r--r--   0 root         (0) root         (0)      274 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-space.sreq
--rw-r--r--   0 root         (0) root         (0)       75 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slash-dot-slash.req
--rw-r--r--   0 root         (0) root         (0)      129 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded.req
--rw-r--r--   0 root         (0) root         (0)      207 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved.req
--rw-r--r--   0 root         (0) root         (0)      278 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-space.sreq
--rw-r--r--   0 root         (0) root         (0)      153 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value.creq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-key-sort.sts
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value.authz
--rw-r--r--   0 root         (0) root         (0)       84 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-space.req
--rw-r--r--   0 root         (0) root         (0)       81 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key.req
--rw-r--r--   0 root         (0) root         (0)      284 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-key-sort.sreq
--rw-r--r--   0 root         (0) root         (0)      283 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case.sreq
--rw-r--r--   0 root         (0) root         (0)      267 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla.sreq
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-ut8-query.authz
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla.sts
--rw-r--r--   0 root         (0) root         (0)      173 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-key-duplicate.creq
--rw-r--r--   0 root         (0) root         (0)      276 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-utf8.sreq
--rw-r--r--   0 root         (0) root         (0)      281 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-value-trim.sreq
--rw-r--r--   0 root         (0) root         (0)      181 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-key-sort.authz
--rw-r--r--   0 root         (0) root         (0)      142 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-relative.creq
--rw-r--r--   0 root         (0) root         (0)      156 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-header-value-order.creq
--rw-r--r--   0 root         (0) root         (0)      190 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters.authz
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-key-case.authz
--rw-r--r--   0 root         (0) root         (0)       86 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-value-case.req
--rw-r--r--   0 root         (0) root         (0)      177 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-vanilla.authz
--rw-r--r--   0 root         (0) root         (0)      149 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key.creq
--rw-r--r--   0 root         (0) root         (0)      275 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-vanilla-ut8-query.sreq
--rw-r--r--   0 root         (0) root         (0)      159 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-header-key-sort.creq
--rw-r--r--   0 root         (0) root         (0)      138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-utf8.sts
--rw-r--r--   0 root         (0) root         (0)       82 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-utf8.req
--rw-r--r--   0 root         (0) root         (0)       79 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/get-slashes.req
--rw-r--r--   0 root         (0) root         (0)      204 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded.creq
--rw-r--r--   0 root         (0) root         (0)    43875 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/test_signers.py
--rw-r--r--   0 root         (0) root         (0)     7115 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/auth/test_sigv4.py
--rwxr-xr-x   0 root         (0) root         (0)    38643 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_signers.py
--rw-r--r--   0 root         (0) root         (0)     1351 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/unit/test_auth_sigv4.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/functional/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/functional/models/
--rw-r--r--   0 root         (0) root         (0)    77688 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/models/endpoints.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/functional/models/custom-acm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/functional/models/custom-acm/2015-12-08/
--rw-r--r--   0 root         (0) root         (0)    57976 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/models/custom-acm/2015-12-08/service-2.json
--rw-r--r--   0 root         (0) root         (0)      874 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/models/custom-acm/2015-12-08/waiters-2.json
--rw-r--r--   0 root         (0) root         (0)      203 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/models/custom-acm/2015-12-08/paginators-1.json
--rw-r--r--   0 root         (0) root         (0)       44 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/models/custom-acm/2015-12-08/examples-1.json
--rw-r--r--   0 root         (0) root         (0)     1766 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8496 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_paginate.py
--rwxr-xr-x   0 root         (0) root         (0)     4647 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_session.py
--rwxr-xr-x   0 root         (0) root         (0)     8133 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_retry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/functional/leak/
--rw-r--r--   0 root         (0) root         (0)     5529 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/leak/test_resource_leaks.py
--rw-r--r--   0 root         (0) root         (0)      561 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/leak/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1872 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_client_metadata.py
--rwxr-xr-x   0 root         (0) root         (0)     7146 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     1621 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_loaders.py
--rw-r--r--   0 root         (0) root         (0)    12523 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_stub.py
--rw-r--r--   0 root         (0) root         (0)     1677 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_six_threading.py
--rw-r--r--   0 root         (0) root         (0)     2416 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_service_names.py
--rw-r--r--   0 root         (0) root         (0)     7370 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_waiter_config.py
--rwxr-xr-x   0 root         (0) root         (0)    33878 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_credentials.py
--rw-r--r--   0 root         (0) root         (0)     1878 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_six_imports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/functional/utils/
--rw-r--r--   0 root         (0) root         (0)      561 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1168 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/utils/credentialprocess.py
--rw-r--r--   0 root         (0) root         (0)     5357 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_history.py
--rw-r--r--   0 root         (0) root         (0)     2043 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_h2_required.py
--rw-r--r--   0 root         (0) root         (0)    26056 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_regions.py
--rwxr-xr-x   0 root         (0) root         (0)    12258 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_paginator_config.py
--rw-r--r--   0 root         (0) root         (0)    76799 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/functional/docs/
--rw-r--r--   0 root         (0) root         (0)     4622 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5147 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/docs/test_shared_example_config.py
--rw-r--r--   0 root         (0) root         (0)     1764 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/docs/test_streaming_body.py
--rwxr-xr-x   0 root         (0) root         (0)     2875 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/docs/test_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/functional/csm/
--rw-r--r--   0 root         (0) root         (0)      561 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/csm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/functional/csm/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/functional/csm/data/csmtest/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/tests/functional/csm/data/csmtest/2018-06-19/
--rw-r--r--   0 root         (0) root         (0)      895 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/csm/data/csmtest/2018-06-19/service-2.json
--rwxr-xr-x   0 root         (0) root         (0)     6821 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/csm/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)    32068 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/csm/cases.json
--rwxr-xr-x   0 root         (0) root         (0)     1145 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_client_class_names.py
--rw-r--r--   0 root         (0) root         (0)     3621 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_model_backcompat.py
--rw-r--r--   0 root         (0) root         (0)     1809 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/functional/test_model_completeness.py
--rw-r--r--   0 root         (0) root         (0)     8452 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/tests/cmd-runner
--rw-r--r--   0 root         (0) root         (0)    10174 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/LICENSE.txt
--rwxr-xr-x   0 root         (0) root         (0)      157 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/
--rw-r--r--   0 root         (0) root         (0)    10428 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/discovery.py
--rwxr-xr-x   0 root         (0) root         (0)     3508 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14409 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/stub.py
--rw-r--r--   0 root         (0) root         (0)     1748 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/history.py
--rw-r--r--   0 root         (0) root         (0)    11614 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/compat.py
--rw-r--r--   0 root         (0) root         (0)    20594 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/monitoring.py
--rwxr-xr-x   0 root         (0) root         (0)    40685 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/handlers.py
--rwxr-xr-x   0 root         (0) root         (0)    16132 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/args.py
--rw-r--r--   0 root         (0) root         (0)     4103 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/errorfactory.py
--rw-r--r--   0 root         (0) root         (0)    12454 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/waiter.py
--rw-r--r--   0 root         (0) root         (0)    36069 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/auth.py
--rwxr-xr-x   0 root         (0) root         (0)    48086 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/session.py
--rw-r--r--   0 root         (0) root         (0)     8424 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/regions.py
--rw-r--r--   0 root         (0) root         (0)    23291 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/awsrequest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/
--rw-r--r--   0 root         (0) root         (0)      125 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1615 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/special.py
--rw-r--r--   0 root         (0) root         (0)    19618 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/standard.py
--rw-r--r--   0 root         (0) root         (0)     4203 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/adaptive.py
--rw-r--r--   0 root         (0) root         (0)      813 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/base.py
--rw-r--r--   0 root         (0) root         (0)     4024 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/bucket.py
--rw-r--r--   0 root         (0) root         (0)     1788 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/throttling.py
--rw-r--r--   0 root         (0) root         (0)     1963 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/quota.py
--rwxr-xr-x   0 root         (0) root         (0)    13785 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/retryhandler.py
--rwxr-xr-x   0 root         (0) root         (0)    11818 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/config.py
--rw-r--r--   0 root         (0) root         (0)    28138 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/signers.py
--rwxr-xr-x   0 root         (0) root         (0)    17554 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/vendored/
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/vendored/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30098 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/vendored/six.py
--rw-r--r--   0 root         (0) root         (0)    27148 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/paginate.py
--rw-r--r--   0 root         (0) root         (0)    40372 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/parsers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/data/
--rw-r--r--   0 root         (0) root         (0)   171243 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/data/endpoints.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/data/s3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/data/s3/2006-03-01/
--rwxr-xr-x   0 root         (0) root         (0)   460879 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/data/s3/2006-03-01/service-2.json
--rw-r--r--   0 root         (0) root         (0)     1436 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/data/s3/2006-03-01/waiters-2.json
--rwxr-xr-x   0 root         (0) root         (0)     1404 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/data/s3/2006-03-01/paginators-1.json
--rw-r--r--   0 root         (0) root         (0)       44 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/data/s3/2006-03-01/examples-1.json
--rw-r--r--   0 root         (0) root         (0)     7025 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/data/_retry.json
--rw-r--r--   0 root         (0) root         (0)    11521 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/validate.py
--rw-r--r--   0 root         (0) root         (0)    11508 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/httpsession.py
--rw-r--r--   0 root         (0) root         (0)    20113 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/eventstream.py
--rw-r--r--   0 root         (0) root         (0)    64616 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/utils.py
--rw-r--r--   0 root         (0) root         (0)    24581 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/hooks.py
--rwxr-xr-x   0 root         (0) root         (0)   110082 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/credentials.py
--rw-r--r--   0 root         (0) root         (0)    17411 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/loaders.py
--rw-r--r--   0 root         (0) root         (0)    26898 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/model.py
--rw-r--r--   0 root         (0) root         (0)    21581 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/configprovider.py
--rw-r--r--   0 root         (0) root         (0)     9604 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/configloader.py
--rwxr-xr-x   0 root         (0) root         (0)    39542 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/client.py
--rwxr-xr-x   0 root         (0) root         (0)     3416 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/translate.py
--rw-r--r--   0 root         (0) root         (0)   271088 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/cacert.pem
--rw-r--r--   0 root         (0) root         (0)     6456 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/
--rw-r--r--   0 root         (0) root         (0)     1551 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7070 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/paginator.py
--rw-r--r--   0 root         (0) root         (0)     3715 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/docstring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/bcdoc/
--rw-r--r--   0 root         (0) root         (0)      588 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/bcdoc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4733 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/bcdoc/docevents.py
--rw-r--r--   0 root         (0) root         (0)    11833 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/bcdoc/style.py
--rw-r--r--   0 root         (0) root         (0)     5893 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/bcdoc/docstringparser.py
--rw-r--r--   0 root         (0) root         (0)    20611 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/bcdoc/textwriter.py
--rw-r--r--   0 root         (0) root         (0)     7238 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/bcdoc/restdoc.py
--rw-r--r--   0 root         (0) root         (0)     4843 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/waiter.py
--rw-r--r--   0 root         (0) root         (0)    11565 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/method.py
--rwxr-xr-x   0 root         (0) root         (0)     3717 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/service.py
--rw-r--r--   0 root         (0) root         (0)     7176 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/utils.py
--rw-r--r--   0 root         (0) root         (0)     8759 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/example.py
--rw-r--r--   0 root         (0) root         (0)     4693 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/client.py
--rw-r--r--   0 root         (0) root         (0)     9338 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/sharedexample.py
--rw-r--r--   0 root         (0) root         (0)     9569 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/params.py
--rw-r--r--   0 root         (0) root         (0)     4998 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/shape.py
--rwxr-xr-x   0 root         (0) root         (0)    12616 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/endpoint.py
--rw-r--r--   0 root         (0) root         (0)    29839 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/ibm_botocore/serialize.py
--rwxr-xr-x   0 root         (0) root         (0)     1394 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/docs/source/
--rwxr-xr-x   0 root         (0) root         (0)     8625 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/docs/source/conf.py
--rwxr-xr-x   0 root         (0) root         (0)     8369 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/docs/source/client_upgrades.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/docs/source/_static/
--rwxr-xr-x   0 root         (0) root         (0)      717 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/docs/source/_static/404.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/docs/source/reference/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:24.000000 ibm-cos-sdk-core-2.8.0/docs/source/reference/services/
--rwxr-xr-x   0 root         (0) root         (0)   214436 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/docs/source/reference/services/s3.rst
--rwxr-xr-x   0 root         (0) root         (0)      160 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/docs/source/reference/config.rst
--rwxr-xr-x   0 root         (0) root         (0)      105 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/docs/source/reference/index.rst
--rwxr-xr-x   0 root         (0) root         (0)      511 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/docs/source/index.rst
--rwxr-xr-x   0 root         (0) root         (0)     5109 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/docs/make.bat
--rwxr-xr-x   0 root         (0) root         (0)     5581 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/docs/Makefile
--rwxr-xr-x   0 root         (0) root         (0)      208 2020-10-27 20:35:23.000000 ibm-cos-sdk-core-2.8.0/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_cos_sdk_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       71 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_cos_sdk_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1836 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_cos_sdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20124 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_cos_sdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_cos_sdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_cos_sdk_core.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      178 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1836 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      855 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/
+-rwxr-xr-x   0 root         (0) root         (0)    17207 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2913 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     4176 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_apigateway.py
+-rw-r--r--   0 root         (0) root         (0)      566 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3411 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_ec2.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_rds.py
+-rw-r--r--   0 root         (0) root         (0)     3045 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_elastictranscoder.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_session.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_cognito_identity.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_route53.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_loaders.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_glacier.py
+-rw-r--r--   0 root         (0) root         (0)      146 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test-credentials
+-rw-r--r--   0 root         (0) root         (0)     1970 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_sts.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_emr.py
+-rw-r--r--   0 root         (0) root         (0)    14253 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    12855 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_smoke.py
+-rw-r--r--   0 root         (0) root         (0)     7917 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_client_http.py
+-rw-r--r--   0 root         (0) root         (0)     7303 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_cloudformation.py
+-rw-r--r--   0 root         (0) root         (0)    53489 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/integration/test_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/
+-rw-r--r--   0 root         (0) root         (0)     1691 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/steps/
+-rw-r--r--   0 root         (0) root         (0)     3608 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/steps/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/codedeploy/
+-rw-r--r--   0 root         (0) root         (0)      443 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/codedeploy/codedeploy.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cognitosync/
+-rw-r--r--   0 root         (0) root         (0)      498 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cognitosync/cognitosync.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/support/
+-rw-r--r--   0 root         (0) root         (0)      627 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/support/support.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/importexport/
+-rw-r--r--   0 root         (0) root         (0)      485 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/importexport/importexport.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/codecommit/
+-rw-r--r--   0 root         (0) root         (0)      440 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/codecommit/codecommit.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/efs/
+-rw-r--r--   0 root         (0) root         (0)      438 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/efs/efs.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudwatch/
+-rw-r--r--   0 root         (0) root         (0)      504 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudwatch/cloudwatch.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/machinelearning/
+-rw-r--r--   0 root         (0) root         (0)      487 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/machinelearning/machinelearning.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/storagegateway/
+-rw-r--r--   0 root         (0) root         (0)      477 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/storagegateway/storagegateway.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/directconnect/
+-rw-r--r--   0 root         (0) root         (0)      454 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/directconnect/directconnect.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/workspaces/
+-rw-r--r--   0 root         (0) root         (0)      464 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/workspaces/workspaces.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/route53/
+-rw-r--r--   0 root         (0) root         (0)      407 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/route53/route53.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)      546 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/autoscaling/autoscaling.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/lambda/
+-rw-r--r--   0 root         (0) root         (0)      417 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/lambda/lambda.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudhsm/
+-rw-r--r--   0 root         (0) root         (0)      407 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudhsm/cloudhsm.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudsearch/
+-rw-r--r--   0 root         (0) root         (0)      435 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudsearch/cloudsearch.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/sns/
+-rw-r--r--   0 root         (0) root         (0)      443 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/sns/sns.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/glacier/
+-rw-r--r--   0 root         (0) root         (0)      414 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/glacier/glacier.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/configservice/
+-rw-r--r--   0 root         (0) root         (0)      499 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/configservice/configservice.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/redshift/
+-rw-r--r--   0 root         (0) root         (0)      440 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/redshift/redshift.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/sqs/
+-rw-r--r--   0 root         (0) root         (0)      437 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/sqs/sqs.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudtrail/
+-rw-r--r--   0 root         (0) root         (0)      412 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudtrail/cloudtrail.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/opsworks/
+-rw-r--r--   0 root         (0) root         (0)      415 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/opsworks/opsworks.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/es/
+-rw-r--r--   0 root         (0) root         (0)      477 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/es/es.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/devicefarm/
+-rw-r--r--   0 root         (0) root         (0)      460 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/devicefarm/devicefarm.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/waf/
+-rw-r--r--   0 root         (0) root         (0)      490 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/waf/waf.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/elasticache/
+-rw-r--r--   0 root         (0) root         (0)      429 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/elasticache/elasticache.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/codepipeline/
+-rw-r--r--   0 root         (0) root         (0)      425 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/codepipeline/codepipeline.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/directoryservice/
+-rw-r--r--   0 root         (0) root         (0)      471 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/directoryservice/directoryservice.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/dynamodb/
+-rw-r--r--   0 root         (0) root         (0)      463 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/dynamodb/dynamodb.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/emr/
+-rw-r--r--   0 root         (0) root         (0)      437 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/emr/emr.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/elasticbeanstalk/
+-rw-r--r--   0 root         (0) root         (0)      475 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/elasticbeanstalk/elasticbeanstalk.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudfront/
+-rw-r--r--   0 root         (0) root         (0)      459 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudfront/cloudfront.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/elasticloadbalancing/
+-rw-r--r--   0 root         (0) root         (0)      501 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/elasticloadbalancing/elasticloadbalancing.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/iam/
+-rw-r--r--   0 root         (0) root         (0)      406 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/iam/iam.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudwatchlogs/
+-rw-r--r--   0 root         (0) root         (0)      483 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudwatchlogs/cloudwatchlogs.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/ecs/
+-rw-r--r--   0 root         (0) root         (0)      400 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/ecs/ecs.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/kinesis/
+-rw-r--r--   0 root         (0) root         (0)      425 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/kinesis/kinesis.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/ses/
+-rw-r--r--   0 root         (0) root         (0)      442 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/ses/ses.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)      497 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cloudformation/cloudformation.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/rds/
+-rw-r--r--   0 root         (0) root         (0)      436 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/rds/rds.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/sts/
+-rw-r--r--   0 root         (0) root         (0)      450 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/sts/sts.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/dynamodbstreams/
+-rw-r--r--   0 root         (0) root         (0)      505 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/dynamodbstreams/dynamodbstreams.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/kms/
+-rw-r--r--   0 root         (0) root         (0)      502 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/kms/kms.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/datapipeline/
+-rw-r--r--   0 root         (0) root         (0)      438 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/datapipeline/datapipeline.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/acm/
+-rw-r--r--   0 root         (0) root         (0)      444 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/acm/acm.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/ssm/
+-rw-r--r--   0 root         (0) root         (0)      409 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/ssm/ssm.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/swf/
+-rw-r--r--   0 root         (0) root         (0)      469 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/swf/swf.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/elastictranscoder/
+-rw-r--r--   0 root         (0) root         (0)      415 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/elastictranscoder/elastictranscoder.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/route53domains/
+-rw-r--r--   0 root         (0) root         (0)      426 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/route53domains/route53domains.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cognitoidentity/
+-rw-r--r--   0 root         (0) root         (0)      541 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cognitoidentity/cognitoidentity.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/ec2/
+-rw-r--r--   0 root         (0) root         (0)      460 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/ec2/ec2.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)    26334 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_waiters.py
+-rw-r--r--   0 root         (0) root         (0)    14368 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_protocols.py
+-rw-r--r--   0 root         (0) root         (0)     5621 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_errorfactory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/
+-rw-r--r--   0 root         (0) root         (0)      181 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/aws_config_nested
+-rw-r--r--   0 root         (0) root         (0)       44 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/boto_config_empty
+-rw-r--r--   0 root         (0) root         (0)      176 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/aws_config_other
+-rw-r--r--   0 root         (0) root         (0)       36 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/aws_credentials
+-rw-r--r--   0 root         (0) root         (0)    51200 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/aws_config_badbytes
+-rw-r--r--   0 root         (0) root         (0)       29 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/aws_config_nocreds
+-rw-r--r--   0 root         (0) root         (0)      191 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/aws_third_config
+-rw-r--r--   0 root         (0) root         (0)      164 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/aws_config
+-rw-r--r--   0 root         (0) root         (0)      147 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/aws_config_nested_bad
+-rw-r--r--   0 root         (0) root         (0)       66 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/boto_config
+-rw-r--r--   0 root         (0) root         (0)      494 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/aws_bad_profile
+-rw-r--r--   0 root         (0) root         (0)      154 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/foo_config
+-rw-r--r--   0 root         (0) root         (0)      126 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/cfg/aws_config_bad
+-rw-r--r--   0 root         (0) root         (0)     1730 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10833 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_http_session.py
+-rw-r--r--   0 root         (0) root         (0)    14080 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_eventstream.py
+-rw-r--r--   0 root         (0) root         (0)    27532 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_hooks.py
+-rw-r--r--   0 root         (0) root         (0)    55239 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_paginate.py
+-rw-r--r--   0 root         (0) root         (0)    14270 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_retryhandler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/
+-rwxr-xr-x   0 root         (0) root         (0)    13915 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/test_response_parsing.py
+-rw-r--r--   0 root         (0) root         (0)      621 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/
+-rw-r--r--   0 root         (0) root         (0)      965 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-objects.xml
+-rw-r--r--   0 root         (0) root         (0)       64 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-location.json
+-rw-r--r--   0 root         (0) root         (0)      153 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-policy.xml
+-rw-r--r--   0 root         (0) root         (0)     2733 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-object-versions.xml
+-rw-r--r--   0 root         (0) root         (0)     5077 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-buckets.json
+-rw-r--r--   0 root         (0) root         (0)     2057 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.json
+-rw-r--r--   0 root         (0) root         (0)      353 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.json
+-rw-r--r--   0 root         (0) root         (0)     2036 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.xml
+-rw-r--r--   0 root         (0) root         (0)      566 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.xml
+-rw-r--r--   0 root         (0) root         (0)     4007 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-buckets.xml
+-rw-r--r--   0 root         (0) root         (0)      503 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.json
+-rw-r--r--   0 root         (0) root         (0)      228 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-policy.json
+-rw-r--r--   0 root         (0) root         (0)     2567 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-object-versions.json
+-rw-r--r--   0 root         (0) root         (0)      131 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-location.xml
+-rw-r--r--   0 root         (0) root         (0)      398 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.json
+-rw-r--r--   0 root         (0) root         (0)      937 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-objects.json
+-rw-r--r--   0 root         (0) root         (0)      620 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.xml
+-rw-r--r--   0 root         (0) root         (0)      568 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/errors/
+-rw-r--r--   0 root         (0) root         (0)      245 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/errors/s3-list-objects.xml
+-rw-r--r--   0 root         (0) root         (0)      325 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/errors/s3-create-bucket.xml
+-rw-r--r--   0 root         (0) root         (0)      237 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/errors/s3-create-bucket.json
+-rw-r--r--   0 root         (0) root         (0)      120 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/errors/s3-list-objects.json
+-rw-r--r--   0 root         (0) root         (0)     1385 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/README.rst
+-rw-r--r--   0 root         (0) root         (0)     6150 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_compat.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_http_client_exception_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    37167 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_model.py
+-rw-r--r--   0 root         (0) root         (0)    93660 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)    44891 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_parsers.py
+-rw-r--r--   0 root         (0) root         (0)    36371 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_session.py
+-rw-r--r--   0 root         (0) root         (0)     4404 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_translate.py
+-rw-r--r--   0 root         (0) root         (0)    16101 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_args.py
+-rw-r--r--   0 root         (0) root         (0)       28 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/put_object_data
+-rw-r--r--   0 root         (0) root         (0)    34817 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_session_legacy.py
+-rw-r--r--   0 root         (0) root         (0)    17699 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_loaders.py
+-rw-r--r--   0 root         (0) root         (0)    12096 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_response.py
+-rw-r--r--   0 root         (0) root         (0)     8030 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_stub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/data/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/data/aws/s3/
+-rw-r--r--   0 root         (0) root         (0)       44 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/data/aws/s3/2006-03-01.normal.json
+-rw-r--r--   0 root         (0) root         (0)      213 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/data/non_ascii.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/data/someservice/
+-rw-r--r--   0 root         (0) root         (0)       70 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/data/someservice/2013-08-21.normal.json
+-rw-r--r--   0 root         (0) root         (0)       69 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/data/someservice/2012-10-01.normal.json
+-rw-r--r--   0 root         (0) root         (0)      231 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/data/foo.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/data/sub/
+-rw-r--r--   0 root         (0) root         (0)       37 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/data/sub/fie.normal.json
+-rw-r--r--   0 root         (0) root         (0)       19 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/data/baz.json
+-rw-r--r--   0 root         (0) root         (0)    18826 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_serialize.py
+-rw-r--r--   0 root         (0) root         (0)    47335 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_handlers.py
+-rw-r--r--   0 root         (0) root         (0)     9749 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_s3_addressing.py
+-rw-r--r--   0 root         (0) root         (0)    34014 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)    14224 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)     6481 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7531 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_configloader.py
+-rw-r--r--   0 root         (0) root         (0)   126104 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    16043 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_validate.py
+-rw-r--r--   0 root         (0) root         (0)    29080 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_awsrequest.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_idempotency.py
+-rw-r--r--   0 root         (0) root         (0)    19455 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)    87997 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_history.py
+-rw-r--r--   0 root         (0) root         (0)     9926 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_regions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/
+-rw-r--r--   0 root         (0) root         (0)      626 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/
+-rw-r--r--   0 root         (0) root         (0)      142 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla.creq
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved.authz
+-rw-r--r--   0 root         (0) root         (0)       86 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-key-sort.req
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-relative-relative.sts
+-rw-r--r--   0 root         (0) root         (0)      272 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash-pointless-dot.sreq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-key-duplicate.sts
+-rw-r--r--   0 root         (0) root         (0)      139 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-unreserved.req
+-rw-r--r--   0 root         (0) root         (0)      333 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-unreserved.sreq
+-rw-r--r--   0 root         (0) root         (0)      279 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key.sreq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query.sts
+-rw-r--r--   0 root         (0) root         (0)      142 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash-dot-slash.creq
+-rw-r--r--   0 root         (0) root         (0)      157 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-utf8.creq
+-rw-r--r--   0 root         (0) root         (0)       74 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash.req
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-value-trim.sts
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-relative.authz
+-rw-r--r--   0 root         (0) root         (0)      142 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-relative-relative.creq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla.sts
+-rw-r--r--   0 root         (0) root         (0)      218 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters.creq
+-rw-r--r--   0 root         (0) root         (0)      273 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slashes.sreq
+-rw-r--r--   0 root         (0) root         (0)       82 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query.req
+-rw-r--r--   0 root         (0) root         (0)      146 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slashes.creq
+-rw-r--r--   0 root         (0) root         (0)      153 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key.creq
+-rw-r--r--   0 root         (0) root         (0)      208 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-unreserved.creq
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-unreserved.authz
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash.authz
+-rw-r--r--   0 root         (0) root         (0)      143 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters.req
+-rw-r--r--   0 root         (0) root         (0)      181 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-key-duplicate.authz
+-rw-r--r--   0 root         (0) root         (0)       78 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash-pointless-dot.req
+-rw-r--r--   0 root         (0) root         (0)      268 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash.sreq
+-rw-r--r--   0 root         (0) root         (0)       94 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-value-order.req
+-rw-r--r--   0 root         (0) root         (0)       85 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value.req
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query.authz
+-rw-r--r--   0 root         (0) root         (0)       79 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-relative.req
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query.authz
+-rw-r--r--   0 root         (0) root         (0)      336 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded.sreq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value.sts
+-rw-r--r--   0 root         (0) root         (0)      276 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query.sreq
+-rw-r--r--   0 root         (0) root         (0)      268 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla.sreq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slashes.sts
+-rw-r--r--   0 root         (0) root         (0)      150 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query.creq
+-rw-r--r--   0 root         (0) root         (0)      143 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-key-case.creq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters.sts
+-rw-r--r--   0 root         (0) root         (0)      269 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash-dot-slash.sreq
+-rw-r--r--   0 root         (0) root         (0)      143 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla.creq
+-rw-r--r--   0 root         (0) root         (0)      276 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value.sreq
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key.authz
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value.sts
+-rw-r--r--   0 root         (0) root         (0)      142 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash.creq
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slashes.authz
+-rw-r--r--   0 root         (0) root         (0)      124 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-nonunreserved.req
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case.sts
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-utf8.authz
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-space.sts
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash-pointless-dot.sts
+-rw-r--r--   0 root         (0) root         (0)      275 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved.creq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash.sts
+-rw-r--r--   0 root         (0) root         (0)       89 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case.req
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-relative-relative.authz
+-rw-r--r--   0 root         (0) root         (0)      145 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash-pointless-dot.creq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-unreserved.sts
+-rw-r--r--   0 root         (0) root         (0)       73 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla.req
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-space.authz
+-rw-r--r--   0 root         (0) root         (0)      350 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters.sreq
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla.authz
+-rw-r--r--   0 root         (0) root         (0)      151 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-space.creq
+-rw-r--r--   0 root         (0) root         (0)      157 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case.creq
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-space.authz
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-nonunreserved.authz
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-key-case.sts
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case.authz
+-rw-r--r--   0 root         (0) root         (0)       85 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-value-trim.req
+-rw-r--r--   0 root         (0) root         (0)      275 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key.sreq
+-rw-r--r--   0 root         (0) root         (0)      279 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value.sreq
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key.authz
+-rw-r--r--   0 root         (0) root         (0)       74 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla.req
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-value-order.sts
+-rw-r--r--   0 root         (0) root         (0)       81 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-ut8-query.req
+-rw-r--r--   0 root         (0) root         (0)      318 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-nonunreserved.sreq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query.sts
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded.sts
+-rw-r--r--   0 root         (0) root         (0)       82 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value.req
+-rw-r--r--   0 root         (0) root         (0)       85 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key.req
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-space.sts
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash-dot-slash.sts
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved.sts
+-rw-r--r--   0 root         (0) root         (0)       74 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-key-case.req
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash-dot-slash.authz
+-rw-r--r--   0 root         (0) root         (0)       86 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-relative-relative.req
+-rw-r--r--   0 root         (0) root         (0)      154 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-value-trim.creq
+-rw-r--r--   0 root         (0) root         (0)      155 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-ut8-query.creq
+-rw-r--r--   0 root         (0) root         (0)      209 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-nonunreserved.creq
+-rw-r--r--   0 root         (0) root         (0)       80 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-space.req
+-rw-r--r--   0 root         (0) root         (0)      179 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-value-order.authz
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-value-case.sts
+-rw-r--r--   0 root         (0) root         (0)      142 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query.creq
+-rw-r--r--   0 root         (0) root         (0)       73 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query.req
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-nonunreserved.sts
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key.sts
+-rw-r--r--   0 root         (0) root         (0)      110 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-key-duplicate.req
+-rw-r--r--   0 root         (0) root         (0)      308 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-key-duplicate.sreq
+-rw-r--r--   0 root         (0) root         (0)      190 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded.authz
+-rw-r--r--   0 root         (0) root         (0)      181 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-value-case.authz
+-rw-r--r--   0 root         (0) root         (0)      273 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-relative.sreq
+-rw-r--r--   0 root         (0) root         (0)      150 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value.creq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-relative.sts
+-rw-r--r--   0 root         (0) root         (0)      284 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-value-case.sreq
+-rw-r--r--   0 root         (0) root         (0)      280 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-relative-relative.sreq
+-rw-r--r--   0 root         (0) root         (0)      145 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-space.creq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key.sts
+-rw-r--r--   0 root         (0) root         (0)      179 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-value-trim.authz
+-rw-r--r--   0 root         (0) root         (0)      268 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-key-case.sreq
+-rw-r--r--   0 root         (0) root         (0)      290 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-value-order.sreq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-ut8-query.sts
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value.authz
+-rw-r--r--   0 root         (0) root         (0)      159 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-value-case.creq
+-rw-r--r--   0 root         (0) root         (0)      267 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query.sreq
+-rw-r--r--   0 root         (0) root         (0)      401 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved.sreq
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash-pointless-dot.authz
+-rw-r--r--   0 root         (0) root         (0)      274 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-space.sreq
+-rw-r--r--   0 root         (0) root         (0)       75 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slash-dot-slash.req
+-rw-r--r--   0 root         (0) root         (0)      129 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded.req
+-rw-r--r--   0 root         (0) root         (0)      207 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved.req
+-rw-r--r--   0 root         (0) root         (0)      278 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-space.sreq
+-rw-r--r--   0 root         (0) root         (0)      153 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value.creq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-key-sort.sts
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value.authz
+-rw-r--r--   0 root         (0) root         (0)       84 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla-query-space.req
+-rw-r--r--   0 root         (0) root         (0)       81 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key.req
+-rw-r--r--   0 root         (0) root         (0)      284 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-key-sort.sreq
+-rw-r--r--   0 root         (0) root         (0)      283 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case.sreq
+-rw-r--r--   0 root         (0) root         (0)      267 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla.sreq
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-ut8-query.authz
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla.sts
+-rw-r--r--   0 root         (0) root         (0)      173 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-key-duplicate.creq
+-rw-r--r--   0 root         (0) root         (0)      276 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-utf8.sreq
+-rw-r--r--   0 root         (0) root         (0)      281 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-value-trim.sreq
+-rw-r--r--   0 root         (0) root         (0)      181 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-key-sort.authz
+-rw-r--r--   0 root         (0) root         (0)      142 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-relative.creq
+-rw-r--r--   0 root         (0) root         (0)      156 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-header-value-order.creq
+-rw-r--r--   0 root         (0) root         (0)      190 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters.authz
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-key-case.authz
+-rw-r--r--   0 root         (0) root         (0)       86 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-value-case.req
+-rw-r--r--   0 root         (0) root         (0)      177 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-vanilla.authz
+-rw-r--r--   0 root         (0) root         (0)      149 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key.creq
+-rw-r--r--   0 root         (0) root         (0)      275 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-vanilla-ut8-query.sreq
+-rw-r--r--   0 root         (0) root         (0)      159 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-header-key-sort.creq
+-rw-r--r--   0 root         (0) root         (0)      138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-utf8.sts
+-rw-r--r--   0 root         (0) root         (0)       82 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-utf8.req
+-rw-r--r--   0 root         (0) root         (0)       79 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/get-slashes.req
+-rw-r--r--   0 root         (0) root         (0)      204 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded.creq
+-rw-r--r--   0 root         (0) root         (0)    43875 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/test_signers.py
+-rw-r--r--   0 root         (0) root         (0)     7115 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/auth/test_sigv4.py
+-rwxr-xr-x   0 root         (0) root         (0)    38643 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_signers.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/unit/test_auth_sigv4.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/functional/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/functional/models/
+-rw-r--r--   0 root         (0) root         (0)    77688 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/models/endpoints.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/functional/models/custom-acm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/functional/models/custom-acm/2015-12-08/
+-rw-r--r--   0 root         (0) root         (0)    57976 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/models/custom-acm/2015-12-08/service-2.json
+-rw-r--r--   0 root         (0) root         (0)      874 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/models/custom-acm/2015-12-08/waiters-2.json
+-rw-r--r--   0 root         (0) root         (0)      203 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/models/custom-acm/2015-12-08/paginators-1.json
+-rw-r--r--   0 root         (0) root         (0)       44 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/models/custom-acm/2015-12-08/examples-1.json
+-rw-r--r--   0 root         (0) root         (0)     1766 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8496 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_paginate.py
+-rwxr-xr-x   0 root         (0) root         (0)     4647 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_session.py
+-rwxr-xr-x   0 root         (0) root         (0)     8133 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_retry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/functional/leak/
+-rw-r--r--   0 root         (0) root         (0)     5529 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/leak/test_resource_leaks.py
+-rw-r--r--   0 root         (0) root         (0)      561 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/leak/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_client_metadata.py
+-rwxr-xr-x   0 root         (0) root         (0)     7146 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_loaders.py
+-rw-r--r--   0 root         (0) root         (0)    12523 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_stub.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_six_threading.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_service_names.py
+-rw-r--r--   0 root         (0) root         (0)     7370 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_waiter_config.py
+-rwxr-xr-x   0 root         (0) root         (0)    33878 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_six_imports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/functional/utils/
+-rw-r--r--   0 root         (0) root         (0)      561 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/utils/credentialprocess.py
+-rw-r--r--   0 root         (0) root         (0)     5357 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_history.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_h2_required.py
+-rw-r--r--   0 root         (0) root         (0)    26056 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_regions.py
+-rwxr-xr-x   0 root         (0) root         (0)    12258 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_paginator_config.py
+-rw-r--r--   0 root         (0) root         (0)    76799 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/functional/docs/
+-rw-r--r--   0 root         (0) root         (0)     4622 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/docs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5147 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/docs/test_shared_example_config.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/docs/test_streaming_body.py
+-rwxr-xr-x   0 root         (0) root         (0)     2875 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/docs/test_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/functional/csm/
+-rw-r--r--   0 root         (0) root         (0)      561 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/csm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/functional/csm/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/functional/csm/data/csmtest/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/tests/functional/csm/data/csmtest/2018-06-19/
+-rw-r--r--   0 root         (0) root         (0)      895 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/csm/data/csmtest/2018-06-19/service-2.json
+-rwxr-xr-x   0 root         (0) root         (0)     6821 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/csm/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)    32068 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/csm/cases.json
+-rwxr-xr-x   0 root         (0) root         (0)     1145 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_client_class_names.py
+-rw-r--r--   0 root         (0) root         (0)     3621 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_model_backcompat.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/functional/test_model_completeness.py
+-rw-r--r--   0 root         (0) root         (0)     8452 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/tests/cmd-runner
+-rw-r--r--   0 root         (0) root         (0)    10174 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/LICENSE.txt
+-rwxr-xr-x   0 root         (0) root         (0)      141 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/
+-rw-r--r--   0 root         (0) root         (0)    10428 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/discovery.py
+-rwxr-xr-x   0 root         (0) root         (0)     3508 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14409 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/stub.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/history.py
+-rw-r--r--   0 root         (0) root         (0)    11614 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/compat.py
+-rw-r--r--   0 root         (0) root         (0)    20594 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/monitoring.py
+-rwxr-xr-x   0 root         (0) root         (0)    40685 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/handlers.py
+-rwxr-xr-x   0 root         (0) root         (0)    16132 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/args.py
+-rw-r--r--   0 root         (0) root         (0)     4103 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/errorfactory.py
+-rw-r--r--   0 root         (0) root         (0)    12454 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/waiter.py
+-rw-r--r--   0 root         (0) root         (0)    36069 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/auth.py
+-rwxr-xr-x   0 root         (0) root         (0)    48086 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/session.py
+-rw-r--r--   0 root         (0) root         (0)     8424 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/regions.py
+-rw-r--r--   0 root         (0) root         (0)    23291 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/awsrequest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/
+-rw-r--r--   0 root         (0) root         (0)      125 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/special.py
+-rw-r--r--   0 root         (0) root         (0)    19618 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/standard.py
+-rw-r--r--   0 root         (0) root         (0)     4203 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/adaptive.py
+-rw-r--r--   0 root         (0) root         (0)      813 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/base.py
+-rw-r--r--   0 root         (0) root         (0)     4024 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/throttling.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/quota.py
+-rwxr-xr-x   0 root         (0) root         (0)    13785 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/retryhandler.py
+-rwxr-xr-x   0 root         (0) root         (0)    11818 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/config.py
+-rw-r--r--   0 root         (0) root         (0)    28138 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/signers.py
+-rwxr-xr-x   0 root         (0) root         (0)    17554 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/vendored/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/vendored/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30098 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/vendored/six.py
+-rw-r--r--   0 root         (0) root         (0)    27148 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/paginate.py
+-rw-r--r--   0 root         (0) root         (0)    40372 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/parsers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/data/
+-rw-r--r--   0 root         (0) root         (0)   171243 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/data/endpoints.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/data/s3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/data/s3/2006-03-01/
+-rwxr-xr-x   0 root         (0) root         (0)   486225 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/data/s3/2006-03-01/service-2.json
+-rw-r--r--   0 root         (0) root         (0)     1436 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/data/s3/2006-03-01/waiters-2.json
+-rwxr-xr-x   0 root         (0) root         (0)     1404 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/data/s3/2006-03-01/paginators-1.json
+-rw-r--r--   0 root         (0) root         (0)       44 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/data/s3/2006-03-01/examples-1.json
+-rw-r--r--   0 root         (0) root         (0)     7025 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/data/_retry.json
+-rw-r--r--   0 root         (0) root         (0)    11521 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/validate.py
+-rw-r--r--   0 root         (0) root         (0)    11508 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/httpsession.py
+-rw-r--r--   0 root         (0) root         (0)    20113 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/eventstream.py
+-rw-r--r--   0 root         (0) root         (0)    64616 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/utils.py
+-rw-r--r--   0 root         (0) root         (0)    24581 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/hooks.py
+-rwxr-xr-x   0 root         (0) root         (0)   109835 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/credentials.py
+-rw-r--r--   0 root         (0) root         (0)    17411 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/loaders.py
+-rw-r--r--   0 root         (0) root         (0)    26898 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/model.py
+-rw-r--r--   0 root         (0) root         (0)    21581 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/configprovider.py
+-rw-r--r--   0 root         (0) root         (0)     9604 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/configloader.py
+-rwxr-xr-x   0 root         (0) root         (0)    39542 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/client.py
+-rwxr-xr-x   0 root         (0) root         (0)     3416 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/translate.py
+-rw-r--r--   0 root         (0) root         (0)   271088 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/cacert.pem
+-rw-r--r--   0 root         (0) root         (0)     6456 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/
+-rw-r--r--   0 root         (0) root         (0)     1551 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7070 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/paginator.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/docstring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/bcdoc/
+-rw-r--r--   0 root         (0) root         (0)      588 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/bcdoc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11833 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/bcdoc/style.py
+-rw-r--r--   0 root         (0) root         (0)     5893 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/bcdoc/docstringparser.py
+-rw-r--r--   0 root         (0) root         (0)     7238 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/bcdoc/restdoc.py
+-rw-r--r--   0 root         (0) root         (0)     4843 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/waiter.py
+-rw-r--r--   0 root         (0) root         (0)    11565 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/method.py
+-rwxr-xr-x   0 root         (0) root         (0)     3717 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/service.py
+-rw-r--r--   0 root         (0) root         (0)     7176 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8759 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/example.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/client.py
+-rw-r--r--   0 root         (0) root         (0)     9338 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/sharedexample.py
+-rw-r--r--   0 root         (0) root         (0)     9569 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/params.py
+-rw-r--r--   0 root         (0) root         (0)     4998 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/shape.py
+-rwxr-xr-x   0 root         (0) root         (0)    12616 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/endpoint.py
+-rw-r--r--   0 root         (0) root         (0)    29839 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/ibm_botocore/serialize.py
+-rwxr-xr-x   0 root         (0) root         (0)     1358 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/docs/source/
+-rwxr-xr-x   0 root         (0) root         (0)     8625 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/docs/source/conf.py
+-rwxr-xr-x   0 root         (0) root         (0)     8369 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/docs/source/client_upgrades.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/docs/source/_static/
+-rwxr-xr-x   0 root         (0) root         (0)      717 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/docs/source/_static/404.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/docs/source/reference/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:41.000000 ibm-cos-sdk-core-2.9.0/docs/source/reference/services/
+-rwxr-xr-x   0 root         (0) root         (0)   214436 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/docs/source/reference/services/s3.rst
+-rwxr-xr-x   0 root         (0) root         (0)      160 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/docs/source/reference/config.rst
+-rwxr-xr-x   0 root         (0) root         (0)      105 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/docs/source/reference/index.rst
+-rwxr-xr-x   0 root         (0) root         (0)      511 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/docs/source/index.rst
+-rwxr-xr-x   0 root         (0) root         (0)     5109 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/docs/make.bat
+-rwxr-xr-x   0 root         (0) root         (0)     5581 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/docs/Makefile
+-rwxr-xr-x   0 root         (0) root         (0)      187 2020-12-14 21:54:40.000000 ibm-cos-sdk-core-2.9.0/requirements.txt
```

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_cos_sdk_core.egg-info/PKG-INFO` & `ibm-cos-sdk-core-2.9.0/ibm_cos_sdk_core.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: ibm-cos-sdk-core
-Version: 2.8.0
+Version: 2.9.0
 Summary: Low-level, data-driven core of IBM SDK for Python
 Home-page: https://github.com/ibm/ibm-cos-sdk-python-core
 Author: IBM
 License: Apache License 2.0
 Description: # `ibm-cos-sdk-python-core`
         
-        A low-level interface to IBM Cloud Object Storage based on the
-        `ibm_botocore` package. This core package is the foundation for the
-        [`ibm-cos-sdk-python`](https://github.com/ibm/ibm-cos-sdk-python) package.
+        A low-level interface to IBM Cloud Object Storage based on the `ibm_botocore` package. This core package is the foundation for the [`ibm-cos-sdk-python`](https://github.com/ibm/ibm-cos-sdk-python) package.
         
         ## Documentation
         
-        Documentation for `ibm-cos-sdk-python-core` can be found
-        [here](https://ibm.github.io/ibm-cos-sdk-python-core/).
+        Documentation for `ibm-cos-sdk-python-core` can be found [here](https://ibm.github.io/ibm-cos-sdk-python-core/).
         
         ## Getting Help
         
-        Feel free to use GitHub issues for tracking bugs and feature requests,
-        but for help please use one of the following resources:
+        Feel free to use GitHub issues for tracking bugs and feature requests, but for help please use one of the following resources:
         
         * Ask a question on [Stack Overflow](https://stackoverflow.com/) and tag it with `ibm` and `object-storage`.
         * Open a support ticket with [IBM Cloud Support](https://cloud.ibm.com/unifiedsupport/supportcenter/)
         * If it turns out that you may have found a bug, please [open an issue](https://github.com/ibm/ibm-cos-sdk-python-core/issues/new)
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_cos_sdk_core.egg-info/SOURCES.txt` & `ibm-cos-sdk-core-2.9.0/ibm_cos_sdk_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,19 +64,17 @@
 ibm_botocore/docs/params.py
 ibm_botocore/docs/service.py
 ibm_botocore/docs/shape.py
 ibm_botocore/docs/sharedexample.py
 ibm_botocore/docs/utils.py
 ibm_botocore/docs/waiter.py
 ibm_botocore/docs/bcdoc/__init__.py
-ibm_botocore/docs/bcdoc/docevents.py
 ibm_botocore/docs/bcdoc/docstringparser.py
 ibm_botocore/docs/bcdoc/restdoc.py
 ibm_botocore/docs/bcdoc/style.py
-ibm_botocore/docs/bcdoc/textwriter.py
 ibm_botocore/retries/__init__.py
 ibm_botocore/retries/adaptive.py
 ibm_botocore/retries/base.py
 ibm_botocore/retries/bucket.py
 ibm_botocore/retries/quota.py
 ibm_botocore/retries/special.py
 ibm_botocore/retries/standard.py
```

### Comparing `ibm-cos-sdk-core-2.8.0/PKG-INFO` & `ibm-cos-sdk-core-2.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: ibm-cos-sdk-core
-Version: 2.8.0
+Version: 2.9.0
 Summary: Low-level, data-driven core of IBM SDK for Python
 Home-page: https://github.com/ibm/ibm-cos-sdk-python-core
 Author: IBM
 License: Apache License 2.0
 Description: # `ibm-cos-sdk-python-core`
         
-        A low-level interface to IBM Cloud Object Storage based on the
-        `ibm_botocore` package. This core package is the foundation for the
-        [`ibm-cos-sdk-python`](https://github.com/ibm/ibm-cos-sdk-python) package.
+        A low-level interface to IBM Cloud Object Storage based on the `ibm_botocore` package. This core package is the foundation for the [`ibm-cos-sdk-python`](https://github.com/ibm/ibm-cos-sdk-python) package.
         
         ## Documentation
         
-        Documentation for `ibm-cos-sdk-python-core` can be found
-        [here](https://ibm.github.io/ibm-cos-sdk-python-core/).
+        Documentation for `ibm-cos-sdk-python-core` can be found [here](https://ibm.github.io/ibm-cos-sdk-python-core/).
         
         ## Getting Help
         
-        Feel free to use GitHub issues for tracking bugs and feature requests,
-        but for help please use one of the following resources:
+        Feel free to use GitHub issues for tracking bugs and feature requests, but for help please use one of the following resources:
         
         * Ask a question on [Stack Overflow](https://stackoverflow.com/) and tag it with `ibm` and `object-storage`.
         * Open a support ticket with [IBM Cloud Support](https://cloud.ibm.com/unifiedsupport/supportcenter/)
         * If it turns out that you may have found a bug, please [open an issue](https://github.com/ibm/ibm-cos-sdk-python-core/issues/new)
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ibm-cos-sdk-core-2.8.0/README.md` & `ibm-cos-sdk-core-2.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # `ibm-cos-sdk-python-core`
 
-A low-level interface to IBM Cloud Object Storage based on the
-`ibm_botocore` package. This core package is the foundation for the
-[`ibm-cos-sdk-python`](https://github.com/ibm/ibm-cos-sdk-python) package.
+A low-level interface to IBM Cloud Object Storage based on the `ibm_botocore` package. This core package is the foundation for the [`ibm-cos-sdk-python`](https://github.com/ibm/ibm-cos-sdk-python) package.
 
 ## Documentation
 
-Documentation for `ibm-cos-sdk-python-core` can be found
-[here](https://ibm.github.io/ibm-cos-sdk-python-core/).
+Documentation for `ibm-cos-sdk-python-core` can be found [here](https://ibm.github.io/ibm-cos-sdk-python-core/).
 
 ## Getting Help
 
-Feel free to use GitHub issues for tracking bugs and feature requests,
-but for help please use one of the following resources:
+Feel free to use GitHub issues for tracking bugs and feature requests, but for help please use one of the following resources:
 
 * Ask a question on [Stack Overflow](https://stackoverflow.com/) and tag it with `ibm` and `object-storage`.
 * Open a support ticket with [IBM Cloud Support](https://cloud.ibm.com/unifiedsupport/supportcenter/)
 * If it turns out that you may have found a bug, please [open an issue](https://github.com/ibm/ibm-cos-sdk-python-core/issues/new)
```

### Comparing `ibm-cos-sdk-core-2.8.0/tests/__init__.py` & `ibm-cos-sdk-core-2.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_waiters.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_waiters.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_kinesis.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_kinesis.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_apigateway.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/__init__.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_ec2.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_ec2.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_rds.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_rds.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_elastictranscoder.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_elastictranscoder.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_utils.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_session.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_session.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_cognito_identity.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_cognito_identity.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_route53.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_route53.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_loaders.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_loaders.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_glacier.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_glacier.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_sts.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_sts.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_emr.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_emr.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_credentials.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_credentials.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_smoke.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_smoke.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_client_http.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_client_http.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_client.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_cloudformation.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_cloudformation.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/integration/test_s3.py` & `ibm-cos-sdk-core-2.9.0/tests/integration/test_s3.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/acceptance/features/environment.py` & `ibm-cos-sdk-core-2.9.0/tests/acceptance/features/environment.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/acceptance/features/steps/base.py` & `ibm-cos-sdk-core-2.9.0/tests/acceptance/features/steps/base.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/support/support.feature` & `ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/support/support.feature`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/autoscaling/autoscaling.feature` & `ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/autoscaling/autoscaling.feature`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/acceptance/features/smoke/cognitoidentity/cognitoidentity.feature` & `ibm-cos-sdk-core-2.9.0/tests/acceptance/features/smoke/cognitoidentity/cognitoidentity.feature`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_waiters.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_waiters.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_protocols.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_protocols.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_errorfactory.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_errorfactory.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/cfg/aws_config_badbytes` & `ibm-cos-sdk-core-2.9.0/tests/unit/cfg/aws_config_badbytes`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/__init__.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_http_session.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_http_session.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_eventstream.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_eventstream.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_hooks.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_hooks.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_paginate.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_retryhandler.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/test_response_parsing.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/test_response_parsing.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/__init__.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-objects.xml` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-objects.xml`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-object-versions.xml` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-object-versions.xml`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-buckets.json` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-buckets.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.json` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.xml` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.xml`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.xml` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.xml`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-buckets.xml` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-buckets.xml`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-object-versions.json` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-object-versions.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-list-objects.json` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-list-objects.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.xml` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.xml`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.xml` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.xml`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/response_parsing/README.rst` & `ibm-cos-sdk-core-2.9.0/tests/unit/response_parsing/README.rst`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_compat.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_compat.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_http_client_exception_mapping.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_http_client_exception_mapping.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_model.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_utils.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_parsers.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_session.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_translate.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_translate.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_args.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_args.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_session_legacy.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_session_legacy.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_loaders.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_response.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_response.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_stub.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_stub.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_serialize.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_serialize.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_handlers.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_handlers.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_s3_addressing.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_s3_addressing.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_monitoring.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_endpoint.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_exceptions.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_configloader.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_configloader.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_credentials.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_validate.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_awsrequest.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_awsrequest.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_idempotency.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_idempotency.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_config_provider.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_config_provider.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_client.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_history.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_history.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_regions.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_regions.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/auth/__init__.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/auth/test_signers.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/auth/test_signers.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/auth/test_sigv4.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/auth/test_sigv4.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_signers.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/unit/test_auth_sigv4.py` & `ibm-cos-sdk-core-2.9.0/tests/unit/test_auth_sigv4.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/models/endpoints.json` & `ibm-cos-sdk-core-2.9.0/tests/functional/models/endpoints.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/models/custom-acm/2015-12-08/service-2.json` & `ibm-cos-sdk-core-2.9.0/tests/functional/models/custom-acm/2015-12-08/service-2.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/models/custom-acm/2015-12-08/waiters-2.json` & `ibm-cos-sdk-core-2.9.0/tests/functional/models/custom-acm/2015-12-08/waiters-2.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/__init__.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_paginate.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_paginate.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_session.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_session.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_retry.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_retry.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/leak/test_resource_leaks.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/leak/test_resource_leaks.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/leak/__init__.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/leak/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_client_metadata.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_client_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_endpoints.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_loaders.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_loaders.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_stub.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_stub.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_six_threading.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_six_threading.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_service_names.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_service_names.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_waiter_config.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_waiter_config.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_credentials.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_credentials.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_six_imports.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_six_imports.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/utils/__init__.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/utils/credentialprocess.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/utils/credentialprocess.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_history.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_history.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_h2_required.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_h2_required.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_regions.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_regions.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_paginator_config.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_paginator_config.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_s3.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_s3.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/docs/__init__.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/docs/test_shared_example_config.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/docs/test_shared_example_config.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/docs/test_streaming_body.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/docs/test_streaming_body.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/docs/test_s3.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/docs/test_s3.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/csm/__init__.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/csm/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/csm/data/csmtest/2018-06-19/service-2.json` & `ibm-cos-sdk-core-2.9.0/tests/functional/csm/data/csmtest/2018-06-19/service-2.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/csm/test_monitoring.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/csm/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/csm/cases.json` & `ibm-cos-sdk-core-2.9.0/tests/functional/csm/cases.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_client_class_names.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_client_class_names.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_model_backcompat.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_model_backcompat.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/functional/test_model_completeness.py` & `ibm-cos-sdk-core-2.9.0/tests/functional/test_model_completeness.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/tests/cmd-runner` & `ibm-cos-sdk-core-2.9.0/tests/cmd-runner`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/LICENSE.txt` & `ibm-cos-sdk-core-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/discovery.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/discovery.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/__init__.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # language governing permissions and limitations under the License.
 
 import os
 import re
 import logging
 
 __author__ = 'IBM'
-__version__ = '2.8.0'
+__version__ = '2.9.0'
 
 
 class NullHandler(logging.Handler):
     def emit(self, record):
         pass
 
 # Configure default logger to do nothing
```

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/stub.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/stub.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/history.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/history.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/compat.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/compat.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/monitoring.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/monitoring.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/handlers.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/handlers.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/args.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/args.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/errorfactory.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/errorfactory.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/waiter.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/waiter.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/auth.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/auth.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/session.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/session.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/regions.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/regions.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/awsrequest.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/awsrequest.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/special.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/special.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/standard.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/standard.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/adaptive.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/adaptive.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/base.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/base.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/bucket.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/bucket.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/throttling.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/throttling.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/retries/quota.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/retries/quota.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/retryhandler.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/retryhandler.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/config.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/config.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/signers.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/signers.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/exceptions.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/exceptions.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/vendored/six.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/vendored/six.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/paginate.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/paginate.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/parsers.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/parsers.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/data/endpoints.json` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/data/endpoints.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/data/s3/2006-03-01/service-2.json` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/data/s3/2006-03-01/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875979912451145%*

 * *Differences: {"'operations'": "{'GetBucketInventoryConfiguration': {'documentation': '<p>Returns an inventory "*

 * *                 'configuration (identified by the inventory configuration ID) from the '*

 * *                 'bucket.</p> <p>To use this operation, you must have permissions to perform the '*

 * *                 '<code>s3:GetInventoryConfiguration</code> action. The bucket owner has this '*

 * *                 'permission by default and can grant this permission to others. For more '*

 * *                 'information about  […]*

```diff
@@ -271,14 +271,29 @@
                 "shape": "DeleteObjectRequest"
             },
             "name": "DeleteObject",
             "output": {
                 "shape": "DeleteObjectOutput"
             }
         },
+        "DeleteObjectTagging": {
+            "documentation": "<p>Removes the entire tag set from the specified object. For more information about managing object tags, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/object-tagging.html\"> Object Tagging</a>.</p> <p>To use this operation, you must have permission to perform the <code>s3:DeleteObjectTagging</code> action.</p> <p>To delete tags of a specific object version, add the <code>versionId</code> query parameter in the request. You will need permission for the <code>s3:DeleteObjectVersionTagging</code> action.</p> <p>The following operations are related to <code>DeleteBucketMetricsConfiguration</code>:</p> <ul> <li> <p> <a>PutObjectTagging</a> </p> </li> <li> <p> <a>GetObjectTagging</a> </p> </li> </ul>",
+            "http": {
+                "method": "DELETE",
+                "requestUri": "/{Bucket}/{Key+}?tagging",
+                "responseCode": 204
+            },
+            "input": {
+                "shape": "DeleteObjectTaggingRequest"
+            },
+            "name": "DeleteObjectTagging",
+            "output": {
+                "shape": "DeleteObjectTaggingOutput"
+            }
+        },
         "DeleteObjects": {
             "__documentationUrl": "http://docs.amazonwebservices.com/AmazonS3/latest/API/multiobjectdeleteapi.html",
             "alias": "DeleteMultipleObjects",
             "documentation": "<p>This operation enables you to delete multiple objects from a bucket using a single HTTP request. If you know the object keys that you want to delete, then this operation provides a suitable alternative to sending individual delete requests, reducing per-request overhead.</p> <p>The request contains a list of up to 1000 keys that you want to delete. In the XML, you provide the object key names, and optionally, version IDs if you want to delete a specific version of the object from a versioning-enabled bucket. For each key, Amazon S3 performs a delete operation and returns the result of that delete, success, or failure, in the response. Note that if the object specified in the request is not found, Amazon S3 returns the result as deleted.</p> <p> The operation supports two modes for the response: verbose and quiet. By default, the operation uses verbose mode in which the response includes the result of deletion of each key in your request. In quiet mode the response includes only keys where the delete operation encountered an error. For a successful deletion, the operation does not return any information about the delete in the response body.</p> <p>When performing this operation on an MFA Delete enabled bucket, that attempts to delete any versioned objects, you must include an MFA token. If you do not provide one, the entire request will fail, even if there are non-versioned objects you are trying to delete. If you provide an invalid token, whether there are versioned keys in the request or not, the entire Multi-Object Delete request will fail. For information about MFA Delete, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/Versioning.html#MultiFactorAuthenticationDelete\"> MFA Delete</a>.</p> <p>Finally, the Content-MD5 header is required for all Multi-Object Delete requests. Amazon S3 uses the header value to ensure that your request body has not been altered in transit.</p> <p>The following operations are related to <code>DeleteObjects</code>:</p> <ul> <li> <p> <a>CreateMultipartUpload</a> </p> </li> <li> <p> <a>UploadPart</a> </p> </li> <li> <p> <a>CompleteMultipartUpload</a> </p> </li> <li> <p> <a>ListParts</a> </p> </li> <li> <p> <a>AbortMultipartUpload</a> </p> </li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/{Bucket}?delete"
@@ -287,14 +302,26 @@
                 "shape": "DeleteObjectsRequest"
             },
             "name": "DeleteObjects",
             "output": {
                 "shape": "DeleteObjectsOutput"
             }
         },
+        "DeletePublicAccessBlock": {
+            "documentation": "<p>Removes the <code>PublicAccessBlock</code> configuration for an Amazon S3 bucket. To use this operation, you must have the <code>s3:PutBucketPublicAccessBlock</code> permission. For more information about permissions, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/using-with-s3-actions.html#using-with-s3-actions-related-to-bucket-subresources\">Permissions Related to Bucket Subresource Operations</a> and <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-access-control.html\">Managing Access Permissions to Your Amazon S3 Resources</a>.</p> <p>The following operations are related to <code>DeleteBucketMetricsConfiguration</code>:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/access-control-block-public-access.html\">Using Amazon S3 Block Public Access</a> </p> </li> <li> <p> <a>GetPublicAccessBlock</a> </p> </li> <li> <p> <a>PutPublicAccessBlock</a> </p> </li> <li> <p> <a>GetBucketPolicyStatus</a> </p> </li> </ul>",
+            "http": {
+                "method": "DELETE",
+                "requestUri": "/{Bucket}?publicAccessBlock",
+                "responseCode": 204
+            },
+            "input": {
+                "shape": "DeletePublicAccessBlockRequest"
+            },
+            "name": "DeletePublicAccessBlock"
+        },
         "ExtendObjectRetention": {
             "documentation": "This implementation of the POST operation uses the extendRetention sub-resource to extend the retention period of a protected object in a protected vault.",
             "http": {
                 "method": "POST",
                 "requestUri": "/{Bucket}/{Key+}?extendRetention"
             },
             "input": {
@@ -372,15 +399,15 @@
             },
             "name": "GetBucketCors",
             "output": {
                 "shape": "GetBucketCorsOutput"
             }
         },
         "GetBucketInventoryConfiguration": {
-            "documentation": "Returns an inventory configuration (identified by the inventory ID) from the bucket.",
+            "documentation": "<p>Returns an inventory configuration (identified by the inventory configuration ID) from the bucket.</p> <p>To use this operation, you must have permissions to perform the <code>s3:GetInventoryConfiguration</code> action. The bucket owner has this permission by default and can grant this permission to others. For more information about permissions, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/using-with-s3-actions.html#using-with-s3-actions-related-to-bucket-subresources\">Permissions Related to Bucket Subresource Operations</a> and <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-access-control.html\">Managing Access Permissions to Your Amazon S3 Resources</a>.</p> <p>For information about the Amazon S3 inventory feature, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/storage-inventory.html\">Amazon S3 Inventory</a>.</p> <p>The following operations are related to <code>GetBucketInventoryConfiguration</code>:</p> <ul> <li> <p> <a>DeleteBucketInventoryConfiguration</a> </p> </li> <li> <p> <a>ListBucketInventoryConfigurations</a> </p> </li> <li> <p> <a>PutBucketInventoryConfiguration</a> </p> </li> </ul>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?inventory"
             },
             "input": {
                 "shape": "GetBucketInventoryConfigurationRequest"
             },
@@ -415,15 +442,15 @@
             },
             "name": "GetBucketLocation",
             "output": {
                 "shape": "GetBucketLocationOutput"
             }
         },
         "GetBucketMetricsConfiguration": {
-            "documentation": "Gets a metrics configuration (specified by the metrics configuration ID) from the bucket.",
+            "documentation": "<p>Gets a metrics configuration (specified by the metrics configuration ID) from the bucket. Note that this doesn't include the daily storage metrics.</p> <p> To use this operation, you must have permissions to perform the <code>s3:GetMetricsConfiguration</code> action. The bucket owner has this permission by default. The bucket owner can grant this permission to others. For more information about permissions, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/using-with-s3-actions.html#using-with-s3-actions-related-to-bucket-subresources\">Permissions Related to Bucket Subresource Operations</a> and <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-access-control.html\">Managing Access Permissions to Your Amazon S3 Resources</a>.</p> <p> For information about CloudWatch request metrics for Amazon S3, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/cloudwatch-monitoring.html\">Monitoring Metrics with Amazon CloudWatch</a>.</p> <p>The following operations are related to <code>GetBucketMetricsConfiguration</code>:</p> <ul> <li> <p> <a>PutBucketMetricsConfiguration</a> </p> </li> <li> <p> <a>DeleteBucketMetricsConfiguration</a> </p> </li> <li> <p> <a>ListBucketMetricsConfigurations</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/cloudwatch-monitoring.html\">Monitoring Metrics with Amazon CloudWatch</a> </p> </li> </ul>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?metrics"
             },
             "input": {
                 "shape": "GetBucketMetricsConfigurationRequest"
             },
@@ -540,29 +567,57 @@
                 "shape": "GetObjectAclRequest"
             },
             "name": "GetObjectAcl",
             "output": {
                 "shape": "GetObjectAclOutput"
             }
         },
+        "GetObjectTagging": {
+            "documentation": "<p>Returns the tag-set of an object. You send the GET request against the tagging subresource associated with the object.</p> <p>To use this operation, you must have permission to perform the <code>s3:GetObjectTagging</code> action. By default, the GET operation returns information about current version of an object. For a versioned bucket, you can have multiple versions of an object in your bucket. To retrieve tags of any other version, use the versionId query parameter. You also need permission for the <code>s3:GetObjectVersionTagging</code> action.</p> <p> By default, the bucket owner has this permission and can grant this permission to others.</p> <p> For information about the Amazon S3 object tagging feature, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/object-tagging.html\">Object Tagging</a>.</p> <p>The following operation is related to <code>GetObjectTagging</code>:</p> <ul> <li> <p> <a>PutObjectTagging</a> </p> </li> </ul>",
+            "http": {
+                "method": "GET",
+                "requestUri": "/{Bucket}/{Key+}?tagging"
+            },
+            "input": {
+                "shape": "GetObjectTaggingRequest"
+            },
+            "name": "GetObjectTagging",
+            "output": {
+                "shape": "GetObjectTaggingOutput"
+            }
+        },
         "GetObjectTorrent": {
             "__documentationUrl": "http://docs.amazonwebservices.com/AmazonS3/latest/API/RESTObjectGETtorrent.html",
-            "documentation": "Return torrent files from a bucket.",
+            "documentation": "<p>Return torrent files from a bucket. BitTorrent can save you bandwidth when you're distributing large files. For more information about BitTorrent, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/S3Torrent.html\">Amazon S3 Torrent</a>.</p> <note> <p>You can get torrent only for objects that are less than 5 GB in size and that are not encrypted using server-side encryption with customer-provided encryption key.</p> </note> <p>To use GET, you must have READ access to the object.</p> <p>The following operation is related to <code>GetObjectTorrent</code>:</p> <ul> <li> <p> <a>GetObject</a> </p> </li> </ul>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}/{Key+}?torrent"
             },
             "input": {
                 "shape": "GetObjectTorrentRequest"
             },
             "name": "GetObjectTorrent",
             "output": {
                 "shape": "GetObjectTorrentOutput"
             }
         },
+        "GetPublicAccessBlock": {
+            "documentation": "<p>Retrieves the <code>PublicAccessBlock</code> configuration for an Amazon S3 bucket. To use this operation, you must have the <code>s3:GetBucketPublicAccessBlock</code> permission. For more information about Amazon S3 permissions, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/using-with-s3-actions.html\">Specifying Permissions in a Policy</a>.</p> <important> <p>When Amazon S3 evaluates the <code>PublicAccessBlock</code> configuration for a bucket or an object, it checks the <code>PublicAccessBlock</code> configuration for both the bucket (or the bucket that contains the object) and the bucket owner's account. If the <code>PublicAccessBlock</code> settings are different between the bucket and the account, Amazon S3 uses the most restrictive combination of the bucket-level and account-level settings.</p> </important> <p>For more information about when Amazon S3 considers a bucket or an object public, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/access-control-block-public-access.html#access-control-block-public-access-policy-status\">The Meaning of \"Public\"</a>.</p> <p>The following operations are related to <code>GetPublicAccessBlock</code>:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/access-control-block-public-access.html\">Using Amazon S3 Block Public Access</a> </p> </li> <li> <p> <a>PutPublicAccessBlock</a> </p> </li> <li> <p> <a>GetPublicAccessBlock</a> </p> </li> <li> <p> <a>DeletePublicAccessBlock</a> </p> </li> </ul>",
+            "http": {
+                "method": "GET",
+                "requestUri": "/{Bucket}?publicAccessBlock"
+            },
+            "input": {
+                "shape": "GetPublicAccessBlockRequest"
+            },
+            "name": "GetPublicAccessBlock",
+            "output": {
+                "shape": "GetPublicAccessBlockOutput"
+            }
+        },
         "HeadBucket": {
             "__documentationUrl": "http://docs.amazonwebservices.com/AmazonS3/latest/API/RESTBucketHEAD.html",
             "documentation": "<p>This operation is useful to determine if a bucket exists and you have permission to access it. The operation returns a <code>200 OK</code> if the bucket exists and you have permission to access it. Otherwise, the operation might return responses such as <code>404 Not Found</code> and <code>403 Forbidden</code>. </p> <p>To use this operation, you must have permissions to perform the <code>s3:ListBucket</code> action. The bucket owner has this permission by default and can grant this permission to others. For more information about permissions, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/using-with-s3-actions.html#using-with-s3-actions-related-to-bucket-subresources\">Permissions Related to Bucket Subresource Operations</a> and <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-access-control.html\">Managing Access Permissions to Your Amazon S3 Resources</a>.</p>",
             "errors": [
                 {
                     "shape": "NoSuchBucket"
                 }
@@ -942,14 +997,39 @@
                 "shape": "PutObjectAclRequest"
             },
             "name": "PutObjectAcl",
             "output": {
                 "shape": "PutObjectAclOutput"
             }
         },
+        "PutObjectTagging": {
+            "documentation": "<p>Sets the supplied tag-set to an object that already exists in a bucket</p> <p>A tag is a key-value pair. You can associate tags with an object by sending a PUT request against the tagging subresource that is associated with the object. You can retrieve tags by sending a GET request. For more information, see <a>GetObjectTagging</a>.</p> <p>For tagging-related restrictions related to characters and encodings, see <a href=\"https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/allocation-tag-restrictions.html\">Tag Restrictions</a>. Note that Amazon S3 limits the maximum number of tags to 10 tags per object.</p> <p>To use this operation, you must have permission to perform the <code>s3:PutObjectTagging</code> action. By default, the bucket owner has this permission and can grant this permission to others.</p> <p>To put tags of any other version, use the <code>versionId</code> query parameter. You also need permission for the <code>s3:PutObjectVersionTagging</code> action.</p> <p>For information about the Amazon S3 object tagging feature, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/object-tagging.html\">Object Tagging</a>.</p> <p class=\"title\"> <b>Special Errors</b> </p> <ul> <li> <p class=\"title\"> <b/> </p> <ul> <li> <p> <i>Code: InvalidTagError </i> </p> </li> <li> <p> <i>Cause: The tag provided was not a valid tag. This error can occur if the tag did not pass input validation. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/object-tagging.html\">Object Tagging</a>.</i> </p> </li> </ul> </li> <li> <p class=\"title\"> <b/> </p> <ul> <li> <p> <i>Code: MalformedXMLError </i> </p> </li> <li> <p> <i>Cause: The XML provided does not match the schema.</i> </p> </li> </ul> </li> <li> <ul> <li> <p> <i>Code: OperationAbortedError </i> </p> </li> <li> <p> <i>Cause: A conflicting conditional operation is currently in progress against this resource. Please try again.</i> </p> </li> </ul> </li> <li> <ul> <li> <p> <i>Code: InternalError</i> </p> </li> <li> <p> <i>Cause: The service was unable to apply the provided tag to the object.</i> </p> </li> </ul> </li> </ul> <p class=\"title\"> <b>Related Resources</b> </p> <ul> <li> <p> <a>GetObjectTagging</a> </p> </li> </ul>",
+            "http": {
+                "method": "PUT",
+                "requestUri": "/{Bucket}/{Key+}?tagging"
+            },
+            "input": {
+                "shape": "PutObjectTaggingRequest"
+            },
+            "name": "PutObjectTagging",
+            "output": {
+                "shape": "PutObjectTaggingOutput"
+            }
+        },
+        "PutPublicAccessBlock": {
+            "documentation": "<p>Creates or modifies the <code>PublicAccessBlock</code> configuration for an Amazon S3 bucket. To use this operation, you must have the <code>s3:PutBucketPublicAccessBlock</code> permission. For more information about Amazon S3 permissions, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/using-with-s3-actions.html\">Specifying Permissions in a Policy</a>.</p> <important> <p>When Amazon S3 evaluates the <code>PublicAccessBlock</code> configuration for a bucket or an object, it checks the <code>PublicAccessBlock</code> configuration for both the bucket (or the bucket that contains the object) and the bucket owner's account. If the <code>PublicAccessBlock</code> configurations are different between the bucket and the account, Amazon S3 uses the most restrictive combination of the bucket-level and account-level settings.</p> </important> <p>For more information about when Amazon S3 considers a bucket or an object public, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/access-control-block-public-access.html#access-control-block-public-access-policy-status\">The Meaning of \"Public\"</a>.</p> <p class=\"title\"> <b>Related Resources</b> </p> <ul> <li> <p> <a>GetPublicAccessBlock</a> </p> </li> <li> <p> <a>DeletePublicAccessBlock</a> </p> </li> <li> <p> <a>GetBucketPolicyStatus</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/access-control-block-public-access.html\">Using Amazon S3 Block Public Access</a> </p> </li> </ul>",
+            "http": {
+                "method": "PUT",
+                "requestUri": "/{Bucket}?publicAccessBlock"
+            },
+            "input": {
+                "shape": "PutPublicAccessBlockRequest"
+            },
+            "name": "PutPublicAccessBlock"
+        },
         "RestoreObject": {
             "__documentationUrl": "http://docs.amazonwebservices.com/AmazonS3/latest/API/RESTObjectRestore.html",
             "_output": {
                 "shape": "RestoreObjectOutput"
             },
             "alias": "PostObjectRestore",
             "documentation": "<p>Restores an archived copy of an object back into Amazon S3</p> <p>This operation performs the following types of requests: </p> <ul> <li> <p> <code>select</code> - Perform a select query on an archived object</p> </li> <li> <p> <code>restore an archive</code> - Restore an archived object</p> </li> </ul> <p>To use this operation, you must have permissions to perform the <code>s3:RestoreObject</code> and <code>s3:GetObject</code> actions. The bucket owner has this permission by default and can grant this permission to others. For more information about permissions, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/using-with-s3-actions.html#using-with-s3-actions-related-to-bucket-subresources\">Permissions Related to Bucket Subresource Operations</a> and <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-access-control.html\">Managing Access Permissions to Your Amazon S3 Resources</a> in the <i>Amazon Simple Storage Service Developer Guide</i>.</p> <p> <b>Querying Archives with Select Requests</b> </p> <p>You use a select type of request to perform SQL queries on archived objects. The archived objects that are being queried by the select request must be formatted as uncompressed comma-separated values (CSV) files. You can run queries and custom analytics on your archived data without having to restore your data to a hotter Amazon S3 tier. For an overview about select requests, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/querying-glacier-archives.html\">Querying Archived Objects</a> in the <i>Amazon Simple Storage Service Developer Guide</i>.</p> <p>When making a select request, do the following:</p> <ul> <li> <p>Define an output location for the select query's output. This must be an Amazon S3 bucket in the same AWS Region as the bucket that contains the archive object that is being queried. The AWS account that initiates the job must have permissions to write to the S3 bucket. You can specify the storage class and encryption for the output objects stored in the bucket. For more information about output, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/querying-glacier-archives.html\">Querying Archived Objects</a> in the <i>Amazon Simple Storage Service Developer Guide</i>.</p> <p>For more information about the <code>S3</code> structure in the request body, see the following:</p> <ul> <li> <p> <a>PutObject</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/S3_ACLs_UsingACLs.html\">Managing Access with ACLs</a> in the <i>Amazon Simple Storage Service Developer Guide</i> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/serv-side-encryption.html\">Protecting Data Using Server-Side Encryption</a> in the <i>Amazon Simple Storage Service Developer Guide</i> </p> </li> </ul> </li> <li> <p>Define the SQL expression for the <code>SELECT</code> type of restoration for your query in the request body's <code>SelectParameters</code> structure. You can use expressions like the following examples.</p> <ul> <li> <p>The following expression returns all records from the specified object.</p> <p> <code>SELECT * FROM Object</code> </p> </li> <li> <p>Assuming that you are not using any headers for data stored in the object, you can specify columns with positional headers.</p> <p> <code>SELECT s._1, s._2 FROM Object s WHERE s._3 &gt; 100</code> </p> </li> <li> <p>If you have headers and you set the <code>fileHeaderInfo</code> in the <code>CSV</code> structure in the request body to <code>USE</code>, you can specify headers in the query. (If you set the <code>fileHeaderInfo</code> field to <code>IGNORE</code>, the first row is skipped for the query.) You cannot mix ordinal positions with header column names. </p> <p> <code>SELECT s.Id, s.FirstName, s.SSN FROM S3Object s</code> </p> </li> </ul> </li> </ul> <p>For more information about using SQL with Glacier Select restore, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-glacier-select-sql-reference.html\">SQL Reference for Amazon S3 Select and Glacier Select</a> in the <i>Amazon Simple Storage Service Developer Guide</i>. </p> <p>When making a select request, you can also do the following:</p> <ul> <li> <p>To expedite your queries, specify the <code>Expedited</code> tier. For more information about tiers, see \"Restoring Archives,\" later in this topic.</p> </li> <li> <p>Specify details about the data serialization format of both the input object that is being queried and the serialization of the CSV-encoded query results.</p> </li> </ul> <p>The following are additional important facts about the select feature:</p> <ul> <li> <p>The output results are new Amazon S3 objects. Unlike archive retrievals, they are stored until explicitly deleted-manually or through a lifecycle policy.</p> </li> <li> <p>You can issue more than one select request on the same Amazon S3 object. Amazon S3 doesn't deduplicate requests, so avoid issuing duplicate requests.</p> </li> <li> <p> Amazon S3 accepts a select request even if the object has already been restored. A select request doesn\u2019t return error response <code>409</code>.</p> </li> </ul> <p> <b>Restoring Archives</b> </p> <p>Objects in the GLACIER and DEEP_ARCHIVE storage classes are archived. To access an archived object, you must first initiate a restore request. This restores a temporary copy of the archived object. In a restore request, you specify the number of days that you want the restored copy to exist. After the specified period, Amazon S3 deletes the temporary copy but the object remains archived in the GLACIER or DEEP_ARCHIVE storage class that object was restored from. </p> <p>To restore a specific object version, you can provide a version ID. If you don't provide a version ID, Amazon S3 restores the current version.</p> <p>The time it takes restore jobs to finish depends on which storage class the object is being restored from and which data access tier you specify. </p> <p>When restoring an archived object (or using a select request), you can specify one of the following data access tier options in the <code>Tier</code> element of the request body: </p> <ul> <li> <p> <b> <code>Expedited</code> </b> - Expedited retrievals allow you to quickly access your data stored in the GLACIER storage class when occasional urgent requests for a subset of archives are required. For all but the largest archived objects (250 MB+), data accessed using Expedited retrievals are typically made available within 1\u20135 minutes. Provisioned capacity ensures that retrieval capacity for Expedited retrievals is available when you need it. Expedited retrievals and provisioned capacity are not available for the DEEP_ARCHIVE storage class.</p> </li> <li> <p> <b> <code>Standard</code> </b> - Standard retrievals allow you to access any of your archived objects within several hours. This is the default option for the GLACIER and DEEP_ARCHIVE retrieval requests that do not specify the retrieval option. Standard retrievals typically complete within 3-5 hours from the GLACIER storage class and typically complete within 12 hours from the DEEP_ARCHIVE storage class. </p> </li> <li> <p> <b> <code>Bulk</code> </b> - Bulk retrievals are Amazon S3 Glacier\u2019s lowest-cost retrieval option, enabling you to retrieve large amounts, even petabytes, of data inexpensively in a day. Bulk retrievals typically complete within 5-12 hours from the GLACIER storage class and typically complete within 48 hours from the DEEP_ARCHIVE storage class.</p> </li> </ul> <p>For more information about archive retrieval options and provisioned capacity for <code>Expedited</code> data access, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/restoring-objects.html\">Restoring Archived Objects</a> in the <i>Amazon Simple Storage Service Developer Guide</i>. </p> <p>You can use Amazon S3 restore speed upgrade to change the restore speed to a faster speed while it is in progress. You upgrade the speed of an in-progress restoration by issuing another restore request to the same object, setting a new <code>Tier</code> request element. When issuing a request to upgrade the restore tier, you must choose a tier that is faster than the tier that the in-progress restore is using. You must not change any other parameters, such as the <code>Days</code> request element. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/restoring-objects.html#restoring-objects-upgrade-tier.title.html\"> Upgrading the Speed of an In-Progress Restore</a> in the <i>Amazon Simple Storage Service Developer Guide</i>. </p> <p>To get the status of object restoration, you can send a <code>HEAD</code> request. Operations return the <code>x-amz-restore</code> header, which provides information about the restoration status, in the response. You can use Amazon S3 event notifications to notify you when a restore is initiated or completed. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/NotificationHowTo.html\">Configuring Amazon S3 Event Notifications</a> in the <i>Amazon Simple Storage Service Developer Guide</i>.</p> <p>After restoring an archived object, you can update the restoration period by reissuing the request with a new period. Amazon S3 updates the restoration period relative to the current time and charges only for the request-there are no data transfer charges. You cannot update the restoration period when Amazon S3 is actively processing your current restore request for the object.</p> <p>If your bucket has a lifecycle configuration with a rule that includes an expiration action, the object expiration overrides the life span that you specify in a restore request. For example, if you restore an object copy for 10 days, but the object is scheduled to expire in 3 days, Amazon S3 deletes the object in 3 days. For more information about lifecycle configuration, see <a>PutBucketLifecycleConfiguration</a> and <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/object-lifecycle-mgmt.html\">Object Lifecycle Management</a> in <i>Amazon Simple Storage Service Developer Guide</i>.</p> <p> <b>Responses</b> </p> <p>A successful operation returns either the <code>200 OK</code> or <code>202 Accepted</code> status code. </p> <ul> <li> <p>If the object copy is not previously restored, then Amazon S3 returns <code>202 Accepted</code> in the response. </p> </li> <li> <p>If the object copy is previously restored, Amazon S3 returns <code>200 OK</code> in the response. </p> </li> </ul> <p class=\"title\"> <b>Special Errors</b> </p> <ul> <li> <p class=\"title\"> <b/> </p> <ul> <li> <p> <i>Code: RestoreAlreadyInProgress</i> </p> </li> <li> <p> <i>Cause: Object restore is already in progress. (This error does not apply to SELECT type requests.)</i> </p> </li> <li> <p> <i>HTTP Status Code: 409 Conflict</i> </p> </li> <li> <p> <i>SOAP Fault Code Prefix: Client</i> </p> </li> </ul> </li> <li> <p class=\"title\"> <b/> </p> <ul> <li> <p> <i>Code: GlacierExpeditedRetrievalNotAvailable</i> </p> </li> <li> <p> <i>Cause: Glacier expedited retrievals are currently not available. Try again later. (Returned if there is insufficient capacity to process the Expedited request. This error applies only to Expedited retrievals and not to Standard or Bulk retrievals.)</i> </p> </li> <li> <p> <i>HTTP Status Code: 503</i> </p> </li> <li> <p> <i>SOAP Fault Code Prefix: N/A</i> </p> </li> </ul> </li> </ul> <p class=\"title\"> <b>Related Resources</b> </p> <ul> <li> <p> <a>PutBucketLifecycleConfiguration</a> </p> </li> <li> <p> <a>GetBucketNotificationConfiguration</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-glacier-select-sql-reference.html\">SQL Reference for Amazon S3 Select and Glacier Select </a> in the <i>Amazon Simple Storage Service Developer Guide</i> </p> </li> </ul>",
@@ -1140,14 +1220,20 @@
         },
         "AnalyticsAndOperator": {
             "documentation": "<p>A conjunction (logical AND) of predicates, which is used in evaluating a metrics filter. The operator must have at least two predicates in any combination, and an object must match all of the predicates for the filter to apply.</p>",
             "members": {
                 "Prefix": {
                     "documentation": "<p>The prefix to use when evaluating an AND predicate: The prefix that an object must have to be included in the metrics results.</p>",
                     "shape": "Prefix"
+                },
+                "Tags": {
+                    "documentation": "<p>The list of tags to use when evaluating an AND predicate.</p>",
+                    "flattened": true,
+                    "locationName": "Tag",
+                    "shape": "TagSet"
                 }
             },
             "type": "structure"
         },
         "AnalyticsConfiguration": {
             "documentation": "<p> Specifies the configuration and any analyses for the analytics filter of an Amazon S3 bucket.</p>",
             "members": {
@@ -1246,15 +1332,15 @@
         "Body": {
             "type": "blob"
         },
         "Bucket": {
             "documentation": "<p> In terms of implementation, a Bucket is a resource. An Amazon S3 bucket name is globally unique, and the namespace is shared by all AWS accounts. </p>",
             "members": {
                 "CreationDate": {
-                    "documentation": "Date the bucket was created.",
+                    "documentation": "<p>Date the bucket was created.</p>",
                     "shape": "CreationDate"
                 },
                 "LocationConstraint": {
                     "documentation": "Specifies the region where the bucket will be created. If you don't specify a region, the bucket will be created in US Standard.",
                     "shape": "BucketLocationConstraint"
                 },
                 "Name": {
@@ -1528,14 +1614,17 @@
         },
         "CloudFunctionInvocationRole": {
             "type": "string"
         },
         "Code": {
             "type": "string"
         },
+        "Comments": {
+            "type": "string"
+        },
         "CommonPrefix": {
             "documentation": "<p>Container for all (if there are any) keys between Prefix and the next occurrence of the string specified by a delimiter. CommonPrefixes lists keys that act like subdirectories in the directory specified by Prefix. For example, if the prefix is notes/ and the delimiter is a slash (/) as in notes/summer/july, the common prefix is notes/summer/. </p>",
             "members": {
                 "Prefix": {
                     "documentation": "<p>Container for the specified common prefix.</p>",
                     "shape": "Prefix"
                 }
@@ -1986,14 +2075,26 @@
                 },
                 "StorageClass": {
                     "documentation": "<p>The type of storage to use for the object. Defaults to 'STANDARD'.</p>",
                     "location": "header",
                     "locationName": "x-amz-storage-class",
                     "shape": "StorageClass"
                 },
+                "Tagging": {
+                    "documentation": "<p>The tag-set for the object destination object this value must be used in conjunction with the <code>TaggingDirective</code>. The tag-set must be encoded as URL Query parameters.</p>",
+                    "location": "header",
+                    "locationName": "x-amz-tagging",
+                    "shape": "TaggingHeader"
+                },
+                "TaggingDirective": {
+                    "documentation": "<p>Specifies whether the object tag-set are copied from the source object or replaced with tag-set provided in the request.</p>",
+                    "location": "header",
+                    "locationName": "x-amz-tagging-directive",
+                    "shape": "TaggingDirective"
+                },
                 "WebsiteRedirectLocation": {
                     "documentation": "<p>If the bucket is configured as a website, redirects requests for this object to another object in the same bucket or to an external URL. Amazon S3 stores the value of this header in the object metadata.</p>",
                     "location": "header",
                     "locationName": "x-amz-website-redirect-location",
                     "shape": "WebsiteRedirectLocation"
                 }
             },
@@ -2345,14 +2446,20 @@
                 },
                 "StorageClass": {
                     "documentation": "<p>The type of storage to use for the object. Defaults to 'STANDARD'.</p>",
                     "location": "header",
                     "locationName": "x-amz-storage-class",
                     "shape": "StorageClass"
                 },
+                "Tagging": {
+                    "documentation": "<p>The tag-set for the object. The tag-set must be encoded as URL Query parameters.</p>",
+                    "location": "header",
+                    "locationName": "x-amz-tagging",
+                    "shape": "TaggingHeader"
+                },
                 "WebsiteRedirectLocation": {
                     "documentation": "<p>If the bucket is configured as a website, redirects requests for this object to another object in the same bucket or to an external URL. Amazon S3 stores the value of this header in the object metadata.</p>",
                     "location": "header",
                     "locationName": "x-amz-website-redirect-location",
                     "shape": "WebsiteRedirectLocation"
                 }
             },
@@ -2651,14 +2758,52 @@
             },
             "required": [
                 "Bucket",
                 "Key"
             ],
             "type": "structure"
         },
+        "DeleteObjectTaggingOutput": {
+            "members": {
+                "VersionId": {
+                    "documentation": "<p>The versionId of the object the tag-set was removed from.</p>",
+                    "location": "header",
+                    "locationName": "x-amz-version-id",
+                    "shape": "ObjectVersionId"
+                }
+            },
+            "type": "structure"
+        },
+        "DeleteObjectTaggingRequest": {
+            "members": {
+                "Bucket": {
+                    "documentation": "<p>The bucket name containing the objects from which to remove the tags. </p> <p>When using this API with an access point, you must direct requests to the access point hostname. The access point hostname takes the form <i>AccessPointName</i>-<i>AccountId</i>.s3-accesspoint.<i>Region</i>.amazonaws.com. When using this operation using an access point through the AWS SDKs, you provide the access point ARN in place of the bucket name. For more information about access point ARNs, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/using-access-points.html\">Using Access Points</a> in the <i>Amazon Simple Storage Service Developer Guide</i>.</p>",
+                    "location": "uri",
+                    "locationName": "Bucket",
+                    "shape": "BucketName"
+                },
+                "Key": {
+                    "documentation": "<p>Name of the tag.</p>",
+                    "location": "uri",
+                    "locationName": "Key",
+                    "shape": "ObjectKey"
+                },
+                "VersionId": {
+                    "documentation": "<p>The versionId of the object that the tag-set will be removed from.</p>",
+                    "location": "querystring",
+                    "locationName": "versionId",
+                    "shape": "ObjectVersionId"
+                }
+            },
+            "required": [
+                "Bucket",
+                "Key"
+            ],
+            "type": "structure"
+        },
         "DeleteObjectsOutput": {
             "members": {
                 "Deleted": {
                     "documentation": "<p>Container element for a successful delete. It identifies the object that was successfully deleted.</p>",
                     "shape": "DeletedObjects"
                 },
                 "Errors": {
@@ -2706,14 +2851,28 @@
             "payload": "Delete",
             "required": [
                 "Bucket",
                 "Delete"
             ],
             "type": "structure"
         },
+        "DeletePublicAccessBlockRequest": {
+            "members": {
+                "Bucket": {
+                    "documentation": "<p>The Amazon S3 bucket whose <code>PublicAccessBlock</code> configuration you want to delete. </p>",
+                    "location": "uri",
+                    "locationName": "Bucket",
+                    "shape": "BucketName"
+                }
+            },
+            "required": [
+                "Bucket"
+            ],
+            "type": "structure"
+        },
         "DeletedObject": {
             "documentation": "<p>Information about the deleted object.</p>",
             "members": {
                 "DeleteMarker": {
                     "documentation": "<p>Specifies whether the versioned object that was permanently deleted was (true) or was not (false) a delete marker. In a simple DELETE, this header indicates whether (true) or not (false) a delete marker was created.</p>",
                     "shape": "DeleteMarker"
                 },
@@ -3262,14 +3421,15 @@
             },
             "payload": "ProtectionConfiguration",
             "type": "structure"
         },
         "GetBucketProtectionConfigurationRequest": {
             "members": {
                 "Bucket": {
+                    "documentation": "<p>The name of the Amazon S3 bucket whose policy status you want to retrieve.</p>",
                     "location": "uri",
                     "locationName": "Bucket",
                     "shape": "BucketName"
                 }
             },
             "required": [
                 "Bucket"
@@ -3626,14 +3786,20 @@
                 },
                 "StorageClass": {
                     "documentation": "<p>Provides storage class information of the object. Amazon S3 returns this header for all objects except for Standard storage class objects.</p>",
                     "location": "header",
                     "locationName": "x-amz-storage-class",
                     "shape": "StorageClass"
                 },
+                "TagCount": {
+                    "documentation": "<p>The number of tags, if any, on the object.</p>",
+                    "location": "header",
+                    "locationName": "x-amz-tagging-count",
+                    "shape": "TagCount"
+                },
                 "VersionId": {
                     "documentation": "<p>Version of the object.</p>",
                     "location": "header",
                     "locationName": "x-amz-version-id",
                     "shape": "ObjectVersionId"
                 },
                 "WebsiteRedirectLocation": {
@@ -3770,14 +3936,59 @@
             },
             "required": [
                 "Bucket",
                 "Key"
             ],
             "type": "structure"
         },
+        "GetObjectTaggingOutput": {
+            "members": {
+                "TagSet": {
+                    "documentation": "<p>Contains the tag set.</p>",
+                    "shape": "TagSet"
+                },
+                "VersionId": {
+                    "documentation": "<p>The versionId of the object for which you got the tagging information.</p>",
+                    "location": "header",
+                    "locationName": "x-amz-version-id",
+                    "shape": "ObjectVersionId"
+                }
+            },
+            "required": [
+                "TagSet"
+            ],
+            "type": "structure"
+        },
+        "GetObjectTaggingRequest": {
+            "members": {
+                "Bucket": {
+                    "documentation": "<p>The bucket name containing the object for which to get the tagging information. </p> <p>When using this API with an access point, you must direct requests to the access point hostname. The access point hostname takes the form <i>AccessPointName</i>-<i>AccountId</i>.s3-accesspoint.<i>Region</i>.amazonaws.com. When using this operation using an access point through the AWS SDKs, you provide the access point ARN in place of the bucket name. For more information about access point ARNs, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/using-access-points.html\">Using Access Points</a> in the <i>Amazon Simple Storage Service Developer Guide</i>.</p>",
+                    "location": "uri",
+                    "locationName": "Bucket",
+                    "shape": "BucketName"
+                },
+                "Key": {
+                    "documentation": "<p>Object key for which to get the tagging information.</p>",
+                    "location": "uri",
+                    "locationName": "Key",
+                    "shape": "ObjectKey"
+                },
+                "VersionId": {
+                    "documentation": "<p>The versionId of the object for which to get the tagging information.</p>",
+                    "location": "querystring",
+                    "locationName": "versionId",
+                    "shape": "ObjectVersionId"
+                }
+            },
+            "required": [
+                "Bucket",
+                "Key"
+            ],
+            "type": "structure"
+        },
         "GetObjectTorrentOutput": {
             "members": {
                 "Body": {
                     "documentation": "<p>A Bencoded dictionary as defined by the BitTorrent specification</p>",
                     "shape": "Body",
                     "streaming": true
                 },
@@ -3813,14 +4024,38 @@
             },
             "required": [
                 "Bucket",
                 "Key"
             ],
             "type": "structure"
         },
+        "GetPublicAccessBlockOutput": {
+            "members": {
+                "PublicAccessBlockConfiguration": {
+                    "documentation": "<p>The <code>PublicAccessBlock</code> configuration currently in effect for this Amazon S3 bucket.</p>",
+                    "shape": "PublicAccessBlockConfiguration"
+                }
+            },
+            "payload": "PublicAccessBlockConfiguration",
+            "type": "structure"
+        },
+        "GetPublicAccessBlockRequest": {
+            "members": {
+                "Bucket": {
+                    "documentation": "<p>The name of the Amazon S3 bucket whose <code>PublicAccessBlock</code> configuration you want to retrieve. </p>",
+                    "location": "uri",
+                    "locationName": "Bucket",
+                    "shape": "BucketName"
+                }
+            },
+            "required": [
+                "Bucket"
+            ],
+            "type": "structure"
+        },
         "GlacierJobParameters": {
             "documentation": "<p>Container for Glacier job parameters.</p>",
             "members": {
                 "Tier": {
                     "documentation": "<p>Glacier retrieval tier at which the restore will be processed.</p>",
                     "shape": "Tier"
                 }
@@ -4410,14 +4645,17 @@
         },
         "IsEnabled": {
             "type": "boolean"
         },
         "IsLatest": {
             "type": "boolean"
         },
+        "IsPublic": {
+            "type": "boolean"
+        },
         "IsTruncated": {
             "type": "boolean"
         },
         "KeyCount": {
             "type": "integer"
         },
         "KeyMarker": {
@@ -4555,14 +4793,18 @@
         },
         "LifecycleRuleFilter": {
             "documentation": "<p>The <code>Filter</code> is used to identify objects that a Lifecycle Rule applies to. A <code>Filter</code> must have exactly one of <code>Prefix</code>, <code>Tag</code>, or <code>And</code> specified.</p>",
             "members": {
                 "Prefix": {
                     "documentation": "<p>Prefix identifying one or more objects to which the rule applies.</p>",
                     "shape": "Prefix"
+                },
+                "Tag": {
+                    "documentation": "<p>This tag must exist in the object's tag set in order for the rule to apply.</p>",
+                    "shape": "Tag"
                 }
             },
             "type": "structure"
         },
         "LifecycleRules": {
             "documentation": "Currently only one Rule allowed.",
             "flattened": true,
@@ -5446,14 +5688,20 @@
         },
         "MetricsAndOperator": {
             "documentation": "<p>A conjunction (logical AND) of predicates, which is used in evaluating a metrics filter. The operator must have at least two predicates, and an object must match all of the predicates in order for the filter to apply.</p>",
             "members": {
                 "Prefix": {
                     "documentation": "<p>The prefix used when evaluating an AND predicate.</p>",
                     "shape": "Prefix"
+                },
+                "Tags": {
+                    "documentation": "<p>The list of tags used when evaluating an AND predicate.</p>",
+                    "flattened": true,
+                    "locationName": "Tag",
+                    "shape": "TagSet"
                 }
             },
             "type": "structure"
         },
         "MetricsConfiguration": {
             "documentation": "<p>Specifies a metrics configuration for the CloudWatch request metrics (specified by the metrics configuration ID) from an Amazon S3 bucket. If you're updating an existing metrics configuration, note that this is a full replacement of the existing metrics configuration. If you don't include the elements you want to keep, they are erased. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketPUTMetricConfiguration.html\"> PUT Bucket metrics</a> in the <i>Amazon Simple Storage Service API Reference</i>.</p>",
             "members": {
@@ -5902,14 +6150,30 @@
         "Protocol": {
             "enum": [
                 "http",
                 "https"
             ],
             "type": "string"
         },
+        "PublicAccessBlockConfiguration": {
+            "documentation": "<p>The PublicAccessBlock configuration that you want to apply to this Amazon S3 bucket. You can enable the configuration options in any combination. For more information about when Amazon S3 considers a bucket or object public, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/access-control-block-public-access.html#access-control-block-public-access-policy-status\">The Meaning of \"Public\"</a> in the <i>Amazon Simple Storage Service Developer Guide</i>. </p>",
+            "members": {
+                "BlockPublicAcls": {
+                    "documentation": "<p>Specifies whether Amazon S3 should block public access control lists (ACLs) for this bucket and objects in this bucket. Setting this element to <code>TRUE</code> causes the following behavior:</p> <ul> <li> <p>PUT Bucket acl and PUT Object acl calls fail if the specified ACL is public.</p> </li> <li> <p>PUT Object calls fail if the request includes a public ACL.</p> </li> <li> <p>PUT Bucket calls fail if the request includes a public ACL.</p> </li> </ul> <p>Enabling this setting doesn't affect existing policies or ACLs.</p>",
+                    "locationName": "BlockPublicAcls",
+                    "shape": "Setting"
+                },
+                "IgnorePublicAcls": {
+                    "documentation": "<p>Specifies whether Amazon S3 should ignore public ACLs for this bucket and objects in this bucket. Setting this element to <code>TRUE</code> causes Amazon S3 to ignore all public ACLs on this bucket and objects in this bucket.</p> <p>Enabling this setting doesn't affect the persistence of any existing ACLs and doesn't prevent new public ACLs from being set.</p>",
+                    "locationName": "IgnorePublicAcls",
+                    "shape": "Setting"
+                }
+            },
+            "type": "structure"
+        },
         "PutBucketAccelerateConfigurationRequest": {
             "members": {
                 "AccelerateConfiguration": {
                     "documentation": "<p>Container for setting the transfer acceleration state.</p>",
                     "locationName": "AccelerateConfiguration",
                     "shape": "AccelerateConfiguration",
                     "xmlNamespace": {
@@ -6591,28 +6855,118 @@
                 },
                 "StorageClass": {
                     "documentation": "<p>If you don't specify, Standard is the default storage class. Amazon S3 supports other storage classes.</p>",
                     "location": "header",
                     "locationName": "x-amz-storage-class",
                     "shape": "StorageClass"
                 },
+                "Tagging": {
+                    "documentation": "<p>The tag-set for the object. The tag-set must be encoded as URL Query parameters. (For example, \"Key1=Value1\")</p>",
+                    "location": "header",
+                    "locationName": "x-amz-tagging",
+                    "shape": "TaggingHeader"
+                },
                 "WebsiteRedirectLocation": {
                     "documentation": "<p>If the bucket is configured as a website, redirects requests for this object to another object in the same bucket or to an external URL. Amazon S3 stores the value of this header in the object metadata. For information about object metadata, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingMetadata.html\">Object Key and Metadata</a>.</p> <p>In the following example, the request header sets the redirect to an object (anotherPage.html) in the same bucket:</p> <p> <code>x-amz-website-redirect-location: /anotherPage.html</code> </p> <p>In the following example, the request header sets the object redirect to another website:</p> <p> <code>x-amz-website-redirect-location: http://www.example.com/</code> </p> <p>For more information about website hosting in Amazon S3, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/WebsiteHosting.html\">Hosting Websites on Amazon S3</a> and <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/how-to-page-redirect.html\">How to Configure Website Page Redirects</a>. </p>",
                     "location": "header",
                     "locationName": "x-amz-website-redirect-location",
                     "shape": "WebsiteRedirectLocation"
                 }
             },
             "payload": "Body",
             "required": [
                 "Bucket",
                 "Key"
             ],
             "type": "structure"
         },
+        "PutObjectTaggingOutput": {
+            "members": {
+                "VersionId": {
+                    "documentation": "<p>The versionId of the object the tag-set was added to.</p>",
+                    "location": "header",
+                    "locationName": "x-amz-version-id",
+                    "shape": "ObjectVersionId"
+                }
+            },
+            "type": "structure"
+        },
+        "PutObjectTaggingRequest": {
+            "members": {
+                "Bucket": {
+                    "documentation": "<p>The bucket name containing the object. </p> <p>When using this API with an access point, you must direct requests to the access point hostname. The access point hostname takes the form <i>AccessPointName</i>-<i>AccountId</i>.s3-accesspoint.<i>Region</i>.amazonaws.com. When using this operation using an access point through the AWS SDKs, you provide the access point ARN in place of the bucket name. For more information about access point ARNs, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/using-access-points.html\">Using Access Points</a> in the <i>Amazon Simple Storage Service Developer Guide</i>.</p>",
+                    "location": "uri",
+                    "locationName": "Bucket",
+                    "shape": "BucketName"
+                },
+                "ContentMD5": {
+                    "documentation": "<p>The MD5 hash for the request body.</p>",
+                    "location": "header",
+                    "locationName": "Content-MD5",
+                    "shape": "ContentMD5"
+                },
+                "Key": {
+                    "documentation": "<p>Name of the tag.</p>",
+                    "location": "uri",
+                    "locationName": "Key",
+                    "shape": "ObjectKey"
+                },
+                "Tagging": {
+                    "documentation": "<p>Container for the <code>TagSet</code> and <code>Tag</code> elements</p>",
+                    "locationName": "Tagging",
+                    "shape": "Tagging",
+                    "xmlNamespace": {
+                        "uri": "http://s3.amazonaws.com/doc/2006-03-01/"
+                    }
+                },
+                "VersionId": {
+                    "documentation": "<p>The versionId of the object that the tag-set will be added to.</p>",
+                    "location": "querystring",
+                    "locationName": "versionId",
+                    "shape": "ObjectVersionId"
+                }
+            },
+            "payload": "Tagging",
+            "required": [
+                "Bucket",
+                "Key",
+                "Tagging"
+            ],
+            "type": "structure"
+        },
+        "PutPublicAccessBlockRequest": {
+            "members": {
+                "Bucket": {
+                    "documentation": "<p>The name of the Amazon S3 bucket whose <code>PublicAccessBlock</code> configuration you want to set.</p>",
+                    "location": "uri",
+                    "locationName": "Bucket",
+                    "shape": "BucketName"
+                },
+                "ContentMD5": {
+                    "documentation": "<p>The MD5 hash of the <code>PutPublicAccessBlock</code> request body. </p>",
+                    "location": "header",
+                    "locationName": "Content-MD5",
+                    "shape": "ContentMD5"
+                },
+                "PublicAccessBlockConfiguration": {
+                    "documentation": "<p>The <code>PublicAccessBlock</code> configuration that you want to apply to this Amazon S3 bucket. You can enable the configuration options in any combination. For more information about when Amazon S3 considers a bucket or object public, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/access-control-block-public-access.html#access-control-block-public-access-policy-status\">The Meaning of \"Public\"</a> in the <i>Amazon Simple Storage Service Developer Guide</i>.</p>",
+                    "locationName": "PublicAccessBlockConfiguration",
+                    "shape": "PublicAccessBlockConfiguration",
+                    "xmlNamespace": {
+                        "uri": "http://s3.amazonaws.com/doc/2006-03-01/"
+                    }
+                }
+            },
+            "payload": "PublicAccessBlockConfiguration",
+            "required": [
+                "Bucket",
+                "PublicAccessBlockConfiguration"
+            ],
+            "type": "structure"
+        },
         "QueueArn": {
             "type": "string"
         },
         "QueueConfiguration": {
             "documentation": "<p>Specifies the configuration for publishing messages to an Amazon Simple Queue Service (Amazon SQS) queue when Amazon S3 detects specified events.</p>",
             "members": {
                 "Events": {
@@ -6986,14 +7340,17 @@
         },
         "ServerSideEncryption": {
             "enum": [
                 "AES256"
             ],
             "type": "string"
         },
+        "Setting": {
+            "type": "boolean"
+        },
         "Size": {
             "type": "integer"
         },
         "StartAfter": {
             "type": "string"
         },
         "StorageClass": {
@@ -7060,14 +7417,17 @@
             },
             "required": [
                 "Key",
                 "Value"
             ],
             "type": "structure"
         },
+        "TagCount": {
+            "type": "integer"
+        },
         "TagSet": {
             "member": {
                 "locationName": "Tag",
                 "shape": "Tag"
             },
             "type": "list"
         },
@@ -7080,14 +7440,24 @@
                 }
             },
             "required": [
                 "TagSet"
             ],
             "type": "structure"
         },
+        "TaggingDirective": {
+            "enum": [
+                "COPY",
+                "REPLACE"
+            ],
+            "type": "string"
+        },
+        "TaggingHeader": {
+            "type": "string"
+        },
         "TargetBucket": {
             "type": "string"
         },
         "TargetGrant": {
             "documentation": "<p>Container for granting information.</p>",
             "members": {
                 "Grantee": {
```

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/data/s3/2006-03-01/waiters-2.json` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/data/s3/2006-03-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/data/s3/2006-03-01/paginators-1.json` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/data/s3/2006-03-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/data/_retry.json` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/data/_retry.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/validate.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/validate.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/httpsession.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/httpsession.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/eventstream.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/eventstream.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/utils.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/utils.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/hooks.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/hooks.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/credentials.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1096,15 +1096,15 @@
 
         if ibm_api_key_id:
             logger.info('Found IBM credentials in environment variables.')
             ibm_api_key_id, ibm_service_instance_id, ibm_auth_endpoint = self._extract_creds_from_mapping(
                 self.environ, self._mapping['ibm_api_key_id'],
                 self._mapping['ibm_service_instance_id'],
                 self._mapping['ibm_auth_endpoint'])
-            
+
             return OAuth2Credentials(api_key_id=ibm_api_key_id,
                                      service_instance_id=ibm_service_instance_id,
                                      auth_endpoint=ibm_auth_endpoint,
                                      method=self.METHOD)
         elif access_key:
             logger.info('Found credentials in environment variables.')
             fetcher = self._create_credentials_fetcher()
@@ -1312,15 +1312,15 @@
         if self._profile_name in full_config['profiles']:
             profile_config = full_config['profiles'][self._profile_name]
             if self.IBM_COS_API_KEY_ID in profile_config:
                 logger.info("IBM Credentials found in AWS config file: %s",
                             self._config_filename)
                 ibm_api_key_id, ibm_service_instance_id, ibm_auth_endpoint = self._extract_creds_from_mapping(
                     profile_config, self.IBM_COS_API_KEY_ID, self.IBM_COS_SERVICE_INSTANCE_ID, self.IBM_COS_AUTH_ENDPOINT)
-                
+
                 return OAuth2Credentials(api_key_id=ibm_api_key_id,
                                          service_instance_id=ibm_service_instance_id,
                                          auth_endpoint=ibm_auth_endpoint,
                                          method=self.METHOD)
             elif self.ACCESS_KEY in profile_config:
                 logger.info("Credentials found in AWS config file: %s",
                             self._config_filename)
@@ -2167,15 +2167,15 @@
 
         :type auth_endpoint: str
 
         :param auth_endpoint: URL used for IAM authentication. If not provided,
             API_TOKEN_URL will be used.
 
         :type time_fetcher: datetime
-        
+
         :param time_fetcher: current date and time used for calculating
             expiration time for token.
 
         :type auth_function: function
 
         :param auth_function: function that does custom authentication
             and returns json with token, refresh token, expiry time
@@ -2218,29 +2218,29 @@
         self._initial_token_set_event = threading.Event()
         self._shutdown = False
         atexit.register(self._cleanup)
 
 
     def _cleanup(self):
         """
-        Cleaup resources 
+        Cleaup resources
         """
         self.stop_refresh_thread()
-        
+
     def stop_refresh_thread(self):
         """
         Stop the background thread
         """
         if not self._shutdown:
             self._shutdown = True
             if self._background_thread:
-                if self._background_thread.isAlive():
+                if self._background_thread.is_alive():
                     self.wakeup_refresh_thread()
                     self._background_thread_stopped_event.wait(3)
-        
+
     def wakeup_refresh_thread(self):
         """
         Force the background thread to wakeup and refresh
         """
         self._background_thread_wakeup_event.set()
 
     def _background_refresher(self):
@@ -2264,15 +2264,15 @@
                     new_remaining = 5 # possible expired token let the _refresh method throw an exception, if required
 
                 logger.debug('Background refresh thread going to sleep for ' + str(new_remaining) + ' seconds')
                 self._background_thread_wakeup_event.clear()
                 self._background_thread_wakeup_event.wait(new_remaining)
         except Exception as e:
              logger.error("Exiting background refresh thread: " + str(e))
-            
+
         self._background_thread_stopped_event.set()
 
     def get_token(self):
         """Returns a token, possibly retrieving it first.
         Always returns token. If token is not available, retrieves.
         It also spawns background thread that makes sure that token
         never expires.
@@ -2284,62 +2284,62 @@
                 try:
                     if not self._get_cache_token(): # try again another thread may have refreshed it
                         self._get_initial_token()
                         self._initial_token_set_event.set();
 
                         if self._background_thread:
                             # check to see if the thread is still running
-                            if not self._background_thread.isAlive():
+                            if not self._background_thread.is_alive():
                                 self._background_thread = None
-                        
+
                         if not self._background_thread:
                             self._background_thread = threading.Thread(target=self._background_refresher)
                             self._background_thread.daemon = True
                             self._background_thread.start()
                 finally:
-                    self._initial_token_set_event.set(); 
+                    self._initial_token_set_event.set();
                     self._refresh_lock.release()
             else:
                 self._initial_token_set_event.wait(5);
 
         return self._get_cache_token()
 
     def set_verify(self, verify):
-        """ Turn on/off ssl cert verify 
+        """ Turn on/off ssl cert verify
         """
         self._verify = verify
 
     def get_verify(self):
-        """ True/False - get if ssl cert verify is enabled 
+        """ True/False - get if ssl cert verify is enabled
         """
         return self._verify
 
     def _seconds_remaining(self):
-        """ Seconds to expiry time 
+        """ Seconds to expiry time
         """
         if not self._expiry_time:
             return -1
         delta = self._expiry_time - self._time_fetcher()
         return total_seconds(delta)
 
     def _get_token_url(self):
-        """ Get the IAM server url if set 
+        """ Get the IAM server url if set
         If not set use the default usl
         """
         if self.auth_endpoint:
             return self.auth_endpoint
         else:
             return DefaultTokenManager.API_TOKEN_URL
 
     def set_from_config(self, config):
         """ store any values that are required from the config
         """
         if config:
             self.proxies = config.proxies
-        
+
     def _get_data(self):
         """ Get the data posted to IAM server
         If refresh token exists request a token refresh
         """
         if self._get_cache_refresh_token():
             return {u'grant_type': u'refresh_token',
                     u'response_type': u'cloud_iam',
@@ -2445,36 +2445,36 @@
             # If we're within the mandatory refresh window,
             # we must block until we get refreshed credentials.
             with self._refresh_lock:
                 if not self._refresh_needed(self._mandatory_refresh_timeout):
                     return
                 self._protected_refresh(is_mandatory=True)
 
-    
+
     def _protected_refresh(self, is_mandatory):
         """Performs mandatory or advisory refresh.
         Precondition: this method should only be called if you've acquired
         the self._refresh_lock.
         """
         try:
             metadata = self.auth_function()
         except Exception as e:
             period_name = 'mandatory' if is_mandatory else 'advisory'
             logger.warning("Refreshing temporary credentials failed "
                            "during %s refresh period.",
                            period_name, exc_info=True)
-            
+
             if is_mandatory:
                 if self._is_expired():
                     self._set_cache_token() # clear the cache
                     raise
 
             # if token hasnt expired continue to use it
             return
-        
+
         self._set_from_data(metadata)
 
     def _get_initial_token(self, retry_count=3, retry_delay=1):
         """ get the inital token - if it fails raise exception
         """
         _total_attempts = retry_count
         while True:
@@ -2486,73 +2486,73 @@
                 if _total_attempts > 0:
                     logger.debug("Retrying auth call")
                     time.sleep(retry_delay)
                 else:
                     logger.warning("Problem fetching initial IAM token.", exc_info=True)
                     self._set_cache_token() # clear the cache
                     raise
-        
+
         self._set_from_data(metadata)
         self._set_refresh_timeouts()
 
-    def _get_cache_refresh_token(self): 
+    def _get_cache_refresh_token(self):
         """ get the cached refresh token from previous call to IAM server
-        """  
+        """
         return self._refresh_token
 
-       
-    def _get_cache_token(self): 
+
+    def _get_cache_token(self):
         """ get the cached access token from previous call to IAM server
-        """  
+        """
         with self._token_update_lock:
             if self._token:
                 if self._seconds_remaining() <= 0:
                     return None
-                
+
             return self._token
 
 
-    def _set_cache_token(self, 
-                          access_token=None, 
-                          refresh_token=None, 
-                          token_type=None, 
+    def _set_cache_token(self,
+                          access_token=None,
+                          refresh_token=None,
+                          token_type=None,
                           refresh_in_secs=None):
         """ cache token and expiry date details retrieved in call to IAM server
         if the token is expired raise an exception and return error to user
-        """  
+        """
         with self._token_update_lock:
             self._token = access_token
             self._refresh_token = refresh_token
             self._token_type = token_type
-            
+
             if refresh_in_secs is None:
                 self._expiry_time = None
-            else:        
+            else:
                 _refresh_in_secs = self.REFRESH_OVERRIDE_IN_SECS if self.REFRESH_OVERRIDE_IN_SECS > 0 else refresh_in_secs
                 # Add expires_in to current system time.
                 self._expiry_time = self._time_fetcher() + datetime.timedelta(seconds=_refresh_in_secs)
 
                 if self._is_expired():
                     self._token = None
                     self._refresh_token = None
                     self._token_type = None
                     self._expiry_time = None
-                    
+
                     msg = ("Credentials fetched ok : but are expired.")
                     logger.warning(msg)
                     raise RuntimeError(msg)
-                    
+
                 logger.debug("Retrieved credentials will expire at: %s", self._expiry_time)
 
 
     def _set_from_data(self, data):
         """ extract required values from metadata returned from IAM server
         """
         _refresh_token = data['refresh_token'] if 'refresh_token' in data  else None
-        self._set_cache_token(data['access_token'], _refresh_token, data['token_type'], data['expires_in'])        
+        self._set_cache_token(data['access_token'], _refresh_token, data['token_type'], data['expires_in'])
 
     def _set_refresh_timeouts(self):
         """
         Set the advisory  timeout to 25% of remaining time - usually 15 minutes on 1 hour expiry
         Set the mandatory timeout to 17% of remaining time - usually 10 minutes on 1 hour expiry
         """
         if self._expiry_time:
@@ -2564,24 +2564,24 @@
                          ') Mandatory(' +
                          str(self._mandatory_refresh_timeout) + ')')
 
 
 class DelegatedTokenManager(DefaultTokenManager):
     """ Requests and processes IAM delegate tokens
         Delegate token refreshed every six days """
-    def __init__(self, 
+    def __init__(self,
                  api_key_id=None,
                  service_instance_id=None,
                  auth_endpoint=None,
                  time_fetcher=_local_now,
                  auth_function=None,
                  verify=True,
                  receiver_client_ids=None):
 
-        super(DelegatedTokenManager, self).__init__(api_key_id, 
+        super(DelegatedTokenManager, self).__init__(api_key_id,
                                                     service_instance_id,
                                                     auth_endpoint,
                                                     time_fetcher,
                                                     auth_function,
                                                     verify)
 
         self._receiver_client_ids = receiver_client_ids
@@ -2594,19 +2594,19 @@
                 u'response_type': u'delegated_refresh_token',
                 u'apikey': self.api_key_id}
 
         if self._receiver_client_ids is not None:
             data[u'receiver_client_ids'] = u'%s' % self._receiver_client_ids
 
         return data
-        
+
     def _set_from_data(self, data):
         """ extract required values from metadata returned from IAM server """
         _REFRESH_SIX_DAYS_IN_SECS = 518400  #refresh delgate token every 6days
-        self._set_cache_token(data['delegated_refresh_token'], 
+        self._set_cache_token(data['delegated_refresh_token'],
                               None,
                               data.get('token_type'),
                               _REFRESH_SIX_DAYS_IN_SECS)
 
 
 class OAuth2Credentials(Credentials):
     """
@@ -2742,8 +2742,7 @@
 
         """
         token = self.token_manager.get_token()
 
         # Signer is only interested in token, and besides, we might not even have api key
         return ReadOnlyCredentials(
             None, None, token)
-
```

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/loaders.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/loaders.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/model.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/model.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/configprovider.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/configprovider.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/configloader.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/configloader.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/client.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/client.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/translate.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/translate.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/cacert.pem` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/cacert.pem`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/response.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/response.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/__init__.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/paginator.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/paginator.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/docstring.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/docstring.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/bcdoc/__init__.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/bcdoc/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/bcdoc/style.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/bcdoc/style.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/bcdoc/docstringparser.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/bcdoc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/bcdoc/restdoc.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/bcdoc/restdoc.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/waiter.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/waiter.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/method.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/method.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/service.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/service.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/utils.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/utils.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/example.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/example.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/client.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/client.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/sharedexample.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/sharedexample.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/params.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/params.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/docs/shape.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/docs/shape.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/endpoint.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/endpoint.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/ibm_botocore/serialize.py` & `ibm-cos-sdk-core-2.9.0/ibm_botocore/serialize.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/setup.py` & `ibm-cos-sdk-core-2.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 import ibm_botocore
 
 requires = ['jmespath>=0.7.1,<1.0.0',
-            'docutils>=0.10,<0.16',
             'requests>=2.18,<3.0',
             'python-dateutil>=2.1,<3.0.0']
 
 setup(
     name='ibm-cos-sdk-core',
     version=ibm_botocore.__version__,
     description='Low-level, data-driven core of IBM SDK for Python',
```

### Comparing `ibm-cos-sdk-core-2.8.0/docs/source/conf.py` & `ibm-cos-sdk-core-2.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/docs/source/client_upgrades.rst` & `ibm-cos-sdk-core-2.9.0/docs/source/client_upgrades.rst`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/docs/source/_static/404.html` & `ibm-cos-sdk-core-2.9.0/docs/source/_static/404.html`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/docs/source/reference/services/s3.rst` & `ibm-cos-sdk-core-2.9.0/docs/source/reference/services/s3.rst`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/docs/make.bat` & `ibm-cos-sdk-core-2.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-core-2.8.0/docs/Makefile` & `ibm-cos-sdk-core-2.9.0/docs/Makefile`

 * *Files identical despite different names*

