# Comparing `tmp/rockset_v2_internal-2.0.2.tar.gz` & `tmp/rockset_v2_internal-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockset_v2_internal-2.0.2.tar", max compression
+gzip compressed data, was "rockset_v2_internal-2.0.3.tar", max compression
```

## Comparing `rockset_v2_internal-2.0.2.tar` & `rockset_v2_internal-2.0.3.tar`

### file list

```diff
@@ -1,240 +1,240 @@
--rw-r--r--   0        0        0      357 2023-05-31 19:49:16.995381 rockset_v2_internal-2.0.2/LONG_DESCRIPTION.rst
--rw-r--r--   0        0        0     1631 2023-05-31 20:54:20.725789 rockset_v2_internal-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     1374 2023-05-31 20:52:54.668784 rockset_v2_internal-2.0.2/rockset_v2/__init__.py
--rw-r--r--   0        0        0      211 2023-05-31 20:52:54.669430 rockset_v2_internal-2.0.2/rockset_v2/api/__init__.py
--rw-r--r--   0        0        0    34326 2023-05-31 20:52:54.678835 rockset_v2_internal-2.0.2/rockset_v2/api/aliases_api.py
--rw-r--r--   0        0        0    29389 2023-05-31 20:52:54.679641 rockset_v2_internal-2.0.2/rockset_v2/api/api_keys_api.py
--rw-r--r--   0        0        0   123960 2023-05-31 20:52:54.680752 rockset_v2_internal-2.0.2/rockset_v2/api/collections_api.py
--rw-r--r--   0        0        0    27749 2023-05-31 20:52:54.681502 rockset_v2_internal-2.0.2/rockset_v2/api/custom_roles_api.py
--rw-r--r--   0        0        0    20873 2023-05-31 20:52:54.682223 rockset_v2_internal-2.0.2/rockset_v2/api/documents_api.py
--rw-r--r--   0        0        0    72229 2023-05-31 20:52:54.683722 rockset_v2_internal-2.0.2/rockset_v2/api/integrations_api.py
--rw-r--r--   0        0        0     6127 2023-05-31 20:52:54.684546 rockset_v2_internal-2.0.2/rockset_v2/api/organizations_api.py
--rw-r--r--   0        0        0    34713 2023-05-31 20:52:54.685380 rockset_v2_internal-2.0.2/rockset_v2/api/queries_api.py
--rw-r--r--   0        0        0    86522 2023-05-31 20:52:54.686206 rockset_v2_internal-2.0.2/rockset_v2/api/query_lambdas_api.py
--rw-r--r--   0        0        0     7681 2023-05-31 20:52:54.686848 rockset_v2_internal-2.0.2/rockset_v2/api/shared_lambdas_api.py
--rw-r--r--   0        0        0    42739 2023-05-31 20:52:54.687560 rockset_v2_internal-2.0.2/rockset_v2/api/users_api.py
--rw-r--r--   0        0        0    34074 2023-05-31 20:52:54.688393 rockset_v2_internal-2.0.2/rockset_v2/api/views_api.py
--rw-r--r--   0        0        0    76699 2023-05-31 20:52:54.689360 rockset_v2_internal-2.0.2/rockset_v2/api/virtual_instances_api.py
--rw-r--r--   0        0        0    21874 2023-05-31 20:52:54.690146 rockset_v2_internal-2.0.2/rockset_v2/api/workspaces_api.py
--rw-r--r--   0        0        0    36257 2023-05-31 20:52:54.690953 rockset_v2_internal-2.0.2/rockset_v2/api_client.py
--rw-r--r--   0        0        0     1154 2023-05-31 20:52:54.691846 rockset_v2_internal-2.0.2/rockset_v2/apis/__init__.py
--rw-r--r--   0        0        0    15525 2023-05-31 20:52:54.692561 rockset_v2_internal-2.0.2/rockset_v2/configuration.py
--rw-r--r--   0        0        0     3831 2023-05-31 20:22:57.717401 rockset_v2_internal-2.0.2/rockset_v2/document.py
--rw-r--r--   0        0        0     6072 2023-05-31 20:22:57.717639 rockset_v2_internal-2.0.2/rockset_v2/exceptions.py
--rw-r--r--   0        0        0      348 2023-05-31 20:22:57.717962 rockset_v2_internal-2.0.2/rockset_v2/model/__init__.py
--rw-r--r--   0        0        0    11956 2023-05-31 20:52:54.693630 rockset_v2_internal-2.0.2/rockset_v2/model/add_documents_request.py
--rw-r--r--   0        0        0    11931 2023-05-31 20:52:54.694218 rockset_v2_internal-2.0.2/rockset_v2/model/add_documents_response.py
--rw-r--r--   0        0        0    13629 2023-05-31 20:52:54.695024 rockset_v2_internal-2.0.2/rockset_v2/model/alias.py
--rw-r--r--   0        0        0    13951 2023-05-31 20:52:54.696295 rockset_v2_internal-2.0.2/rockset_v2/model/api_key.py
--rw-r--r--   0        0        0    13816 2023-05-31 20:52:54.697323 rockset_v2_internal-2.0.2/rockset_v2/model/async_query_options.py
--rw-r--r--   0        0        0    13738 2023-05-31 20:52:54.697710 rockset_v2_internal-2.0.2/rockset_v2/model/auto_scaling_policy.py
--rw-r--r--   0        0        0    12235 2023-05-31 20:52:54.698681 rockset_v2_internal-2.0.2/rockset_v2/model/aws_access_key.py
--rw-r--r--   0        0        0    12107 2023-05-31 20:52:54.699789 rockset_v2_internal-2.0.2/rockset_v2/model/aws_role.py
--rw-r--r--   0        0        0    15090 2023-05-31 20:52:54.700798 rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_collection_creation_request.py
--rw-r--r--   0        0        0    11899 2023-05-31 20:52:54.701579 rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_integration.py
--rw-r--r--   0        0        0    12625 2023-05-31 20:52:54.702781 rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_integration_creation_request.py
--rw-r--r--   0        0        0    14461 2023-05-31 20:52:54.703521 rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_source_wrapper.py
--rw-r--r--   0        0        0    15070 2023-05-31 20:52:54.704595 rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_collection_creation_request.py
--rw-r--r--   0        0        0    11793 2023-05-31 20:52:54.705820 rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_integration.py
--rw-r--r--   0        0        0    12595 2023-05-31 20:52:54.706772 rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_integration_creation_request.py
--rw-r--r--   0        0        0    13464 2023-05-31 20:52:54.707823 rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_source_wrapper.py
--rw-r--r--   0        0        0    15080 2023-05-31 20:52:54.709390 rockset_v2_internal-2.0.2/rockset_v2/model/azure_service_bus_collection_creation_request.py
--rw-r--r--   0        0        0    11894 2023-05-31 20:52:54.710837 rockset_v2_internal-2.0.2/rockset_v2/model/azure_service_bus_integration.py
--rw-r--r--   0        0        0    13345 2023-05-31 20:52:54.712479 rockset_v2_internal-2.0.2/rockset_v2/model/azure_service_bus_source_wrapper.py
--rw-r--r--   0        0        0    18749 2023-05-31 20:52:54.713846 rockset_v2_internal-2.0.2/rockset_v2/model/bulk_stats.py
--rw-r--r--   0        0        0    11807 2023-05-31 20:52:54.715183 rockset_v2_internal-2.0.2/rockset_v2/model/cancel_query_response.py
--rw-r--r--   0        0        0    13231 2023-05-31 20:52:54.715939 rockset_v2_internal-2.0.2/rockset_v2/model/cluster.py
--rw-r--r--   0        0        0    17711 2023-05-31 20:52:54.717512 rockset_v2_internal-2.0.2/rockset_v2/model/collection.py
--rw-r--r--   0        0        0    14856 2023-05-31 20:52:54.719559 rockset_v2_internal-2.0.2/rockset_v2/model/collection_mount.py
--rw-r--r--   0        0        0    11861 2023-05-31 20:52:54.720428 rockset_v2_internal-2.0.2/rockset_v2/model/collection_mount_response.py
--rw-r--r--   0        0        0    11778 2023-05-31 20:52:54.721389 rockset_v2_internal-2.0.2/rockset_v2/model/collection_mount_stats.py
--rw-r--r--   0        0        0    16971 2023-05-31 20:52:54.725144 rockset_v2_internal-2.0.2/rockset_v2/model/collection_stats.py
--rw-r--r--   0        0        0    12339 2023-05-31 20:52:54.727224 rockset_v2_internal-2.0.2/rockset_v2/model/create_alias_request.py
--rw-r--r--   0        0        0    11778 2023-05-31 20:52:54.737776 rockset_v2_internal-2.0.2/rockset_v2/model/create_alias_response.py
--rw-r--r--   0        0        0    12104 2023-05-31 20:52:54.761872 rockset_v2_internal-2.0.2/rockset_v2/model/create_api_key_request.py
--rw-r--r--   0        0        0    11789 2023-05-31 20:52:54.763333 rockset_v2_internal-2.0.2/rockset_v2/model/create_api_key_response.py
--rw-r--r--   0        0        0    11771 2023-05-31 20:52:54.764061 rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_mount_request.py
--rw-r--r--   0        0        0    11922 2023-05-31 20:52:54.764798 rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_mounts_response.py
--rw-r--r--   0        0        0    14469 2023-05-31 20:52:54.765467 rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_request.py
--rw-r--r--   0        0        0    11828 2023-05-31 20:52:54.765965 rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_response.py
--rw-r--r--   0        0        0    16073 2023-05-31 20:52:54.766729 rockset_v2_internal-2.0.2/rockset_v2/model/create_integration_request.py
--rw-r--r--   0        0        0    11838 2023-05-31 20:52:54.767246 rockset_v2_internal-2.0.2/rockset_v2/model/create_integration_response.py
--rw-r--r--   0        0        0    12580 2023-05-31 20:52:54.767852 rockset_v2_internal-2.0.2/rockset_v2/model/create_query_lambda_request.py
--rw-r--r--   0        0        0    12069 2023-05-31 20:52:54.768352 rockset_v2_internal-2.0.2/rockset_v2/model/create_query_lambda_tag_request.py
--rw-r--r--   0        0        0    12510 2023-05-31 20:52:54.768856 rockset_v2_internal-2.0.2/rockset_v2/model/create_role_request.py
--rw-r--r--   0        0        0    12485 2023-05-31 20:52:54.769418 rockset_v2_internal-2.0.2/rockset_v2/model/create_user_request.py
--rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.770225 rockset_v2_internal-2.0.2/rockset_v2/model/create_user_response.py
--rw-r--r--   0        0        0    12176 2023-05-31 20:52:54.770846 rockset_v2_internal-2.0.2/rockset_v2/model/create_view_request.py
--rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.771427 rockset_v2_internal-2.0.2/rockset_v2/model/create_view_response.py
--rw-r--r--   0        0        0    14411 2023-05-31 20:52:54.771968 rockset_v2_internal-2.0.2/rockset_v2/model/create_virtual_instance_request.py
--rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.772546 rockset_v2_internal-2.0.2/rockset_v2/model/create_virtual_instance_response.py
--rw-r--r--   0        0        0    12044 2023-05-31 20:52:54.773122 rockset_v2_internal-2.0.2/rockset_v2/model/create_workspace_request.py
--rw-r--r--   0        0        0    11818 2023-05-31 20:52:54.773681 rockset_v2_internal-2.0.2/rockset_v2/model/create_workspace_response.py
--rw-r--r--   0        0        0    14185 2023-05-31 20:52:54.774385 rockset_v2_internal-2.0.2/rockset_v2/model/csv_params.py
--rw-r--r--   0        0        0    11778 2023-05-31 20:52:54.774966 rockset_v2_internal-2.0.2/rockset_v2/model/delete_alias_response.py
--rw-r--r--   0        0        0    11789 2023-05-31 20:52:54.775639 rockset_v2_internal-2.0.2/rockset_v2/model/delete_api_key_response.py
--rw-r--r--   0        0        0    11828 2023-05-31 20:52:54.776278 rockset_v2_internal-2.0.2/rockset_v2/model/delete_collection_response.py
--rw-r--r--   0        0        0    12045 2023-05-31 20:52:54.776848 rockset_v2_internal-2.0.2/rockset_v2/model/delete_documents_request.py
--rw-r--r--   0        0        0    11692 2023-05-31 20:52:54.777489 rockset_v2_internal-2.0.2/rockset_v2/model/delete_documents_request_data.py
--rw-r--r--   0        0        0    11936 2023-05-31 20:52:54.778541 rockset_v2_internal-2.0.2/rockset_v2/model/delete_documents_response.py
--rw-r--r--   0        0        0    11838 2023-05-31 20:52:54.779445 rockset_v2_internal-2.0.2/rockset_v2/model/delete_integration_response.py
--rw-r--r--   0        0        0    11839 2023-05-31 20:52:54.780123 rockset_v2_internal-2.0.2/rockset_v2/model/delete_query_lambda_response.py
--rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.780776 rockset_v2_internal-2.0.2/rockset_v2/model/delete_user_response.py
--rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.781405 rockset_v2_internal-2.0.2/rockset_v2/model/delete_view_response.py
--rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.781884 rockset_v2_internal-2.0.2/rockset_v2/model/delete_virtual_instance_response.py
--rw-r--r--   0        0        0    11818 2023-05-31 20:52:54.782423 rockset_v2_internal-2.0.2/rockset_v2/model/delete_workspace_response.py
--rw-r--r--   0        0        0    13032 2023-05-31 20:52:54.783053 rockset_v2_internal-2.0.2/rockset_v2/model/document_status.py
--rw-r--r--   0        0        0    15008 2023-05-31 20:52:54.783640 rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_collection_creation_request.py
--rw-r--r--   0        0        0    12575 2023-05-31 20:52:54.784429 rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_integration.py
--rw-r--r--   0        0        0    12493 2023-05-31 20:52:54.785247 rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_integration_creation_request.py
--rw-r--r--   0        0        0    14455 2023-05-31 20:52:54.785747 rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_source_wrapper.py
--rw-r--r--   0        0        0    14526 2023-05-31 20:52:54.786379 rockset_v2_internal-2.0.2/rockset_v2/model/error_model.py
--rw-r--r--   0        0        0    12398 2023-05-31 20:52:54.787029 rockset_v2_internal-2.0.2/rockset_v2/model/event_time_info.py
--rw-r--r--   0        0        0    12665 2023-05-31 20:52:54.788776 rockset_v2_internal-2.0.2/rockset_v2/model/execute_public_query_lambda_request.py
--rw-r--r--   0        0        0    15071 2023-05-31 20:52:54.789474 rockset_v2_internal-2.0.2/rockset_v2/model/execute_query_lambda_request.py
--rw-r--r--   0        0        0    11749 2023-05-31 20:52:54.790079 rockset_v2_internal-2.0.2/rockset_v2/model/field_mapping_query.py
--rw-r--r--   0        0        0    13087 2023-05-31 20:52:54.790704 rockset_v2_internal-2.0.2/rockset_v2/model/field_mapping_v2.py
--rw-r--r--   0        0        0    12549 2023-05-31 20:52:54.791297 rockset_v2_internal-2.0.2/rockset_v2/model/field_partition.py
--rw-r--r--   0        0        0    15029 2023-05-31 20:52:54.791891 rockset_v2_internal-2.0.2/rockset_v2/model/file_upload_collection_creation_request.py
--rw-r--r--   0        0        0    13623 2023-05-31 20:52:54.792409 rockset_v2_internal-2.0.2/rockset_v2/model/file_upload_source_wrapper.py
--rw-r--r--   0        0        0    13214 2023-05-31 20:52:54.792957 rockset_v2_internal-2.0.2/rockset_v2/model/format_params.py
--rw-r--r--   0        0        0    12007 2023-05-31 20:52:54.793500 rockset_v2_internal-2.0.2/rockset_v2/model/gcp_service_account.py
--rw-r--r--   0        0        0    14958 2023-05-31 20:52:54.794134 rockset_v2_internal-2.0.2/rockset_v2/model/gcs_collection_creation_request.py
--rw-r--r--   0        0        0    11924 2023-05-31 20:52:54.794888 rockset_v2_internal-2.0.2/rockset_v2/model/gcs_integration.py
--rw-r--r--   0        0        0    12418 2023-05-31 20:52:54.795809 rockset_v2_internal-2.0.2/rockset_v2/model/gcs_integration_creation_request.py
--rw-r--r--   0        0        0    14678 2023-05-31 20:52:54.796507 rockset_v2_internal-2.0.2/rockset_v2/model/gcs_source_wrapper.py
--rw-r--r--   0        0        0    11769 2023-05-31 20:52:54.797210 rockset_v2_internal-2.0.2/rockset_v2/model/get_alias_response.py
--rw-r--r--   0        0        0    11780 2023-05-31 20:52:54.797823 rockset_v2_internal-2.0.2/rockset_v2/model/get_api_key_response.py
--rw-r--r--   0        0        0    11819 2023-05-31 20:52:54.798426 rockset_v2_internal-2.0.2/rockset_v2/model/get_collection_response.py
--rw-r--r--   0        0        0    11829 2023-05-31 20:52:54.799070 rockset_v2_internal-2.0.2/rockset_v2/model/get_integration_response.py
--rw-r--r--   0        0        0    11798 2023-05-31 20:52:54.799760 rockset_v2_internal-2.0.2/rockset_v2/model/get_query_response.py
--rw-r--r--   0        0        0    11759 2023-05-31 20:52:54.800502 rockset_v2_internal-2.0.2/rockset_v2/model/get_view_response.py
--rw-r--r--   0        0        0    11870 2023-05-31 20:52:54.801176 rockset_v2_internal-2.0.2/rockset_v2/model/get_virtual_instance_response.py
--rw-r--r--   0        0        0    11809 2023-05-31 20:52:54.801799 rockset_v2_internal-2.0.2/rockset_v2/model/get_workspace_response.py
--rw-r--r--   0        0        0    12710 2023-05-31 20:52:54.802549 rockset_v2_internal-2.0.2/rockset_v2/model/input_field.py
--rw-r--r--   0        0        0    17401 2023-05-31 20:52:54.803292 rockset_v2_internal-2.0.2/rockset_v2/model/integration.py
--rw-r--r--   0        0        0    14978 2023-05-31 20:52:54.803958 rockset_v2_internal-2.0.2/rockset_v2/model/kafka_collection_creation_request.py
--rw-r--r--   0        0        0    14844 2023-05-31 20:52:54.804557 rockset_v2_internal-2.0.2/rockset_v2/model/kafka_integration.py
--rw-r--r--   0        0        0    12448 2023-05-31 20:52:54.805231 rockset_v2_internal-2.0.2/rockset_v2/model/kafka_integration_creation_request.py
--rw-r--r--   0        0        0    14039 2023-05-31 20:52:54.806144 rockset_v2_internal-2.0.2/rockset_v2/model/kafka_source_wrapper.py
--rw-r--r--   0        0        0    11851 2023-05-31 20:52:54.806771 rockset_v2_internal-2.0.2/rockset_v2/model/kafka_v3_security_config.py
--rw-r--r--   0        0        0    14998 2023-05-31 20:52:54.807438 rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_collection_creation_request.py
--rw-r--r--   0        0        0    12181 2023-05-31 20:52:54.808157 rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_integration.py
--rw-r--r--   0        0        0    12478 2023-05-31 20:52:54.808764 rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_integration_creation_request.py
--rw-r--r--   0        0        0    14277 2023-05-31 20:52:54.809373 rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_source_wrapper.py
--rw-r--r--   0        0        0    11828 2023-05-31 20:52:54.809989 rockset_v2_internal-2.0.2/rockset_v2/model/list_aliases_response.py
--rw-r--r--   0        0        0    11844 2023-05-31 20:52:54.810528 rockset_v2_internal-2.0.2/rockset_v2/model/list_api_keys_response.py
--rw-r--r--   0        0        0    11946 2023-05-31 20:52:54.811273 rockset_v2_internal-2.0.2/rockset_v2/model/list_collection_mounts_response.py
--rw-r--r--   0        0        0    11883 2023-05-31 20:52:54.811866 rockset_v2_internal-2.0.2/rockset_v2/model/list_collections_response.py
--rw-r--r--   0        0        0    11901 2023-05-31 20:52:54.812416 rockset_v2_internal-2.0.2/rockset_v2/model/list_integrations_response.py
--rw-r--r--   0        0        0    11813 2023-05-31 20:52:54.813018 rockset_v2_internal-2.0.2/rockset_v2/model/list_queries_response.py
--rw-r--r--   0        0        0    11973 2023-05-31 20:52:54.813725 rockset_v2_internal-2.0.2/rockset_v2/model/list_query_lambda_tags_response.py
--rw-r--r--   0        0        0    12019 2023-05-31 20:52:54.814288 rockset_v2_internal-2.0.2/rockset_v2/model/list_query_lambda_versions_response.py
--rw-r--r--   0        0        0    11898 2023-05-31 20:52:54.814906 rockset_v2_internal-2.0.2/rockset_v2/model/list_query_lambdas_response.py
--rw-r--r--   0        0        0    11811 2023-05-31 20:52:54.815485 rockset_v2_internal-2.0.2/rockset_v2/model/list_roles_response.py
--rw-r--r--   0        0        0    12012 2023-05-31 20:52:54.816034 rockset_v2_internal-2.0.2/rockset_v2/model/list_unsubscribe_preferences_response.py
--rw-r--r--   0        0        0    11803 2023-05-31 20:52:54.816755 rockset_v2_internal-2.0.2/rockset_v2/model/list_users_response.py
--rw-r--r--   0        0        0    11811 2023-05-31 20:52:54.817393 rockset_v2_internal-2.0.2/rockset_v2/model/list_views_response.py
--rw-r--r--   0        0        0    11946 2023-05-31 20:52:54.818009 rockset_v2_internal-2.0.2/rockset_v2/model/list_virtual_instances_response.py
--rw-r--r--   0        0        0    11863 2023-05-31 20:52:54.818520 rockset_v2_internal-2.0.2/rockset_v2/model/list_workspaces_response.py
--rw-r--r--   0        0        0    11821 2023-05-31 20:52:54.818957 rockset_v2_internal-2.0.2/rockset_v2/model/mongo_db_integration.py
--rw-r--r--   0        0        0    14998 2023-05-31 20:52:54.819368 rockset_v2_internal-2.0.2/rockset_v2/model/mongodb_collection_creation_request.py
--rw-r--r--   0        0        0    12479 2023-05-31 20:52:54.819828 rockset_v2_internal-2.0.2/rockset_v2/model/mongodb_integration_creation_request.py
--rw-r--r--   0        0        0    14135 2023-05-31 20:52:54.820417 rockset_v2_internal-2.0.2/rockset_v2/model/mongodb_source_wrapper.py
--rw-r--r--   0        0        0    13286 2023-05-31 20:52:54.821198 rockset_v2_internal-2.0.2/rockset_v2/model/organization.py
--rw-r--r--   0        0        0    11830 2023-05-31 20:52:54.821707 rockset_v2_internal-2.0.2/rockset_v2/model/organization_response.py
--rw-r--r--   0        0        0    12536 2023-05-31 20:52:54.822222 rockset_v2_internal-2.0.2/rockset_v2/model/output_field.py
--rw-r--r--   0        0        0    11781 2023-05-31 20:52:54.822887 rockset_v2_internal-2.0.2/rockset_v2/model/pagination.py
--rw-r--r--   0        0        0    13061 2023-05-31 20:52:54.823465 rockset_v2_internal-2.0.2/rockset_v2/model/pagination_info.py
--rw-r--r--   0        0        0    12164 2023-05-31 20:52:54.823998 rockset_v2_internal-2.0.2/rockset_v2/model/patch_document.py
--rw-r--r--   0        0        0    11929 2023-05-31 20:52:54.824597 rockset_v2_internal-2.0.2/rockset_v2/model/patch_documents_request.py
--rw-r--r--   0        0        0    11877 2023-05-31 20:52:54.825322 rockset_v2_internal-2.0.2/rockset_v2/model/patch_documents_response.py
--rw-r--r--   0        0        0    13678 2023-05-31 20:52:54.826018 rockset_v2_internal-2.0.2/rockset_v2/model/patch_operation.py
--rw-r--r--   0        0        0    15368 2023-05-31 20:52:54.826678 rockset_v2_internal-2.0.2/rockset_v2/model/privilege.py
--rw-r--r--   0        0        0    12413 2023-05-31 20:52:54.827279 rockset_v2_internal-2.0.2/rockset_v2/model/query_error.py
--rw-r--r--   0        0        0    11913 2023-05-31 20:52:54.827812 rockset_v2_internal-2.0.2/rockset_v2/model/query_field_type.py
--rw-r--r--   0        0        0    14987 2023-05-31 20:52:54.828428 rockset_v2_internal-2.0.2/rockset_v2/model/query_info.py
--rw-r--r--   0        0        0    13697 2023-05-31 20:52:54.829507 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda.py
--rw-r--r--   0        0        0    12228 2023-05-31 20:52:54.830135 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_sql.py
--rw-r--r--   0        0        0    12792 2023-05-31 20:52:54.830680 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_stats.py
--rw-r--r--   0        0        0    12133 2023-05-31 20:52:54.831264 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_tag.py
--rw-r--r--   0        0        0    11852 2023-05-31 20:52:54.831771 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_tag_response.py
--rw-r--r--   0        0        0    14853 2023-05-31 20:52:54.832400 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_version.py
--rw-r--r--   0        0        0    11892 2023-05-31 20:52:54.832985 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_version_response.py
--rw-r--r--   0        0        0    12738 2023-05-31 20:52:54.833662 rockset_v2_internal-2.0.2/rockset_v2/model/query_pagination_response.py
--rw-r--r--   0        0        0    12194 2023-05-31 20:52:54.834352 rockset_v2_internal-2.0.2/rockset_v2/model/query_parameter.py
--rw-r--r--   0        0        0    12931 2023-05-31 20:52:54.834962 rockset_v2_internal-2.0.2/rockset_v2/model/query_request.py
--rw-r--r--   0        0        0    13635 2023-05-31 20:52:54.835566 rockset_v2_internal-2.0.2/rockset_v2/model/query_request_sql.py
--rw-r--r--   0        0        0    15855 2023-05-31 20:52:54.836172 rockset_v2_internal-2.0.2/rockset_v2/model/query_response.py
--rw-r--r--   0        0        0    12111 2023-05-31 20:52:54.836759 rockset_v2_internal-2.0.2/rockset_v2/model/query_response_stats.py
--rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.837479 rockset_v2_internal-2.0.2/rockset_v2/model/resume_virtual_instance_response.py
--rw-r--r--   0        0        0    13372 2023-05-31 20:52:54.837978 rockset_v2_internal-2.0.2/rockset_v2/model/role.py
--rw-r--r--   0        0        0    11750 2023-05-31 20:52:54.838436 rockset_v2_internal-2.0.2/rockset_v2/model/role_response.py
--rw-r--r--   0        0        0    14948 2023-05-31 20:52:54.838895 rockset_v2_internal-2.0.2/rockset_v2/model/s3_collection_creation_request.py
--rw-r--r--   0        0        0    12166 2023-05-31 20:52:54.839359 rockset_v2_internal-2.0.2/rockset_v2/model/s3_integration.py
--rw-r--r--   0        0        0    12403 2023-05-31 20:52:54.839833 rockset_v2_internal-2.0.2/rockset_v2/model/s3_integration_creation_request.py
--rw-r--r--   0        0        0    15251 2023-05-31 20:52:54.840241 rockset_v2_internal-2.0.2/rockset_v2/model/s3_source_wrapper.py
--rw-r--r--   0        0        0    12207 2023-05-31 20:52:54.840748 rockset_v2_internal-2.0.2/rockset_v2/model/schema_registry_config.py
--rw-r--r--   0        0        0    11696 2023-05-31 20:22:57.768957 rockset_v2_internal-2.0.2/rockset_v2/model/segment_integration.py
--rw-r--r--   0        0        0    12465 2023-05-31 20:22:57.769388 rockset_v2_internal-2.0.2/rockset_v2/model/segment_integration_creation_request.py
--rw-r--r--   0        0        0    15018 2023-05-31 20:52:54.841148 rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_collection_creation_request.py
--rw-r--r--   0        0        0    14462 2023-05-31 20:52:54.841656 rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_integration.py
--rw-r--r--   0        0        0    12508 2023-05-31 20:52:54.842466 rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_integration_creation_request.py
--rw-r--r--   0        0        0    13919 2023-05-31 20:52:54.843061 rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_source_wrapper.py
--rw-r--r--   0        0        0    12513 2023-05-31 20:52:54.843639 rockset_v2_internal-2.0.2/rockset_v2/model/source.py
--rw-r--r--   0        0        0    13175 2023-05-31 20:52:54.844600 rockset_v2_internal-2.0.2/rockset_v2/model/source_azure_blob_storage.py
--rw-r--r--   0        0        0    12673 2023-05-31 20:52:54.845250 rockset_v2_internal-2.0.2/rockset_v2/model/source_azure_event_hubs.py
--rw-r--r--   0        0        0    12561 2023-05-31 20:52:54.845894 rockset_v2_internal-2.0.2/rockset_v2/model/source_azure_service_bus.py
--rw-r--r--   0        0        0    13636 2023-05-31 20:52:54.846554 rockset_v2_internal-2.0.2/rockset_v2/model/source_dynamo_db.py
--rw-r--r--   0        0        0    12397 2023-05-31 20:52:54.847182 rockset_v2_internal-2.0.2/rockset_v2/model/source_file_upload.py
--rw-r--r--   0        0        0    13377 2023-05-31 20:52:54.847838 rockset_v2_internal-2.0.2/rockset_v2/model/source_gcs.py
--rw-r--r--   0        0        0    13218 2023-05-31 20:52:54.848518 rockset_v2_internal-2.0.2/rockset_v2/model/source_kafka.py
--rw-r--r--   0        0        0    13030 2023-05-31 20:52:54.849174 rockset_v2_internal-2.0.2/rockset_v2/model/source_kinesis.py
--rw-r--r--   0        0        0    13324 2023-05-31 20:52:54.849861 rockset_v2_internal-2.0.2/rockset_v2/model/source_mongo_db.py
--rw-r--r--   0        0        0    13929 2023-05-31 20:52:54.850690 rockset_v2_internal-2.0.2/rockset_v2/model/source_s3.py
--rw-r--r--   0        0        0    13119 2023-05-31 20:52:54.851312 rockset_v2_internal-2.0.2/rockset_v2/model/source_snowflake.py
--rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.851690 rockset_v2_internal-2.0.2/rockset_v2/model/source_system.py
--rw-r--r--   0        0        0    11667 2023-05-31 20:52:54.852404 rockset_v2_internal-2.0.2/rockset_v2/model/sql_expression.py
--rw-r--r--   0        0        0    13122 2023-05-31 20:52:54.853717 rockset_v2_internal-2.0.2/rockset_v2/model/stats.py
--rw-r--r--   0        0        0    13664 2023-05-31 20:52:54.854365 rockset_v2_internal-2.0.2/rockset_v2/model/status.py
--rw-r--r--   0        0        0    13120 2023-05-31 20:52:54.854952 rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_event_hubs.py
--rw-r--r--   0        0        0    12370 2023-05-31 20:52:54.855801 rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_event_hubs_partition.py
--rw-r--r--   0        0        0    12736 2023-05-31 20:52:54.856414 rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_service_bus.py
--rw-r--r--   0        0        0    12216 2023-05-31 20:52:54.857296 rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_service_bus_session.py
--rw-r--r--   0        0        0    13569 2023-05-31 20:52:54.857991 rockset_v2_internal-2.0.2/rockset_v2/model/status_dynamo_db.py
--rw-r--r--   0        0        0    12711 2023-05-31 20:52:54.858679 rockset_v2_internal-2.0.2/rockset_v2/model/status_dynamo_db_v2.py
--rw-r--r--   0        0        0    13132 2023-05-31 20:52:54.859333 rockset_v2_internal-2.0.2/rockset_v2/model/status_kafka.py
--rw-r--r--   0        0        0    12343 2023-05-31 20:52:54.859863 rockset_v2_internal-2.0.2/rockset_v2/model/status_kafka_partition.py
--rw-r--r--   0        0        0    15620 2023-05-31 20:52:54.860443 rockset_v2_internal-2.0.2/rockset_v2/model/status_mongo_db.py
--rw-r--r--   0        0        0    11930 2023-05-31 20:52:54.860923 rockset_v2_internal-2.0.2/rockset_v2/model/status_snowflake.py
--rw-r--r--   0        0        0    11882 2023-05-31 20:52:54.861396 rockset_v2_internal-2.0.2/rockset_v2/model/suspend_virtual_instance_response.py
--rw-r--r--   0        0        0    11900 2023-05-31 20:52:54.862111 rockset_v2_internal-2.0.2/rockset_v2/model/unsubscribe_preference.py
--rw-r--r--   0        0        0    12125 2023-05-31 20:52:54.862684 rockset_v2_internal-2.0.2/rockset_v2/model/update_alias_request.py
--rw-r--r--   0        0        0    11824 2023-05-31 20:52:54.863145 rockset_v2_internal-2.0.2/rockset_v2/model/update_api_key_request.py
--rw-r--r--   0        0        0    11789 2023-05-31 20:52:54.863693 rockset_v2_internal-2.0.2/rockset_v2/model/update_api_key_response.py
--rw-r--r--   0        0        0    12256 2023-05-31 20:52:54.864067 rockset_v2_internal-2.0.2/rockset_v2/model/update_collection_request.py
--rw-r--r--   0        0        0    11867 2023-05-31 20:22:57.782858 rockset_v2_internal-2.0.2/rockset_v2/model/update_integration_request.py
--rw-r--r--   0        0        0    11829 2023-05-31 20:22:57.783231 rockset_v2_internal-2.0.2/rockset_v2/model/update_integration_response.py
--rw-r--r--   0        0        0    12338 2023-05-31 20:52:54.864615 rockset_v2_internal-2.0.2/rockset_v2/model/update_query_lambda_request.py
--rw-r--r--   0        0        0    12231 2023-05-31 20:52:54.865200 rockset_v2_internal-2.0.2/rockset_v2/model/update_role_request.py
--rw-r--r--   0        0        0    12015 2023-05-31 20:52:54.865776 rockset_v2_internal-2.0.2/rockset_v2/model/update_unsubscribe_preferences_request.py
--rw-r--r--   0        0        0    12018 2023-05-31 20:52:54.866368 rockset_v2_internal-2.0.2/rockset_v2/model/update_unsubscribe_preferences_response.py
--rw-r--r--   0        0        0    12212 2023-05-31 20:52:54.866855 rockset_v2_internal-2.0.2/rockset_v2/model/update_user_request.py
--rw-r--r--   0        0        0    11964 2023-05-31 20:52:54.867381 rockset_v2_internal-2.0.2/rockset_v2/model/update_view_request.py
--rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.867851 rockset_v2_internal-2.0.2/rockset_v2/model/update_view_response.py
--rw-r--r--   0        0        0    15183 2023-05-31 20:52:54.868410 rockset_v2_internal-2.0.2/rockset_v2/model/update_virtual_instance_request.py
--rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.869001 rockset_v2_internal-2.0.2/rockset_v2/model/update_virtual_instance_response.py
--rw-r--r--   0        0        0    12913 2023-05-31 20:52:54.869670 rockset_v2_internal-2.0.2/rockset_v2/model/user.py
--rw-r--r--   0        0        0    12161 2023-05-31 20:52:54.870144 rockset_v2_internal-2.0.2/rockset_v2/model/validate_query_response.py
--rw-r--r--   0        0        0    14479 2023-05-31 20:52:54.870672 rockset_v2_internal-2.0.2/rockset_v2/model/view.py
--rw-r--r--   0        0        0    18641 2023-05-31 20:52:54.871271 rockset_v2_internal-2.0.2/rockset_v2/model/virtual_instance.py
--rw-r--r--   0        0        0    11778 2023-05-31 20:52:54.871892 rockset_v2_internal-2.0.2/rockset_v2/model/virtual_instance_stats.py
--rw-r--r--   0        0        0    12977 2023-05-31 20:52:54.872539 rockset_v2_internal-2.0.2/rockset_v2/model/workspace.py
--rw-r--r--   0        0        0    13004 2023-05-31 20:52:54.873194 rockset_v2_internal-2.0.2/rockset_v2/model/xml_params.py
--rw-r--r--   0        0        0    84040 2023-05-31 20:52:54.874454 rockset_v2_internal-2.0.2/rockset_v2/model_utils.py
--rw-r--r--   0        0        0    15316 2023-05-31 20:52:54.875183 rockset_v2_internal-2.0.2/rockset_v2/models/__init__.py
--rw-r--r--   0        0        0     1819 2023-05-31 20:22:57.821569 rockset_v2_internal-2.0.2/rockset_v2/query_paginator.py
--rw-r--r--   0        0        0    14648 2023-05-31 20:52:54.875917 rockset_v2_internal-2.0.2/rockset_v2/rest.py
--rw-r--r--   0        0        0     8926 2023-05-31 20:52:54.876525 rockset_v2_internal-2.0.2/rockset_v2/rockset_client.py
--rw-r--r--   0        0        0     3644 2023-05-31 20:22:57.826319 rockset_v2_internal-2.0.2/rockset_v2/value.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 rockset_v2_internal-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      357 2023-05-31 19:49:16.995381 rockset_v2_internal-2.0.3/LONG_DESCRIPTION.rst
+-rw-r--r--   0        0        0     1631 2023-05-31 20:57:10.217085 rockset_v2_internal-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1374 2023-05-31 20:52:54.668784 rockset_v2_internal-2.0.3/rockset_v2/__init__.py
+-rw-r--r--   0        0        0      211 2023-05-31 20:52:54.669430 rockset_v2_internal-2.0.3/rockset_v2/api/__init__.py
+-rw-r--r--   0        0        0    34326 2023-05-31 20:52:54.678835 rockset_v2_internal-2.0.3/rockset_v2/api/aliases_api.py
+-rw-r--r--   0        0        0    29389 2023-05-31 20:52:54.679641 rockset_v2_internal-2.0.3/rockset_v2/api/api_keys_api.py
+-rw-r--r--   0        0        0   123960 2023-05-31 20:52:54.680752 rockset_v2_internal-2.0.3/rockset_v2/api/collections_api.py
+-rw-r--r--   0        0        0    27749 2023-05-31 20:52:54.681502 rockset_v2_internal-2.0.3/rockset_v2/api/custom_roles_api.py
+-rw-r--r--   0        0        0    20873 2023-05-31 20:52:54.682223 rockset_v2_internal-2.0.3/rockset_v2/api/documents_api.py
+-rw-r--r--   0        0        0    72229 2023-05-31 20:52:54.683722 rockset_v2_internal-2.0.3/rockset_v2/api/integrations_api.py
+-rw-r--r--   0        0        0     6127 2023-05-31 20:52:54.684546 rockset_v2_internal-2.0.3/rockset_v2/api/organizations_api.py
+-rw-r--r--   0        0        0    34713 2023-05-31 20:52:54.685380 rockset_v2_internal-2.0.3/rockset_v2/api/queries_api.py
+-rw-r--r--   0        0        0    86522 2023-05-31 20:52:54.686206 rockset_v2_internal-2.0.3/rockset_v2/api/query_lambdas_api.py
+-rw-r--r--   0        0        0     7681 2023-05-31 20:52:54.686848 rockset_v2_internal-2.0.3/rockset_v2/api/shared_lambdas_api.py
+-rw-r--r--   0        0        0    42739 2023-05-31 20:52:54.687560 rockset_v2_internal-2.0.3/rockset_v2/api/users_api.py
+-rw-r--r--   0        0        0    34074 2023-05-31 20:52:54.688393 rockset_v2_internal-2.0.3/rockset_v2/api/views_api.py
+-rw-r--r--   0        0        0    76699 2023-05-31 20:52:54.689360 rockset_v2_internal-2.0.3/rockset_v2/api/virtual_instances_api.py
+-rw-r--r--   0        0        0    21874 2023-05-31 20:52:54.690146 rockset_v2_internal-2.0.3/rockset_v2/api/workspaces_api.py
+-rw-r--r--   0        0        0    36257 2023-05-31 20:52:54.690953 rockset_v2_internal-2.0.3/rockset_v2/api_client.py
+-rw-r--r--   0        0        0     1154 2023-05-31 20:52:54.691846 rockset_v2_internal-2.0.3/rockset_v2/apis/__init__.py
+-rw-r--r--   0        0        0    15525 2023-05-31 20:52:54.692561 rockset_v2_internal-2.0.3/rockset_v2/configuration.py
+-rw-r--r--   0        0        0     3831 2023-05-31 20:22:57.717401 rockset_v2_internal-2.0.3/rockset_v2/document.py
+-rw-r--r--   0        0        0     6072 2023-05-31 20:22:57.717639 rockset_v2_internal-2.0.3/rockset_v2/exceptions.py
+-rw-r--r--   0        0        0      348 2023-05-31 20:22:57.717962 rockset_v2_internal-2.0.3/rockset_v2/model/__init__.py
+-rw-r--r--   0        0        0    11956 2023-05-31 20:52:54.693630 rockset_v2_internal-2.0.3/rockset_v2/model/add_documents_request.py
+-rw-r--r--   0        0        0    11931 2023-05-31 20:52:54.694218 rockset_v2_internal-2.0.3/rockset_v2/model/add_documents_response.py
+-rw-r--r--   0        0        0    13629 2023-05-31 20:52:54.695024 rockset_v2_internal-2.0.3/rockset_v2/model/alias.py
+-rw-r--r--   0        0        0    13951 2023-05-31 20:52:54.696295 rockset_v2_internal-2.0.3/rockset_v2/model/api_key.py
+-rw-r--r--   0        0        0    13816 2023-05-31 20:52:54.697323 rockset_v2_internal-2.0.3/rockset_v2/model/async_query_options.py
+-rw-r--r--   0        0        0    13738 2023-05-31 20:52:54.697710 rockset_v2_internal-2.0.3/rockset_v2/model/auto_scaling_policy.py
+-rw-r--r--   0        0        0    12235 2023-05-31 20:52:54.698681 rockset_v2_internal-2.0.3/rockset_v2/model/aws_access_key.py
+-rw-r--r--   0        0        0    12107 2023-05-31 20:52:54.699789 rockset_v2_internal-2.0.3/rockset_v2/model/aws_role.py
+-rw-r--r--   0        0        0    15090 2023-05-31 20:52:54.700798 rockset_v2_internal-2.0.3/rockset_v2/model/azure_blob_storage_collection_creation_request.py
+-rw-r--r--   0        0        0    11899 2023-05-31 20:52:54.701579 rockset_v2_internal-2.0.3/rockset_v2/model/azure_blob_storage_integration.py
+-rw-r--r--   0        0        0    12625 2023-05-31 20:52:54.702781 rockset_v2_internal-2.0.3/rockset_v2/model/azure_blob_storage_integration_creation_request.py
+-rw-r--r--   0        0        0    14461 2023-05-31 20:52:54.703521 rockset_v2_internal-2.0.3/rockset_v2/model/azure_blob_storage_source_wrapper.py
+-rw-r--r--   0        0        0    15070 2023-05-31 20:52:54.704595 rockset_v2_internal-2.0.3/rockset_v2/model/azure_event_hubs_collection_creation_request.py
+-rw-r--r--   0        0        0    11793 2023-05-31 20:52:54.705820 rockset_v2_internal-2.0.3/rockset_v2/model/azure_event_hubs_integration.py
+-rw-r--r--   0        0        0    12595 2023-05-31 20:52:54.706772 rockset_v2_internal-2.0.3/rockset_v2/model/azure_event_hubs_integration_creation_request.py
+-rw-r--r--   0        0        0    13464 2023-05-31 20:52:54.707823 rockset_v2_internal-2.0.3/rockset_v2/model/azure_event_hubs_source_wrapper.py
+-rw-r--r--   0        0        0    15080 2023-05-31 20:52:54.709390 rockset_v2_internal-2.0.3/rockset_v2/model/azure_service_bus_collection_creation_request.py
+-rw-r--r--   0        0        0    11894 2023-05-31 20:52:54.710837 rockset_v2_internal-2.0.3/rockset_v2/model/azure_service_bus_integration.py
+-rw-r--r--   0        0        0    13345 2023-05-31 20:52:54.712479 rockset_v2_internal-2.0.3/rockset_v2/model/azure_service_bus_source_wrapper.py
+-rw-r--r--   0        0        0    18749 2023-05-31 20:52:54.713846 rockset_v2_internal-2.0.3/rockset_v2/model/bulk_stats.py
+-rw-r--r--   0        0        0    11807 2023-05-31 20:52:54.715183 rockset_v2_internal-2.0.3/rockset_v2/model/cancel_query_response.py
+-rw-r--r--   0        0        0    13231 2023-05-31 20:52:54.715939 rockset_v2_internal-2.0.3/rockset_v2/model/cluster.py
+-rw-r--r--   0        0        0    17711 2023-05-31 20:52:54.717512 rockset_v2_internal-2.0.3/rockset_v2/model/collection.py
+-rw-r--r--   0        0        0    14856 2023-05-31 20:52:54.719559 rockset_v2_internal-2.0.3/rockset_v2/model/collection_mount.py
+-rw-r--r--   0        0        0    11861 2023-05-31 20:52:54.720428 rockset_v2_internal-2.0.3/rockset_v2/model/collection_mount_response.py
+-rw-r--r--   0        0        0    11778 2023-05-31 20:52:54.721389 rockset_v2_internal-2.0.3/rockset_v2/model/collection_mount_stats.py
+-rw-r--r--   0        0        0    16971 2023-05-31 20:52:54.725144 rockset_v2_internal-2.0.3/rockset_v2/model/collection_stats.py
+-rw-r--r--   0        0        0    12339 2023-05-31 20:52:54.727224 rockset_v2_internal-2.0.3/rockset_v2/model/create_alias_request.py
+-rw-r--r--   0        0        0    11778 2023-05-31 20:52:54.737776 rockset_v2_internal-2.0.3/rockset_v2/model/create_alias_response.py
+-rw-r--r--   0        0        0    12104 2023-05-31 20:52:54.761872 rockset_v2_internal-2.0.3/rockset_v2/model/create_api_key_request.py
+-rw-r--r--   0        0        0    11789 2023-05-31 20:52:54.763333 rockset_v2_internal-2.0.3/rockset_v2/model/create_api_key_response.py
+-rw-r--r--   0        0        0    11771 2023-05-31 20:52:54.764061 rockset_v2_internal-2.0.3/rockset_v2/model/create_collection_mount_request.py
+-rw-r--r--   0        0        0    11922 2023-05-31 20:52:54.764798 rockset_v2_internal-2.0.3/rockset_v2/model/create_collection_mounts_response.py
+-rw-r--r--   0        0        0    14469 2023-05-31 20:52:54.765467 rockset_v2_internal-2.0.3/rockset_v2/model/create_collection_request.py
+-rw-r--r--   0        0        0    11828 2023-05-31 20:52:54.765965 rockset_v2_internal-2.0.3/rockset_v2/model/create_collection_response.py
+-rw-r--r--   0        0        0    16073 2023-05-31 20:52:54.766729 rockset_v2_internal-2.0.3/rockset_v2/model/create_integration_request.py
+-rw-r--r--   0        0        0    11838 2023-05-31 20:52:54.767246 rockset_v2_internal-2.0.3/rockset_v2/model/create_integration_response.py
+-rw-r--r--   0        0        0    12580 2023-05-31 20:52:54.767852 rockset_v2_internal-2.0.3/rockset_v2/model/create_query_lambda_request.py
+-rw-r--r--   0        0        0    12069 2023-05-31 20:52:54.768352 rockset_v2_internal-2.0.3/rockset_v2/model/create_query_lambda_tag_request.py
+-rw-r--r--   0        0        0    12510 2023-05-31 20:52:54.768856 rockset_v2_internal-2.0.3/rockset_v2/model/create_role_request.py
+-rw-r--r--   0        0        0    12485 2023-05-31 20:52:54.769418 rockset_v2_internal-2.0.3/rockset_v2/model/create_user_request.py
+-rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.770225 rockset_v2_internal-2.0.3/rockset_v2/model/create_user_response.py
+-rw-r--r--   0        0        0    12176 2023-05-31 20:52:54.770846 rockset_v2_internal-2.0.3/rockset_v2/model/create_view_request.py
+-rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.771427 rockset_v2_internal-2.0.3/rockset_v2/model/create_view_response.py
+-rw-r--r--   0        0        0    14411 2023-05-31 20:52:54.771968 rockset_v2_internal-2.0.3/rockset_v2/model/create_virtual_instance_request.py
+-rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.772546 rockset_v2_internal-2.0.3/rockset_v2/model/create_virtual_instance_response.py
+-rw-r--r--   0        0        0    12044 2023-05-31 20:52:54.773122 rockset_v2_internal-2.0.3/rockset_v2/model/create_workspace_request.py
+-rw-r--r--   0        0        0    11818 2023-05-31 20:52:54.773681 rockset_v2_internal-2.0.3/rockset_v2/model/create_workspace_response.py
+-rw-r--r--   0        0        0    14185 2023-05-31 20:52:54.774385 rockset_v2_internal-2.0.3/rockset_v2/model/csv_params.py
+-rw-r--r--   0        0        0    11778 2023-05-31 20:52:54.774966 rockset_v2_internal-2.0.3/rockset_v2/model/delete_alias_response.py
+-rw-r--r--   0        0        0    11789 2023-05-31 20:52:54.775639 rockset_v2_internal-2.0.3/rockset_v2/model/delete_api_key_response.py
+-rw-r--r--   0        0        0    11828 2023-05-31 20:52:54.776278 rockset_v2_internal-2.0.3/rockset_v2/model/delete_collection_response.py
+-rw-r--r--   0        0        0    12045 2023-05-31 20:52:54.776848 rockset_v2_internal-2.0.3/rockset_v2/model/delete_documents_request.py
+-rw-r--r--   0        0        0    11692 2023-05-31 20:52:54.777489 rockset_v2_internal-2.0.3/rockset_v2/model/delete_documents_request_data.py
+-rw-r--r--   0        0        0    11936 2023-05-31 20:52:54.778541 rockset_v2_internal-2.0.3/rockset_v2/model/delete_documents_response.py
+-rw-r--r--   0        0        0    11838 2023-05-31 20:52:54.779445 rockset_v2_internal-2.0.3/rockset_v2/model/delete_integration_response.py
+-rw-r--r--   0        0        0    11839 2023-05-31 20:52:54.780123 rockset_v2_internal-2.0.3/rockset_v2/model/delete_query_lambda_response.py
+-rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.780776 rockset_v2_internal-2.0.3/rockset_v2/model/delete_user_response.py
+-rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.781405 rockset_v2_internal-2.0.3/rockset_v2/model/delete_view_response.py
+-rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.781884 rockset_v2_internal-2.0.3/rockset_v2/model/delete_virtual_instance_response.py
+-rw-r--r--   0        0        0    11818 2023-05-31 20:52:54.782423 rockset_v2_internal-2.0.3/rockset_v2/model/delete_workspace_response.py
+-rw-r--r--   0        0        0    13032 2023-05-31 20:52:54.783053 rockset_v2_internal-2.0.3/rockset_v2/model/document_status.py
+-rw-r--r--   0        0        0    15008 2023-05-31 20:52:54.783640 rockset_v2_internal-2.0.3/rockset_v2/model/dynamodb_collection_creation_request.py
+-rw-r--r--   0        0        0    12575 2023-05-31 20:52:54.784429 rockset_v2_internal-2.0.3/rockset_v2/model/dynamodb_integration.py
+-rw-r--r--   0        0        0    12493 2023-05-31 20:52:54.785247 rockset_v2_internal-2.0.3/rockset_v2/model/dynamodb_integration_creation_request.py
+-rw-r--r--   0        0        0    14455 2023-05-31 20:52:54.785747 rockset_v2_internal-2.0.3/rockset_v2/model/dynamodb_source_wrapper.py
+-rw-r--r--   0        0        0    14526 2023-05-31 20:52:54.786379 rockset_v2_internal-2.0.3/rockset_v2/model/error_model.py
+-rw-r--r--   0        0        0    12398 2023-05-31 20:52:54.787029 rockset_v2_internal-2.0.3/rockset_v2/model/event_time_info.py
+-rw-r--r--   0        0        0    12665 2023-05-31 20:52:54.788776 rockset_v2_internal-2.0.3/rockset_v2/model/execute_public_query_lambda_request.py
+-rw-r--r--   0        0        0    15071 2023-05-31 20:52:54.789474 rockset_v2_internal-2.0.3/rockset_v2/model/execute_query_lambda_request.py
+-rw-r--r--   0        0        0    11749 2023-05-31 20:52:54.790079 rockset_v2_internal-2.0.3/rockset_v2/model/field_mapping_query.py
+-rw-r--r--   0        0        0    13087 2023-05-31 20:52:54.790704 rockset_v2_internal-2.0.3/rockset_v2/model/field_mapping_v2.py
+-rw-r--r--   0        0        0    12549 2023-05-31 20:52:54.791297 rockset_v2_internal-2.0.3/rockset_v2/model/field_partition.py
+-rw-r--r--   0        0        0    15029 2023-05-31 20:52:54.791891 rockset_v2_internal-2.0.3/rockset_v2/model/file_upload_collection_creation_request.py
+-rw-r--r--   0        0        0    13623 2023-05-31 20:52:54.792409 rockset_v2_internal-2.0.3/rockset_v2/model/file_upload_source_wrapper.py
+-rw-r--r--   0        0        0    13214 2023-05-31 20:52:54.792957 rockset_v2_internal-2.0.3/rockset_v2/model/format_params.py
+-rw-r--r--   0        0        0    12007 2023-05-31 20:52:54.793500 rockset_v2_internal-2.0.3/rockset_v2/model/gcp_service_account.py
+-rw-r--r--   0        0        0    14958 2023-05-31 20:52:54.794134 rockset_v2_internal-2.0.3/rockset_v2/model/gcs_collection_creation_request.py
+-rw-r--r--   0        0        0    11924 2023-05-31 20:52:54.794888 rockset_v2_internal-2.0.3/rockset_v2/model/gcs_integration.py
+-rw-r--r--   0        0        0    12418 2023-05-31 20:52:54.795809 rockset_v2_internal-2.0.3/rockset_v2/model/gcs_integration_creation_request.py
+-rw-r--r--   0        0        0    14678 2023-05-31 20:52:54.796507 rockset_v2_internal-2.0.3/rockset_v2/model/gcs_source_wrapper.py
+-rw-r--r--   0        0        0    11769 2023-05-31 20:52:54.797210 rockset_v2_internal-2.0.3/rockset_v2/model/get_alias_response.py
+-rw-r--r--   0        0        0    11780 2023-05-31 20:52:54.797823 rockset_v2_internal-2.0.3/rockset_v2/model/get_api_key_response.py
+-rw-r--r--   0        0        0    11819 2023-05-31 20:52:54.798426 rockset_v2_internal-2.0.3/rockset_v2/model/get_collection_response.py
+-rw-r--r--   0        0        0    11829 2023-05-31 20:52:54.799070 rockset_v2_internal-2.0.3/rockset_v2/model/get_integration_response.py
+-rw-r--r--   0        0        0    11798 2023-05-31 20:52:54.799760 rockset_v2_internal-2.0.3/rockset_v2/model/get_query_response.py
+-rw-r--r--   0        0        0    11759 2023-05-31 20:52:54.800502 rockset_v2_internal-2.0.3/rockset_v2/model/get_view_response.py
+-rw-r--r--   0        0        0    11870 2023-05-31 20:52:54.801176 rockset_v2_internal-2.0.3/rockset_v2/model/get_virtual_instance_response.py
+-rw-r--r--   0        0        0    11809 2023-05-31 20:52:54.801799 rockset_v2_internal-2.0.3/rockset_v2/model/get_workspace_response.py
+-rw-r--r--   0        0        0    12710 2023-05-31 20:52:54.802549 rockset_v2_internal-2.0.3/rockset_v2/model/input_field.py
+-rw-r--r--   0        0        0    17401 2023-05-31 20:52:54.803292 rockset_v2_internal-2.0.3/rockset_v2/model/integration.py
+-rw-r--r--   0        0        0    14978 2023-05-31 20:52:54.803958 rockset_v2_internal-2.0.3/rockset_v2/model/kafka_collection_creation_request.py
+-rw-r--r--   0        0        0    14844 2023-05-31 20:52:54.804557 rockset_v2_internal-2.0.3/rockset_v2/model/kafka_integration.py
+-rw-r--r--   0        0        0    12448 2023-05-31 20:52:54.805231 rockset_v2_internal-2.0.3/rockset_v2/model/kafka_integration_creation_request.py
+-rw-r--r--   0        0        0    14039 2023-05-31 20:52:54.806144 rockset_v2_internal-2.0.3/rockset_v2/model/kafka_source_wrapper.py
+-rw-r--r--   0        0        0    11851 2023-05-31 20:52:54.806771 rockset_v2_internal-2.0.3/rockset_v2/model/kafka_v3_security_config.py
+-rw-r--r--   0        0        0    14998 2023-05-31 20:52:54.807438 rockset_v2_internal-2.0.3/rockset_v2/model/kinesis_collection_creation_request.py
+-rw-r--r--   0        0        0    12181 2023-05-31 20:52:54.808157 rockset_v2_internal-2.0.3/rockset_v2/model/kinesis_integration.py
+-rw-r--r--   0        0        0    12478 2023-05-31 20:52:54.808764 rockset_v2_internal-2.0.3/rockset_v2/model/kinesis_integration_creation_request.py
+-rw-r--r--   0        0        0    14277 2023-05-31 20:52:54.809373 rockset_v2_internal-2.0.3/rockset_v2/model/kinesis_source_wrapper.py
+-rw-r--r--   0        0        0    11828 2023-05-31 20:52:54.809989 rockset_v2_internal-2.0.3/rockset_v2/model/list_aliases_response.py
+-rw-r--r--   0        0        0    11844 2023-05-31 20:52:54.810528 rockset_v2_internal-2.0.3/rockset_v2/model/list_api_keys_response.py
+-rw-r--r--   0        0        0    11946 2023-05-31 20:52:54.811273 rockset_v2_internal-2.0.3/rockset_v2/model/list_collection_mounts_response.py
+-rw-r--r--   0        0        0    11883 2023-05-31 20:52:54.811866 rockset_v2_internal-2.0.3/rockset_v2/model/list_collections_response.py
+-rw-r--r--   0        0        0    11901 2023-05-31 20:52:54.812416 rockset_v2_internal-2.0.3/rockset_v2/model/list_integrations_response.py
+-rw-r--r--   0        0        0    11813 2023-05-31 20:52:54.813018 rockset_v2_internal-2.0.3/rockset_v2/model/list_queries_response.py
+-rw-r--r--   0        0        0    11973 2023-05-31 20:52:54.813725 rockset_v2_internal-2.0.3/rockset_v2/model/list_query_lambda_tags_response.py
+-rw-r--r--   0        0        0    12019 2023-05-31 20:52:54.814288 rockset_v2_internal-2.0.3/rockset_v2/model/list_query_lambda_versions_response.py
+-rw-r--r--   0        0        0    11898 2023-05-31 20:52:54.814906 rockset_v2_internal-2.0.3/rockset_v2/model/list_query_lambdas_response.py
+-rw-r--r--   0        0        0    11811 2023-05-31 20:52:54.815485 rockset_v2_internal-2.0.3/rockset_v2/model/list_roles_response.py
+-rw-r--r--   0        0        0    12012 2023-05-31 20:52:54.816034 rockset_v2_internal-2.0.3/rockset_v2/model/list_unsubscribe_preferences_response.py
+-rw-r--r--   0        0        0    11803 2023-05-31 20:52:54.816755 rockset_v2_internal-2.0.3/rockset_v2/model/list_users_response.py
+-rw-r--r--   0        0        0    11811 2023-05-31 20:52:54.817393 rockset_v2_internal-2.0.3/rockset_v2/model/list_views_response.py
+-rw-r--r--   0        0        0    11946 2023-05-31 20:52:54.818009 rockset_v2_internal-2.0.3/rockset_v2/model/list_virtual_instances_response.py
+-rw-r--r--   0        0        0    11863 2023-05-31 20:52:54.818520 rockset_v2_internal-2.0.3/rockset_v2/model/list_workspaces_response.py
+-rw-r--r--   0        0        0    11821 2023-05-31 20:52:54.818957 rockset_v2_internal-2.0.3/rockset_v2/model/mongo_db_integration.py
+-rw-r--r--   0        0        0    14998 2023-05-31 20:52:54.819368 rockset_v2_internal-2.0.3/rockset_v2/model/mongodb_collection_creation_request.py
+-rw-r--r--   0        0        0    12479 2023-05-31 20:52:54.819828 rockset_v2_internal-2.0.3/rockset_v2/model/mongodb_integration_creation_request.py
+-rw-r--r--   0        0        0    14135 2023-05-31 20:52:54.820417 rockset_v2_internal-2.0.3/rockset_v2/model/mongodb_source_wrapper.py
+-rw-r--r--   0        0        0    13286 2023-05-31 20:52:54.821198 rockset_v2_internal-2.0.3/rockset_v2/model/organization.py
+-rw-r--r--   0        0        0    11830 2023-05-31 20:52:54.821707 rockset_v2_internal-2.0.3/rockset_v2/model/organization_response.py
+-rw-r--r--   0        0        0    12536 2023-05-31 20:52:54.822222 rockset_v2_internal-2.0.3/rockset_v2/model/output_field.py
+-rw-r--r--   0        0        0    11781 2023-05-31 20:52:54.822887 rockset_v2_internal-2.0.3/rockset_v2/model/pagination.py
+-rw-r--r--   0        0        0    13061 2023-05-31 20:52:54.823465 rockset_v2_internal-2.0.3/rockset_v2/model/pagination_info.py
+-rw-r--r--   0        0        0    12164 2023-05-31 20:52:54.823998 rockset_v2_internal-2.0.3/rockset_v2/model/patch_document.py
+-rw-r--r--   0        0        0    11929 2023-05-31 20:52:54.824597 rockset_v2_internal-2.0.3/rockset_v2/model/patch_documents_request.py
+-rw-r--r--   0        0        0    11877 2023-05-31 20:52:54.825322 rockset_v2_internal-2.0.3/rockset_v2/model/patch_documents_response.py
+-rw-r--r--   0        0        0    13678 2023-05-31 20:52:54.826018 rockset_v2_internal-2.0.3/rockset_v2/model/patch_operation.py
+-rw-r--r--   0        0        0    15368 2023-05-31 20:52:54.826678 rockset_v2_internal-2.0.3/rockset_v2/model/privilege.py
+-rw-r--r--   0        0        0    12413 2023-05-31 20:52:54.827279 rockset_v2_internal-2.0.3/rockset_v2/model/query_error.py
+-rw-r--r--   0        0        0    11913 2023-05-31 20:52:54.827812 rockset_v2_internal-2.0.3/rockset_v2/model/query_field_type.py
+-rw-r--r--   0        0        0    14987 2023-05-31 20:52:54.828428 rockset_v2_internal-2.0.3/rockset_v2/model/query_info.py
+-rw-r--r--   0        0        0    13697 2023-05-31 20:52:54.829507 rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda.py
+-rw-r--r--   0        0        0    12228 2023-05-31 20:52:54.830135 rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda_sql.py
+-rw-r--r--   0        0        0    12792 2023-05-31 20:52:54.830680 rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda_stats.py
+-rw-r--r--   0        0        0    12133 2023-05-31 20:52:54.831264 rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda_tag.py
+-rw-r--r--   0        0        0    11852 2023-05-31 20:52:54.831771 rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda_tag_response.py
+-rw-r--r--   0        0        0    14853 2023-05-31 20:52:54.832400 rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda_version.py
+-rw-r--r--   0        0        0    11892 2023-05-31 20:52:54.832985 rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda_version_response.py
+-rw-r--r--   0        0        0    12738 2023-05-31 20:52:54.833662 rockset_v2_internal-2.0.3/rockset_v2/model/query_pagination_response.py
+-rw-r--r--   0        0        0    12194 2023-05-31 20:52:54.834352 rockset_v2_internal-2.0.3/rockset_v2/model/query_parameter.py
+-rw-r--r--   0        0        0    12931 2023-05-31 20:52:54.834962 rockset_v2_internal-2.0.3/rockset_v2/model/query_request.py
+-rw-r--r--   0        0        0    13635 2023-05-31 20:52:54.835566 rockset_v2_internal-2.0.3/rockset_v2/model/query_request_sql.py
+-rw-r--r--   0        0        0    15855 2023-05-31 20:52:54.836172 rockset_v2_internal-2.0.3/rockset_v2/model/query_response.py
+-rw-r--r--   0        0        0    12111 2023-05-31 20:52:54.836759 rockset_v2_internal-2.0.3/rockset_v2/model/query_response_stats.py
+-rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.837479 rockset_v2_internal-2.0.3/rockset_v2/model/resume_virtual_instance_response.py
+-rw-r--r--   0        0        0    13372 2023-05-31 20:52:54.837978 rockset_v2_internal-2.0.3/rockset_v2/model/role.py
+-rw-r--r--   0        0        0    11750 2023-05-31 20:52:54.838436 rockset_v2_internal-2.0.3/rockset_v2/model/role_response.py
+-rw-r--r--   0        0        0    14948 2023-05-31 20:52:54.838895 rockset_v2_internal-2.0.3/rockset_v2/model/s3_collection_creation_request.py
+-rw-r--r--   0        0        0    12166 2023-05-31 20:52:54.839359 rockset_v2_internal-2.0.3/rockset_v2/model/s3_integration.py
+-rw-r--r--   0        0        0    12403 2023-05-31 20:52:54.839833 rockset_v2_internal-2.0.3/rockset_v2/model/s3_integration_creation_request.py
+-rw-r--r--   0        0        0    15251 2023-05-31 20:52:54.840241 rockset_v2_internal-2.0.3/rockset_v2/model/s3_source_wrapper.py
+-rw-r--r--   0        0        0    12207 2023-05-31 20:52:54.840748 rockset_v2_internal-2.0.3/rockset_v2/model/schema_registry_config.py
+-rw-r--r--   0        0        0    11696 2023-05-31 20:22:57.768957 rockset_v2_internal-2.0.3/rockset_v2/model/segment_integration.py
+-rw-r--r--   0        0        0    12465 2023-05-31 20:22:57.769388 rockset_v2_internal-2.0.3/rockset_v2/model/segment_integration_creation_request.py
+-rw-r--r--   0        0        0    15018 2023-05-31 20:52:54.841148 rockset_v2_internal-2.0.3/rockset_v2/model/snowflake_collection_creation_request.py
+-rw-r--r--   0        0        0    14462 2023-05-31 20:52:54.841656 rockset_v2_internal-2.0.3/rockset_v2/model/snowflake_integration.py
+-rw-r--r--   0        0        0    12508 2023-05-31 20:52:54.842466 rockset_v2_internal-2.0.3/rockset_v2/model/snowflake_integration_creation_request.py
+-rw-r--r--   0        0        0    13919 2023-05-31 20:52:54.843061 rockset_v2_internal-2.0.3/rockset_v2/model/snowflake_source_wrapper.py
+-rw-r--r--   0        0        0    12513 2023-05-31 20:52:54.843639 rockset_v2_internal-2.0.3/rockset_v2/model/source.py
+-rw-r--r--   0        0        0    13175 2023-05-31 20:52:54.844600 rockset_v2_internal-2.0.3/rockset_v2/model/source_azure_blob_storage.py
+-rw-r--r--   0        0        0    12673 2023-05-31 20:52:54.845250 rockset_v2_internal-2.0.3/rockset_v2/model/source_azure_event_hubs.py
+-rw-r--r--   0        0        0    12561 2023-05-31 20:52:54.845894 rockset_v2_internal-2.0.3/rockset_v2/model/source_azure_service_bus.py
+-rw-r--r--   0        0        0    13636 2023-05-31 20:52:54.846554 rockset_v2_internal-2.0.3/rockset_v2/model/source_dynamo_db.py
+-rw-r--r--   0        0        0    12397 2023-05-31 20:52:54.847182 rockset_v2_internal-2.0.3/rockset_v2/model/source_file_upload.py
+-rw-r--r--   0        0        0    13377 2023-05-31 20:52:54.847838 rockset_v2_internal-2.0.3/rockset_v2/model/source_gcs.py
+-rw-r--r--   0        0        0    13218 2023-05-31 20:52:54.848518 rockset_v2_internal-2.0.3/rockset_v2/model/source_kafka.py
+-rw-r--r--   0        0        0    13030 2023-05-31 20:52:54.849174 rockset_v2_internal-2.0.3/rockset_v2/model/source_kinesis.py
+-rw-r--r--   0        0        0    13324 2023-05-31 20:52:54.849861 rockset_v2_internal-2.0.3/rockset_v2/model/source_mongo_db.py
+-rw-r--r--   0        0        0    13929 2023-05-31 20:52:54.850690 rockset_v2_internal-2.0.3/rockset_v2/model/source_s3.py
+-rw-r--r--   0        0        0    13119 2023-05-31 20:52:54.851312 rockset_v2_internal-2.0.3/rockset_v2/model/source_snowflake.py
+-rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.851690 rockset_v2_internal-2.0.3/rockset_v2/model/source_system.py
+-rw-r--r--   0        0        0    11667 2023-05-31 20:52:54.852404 rockset_v2_internal-2.0.3/rockset_v2/model/sql_expression.py
+-rw-r--r--   0        0        0    13122 2023-05-31 20:52:54.853717 rockset_v2_internal-2.0.3/rockset_v2/model/stats.py
+-rw-r--r--   0        0        0    13664 2023-05-31 20:52:54.854365 rockset_v2_internal-2.0.3/rockset_v2/model/status.py
+-rw-r--r--   0        0        0    13120 2023-05-31 20:52:54.854952 rockset_v2_internal-2.0.3/rockset_v2/model/status_azure_event_hubs.py
+-rw-r--r--   0        0        0    12370 2023-05-31 20:52:54.855801 rockset_v2_internal-2.0.3/rockset_v2/model/status_azure_event_hubs_partition.py
+-rw-r--r--   0        0        0    12736 2023-05-31 20:52:54.856414 rockset_v2_internal-2.0.3/rockset_v2/model/status_azure_service_bus.py
+-rw-r--r--   0        0        0    12216 2023-05-31 20:52:54.857296 rockset_v2_internal-2.0.3/rockset_v2/model/status_azure_service_bus_session.py
+-rw-r--r--   0        0        0    13569 2023-05-31 20:52:54.857991 rockset_v2_internal-2.0.3/rockset_v2/model/status_dynamo_db.py
+-rw-r--r--   0        0        0    12711 2023-05-31 20:52:54.858679 rockset_v2_internal-2.0.3/rockset_v2/model/status_dynamo_db_v2.py
+-rw-r--r--   0        0        0    13132 2023-05-31 20:52:54.859333 rockset_v2_internal-2.0.3/rockset_v2/model/status_kafka.py
+-rw-r--r--   0        0        0    12343 2023-05-31 20:52:54.859863 rockset_v2_internal-2.0.3/rockset_v2/model/status_kafka_partition.py
+-rw-r--r--   0        0        0    15620 2023-05-31 20:52:54.860443 rockset_v2_internal-2.0.3/rockset_v2/model/status_mongo_db.py
+-rw-r--r--   0        0        0    11930 2023-05-31 20:52:54.860923 rockset_v2_internal-2.0.3/rockset_v2/model/status_snowflake.py
+-rw-r--r--   0        0        0    11882 2023-05-31 20:52:54.861396 rockset_v2_internal-2.0.3/rockset_v2/model/suspend_virtual_instance_response.py
+-rw-r--r--   0        0        0    11900 2023-05-31 20:52:54.862111 rockset_v2_internal-2.0.3/rockset_v2/model/unsubscribe_preference.py
+-rw-r--r--   0        0        0    12125 2023-05-31 20:52:54.862684 rockset_v2_internal-2.0.3/rockset_v2/model/update_alias_request.py
+-rw-r--r--   0        0        0    11824 2023-05-31 20:52:54.863145 rockset_v2_internal-2.0.3/rockset_v2/model/update_api_key_request.py
+-rw-r--r--   0        0        0    11789 2023-05-31 20:52:54.863693 rockset_v2_internal-2.0.3/rockset_v2/model/update_api_key_response.py
+-rw-r--r--   0        0        0    12256 2023-05-31 20:52:54.864067 rockset_v2_internal-2.0.3/rockset_v2/model/update_collection_request.py
+-rw-r--r--   0        0        0    11867 2023-05-31 20:22:57.782858 rockset_v2_internal-2.0.3/rockset_v2/model/update_integration_request.py
+-rw-r--r--   0        0        0    11829 2023-05-31 20:22:57.783231 rockset_v2_internal-2.0.3/rockset_v2/model/update_integration_response.py
+-rw-r--r--   0        0        0    12338 2023-05-31 20:52:54.864615 rockset_v2_internal-2.0.3/rockset_v2/model/update_query_lambda_request.py
+-rw-r--r--   0        0        0    12231 2023-05-31 20:52:54.865200 rockset_v2_internal-2.0.3/rockset_v2/model/update_role_request.py
+-rw-r--r--   0        0        0    12015 2023-05-31 20:52:54.865776 rockset_v2_internal-2.0.3/rockset_v2/model/update_unsubscribe_preferences_request.py
+-rw-r--r--   0        0        0    12018 2023-05-31 20:52:54.866368 rockset_v2_internal-2.0.3/rockset_v2/model/update_unsubscribe_preferences_response.py
+-rw-r--r--   0        0        0    12212 2023-05-31 20:52:54.866855 rockset_v2_internal-2.0.3/rockset_v2/model/update_user_request.py
+-rw-r--r--   0        0        0    11964 2023-05-31 20:52:54.867381 rockset_v2_internal-2.0.3/rockset_v2/model/update_view_request.py
+-rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.867851 rockset_v2_internal-2.0.3/rockset_v2/model/update_view_response.py
+-rw-r--r--   0        0        0    15183 2023-05-31 20:52:54.868410 rockset_v2_internal-2.0.3/rockset_v2/model/update_virtual_instance_request.py
+-rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.869001 rockset_v2_internal-2.0.3/rockset_v2/model/update_virtual_instance_response.py
+-rw-r--r--   0        0        0    12913 2023-05-31 20:52:54.869670 rockset_v2_internal-2.0.3/rockset_v2/model/user.py
+-rw-r--r--   0        0        0    12161 2023-05-31 20:52:54.870144 rockset_v2_internal-2.0.3/rockset_v2/model/validate_query_response.py
+-rw-r--r--   0        0        0    14479 2023-05-31 20:52:54.870672 rockset_v2_internal-2.0.3/rockset_v2/model/view.py
+-rw-r--r--   0        0        0    18641 2023-05-31 20:52:54.871271 rockset_v2_internal-2.0.3/rockset_v2/model/virtual_instance.py
+-rw-r--r--   0        0        0    11778 2023-05-31 20:52:54.871892 rockset_v2_internal-2.0.3/rockset_v2/model/virtual_instance_stats.py
+-rw-r--r--   0        0        0    12977 2023-05-31 20:52:54.872539 rockset_v2_internal-2.0.3/rockset_v2/model/workspace.py
+-rw-r--r--   0        0        0    13004 2023-05-31 20:52:54.873194 rockset_v2_internal-2.0.3/rockset_v2/model/xml_params.py
+-rw-r--r--   0        0        0    84040 2023-05-31 20:52:54.874454 rockset_v2_internal-2.0.3/rockset_v2/model_utils.py
+-rw-r--r--   0        0        0    15316 2023-05-31 20:52:54.875183 rockset_v2_internal-2.0.3/rockset_v2/models/__init__.py
+-rw-r--r--   0        0        0     1829 2023-05-31 20:56:40.127308 rockset_v2_internal-2.0.3/rockset_v2/query_paginator.py
+-rw-r--r--   0        0        0    14648 2023-05-31 20:52:54.875917 rockset_v2_internal-2.0.3/rockset_v2/rest.py
+-rw-r--r--   0        0        0     8926 2023-05-31 20:52:54.876525 rockset_v2_internal-2.0.3/rockset_v2/rockset_client.py
+-rw-r--r--   0        0        0     3644 2023-05-31 20:22:57.826319 rockset_v2_internal-2.0.3/rockset_v2/value.py
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 rockset_v2_internal-2.0.3/PKG-INFO
```

### Comparing `rockset_v2_internal-2.0.2/pyproject.toml` & `rockset_v2_internal-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-name = "rockset_v2_internal"
-version = "2.0.2"
+name = "rockset-v2-internal"
+version = "2.0.3"
 description = "The python client for the Rockset API."
 authors = ["Rockset <support@rockset.com>"]
 packages = [
     {include = "rockset_v2"}
 ]
 documentation = "https://github.com/rockset/rockset-python-client"
 repository = "https://github.com/rockset/rockset-python-client"
