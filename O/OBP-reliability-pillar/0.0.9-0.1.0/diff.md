# Comparing `tmp/OBP_reliability_pillar-0.0.9.tar.gz` & `tmp/OBP_reliability_pillar-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_reliability_pillar-0.0.9.tar", last modified: Mon Dec 19 13:46:49 2022, max compression
+gzip compressed data, was "OBP_reliability_pillar-0.1.0.tar", last modified: Wed May 31 11:41:04 2023, max compression
```

## Comparing `OBP_reliability_pillar-0.0.9.tar` & `OBP_reliability_pillar-0.1.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.738896 OBP_reliability_pillar-0.0.9/
--rw-rw-rw-   0        0        0        0 2022-11-24 06:08:48.000000 OBP_reliability_pillar-0.0.9/LICENCE
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.295796 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/
--rw-rw-rw-   0        0        0     3014 2022-12-19 13:45:08.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.351494 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/auto_scaling/
--rw-rw-rw-   0        0        0      197 2022-12-14 17:58:06.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/auto_scaling/__init__.py
--rw-rw-rw-   0        0        0     1978 2022-12-15 04:41:01.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py
--rw-rw-rw-   0        0        0      514 2022-12-15 06:10:23.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/auto_scaling/compliance.py
--rw-rw-rw-   0        0        0     2068 2022-12-15 05:13:33.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.373942 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/cloudwatch/
--rw-rw-rw-   0        0        0      193 2022-12-14 16:55:31.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/cloudwatch/__init__.py
--rw-rw-rw-   0        0        0     2985 2022-12-15 04:41:02.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/cloudwatch/alarm_action_check.py
--rw-rw-rw-   0        0        0      392 2022-12-15 04:41:02.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/cloudwatch/compliance.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.413116 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/dynamodb/
--rw-rw-rw-   0        0        0      187 2022-12-14 13:37:49.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      617 2022-12-19 12:55:46.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/dynamodb/compliance.py
--rw-rw-rw-   0        0        0     2066 2022-12-19 12:44:27.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py
--rw-rw-rw-   0        0        0     1952 2022-12-19 12:55:46.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py
--rw-rw-rw-   0        0        0      557 2022-12-14 17:33:05.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/dynamodb/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.444154 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/ec2/
--rw-rw-rw-   0        0        0      177 2022-12-15 09:13:29.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/ec2/__init__.py
--rw-rw-rw-   0        0        0      609 2022-12-15 08:36:08.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/ec2/compliance.py
--rw-rw-rw-   0        0        0     2113 2022-12-15 08:32:29.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py
--rw-rw-rw-   0        0        0     2096 2022-12-15 08:36:08.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/ec2/instance_in_vpc.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.466479 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_beanstalk/
--rw-rw-rw-   0        0        0      205 2022-12-14 17:23:50.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_beanstalk/__init__.py
--rw-rw-rw-   0        0        0      490 2022-12-15 04:41:02.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_beanstalk/compliance.py
--rw-rw-rw-   0        0        0     2184 2022-12-15 04:41:01.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.501255 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_load_balancer/
--rw-rw-rw-   0        0        0      175 2022-12-14 16:09:12.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_load_balancer/__init__.py
--rw-rw-rw-   0        0        0      687 2022-12-19 13:44:55.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_load_balancer/compliance.py
--rw-rw-rw-   0        0        0     1681 2022-12-15 08:52:50.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py
--rw-rw-rw-   0        0        0     1843 2022-12-15 08:58:06.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py
--rw-rw-rw-   0        0        0      940 2022-12-15 08:52:50.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_load_balancer/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.523783 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_search/
--rw-rw-rw-   0        0        0      195 2022-12-15 13:20:24.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_search/__init__.py
--rw-rw-rw-   0        0        0      393 2022-12-15 12:50:30.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_search/compliance.py
--rw-rw-rw-   0        0        0     1765 2022-12-15 13:23:40.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.545200 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/guard_duty/
--rw-rw-rw-   0        0        0      207 2022-12-15 13:21:10.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/guard_duty/__init__.py
--rw-rw-rw-   0        0        0      357 2022-12-15 13:20:24.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/guard_duty/compliance.py
--rw-rw-rw-   0        0        0     1822 2022-12-15 13:20:24.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.583400 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/lambdafn/
--rw-rw-rw-   0        0        0      181 2022-12-15 07:01:14.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/lambdafn/__init__.py
--rw-rw-rw-   0        0        0      536 2022-12-18 12:53:29.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/lambdafn/compliance.py
--rw-rw-rw-   0        0        0     1809 2022-12-18 12:49:35.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py
--rw-rw-rw-   0        0        0     1582 2022-12-18 12:53:29.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py
--rw-rw-rw-   0        0        0      844 2022-12-18 12:40:40.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/lambdafn/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.637091 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/
--rw-rw-rw-   0        0        0      179 2022-12-14 16:51:39.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/__init__.py
--rw-rw-rw-   0        0        0      946 2022-12-18 12:13:38.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/compliance.py
--rw-rw-rw-   0        0        0     2038 2022-12-15 04:41:02.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
--rw-rw-rw-   0        0        0     2078 2022-12-18 12:15:28.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/rds_backup_enabled.py
--rw-rw-rw-   0        0        0     1993 2022-12-14 16:48:56.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py
--rw-rw-rw-   0        0        0     2025 2022-12-14 16:48:56.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py
--rw-rw-rw-   0        0        0     1923 2022-12-14 16:48:56.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.668920 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/redshift/
--rw-rw-rw-   0        0        0      189 2022-12-19 12:39:09.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/redshift/__init__.py
--rw-rw-rw-   0        0        0      673 2022-12-19 12:39:09.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/redshift/compliance.py
--rw-rw-rw-   0        0        0     1954 2022-12-15 04:41:02.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/redshift/redshift_backup_enabled.py
--rw-rw-rw-   0        0        0     2309 2022-12-19 12:46:11.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.718244 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/s3/
--rw-rw-rw-   0        0        0      175 2022-12-14 17:23:50.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/s3/__init__.py
--rw-rw-rw-   0        0        0      758 2022-12-18 12:28:01.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/s3/compliance.py
--rw-rw-rw-   0        0        0     1682 2022-12-18 12:33:53.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py
--rw-rw-rw-   0        0        0     1653 2022-12-14 17:23:50.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py
--rw-rw-rw-   0        0        0     1569 2022-12-14 17:23:50.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.728141 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/security_hub/
--rw-rw-rw-   0        0        0     1474 2022-12-14 17:58:06.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/security_hub/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-19 13:46:49.320687 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar.egg-info/
--rw-rw-rw-   0        0        0     1114 2022-12-19 13:46:49.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3079 2022-12-19 13:46:49.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-19 13:46:49.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-12-19 13:46:49.000000 OBP_reliability_pillar-0.0.9/OBP_reliability_pillar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1114 2022-12-19 13:46:49.734038 OBP_reliability_pillar-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      755 2022-12-19 13:35:30.000000 OBP_reliability_pillar-0.0.9/README.md
--rw-rw-rw-   0        0        0      498 2022-12-19 13:45:34.000000 OBP_reliability_pillar-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-19 13:46:49.739394 OBP_reliability_pillar-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:04.049144 OBP_reliability_pillar-0.1.0/
+-rw-rw-rw-   0        0        0        0 2022-11-24 06:08:48.000000 OBP_reliability_pillar-0.1.0/LICENCE
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.410146 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/
+-rw-rw-rw-   0        0        0     4908 2023-05-31 11:40:25.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.499243 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/auto_scaling/
+-rw-rw-rw-   0        0        0      197 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/auto_scaling/__init__.py
+-rw-rw-rw-   0        0        0     2101 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py
+-rw-rw-rw-   0        0        0      607 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/auto_scaling/compliance.py
+-rw-rw-rw-   0        0        0     2223 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.534144 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/cloudwatch/
+-rw-rw-rw-   0        0        0      193 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/cloudwatch/__init__.py
+-rw-rw-rw-   0        0        0     3134 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/cloudwatch/alarm_action_check.py
+-rw-rw-rw-   0        0        0      485 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/cloudwatch/compliance.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.580242 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/dynamodb/
+-rw-rw-rw-   0        0        0      187 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      667 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/dynamodb/compliance.py
+-rw-rw-rw-   0        0        0     2222 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py
+-rw-rw-rw-   0        0        0     2106 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py
+-rw-rw-rw-   0        0        0      557 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/dynamodb/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.624145 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/ec2/
+-rw-rw-rw-   0        0        0      177 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/ec2/__init__.py
+-rw-rw-rw-   0        0        0      709 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/ec2/compliance.py
+-rw-rw-rw-   0        0        0     2233 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     2257 2023-05-31 08:17:16.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/ec2/instance_in_vpc.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.656154 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_beanstalk/
+-rw-rw-rw-   0        0        0      205 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_beanstalk/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_beanstalk/compliance.py
+-rw-rw-rw-   0        0        0     2339 2023-05-31 08:23:26.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.691143 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_load_balancer/
+-rw-rw-rw-   0        0        0      177 2023-01-27 09:44:59.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_load_balancer/__init__.py
+-rw-rw-rw-   0        0        0      737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_load_balancer/compliance.py
+-rw-rw-rw-   0        0        0     1829 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py
+-rw-rw-rw-   0        0        0     1994 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py
+-rw-rw-rw-   0        0        0     1700 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_load_balancer/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.763146 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_search/
+-rw-rw-rw-   0        0        0      197 2023-01-27 11:52:50.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_search/__init__.py
+-rw-rw-rw-   0        0        0      432 2023-05-31 11:40:25.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_search/compliance.py
+-rw-rw-rw-   0        0        0     1940 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.803144 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/guard_duty/
+-rw-rw-rw-   0        0        0      207 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/guard_duty/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/guard_duty/compliance.py
+-rw-rw-rw-   0        0        0     1965 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.843145 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/lambdafn/
+-rw-rw-rw-   0        0        0      181 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/lambdafn/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/lambdafn/compliance.py
+-rw-rw-rw-   0        0        0     1932 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py
+-rw-rw-rw-   0        0        0     1737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py
+-rw-rw-rw-   0        0        0      844 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/lambdafn/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.927156 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/
+-rw-rw-rw-   0        0        0      199 2023-05-31 08:47:40.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/__init__.py
+-rw-rw-rw-   0        0        0     2126 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/compliance.py
+-rw-rw-rw-   0        0        0     1558 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
+-rw-rw-rw-   0        0        0     2319 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/rds_backup_enabled.py
+-rw-rw-rw-   0        0        0     2126 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     1479 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py
+-rw-rw-rw-   0        0        0     1375 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.976158 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/redshift/
+-rw-rw-rw-   0        0        0      213 2023-05-31 08:47:40.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/redshift/__init__.py
+-rw-rw-rw-   0        0        0     1738 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/redshift/compliance.py
+-rw-rw-rw-   0        0        0     1383 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/redshift/redshift_backup_enabled.py
+-rw-rw-rw-   0        0        0     1710 2023-05-31 08:41:05.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:04.030145 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/s3/
+-rw-rw-rw-   0        0        0      192 2023-05-31 08:47:40.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/s3/__init__.py
+-rw-rw-rw-   0        0        0     1112 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/s3/compliance.py
+-rw-rw-rw-   0        0        0     1825 2023-05-31 08:23:26.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py
+-rw-rw-rw-   0        0        0     1796 2023-05-31 09:39:39.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py
+-rw-rw-rw-   0        0        0     1716 2023-05-31 08:23:25.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:04.043144 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/security_hub/
+-rw-rw-rw-   0        0        0     1586 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/security_hub/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:41:03.450233 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar.egg-info/
+-rw-rw-rw-   0        0        0     1114 2023-05-31 11:41:03.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3079 2023-05-31 11:41:03.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 11:41:03.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-31 11:41:03.000000 OBP_reliability_pillar-0.1.0/OBP_reliability_pillar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1114 2023-05-31 11:41:04.048143 OBP_reliability_pillar-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2022-12-19 13:35:30.000000 OBP_reliability_pillar-0.1.0/README.md
+-rw-rw-rw-   0        0        0      498 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 11:41:04.050143 OBP_reliability_pillar-0.1.0/setup.cfg
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,17 +12,19 @@
     :return dict:
     """
     logger.info(" ---Inside autoscaling :: asg_elb_healthcheck_required()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.11'
     compliance_type = "AutoScaling Group ELB health check required"
     description = "Checks if ELB health check is enabled on autoscaling group"
     resource_type = "Auto Scaling Group"
+    risk_level = 'Medium'
 
     regions = self.session.get_available_regions('autoscaling')
 
     for region in regions:
         try:
             client = self.session.client('autoscaling', region_name=region)
             marker = ''
@@ -52,10 +54,12 @@
             pass
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
+        'ControlId': control_id,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/auto_scaling/compliance.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/auto_scaling/compliance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from OBP_reliability_pillar.auto_scaling.launch_config_public_ip_disabled import *
 from OBP_reliability_pillar.auto_scaling.asg_elb_healthcheck_required import *
 
-
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
+
 # checks autoscaling compliance
-def auto_scaling_compliance(self) -> dict:
+def auto_scaling_compliance(self, regions) -> dict:
     logger.info(" ---Inside auto_scaling_compliance()")
     response = [
-        launch_config_public_ip_disabled(self),
-        asg_elb_healthcheck_required(self)
+        launch_config_public_ip_disabled(self, regions),
+        # Already covered in monitoring module, hence commenting here
+        # asg_elb_healthcheck_required(self)
     ]
 
-    return response
+    return response
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 
 import botocore
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def launch_config_public_ip_disabled(self) -> dict:
+def launch_config_public_ip_disabled(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside autoscaling :: launch_config_public_ip_disabled()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.12'
     compliance_type = "Launch configuration public ip disabled"
     description = "Checks if public ip is disabled in launch configuration or not"
     resource_type = "Auto Scaling"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('autoscaling')
+    # regions = self.session.get_available_regions('autoscaling')
 
     for region in regions:
         try:
             client_asg = self.session.client('autoscaling', region_name=region)
 
             n_token = ''
             while True:
@@ -54,10 +57,12 @@
             pass
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
+        'ControlId': control_id,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/cloudwatch/alarm_action_check.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/cloudwatch/alarm_action_check.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # compliance.py check for cloudwatch alarm check
-def alarm_action_check(self) -> dict:
+def alarm_action_check(self, regions) -> dict:
     """
