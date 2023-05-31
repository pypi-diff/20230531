# Comparing `tmp/csle_common-0.2.0.tar.gz` & `tmp/csle_common-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_common-0.2.0.tar", last modified: Sun Apr 30 12:36:20 2023, max compression
+gzip compressed data, was "csle_common-0.2.1.tar", last modified: Wed May 31 11:23:35 2023, max compression
```

## Comparing `csle_common-0.2.0.tar` & `csle_common-0.2.1.tar`

### file list

```diff
@@ -1,293 +1,290 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.864460 csle_common-0.2.0/
--rw-rw-r--   0 kim       (1000) kim       (1000)      685 2023-04-30 12:36:20.864460 csle_common-0.2.0/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-03-28 14:03:22.000000 csle_common-0.2.0/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1483 2023-04-30 12:36:20.864460 csle_common-0.2.0/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_common-0.2.0/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.804460 csle_common-0.2.0/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.808460 csle_common-0.2.0/src/csle_common/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 csle_common-0.2.0/src/csle_common/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.808460 csle_common-0.2.0/src/csle_common/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    67243 2023-04-30 06:59:23.000000 csle_common-0.2.0/src/csle_common/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.812460 csle_common-0.2.0/src/csle_common/consumer_threads/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4795 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_host_metrics_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3154 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_ossec_ids_log_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3207 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_snort_ids_log_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3202 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_snort_ids_rule_log_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2417 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/attacker_actions_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2807 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/avg_host_metrics_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3905 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/client_population_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2494 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/defender_actions_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2444 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4779 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/docker_stats_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2390 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/host_metrics_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2564 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/ossec_ids_log_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2493 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/snort_ids_log_consumer_thread.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.816460 csle_common-0.2.0/src/csle_common/controllers/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    37512 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/container_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17707 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/elk_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    48222 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/emulation_env_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2255 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/flags_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    71893 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/host_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11832 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/installation_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14738 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/kafka_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    23308 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/management_system_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    20424 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/ossec_ids_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5548 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/ovs_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3974 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/resource_constraints_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15201 2023-04-18 12:48:17.000000 csle_common-0.2.0/src/csle_common/controllers/sdn_controller_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1214 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/simulation_env_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    21969 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/snort_ids_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11243 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/topology_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    37012 2023-04-18 12:48:40.000000 csle_common-0.2.0/src/csle_common/controllers/traffic_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3839 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/users_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2884 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/vulnerabilities_controller.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.816460 csle_common-0.2.0/src/csle_common/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.816460 csle_common-0.2.0/src/csle_common/dao/datasets/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/datasets/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5914 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/datasets/statistics_dataset.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5674 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/datasets/traces_dataset.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.816460 csle_common-0.2.0/src/csle_common/dao/docker/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/docker/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6387 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/docker/docker_container_metadata.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3595 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/docker/docker_env_metadata.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.820460 csle_common-0.2.0/src/csle_common/dao/domain_randomization/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/domain_randomization/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2141 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/domain_randomization/node_randomizer_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      556 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/domain_randomization/randomization_space.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2900 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/domain_randomization/randomization_space_config.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.820460 csle_common-0.2.0/src/csle_common/dao/emulation_action/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.820460 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11189 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    19992 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2172 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      362 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_outcome.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      295 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1728 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_masscan_actions.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1517 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_network_service_actions.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1551 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nikto_actions.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    29225 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nmap_actions.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12817 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_shell_actions.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2091 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_stopping_actions.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.824460 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6875 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4063 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      221 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action_id.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      286 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action_outcome.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      247 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4705 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_stopping_actions.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.828460 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      953 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nikto_scan_result.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1997 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nikto_vuln.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      192 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_addr_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1938 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_brute_credentials.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2523 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_hop.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3104 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_host_result.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      199 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_host_status.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      395 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_http_enum.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      411 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_http_grep.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1174 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_os.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3715 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_port.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      199 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_port_status.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1007 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_scan_result.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2326 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_trace.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2546 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_vuln.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      400 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_vulscan.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.840460 csle_common-0.2.0/src/csle_common/dao/emulation_config/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4068 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/beats_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3182 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/client_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     9637 2023-04-01 08:34:56.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/client_population_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      343 2023-04-01 08:34:56.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/client_population_process_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2576 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/cluster_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2926 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/cluster_node.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    37157 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4143 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/connection_setup_dto.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4084 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/container_network.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7691 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/containers_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4325 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/credential.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4829 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/default_network_firewall_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5296 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/docker_stats_manager_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3418 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/docker_stats_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7236 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/elk_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3728 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/elk_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    21925 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_env_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7640 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_env_generation_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7486 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_env_state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2392 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_execution.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7851 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_execution_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    18879 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_metrics_time_series.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2768 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_simulation_trace.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3406 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_statistics_windowed.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    42526 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_trace.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3693 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/flag.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3446 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/flags_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4658 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/host_manager_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3103 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/host_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7618 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/kafka_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3108 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/kafka_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3550 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/kafka_topic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5079 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/network_service.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6950 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_beats_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7334 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_container_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8495 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_firewall_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3630 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_flags_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15661 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_network_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5446 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_resources_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3052 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_services_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5232 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_traffic_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3633 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_users_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5560 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_vulnerability_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5008 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/ossec_ids_manager_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3328 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/ossec_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3016 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/ovs_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5399 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/ovs_switch_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      316 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/packet_delay_distribution_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      269 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/packet_loss_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3214 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/resources_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3888 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/ryu_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7312 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/sdn_controller_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      205 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/sdn_controller_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3562 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/services_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4910 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/snort_ids_manager_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3618 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/snort_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      254 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/static_emulation_attacker_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3503 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/topology_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4287 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/traffic_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3216 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/traffic_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      782 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/transport_protocol.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2435 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/user.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3431 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/users_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3787 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/vulnerabilities_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      302 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/vulnerability_type.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.840460 csle_common-0.2.0/src/csle_common/dao/emulation_observation/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.844460 csle_common-0.2.0/src/csle_common/dao/emulation_observation/attacker/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/attacker/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    20660 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_machine_observation_state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10470 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_observation_state.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.844460 csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6143 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/emulation_connection_observation_state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6055 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/emulation_port_observation_state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6278 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/emulation_vulnerability_observation_state.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.844460 csle_common-0.2.0/src/csle_common/dao/emulation_observation/defender/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/defender/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12266 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/defender/emulation_defender_machine_observation_state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    22453 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/defender/emulation_defender_observation_state.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.844460 csle_common-0.2.0/src/csle_common/dao/encoding/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/encoding/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      411 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/encoding/np_encoder.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.844460 csle_common-0.2.0/src/csle_common/dao/jobs/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/jobs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7391 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/jobs/data_collection_job_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4781 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/jobs/system_identification_job_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5823 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/jobs/training_job_config.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.844460 csle_common-0.2.0/src/csle_common/dao/management/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/management/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3542 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/management/management_user.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2775 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/management/session_token.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.852460 csle_common-0.2.0/src/csle_common/dao/simulation_config/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1073 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/action.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2022 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/action_space_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      483 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/agent_log.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      747 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/base_env.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1228 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/env_parameter.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1216 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/env_parameters_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1312 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/initial_state_distribution_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1302 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/joint_action_space_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1163 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/joint_observation_space_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1242 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/observation.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1505 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/observation_function_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5039 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/observation_space_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1226 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/player_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1271 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/players_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1047 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/reward_function_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11210 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/simulation_env_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      337 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/simulation_env_input_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5489 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/simulation_trace.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1451 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1274 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/state_space_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      157 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/state_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      166 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/time_step_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1121 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/transition_operator_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      159 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/value_type.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.852460 csle_common-0.2.0/src/csle_common/dao/system_identification/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2998 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/empirical_conditional.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6116 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/empirical_system_model.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    29651 2023-04-18 12:47:23.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/emulation_statistics.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7292 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/gaussian_mixture_conditional.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6623 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/gaussian_mixture_system_model.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5215 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/gp_conditional.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6461 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/gp_system_model.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3260 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/system_identification_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      768 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/system_model.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      219 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/system_model_type.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.860460 csle_common-0.2.0/src/csle_common/dao/training/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      633 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/agent_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6794 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/alpha_vectors_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7536 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/dqn_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4362 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/experiment_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3648 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/experiment_execution.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3222 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/experiment_result.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11703 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/fnn_with_softmax_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1959 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/hparam.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7245 2023-04-30 06:59:23.000000 csle_common-0.2.0/src/csle_common/dao/training/linear_threshold_stopping_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14240 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14042 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/multi_threshold_stopping_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      179 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/player_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      963 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      320 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/policy_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7603 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/ppo_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4763 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/random_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5459 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/tabular_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4809 2023-04-30 06:59:23.000000 csle_common-0.2.0/src/csle_common/dao/training/vector_policy.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.860460 csle_common-0.2.0/src/csle_common/logging/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/logging/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      624 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/logging/custom_formatter.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2646 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/logging/log.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.860460 csle_common-0.2.0/src/csle_common/metastore/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/metastore/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   228115 2023-04-30 06:59:23.000000 csle_common-0.2.0/src/csle_common/metastore/metastore_facade.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.860460 csle_common-0.2.0/src/csle_common/models/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/models/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4091 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/models/fnn_w_softmax.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.860460 csle_common-0.2.0/src/csle_common/tunneling/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/tunneling/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2325 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/tunneling/forward_ssh_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      280 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/tunneling/forward_ssh_server.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1620 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/tunneling/forward_tunnel_thread.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.864460 csle_common-0.2.0/src/csle_common/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6225 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/cluster_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    35781 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/connection_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8718 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/docker_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    21328 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/emulation_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    37779 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/env_dynamics_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    16211 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/experiment_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    19188 2023-04-18 12:45:40.000000 csle_common-0.2.0/src/csle_common/util/export_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2000 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/general_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      533 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/grpc_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2514 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/import_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3542 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/management_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2165 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/plotting_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    22141 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/read_emulation_statistics_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2512 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/ssh_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.808460 csle_common-0.2.0/src/csle_common.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      685 2023-04-30 12:36:20.000000 csle_common-0.2.0/src/csle_common.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)    14903 2023-04-30 12:36:20.000000 csle_common-0.2.0/src/csle_common.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:36:20.000000 csle_common-0.2.0/src/csle_common.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:28:51.000000 csle_common-0.2.0/src/csle_common.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      406 2023-04-30 12:36:20.000000 csle_common-0.2.0/src/csle_common.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       12 2023-04-30 12:36:20.000000 csle_common-0.2.0/src/csle_common.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.357721 csle_common-0.2.1/
+-rw-r--r--   0 kimham     (501) staff       (20)      685 2023-05-31 11:23:35.357909 csle_common-0.2.1/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)      671 2023-02-12 08:59:32.000000 csle_common-0.2.1/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1483 2023-05-31 11:23:35.358870 csle_common-0.2.1/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_common-0.2.1/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.045909 csle_common-0.2.1/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.051240 csle_common-0.2.1/src/csle_common/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:22:38.000000 csle_common-0.2.1/src/csle_common/__version__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.053599 csle_common-0.2.1/src/csle_common/constants/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/constants/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    67243 2023-04-25 08:36:45.000000 csle_common-0.2.1/src/csle_common/constants/constants.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.060867 csle_common-0.2.1/src/csle_common/consumer_threads/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/consumer_threads/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4795 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/consumer_threads/aggregated_host_metrics_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3154 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/consumer_threads/aggregated_ossec_ids_log_consumer_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3207 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/consumer_threads/aggregated_snort_ids_log_consumer_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3202 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/consumer_threads/aggregated_snort_ids_rule_log_consumer_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2417 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/consumer_threads/attacker_actions_consumer_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2807 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/consumer_threads/avg_host_metrics_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3905 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/consumer_threads/client_population_consumer_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2494 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/consumer_threads/defender_actions_consumer_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2444 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4779 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/consumer_threads/docker_stats_consumer_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2390 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/consumer_threads/host_metrics_consumer_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2564 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/consumer_threads/ossec_ids_log_consumer_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2493 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/consumer_threads/snort_ids_log_consumer_thread.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.076756 csle_common-0.2.1/src/csle_common/controllers/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/controllers/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    37512 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/controllers/container_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)    17707 2023-03-20 17:20:29.000000 csle_common-0.2.1/src/csle_common/controllers/elk_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)    48222 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/controllers/emulation_env_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2255 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/controllers/flags_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)    71893 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/controllers/host_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)    11832 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/controllers/installation_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)    14738 2023-03-05 07:26:30.000000 csle_common-0.2.1/src/csle_common/controllers/kafka_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)    23199 2023-05-01 08:01:52.000000 csle_common-0.2.1/src/csle_common/controllers/management_system_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)    20424 2023-03-05 07:26:30.000000 csle_common-0.2.1/src/csle_common/controllers/ossec_ids_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5548 2023-03-20 19:52:56.000000 csle_common-0.2.1/src/csle_common/controllers/ovs_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3974 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/controllers/resource_constraints_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)    15201 2023-04-19 06:25:48.000000 csle_common-0.2.1/src/csle_common/controllers/sdn_controller_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1214 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/controllers/simulation_env_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)    21969 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/controllers/snort_ids_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)    11243 2023-03-22 11:50:26.000000 csle_common-0.2.1/src/csle_common/controllers/topology_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)    33524 2023-05-31 11:20:59.000000 csle_common-0.2.1/src/csle_common/controllers/traffic_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3839 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/controllers/users_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2884 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/controllers/vulnerabilities_controller.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.078544 csle_common-0.2.1/src/csle_common/dao/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/__init__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.103102 csle_common-0.2.1/src/csle_common/dao/datasets/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/datasets/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5914 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/datasets/statistics_dataset.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5674 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/datasets/traces_dataset.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.104858 csle_common-0.2.1/src/csle_common/dao/docker/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/docker/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6387 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/docker/docker_container_metadata.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3595 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/docker/docker_env_metadata.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.105359 csle_common-0.2.1/src/csle_common/dao/emulation_action/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/__init__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.111304 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    11189 2023-03-16 08:30:07.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py
+-rw-r--r--   0 kimham     (501) staff       (20)    19992 2023-03-22 11:50:26.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2172 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py
+-rw-r--r--   0 kimham     (501) staff       (20)      362 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_outcome.py
+-rw-r--r--   0 kimham     (501) staff       (20)      295 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1728 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_masscan_actions.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1517 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_network_service_actions.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1551 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nikto_actions.py
+-rw-r--r--   0 kimham     (501) staff       (20)    29225 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nmap_actions.py
+-rw-r--r--   0 kimham     (501) staff       (20)    12817 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_shell_actions.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2091 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_stopping_actions.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.114363 csle_common-0.2.1/src/csle_common/dao/emulation_action/defender/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/defender/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6875 2023-03-16 08:29:37.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/defender/emulation_defender_action.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4063 2023-03-22 11:50:26.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/defender/emulation_defender_action_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)      221 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/defender/emulation_defender_action_id.py
+-rw-r--r--   0 kimham     (501) staff       (20)      286 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/defender/emulation_defender_action_outcome.py
+-rw-r--r--   0 kimham     (501) staff       (20)      247 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/defender/emulation_defender_action_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4705 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action/defender/emulation_defender_stopping_actions.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.126843 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)      953 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nikto_scan_result.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1997 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nikto_vuln.py
+-rw-r--r--   0 kimham     (501) staff       (20)      192 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_addr_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1938 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_brute_credentials.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2523 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_hop.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3104 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_host_result.py
+-rw-r--r--   0 kimham     (501) staff       (20)      199 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_host_status.py
+-rw-r--r--   0 kimham     (501) staff       (20)      395 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_http_enum.py
+-rw-r--r--   0 kimham     (501) staff       (20)      411 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_http_grep.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1174 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_os.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3715 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_port.py
+-rw-r--r--   0 kimham     (501) staff       (20)      199 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_port_status.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1007 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_scan_result.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2326 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_trace.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2546 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_vuln.py
+-rw-r--r--   0 kimham     (501) staff       (20)      400 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_vulscan.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.177181 csle_common-0.2.1/src/csle_common/dao/emulation_config/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4068 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/beats_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3182 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/client_managers_info.py
+-rw-r--r--   0 kimham     (501) staff       (20)     8240 2023-05-31 08:19:28.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/client_population_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2576 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/cluster_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2926 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/cluster_node.py
+-rw-r--r--   0 kimham     (501) staff       (20)    37157 2023-03-05 07:34:13.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4143 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/connection_setup_dto.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4084 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/container_network.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7691 2023-03-05 07:26:30.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/containers_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4325 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/credential.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4829 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/default_network_firewall_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5296 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/docker_stats_manager_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3418 2023-02-12 12:41:34.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/docker_stats_managers_info.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7236 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/elk_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3728 2023-03-22 11:50:26.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/elk_managers_info.py
+-rw-r--r--   0 kimham     (501) staff       (20)    21925 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_env_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7640 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_env_generation_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7486 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_env_state.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2392 2023-02-17 16:35:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_execution.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7851 2022-12-07 09:01:16.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_execution_info.py
+-rw-r--r--   0 kimham     (501) staff       (20)    18879 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_metrics_time_series.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2768 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_simulation_trace.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3406 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_statistics_windowed.py
+-rw-r--r--   0 kimham     (501) staff       (20)    42526 2022-11-29 07:04:09.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_trace.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3693 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/flag.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3446 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/flags_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4658 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/host_manager_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3103 2022-11-29 17:55:52.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/host_managers_info.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7618 2023-03-16 10:11:01.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/kafka_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3108 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/kafka_managers_info.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3550 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/kafka_topic.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5079 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/network_service.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6950 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/node_beats_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7334 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/node_container_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     8495 2023-03-22 11:50:26.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/node_firewall_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3630 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/node_flags_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)    15661 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/node_network_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5446 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/node_resources_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3052 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/node_services_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5232 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/node_traffic_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3633 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/node_users_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5560 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/node_vulnerability_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5008 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/ossec_ids_manager_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3328 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/ossec_managers_info.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3016 2023-03-22 11:50:26.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/ovs_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5399 2023-03-20 19:41:31.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/ovs_switch_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)      316 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/packet_delay_distribution_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)      269 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/packet_loss_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3214 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/resources_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3888 2023-03-20 17:20:29.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/ryu_managers_info.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7312 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/sdn_controller_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)      205 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/sdn_controller_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3562 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/services_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4910 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/snort_ids_manager_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3618 2023-03-16 16:23:09.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/snort_managers_info.py
+-rw-r--r--   0 kimham     (501) staff       (20)      254 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/static_emulation_attacker_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3503 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/topology_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4286 2023-05-31 08:19:28.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/traffic_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3216 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/traffic_managers_info.py
+-rw-r--r--   0 kimham     (501) staff       (20)      782 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/transport_protocol.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2435 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/user.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3431 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/users_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3787 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/vulnerabilities_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)      302 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_config/vulnerability_type.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.178050 csle_common-0.2.1/src/csle_common/dao/emulation_observation/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_observation/__init__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.179577 csle_common-0.2.1/src/csle_common/dao/emulation_observation/attacker/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_observation/attacker/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    20660 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_machine_observation_state.py
+-rw-r--r--   0 kimham     (501) staff       (20)    10470 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_observation_state.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.182620 csle_common-0.2.1/src/csle_common/dao/emulation_observation/common/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_observation/common/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6143 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_observation/common/emulation_connection_observation_state.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6055 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_observation/common/emulation_port_observation_state.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6278 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/emulation_observation/common/emulation_vulnerability_observation_state.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.185081 csle_common-0.2.1/src/csle_common/dao/emulation_observation/defender/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/emulation_observation/defender/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    12682 2023-05-24 17:41:18.000000 csle_common-0.2.1/src/csle_common/dao/emulation_observation/defender/emulation_defender_machine_observation_state.py
+-rw-r--r--   0 kimham     (501) staff       (20)    22453 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/dao/emulation_observation/defender/emulation_defender_observation_state.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.188999 csle_common-0.2.1/src/csle_common/dao/encoding/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/encoding/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)      411 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/encoding/np_encoder.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.192581 csle_common-0.2.1/src/csle_common/dao/jobs/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/jobs/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7391 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/dao/jobs/data_collection_job_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4781 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/dao/jobs/system_identification_job_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5823 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/dao/jobs/training_job_config.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.195113 csle_common-0.2.1/src/csle_common/dao/management/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/management/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3542 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/management/management_user.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2775 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/management/session_token.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.224597 csle_common-0.2.1/src/csle_common/dao/simulation_config/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1073 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/action.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2022 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/action_space_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)      483 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/agent_log.py
+-rw-r--r--   0 kimham     (501) staff       (20)      747 2023-03-22 11:50:26.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/base_env.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1228 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/env_parameter.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1216 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/env_parameters_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1312 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/initial_state_distribution_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1302 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/joint_action_space_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1163 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/joint_observation_space_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1242 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/observation.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1505 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/observation_function_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5039 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/observation_space_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1226 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/player_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1271 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/players_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1047 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/reward_function_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)    11210 2023-03-08 07:57:44.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/simulation_env_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)      337 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/simulation_env_input_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5489 2023-03-01 10:57:15.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/simulation_trace.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1451 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/state.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1274 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/state_space_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)      157 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/state_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)      166 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/time_step_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1121 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/transition_operator_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)      159 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/simulation_config/value_type.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.239709 csle_common-0.2.1/src/csle_common/dao/system_identification/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/system_identification/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2998 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/system_identification/empirical_conditional.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6116 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/system_identification/empirical_system_model.py
+-rw-r--r--   0 kimham     (501) staff       (20)    29651 2023-04-19 06:25:48.000000 csle_common-0.2.1/src/csle_common/dao/system_identification/emulation_statistics.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7292 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/system_identification/gaussian_mixture_conditional.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6623 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/system_identification/gaussian_mixture_system_model.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5215 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/system_identification/gp_conditional.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6461 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/system_identification/gp_system_model.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3260 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/system_identification/system_identification_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)      768 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/system_identification/system_model.py
+-rw-r--r--   0 kimham     (501) staff       (20)      219 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/system_identification/system_model_type.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.282092 csle_common-0.2.1/src/csle_common/dao/training/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/training/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)      653 2023-05-01 11:54:10.000000 csle_common-0.2.1/src/csle_common/dao/training/agent_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6794 2023-04-19 15:40:32.000000 csle_common-0.2.1/src/csle_common/dao/training/alpha_vectors_policy.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7536 2023-04-19 15:40:32.000000 csle_common-0.2.1/src/csle_common/dao/training/dqn_policy.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4362 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/training/experiment_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3648 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/training/experiment_execution.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3222 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/training/experiment_result.py
+-rw-r--r--   0 kimham     (501) staff       (20)    11703 2023-04-19 15:40:32.000000 csle_common-0.2.1/src/csle_common/dao/training/fnn_with_softmax_policy.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1959 2023-03-01 07:00:43.000000 csle_common-0.2.1/src/csle_common/dao/training/hparam.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7082 2023-05-02 14:18:43.000000 csle_common-0.2.1/src/csle_common/dao/training/linear_tabular_policy.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7246 2023-05-02 14:18:43.000000 csle_common-0.2.1/src/csle_common/dao/training/linear_threshold_stopping_policy.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6437 2023-05-02 11:30:45.000000 csle_common-0.2.1/src/csle_common/dao/training/mixed_linear_tabular.py
+-rw-r--r--   0 kimham     (501) staff       (20)    14240 2023-04-19 15:37:18.000000 csle_common-0.2.1/src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6204 2023-05-02 07:31:12.000000 csle_common-0.2.1/src/csle_common/dao/training/mixed_ppo_policy.py
+-rw-r--r--   0 kimham     (501) staff       (20)    14042 2023-04-19 15:40:32.000000 csle_common-0.2.1/src/csle_common/dao/training/multi_threshold_stopping_policy.py
+-rw-r--r--   0 kimham     (501) staff       (20)      179 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/training/player_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)      963 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/dao/training/policy.py
+-rw-r--r--   0 kimham     (501) staff       (20)      400 2023-05-02 11:30:45.000000 csle_common-0.2.1/src/csle_common/dao/training/policy_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7334 2023-05-02 07:31:12.000000 csle_common-0.2.1/src/csle_common/dao/training/ppo_policy.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4763 2023-04-19 15:36:26.000000 csle_common-0.2.1/src/csle_common/dao/training/random_policy.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5540 2023-05-24 17:19:50.000000 csle_common-0.2.1/src/csle_common/dao/training/tabular_policy.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4809 2023-04-25 09:10:49.000000 csle_common-0.2.1/src/csle_common/dao/training/vector_policy.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.286209 csle_common-0.2.1/src/csle_common/logging/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/logging/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)      624 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/logging/custom_formatter.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2646 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/logging/log.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.287549 csle_common-0.2.1/src/csle_common/metastore/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/metastore/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)   228299 2023-05-24 17:19:50.000000 csle_common-0.2.1/src/csle_common/metastore/metastore_facade.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.295470 csle_common-0.2.1/src/csle_common/models/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-12-13 08:21:49.000000 csle_common-0.2.1/src/csle_common/models/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4091 2022-12-13 08:21:49.000000 csle_common-0.2.1/src/csle_common/models/fnn_w_softmax.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.304374 csle_common-0.2.1/src/csle_common/tunneling/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/tunneling/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2325 2022-12-07 07:23:42.000000 csle_common-0.2.1/src/csle_common/tunneling/forward_ssh_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)      280 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/tunneling/forward_ssh_server.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1620 2022-12-07 07:23:42.000000 csle_common-0.2.1/src/csle_common/tunneling/forward_tunnel_thread.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.356990 csle_common-0.2.1/src/csle_common/util/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/util/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6225 2023-02-17 08:04:16.000000 csle_common-0.2.1/src/csle_common/util/cluster_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)    35781 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/util/connection_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     8718 2023-03-20 10:38:35.000000 csle_common-0.2.1/src/csle_common/util/docker_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)    21328 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/util/emulation_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)    37779 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/util/env_dynamics_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)    16211 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/util/experiment_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)    19188 2023-04-19 06:25:48.000000 csle_common-0.2.1/src/csle_common/util/export_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2000 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/util/general_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)      533 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/util/grpc_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2514 2022-12-28 18:49:38.000000 csle_common-0.2.1/src/csle_common/util/import_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3542 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/util/management_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2165 2023-03-16 16:22:51.000000 csle_common-0.2.1/src/csle_common/util/plotting_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)    22141 2023-03-31 11:14:06.000000 csle_common-0.2.1/src/csle_common/util/read_emulation_statistics_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2512 2022-11-28 13:00:49.000000 csle_common-0.2.1/src/csle_common/util/ssh_util.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:23:35.053180 csle_common-0.2.1/src/csle_common.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      685 2023-05-31 11:23:34.000000 csle_common-0.2.1/src/csle_common.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)    14733 2023-05-31 11:23:35.000000 csle_common-0.2.1/src/csle_common.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:23:34.000000 csle_common-0.2.1/src/csle_common.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:23.000000 csle_common-0.2.1/src/csle_common.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      406 2023-05-31 11:23:34.000000 csle_common-0.2.1/src/csle_common.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       12 2023-05-31 11:23:34.000000 csle_common-0.2.1/src/csle_common.egg-info/top_level.txt
```

### Comparing `csle_common-0.2.0/PKG-INFO` & `csle_common-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_common
-Version: 0.2.0
+Version: 0.2.1
 Summary: Common functionality of the Cyber Security Learning Environment (CSLE)
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_common-0.2.0/pyproject.toml` & `csle_common-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/setup.cfg` & `csle_common-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 	random_username>=1.0.2
 	psycopg==3.1.4
 	click>=8.1.3
 	flask>=2.2.2
 	waitress>=2.1.2
 	psutil>=5.9.4
 	csle_collector>=0.1.5