```

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/__init__.py` & `rockset_v2_internal-2.0.3/rockset_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/aliases_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/aliases_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/api_keys_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/api_keys_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/collections_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/collections_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/custom_roles_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/custom_roles_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/documents_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/documents_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/integrations_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/integrations_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/organizations_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/queries_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/queries_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/query_lambdas_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/query_lambdas_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/shared_lambdas_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/shared_lambdas_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/users_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/users_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/views_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/views_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/virtual_instances_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/virtual_instances_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api/workspaces_api.py` & `rockset_v2_internal-2.0.3/rockset_v2/api/workspaces_api.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/api_client.py` & `rockset_v2_internal-2.0.3/rockset_v2/api_client.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/apis/__init__.py` & `rockset_v2_internal-2.0.3/rockset_v2/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/configuration.py` & `rockset_v2_internal-2.0.3/rockset_v2/configuration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/document.py` & `rockset_v2_internal-2.0.3/rockset_v2/document.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/exceptions.py` & `rockset_v2_internal-2.0.3/rockset_v2/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/add_documents_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/add_documents_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/add_documents_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/add_documents_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/alias.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/alias.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/api_key.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/api_key.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/async_query_options.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/async_query_options.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/auto_scaling_policy.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/auto_scaling_policy.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/aws_access_key.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/aws_access_key.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/aws_role.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/aws_role.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_collection_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/azure_blob_storage_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_integration.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/azure_blob_storage_integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_integration_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/azure_blob_storage_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_source_wrapper.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/azure_blob_storage_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_collection_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/azure_event_hubs_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_integration.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/azure_event_hubs_integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_integration_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/azure_event_hubs_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_source_wrapper.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/azure_event_hubs_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/azure_service_bus_collection_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/azure_service_bus_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/azure_service_bus_integration.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/azure_service_bus_integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/azure_service_bus_source_wrapper.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/azure_service_bus_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/bulk_stats.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/bulk_stats.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/cancel_query_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/cancel_query_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/cluster.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/cluster.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/collection.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/collection.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/collection_mount.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/collection_mount.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/collection_mount_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/collection_mount_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/collection_mount_stats.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/collection_mount_stats.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/collection_stats.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/collection_stats.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_alias_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_alias_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_alias_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_alias_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_api_key_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_api_key_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_api_key_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_mount_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_collection_mount_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_mounts_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_collection_mounts_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_collection_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_integration_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_integration_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_query_lambda_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_query_lambda_tag_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_query_lambda_tag_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_role_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_role_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_user_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_user_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_user_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_user_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_view_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_view_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_view_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_virtual_instance_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_virtual_instance_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_virtual_instance_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_workspace_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/create_workspace_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/csv_params.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/csv_params.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/delete_alias_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/delete_alias_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/delete_api_key_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/delete_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/delete_collection_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/delete_collection_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/delete_documents_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/delete_documents_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/delete_documents_request_data.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/delete_documents_request_data.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/delete_documents_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/delete_documents_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/delete_integration_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/delete_query_lambda_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/delete_query_lambda_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/delete_user_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/delete_user_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/delete_view_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/delete_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/delete_virtual_instance_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/delete_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/delete_workspace_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/delete_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/document_status.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/document_status.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_collection_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/dynamodb_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_integration.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/dynamodb_integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_integration_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/dynamodb_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_source_wrapper.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/dynamodb_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/error_model.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/error_model.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/event_time_info.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/event_time_info.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/execute_public_query_lambda_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/execute_public_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/execute_query_lambda_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/execute_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/field_mapping_query.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/field_mapping_query.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/field_mapping_v2.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/field_mapping_v2.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/field_partition.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/field_partition.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/file_upload_collection_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/file_upload_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/file_upload_source_wrapper.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/file_upload_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/format_params.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/format_params.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/gcp_service_account.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/gcp_service_account.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/gcs_collection_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/gcs_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/gcs_integration.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/gcs_integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/gcs_integration_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/gcs_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/gcs_source_wrapper.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/gcs_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/get_alias_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/get_alias_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/get_api_key_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/get_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/get_collection_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/get_collection_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/get_integration_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/get_query_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/get_query_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/get_view_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/get_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/get_virtual_instance_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/get_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/get_workspace_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/input_field.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/input_field.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/integration.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/kafka_collection_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/kafka_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/kafka_integration.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/kafka_integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/kafka_integration_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/kafka_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/kafka_source_wrapper.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/kafka_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/kafka_v3_security_config.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/kafka_v3_security_config.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_collection_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/kinesis_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_integration.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/kinesis_integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_integration_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/kinesis_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_source_wrapper.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/kinesis_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_aliases_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_aliases_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_api_keys_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_collection_mounts_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_collection_mounts_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_collections_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_collections_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_integrations_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_queries_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_queries_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_query_lambda_tags_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_query_lambda_tags_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_query_lambda_versions_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_query_lambda_versions_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_query_lambdas_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_query_lambdas_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_roles_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_roles_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_unsubscribe_preferences_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_unsubscribe_preferences_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_users_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_users_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_views_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_views_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_virtual_instances_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_virtual_instances_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/list_workspaces_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/mongo_db_integration.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/mongo_db_integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/mongodb_collection_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/mongodb_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/mongodb_integration_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/mongodb_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/mongodb_source_wrapper.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/mongodb_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/organization.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/organization.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/organization_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/organization_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/output_field.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/output_field.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/pagination.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/pagination.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/pagination_info.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/pagination_info.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/patch_document.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/patch_document.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/patch_documents_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/patch_documents_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/patch_documents_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/patch_documents_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/patch_operation.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/patch_operation.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/privilege.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/privilege.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_error.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_error.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_field_type.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_field_type.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_info.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_info.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_sql.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda_sql.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_stats.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda_stats.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_tag.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda_tag.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_tag_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda_tag_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_version.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda_version.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_version_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_lambda_version_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_pagination_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_pagination_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_parameter.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_parameter.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_request_sql.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_request_sql.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/query_response_stats.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/query_response_stats.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/resume_virtual_instance_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/resume_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/role.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/role.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/role_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/role_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/s3_collection_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/s3_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/s3_integration.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/s3_integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/s3_integration_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/s3_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/s3_source_wrapper.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/s3_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/schema_registry_config.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/schema_registry_config.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/segment_integration.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/segment_integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/segment_integration_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/segment_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_collection_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/snowflake_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_integration.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/snowflake_integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_integration_creation_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/snowflake_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_source_wrapper.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/snowflake_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source_azure_blob_storage.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source_azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source_azure_event_hubs.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source_azure_event_hubs.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source_azure_service_bus.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source_azure_service_bus.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source_dynamo_db.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source_dynamo_db.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source_file_upload.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source_file_upload.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source_gcs.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source_gcs.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source_kafka.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source_kafka.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source_kinesis.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source_kinesis.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source_mongo_db.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source_mongo_db.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source_s3.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source_s3.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source_snowflake.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source_snowflake.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/source_system.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/source_system.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/sql_expression.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/sql_expression.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/stats.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/stats.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/status.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/status.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_event_hubs.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/status_azure_event_hubs.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_event_hubs_partition.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/status_azure_event_hubs_partition.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_service_bus.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/status_azure_service_bus.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_service_bus_session.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/status_azure_service_bus_session.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/status_dynamo_db.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/status_dynamo_db.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/status_dynamo_db_v2.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/status_dynamo_db_v2.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/status_kafka.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/status_kafka.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/status_kafka_partition.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/status_kafka_partition.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/status_mongo_db.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/status_mongo_db.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/status_snowflake.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/status_snowflake.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/suspend_virtual_instance_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/suspend_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/unsubscribe_preference.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/unsubscribe_preference.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_alias_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_alias_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_api_key_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_api_key_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_api_key_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_collection_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_collection_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_integration_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_integration_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_integration_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_query_lambda_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_role_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_role_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_unsubscribe_preferences_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_unsubscribe_preferences_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_unsubscribe_preferences_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_unsubscribe_preferences_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_user_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_user_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_view_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_view_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_view_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_virtual_instance_request.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_virtual_instance_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/update_virtual_instance_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/update_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/user.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/user.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/validate_query_response.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/validate_query_response.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/view.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/view.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/virtual_instance.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/virtual_instance.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/virtual_instance_stats.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/virtual_instance_stats.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/workspace.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/workspace.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model/xml_params.py` & `rockset_v2_internal-2.0.3/rockset_v2/model/xml_params.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/model_utils.py` & `rockset_v2_internal-2.0.3/rockset_v2/model_utils.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/models/__init__.py` & `rockset_v2_internal-2.0.3/rockset_v2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/query_paginator.py` & `rockset_v2_internal-2.0.3/rockset_v2/query_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from rockset import RocksetClient
-from rockset.exceptions import RocksetException
-from rockset.models import QueryResponse
+from rockset_v2 import RocksetClient
+from rockset_v2.exceptions import RocksetException
+from rockset_v2.models import QueryResponse
 
 
 class QueryPaginator:
     def __init__(self, client: RocksetClient, query_response: QueryResponse):
         self._client = client
         if hasattr(query_response, "query_errors") and query_response.query_errors:
             raise RocksetException(f"Provided query has errors: {query_response.query_errors}")
@@ -40,8 +40,8 @@
         return current_results
         
     def current_results(self):
         return self._current_results
 
     def initial_query_response(self):
         return self._query_response
-        
+
```

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/rest.py` & `rockset_v2_internal-2.0.3/rockset_v2/rest.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/rockset_client.py` & `rockset_v2_internal-2.0.3/rockset_v2/rockset_client.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/rockset_v2/value.py` & `rockset_v2_internal-2.0.3/rockset_v2/value.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.2/PKG-INFO` & `rockset_v2_internal-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockset-v2-internal
-Version: 2.0.2
+Version: 2.0.3
 Summary: The python client for the Rockset API.
 Home-page: https://github.com/rockset/rockset-python-client
 License: Apache-2.0
 Author: Rockset
 Author-email: support@rockset.com
 Requires-Python: >=3.6,<4.0
 Classifier: Environment :: Console
```