-
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside cloudwatch :: alarm_action_check()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.17'
     compliance_type = "Cloudwatch Alarm check"
     description = "Checks whether CloudWatch alarms have at least one alarm action, one INSUFFICIENT_DATA action, or one OK action enabled."
     resource_type = "Cloudwatch"
+    risk_level = 'Low'
 
-    regions  = self.session.get_available_regions('cloudwatch')
+    # regions = self.session.get_available_regions('cloudwatch')
 
     for region in regions:
         try:
             client = self.session.client('cloudwatch', region_name=region)
             marker = ''
             while True:
                 if marker == '' or marker is None:
@@ -40,15 +42,14 @@
                     ok_action = len(alarm['OKActions'])
 
                     if not alarm_action or not insufficient_data_action or not ok_action:
                         result = False
                         failReason = 'CloudWatch alarms does not have at least one alarm action, one INSUFFICIENT_DATA action, or one OK action enabled.'
                         offenders.append(alarm['AlarmName'])
 
-
                 for alarm in response_describe_alarms['MetricAlarms']:
                     alarm_action = len(alarm['AlarmActions'])
                     insufficient_data_action = len(alarm['InsufficientDataActions'])
                     ok_action = len(alarm['OKActions'])
 
                     if alarm_action or insufficient_data_action or ok_action:
                         result = False