-	csle-ryu>=0.2.0
+	csle-ryu>=0.2.1
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_common-0.2.0/src/csle_common/constants/constants.py` & `csle_common-0.2.1/src/csle_common/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_host_metrics_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/aggregated_host_metrics_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_ossec_ids_log_consumer_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/aggregated_ossec_ids_log_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_snort_ids_log_consumer_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/aggregated_snort_ids_log_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_snort_ids_rule_log_consumer_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/aggregated_snort_ids_rule_log_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/attacker_actions_consumer_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/attacker_actions_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/avg_host_metrics_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/avg_host_metrics_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/client_population_consumer_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/client_population_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/defender_actions_consumer_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/defender_actions_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/docker_stats_consumer_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/docker_stats_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/host_metrics_consumer_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/host_metrics_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/ossec_ids_log_consumer_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/ossec_ids_log_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/consumer_threads/snort_ids_log_consumer_thread.py` & `csle_common-0.2.1/src/csle_common/consumer_threads/snort_ids_log_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/container_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/container_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/elk_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/elk_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/emulation_env_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/emulation_env_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/flags_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/flags_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/host_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/host_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/installation_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/installation_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/kafka_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/kafka_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/management_system_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/management_system_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from typing import Any
 import subprocess
 import docker
+import psutil
 import os
 import csle_common.constants.constants as constants
 import sys
 import shutil
 
 
 class ManagementSystemController:
@@ -559,35 +560,33 @@
         pid = ManagementSystemController.read_pid_file(constants.COMMANDS.CLUSTER_MANAGER_PIDFILE)
         cmd = constants.COMMANDS.KILL_PROCESS.format(pid)
         p = subprocess.Popen(cmd, stdout=subprocess.DEVNULL, shell=True)
         (output, err) = p.communicate()
         return True
 
     @staticmethod
-    def is_pid_running(pid: int) -> bool:
+    def is_pid_running(pid: int, logger: logging.Logger) -> bool:
         """
         Checks if the given pid is running on the host
 
         :param pid: the pid to check
+        :param logger: the logger to use for logging
         :return: True if it is running, false otherwise
         """
-        cmd = (constants.COMMANDS.PS_AUX + constants.COMMANDS.SPACE_DELIM + constants.COMMANDS.PIPE_DELIM +
-               constants.COMMANDS.SPACE_DELIM + constants.COMMANDS.GREP + constants.COMMANDS.SPACE_DELIM + str(pid))
-        p = subprocess.Popen(cmd, stdout=subprocess.PIPE, shell=True)
-        (output, err) = p.communicate()
-        output = str(output)
-        return str(pid) in output
+        logger.info(f"Checking if PID: {pid} is running")
+        return psutil.pid_exists(pid)
 
     @staticmethod