@@ -64,11 +65,13 @@
         except ClientError as e:
             logger.error("Something went wrong with region {}: {}".format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
-    }
+        'Description': description,
+        'Risk Level': risk_level
+    }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/dynamodb/compliance.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/dynamodb/compliance.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 from OBP_reliability_pillar.dynamodb.dynamodb_pitr_enabled import dynamodb_pitr_enabled
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # returns consolidated dynamodb compliance
-def dynamodb_compliance(self) -> list:
+def dynamodb_compliance(self, regions) -> list:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside dynamodb :: dynamodb_compliance()")
 
     response = [
-        dynamodb_autoscaling_enabled(self),
-        dynamodb_pitr_enabled(self),
+        dynamodb_autoscaling_enabled(self, regions),
+        dynamodb_pitr_enabled(self, regions),
     ]
 
-    return response
+    return response
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,33 +4,36 @@
 from OBP_reliability_pillar.dynamodb.utils import list_dynamodb_tables
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # checks compliance.py for dynamodb auto-scaling is enabled
-def dynamodb_autoscaling_enabled(self) -> dict:
+def dynamodb_autoscaling_enabled(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside dynamodb :: dynamodb_autoscaling_enabled()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.25'
     compliance_type = "Dynamodb autoscaling enabled"
     description = "Checks if Auto Scaling or On-Demand is enabled on your DynamoDB tables"
     resource_type = "Dynamodb"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('dynamodb')
+    # regions = self.session.get_available_regions('dynamodb')
 
     for region in regions:
         try:
-            client = self.session.client('dynamodb',region_name=region)
+            client = self.session.client('dynamodb', region_name=region)
 
             dynamodb_tables = list_dynamodb_tables(client)
             for table in dynamodb_tables:
                 response = client.describe_table(
                     TableName=table
                 )
                 global_secondary_index = [index_name['IndexName'] for index_name in response['table']['GlobalSecondaryIndexes']]
@@ -45,11 +48,13 @@
         except botocore.exceptions.ClientError as e:
             logger.error("Something went wrong with region {}: {}".format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 from OBP_reliability_pillar.dynamodb.utils import list_dynamodb_tables
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # Checks compliance for dynamodb-pitr-enabled
-def dynamodb_pitr_enabled(self) -> dict:
+def dynamodb_pitr_enabled(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside dynamodb :: dynamodb_pitr_enabled()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id5.5'
     compliance_type = "Dynamodb pitr enabled"
     description = "Checks that point in time recovery (PITR) is enabled for Amazon DynamoDB tables"
     resource_type = "Dynamodb"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('dynamodb')
+    # regions = self.session.get_available_regions('dynamodb')
 
     for region in regions:
         try:
             client = self.session.client('dynamodb', region_name=region)
 
             dynamodb_tables = list_dynamodb_tables(client)
             for table in dynamodb_tables:
@@ -50,11 +53,13 @@
         except ClientError as e:
             logger.error("Something went wrong with region {}: {}".format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/dynamodb/utils.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/ec2/compliance.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/ec2/compliance.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
 
-from OBP_reliability_pillar.ec2.ec2_instance_detailed_monitoring_enabled import ec2_instance_detailed_monitoring_enabled
+from OBP_reliability_pillar.ec2.ec2_instance_detailed_monitoring_enabled import \
+    ec2_instance_detailed_monitoring_enabled
 from OBP_reliability_pillar.ec2.instance_in_vpc import instance_in_vpc
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # returns consolidated dynamodb compliance
-def ec2_compliance(self) -> list:
+def ec2_compliance(self, regions) -> list:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_compliance()")
 
     response = [
-        ec2_instance_detailed_monitoring_enabled(self),
-        instance_in_vpc(self)
+        # Already covered in monitoring module, hence commenting here
+        # ec2_instance_detailed_monitoring_enabled(self),
+        instance_in_vpc(self, regions)
     ]
 
-    return response
+    return response
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,19 @@
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_instance_detailed_monitoring_enabled")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.30'
     compliance_type = "EC2 instance detailed monitoring enabled"
     description = "Checks if detailed monitoring is enabled for EC2 instances."
     resource_type = "EC2 Instance"
+    risk_level = 'Low'
 
     regions = self.session.get_available_regions('ec2')
 
     for region in regions:
         try:
             client = self.session.client('ec2', region_name=region)
             marker = ''
@@ -49,11 +51,13 @@
         except botocore.exceptions.ClientError as e:
             logger.error('Something went wrong with region {}: {}'.format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/ec2/instance_in_vpc.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/ec2/instance_in_vpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import botocore
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def instance_in_vpc(self) -> dict:
+def instance_in_vpc(self, regions: list) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 : instance_in_vpc()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.67'
     compliance_type = "EC2 instance In VPC"
     description = "Checks if your EC2 instances belong to a virtual private cloud (VPC)"
     resource_type = "EC2 Instance"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('ec2')
+    # regions = self.session.get_available_regions('ec2')
 
     for region in regions:
         try:
             client = self.session.client('ec2', region_name=region)
             marker = ''
             while True:
                 response = client.describe_instances(
@@ -51,11 +54,13 @@
         except botocore.exceptions.ClientError as e:
             logger.error('Something went wrong with region {}: {}'.format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 
 from botocore.exceptions import ClientError
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def enhanced_health_reporting_enabled(self) -> dict:
+def enhanced_health_reporting_enabled(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside elastic_beanstalk :: enhanced_health_reporting_enabled()")
 
-    regions = self.session.get_available_regions('elasticbeanstalk')
+    # regions = self.session.get_available_regions('elasticbeanstalk')
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.13'
     compliance_type = "Beanstalk Enhanced Health Reporting Enabled"
     description = "Checks if an AWS Elastic Beanstalk environment is configured for enhanced health reporting. The rule is COMPLIANT if the environment is configured for enhanced health reporting."
     resource_type = "Elastic Beanstalk"
+    risk_level = 'Medium'
 
     for region in regions:
         try:
             client = self.session.client('elasticbeanstalk', region_name=region)
             marker = ''
             while True:
                 if marker == '' or marker is None:
@@ -49,11 +52,13 @@
         except ClientError as e:
             logger.error("Something went wrong with region {}: {}".format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_load_balancer/compliance.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_load_balancer/compliance.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 from OBP_reliability_pillar.elastic_load_balancer.elb_deletion_protection import elb_deletion_protection_enabled
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # returns consolidated dynamodb compliance
-def elb_compliance(self) -> list:
+def elb_compliance(self, regions) -> list:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside elastic_load_balancer :: elb_compliance()")
 
     response = [
-        cross_zone_load_balancing_enabled(self),
-        elb_deletion_protection_enabled(self)
+        cross_zone_load_balancing_enabled(self, regions),
+        elb_deletion_protection_enabled(self, regions)
     ]
 
-    return response
+    return response
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from botocore.exceptions import ClientError
 import logging
 
-from OBP_reliability_pillar.elastic_load_balancer.utils import list_elb
+from OBP_reliability_pillar.elastic_load_balancer.utils import *
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def cross_zone_load_balancing_enabled(self) -> dict:
+def cross_zone_load_balancing_enabled(self, regions) -> dict:
     """
-
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside elastic_load_balancer :: cross_zone_load_balancing_enabled()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.47'
     compliance_type = "Cross Zone Load Balancing Enabled"
     description = "Checks if cross zone load balancing is enabled or not"
     resource_type = "Elastic Load Balancer"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('elb')
+    # regions = self.session.get_available_regions('elb')
 
     for region in regions:
         try:
             client = self.session.client('elb', region_name=region)
             elb_list = list_elb(self, region)
 
             for elb in elb_list:
@@ -41,11 +43,13 @@
         except ClientError as e:
             logger.error("Something went wrong with the regions {}: {}".format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
-    }
+        'Description': description,
+        'Risk Level': risk_level
+    }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import logging
 
 from botocore.exceptions import ClientError
 
-from OBP_reliability_pillar.elastic_load_balancer.utils import list_elb
+from OBP_reliability_pillar.elastic_load_balancer.utils import *
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # checks compliance for elb deletion protection enabled
-def elb_deletion_protection_enabled(self) -> dict:
+def elb_deletion_protection_enabled(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside elastic_load_balancer :: elb_deletion_protection_enabled()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.48'
     compliance_type = "ELB Deletion Protection Enabled"
     description = "Checks whether an Elastic Load Balancer has deletion protection enabled"
     resource_type = "Elastic Load Balancer"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('elbv2')
+    # regions = self.session.get_available_regions('elbv2')
 
     for region in regions:
         try:
             client = self.session.client('elbv2', region_name=region)
-            elb_list = list_elb(self, region)
+            elb_list = list_elb_v2(self, region)
 
             for elb in elb_list:
                 response = client.describe_load_balancer_attributes(
                     LoadBalancerArn=elb['arn']
                 )
                 for attr in response['Attributes']:
                     if attr['Key'] == 'deletion_protection.enabled':
@@ -44,11 +47,13 @@
         except ClientError as e:
             logger.error("Something went wrong with the regions {}: {}".format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_load_balancer/utils.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_load_balancer/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,64 @@
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # returns the list of load balancers
-def list_elb(self, region: str)-> list:
+def list_elb_v2(self, region: str) -> list:
     logger.info(" ---Inside list_elb()")
     res = []
-    client = self.session.client('elb', region_name= region)
+    client = self.session.client('elbv2', region_name=region)
 
     marker = ''
     while True:
         if marker == '' or marker is None:
             response = client.describe_load_balancers()
         else:
             response = client.describe_load_balancers(
                 Marker=marker
             )
-        for lb in response['LoadBalancerDescriptions']:
+        for lb in response['LoadBalancers']:
             temp = {
                 'name': lb['LoadBalancerName'],
                 'arn': lb['LoadBalancerArn']
             }
             res.append(temp)
 
         try:
             marker = response['NextMarker']
             if marker == '':
                 break
+        except KeyError:
+            break
+
+    return res
+
+
+def list_elb(self, region: str) -> list:
+    logger.info(" ---Inside list_elb()")
+    res = []
+    client = self.session.client('elb', region_name=region)
+
+    marker = ''
+    while True:
+        if marker == '' or marker is None:
+            response = client.describe_load_balancers()
+        else:
+            response = client.describe_load_balancers(
+                Marker=marker
+            )
+        for lb in response['LoadBalancerDescriptions']:
+            temp = {
+                'name': lb['LoadBalancerName']
+            }
+            res.append(temp)
+
+        try:
+            marker = response['NextMarker']
+            if marker == '':
+                break
         except KeyError:
             break
 
     return res
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 from botocore.exceptions import ClientError
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # checks compliance for elastic search in vpc only
-def elastic_search_in_vpc_only(self) -> dict:
+def elastic_search_in_vpc_only(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside elastic_search :: elastic_search_in_vpc_only()")
 
     result = True
     failReason = ""
     offenders = []
+    control_id = 'Id3.43'
     compliance_type = "Elastic search in vpc"
     description = "Checks if Elasticsearch domains are in Amazon Virtual Private Cloud (Amazon VPC)"
     resource_type = "Elastic Search"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('es')
+    # regions = self.session.get_available_regions('es')
 
     for region in regions:
         try:
             client = self.session.client('es', region_name=region)
             domain_names = client.list_domain_names()
 
             for domain in domain_names['DomainNames']:
@@ -39,16 +42,18 @@
                 except KeyError:
                     result = False
                     failReason = "Elastic search domain does not reside in a vpc"
                     offenders.append(domain['DomainName'])
 
         except ClientError as e:
             logger.error("Something wrong with the region {}: {}".format(region, e))
-
+    print('dheeraj')
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,23 +12,25 @@
     :return:
     """
     logger.info(" ---Inside guard_duty :: guard_duty_enabled()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.55'
     compliance_type = "Guard Duty Enabled"
     description = "Checks if Amazon GuardDuty is enabled in your AWS account and region"
     resource_type = "Guard Duty"
+    risk_level = 'Medium'
 
     regions = self.session.get_available_regions('guardduty')
 
     for region in regions:
         try:
-            client = self.session.client('guardduty')
+            client = self.session.client('guardduty', region_name=region)
             detectors = []
             marker = ''
             while True:
                 if marker == '' or marker is None:
                     response = client.list_detectors()
                 else:
                     response = client.list_detectors(
@@ -50,11 +52,13 @@
         except ClientError as e:
             logger.error("Something went wrong with the region {}: {}".format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/lambdafn/compliance.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/lambdafn/compliance.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 from OBP_reliability_pillar.lambdafn.lambda_inside_vpc import lambda_inside_vpc
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # checks aws lambda compliance
-def lambda_compliance(self) -> dict:
+def lambda_compliance(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside lambdafn :: lambda_compliance()")
     response = [
-        lambda_dlq_check(self),
-        lambda_inside_vpc(self),
+        # Already covered in monitoring module, hence commenting here
+        # lambda_dlq_check(self),
+        lambda_inside_vpc(self, regions),
     ]
 
     return response
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,17 +14,19 @@
     :return:
     """
     logger.info(" ---Inside lambdafn :: lambda_dlq_check()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id13.1'
     compliance_type = "Lambda DLQ check"
     description = "Checks whether an AWS Lambda function is configured with a dead-letter queue."
     resource_type = "AWS Lambda"
+    risk_level = 'Medium'
 
     regions = self.session.get_available_regions('lambda')
 
     for region in regions:
         try:
             client = self.session.client('lambda', region_name=region)
             function_lst = list_lambda_functions(client)
@@ -45,11 +47,13 @@
         except ClientError as e:
             logger.error("Something went wrong with the region {}: {}".format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 from OBP_reliability_pillar.lambdafn.utils import list_lambda_functions
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # checks the compliance for lambda-inside-vpc
-def lambda_inside_vpc(self) -> dict:
+def lambda_inside_vpc(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside lambda :: lambda_inside_vpc()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.72'
     compliance_type = "Lambda DLQ check"
     description = "Checks whether an AWS Lambda function is configured with a dead-letter queue."
     resource_type = "AWS Lambda"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('lambda')
+    # regions = self.session.get_available_regions('lambda')
 
     for region in regions:
         try:
             client = self.session.client('lambda', region_name=region)
             function_lst = list_lambda_functions(client)
 
             for function in function_lst:
@@ -40,11 +43,13 @@
         except ClientError as e:
             logger.error("Something went wrong with the region {}: {}".format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/lambdafn/utils.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/lambdafn/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,45 @@
 import logging
 import botocore
+
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
+
 # checks compliance.py for rds automatic minor version enabled
-def rds_automatic_minor_version_upgrade_enabled(self) -> dict:
+def rds_automatic_minor_version_upgrade_enabled(self, rds_instances: dict) -> dict:
     """
+    :param rds_instances:
     :param self:
     :return dict: AWS RDS automatic minor version enabled compliance.py
     """
     logger.info(" ---Inside rds :: rds_automatic_minor_version_upgrade_enabled()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id5.12'
     compliance_type = "RDS instance automatic minor version upgrade enabled"
     description = "Checks if automatic minor version upgrade is enabled for RDS instances."
     resource_type = "RDS Instance"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('rds')
+    # regions = self.session.get_available_regions('rds')
 
-    for region in regions:
-        try:
-            client = self.session.client('rds', region_name=region)
-            marker = ''
-            while True:
-                response = client.describe_db_instances(
-                    MaxRecords=100,
-                    Marker=marker
-                )
-                for instance in response['DBInstances']:
-                    minor_version = instance['AutoMinorVersionUpgrade']
-                    if not minor_version:
-                        result = False
-                        failReason = "Automatic minor version upgrade is not enabled"
-                        offenders.append(region+': '+instance['DBInstanceIdentifier'])
-
-                try:
-                    marker = response['Marker']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
-        except botocore.exceptions.ClientError as e:
-            logger.error('Something went wrong with region {}: {}'.format(region, e))
+    for region, instances in rds_instances.items():
+        for instance in instances:
+            minor_version = instance['AutoMinorVersionUpgrade']
+            if not minor_version:
+                result = False
+                failReason = "Automatic minor version upgrade is not enabled"
+                offenders.append(region + ': ' + instance['DBInstanceIdentifier'])
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
-    }
+        'Description': description,
+        'Risk Level': risk_level
+    }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/rds_backup_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/rds_backup_enabled.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,68 @@
-import logging
-
-from botocore.exceptions import ClientError
-
-logging.basicConfig(level=logging.INFO)
-logger = logging.getLogger()
-
-
-# Checks compliance for rds backup enabled
-def rds_backup_enabled(self) -> dict:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(" ---Inside rds :: rds_backup_enabled()")
-
-    result = True
-    failReason = ''
-    offenders = []
-    compliance_type = "RDS instance backup enabled"
-    description = "Checks if RDS DB instances have backups enabled"
-    resource_type = "RDS Instance"
-
-    regions = self.session.get_available_regions('rds')
-
-    for region in regions:
-        try:
-            client = self.session.client('rds', region_name=region)
-            marker = ''
-            while True:
-                if marker == '' or marker is None:
-                    response = client.describe_db_instances(
-                        MaxRecords=100
-                    )
-                else:
-                    response = client.describe_db_instances(
-                        MaxRecords=100,
-                        Marker=marker
-                    )
-                for instance in response['DBInstances']:
-                    retention_period = instance['BackupRetentionPeriod']
-                    if retention_period <= 0:
-                        result = False
-                        failReason = 'RDS Instance backup is not enabled'
-                        offenders.append(instance['DBInstanceIdentifier'])
-
-                try:
-                    marker = response['Marker']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
-        except ClientError as e:
-            logger.error('Something went wrong with the region {}: {}'.format(region,e))
-
-    return {
-        'Result': result,
-        'failReason': failReason,
-        'resource_type': resource_type,
-        'Offenders': offenders,
-        'Compliance_type': compliance_type,
-        'Description': description
-    }
-
+# import logging
+#
+# from botocore.exceptions import ClientError
+#
+# logging.basicConfig(level=logging.INFO)
+# logger = logging.getLogger()
+#
+#
+# # Checks compliance for rds backup enabled
+# def rds_backup_enabled(self) -> dict:
+#     """
+#     :param self:
+#     :return:
+#     """
+#     logger.info(" ---Inside rds :: rds_backup_enabled()")
+#
+#     result = True
+#     failReason = ''
+#     offenders = []
+#     control_id = ''
+#     compliance_type = "RDS instance backup enabled"
+#     description = "Checks if RDS DB instances have backups enabled"
+#     resource_type = "RDS Instance"
+#     risk_level = 'High'
+#
+#     regions = self.session.get_available_regions('rds')
+#
+#     for region in regions:
+#         try:
+#             client = self.session.client('rds', region_name=region)
+#             marker = ''
+#             while True:
+#                 if marker == '' or marker is None:
+#                     response = client.describe_db_instances(
+#                         MaxRecords=100
+#                     )
+#                 else:
+#                     response = client.describe_db_instances(
+#                         MaxRecords=100,
+#                         Marker=marker
+#                     )
+#                 for instance in response['DBInstances']:
+#                     retention_period = instance['BackupRetentionPeriod']
+#                     if retention_period <= 0:
+#                         result = False
+#                         failReason = 'RDS Instance backup is not enabled'
+#                         offenders.append(instance['DBInstanceIdentifier'])
+#
+#                 try:
+#                     marker = response['Marker']
+#                     if marker == '':
+#                         break
+#                 except KeyError:
+#                     break
+#         except ClientError as e:
+#             logger.error('Something went wrong with the region {}: {}'.format(region,e))
+#
+#     return {
+#         'Result': result,
+#         'failReason': failReason,
+#         'resource_type': resource_type,
+#         'ControlId': control_id,
+#         'Offenders': offenders,
+#         'Compliance_type': compliance_type,
+#         'Description': description,
+#         'Risk Level': risk_level
+#     }
+#
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import logging
 import botocore
+
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
+
 # checks compliance.py for rds automatic minor version enabled
 def rds_enhanced_monitoring_enabled(self) -> dict:
     """
 
     :param self:
     :return dict: rds enhanced monitoring enabled compliance.py details
     """
     logger.info(" ---Inside rds :: rds_enhanced_monitoring_enabled()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.74'
     compliance_type = "RDS instance enhanced monitoring enabled"
     description = "Checks if enhanced monitoring is enabled for RDS instances."
     resource_type = "RDS Instance"
+    risk_level = 'Medium'
 
     regions = self.session.get_available_regions('rds')
 
     for region in regions:
         try:
             client = self.session.client('rds', region_name=region)
             marker = ''
@@ -31,26 +35,28 @@
                     Marker=marker
                 )
                 for instance in response['DBInstances']:
                     monitoring_interval = int(instance['MonitoringInterval'])
                     if monitoring_interval <= 0:
                         result = False
                         failReason = "enhanced monitoring is not enabled"
-                        offenders.append(region+': '+instance['DBInstanceIdentifier'])
+                        offenders.append(region + ': ' + instance['DBInstanceIdentifier'])
 
                 try:
                     marker = response['Marker']
                     if marker == '':
                         break
                 except KeyError:
                     break
         except botocore.exceptions.ClientError as e:
             logger.error('Something went wrong with region {}: {}'.format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
-    }
+        'Description': description,
+        'Risk Level': risk_level
+    }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,45 @@
 import logging
 import botocore
+
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
+
 # checks compliance.py for rds automatic minor version enabled
-def rds_instance_deletion_protection_enabled(self) -> dict:
+def rds_instance_deletion_protection_enabled(self, rds_instances: dict) -> dict:
     """
-
-    @param self:
-    @return dict: AWS RDS instance deletion protection enabled compliance.py
+    :param self:
+    :param rds_instances:
+    :return:
     """
     logger.info(" ---Inside rds :: rds_instance_deletion_protection_enabled()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.76'
     compliance_type = "RDS instance deletion protection enabled"
     description = "Checks if deletion protection is enabled for RDS instances."
     resource_type = "RDS Instance"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('rds')
+    # regions = self.session.get_available_regions('rds')
 
-    for region in regions:
-        try:
-            client = self.session.client('rds', region_name=region)
-            marker = ''
-            while True:
-                response = client.describe_db_instances(
-                    MaxRecords=100,
-                    Marker=marker
-                )
-                for instance in response['DBInstances']:
-                    deletion_protection = instance['DeletionProtection']
-                    if not deletion_protection:
-                        result = False
-                        failReason = "Deletion protection is not enabled is not enabled"
-                        offenders.append(region+': '+instance['DBInstanceIdentifier'])
-
-                try:
-                    marker = response['Marker']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
-        except botocore.exceptions.ClientError as e:
-            logger.error('Something went wrong with region {}: {}'.format(region, e))
+    for region, instances in rds_instances.items():
+        for instance in instances:
+            deletion_protection = instance['DeletionProtection']
+            if not deletion_protection:
+                result = False
+                failReason = "Deletion protection is not enabled is not enabled"
+                offenders.append(region + ': ' + instance['DBInstanceIdentifier'])
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
-    }
+        'Description': description,
+        'Risk Level': risk_level
+    }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,44 @@
 import logging
 import botocore
+
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
+
 # checks compliance.py for rds automatic minor version enabled
-def rds_multi_az_support_enabled(self) -> dict:
+def rds_multi_az_support_enabled(self, rds_instances: dict) -> dict:
     """
-
-    @param self:
-    @return dict: AWS RDS multi az support enabled compliance.py
+    :param self:
+    :param rds_instances:
     """
     logger.info(" ---Inside rds :: rds_multi_az_support_enabled()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.78'
     compliance_type = "RDS multi az support enabled"
     description = "Checks if multi az support is enabled for RDS instances."
     resource_type = "RDS Instance"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('rds')
+    # regions = self.session.get_available_regions('rds')
 
-    for region in regions:
-        try:
-            client = self.session.client('rds', region_name=region)
-            marker = ''
-            while True:
-                response = client.describe_db_instances(
-                    MaxRecords=100,
-                    Marker=marker
-                )
-                for instance in response['DBInstances']:
-                    multi_az = instance['MultiAZ']
-                    if not multi_az:
-                        result = False
-                        failReason = "Multi az support is not enabled"
-                        offenders.append(region+': '+instance['DBInstanceIdentifier'])
-
-                try:
-                    marker = response['Marker']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
-        except botocore.exceptions.ClientError as e:
-            logger.error('Something went wrong with region {}: {}'.format(region, e))
+    for region, instances in rds_instances.items():
+        for instance in instances:
+            multi_az = instance['MultiAZ']
+            if not multi_az:
+                result = False
+                failReason = "Multi az support is not enabled"
+                offenders.append(region + ': ' + instance['DBInstanceIdentifier'])
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
-    }
+        'Description': description,
+        'Risk Level': risk_level
+    }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/redshift/redshift_backup_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,58 +2,48 @@
 
 from botocore.exceptions import ClientError
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def redshift_backup_enabled(self) -> dict:
+# checks compliance for redshift cluster maintenance settings check
+def redshift_cluster_maintenance_settings_check(self, redshift_clusters) -> dict:
     """
+    :param redshift_clusters:
     :param self:
     :return:
     """
-    logger.info(" ---Inside redshift :: redshift_backup_enabled()")
+    logger.info(" ---Inside redshift :: redshift_cluster_maintenance_settings_check()")
 
     result = True
     failReason = ''
     offenders = []
-    compliance_type = "Redshift Backup Enabled"
-    description = "Checks if backup is enabled on redshift cluster or not"
+    control_id = 'Id3.83'
+    compliance_type = "Redshift cluster maintenance settings check"
+    description = "Checks whether Amazon Redshift clusters have the specified maintenance settings"
     resource_type = "Redshift"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('redshift')
+    # regions = self.session.get_available_regions('redshift')
 
-    for region in regions:
-        try:
-            client = self.session.client('redshift', region_name=region)
-            marker = ''
-            while True:
-                if marker == '' or marker is None:
-                    response = client.describe_clusters()
-                else:
-                    response = client.describe_clusters(
-                        Marker=marker
-                    )
-                for cluster in response['Clusters']:
-                    retention_period = cluster['AutomatedSnapshotRetentionPeriod']
-                    if retention_period <= 0:
-                        result = False
-                        failReason = "Redshift backup is not enabled"
-                        offenders.append(region + ': ' + cluster['ClusterIdentifier'])
-
-                try:
-                    marker = response['Marker']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
-        except ClientError as e:
-            logger.error("Something went wrong with region {}: {}".format(region, e))
+    for region, clusters in redshift_clusters.items():
+        for cluster in clusters:
+            version_upgrade = cluster['AllowVersionUpgrade']
+            window = cluster['PreferredMaintenanceWindow']
+            automated_snapshot_retention_period = cluster['AutomatedSnapshotRetentionPeriod']
+
+            if not version_upgrade and automated_snapshot_retention_period > 0:
+                result = False
+                failReason = 'allowVersionUpgrade is not enabled'
+                offenders.append(cluster['ClusterIdentifier'])
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
-    }
+        'Description': description,
+        'Risk Level': risk_level
+    }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/redshift/compliance.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,57 @@
 import logging
-
-from botocore.exceptions import ClientError
+from OBP_reliability_pillar.redshift.redshift_backup_enabled import redshift_backup_enabled
+from OBP_reliability_pillar.redshift.redshift_cluster_maintenancesettings_check import \
+    redshift_cluster_maintenance_settings_check
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
-# checks compliance for redshift cluster maintenance settings check
-def redshift_cluster_maintenance_settings_check(self) -> dict:
+
+# returns the list of redshift clusters
+def list_redshift_clusters(self, regions) -> dict:
     """
     :param self:
+    :param regions:
     :return:
     """
-    logger.info(" ---Inside redshift :: redshift_cluster_maintenance_settings_check()")
-
-    result = True
-    failReason = ''
-    offenders = []
-    compliance_type = "Redshift cluster maintenance settings check"
-    description = "Checks whether Amazon Redshift clusters have the specified maintenance settings"
-    resource_type = "Redshift"
-
-    regions = self.session.get_available_regions('redshift')
+    logger.info(" ---Inside redshift :: list_redshift_clusters()--- ")
+    redshift_clusters = {}
 
     for region in regions:
-        try:
-            client = self.session.client('redshift', region_name=region)
-            marker = ''
-            while True:
-                if marker == '' or marker is None:
-                    response = client.describe_clusters()
-                else:
-                    response = client.describe_clusters(
-                        Marker = marker
-                    )
-                for cluster in response['Clusters']:
-                    version_upgrade = cluster['AllowVersionUpgrade']
-                    window = cluster['PreferredMaintenanceWindow']
-                    automated_snapshot_retention_period = cluster['AutomatedSnapshotRetentionPeriod']
-
-                    if not version_upgrade and automated_snapshot_retention_period > 0:
-                        result = False
-                        failReason = 'allowVersionUpgrade is not enabled'
-                        offenders.append(cluster['ClusterIdentifier'])
-
-                try:
-                    marker = response['Marker']
-                    if marker == '':
-                        break
-                except KeyError:
+        client = self.session.client('redshift', region_name=region)
+        marker = ''
+        while True:
+            if marker == '' or marker is None:
+                response = client.describe_clusters()
+            else:
+                response = client.describe_clusters(
+                    Marker=marker
+                )
+            redshift_clusters.setdefault(region, []).extend(response['Clusters'])
+
+            try:
+                marker = response['Marker']
+                if marker == '':
                     break
+            except KeyError:
+                break
+
+    return redshift_clusters
 
-        except ClientError as e:
-            logger.error("Something went wrong with the region {}: {}".format(region, e))
 
-    return {
-        'Result': result,
-        'failReason': failReason,
-        'resource_type': resource_type,
-        'Offenders': offenders,
-        'Compliance_type': compliance_type,
-        'Description': description
-    }
+# returns consolidated dynamodb compliance
+def redshift_compliance(self, regions) -> list:
+    """
+    :param regions:
+    :param self:
+    :return:
+    """
+    redshift_clusters = self.list_redshift_clusters(regions)
+    logger.info(" ---Inside redshift :: redshift_compliance()")
 
+    response = [
+        redshift_backup_enabled(self, redshift_clusters),
+        redshift_cluster_maintenance_settings_check(self, redshift_clusters),
+    ]
 
+    return response
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/s3/compliance.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/s3/compliance.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,22 +4,39 @@
 from OBP_reliability_pillar.s3.s3_bucket_replication_enabled import s3_bucket_replication_enabled
 from OBP_reliability_pillar.s3.s3_bucket_versioning_enabled import s3_bucket_versioning_enabled
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
+#     list s3 buckets
+def list_s3_buckets(self) -> list:
+    """
+    :return:
+    """
+    logger.info(" ---Inside utils :: list_s3_buckets")
+
+    buckets = []
+
+    client = self.session.client('s3')
+    response = client.list_buckets()
+
+    return response['Buckets']
+
+
 # returns consolidated dynamodb compliance
 def s3_compliance(self) -> list:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside s3 :: s3_compliance()")
 
+    buckets = self.list_s3_buckets()
+
     response = [
-        s3_bucket_replication_enabled(self),
-        s3_bucket_versioning_enabled(self),
-        s3_bucket_default_lock_enabled(self)
+        s3_bucket_replication_enabled(self, buckets),
+        s3_bucket_versioning_enabled(self, buckets),
+        s3_bucket_default_lock_enabled(self, buckets)
     ]
 
-    return response
+    return response
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,33 +3,36 @@
 from botocore.exceptions import ClientError
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # Checks for the compliance s3 bucket default lock enabled
-def s3_bucket_default_lock_enabled(self) -> dict:
+def s3_bucket_default_lock_enabled(self, buckets) -> dict:
     """
+    :param buckets:
     :param self:
     :return:
     """
     logger.info(" ---Inside s3 :: s3_bucket_default_lock_enabled")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.88'
     compliance_type = "S3 bucket default lock enabled"
     description = "Checks whether Amazon S3 bucket has lock enabled, by default"
     resource_type = "S3"
+    risk_level = 'Medium'
 
     client = self.session.client('s3')
 
-    response = client.list_buckets()
+    # response = client.list_buckets()
 
-    for bucket in response['Buckets']:
+    for bucket in buckets:
         try:
             response = client.get_object_lock_configuration(
                 Bucket=bucket['Name']
             )
             object_lock_status = response['ObjectLockConfiguration']['ObjectLockEnabled']
             if object_lock_status != 'Enabled':
                 result = False
@@ -44,11 +47,13 @@
             failReason = 'Configuration not found'
             offenders.append(bucket['Name'])
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
+
 # checks the compliance.py for s3 bucket versioning enabled
-def s3_bucket_replication_enabled(self):
+def s3_bucket_replication_enabled(self, buckets):
     """
-
+    :param buckets:
     :param self:
-    :return dict: details of s3 bucket versioning enabled compliance.py
+    :return dict: details of s3 bucket replication enabled compliance.py
     """
-    logger.info(" ---Inside s3 :: s3_bucket_versioning_enabled()")
+    logger.info(" ---Inside s3 :: s3_bucket_replication_enabled()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id3.91'
     compliance_type = "S3 bucket replication enabled"
     description = "Checks if bucket replication is enabled in s3 buckets."
     resource_type = "S3 Buckets"
+    risk_level = 'High'
 
     client = self.session.client('s3')
-    response = client.list_buckets()
+    # response = client.list_buckets()
 
-    for bucket in response['Buckets']:
+    for bucket in buckets:
         bucket_name = bucket['Name']
 
         try:
             resp = client.get_bucket_replication(
                 Bucket=bucket_name
             )
 
@@ -43,11 +46,13 @@
             failReason = "Either bucket replication is not enabled or configuration not found"
             offenders.append(bucket_name)
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
+
 # checks the compliance.py for s3 bucket versioning enabled
-def s3_bucket_versioning_enabled(self):
+def s3_bucket_versioning_enabled(self, buckets):
     """
 
+    :param buckets:
     :param self:
     :return dict: details of s3 bucket versioning enabled compliance.py
     """
     logger.info(" ---Inside s3 :: s3_bucket_versioning_enabled()")
 
     result = True
     failReason = ''
     offenders = []
+    control_id = 'Id1.20'
     compliance_type = "S3 bucket versioning enabled"
     description = "Checks if bucket versioning is enabled in s3 buckets."
     resource_type = "S3 Buckets"
+    risk_level = 'Medium'
 
     client = self.session.client('s3')
-    response = client.list_buckets()
+    # response = client.list_buckets()
 
-    for bucket in response['Buckets']:
+    for bucket in buckets:
         bucket_name = bucket['Name']
 
         try:
             resp = client.get_bucket_versioning(
                 Bucket=bucket_name,
             )
             status = resp['Status']
@@ -41,11 +45,13 @@
             failReason = "Either bucket versioning is not enabled or configuration not found"
             offenders.append(bucket_name)
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
+        'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
-    }
+        'Description': description,
+        'Risk Level': risk_level
+    }
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar/security_hub/__init__.py` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar/security_hub/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-import botocore
-import logging
-
-logging.basicConfig(level=logging.INFO)
-logger = logging.getLogger()
-
-
-class security_hub:
-    def __init__(self, session):
-        """
-
-        :param session:
-        """
-        self.session = session
-
-    # checks compliance.py for security hub enabled
-    def security_hub_enabled(self) -> list:
-        logger.info(" ---Inside security_hub_enabled()")
-
-        result = True
-        failReason = ''
-        offenders = []
-        compliance_type = "security hub enabled"
-        description = "Checks if security hub is enabled or not"
-        resource_type = "Security hub"
-
-        client = self.session.client('securityhub')
-        try:
-            response = client.describe_hub()
-            # Scenario 1: SecurityHub is enabled for an AWS Account
-            if response:
-                pass
-        except botocore.exceptions.ClientError as error:
-            # Scenario 2: SecurityHub is not enabled for an AWS account.
-            if error.response['Error']['Code'] == 'InvalidAccessException':
-                result = False
-                offenders = []
-                failReason = "Security hub is disabled"
-
-
-        return [{
-            'Result': result,
-            'failReason': failReason,
-            'resource_type': resource_type,
-            'Offenders': offenders,
-            'Compliance_type': compliance_type,
-            'Description': description
-        }]
+# import botocore
+# import logging
+#
+# logging.basicConfig(level=logging.INFO)
+# logger = logging.getLogger()
+#
+#
+# class security_hub:
+#     def __init__(self, session):
+#         """
+#
+#         :param session:
+#         """
+#         self.session = session
+#
+#     # checks compliance.py for security hub enabled
+#     def security_hub_enabled(self) -> list:
+#         logger.info(" ---Inside security_hub_enabled()")
+#
+#         result = True
+#         failReason = ''
+#         offenders = []
+#         compliance_type = "security hub enabled"
+#         description = "Checks if security hub is enabled or not"
+#         resource_type = "Security hub"
+#
+#         client = self.session.client('securityhub', region_name='ap-south-1')
+#         try:
+#             response = client.describe_hub()
+#             # Scenario 1: SecurityHub is enabled for an AWS Account
+#             if response:
+#                 pass
+#         except botocore.exceptions.ClientError as error:
+#             # Scenario 2: SecurityHub is not enabled for an AWS account.
+#             if error.response['Error']['Code'] == 'InvalidAccessException':
+#                 result = False
+#                 offenders = []
+#                 failReason = "Security hub is disabled"
+#
+#         return [{
+#             'Result': result,
+#             'failReason': failReason,
+#             'resource_type': resource_type,
+#             'Offenders': offenders,
+#             'Compliance_type': compliance_type,
+#             'Description': description
+#         }]
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar.egg-info/PKG-INFO` & `OBP_reliability_pillar-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OBP-reliability-pillar
-Version: 0.0.9
+Name: OBP_reliability_pillar
+Version: 0.1.0
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `OBP_reliability_pillar-0.0.9/OBP_reliability_pillar.egg-info/SOURCES.txt` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.0.9/PKG-INFO` & `OBP_reliability_pillar-0.1.0/OBP_reliability_pillar.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OBP_reliability_pillar
-Version: 0.0.9
+Name: OBP-reliability-pillar
+Version: 0.1.0
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `OBP_reliability_pillar-0.0.9/README.md` & `OBP_reliability_pillar-0.1.0/README.md`

 * *Files identical despite different names*