-    def stop_pid(pid) -> bool:
+    def stop_pid(pid, logger: logging.Logger) -> bool:
         """
         Stops a process with a given pid
 
         :param pid: the pid to stop
         :return: True if the pid was stopped, false if it was not running
         """
-        if not ManagementSystemController.is_pid_running(pid):
+        if not ManagementSystemController.is_pid_running(pid, logger=logger):
             return False
         cmd = constants.COMMANDS.KILL_PROCESS.format(pid)
+        logger.info(f"Stopping PID:{pid} with command: {cmd}")
         p = subprocess.Popen(cmd, stdout=subprocess.DEVNULL, shell=True)
         p.communicate()
         return True
```

### Comparing `csle_common-0.2.0/src/csle_common/controllers/ossec_ids_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/ossec_ids_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/ovs_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/ovs_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/resource_constraints_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/resource_constraints_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/sdn_controller_manager.py` & `csle_common-0.2.1/src/csle_common/controllers/sdn_controller_manager.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/simulation_env_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/simulation_env_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/snort_ids_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/snort_ids_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/topology_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/topology_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/traffic_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/traffic_controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import csle_common.constants.constants as constants
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.emulation_config.client_managers_info import ClientManagersInfo
 from csle_common.dao.emulation_config.node_traffic_config import NodeTrafficConfig
 from csle_common.dao.emulation_config.traffic_managers_info import TrafficManagersInfo
 from csle_common.dao.emulation_config.node_container_config import NodeContainerConfig
 from csle_common.util.emulation_util import EmulationUtil
-from csle_common.dao.emulation_config.client_population_process_type import ClientPopulationProcessType
+from csle_collector.client_manager.dao.client_arrival_type import ClientArrivalType
 
 
 class TrafficController:
     """
     Class managing traffic generators in the emulation environments
     """
 
@@ -297,40 +297,16 @@
         :param emulation_env_config: the emulation environment configuration
         :param physical_server_ip: the ip of the physical server
         :param logger: the logger to use for logging
         :return: None
         """
         if emulation_env_config.traffic_config.client_population_config.physical_host_ip != physical_server_ip:
             return
-        logger.info(
-            f"Starting client population on container: "
-            f"{emulation_env_config.traffic_config.client_population_config.docker_gw_bridge_ip}")
-        commands = []
-        reachable_containers = []
-
-        # Collect commands and reachable containers
-        for container in emulation_env_config.containers_config.containers:
-            match = False
-            for ip, net in container.ips_and_networks:
-                for net2 in emulation_env_config.traffic_config.client_population_config.networks:
-                    if net.name == net2.name:
-                        match = True
-                        break
-            if match:
-                for ip2 in container.get_ips():
-                    reachable_containers.append(ip2)
-
-        for node_traffic_cfg in emulation_env_config.traffic_config.node_traffic_configs:
-            if node_traffic_cfg.ip in reachable_containers:
-                for cmd in node_traffic_cfg.commands:
-                    commands.append(cmd.format(node_traffic_cfg.ip))
-
-        for net in emulation_env_config.traffic_config.client_population_config.networks:
-            for cmd in constants.TRAFFIC_COMMANDS.DEFAULT_COMMANDS[constants.TRAFFIC_COMMANDS.CLIENT_1_SUBNET]:
-                commands.append(cmd.format(net.subnet_mask))
+        logger.info(f"Starting client population on container: "
+                    f"{emulation_env_config.traffic_config.client_population_config.docker_gw_bridge_ip}")
 
         TrafficController.start_client_manager(emulation_env_config=emulation_env_config, logger=logger)
 
         client_dto = TrafficController.get_clients_dto_by_ip_and_port(
             ip=emulation_env_config.traffic_config.client_population_config.docker_gw_bridge_ip,
             port=emulation_env_config.traffic_config.client_population_config.client_manager_port
         )
@@ -343,61 +319,28 @@
 
             # Stop the client population if it is already running
             if client_dto.client_process_active:
                 csle_collector.client_manager.query_clients.stop_clients(stub)
                 time.sleep(2)
 
             # Start the client population
-            sine_modulated = False
-            if (emulation_env_config.traffic_config.client_population_config.client_process_type ==
-                    ClientPopulationProcessType.SINE_MODULATED_POISSON):
-                sine_modulated = True
-            spiking = False
-            if (emulation_env_config.traffic_config.client_population_config.client_process_type ==
-                    ClientPopulationProcessType.SPIKING):
-                spiking = True
-            piece_wise_constant = False
-            if (emulation_env_config.traffic_config.client_population_config.client_process_type ==
-                    ClientPopulationProcessType.PIECE_WISE_CONSTANT):
-                piece_wise_constant = True
             time_step_len = emulation_env_config.traffic_config.client_population_config.client_time_step_len_seconds
+            num_workflows = len(
+                emulation_env_config.traffic_config.client_population_config.workflows_config.workflow_markov_chains)
+            num_services = len(
+                emulation_env_config.traffic_config.client_population_config.workflows_config.workflow_services)
             logger.info(
-                f"Starting the client population, "
-                f"mu: {emulation_env_config.traffic_config.client_population_config.mu},\n"
-                f"lamb: {emulation_env_config.traffic_config.client_population_config.lamb},\n"
+                f"Starting the client population, "                
                 f"time_step_len_seconds: {time_step_len},\n"
-                f"commands: {commands},\n"
-                f"num_commands: {emulation_env_config.traffic_config.client_population_config.num_commands},\n"
-                f"sine_modulated: {sine_modulated},\n"
-                f"time_scaling_factor:"
-                f"{emulation_env_config.traffic_config.client_population_config.time_scaling_factor},\n"
-                f"period_scaling_factor: "
-                f"{emulation_env_config.traffic_config.client_population_config.period_scaling_factor},\n"
-                f"spiking: {spiking},\n piece_wise_constant: {piece_wise_constant},\n "
-                f"exponents: {emulation_env_config.traffic_config.client_population_config.exponents},\n "
-                f"factors: {emulation_env_config.traffic_config.client_population_config.factors},\n "
-                f"breakvalues: {emulation_env_config.traffic_config.client_population_config.breakvalues}, \n"
-                f"breakpoints: {emulation_env_config.traffic_config.client_population_config.breakpoints}"
-            )
+                f"num client profiles: {len(emulation_env_config.traffic_config.client_population_config.clients)}, \n"
+                f"num workflows: {num_workflows}, num_services: {num_services}")
             csle_collector.client_manager.query_clients.start_clients(
-                stub=stub, mu=emulation_env_config.traffic_config.client_population_config.mu,
-                lamb=emulation_env_config.traffic_config.client_population_config.lamb,
-                time_step_len_seconds=time_step_len,
-                commands=commands,
-                num_commands=emulation_env_config.traffic_config.client_population_config.num_commands,
-                sine_modulated=sine_modulated,
-                time_scaling_factor=emulation_env_config.traffic_config.client_population_config.time_scaling_factor,
-                period_scaling_factor=(
-                    emulation_env_config.traffic_config.client_population_config.period_scaling_factor),
-                spiking=spiking, piece_wise_constant=piece_wise_constant,
-                exponents=emulation_env_config.traffic_config.client_population_config.exponents,
-                factors=emulation_env_config.traffic_config.client_population_config.factors,
-                breakvalues=emulation_env_config.traffic_config.client_population_config.breakvalues,
-                breakpoints=emulation_env_config.traffic_config.client_population_config.breakpoints
-            )
+                stub=stub, time_step_len_seconds=time_step_len,
+                workflows_config=emulation_env_config.traffic_config.client_population_config.workflows_config,
+                clients=emulation_env_config.traffic_config.client_population_config.clients)
 
     @staticmethod
     def get_num_active_clients(emulation_env_config: EmulationEnvConfig, logger: logging.Logger) \
             -> csle_collector.client_manager.client_manager_pb2.ClientsDTO:
         """
         Gets the number of active clients
```

### Comparing `csle_common-0.2.0/src/csle_common/controllers/users_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/users_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/controllers/vulnerabilities_controller.py` & `csle_common-0.2.1/src/csle_common/controllers/vulnerabilities_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/datasets/statistics_dataset.py` & `csle_common-0.2.1/src/csle_common/dao/datasets/statistics_dataset.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/datasets/traces_dataset.py` & `csle_common-0.2.1/src/csle_common/dao/datasets/traces_dataset.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/docker/docker_container_metadata.py` & `csle_common-0.2.1/src/csle_common/dao/docker/docker_container_metadata.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/docker/docker_env_metadata.py` & `csle_common-0.2.1/src/csle_common/dao/docker/docker_env_metadata.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_masscan_actions.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_masscan_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_network_service_actions.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_network_service_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nikto_actions.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nikto_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nmap_actions.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nmap_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_shell_actions.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_shell_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_stopping_actions.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action/attacker/emulation_attacker_stopping_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action/defender/emulation_defender_action.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action/defender/emulation_defender_action_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_stopping_actions.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action/defender/emulation_defender_stopping_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nikto_scan_result.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nikto_scan_result.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nikto_vuln.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nikto_vuln.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_brute_credentials.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_brute_credentials.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_hop.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_hop.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_host_result.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_host_result.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_os.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_os.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_port.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_port.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_scan_result.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_scan_result.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_trace.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_trace.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_vuln.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_action_result/nmap_vuln.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/beats_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/beats_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/client_managers_info.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/client_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/client_population_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/client_population_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,147 +1,125 @@
 from typing import List, Dict, Any
-from csle_common.dao.emulation_config.client_population_process_type import ClientPopulationProcessType
+from csle_collector.client_manager.dao.constant_arrival_config import ConstantArrivalConfig
+from csle_collector.client_manager.dao.workflows_config import WorkflowsConfig
+from csle_collector.client_manager.dao.workflow_markov_chain import WorkflowMarkovChain
+from csle_collector.client_manager.dao.workflow_service import WorkflowService
+from csle_collector.client_manager.dao.client import Client
 from csle_common.dao.emulation_config.container_network import ContainerNetwork
 from csle_common.util.general_util import GeneralUtil
 
 
 class ClientPopulationConfig:
     """
     A DTO object representing the configuration of the client population of an emulation
     """
 
-    def __init__(self, ip: str, networks: List[ContainerNetwork], client_process_type: ClientPopulationProcessType,
-                 lamb: float, mu: float, client_manager_port: int, client_manager_log_file: str,
+    def __init__(self, ip: str, networks: List[ContainerNetwork],
+                 client_manager_port: int, client_manager_log_file: str,
                  client_manager_log_dir: str, client_manager_max_workers: int,
-                 num_commands: int = 5,
-                 client_time_step_len_seconds: int = 1, time_scaling_factor: float = 0.01,
-                 period_scaling_factor: float = 20, docker_gw_bridge_ip: str = "", physical_host_ip: str = "",
-                 exponents=None, factors=None, breakpoints=None, breakvalues=None):
+                 clients: List[Client], workflows_config: WorkflowsConfig,
+                 client_time_step_len_seconds: int = 1,
+                 docker_gw_bridge_ip: str = "", physical_host_ip: str = ""):
         """
         Creates a ClientPopulationConfig DTO Object
 
         :param ip: the ip of the client container
         :param networks: a list of networks in the emulation that are accessible for external networks
-        :param client_process_type: the type of client arrival process (e.g. a Poisson process)
-        :param lamb: the lambda parameter of the arrival process
-        :param mu: the service-time parameter of the arrivals
         :param client_time_step_len_seconds: time-step length to measure the arrival process
-        :param time_scaling_factor: the time-scaling factor for sine-modulated arrival processes
-        :param period_scaling_factor: the period-scaling factor for sine-modulated arrival processes
         :param client_manager_log_file: the log file of the client manager
         :param client_manager_log_dir: the log dir of the client manager
         :param client_manager_max_workers: the maximum number of GRPC workers for the client manager
         :param docker_gw_bridge_ip: IP to reach the container from the host network
         :param physical_host_ip: IP of the physical host where the container is running
-        :param exponents: exponents for spike-moduldated arrival process
-        :param factors: factors for spike-moduldated arrival process
-        :param breakpoints: breakpoints for piece-wise constant arrival process
-        :param breakvalues: breakvalues for piece-wise constant arrival process
+        :param clients: list of client configurations
+        :param workflows_config: the workflows configurations
         """
         self.networks = networks
         self.ip = ip
-        self.client_process_type = client_process_type
-        self.lamb = lamb
-        self.mu = mu
         self.client_manager_port = client_manager_port
-        self.num_commands = num_commands
         self.client_time_step_len_seconds = client_time_step_len_seconds
-        self.time_scaling_factor = time_scaling_factor
-        self.period_scaling_factor = period_scaling_factor
         self.client_manager_log_dir = client_manager_log_dir
         self.client_manager_log_file = client_manager_log_file
         self.client_manager_max_workers = client_manager_max_workers
         self.docker_gw_bridge_ip = docker_gw_bridge_ip
         self.physical_host_ip = physical_host_ip
-        self.exponents = exponents
-        self.factors = factors
-        self.breakpoints = breakpoints
-        self.breakvalues = breakvalues
+        self.clients = clients
+        self.workflows_config = workflows_config
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "ClientPopulationConfig":
         """
         Converts a dict representation to an instance
 
         :param d: the dict to convert
         :return: the created instance
         """
         obj = ClientPopulationConfig(
             ip=d["ip"],
             networks=list(map(lambda x: ContainerNetwork.from_dict(x), d["networks"])),
-            client_process_type=d["client_process_type"],
-            lamb=d["lamb"], mu=d["mu"], client_manager_port=d["client_manager_port"],
-            num_commands=d["num_commands"], client_time_step_len_seconds=d["client_time_step_len_seconds"],
-            period_scaling_factor=d["period_scaling_factor"], time_scaling_factor=d["time_scaling_factor"],
+            client_manager_port=d["client_manager_port"],
+            client_time_step_len_seconds=d["client_time_step_len_seconds"],
             client_manager_log_dir=d["client_manager_log_dir"], client_manager_log_file=d["client_manager_log_file"],
             client_manager_max_workers=d["client_manager_max_workers"],
             docker_gw_bridge_ip=d["docker_gw_bridge_ip"], physical_host_ip=d["physical_host_ip"],
-            exponents=d["exponents"], factors=d["factors"], breakpoints=d["breakpoints"],
-            breakvalues=d["breakvalues"]
+            clients=list(map(lambda x: Client.from_dict(x), d["clients"])),
+            workflows_config=WorkflowsConfig.from_dict(d["workflows_config"])
         )
         return obj
 
     def no_clients(self) -> "ClientPopulationConfig":
         """
         :return: A version of the config with no clients
         """
         return ClientPopulationConfig(
             ip=self.ip,
             networks=self.networks,
-            client_process_type=self.client_process_type,
-            lamb=0, mu=0, client_manager_port=self.client_manager_port,
-            num_commands=0, client_time_step_len_seconds=self.client_time_step_len_seconds,
-            period_scaling_factor=self.period_scaling_factor, time_scaling_factor=self.time_scaling_factor,
+            client_manager_port=self.client_manager_port,
+            client_time_step_len_seconds=self.client_time_step_len_seconds,
             client_manager_log_file="client_manager.log", client_manager_log_dir="/", client_manager_max_workers=10,
             docker_gw_bridge_ip=self.docker_gw_bridge_ip, physical_host_ip=self.physical_host_ip,
-            breakpoints=self.breakpoints, breakvalues=self.breakvalues, exponents=self.exponents, factors=self.factors
+            clients=[Client(id=0, arrival_config=ConstantArrivalConfig(lamb=0), mu=0, exponential_service_time=True,
+                            workflow_distribution=[1])],
+            workflows_config=WorkflowsConfig(
+                workflow_markov_chains=[WorkflowMarkovChain(
+                    initial_state=0, transition_matrix=[[0.8,0.2], [0,1]], id=0)],
+                workflow_services=[WorkflowService(ips_and_commands=[('localhost', "echo ' '")], id=0)])
         )
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
         d["ip"] = self.ip
-        d["client_process_type"] = self.client_process_type
-        d["lamb"] = self.lamb
-        d["mu"] = self.mu
         d["networks"] = list(map(lambda x: x.to_dict(), self.networks))
-        d["num_commands"] = self.num_commands
         d["client_manager_port"] = self.client_manager_port
         d["client_time_step_len_seconds"] = self.client_time_step_len_seconds
-        d["time_scaling_factor"] = self.time_scaling_factor
-        d["period_scaling_factor"] = self.period_scaling_factor
         d["client_manager_log_file"] = self.client_manager_log_file
         d["client_manager_log_dir"] = self.client_manager_log_dir
         d["client_manager_max_workers"] = self.client_manager_max_workers
         d["docker_gw_bridge_ip"] = self.docker_gw_bridge_ip
         d["physical_host_ip"] = self.physical_host_ip
-        d["exponents"] = self.exponents
-        d["factors"] = self.factors
-        d["breakpoints"] = self.breakpoints
-        d["breakvalues"] = self.breakvalues
+        d["clients"] = list(map(lambda x: x.to_dict(), self.clients))
+        d["workflows_config"] = self.workflows_config.to_dict()
         return d
 
     def __str__(self) -> str:
         """
         :return: a string representation of the object
         """
-        return f"ip:{self.ip}, client_population_process_type: {self.client_process_type}, lamb:{self.lamb}, " \
-               f"mu:{self.mu}, self.networks:{list(map(lambda x: str(x), self.networks))}, " \
-               f"client_manager_port: {self.client_manager_port}, num_commands:{self.num_commands}, " \
+        return f"ip:{self.ip}, " \
+               f"networks:{list(map(lambda x: str(x), self.networks))}, " \
+               f"client_manager_port: {self.client_manager_port}, " \
                f"client_time_step_len_seconds: {self.client_time_step_len_seconds}," \
-               f"time_scaling_factor: {self.time_scaling_factor}, " \
-               f"period_scaling_factor: {self.period_scaling_factor}," \
                f"client_manager_log_file: {self.client_manager_log_file}, " \
                f"client_manager_log_dir: {self.client_manager_log_dir}, " \
                f"client_manager_max_workers: {self.client_manager_max_workers}, " \
-               f"docker_gw_bridge_ip:{self.docker_gw_bridge_ip}, physical_host_ip: {self.physical_host_ip}, " \
-               f"exponents: {self.exponents}, factors: {self.factors}, breakpoints: {self.breakpoints}, " \
-               f"breakvalues: {self.breakvalues}"
+               f"docker_gw_bridge_ip:{self.docker_gw_bridge_ip}, physical_host_ip: {self.physical_host_ip}," \
+               f"clients:{list(map(lambda x: str(x), self.clients))}, workflows_config: {self.workflows_config}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
@@ -188,8 +166,9 @@
         :param ip_first_octet: the first octet of the IP of the new execution
         :return: the new config
         """
         config = self.copy()
         config.ip = GeneralUtil.replace_first_octet_of_ip(ip=config.ip, ip_first_octet=ip_first_octet)
         config.networks = list(map(lambda x: x.create_execution_config(ip_first_octet=ip_first_octet),
                                    config.networks))
+        config.workflows_config = config.workflows_config.create_execution_config(ip_first_octet=ip_first_octet)
         return config
```

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/cluster_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/cluster_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/cluster_node.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/cluster_node.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/connection_setup_dto.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/connection_setup_dto.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/container_network.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/container_network.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/containers_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/containers_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/credential.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/credential.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/default_network_firewall_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/default_network_firewall_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/docker_stats_manager_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/docker_stats_manager_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/docker_stats_managers_info.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/docker_stats_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/elk_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/elk_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/elk_managers_info.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/elk_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_env_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_env_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_env_generation_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_env_generation_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_env_state.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_env_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_execution.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_execution.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_execution_info.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_execution_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_metrics_time_series.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_metrics_time_series.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_simulation_trace.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_simulation_trace.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_statistics_windowed.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_statistics_windowed.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_trace.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/emulation_trace.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/flag.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/flag.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/flags_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/flags_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/host_manager_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/host_manager_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/host_managers_info.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/host_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/kafka_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/kafka_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/kafka_managers_info.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/kafka_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/kafka_topic.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/network_service.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/network_service.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_beats_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/node_beats_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_container_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/node_container_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_firewall_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/node_firewall_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_flags_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/node_flags_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_network_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/node_network_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_resources_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/node_resources_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_services_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/node_services_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_traffic_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/node_traffic_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_users_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/node_users_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_vulnerability_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/node_vulnerability_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/ossec_ids_manager_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/ossec_ids_manager_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/ossec_managers_info.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/ossec_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/ovs_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/ovs_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/ovs_switch_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/ovs_switch_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/resources_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/resources_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/ryu_managers_info.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/ryu_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/sdn_controller_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/sdn_controller_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/services_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/services_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/snort_ids_manager_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/snort_ids_manager_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/snort_managers_info.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/snort_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/topology_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/topology_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/traffic_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/traffic_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class TrafficConfig:
     """
     A DTO object representing the traffic configuration of an emulation environment
     """
     def __init__(self, node_traffic_configs: List[NodeTrafficConfig],
-                 client_population_config: ClientPopulationConfig):
+                 client_population_config: ClientPopulationConfig) -> None:
         """
         Initializes the DTO
 
         :param node_traffic_configs: the list of node traffic configurations
         :param client_population_config: the configuration of the client population
         """
         self.node_traffic_configs = node_traffic_configs
@@ -36,16 +36,15 @@
         Converts a dict representation of the object into a an instance
 
         :param d: the dict to convert
         :return: the created instance
         """
         obj = TrafficConfig(
             node_traffic_configs=list(map(lambda x: NodeTrafficConfig.from_dict(x), d["node_traffic_configs"])),
-            client_population_config=ClientPopulationConfig.from_dict(d["client_population_config"])
-        )
+            client_population_config=ClientPopulationConfig.from_dict(d["client_population_config"]))
         return obj
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
```

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/traffic_managers_info.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/traffic_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/transport_protocol.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/transport_protocol.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/user.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/user.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/users_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/users_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_config/vulnerabilities_config.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_config/vulnerabilities_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_machine_observation_state.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_machine_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_observation_state.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/emulation_connection_observation_state.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_observation/common/emulation_connection_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/emulation_port_observation_state.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_observation/common/emulation_port_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/emulation_vulnerability_observation_state.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_observation/common/emulation_vulnerability_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_observation/defender/emulation_defender_machine_observation_state.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_observation/defender/emulation_defender_machine_observation_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,21 +101,27 @@
         :param d: the dict representation
         :return: the object instance
         """
         if "kafka_config" in d and d["kafka_config"] is not None:
             kafka_config = KafkaConfig.from_dict(d["kafka_config"])
         else:
             kafka_config = None
+        if "snort_ids_ip_alert_counters" in d and d["snort_ids_ip_alert_counters"] is not None:
+            ip_alert_counters = SnortIdsIPAlertCounters.from_dict(d["snort_ids_ip_alert_counters"])
+        else:
+            ip_alert_counters = SnortIdsIPAlertCounters()
+        if "ossec_ids_alert_counters" in d and d["ossec_ids_alert_counters"] is not None:
+            ossec_alert_counters = OSSECIdsAlertCounters.from_dict(d["ossec_ids_alert_counters"])
+        else:
+            ossec_alert_counters = OSSECIdsAlertCounters()
         obj = EmulationDefenderMachineObservationState(
             ips=d["ips"], kafka_config=kafka_config,
             host_metrics=HostMetrics.from_dict(d["host_metrics"]),
             docker_stats=DockerStats.from_dict(d["docker_stats"]),
-            snort_ids_ip_alert_counters=SnortIdsIPAlertCounters.from_dict(d["snort_ids_ip_alert_counters"]),
-            ossec_ids_alert_counters=OSSECIdsAlertCounters.from_dict(d["ossec_ids_alert_counters"])
-        )
+            snort_ids_ip_alert_counters=ip_alert_counters, ossec_ids_alert_counters=ossec_alert_counters)
         obj.os = d["os"]
         obj.ports = list(map(lambda x: EmulationPortObservationState.from_dict(x), d["ports"]))
         obj.ssh_connections = list(map(lambda x: EmulationConnectionObservationState.from_dict(x),
                                        d["ssh_connections"]))
         return obj
 
     def to_dict(self) -> Dict[str, Any]:
```

### Comparing `csle_common-0.2.0/src/csle_common/dao/emulation_observation/defender/emulation_defender_observation_state.py` & `csle_common-0.2.1/src/csle_common/dao/emulation_observation/defender/emulation_defender_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/jobs/data_collection_job_config.py` & `csle_common-0.2.1/src/csle_common/dao/jobs/data_collection_job_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/jobs/system_identification_job_config.py` & `csle_common-0.2.1/src/csle_common/dao/jobs/system_identification_job_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/jobs/training_job_config.py` & `csle_common-0.2.1/src/csle_common/dao/jobs/training_job_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/management/management_user.py` & `csle_common-0.2.1/src/csle_common/dao/management/management_user.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/management/session_token.py` & `csle_common-0.2.1/src/csle_common/dao/management/session_token.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/action.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/action.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/action_space_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/action_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/base_env.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/base_env.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/env_parameter.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/env_parameter.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/env_parameters_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/env_parameters_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/initial_state_distribution_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/initial_state_distribution_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/joint_action_space_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/joint_action_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/joint_observation_space_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/joint_observation_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/observation.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/observation.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/observation_function_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/observation_function_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/observation_space_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/observation_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/player_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/player_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/players_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/players_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/reward_function_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/reward_function_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/simulation_env_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/simulation_env_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/simulation_trace.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/simulation_trace.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/state.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/state_space_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/state_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/simulation_config/transition_operator_config.py` & `csle_common-0.2.1/src/csle_common/dao/simulation_config/transition_operator_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/system_identification/empirical_conditional.py` & `csle_common-0.2.1/src/csle_common/dao/system_identification/empirical_conditional.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/system_identification/empirical_system_model.py` & `csle_common-0.2.1/src/csle_common/dao/system_identification/empirical_system_model.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/system_identification/emulation_statistics.py` & `csle_common-0.2.1/src/csle_common/dao/system_identification/emulation_statistics.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/system_identification/gaussian_mixture_conditional.py` & `csle_common-0.2.1/src/csle_common/dao/system_identification/gaussian_mixture_conditional.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/system_identification/gaussian_mixture_system_model.py` & `csle_common-0.2.1/src/csle_common/dao/system_identification/gaussian_mixture_system_model.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/system_identification/gp_conditional.py` & `csle_common-0.2.1/src/csle_common/dao/system_identification/gp_conditional.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/system_identification/gp_system_model.py` & `csle_common-0.2.1/src/csle_common/dao/system_identification/gp_system_model.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/system_identification/system_identification_config.py` & `csle_common-0.2.1/src/csle_common/dao/system_identification/system_identification_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/system_identification/system_model.py` & `csle_common-0.2.1/src/csle_common/dao/system_identification/system_model.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/agent_type.py` & `csle_common-0.2.1/src/csle_common/dao/training/agent_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,7 +25,8 @@
     POLICY_ITERATION = 17
     SHAPLEY_ITERATION = 18
     HSVI_OS_POSG = 19
     FICTITIOUS_PLAY = 20
     LINEAR_PROGRAMMING_NORMAL_FORM = 21
     DYNA_SEC = 22
     BAYESIAN_OPTIMIZATION = 23
+    DFSP_LOCAL = 24
```

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/alpha_vectors_policy.py` & `csle_common-0.2.1/src/csle_common/dao/training/alpha_vectors_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/dqn_policy.py` & `csle_common-0.2.1/src/csle_common/dao/training/dqn_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/experiment_config.py` & `csle_common-0.2.1/src/csle_common/dao/training/experiment_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/experiment_execution.py` & `csle_common-0.2.1/src/csle_common/dao/training/experiment_execution.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/experiment_result.py` & `csle_common-0.2.1/src/csle_common/dao/training/experiment_result.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/fnn_with_softmax_policy.py` & `csle_common-0.2.1/src/csle_common/dao/training/fnn_with_softmax_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/hparam.py` & `csle_common-0.2.1/src/csle_common/dao/training/hparam.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/linear_threshold_stopping_policy.py` & `csle_common-0.2.1/src/csle_common/dao/training/linear_threshold_stopping_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.simulation_name = simulation_name
         self.L = L
         self.states = states
         self.actions = actions
         self.experiment_config = experiment_config
         self.avg_R = avg_R
         self.opponent_strategy = opponent_strategy
-        self.policy_type = PolicyType.MULTI_THRESHOLD
+        self.policy_type = PolicyType.LINEAR_THRESHOLD
 
     def action(self, o: List[float]) -> int:
         """
         Multi-threshold stopping policy
 
         :param o: the current observation
         :return: the selected action
```

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py` & `csle_common-0.2.1/src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/multi_threshold_stopping_policy.py` & `csle_common-0.2.1/src/csle_common/dao/training/multi_threshold_stopping_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/policy.py` & `csle_common-0.2.1/src/csle_common/dao/training/policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/ppo_policy.py` & `csle_common-0.2.1/src/csle_common/dao/training/ppo_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import List, Dict, Union
 import numpy as np
 import torch
 import math
+import iteround
 from stable_baselines3 import PPO
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.dao.simulation_config.state import State
-from csle_common.dao.simulation_config.state_type import StateType
 from csle_common.dao.simulation_config.action import Action
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.policy_type import PolicyType
 from csle_common.logging.log import Logger
 
 
 class PPOPolicy(Policy):
@@ -56,27 +56,25 @@
 
         :param o: the current observation
         :return: the selected action
         """
         a, _ = self.model.predict(np.array(o), deterministic=False)
         return a
 
-    def probability(self, o: List[float], a) -> Union[int, List[int], np.ndarray]:
+    def probability(self, o: List[float], a: int) -> float:
         """
         Multi-threshold stopping policy
 
         :param o: the current observation
-        :return: the selected action
+        :param o: the action
+        :return: the probability of the action
         """
-        actions, values, log_prob = self.model.policy.forward(obs=torch.tensor(o).to(self.model.device))
-        action = actions[0]
-        if action == a:
-            return math.exp(log_prob)
-        else:
-            return 0
+        prob = math.exp(self.model.policy.get_distribution(obs=torch.tensor([o]).to(self.model.device)).log_prob(
+            actions=torch.tensor(a)).item())
+        return prob
 
     def to_dict(self) -> Dict[str, Union[float, int, str]]:
         """
         :return: a dict representation of the policy
         """
         d = {}
         d["id"] = self.id
@@ -115,30 +113,22 @@
     def stage_policy(self, o: Union[List[Union[int, float]], int, float]) -> List[List[float]]:
         """
         Gets the stage policy, i.e a |S|x|A| policy
 
         :param o: the latest observation
         :return: the |S|x|A| stage policy
         """
-        b1 = o[1]
-        l = int(o[0])
-        if not self.player_type == PlayerType.ATTACKER:
-            stage_policy = []
-            for _ in self.states:
-                stage_policy.append(self._get_attacker_dist(obs=o))
-            return stage_policy
-        else:
-            stage_policy = []
-            for s in self.states:
-                if s.state_type != StateType.TERMINAL:
-                    o = [l, b1, s.id]
-                    stage_policy.append(self._get_attacker_dist(obs=o))
-                else:
-                    stage_policy.append([0.5, 0.5])
-            return stage_policy
+        stage_strategy = np.zeros((len(self.states), len(self.actions)))
+        for i, s_a in enumerate(self.states):
+            o[0] = s_a
+            for j, a in enumerate(self.actions):
+                stage_strategy[i][j] = self.probability(o=o, a=j)
+            stage_strategy[i] = iteround.saferound(stage_strategy[i], 2)
+            assert round(sum(stage_strategy[i]), 3) == 1
+        return stage_strategy.tolist()
 
     def _get_attacker_dist(self, obs) -> List[float]:
         """
         Utility function for getting the action distribution conditioned on a given observation
 
         :param obs: the observation to condition on
         :return: the conditional ation distribution
```

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/random_policy.py` & `csle_common-0.2.1/src/csle_common/dao/training/random_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/tabular_policy.py` & `csle_common-0.2.1/src/csle_common/dao/training/tabular_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Union, List, Dict, Any, Optional
+import numpy as np
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.simulation_config.action import Action
 from csle_common.dao.training.policy_type import PolicyType
 
 
@@ -38,15 +39,15 @@
     def action(self, o: Union[List[Union[int, float]], int, float]) -> Union[int, float]:
         """
         Selects the next action
 
         :param o: the input observation
         :return: the next action and its probability
         """
-        return self.lookup_table[o].index(1)
+        return np.random.choice(np.arange(0, len(self.lookup_table[int(o)])), p=self.lookup_table[int(o)])
 
     def probability(self, o: Union[List[Union[int, float]], int, float], a: int) -> float:
         """
         Calculates the probability of taking a given action for a given observation
 
         :param o: the input observation
         :param a: the action
```

### Comparing `csle_common-0.2.0/src/csle_common/dao/training/vector_policy.py` & `csle_common-0.2.1/src/csle_common/dao/training/vector_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/logging/custom_formatter.py` & `csle_common-0.2.1/src/csle_common/logging/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/logging/log.py` & `csle_common-0.2.1/src/csle_common/logging/log.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/metastore/metastore_facade.py` & `csle_common-0.2.1/src/csle_common/metastore/metastore_facade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1246,19 +1246,21 @@
         """
         Logger.__call__().get_logger().debug("Saving a training job in the metastore")
         with psycopg.connect(f"{constants.METADATA_STORE.DB_NAME_PROPERTY}={constants.METADATA_STORE.DBNAME} "
                              f"{constants.METADATA_STORE.USER_PROPERTY}={constants.METADATA_STORE.USER} "
                              f"{constants.METADATA_STORE.PW_PROPERTY}={constants.METADATA_STORE.PASSWORD} "
                              f"{constants.METADATA_STORE.HOST_PROPERTY}={constants.METADATA_STORE.HOST}") as conn:
             with conn.cursor() as cur:
+                id = GeneralUtil.get_latest_table_id(cur=cur,
+                                                     table_name=constants.METADATA_STORE.TRAINING_JOBS_TABLE)
                 training_job_str = json.dumps(training_job.to_dict(), indent=4, sort_keys=True)
                 cur.execute(f"INSERT INTO {constants.METADATA_STORE.TRAINING_JOBS_TABLE} "
-                            f"(config, simulation_name, emulation_name, pid) "
-                            f"VALUES (%s, %s, %s, %s) RETURNING id",
-                            (training_job_str, training_job.simulation_env_name,
+                            f"(id, config, simulation_name, emulation_name, pid) "
+                            f"VALUES (%s, %s, %s, %s, %s) RETURNING id",
+                            (id, training_job_str, training_job.simulation_env_name,
                              training_job.emulation_env_name, training_job.pid))
                 id_of_new_row = cur.fetchone()[0]
                 conn.commit()
                 Logger.__call__().get_logger().debug("Training job saved successfully")
                 return id_of_new_row
 
     @staticmethod
```

### Comparing `csle_common-0.2.0/src/csle_common/models/fnn_w_softmax.py` & `csle_common-0.2.1/src/csle_common/models/fnn_w_softmax.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/tunneling/forward_ssh_controller.py` & `csle_common-0.2.1/src/csle_common/tunneling/forward_ssh_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/tunneling/forward_tunnel_thread.py` & `csle_common-0.2.1/src/csle_common/tunneling/forward_tunnel_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/cluster_util.py` & `csle_common-0.2.1/src/csle_common/util/cluster_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/connection_util.py` & `csle_common-0.2.1/src/csle_common/util/connection_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/docker_util.py` & `csle_common-0.2.1/src/csle_common/util/docker_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/emulation_util.py` & `csle_common-0.2.1/src/csle_common/util/emulation_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/env_dynamics_util.py` & `csle_common-0.2.1/src/csle_common/util/env_dynamics_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/experiment_util.py` & `csle_common-0.2.1/src/csle_common/util/experiment_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/export_util.py` & `csle_common-0.2.1/src/csle_common/util/export_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/general_util.py` & `csle_common-0.2.1/src/csle_common/util/general_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/grpc_util.py` & `csle_common-0.2.1/src/csle_common/util/grpc_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/import_util.py` & `csle_common-0.2.1/src/csle_common/util/import_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/management_util.py` & `csle_common-0.2.1/src/csle_common/util/management_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/plotting_util.py` & `csle_common-0.2.1/src/csle_common/util/plotting_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/read_emulation_statistics_util.py` & `csle_common-0.2.1/src/csle_common/util/read_emulation_statistics_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common/util/ssh_util.py` & `csle_common-0.2.1/src/csle_common/util/ssh_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.2.0/src/csle_common.egg-info/PKG-INFO` & `csle_common-0.2.1/src/csle_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-common
-Version: 0.2.0
+Version: 0.2.1
 Summary: Common functionality of the Cyber Security Learning Environment (CSLE)
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_common-0.2.0/src/csle_common.egg-info/SOURCES.txt` & `csle_common-0.2.1/src/csle_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,14 @@
 src/csle_common/dao/__init__.py
 src/csle_common/dao/datasets/__init__.py
 src/csle_common/dao/datasets/statistics_dataset.py
 src/csle_common/dao/datasets/traces_dataset.py
 src/csle_common/dao/docker/__init__.py
 src/csle_common/dao/docker/docker_container_metadata.py
 src/csle_common/dao/docker/docker_env_metadata.py
-src/csle_common/dao/domain_randomization/__init__.py
-src/csle_common/dao/domain_randomization/node_randomizer_config.py
-src/csle_common/dao/domain_randomization/randomization_space.py
-src/csle_common/dao/domain_randomization/randomization_space_config.py
 src/csle_common/dao/emulation_action/__init__.py
 src/csle_common/dao/emulation_action/attacker/__init__.py
 src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py
 src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py
 src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py
 src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_outcome.py
 src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_type.py
@@ -92,15 +88,14 @@
 src/csle_common/dao/emulation_action_result/nmap_trace.py
 src/csle_common/dao/emulation_action_result/nmap_vuln.py
 src/csle_common/dao/emulation_action_result/nmap_vulscan.py
 src/csle_common/dao/emulation_config/__init__.py
 src/csle_common/dao/emulation_config/beats_config.py
 src/csle_common/dao/emulation_config/client_managers_info.py
 src/csle_common/dao/emulation_config/client_population_config.py
-src/csle_common/dao/emulation_config/client_population_process_type.py
 src/csle_common/dao/emulation_config/cluster_config.py
 src/csle_common/dao/emulation_config/cluster_node.py
 src/csle_common/dao/emulation_config/config.py
 src/csle_common/dao/emulation_config/connection_setup_dto.py
 src/csle_common/dao/emulation_config/container_network.py
 src/csle_common/dao/emulation_config/containers_config.py
 src/csle_common/dao/emulation_config/credential.py
@@ -219,16 +214,19 @@
 src/csle_common/dao/training/alpha_vectors_policy.py
 src/csle_common/dao/training/dqn_policy.py
 src/csle_common/dao/training/experiment_config.py
 src/csle_common/dao/training/experiment_execution.py
 src/csle_common/dao/training/experiment_result.py
 src/csle_common/dao/training/fnn_with_softmax_policy.py
 src/csle_common/dao/training/hparam.py
+src/csle_common/dao/training/linear_tabular_policy.py
 src/csle_common/dao/training/linear_threshold_stopping_policy.py
+src/csle_common/dao/training/mixed_linear_tabular.py
 src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py
+src/csle_common/dao/training/mixed_ppo_policy.py
 src/csle_common/dao/training/multi_threshold_stopping_policy.py
 src/csle_common/dao/training/player_type.py
 src/csle_common/dao/training/policy.py
 src/csle_common/dao/training/policy_type.py
 src/csle_common/dao/training/ppo_policy.py
 src/csle_common/dao/training/random_policy.py
 src/csle_common/dao/training/tabular_policy.py
```

