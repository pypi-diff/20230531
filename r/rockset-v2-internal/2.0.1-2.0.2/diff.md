# Comparing `tmp/rockset_v2_internal-2.0.1.tar.gz` & `tmp/rockset_v2_internal-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockset_v2_internal-2.0.1.tar", max compression
+gzip compressed data, was "rockset_v2_internal-2.0.2.tar", max compression
```

## Comparing `rockset_v2_internal-2.0.1.tar` & `rockset_v2_internal-2.0.2.tar`

### file list

```diff
@@ -1,237 +1,240 @@
--rw-r--r--   0        0        0      357 2023-05-31 19:49:16.995381 rockset_v2_internal-2.0.1/LONG_DESCRIPTION.rst
--rw-r--r--   0        0        0     1631 2023-05-31 20:24:40.629520 rockset_v2_internal-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1338 2023-05-31 20:22:57.709055 rockset_v2_internal-2.0.1/rockset_v2/__init__.py
--rw-r--r--   0        0        0      208 2023-05-31 20:22:57.709444 rockset_v2_internal-2.0.1/rockset_v2/api/__init__.py
--rw-r--r--   0        0        0    34696 2023-05-31 20:22:57.709948 rockset_v2_internal-2.0.1/rockset_v2/api/aliases_api.py
--rw-r--r--   0        0        0    29724 2023-05-31 20:22:57.710296 rockset_v2_internal-2.0.1/rockset_v2/api/api_keys_api.py
--rw-r--r--   0        0        0   130795 2023-05-31 20:22:57.711327 rockset_v2_internal-2.0.1/rockset_v2/api/collections_api.py
--rw-r--r--   0        0        0    28165 2023-05-31 20:22:57.711817 rockset_v2_internal-2.0.1/rockset_v2/api/custom_roles_api.py
--rw-r--r--   0        0        0    21187 2023-05-31 20:22:57.712146 rockset_v2_internal-2.0.1/rockset_v2/api/documents_api.py
--rw-r--r--   0        0        0    73682 2023-05-31 20:22:57.712744 rockset_v2_internal-2.0.1/rockset_v2/api/integrations_api.py
--rw-r--r--   0        0        0     6168 2023-05-31 20:22:57.713144 rockset_v2_internal-2.0.1/rockset_v2/api/organizations_api.py
--rw-r--r--   0        0        0    34734 2023-05-31 20:22:57.713475 rockset_v2_internal-2.0.1/rockset_v2/api/queries_api.py
--rw-r--r--   0        0        0    87549 2023-05-31 20:22:57.714100 rockset_v2_internal-2.0.1/rockset_v2/api/query_lambdas_api.py
--rw-r--r--   0        0        0     7727 2023-05-31 20:22:57.714355 rockset_v2_internal-2.0.1/rockset_v2/api/shared_lambdas_api.py
--rw-r--r--   0        0        0    43268 2023-05-31 20:22:57.714691 rockset_v2_internal-2.0.1/rockset_v2/api/users_api.py
--rw-r--r--   0        0        0    34441 2023-05-31 20:22:57.715101 rockset_v2_internal-2.0.1/rockset_v2/api/views_api.py
--rw-r--r--   0        0        0    76220 2023-05-31 20:22:57.715597 rockset_v2_internal-2.0.1/rockset_v2/api/virtual_instances_api.py
--rw-r--r--   0        0        0    22087 2023-05-31 20:22:57.715908 rockset_v2_internal-2.0.1/rockset_v2/api/workspaces_api.py
--rw-r--r--   0        0        0    36245 2023-05-31 20:22:57.716428 rockset_v2_internal-2.0.1/rockset_v2/api_client.py
--rw-r--r--   0        0        0     1112 2023-05-31 20:22:57.716854 rockset_v2_internal-2.0.1/rockset_v2/apis/__init__.py
--rw-r--r--   0        0        0    15516 2023-05-31 20:22:57.717158 rockset_v2_internal-2.0.1/rockset_v2/configuration.py
--rw-r--r--   0        0        0     3831 2023-05-31 20:22:57.717401 rockset_v2_internal-2.0.1/rockset_v2/document.py
--rw-r--r--   0        0        0     6072 2023-05-31 20:22:57.717639 rockset_v2_internal-2.0.1/rockset_v2/exceptions.py
--rw-r--r--   0        0        0      348 2023-05-31 20:22:57.717962 rockset_v2_internal-2.0.1/rockset_v2/model/__init__.py
--rw-r--r--   0        0        0    11950 2023-05-31 20:22:57.718253 rockset_v2_internal-2.0.1/rockset_v2/model/add_documents_request.py
--rw-r--r--   0        0        0    11922 2023-05-31 20:22:57.718468 rockset_v2_internal-2.0.1/rockset_v2/model/add_documents_response.py
--rw-r--r--   0        0        0    13623 2023-05-31 20:22:57.718891 rockset_v2_internal-2.0.1/rockset_v2/model/alias.py
--rw-r--r--   0        0        0    13945 2023-05-31 20:22:57.719138 rockset_v2_internal-2.0.1/rockset_v2/model/api_key.py
--rw-r--r--   0        0        0    13542 2023-05-31 20:22:57.719417 rockset_v2_internal-2.0.1/rockset_v2/model/async_query_options.py
--rw-r--r--   0        0        0    12229 2023-05-31 20:22:57.719623 rockset_v2_internal-2.0.1/rockset_v2/model/aws_access_key.py
--rw-r--r--   0        0        0    12101 2023-05-31 20:22:57.719846 rockset_v2_internal-2.0.1/rockset_v2/model/aws_role.py
--rw-r--r--   0        0        0    15124 2023-05-31 20:22:57.720098 rockset_v2_internal-2.0.1/rockset_v2/model/azure_blob_storage_collection_creation_request.py
--rw-r--r--   0        0        0    11893 2023-05-31 20:22:57.720330 rockset_v2_internal-2.0.1/rockset_v2/model/azure_blob_storage_integration.py
--rw-r--r--   0        0        0    12616 2023-05-31 20:22:57.720549 rockset_v2_internal-2.0.1/rockset_v2/model/azure_blob_storage_integration_creation_request.py
--rw-r--r--   0        0        0    14449 2023-05-31 20:22:57.720795 rockset_v2_internal-2.0.1/rockset_v2/model/azure_blob_storage_source_wrapper.py
--rw-r--r--   0        0        0    15104 2023-05-31 20:22:57.721090 rockset_v2_internal-2.0.1/rockset_v2/model/azure_event_hubs_collection_creation_request.py
--rw-r--r--   0        0        0    11787 2023-05-31 20:22:57.721410 rockset_v2_internal-2.0.1/rockset_v2/model/azure_event_hubs_integration.py
--rw-r--r--   0        0        0    12586 2023-05-31 20:22:57.721778 rockset_v2_internal-2.0.1/rockset_v2/model/azure_event_hubs_integration_creation_request.py
--rw-r--r--   0        0        0    13452 2023-05-31 20:22:57.722083 rockset_v2_internal-2.0.1/rockset_v2/model/azure_event_hubs_source_wrapper.py
--rw-r--r--   0        0        0    15114 2023-05-31 20:22:57.722382 rockset_v2_internal-2.0.1/rockset_v2/model/azure_service_bus_collection_creation_request.py
--rw-r--r--   0        0        0    11888 2023-05-31 20:22:57.722614 rockset_v2_internal-2.0.1/rockset_v2/model/azure_service_bus_integration.py
--rw-r--r--   0        0        0    13333 2023-05-31 20:22:57.722841 rockset_v2_internal-2.0.1/rockset_v2/model/azure_service_bus_source_wrapper.py
--rw-r--r--   0        0        0    18743 2023-05-31 20:22:57.723105 rockset_v2_internal-2.0.1/rockset_v2/model/bulk_stats.py
--rw-r--r--   0        0        0    11798 2023-05-31 20:22:57.723407 rockset_v2_internal-2.0.1/rockset_v2/model/cancel_query_response.py
--rw-r--r--   0        0        0    13225 2023-05-31 20:22:57.723664 rockset_v2_internal-2.0.1/rockset_v2/model/cluster.py
--rw-r--r--   0        0        0    17684 2023-05-31 20:22:57.723984 rockset_v2_internal-2.0.1/rockset_v2/model/collection.py
--rw-r--r--   0        0        0    14579 2023-05-31 20:22:57.724298 rockset_v2_internal-2.0.1/rockset_v2/model/collection_mount.py
--rw-r--r--   0        0        0    11852 2023-05-31 20:22:57.724521 rockset_v2_internal-2.0.1/rockset_v2/model/collection_mount_response.py
--rw-r--r--   0        0        0    11772 2023-05-31 20:22:57.724703 rockset_v2_internal-2.0.1/rockset_v2/model/collection_mount_stats.py
--rw-r--r--   0        0        0    16965 2023-05-31 20:22:57.724929 rockset_v2_internal-2.0.1/rockset_v2/model/collection_stats.py
--rw-r--r--   0        0        0    12333 2023-05-31 20:22:57.725139 rockset_v2_internal-2.0.1/rockset_v2/model/create_alias_request.py
--rw-r--r--   0        0        0    11769 2023-05-31 20:22:57.725325 rockset_v2_internal-2.0.1/rockset_v2/model/create_alias_response.py
--rw-r--r--   0        0        0    12098 2023-05-31 20:22:57.725564 rockset_v2_internal-2.0.1/rockset_v2/model/create_api_key_request.py
--rw-r--r--   0        0        0    11780 2023-05-31 20:22:57.725835 rockset_v2_internal-2.0.1/rockset_v2/model/create_api_key_response.py
--rw-r--r--   0        0        0    12071 2023-05-31 20:22:57.726120 rockset_v2_internal-2.0.1/rockset_v2/model/create_collection_mount_request.py
--rw-r--r--   0        0        0    11913 2023-05-31 20:22:57.726491 rockset_v2_internal-2.0.1/rockset_v2/model/create_collection_mounts_response.py
--rw-r--r--   0        0        0    14506 2023-05-31 20:22:57.726860 rockset_v2_internal-2.0.1/rockset_v2/model/create_collection_request.py
--rw-r--r--   0        0        0    11819 2023-05-31 20:22:57.727114 rockset_v2_internal-2.0.1/rockset_v2/model/create_collection_response.py
--rw-r--r--   0        0        0    16037 2023-05-31 20:22:57.727371 rockset_v2_internal-2.0.1/rockset_v2/model/create_integration_request.py
--rw-r--r--   0        0        0    11829 2023-05-31 20:22:57.727619 rockset_v2_internal-2.0.1/rockset_v2/model/create_integration_response.py
--rw-r--r--   0        0        0    12571 2023-05-31 20:22:57.727836 rockset_v2_internal-2.0.1/rockset_v2/model/create_query_lambda_request.py
--rw-r--r--   0        0        0    12063 2023-05-31 20:22:57.728059 rockset_v2_internal-2.0.1/rockset_v2/model/create_query_lambda_tag_request.py
--rw-r--r--   0        0        0    12501 2023-05-31 20:22:57.728335 rockset_v2_internal-2.0.1/rockset_v2/model/create_role_request.py
--rw-r--r--   0        0        0    12479 2023-05-31 20:22:57.728556 rockset_v2_internal-2.0.1/rockset_v2/model/create_user_request.py
--rw-r--r--   0        0        0    11759 2023-05-31 20:22:57.728863 rockset_v2_internal-2.0.1/rockset_v2/model/create_user_response.py
--rw-r--r--   0        0        0    12170 2023-05-31 20:22:57.729131 rockset_v2_internal-2.0.1/rockset_v2/model/create_view_request.py
--rw-r--r--   0        0        0    11759 2023-05-31 20:22:57.729491 rockset_v2_internal-2.0.1/rockset_v2/model/create_view_response.py
--rw-r--r--   0        0        0    13224 2023-05-31 20:22:57.729886 rockset_v2_internal-2.0.1/rockset_v2/model/create_virtual_instance_request.py
--rw-r--r--   0        0        0    11870 2023-05-31 20:22:57.730329 rockset_v2_internal-2.0.1/rockset_v2/model/create_virtual_instance_response.py
--rw-r--r--   0        0        0    12038 2023-05-31 20:22:57.730720 rockset_v2_internal-2.0.1/rockset_v2/model/create_workspace_request.py
--rw-r--r--   0        0        0    11809 2023-05-31 20:22:57.731082 rockset_v2_internal-2.0.1/rockset_v2/model/create_workspace_response.py
--rw-r--r--   0        0        0    14179 2023-05-31 20:22:57.731464 rockset_v2_internal-2.0.1/rockset_v2/model/csv_params.py
--rw-r--r--   0        0        0    11769 2023-05-31 20:22:57.731835 rockset_v2_internal-2.0.1/rockset_v2/model/delete_alias_response.py
--rw-r--r--   0        0        0    11780 2023-05-31 20:22:57.732321 rockset_v2_internal-2.0.1/rockset_v2/model/delete_api_key_response.py
--rw-r--r--   0        0        0    11819 2023-05-31 20:22:57.732690 rockset_v2_internal-2.0.1/rockset_v2/model/delete_collection_response.py
--rw-r--r--   0        0        0    12036 2023-05-31 20:22:57.733051 rockset_v2_internal-2.0.1/rockset_v2/model/delete_documents_request.py
--rw-r--r--   0        0        0    11686 2023-05-31 20:22:57.733460 rockset_v2_internal-2.0.1/rockset_v2/model/delete_documents_request_data.py
--rw-r--r--   0        0        0    11927 2023-05-31 20:22:57.733796 rockset_v2_internal-2.0.1/rockset_v2/model/delete_documents_response.py
--rw-r--r--   0        0        0    11829 2023-05-31 20:22:57.734133 rockset_v2_internal-2.0.1/rockset_v2/model/delete_integration_response.py
--rw-r--r--   0        0        0    11830 2023-05-31 20:22:57.734448 rockset_v2_internal-2.0.1/rockset_v2/model/delete_query_lambda_response.py
--rw-r--r--   0        0        0    11759 2023-05-31 20:22:57.734763 rockset_v2_internal-2.0.1/rockset_v2/model/delete_user_response.py
--rw-r--r--   0        0        0    11759 2023-05-31 20:22:57.735128 rockset_v2_internal-2.0.1/rockset_v2/model/delete_view_response.py
--rw-r--r--   0        0        0    11870 2023-05-31 20:22:57.735524 rockset_v2_internal-2.0.1/rockset_v2/model/delete_virtual_instance_response.py
--rw-r--r--   0        0        0    11809 2023-05-31 20:22:57.735906 rockset_v2_internal-2.0.1/rockset_v2/model/delete_workspace_response.py
--rw-r--r--   0        0        0    13023 2023-05-31 20:22:57.736295 rockset_v2_internal-2.0.1/rockset_v2/model/document_status.py
--rw-r--r--   0        0        0    15042 2023-05-31 20:22:57.736613 rockset_v2_internal-2.0.1/rockset_v2/model/dynamodb_collection_creation_request.py
--rw-r--r--   0        0        0    12563 2023-05-31 20:22:57.736920 rockset_v2_internal-2.0.1/rockset_v2/model/dynamodb_integration.py
--rw-r--r--   0        0        0    12484 2023-05-31 20:22:57.737195 rockset_v2_internal-2.0.1/rockset_v2/model/dynamodb_integration_creation_request.py
--rw-r--r--   0        0        0    14440 2023-05-31 20:22:57.737463 rockset_v2_internal-2.0.1/rockset_v2/model/dynamodb_source_wrapper.py
--rw-r--r--   0        0        0    14520 2023-05-31 20:22:57.737757 rockset_v2_internal-2.0.1/rockset_v2/model/error_model.py
--rw-r--r--   0        0        0    12392 2023-05-31 20:22:57.738020 rockset_v2_internal-2.0.1/rockset_v2/model/event_time_info.py
--rw-r--r--   0        0        0    12656 2023-05-31 20:22:57.738323 rockset_v2_internal-2.0.1/rockset_v2/model/execute_public_query_lambda_request.py
--rw-r--r--   0        0        0    14367 2023-05-31 20:22:57.738691 rockset_v2_internal-2.0.1/rockset_v2/model/execute_query_lambda_request.py
--rw-r--r--   0        0        0    11743 2023-05-31 20:22:57.739033 rockset_v2_internal-2.0.1/rockset_v2/model/field_mapping_query.py
--rw-r--r--   0        0        0    13075 2023-05-31 20:22:57.739434 rockset_v2_internal-2.0.1/rockset_v2/model/field_mapping_v2.py
--rw-r--r--   0        0        0    12543 2023-05-31 20:22:57.739790 rockset_v2_internal-2.0.1/rockset_v2/model/field_partition.py
--rw-r--r--   0        0        0    15063 2023-05-31 20:22:57.740099 rockset_v2_internal-2.0.1/rockset_v2/model/file_upload_collection_creation_request.py
--rw-r--r--   0        0        0    13611 2023-05-31 20:22:57.740405 rockset_v2_internal-2.0.1/rockset_v2/model/file_upload_source_wrapper.py
--rw-r--r--   0        0        0    13202 2023-05-31 20:22:57.740737 rockset_v2_internal-2.0.1/rockset_v2/model/format_params.py
--rw-r--r--   0        0        0    12001 2023-05-31 20:22:57.740994 rockset_v2_internal-2.0.1/rockset_v2/model/gcp_service_account.py
--rw-r--r--   0        0        0    14992 2023-05-31 20:22:57.741253 rockset_v2_internal-2.0.1/rockset_v2/model/gcs_collection_creation_request.py
--rw-r--r--   0        0        0    11915 2023-05-31 20:22:57.741556 rockset_v2_internal-2.0.1/rockset_v2/model/gcs_integration.py
--rw-r--r--   0        0        0    12409 2023-05-31 20:22:57.741893 rockset_v2_internal-2.0.1/rockset_v2/model/gcs_integration_creation_request.py
--rw-r--r--   0        0        0    14666 2023-05-31 20:22:57.742242 rockset_v2_internal-2.0.1/rockset_v2/model/gcs_source_wrapper.py
--rw-r--r--   0        0        0    11760 2023-05-31 20:22:57.742503 rockset_v2_internal-2.0.1/rockset_v2/model/get_alias_response.py
--rw-r--r--   0        0        0    11771 2023-05-31 20:22:57.742762 rockset_v2_internal-2.0.1/rockset_v2/model/get_api_key_response.py
--rw-r--r--   0        0        0    11810 2023-05-31 20:22:57.743027 rockset_v2_internal-2.0.1/rockset_v2/model/get_collection_response.py
--rw-r--r--   0        0        0    11820 2023-05-31 20:22:57.743268 rockset_v2_internal-2.0.1/rockset_v2/model/get_integration_response.py
--rw-r--r--   0        0        0    11789 2023-05-31 20:22:57.743487 rockset_v2_internal-2.0.1/rockset_v2/model/get_query_response.py
--rw-r--r--   0        0        0    11750 2023-05-31 20:22:57.743738 rockset_v2_internal-2.0.1/rockset_v2/model/get_view_response.py
--rw-r--r--   0        0        0    11861 2023-05-31 20:22:57.743983 rockset_v2_internal-2.0.1/rockset_v2/model/get_virtual_instance_response.py
--rw-r--r--   0        0        0    11800 2023-05-31 20:22:57.744244 rockset_v2_internal-2.0.1/rockset_v2/model/get_workspace_response.py
--rw-r--r--   0        0        0    12704 2023-05-31 20:22:57.744673 rockset_v2_internal-2.0.1/rockset_v2/model/input_field.py
--rw-r--r--   0        0        0    17362 2023-05-31 20:22:57.745097 rockset_v2_internal-2.0.1/rockset_v2/model/integration.py
--rw-r--r--   0        0        0    15012 2023-05-31 20:22:57.745511 rockset_v2_internal-2.0.1/rockset_v2/model/kafka_collection_creation_request.py
--rw-r--r--   0        0        0    14826 2023-05-31 20:22:57.745878 rockset_v2_internal-2.0.1/rockset_v2/model/kafka_integration.py
--rw-r--r--   0        0        0    12439 2023-05-31 20:22:57.746236 rockset_v2_internal-2.0.1/rockset_v2/model/kafka_integration_creation_request.py
--rw-r--r--   0        0        0    14027 2023-05-31 20:22:57.746573 rockset_v2_internal-2.0.1/rockset_v2/model/kafka_source_wrapper.py
--rw-r--r--   0        0        0    11845 2023-05-31 20:22:57.746991 rockset_v2_internal-2.0.1/rockset_v2/model/kafka_v3_security_config.py
--rw-r--r--   0        0        0    15032 2023-05-31 20:22:57.747264 rockset_v2_internal-2.0.1/rockset_v2/model/kinesis_collection_creation_request.py
--rw-r--r--   0        0        0    12169 2023-05-31 20:22:57.747530 rockset_v2_internal-2.0.1/rockset_v2/model/kinesis_integration.py
--rw-r--r--   0        0        0    12469 2023-05-31 20:22:57.747806 rockset_v2_internal-2.0.1/rockset_v2/model/kinesis_integration_creation_request.py
--rw-r--r--   0        0        0    14265 2023-05-31 20:22:57.748126 rockset_v2_internal-2.0.1/rockset_v2/model/kinesis_source_wrapper.py
--rw-r--r--   0        0        0    11819 2023-05-31 20:22:57.748440 rockset_v2_internal-2.0.1/rockset_v2/model/list_aliases_response.py
--rw-r--r--   0        0        0    11835 2023-05-31 20:22:57.748834 rockset_v2_internal-2.0.1/rockset_v2/model/list_api_keys_response.py
--rw-r--r--   0        0        0    11937 2023-05-31 20:22:57.749077 rockset_v2_internal-2.0.1/rockset_v2/model/list_collection_mounts_response.py
--rw-r--r--   0        0        0    11874 2023-05-31 20:22:57.749297 rockset_v2_internal-2.0.1/rockset_v2/model/list_collections_response.py
--rw-r--r--   0        0        0    11892 2023-05-31 20:22:57.749520 rockset_v2_internal-2.0.1/rockset_v2/model/list_integrations_response.py
--rw-r--r--   0        0        0    11804 2023-05-31 20:22:57.749749 rockset_v2_internal-2.0.1/rockset_v2/model/list_queries_response.py
--rw-r--r--   0        0        0    11964 2023-05-31 20:22:57.750026 rockset_v2_internal-2.0.1/rockset_v2/model/list_query_lambda_tags_response.py
--rw-r--r--   0        0        0    12010 2023-05-31 20:22:57.750366 rockset_v2_internal-2.0.1/rockset_v2/model/list_query_lambda_versions_response.py
--rw-r--r--   0        0        0    11889 2023-05-31 20:22:57.750673 rockset_v2_internal-2.0.1/rockset_v2/model/list_query_lambdas_response.py
--rw-r--r--   0        0        0    11802 2023-05-31 20:22:57.751031 rockset_v2_internal-2.0.1/rockset_v2/model/list_roles_response.py
--rw-r--r--   0        0        0    12003 2023-05-31 20:22:57.751492 rockset_v2_internal-2.0.1/rockset_v2/model/list_unsubscribe_preferences_response.py
--rw-r--r--   0        0        0    11794 2023-05-31 20:22:57.751805 rockset_v2_internal-2.0.1/rockset_v2/model/list_users_response.py
--rw-r--r--   0        0        0    11802 2023-05-31 20:22:57.752112 rockset_v2_internal-2.0.1/rockset_v2/model/list_views_response.py
--rw-r--r--   0        0        0    11937 2023-05-31 20:22:57.752390 rockset_v2_internal-2.0.1/rockset_v2/model/list_virtual_instances_response.py
--rw-r--r--   0        0        0    11854 2023-05-31 20:22:57.752633 rockset_v2_internal-2.0.1/rockset_v2/model/list_workspaces_response.py
--rw-r--r--   0        0        0    11815 2023-05-31 20:22:57.752937 rockset_v2_internal-2.0.1/rockset_v2/model/mongo_db_integration.py
--rw-r--r--   0        0        0    15032 2023-05-31 20:22:57.753250 rockset_v2_internal-2.0.1/rockset_v2/model/mongodb_collection_creation_request.py
--rw-r--r--   0        0        0    12470 2023-05-31 20:22:57.753588 rockset_v2_internal-2.0.1/rockset_v2/model/mongodb_integration_creation_request.py
--rw-r--r--   0        0        0    13434 2023-05-31 20:22:57.753937 rockset_v2_internal-2.0.1/rockset_v2/model/mongodb_source_wrapper.py
--rw-r--r--   0        0        0    13277 2023-05-31 20:22:57.754277 rockset_v2_internal-2.0.1/rockset_v2/model/organization.py
--rw-r--r--   0        0        0    11821 2023-05-31 20:22:57.754684 rockset_v2_internal-2.0.1/rockset_v2/model/organization_response.py
--rw-r--r--   0        0        0    12527 2023-05-31 20:22:57.754999 rockset_v2_internal-2.0.1/rockset_v2/model/output_field.py
--rw-r--r--   0        0        0    11775 2023-05-31 20:22:57.755443 rockset_v2_internal-2.0.1/rockset_v2/model/pagination.py
--rw-r--r--   0        0        0    13055 2023-05-31 20:22:57.755848 rockset_v2_internal-2.0.1/rockset_v2/model/pagination_info.py
--rw-r--r--   0        0        0    12155 2023-05-31 20:22:57.756344 rockset_v2_internal-2.0.1/rockset_v2/model/patch_document.py
--rw-r--r--   0        0        0    11920 2023-05-31 20:22:57.756674 rockset_v2_internal-2.0.1/rockset_v2/model/patch_documents_request.py
--rw-r--r--   0        0        0    11868 2023-05-31 20:22:57.756981 rockset_v2_internal-2.0.1/rockset_v2/model/patch_documents_response.py
--rw-r--r--   0        0        0    13672 2023-05-31 20:22:57.757319 rockset_v2_internal-2.0.1/rockset_v2/model/patch_operation.py
--rw-r--r--   0        0        0    15362 2023-05-31 20:22:57.757664 rockset_v2_internal-2.0.1/rockset_v2/model/privilege.py
--rw-r--r--   0        0        0    12407 2023-05-31 20:22:57.757990 rockset_v2_internal-2.0.1/rockset_v2/model/query_error.py
--rw-r--r--   0        0        0    11907 2023-05-31 20:22:57.758316 rockset_v2_internal-2.0.1/rockset_v2/model/query_field_type.py
--rw-r--r--   0        0        0    14725 2023-05-31 20:22:57.758652 rockset_v2_internal-2.0.1/rockset_v2/model/query_info.py
--rw-r--r--   0        0        0    13688 2023-05-31 20:22:57.759425 rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda.py
--rw-r--r--   0        0        0    12219 2023-05-31 20:22:57.759775 rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda_sql.py
--rw-r--r--   0        0        0    12786 2023-05-31 20:22:57.760074 rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda_stats.py
--rw-r--r--   0        0        0    12124 2023-05-31 20:22:57.760417 rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda_tag.py
--rw-r--r--   0        0        0    11843 2023-05-31 20:22:57.760957 rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda_tag_response.py
--rw-r--r--   0        0        0    14841 2023-05-31 20:22:57.761387 rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda_version.py
--rw-r--r--   0        0        0    11883 2023-05-31 20:22:57.761811 rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda_version_response.py
--rw-r--r--   0        0        0    13051 2023-05-31 20:22:57.762352 rockset_v2_internal-2.0.1/rockset_v2/model/query_pagination_response.py
--rw-r--r--   0        0        0    12164 2023-05-31 20:22:57.762735 rockset_v2_internal-2.0.1/rockset_v2/model/query_parameter.py
--rw-r--r--   0        0        0    12227 2023-05-31 20:22:57.763053 rockset_v2_internal-2.0.1/rockset_v2/model/query_request.py
--rw-r--r--   0        0        0    14009 2023-05-31 20:22:57.763679 rockset_v2_internal-2.0.1/rockset_v2/model/query_request_sql.py
--rw-r--r--   0        0        0    16189 2023-05-31 20:22:57.764493 rockset_v2_internal-2.0.1/rockset_v2/model/query_response.py
--rw-r--r--   0        0        0    12105 2023-05-31 20:22:57.764845 rockset_v2_internal-2.0.1/rockset_v2/model/query_response_stats.py
--rw-r--r--   0        0        0    11870 2023-05-31 20:22:57.765161 rockset_v2_internal-2.0.1/rockset_v2/model/resume_virtual_instance_response.py
--rw-r--r--   0        0        0    13363 2023-05-31 20:22:57.765715 rockset_v2_internal-2.0.1/rockset_v2/model/role.py
--rw-r--r--   0        0        0    11741 2023-05-31 20:22:57.766027 rockset_v2_internal-2.0.1/rockset_v2/model/role_response.py
--rw-r--r--   0        0        0    14982 2023-05-31 20:22:57.766532 rockset_v2_internal-2.0.1/rockset_v2/model/s3_collection_creation_request.py
--rw-r--r--   0        0        0    12154 2023-05-31 20:22:57.767395 rockset_v2_internal-2.0.1/rockset_v2/model/s3_integration.py
--rw-r--r--   0        0        0    12394 2023-05-31 20:22:57.767816 rockset_v2_internal-2.0.1/rockset_v2/model/s3_integration_creation_request.py
--rw-r--r--   0        0        0    15239 2023-05-31 20:22:57.768194 rockset_v2_internal-2.0.1/rockset_v2/model/s3_source_wrapper.py
--rw-r--r--   0        0        0    12201 2023-05-31 20:22:57.768610 rockset_v2_internal-2.0.1/rockset_v2/model/schema_registry_config.py
--rw-r--r--   0        0        0    11696 2023-05-31 20:22:57.768957 rockset_v2_internal-2.0.1/rockset_v2/model/segment_integration.py
--rw-r--r--   0        0        0    12465 2023-05-31 20:22:57.769388 rockset_v2_internal-2.0.1/rockset_v2/model/segment_integration_creation_request.py
--rw-r--r--   0        0        0    15052 2023-05-31 20:22:57.769738 rockset_v2_internal-2.0.1/rockset_v2/model/snowflake_collection_creation_request.py
--rw-r--r--   0        0        0    14450 2023-05-31 20:22:57.770063 rockset_v2_internal-2.0.1/rockset_v2/model/snowflake_integration.py
--rw-r--r--   0        0        0    12499 2023-05-31 20:22:57.770527 rockset_v2_internal-2.0.1/rockset_v2/model/snowflake_integration_creation_request.py
--rw-r--r--   0        0        0    13907 2023-05-31 20:22:57.770850 rockset_v2_internal-2.0.1/rockset_v2/model/snowflake_source_wrapper.py
--rw-r--r--   0        0        0    12501 2023-05-31 20:22:57.771153 rockset_v2_internal-2.0.1/rockset_v2/model/source.py
--rw-r--r--   0        0        0    13169 2023-05-31 20:22:57.771547 rockset_v2_internal-2.0.1/rockset_v2/model/source_azure_blob_storage.py
--rw-r--r--   0        0        0    12664 2023-05-31 20:22:57.771924 rockset_v2_internal-2.0.1/rockset_v2/model/source_azure_event_hubs.py
--rw-r--r--   0        0        0    12552 2023-05-31 20:22:57.772312 rockset_v2_internal-2.0.1/rockset_v2/model/source_azure_service_bus.py
--rw-r--r--   0        0        0    13624 2023-05-31 20:22:57.772763 rockset_v2_internal-2.0.1/rockset_v2/model/source_dynamo_db.py
--rw-r--r--   0        0        0    12391 2023-05-31 20:22:57.773080 rockset_v2_internal-2.0.1/rockset_v2/model/source_file_upload.py
--rw-r--r--   0        0        0    13371 2023-05-31 20:22:57.773541 rockset_v2_internal-2.0.1/rockset_v2/model/source_gcs.py
--rw-r--r--   0        0        0    13209 2023-05-31 20:22:57.773887 rockset_v2_internal-2.0.1/rockset_v2/model/source_kafka.py
--rw-r--r--   0        0        0    13024 2023-05-31 20:22:57.774242 rockset_v2_internal-2.0.1/rockset_v2/model/source_kinesis.py
--rw-r--r--   0        0        0    12652 2023-05-31 20:22:57.774716 rockset_v2_internal-2.0.1/rockset_v2/model/source_mongo_db.py
--rw-r--r--   0        0        0    13923 2023-05-31 20:22:57.775467 rockset_v2_internal-2.0.1/rockset_v2/model/source_s3.py
--rw-r--r--   0        0        0    13110 2023-05-31 20:22:57.775801 rockset_v2_internal-2.0.1/rockset_v2/model/source_snowflake.py
--rw-r--r--   0        0        0    11661 2023-05-31 20:22:57.776181 rockset_v2_internal-2.0.1/rockset_v2/model/sql_expression.py
--rw-r--r--   0        0        0    13116 2023-05-31 20:22:57.776491 rockset_v2_internal-2.0.1/rockset_v2/model/stats.py
--rw-r--r--   0        0        0    13658 2023-05-31 20:22:57.776805 rockset_v2_internal-2.0.1/rockset_v2/model/status.py
--rw-r--r--   0        0        0    13111 2023-05-31 20:22:57.777100 rockset_v2_internal-2.0.1/rockset_v2/model/status_azure_event_hubs.py
--rw-r--r--   0        0        0    12364 2023-05-31 20:22:57.777358 rockset_v2_internal-2.0.1/rockset_v2/model/status_azure_event_hubs_partition.py
--rw-r--r--   0        0        0    12727 2023-05-31 20:22:57.777589 rockset_v2_internal-2.0.1/rockset_v2/model/status_azure_service_bus.py
--rw-r--r--   0        0        0    12210 2023-05-31 20:22:57.777829 rockset_v2_internal-2.0.1/rockset_v2/model/status_azure_service_bus_session.py
--rw-r--r--   0        0        0    13563 2023-05-31 20:22:57.778171 rockset_v2_internal-2.0.1/rockset_v2/model/status_dynamo_db.py
--rw-r--r--   0        0        0    12705 2023-05-31 20:22:57.778541 rockset_v2_internal-2.0.1/rockset_v2/model/status_dynamo_db_v2.py
--rw-r--r--   0        0        0    13123 2023-05-31 20:22:57.778860 rockset_v2_internal-2.0.1/rockset_v2/model/status_kafka.py
--rw-r--r--   0        0        0    12337 2023-05-31 20:22:57.779191 rockset_v2_internal-2.0.1/rockset_v2/model/status_kafka_partition.py
--rw-r--r--   0        0        0    15614 2023-05-31 20:22:57.779535 rockset_v2_internal-2.0.1/rockset_v2/model/status_mongo_db.py
--rw-r--r--   0        0        0    11924 2023-05-31 20:22:57.779903 rockset_v2_internal-2.0.1/rockset_v2/model/status_snowflake.py
--rw-r--r--   0        0        0    11873 2023-05-31 20:22:57.780473 rockset_v2_internal-2.0.1/rockset_v2/model/suspend_virtual_instance_response.py
--rw-r--r--   0        0        0    11894 2023-05-31 20:22:57.780924 rockset_v2_internal-2.0.1/rockset_v2/model/unsubscribe_preference.py
--rw-r--r--   0        0        0    12119 2023-05-31 20:22:57.781584 rockset_v2_internal-2.0.1/rockset_v2/model/update_alias_request.py
--rw-r--r--   0        0        0    11818 2023-05-31 20:22:57.782032 rockset_v2_internal-2.0.1/rockset_v2/model/update_api_key_request.py
--rw-r--r--   0        0        0    11780 2023-05-31 20:22:57.782492 rockset_v2_internal-2.0.1/rockset_v2/model/update_api_key_response.py
--rw-r--r--   0        0        0    11867 2023-05-31 20:22:57.782858 rockset_v2_internal-2.0.1/rockset_v2/model/update_integration_request.py
--rw-r--r--   0        0        0    11829 2023-05-31 20:22:57.783231 rockset_v2_internal-2.0.1/rockset_v2/model/update_integration_response.py
--rw-r--r--   0        0        0    12329 2023-05-31 20:22:57.783606 rockset_v2_internal-2.0.1/rockset_v2/model/update_query_lambda_request.py
--rw-r--r--   0        0        0    12222 2023-05-31 20:22:57.783961 rockset_v2_internal-2.0.1/rockset_v2/model/update_role_request.py
--rw-r--r--   0        0        0    12006 2023-05-31 20:22:57.784322 rockset_v2_internal-2.0.1/rockset_v2/model/update_unsubscribe_preferences_request.py
--rw-r--r--   0        0        0    12009 2023-05-31 20:22:57.784737 rockset_v2_internal-2.0.1/rockset_v2/model/update_unsubscribe_preferences_response.py
--rw-r--r--   0        0        0    12206 2023-05-31 20:22:57.785104 rockset_v2_internal-2.0.1/rockset_v2/model/update_user_request.py
--rw-r--r--   0        0        0    11958 2023-05-31 20:22:57.785462 rockset_v2_internal-2.0.1/rockset_v2/model/update_view_request.py
--rw-r--r--   0        0        0    11759 2023-05-31 20:22:57.786516 rockset_v2_internal-2.0.1/rockset_v2/model/update_view_response.py
--rw-r--r--   0        0        0    13762 2023-05-31 20:22:57.789960 rockset_v2_internal-2.0.1/rockset_v2/model/update_virtual_instance_request.py
--rw-r--r--   0        0        0    11870 2023-05-31 20:22:57.791906 rockset_v2_internal-2.0.1/rockset_v2/model/update_virtual_instance_response.py
--rw-r--r--   0        0        0    12907 2023-05-31 20:22:57.793949 rockset_v2_internal-2.0.1/rockset_v2/model/user.py
--rw-r--r--   0        0        0    12155 2023-05-31 20:22:57.797269 rockset_v2_internal-2.0.1/rockset_v2/model/validate_query_response.py
--rw-r--r--   0        0        0    14473 2023-05-31 20:22:57.799137 rockset_v2_internal-2.0.1/rockset_v2/model/view.py
--rw-r--r--   0        0        0    17180 2023-05-31 20:22:57.802096 rockset_v2_internal-2.0.1/rockset_v2/model/virtual_instance.py
--rw-r--r--   0        0        0    11772 2023-05-31 20:22:57.807892 rockset_v2_internal-2.0.1/rockset_v2/model/virtual_instance_stats.py
--rw-r--r--   0        0        0    12971 2023-05-31 20:22:57.810878 rockset_v2_internal-2.0.1/rockset_v2/model/workspace.py
--rw-r--r--   0        0        0    12998 2023-05-31 20:22:57.815681 rockset_v2_internal-2.0.1/rockset_v2/model/xml_params.py
--rw-r--r--   0        0        0    84037 2023-05-31 20:22:57.820220 rockset_v2_internal-2.0.1/rockset_v2/model_utils.py
--rw-r--r--   0        0        0    14505 2023-05-31 20:22:57.821126 rockset_v2_internal-2.0.1/rockset_v2/models/__init__.py
--rw-r--r--   0        0        0     1819 2023-05-31 20:22:57.821569 rockset_v2_internal-2.0.1/rockset_v2/query_paginator.py
--rw-r--r--   0        0        0    14645 2023-05-31 20:22:57.822226 rockset_v2_internal-2.0.1/rockset_v2/rest.py
--rw-r--r--   0        0        0     8911 2023-05-31 20:22:57.825466 rockset_v2_internal-2.0.1/rockset_v2/rockset_client.py
--rw-r--r--   0        0        0     3644 2023-05-31 20:22:57.826319 rockset_v2_internal-2.0.1/rockset_v2/value.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 rockset_v2_internal-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      357 2023-05-31 19:49:16.995381 rockset_v2_internal-2.0.2/LONG_DESCRIPTION.rst
+-rw-r--r--   0        0        0     1631 2023-05-31 20:54:20.725789 rockset_v2_internal-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1374 2023-05-31 20:52:54.668784 rockset_v2_internal-2.0.2/rockset_v2/__init__.py
+-rw-r--r--   0        0        0      211 2023-05-31 20:52:54.669430 rockset_v2_internal-2.0.2/rockset_v2/api/__init__.py
+-rw-r--r--   0        0        0    34326 2023-05-31 20:52:54.678835 rockset_v2_internal-2.0.2/rockset_v2/api/aliases_api.py
+-rw-r--r--   0        0        0    29389 2023-05-31 20:52:54.679641 rockset_v2_internal-2.0.2/rockset_v2/api/api_keys_api.py
+-rw-r--r--   0        0        0   123960 2023-05-31 20:52:54.680752 rockset_v2_internal-2.0.2/rockset_v2/api/collections_api.py
+-rw-r--r--   0        0        0    27749 2023-05-31 20:52:54.681502 rockset_v2_internal-2.0.2/rockset_v2/api/custom_roles_api.py
+-rw-r--r--   0        0        0    20873 2023-05-31 20:52:54.682223 rockset_v2_internal-2.0.2/rockset_v2/api/documents_api.py
+-rw-r--r--   0        0        0    72229 2023-05-31 20:52:54.683722 rockset_v2_internal-2.0.2/rockset_v2/api/integrations_api.py
+-rw-r--r--   0        0        0     6127 2023-05-31 20:52:54.684546 rockset_v2_internal-2.0.2/rockset_v2/api/organizations_api.py
+-rw-r--r--   0        0        0    34713 2023-05-31 20:52:54.685380 rockset_v2_internal-2.0.2/rockset_v2/api/queries_api.py
+-rw-r--r--   0        0        0    86522 2023-05-31 20:52:54.686206 rockset_v2_internal-2.0.2/rockset_v2/api/query_lambdas_api.py
+-rw-r--r--   0        0        0     7681 2023-05-31 20:52:54.686848 rockset_v2_internal-2.0.2/rockset_v2/api/shared_lambdas_api.py
+-rw-r--r--   0        0        0    42739 2023-05-31 20:52:54.687560 rockset_v2_internal-2.0.2/rockset_v2/api/users_api.py
+-rw-r--r--   0        0        0    34074 2023-05-31 20:52:54.688393 rockset_v2_internal-2.0.2/rockset_v2/api/views_api.py
+-rw-r--r--   0        0        0    76699 2023-05-31 20:52:54.689360 rockset_v2_internal-2.0.2/rockset_v2/api/virtual_instances_api.py
+-rw-r--r--   0        0        0    21874 2023-05-31 20:52:54.690146 rockset_v2_internal-2.0.2/rockset_v2/api/workspaces_api.py
+-rw-r--r--   0        0        0    36257 2023-05-31 20:52:54.690953 rockset_v2_internal-2.0.2/rockset_v2/api_client.py
+-rw-r--r--   0        0        0     1154 2023-05-31 20:52:54.691846 rockset_v2_internal-2.0.2/rockset_v2/apis/__init__.py
+-rw-r--r--   0        0        0    15525 2023-05-31 20:52:54.692561 rockset_v2_internal-2.0.2/rockset_v2/configuration.py
+-rw-r--r--   0        0        0     3831 2023-05-31 20:22:57.717401 rockset_v2_internal-2.0.2/rockset_v2/document.py
+-rw-r--r--   0        0        0     6072 2023-05-31 20:22:57.717639 rockset_v2_internal-2.0.2/rockset_v2/exceptions.py
+-rw-r--r--   0        0        0      348 2023-05-31 20:22:57.717962 rockset_v2_internal-2.0.2/rockset_v2/model/__init__.py
+-rw-r--r--   0        0        0    11956 2023-05-31 20:52:54.693630 rockset_v2_internal-2.0.2/rockset_v2/model/add_documents_request.py
+-rw-r--r--   0        0        0    11931 2023-05-31 20:52:54.694218 rockset_v2_internal-2.0.2/rockset_v2/model/add_documents_response.py
+-rw-r--r--   0        0        0    13629 2023-05-31 20:52:54.695024 rockset_v2_internal-2.0.2/rockset_v2/model/alias.py
+-rw-r--r--   0        0        0    13951 2023-05-31 20:52:54.696295 rockset_v2_internal-2.0.2/rockset_v2/model/api_key.py
+-rw-r--r--   0        0        0    13816 2023-05-31 20:52:54.697323 rockset_v2_internal-2.0.2/rockset_v2/model/async_query_options.py
+-rw-r--r--   0        0        0    13738 2023-05-31 20:52:54.697710 rockset_v2_internal-2.0.2/rockset_v2/model/auto_scaling_policy.py
+-rw-r--r--   0        0        0    12235 2023-05-31 20:52:54.698681 rockset_v2_internal-2.0.2/rockset_v2/model/aws_access_key.py
+-rw-r--r--   0        0        0    12107 2023-05-31 20:52:54.699789 rockset_v2_internal-2.0.2/rockset_v2/model/aws_role.py
+-rw-r--r--   0        0        0    15090 2023-05-31 20:52:54.700798 rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_collection_creation_request.py
+-rw-r--r--   0        0        0    11899 2023-05-31 20:52:54.701579 rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_integration.py
+-rw-r--r--   0        0        0    12625 2023-05-31 20:52:54.702781 rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_integration_creation_request.py
+-rw-r--r--   0        0        0    14461 2023-05-31 20:52:54.703521 rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_source_wrapper.py
+-rw-r--r--   0        0        0    15070 2023-05-31 20:52:54.704595 rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_collection_creation_request.py
+-rw-r--r--   0        0        0    11793 2023-05-31 20:52:54.705820 rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_integration.py
+-rw-r--r--   0        0        0    12595 2023-05-31 20:52:54.706772 rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_integration_creation_request.py
+-rw-r--r--   0        0        0    13464 2023-05-31 20:52:54.707823 rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_source_wrapper.py
+-rw-r--r--   0        0        0    15080 2023-05-31 20:52:54.709390 rockset_v2_internal-2.0.2/rockset_v2/model/azure_service_bus_collection_creation_request.py
+-rw-r--r--   0        0        0    11894 2023-05-31 20:52:54.710837 rockset_v2_internal-2.0.2/rockset_v2/model/azure_service_bus_integration.py
+-rw-r--r--   0        0        0    13345 2023-05-31 20:52:54.712479 rockset_v2_internal-2.0.2/rockset_v2/model/azure_service_bus_source_wrapper.py
+-rw-r--r--   0        0        0    18749 2023-05-31 20:52:54.713846 rockset_v2_internal-2.0.2/rockset_v2/model/bulk_stats.py
+-rw-r--r--   0        0        0    11807 2023-05-31 20:52:54.715183 rockset_v2_internal-2.0.2/rockset_v2/model/cancel_query_response.py
+-rw-r--r--   0        0        0    13231 2023-05-31 20:52:54.715939 rockset_v2_internal-2.0.2/rockset_v2/model/cluster.py
+-rw-r--r--   0        0        0    17711 2023-05-31 20:52:54.717512 rockset_v2_internal-2.0.2/rockset_v2/model/collection.py
+-rw-r--r--   0        0        0    14856 2023-05-31 20:52:54.719559 rockset_v2_internal-2.0.2/rockset_v2/model/collection_mount.py
+-rw-r--r--   0        0        0    11861 2023-05-31 20:52:54.720428 rockset_v2_internal-2.0.2/rockset_v2/model/collection_mount_response.py
+-rw-r--r--   0        0        0    11778 2023-05-31 20:52:54.721389 rockset_v2_internal-2.0.2/rockset_v2/model/collection_mount_stats.py
+-rw-r--r--   0        0        0    16971 2023-05-31 20:52:54.725144 rockset_v2_internal-2.0.2/rockset_v2/model/collection_stats.py
+-rw-r--r--   0        0        0    12339 2023-05-31 20:52:54.727224 rockset_v2_internal-2.0.2/rockset_v2/model/create_alias_request.py
+-rw-r--r--   0        0        0    11778 2023-05-31 20:52:54.737776 rockset_v2_internal-2.0.2/rockset_v2/model/create_alias_response.py
+-rw-r--r--   0        0        0    12104 2023-05-31 20:52:54.761872 rockset_v2_internal-2.0.2/rockset_v2/model/create_api_key_request.py
+-rw-r--r--   0        0        0    11789 2023-05-31 20:52:54.763333 rockset_v2_internal-2.0.2/rockset_v2/model/create_api_key_response.py
+-rw-r--r--   0        0        0    11771 2023-05-31 20:52:54.764061 rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_mount_request.py
+-rw-r--r--   0        0        0    11922 2023-05-31 20:52:54.764798 rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_mounts_response.py
+-rw-r--r--   0        0        0    14469 2023-05-31 20:52:54.765467 rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_request.py
+-rw-r--r--   0        0        0    11828 2023-05-31 20:52:54.765965 rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_response.py
+-rw-r--r--   0        0        0    16073 2023-05-31 20:52:54.766729 rockset_v2_internal-2.0.2/rockset_v2/model/create_integration_request.py
+-rw-r--r--   0        0        0    11838 2023-05-31 20:52:54.767246 rockset_v2_internal-2.0.2/rockset_v2/model/create_integration_response.py
+-rw-r--r--   0        0        0    12580 2023-05-31 20:52:54.767852 rockset_v2_internal-2.0.2/rockset_v2/model/create_query_lambda_request.py
+-rw-r--r--   0        0        0    12069 2023-05-31 20:52:54.768352 rockset_v2_internal-2.0.2/rockset_v2/model/create_query_lambda_tag_request.py
+-rw-r--r--   0        0        0    12510 2023-05-31 20:52:54.768856 rockset_v2_internal-2.0.2/rockset_v2/model/create_role_request.py
+-rw-r--r--   0        0        0    12485 2023-05-31 20:52:54.769418 rockset_v2_internal-2.0.2/rockset_v2/model/create_user_request.py
+-rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.770225 rockset_v2_internal-2.0.2/rockset_v2/model/create_user_response.py
+-rw-r--r--   0        0        0    12176 2023-05-31 20:52:54.770846 rockset_v2_internal-2.0.2/rockset_v2/model/create_view_request.py
+-rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.771427 rockset_v2_internal-2.0.2/rockset_v2/model/create_view_response.py
+-rw-r--r--   0        0        0    14411 2023-05-31 20:52:54.771968 rockset_v2_internal-2.0.2/rockset_v2/model/create_virtual_instance_request.py
+-rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.772546 rockset_v2_internal-2.0.2/rockset_v2/model/create_virtual_instance_response.py
+-rw-r--r--   0        0        0    12044 2023-05-31 20:52:54.773122 rockset_v2_internal-2.0.2/rockset_v2/model/create_workspace_request.py
+-rw-r--r--   0        0        0    11818 2023-05-31 20:52:54.773681 rockset_v2_internal-2.0.2/rockset_v2/model/create_workspace_response.py
+-rw-r--r--   0        0        0    14185 2023-05-31 20:52:54.774385 rockset_v2_internal-2.0.2/rockset_v2/model/csv_params.py
+-rw-r--r--   0        0        0    11778 2023-05-31 20:52:54.774966 rockset_v2_internal-2.0.2/rockset_v2/model/delete_alias_response.py
+-rw-r--r--   0        0        0    11789 2023-05-31 20:52:54.775639 rockset_v2_internal-2.0.2/rockset_v2/model/delete_api_key_response.py
+-rw-r--r--   0        0        0    11828 2023-05-31 20:52:54.776278 rockset_v2_internal-2.0.2/rockset_v2/model/delete_collection_response.py
+-rw-r--r--   0        0        0    12045 2023-05-31 20:52:54.776848 rockset_v2_internal-2.0.2/rockset_v2/model/delete_documents_request.py
+-rw-r--r--   0        0        0    11692 2023-05-31 20:52:54.777489 rockset_v2_internal-2.0.2/rockset_v2/model/delete_documents_request_data.py
+-rw-r--r--   0        0        0    11936 2023-05-31 20:52:54.778541 rockset_v2_internal-2.0.2/rockset_v2/model/delete_documents_response.py
+-rw-r--r--   0        0        0    11838 2023-05-31 20:52:54.779445 rockset_v2_internal-2.0.2/rockset_v2/model/delete_integration_response.py
+-rw-r--r--   0        0        0    11839 2023-05-31 20:52:54.780123 rockset_v2_internal-2.0.2/rockset_v2/model/delete_query_lambda_response.py
+-rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.780776 rockset_v2_internal-2.0.2/rockset_v2/model/delete_user_response.py
+-rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.781405 rockset_v2_internal-2.0.2/rockset_v2/model/delete_view_response.py
+-rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.781884 rockset_v2_internal-2.0.2/rockset_v2/model/delete_virtual_instance_response.py
+-rw-r--r--   0        0        0    11818 2023-05-31 20:52:54.782423 rockset_v2_internal-2.0.2/rockset_v2/model/delete_workspace_response.py
+-rw-r--r--   0        0        0    13032 2023-05-31 20:52:54.783053 rockset_v2_internal-2.0.2/rockset_v2/model/document_status.py
+-rw-r--r--   0        0        0    15008 2023-05-31 20:52:54.783640 rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_collection_creation_request.py
+-rw-r--r--   0        0        0    12575 2023-05-31 20:52:54.784429 rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_integration.py
+-rw-r--r--   0        0        0    12493 2023-05-31 20:52:54.785247 rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_integration_creation_request.py
+-rw-r--r--   0        0        0    14455 2023-05-31 20:52:54.785747 rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_source_wrapper.py
+-rw-r--r--   0        0        0    14526 2023-05-31 20:52:54.786379 rockset_v2_internal-2.0.2/rockset_v2/model/error_model.py
+-rw-r--r--   0        0        0    12398 2023-05-31 20:52:54.787029 rockset_v2_internal-2.0.2/rockset_v2/model/event_time_info.py
+-rw-r--r--   0        0        0    12665 2023-05-31 20:52:54.788776 rockset_v2_internal-2.0.2/rockset_v2/model/execute_public_query_lambda_request.py
+-rw-r--r--   0        0        0    15071 2023-05-31 20:52:54.789474 rockset_v2_internal-2.0.2/rockset_v2/model/execute_query_lambda_request.py
+-rw-r--r--   0        0        0    11749 2023-05-31 20:52:54.790079 rockset_v2_internal-2.0.2/rockset_v2/model/field_mapping_query.py
+-rw-r--r--   0        0        0    13087 2023-05-31 20:52:54.790704 rockset_v2_internal-2.0.2/rockset_v2/model/field_mapping_v2.py
+-rw-r--r--   0        0        0    12549 2023-05-31 20:52:54.791297 rockset_v2_internal-2.0.2/rockset_v2/model/field_partition.py
+-rw-r--r--   0        0        0    15029 2023-05-31 20:52:54.791891 rockset_v2_internal-2.0.2/rockset_v2/model/file_upload_collection_creation_request.py
+-rw-r--r--   0        0        0    13623 2023-05-31 20:52:54.792409 rockset_v2_internal-2.0.2/rockset_v2/model/file_upload_source_wrapper.py
+-rw-r--r--   0        0        0    13214 2023-05-31 20:52:54.792957 rockset_v2_internal-2.0.2/rockset_v2/model/format_params.py
+-rw-r--r--   0        0        0    12007 2023-05-31 20:52:54.793500 rockset_v2_internal-2.0.2/rockset_v2/model/gcp_service_account.py
+-rw-r--r--   0        0        0    14958 2023-05-31 20:52:54.794134 rockset_v2_internal-2.0.2/rockset_v2/model/gcs_collection_creation_request.py
+-rw-r--r--   0        0        0    11924 2023-05-31 20:52:54.794888 rockset_v2_internal-2.0.2/rockset_v2/model/gcs_integration.py
+-rw-r--r--   0        0        0    12418 2023-05-31 20:52:54.795809 rockset_v2_internal-2.0.2/rockset_v2/model/gcs_integration_creation_request.py
+-rw-r--r--   0        0        0    14678 2023-05-31 20:52:54.796507 rockset_v2_internal-2.0.2/rockset_v2/model/gcs_source_wrapper.py
+-rw-r--r--   0        0        0    11769 2023-05-31 20:52:54.797210 rockset_v2_internal-2.0.2/rockset_v2/model/get_alias_response.py
+-rw-r--r--   0        0        0    11780 2023-05-31 20:52:54.797823 rockset_v2_internal-2.0.2/rockset_v2/model/get_api_key_response.py
+-rw-r--r--   0        0        0    11819 2023-05-31 20:52:54.798426 rockset_v2_internal-2.0.2/rockset_v2/model/get_collection_response.py
+-rw-r--r--   0        0        0    11829 2023-05-31 20:52:54.799070 rockset_v2_internal-2.0.2/rockset_v2/model/get_integration_response.py
+-rw-r--r--   0        0        0    11798 2023-05-31 20:52:54.799760 rockset_v2_internal-2.0.2/rockset_v2/model/get_query_response.py
+-rw-r--r--   0        0        0    11759 2023-05-31 20:52:54.800502 rockset_v2_internal-2.0.2/rockset_v2/model/get_view_response.py
+-rw-r--r--   0        0        0    11870 2023-05-31 20:52:54.801176 rockset_v2_internal-2.0.2/rockset_v2/model/get_virtual_instance_response.py
+-rw-r--r--   0        0        0    11809 2023-05-31 20:52:54.801799 rockset_v2_internal-2.0.2/rockset_v2/model/get_workspace_response.py
+-rw-r--r--   0        0        0    12710 2023-05-31 20:52:54.802549 rockset_v2_internal-2.0.2/rockset_v2/model/input_field.py
+-rw-r--r--   0        0        0    17401 2023-05-31 20:52:54.803292 rockset_v2_internal-2.0.2/rockset_v2/model/integration.py
+-rw-r--r--   0        0        0    14978 2023-05-31 20:52:54.803958 rockset_v2_internal-2.0.2/rockset_v2/model/kafka_collection_creation_request.py
+-rw-r--r--   0        0        0    14844 2023-05-31 20:52:54.804557 rockset_v2_internal-2.0.2/rockset_v2/model/kafka_integration.py
+-rw-r--r--   0        0        0    12448 2023-05-31 20:52:54.805231 rockset_v2_internal-2.0.2/rockset_v2/model/kafka_integration_creation_request.py
+-rw-r--r--   0        0        0    14039 2023-05-31 20:52:54.806144 rockset_v2_internal-2.0.2/rockset_v2/model/kafka_source_wrapper.py
+-rw-r--r--   0        0        0    11851 2023-05-31 20:52:54.806771 rockset_v2_internal-2.0.2/rockset_v2/model/kafka_v3_security_config.py
+-rw-r--r--   0        0        0    14998 2023-05-31 20:52:54.807438 rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_collection_creation_request.py
+-rw-r--r--   0        0        0    12181 2023-05-31 20:52:54.808157 rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_integration.py
+-rw-r--r--   0        0        0    12478 2023-05-31 20:52:54.808764 rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_integration_creation_request.py
+-rw-r--r--   0        0        0    14277 2023-05-31 20:52:54.809373 rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_source_wrapper.py
+-rw-r--r--   0        0        0    11828 2023-05-31 20:52:54.809989 rockset_v2_internal-2.0.2/rockset_v2/model/list_aliases_response.py
+-rw-r--r--   0        0        0    11844 2023-05-31 20:52:54.810528 rockset_v2_internal-2.0.2/rockset_v2/model/list_api_keys_response.py
+-rw-r--r--   0        0        0    11946 2023-05-31 20:52:54.811273 rockset_v2_internal-2.0.2/rockset_v2/model/list_collection_mounts_response.py
+-rw-r--r--   0        0        0    11883 2023-05-31 20:52:54.811866 rockset_v2_internal-2.0.2/rockset_v2/model/list_collections_response.py
+-rw-r--r--   0        0        0    11901 2023-05-31 20:52:54.812416 rockset_v2_internal-2.0.2/rockset_v2/model/list_integrations_response.py
+-rw-r--r--   0        0        0    11813 2023-05-31 20:52:54.813018 rockset_v2_internal-2.0.2/rockset_v2/model/list_queries_response.py
+-rw-r--r--   0        0        0    11973 2023-05-31 20:52:54.813725 rockset_v2_internal-2.0.2/rockset_v2/model/list_query_lambda_tags_response.py
+-rw-r--r--   0        0        0    12019 2023-05-31 20:52:54.814288 rockset_v2_internal-2.0.2/rockset_v2/model/list_query_lambda_versions_response.py
+-rw-r--r--   0        0        0    11898 2023-05-31 20:52:54.814906 rockset_v2_internal-2.0.2/rockset_v2/model/list_query_lambdas_response.py
+-rw-r--r--   0        0        0    11811 2023-05-31 20:52:54.815485 rockset_v2_internal-2.0.2/rockset_v2/model/list_roles_response.py
+-rw-r--r--   0        0        0    12012 2023-05-31 20:52:54.816034 rockset_v2_internal-2.0.2/rockset_v2/model/list_unsubscribe_preferences_response.py
+-rw-r--r--   0        0        0    11803 2023-05-31 20:52:54.816755 rockset_v2_internal-2.0.2/rockset_v2/model/list_users_response.py
+-rw-r--r--   0        0        0    11811 2023-05-31 20:52:54.817393 rockset_v2_internal-2.0.2/rockset_v2/model/list_views_response.py
+-rw-r--r--   0        0        0    11946 2023-05-31 20:52:54.818009 rockset_v2_internal-2.0.2/rockset_v2/model/list_virtual_instances_response.py
+-rw-r--r--   0        0        0    11863 2023-05-31 20:52:54.818520 rockset_v2_internal-2.0.2/rockset_v2/model/list_workspaces_response.py
+-rw-r--r--   0        0        0    11821 2023-05-31 20:52:54.818957 rockset_v2_internal-2.0.2/rockset_v2/model/mongo_db_integration.py
+-rw-r--r--   0        0        0    14998 2023-05-31 20:52:54.819368 rockset_v2_internal-2.0.2/rockset_v2/model/mongodb_collection_creation_request.py
+-rw-r--r--   0        0        0    12479 2023-05-31 20:52:54.819828 rockset_v2_internal-2.0.2/rockset_v2/model/mongodb_integration_creation_request.py
+-rw-r--r--   0        0        0    14135 2023-05-31 20:52:54.820417 rockset_v2_internal-2.0.2/rockset_v2/model/mongodb_source_wrapper.py
+-rw-r--r--   0        0        0    13286 2023-05-31 20:52:54.821198 rockset_v2_internal-2.0.2/rockset_v2/model/organization.py
+-rw-r--r--   0        0        0    11830 2023-05-31 20:52:54.821707 rockset_v2_internal-2.0.2/rockset_v2/model/organization_response.py
+-rw-r--r--   0        0        0    12536 2023-05-31 20:52:54.822222 rockset_v2_internal-2.0.2/rockset_v2/model/output_field.py
+-rw-r--r--   0        0        0    11781 2023-05-31 20:52:54.822887 rockset_v2_internal-2.0.2/rockset_v2/model/pagination.py
+-rw-r--r--   0        0        0    13061 2023-05-31 20:52:54.823465 rockset_v2_internal-2.0.2/rockset_v2/model/pagination_info.py
+-rw-r--r--   0        0        0    12164 2023-05-31 20:52:54.823998 rockset_v2_internal-2.0.2/rockset_v2/model/patch_document.py
+-rw-r--r--   0        0        0    11929 2023-05-31 20:52:54.824597 rockset_v2_internal-2.0.2/rockset_v2/model/patch_documents_request.py
+-rw-r--r--   0        0        0    11877 2023-05-31 20:52:54.825322 rockset_v2_internal-2.0.2/rockset_v2/model/patch_documents_response.py
+-rw-r--r--   0        0        0    13678 2023-05-31 20:52:54.826018 rockset_v2_internal-2.0.2/rockset_v2/model/patch_operation.py
+-rw-r--r--   0        0        0    15368 2023-05-31 20:52:54.826678 rockset_v2_internal-2.0.2/rockset_v2/model/privilege.py
+-rw-r--r--   0        0        0    12413 2023-05-31 20:52:54.827279 rockset_v2_internal-2.0.2/rockset_v2/model/query_error.py
+-rw-r--r--   0        0        0    11913 2023-05-31 20:52:54.827812 rockset_v2_internal-2.0.2/rockset_v2/model/query_field_type.py
+-rw-r--r--   0        0        0    14987 2023-05-31 20:52:54.828428 rockset_v2_internal-2.0.2/rockset_v2/model/query_info.py
+-rw-r--r--   0        0        0    13697 2023-05-31 20:52:54.829507 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda.py
+-rw-r--r--   0        0        0    12228 2023-05-31 20:52:54.830135 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_sql.py
+-rw-r--r--   0        0        0    12792 2023-05-31 20:52:54.830680 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_stats.py
+-rw-r--r--   0        0        0    12133 2023-05-31 20:52:54.831264 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_tag.py
+-rw-r--r--   0        0        0    11852 2023-05-31 20:52:54.831771 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_tag_response.py
+-rw-r--r--   0        0        0    14853 2023-05-31 20:52:54.832400 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_version.py
+-rw-r--r--   0        0        0    11892 2023-05-31 20:52:54.832985 rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_version_response.py
+-rw-r--r--   0        0        0    12738 2023-05-31 20:52:54.833662 rockset_v2_internal-2.0.2/rockset_v2/model/query_pagination_response.py
+-rw-r--r--   0        0        0    12194 2023-05-31 20:52:54.834352 rockset_v2_internal-2.0.2/rockset_v2/model/query_parameter.py
+-rw-r--r--   0        0        0    12931 2023-05-31 20:52:54.834962 rockset_v2_internal-2.0.2/rockset_v2/model/query_request.py
+-rw-r--r--   0        0        0    13635 2023-05-31 20:52:54.835566 rockset_v2_internal-2.0.2/rockset_v2/model/query_request_sql.py
+-rw-r--r--   0        0        0    15855 2023-05-31 20:52:54.836172 rockset_v2_internal-2.0.2/rockset_v2/model/query_response.py
+-rw-r--r--   0        0        0    12111 2023-05-31 20:52:54.836759 rockset_v2_internal-2.0.2/rockset_v2/model/query_response_stats.py
+-rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.837479 rockset_v2_internal-2.0.2/rockset_v2/model/resume_virtual_instance_response.py
+-rw-r--r--   0        0        0    13372 2023-05-31 20:52:54.837978 rockset_v2_internal-2.0.2/rockset_v2/model/role.py
+-rw-r--r--   0        0        0    11750 2023-05-31 20:52:54.838436 rockset_v2_internal-2.0.2/rockset_v2/model/role_response.py
+-rw-r--r--   0        0        0    14948 2023-05-31 20:52:54.838895 rockset_v2_internal-2.0.2/rockset_v2/model/s3_collection_creation_request.py
+-rw-r--r--   0        0        0    12166 2023-05-31 20:52:54.839359 rockset_v2_internal-2.0.2/rockset_v2/model/s3_integration.py
+-rw-r--r--   0        0        0    12403 2023-05-31 20:52:54.839833 rockset_v2_internal-2.0.2/rockset_v2/model/s3_integration_creation_request.py
+-rw-r--r--   0        0        0    15251 2023-05-31 20:52:54.840241 rockset_v2_internal-2.0.2/rockset_v2/model/s3_source_wrapper.py
+-rw-r--r--   0        0        0    12207 2023-05-31 20:52:54.840748 rockset_v2_internal-2.0.2/rockset_v2/model/schema_registry_config.py
+-rw-r--r--   0        0        0    11696 2023-05-31 20:22:57.768957 rockset_v2_internal-2.0.2/rockset_v2/model/segment_integration.py
+-rw-r--r--   0        0        0    12465 2023-05-31 20:22:57.769388 rockset_v2_internal-2.0.2/rockset_v2/model/segment_integration_creation_request.py
+-rw-r--r--   0        0        0    15018 2023-05-31 20:52:54.841148 rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_collection_creation_request.py
+-rw-r--r--   0        0        0    14462 2023-05-31 20:52:54.841656 rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_integration.py
+-rw-r--r--   0        0        0    12508 2023-05-31 20:52:54.842466 rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_integration_creation_request.py
+-rw-r--r--   0        0        0    13919 2023-05-31 20:52:54.843061 rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_source_wrapper.py
+-rw-r--r--   0        0        0    12513 2023-05-31 20:52:54.843639 rockset_v2_internal-2.0.2/rockset_v2/model/source.py
+-rw-r--r--   0        0        0    13175 2023-05-31 20:52:54.844600 rockset_v2_internal-2.0.2/rockset_v2/model/source_azure_blob_storage.py
+-rw-r--r--   0        0        0    12673 2023-05-31 20:52:54.845250 rockset_v2_internal-2.0.2/rockset_v2/model/source_azure_event_hubs.py
+-rw-r--r--   0        0        0    12561 2023-05-31 20:52:54.845894 rockset_v2_internal-2.0.2/rockset_v2/model/source_azure_service_bus.py
+-rw-r--r--   0        0        0    13636 2023-05-31 20:52:54.846554 rockset_v2_internal-2.0.2/rockset_v2/model/source_dynamo_db.py
+-rw-r--r--   0        0        0    12397 2023-05-31 20:52:54.847182 rockset_v2_internal-2.0.2/rockset_v2/model/source_file_upload.py
+-rw-r--r--   0        0        0    13377 2023-05-31 20:52:54.847838 rockset_v2_internal-2.0.2/rockset_v2/model/source_gcs.py
+-rw-r--r--   0        0        0    13218 2023-05-31 20:52:54.848518 rockset_v2_internal-2.0.2/rockset_v2/model/source_kafka.py
+-rw-r--r--   0        0        0    13030 2023-05-31 20:52:54.849174 rockset_v2_internal-2.0.2/rockset_v2/model/source_kinesis.py
+-rw-r--r--   0        0        0    13324 2023-05-31 20:52:54.849861 rockset_v2_internal-2.0.2/rockset_v2/model/source_mongo_db.py
+-rw-r--r--   0        0        0    13929 2023-05-31 20:52:54.850690 rockset_v2_internal-2.0.2/rockset_v2/model/source_s3.py
+-rw-r--r--   0        0        0    13119 2023-05-31 20:52:54.851312 rockset_v2_internal-2.0.2/rockset_v2/model/source_snowflake.py
+-rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.851690 rockset_v2_internal-2.0.2/rockset_v2/model/source_system.py
+-rw-r--r--   0        0        0    11667 2023-05-31 20:52:54.852404 rockset_v2_internal-2.0.2/rockset_v2/model/sql_expression.py
+-rw-r--r--   0        0        0    13122 2023-05-31 20:52:54.853717 rockset_v2_internal-2.0.2/rockset_v2/model/stats.py
+-rw-r--r--   0        0        0    13664 2023-05-31 20:52:54.854365 rockset_v2_internal-2.0.2/rockset_v2/model/status.py
+-rw-r--r--   0        0        0    13120 2023-05-31 20:52:54.854952 rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_event_hubs.py
+-rw-r--r--   0        0        0    12370 2023-05-31 20:52:54.855801 rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_event_hubs_partition.py
+-rw-r--r--   0        0        0    12736 2023-05-31 20:52:54.856414 rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_service_bus.py
+-rw-r--r--   0        0        0    12216 2023-05-31 20:52:54.857296 rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_service_bus_session.py
+-rw-r--r--   0        0        0    13569 2023-05-31 20:52:54.857991 rockset_v2_internal-2.0.2/rockset_v2/model/status_dynamo_db.py
+-rw-r--r--   0        0        0    12711 2023-05-31 20:52:54.858679 rockset_v2_internal-2.0.2/rockset_v2/model/status_dynamo_db_v2.py
+-rw-r--r--   0        0        0    13132 2023-05-31 20:52:54.859333 rockset_v2_internal-2.0.2/rockset_v2/model/status_kafka.py
+-rw-r--r--   0        0        0    12343 2023-05-31 20:52:54.859863 rockset_v2_internal-2.0.2/rockset_v2/model/status_kafka_partition.py
+-rw-r--r--   0        0        0    15620 2023-05-31 20:52:54.860443 rockset_v2_internal-2.0.2/rockset_v2/model/status_mongo_db.py
+-rw-r--r--   0        0        0    11930 2023-05-31 20:52:54.860923 rockset_v2_internal-2.0.2/rockset_v2/model/status_snowflake.py
+-rw-r--r--   0        0        0    11882 2023-05-31 20:52:54.861396 rockset_v2_internal-2.0.2/rockset_v2/model/suspend_virtual_instance_response.py
+-rw-r--r--   0        0        0    11900 2023-05-31 20:52:54.862111 rockset_v2_internal-2.0.2/rockset_v2/model/unsubscribe_preference.py
+-rw-r--r--   0        0        0    12125 2023-05-31 20:52:54.862684 rockset_v2_internal-2.0.2/rockset_v2/model/update_alias_request.py
+-rw-r--r--   0        0        0    11824 2023-05-31 20:52:54.863145 rockset_v2_internal-2.0.2/rockset_v2/model/update_api_key_request.py
+-rw-r--r--   0        0        0    11789 2023-05-31 20:52:54.863693 rockset_v2_internal-2.0.2/rockset_v2/model/update_api_key_response.py
+-rw-r--r--   0        0        0    12256 2023-05-31 20:52:54.864067 rockset_v2_internal-2.0.2/rockset_v2/model/update_collection_request.py
+-rw-r--r--   0        0        0    11867 2023-05-31 20:22:57.782858 rockset_v2_internal-2.0.2/rockset_v2/model/update_integration_request.py
+-rw-r--r--   0        0        0    11829 2023-05-31 20:22:57.783231 rockset_v2_internal-2.0.2/rockset_v2/model/update_integration_response.py
+-rw-r--r--   0        0        0    12338 2023-05-31 20:52:54.864615 rockset_v2_internal-2.0.2/rockset_v2/model/update_query_lambda_request.py
+-rw-r--r--   0        0        0    12231 2023-05-31 20:52:54.865200 rockset_v2_internal-2.0.2/rockset_v2/model/update_role_request.py
+-rw-r--r--   0        0        0    12015 2023-05-31 20:52:54.865776 rockset_v2_internal-2.0.2/rockset_v2/model/update_unsubscribe_preferences_request.py
+-rw-r--r--   0        0        0    12018 2023-05-31 20:52:54.866368 rockset_v2_internal-2.0.2/rockset_v2/model/update_unsubscribe_preferences_response.py
+-rw-r--r--   0        0        0    12212 2023-05-31 20:52:54.866855 rockset_v2_internal-2.0.2/rockset_v2/model/update_user_request.py
+-rw-r--r--   0        0        0    11964 2023-05-31 20:52:54.867381 rockset_v2_internal-2.0.2/rockset_v2/model/update_view_request.py
+-rw-r--r--   0        0        0    11768 2023-05-31 20:52:54.867851 rockset_v2_internal-2.0.2/rockset_v2/model/update_view_response.py
+-rw-r--r--   0        0        0    15183 2023-05-31 20:52:54.868410 rockset_v2_internal-2.0.2/rockset_v2/model/update_virtual_instance_request.py
+-rw-r--r--   0        0        0    11879 2023-05-31 20:52:54.869001 rockset_v2_internal-2.0.2/rockset_v2/model/update_virtual_instance_response.py
+-rw-r--r--   0        0        0    12913 2023-05-31 20:52:54.869670 rockset_v2_internal-2.0.2/rockset_v2/model/user.py
+-rw-r--r--   0        0        0    12161 2023-05-31 20:52:54.870144 rockset_v2_internal-2.0.2/rockset_v2/model/validate_query_response.py
+-rw-r--r--   0        0        0    14479 2023-05-31 20:52:54.870672 rockset_v2_internal-2.0.2/rockset_v2/model/view.py
+-rw-r--r--   0        0        0    18641 2023-05-31 20:52:54.871271 rockset_v2_internal-2.0.2/rockset_v2/model/virtual_instance.py
+-rw-r--r--   0        0        0    11778 2023-05-31 20:52:54.871892 rockset_v2_internal-2.0.2/rockset_v2/model/virtual_instance_stats.py
+-rw-r--r--   0        0        0    12977 2023-05-31 20:52:54.872539 rockset_v2_internal-2.0.2/rockset_v2/model/workspace.py
+-rw-r--r--   0        0        0    13004 2023-05-31 20:52:54.873194 rockset_v2_internal-2.0.2/rockset_v2/model/xml_params.py
+-rw-r--r--   0        0        0    84040 2023-05-31 20:52:54.874454 rockset_v2_internal-2.0.2/rockset_v2/model_utils.py
+-rw-r--r--   0        0        0    15316 2023-05-31 20:52:54.875183 rockset_v2_internal-2.0.2/rockset_v2/models/__init__.py
+-rw-r--r--   0        0        0     1819 2023-05-31 20:22:57.821569 rockset_v2_internal-2.0.2/rockset_v2/query_paginator.py
+-rw-r--r--   0        0        0    14648 2023-05-31 20:52:54.875917 rockset_v2_internal-2.0.2/rockset_v2/rest.py
+-rw-r--r--   0        0        0     8926 2023-05-31 20:52:54.876525 rockset_v2_internal-2.0.2/rockset_v2/rockset_client.py
+-rw-r--r--   0        0        0     3644 2023-05-31 20:22:57.826319 rockset_v2_internal-2.0.2/rockset_v2/value.py
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 rockset_v2_internal-2.0.2/PKG-INFO
```

### Comparing `rockset_v2_internal-2.0.1/pyproject.toml` & `rockset_v2_internal-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-name = "rockset-v2-internal"
-version = "2.0.1"
+name = "rockset_v2_internal"
+version = "2.0.2"
 description = "The python client for the Rockset API."
 authors = ["Rockset <support@rockset.com>"]
 packages = [
     {include = "rockset_v2"}
 ]
 documentation = "https://github.com/rockset/rockset-python-client"
 repository = "https://github.com/rockset/rockset-python-client"
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/__init__.py` & `rockset_v2_internal-2.0.2/rockset_v2/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,24 +9,24 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
-from rockset.api_client import ApiClient
+from rockset_v2.api_client import ApiClient
 
 # import Configuration
-from rockset.configuration import Configuration
+from rockset_v2.configuration import Configuration
 
 # import exceptions
-from rockset.exceptions import RocksetException
-from rockset.exceptions import ApiAttributeError
-from rockset.exceptions import ApiTypeError
-from rockset.exceptions import ApiValueError
-from rockset.exceptions import ApiKeyError
-from rockset.exceptions import ApiException
-from rockset.exceptions import BadRequestException
-
-from rockset.rockset_client import DevRegions, Regions, RocksetClient
-from rockset.document import Document
-from rockset.query_paginator import QueryPaginator
+from rockset_v2.exceptions import RocksetException
+from rockset_v2.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiTypeError
+from rockset_v2.exceptions import ApiValueError
+from rockset_v2.exceptions import ApiKeyError
+from rockset_v2.exceptions import ApiException
+from rockset_v2.exceptions import BadRequestException
+
+from rockset_v2.rockset_client import DevRegions, Regions, RocksetClient
+from rockset_v2.document import Document
+from rockset_v2.query_paginator import QueryPaginator
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/aliases_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/aliases_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.create_alias_request import CreateAliasRequest
-from rockset.model.create_alias_response import CreateAliasResponse
-from rockset.model.delete_alias_response import DeleteAliasResponse
-from rockset.model.error_model import ErrorModel
-from rockset.model.get_alias_response import GetAliasResponse
-from rockset.model.list_aliases_response import ListAliasesResponse
-from rockset.model.update_alias_request import UpdateAliasRequest
-from rockset.models import *
+from rockset_v2.model.create_alias_request import CreateAliasRequest
+from rockset_v2.model.create_alias_response import CreateAliasResponse
+from rockset_v2.model.delete_alias_response import DeleteAliasResponse
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.get_alias_response import GetAliasResponse
+from rockset_v2.model.list_aliases_response import ListAliasesResponse
+from rockset_v2.model.update_alias_request import UpdateAliasRequest
+from rockset_v2.models import *
 
 
 class Aliases(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -386,24 +386,24 @@
     ) -> typing.Union[CreateAliasResponse, asyncio.Future]:
         """Create Alias  # noqa: E501
 
         Create new alias in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Aliases.create(
-            collections=["commons.foo","prod.demo"],
-            description="version alias",
-            name="aliasName",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Aliases.create(
+    collections=["commons.foo","prod.demo"],
+    description="version alias",
+    name="aliasName",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             collections ([str]): List of fully qualified collection names referenced by alias.. [required]
             description (str): Optional description.. [optional]
             name (str): Alias name.. [required]
             _return_http_data_only (bool): response data without head status
@@ -479,22 +479,22 @@
     ) -> typing.Union[DeleteAliasResponse, asyncio.Future]:
         """Delete Alias  # noqa: E501
 
         Delete an alias.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Aliases.delete(
-            alias="alias_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Aliases.delete(
+    alias="alias_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             alias (str): name of the alias. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -568,22 +568,22 @@
     ) -> typing.Union[GetAliasResponse, asyncio.Future]:
         """Retrieve Alias  # noqa: E501
 
         Get details about an alias  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Aliases.get(
-            alias="alias_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Aliases.get(
+    alias="alias_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             alias (str): name of the alias. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -654,21 +654,21 @@
     ) -> typing.Union[ListAliasesResponse, asyncio.Future]:
         """List Aliases  # noqa: E501
 
         Retrieve all aliases in an organization  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Aliases.list(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Aliases.list(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -738,24 +738,24 @@
     ) -> typing.Union[GetAliasResponse, asyncio.Future]:
         """Update Alias  # noqa: E501
 
         Update alias in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Aliases.update(
-            alias="alias_example",
-            collections=["commons.foo","prod.demo"],
-            description="version alias",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Aliases.update(
+    alias="alias_example",
+    collections=["commons.foo","prod.demo"],
+    description="version alias",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             alias (str): name of the alias. [required]
             collections ([str]): List of fully qualified collection names referenced by alias.. [required]
             description (str): Optional description.. [optional]
             _return_http_data_only (bool): response data without head status
@@ -832,21 +832,21 @@
     ) -> typing.Union[ListAliasesResponse, asyncio.Future]:
         """List Aliases in Workspace  # noqa: E501
 
         Retrieve all aliases in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Aliases.workspace_aliases(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Aliases.workspace_aliases(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/api_keys_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/api_keys_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.create_api_key_request import CreateApiKeyRequest
-from rockset.model.create_api_key_response import CreateApiKeyResponse
-from rockset.model.delete_api_key_response import DeleteApiKeyResponse
-from rockset.model.error_model import ErrorModel
-from rockset.model.get_api_key_response import GetApiKeyResponse
-from rockset.model.list_api_keys_response import ListApiKeysResponse
-from rockset.model.update_api_key_request import UpdateApiKeyRequest
-from rockset.model.update_api_key_response import UpdateApiKeyResponse
-from rockset.models import *
+from rockset_v2.model.create_api_key_request import CreateApiKeyRequest
+from rockset_v2.model.create_api_key_response import CreateApiKeyResponse
+from rockset_v2.model.delete_api_key_response import DeleteApiKeyResponse
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.get_api_key_response import GetApiKeyResponse
+from rockset_v2.model.list_api_keys_response import ListApiKeysResponse
+from rockset_v2.model.update_api_key_request import UpdateApiKeyRequest
+from rockset_v2.model.update_api_key_response import UpdateApiKeyResponse
+from rockset_v2.models import *
 
 
 class APIKeys(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -341,24 +341,24 @@
     ) -> typing.Union[CreateApiKeyResponse, asyncio.Future]:
         """Create API Key  # noqa: E501
 
         Create a new API key for the authenticated user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.APIKeys.create(
-            created_by="string_example",
-            name="my-app",
-            role="string_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.APIKeys.create(
+    created_by="string_example",
+    name="my-app",
+    role="string_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             created_by (str): [optional]
             name (str): Name for this API key.. [required]
             role (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -431,23 +431,23 @@
     ) -> typing.Union[DeleteApiKeyResponse, asyncio.Future]:
         """Delete API Key  # noqa: E501
 
         Delete an API key for any user in your organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.APIKeys.delete(
-            name="my-key",
-            user="admin@me.com",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.APIKeys.delete(
+    name="my-key",
+    user="admin@me.com",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             name (str): Name of the API key.. [required]
             user (str): Email of the API key owner. Use `self` to specify the currently authenticated user.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -522,23 +522,23 @@
     ) -> typing.Union[GetApiKeyResponse, asyncio.Future]:
         """Retrieve API Key  # noqa: E501
 
         Retrieve a particular API key for any user in your organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.APIKeys.get(
-            user="admin@me.com",
-            name="my-key",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.APIKeys.get(
+    user="admin@me.com",
+    name="my-key",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             user (str): Email of the API key owner. Use `self` to specify the currently authenticated user.. [required]
             name (str): Name of the API key.. [required]
             reveal (bool): Reveal full key.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -615,22 +615,22 @@
     ) -> typing.Union[ListApiKeysResponse, asyncio.Future]:
         """List API Keys  # noqa: E501
 
         List API key metadata for any user in your organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.APIKeys.list(
-            user="admin@me.com",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.APIKeys.list(
+    user="admin@me.com",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             user (str): Email of the API key owner. Use `self` to specify the currently authenticated user.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -702,24 +702,24 @@
     ) -> typing.Union[UpdateApiKeyResponse, asyncio.Future]:
         """Update API Key State  # noqa: E501
 
         Update the state of an API key for any user in your organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.APIKeys.update(
-            name="my-key",
-            user="admin@me.com",
-            state="ACTIVE",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.APIKeys.update(
+    name="my-key",
+    user="admin@me.com",
+    state="ACTIVE",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             name (str): Name of the API key.. [required]
             user (str): Email of the API key owner. Use `self` to specify the currently authenticated user.. [required]
             state (str): State that the api key should be set to.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/collections_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/collections_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,41 +10,42 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.azure_blob_storage_collection_creation_request import AzureBlobStorageCollectionCreationRequest
-from rockset.model.azure_event_hubs_collection_creation_request import AzureEventHubsCollectionCreationRequest
-from rockset.model.azure_service_bus_collection_creation_request import AzureServiceBusCollectionCreationRequest
-from rockset.model.create_collection_response import CreateCollectionResponse
-from rockset.model.delete_collection_response import DeleteCollectionResponse
-from rockset.model.dynamodb_collection_creation_request import DynamodbCollectionCreationRequest
-from rockset.model.error_model import ErrorModel
-from rockset.model.file_upload_collection_creation_request import FileUploadCollectionCreationRequest
-from rockset.model.gcs_collection_creation_request import GcsCollectionCreationRequest
-from rockset.model.get_collection_response import GetCollectionResponse
-from rockset.model.kafka_collection_creation_request import KafkaCollectionCreationRequest
-from rockset.model.kinesis_collection_creation_request import KinesisCollectionCreationRequest
-from rockset.model.list_collections_response import ListCollectionsResponse
-from rockset.model.mongodb_collection_creation_request import MongodbCollectionCreationRequest
-from rockset.model.s3_collection_creation_request import S3CollectionCreationRequest
-from rockset.model.snowflake_collection_creation_request import SnowflakeCollectionCreationRequest
-from rockset.models import *
+from rockset_v2.model.azure_blob_storage_collection_creation_request import AzureBlobStorageCollectionCreationRequest
+from rockset_v2.model.azure_event_hubs_collection_creation_request import AzureEventHubsCollectionCreationRequest
+from rockset_v2.model.azure_service_bus_collection_creation_request import AzureServiceBusCollectionCreationRequest
+from rockset_v2.model.create_collection_response import CreateCollectionResponse
+from rockset_v2.model.delete_collection_response import DeleteCollectionResponse
+from rockset_v2.model.dynamodb_collection_creation_request import DynamodbCollectionCreationRequest
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.file_upload_collection_creation_request import FileUploadCollectionCreationRequest
+from rockset_v2.model.gcs_collection_creation_request import GcsCollectionCreationRequest
+from rockset_v2.model.get_collection_response import GetCollectionResponse
+from rockset_v2.model.kafka_collection_creation_request import KafkaCollectionCreationRequest
+from rockset_v2.model.kinesis_collection_creation_request import KinesisCollectionCreationRequest
+from rockset_v2.model.list_collections_response import ListCollectionsResponse
+from rockset_v2.model.mongodb_collection_creation_request import MongodbCollectionCreationRequest
+from rockset_v2.model.s3_collection_creation_request import S3CollectionCreationRequest
+from rockset_v2.model.snowflake_collection_creation_request import SnowflakeCollectionCreationRequest
+from rockset_v2.model.update_collection_request import UpdateCollectionRequest
+from rockset_v2.models import *
 
 
 class Collections(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -791,14 +792,77 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_0_endpoint = _Endpoint(
+            settings={
+                'response_type': (GetCollectionResponse,),
+                'auth': [
+                    'apikey'
+                ],
+                'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections/{collection}',
+                'operation_id': 'get_0',
+                'http_method': 'PUT',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'workspace',
+                    'collection',
+                    'update_collection_request',
+                ],
+                'required': [
+                    'workspace',
+                    'collection',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'workspace':
+                        (str,),
+                    'collection':
+                        (str,),
+                    'update_collection_request':
+                        (UpdateCollectionRequest,),
+                },
+                'attribute_map': {
+                    'workspace': 'workspace',
+                    'collection': 'collection',
+                },
+                'location_map': {
+                    'workspace': 'path',
+                    'collection': 'path',
+                    'update_collection_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.list_endpoint = _Endpoint(
             settings={
                 'response_type': (ListCollectionsResponse,),
                 'auth': [
                     'apikey'
                 ],
                 'endpoint_path': '/v1/orgs/self/collections',
@@ -895,113 +959,94 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[AzureBlobStorageSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create azure blob storage collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_azure_blob_storage_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                AzureBlobStorageSourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    container="server-logs",
-                    pattern="prefix/to/**/keys/*.format",
-                    prefix="prefix/to/blobs",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.create_azure_blob_storage_collection(
+    clustering_key=[
+        FieldPartition(
+            field_name="address.city.zipcode",
+            keys=["value1","value2"],
+            type="AUTO",
+        ),
+    ],
+    description="transactions from stores worldwide",
+    event_time_info=EventTimeInfo(
+        field="timestamp",
+        format="seconds_since_epoch",
+        time_zone="UTC",
+    ),
+    field_mapping_query=FieldMappingQuery(
+        sql="sql",
+    ),
+    name="global-transactions",
+    retention_secs=1000000,
+    sources=[
+        AzureBlobStorageSourceWrapper(
+            format_params=FormatParams(
+                csv=CsvParams(
+                    column_names=["c1","c2","c3"],
+                    column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
+                    encoding="UTF-8",
+                    escape_char="\\",
+                    first_line_as_column_names=True,
+                    quote_char="\"",
+                    separator=",",
+                ),
+                json=True,
+                mssql_dms=True,
+                mysql_dms=True,
+                oracle_dms=True,
+                postgres_dms=True,
+                xml=XmlParams(
+                    attribute_prefix="_attr",
+                    doc_tag="row",
+                    encoding="UTF-8",
+                    root_tag="root",
+                    value_tag="value",
+                ),
+            ),
+            integration_name="aws-integration",
+            container="server-logs",
+            pattern="prefix/to/**/keys/*.format",
+            prefix="prefix/to/blobs",
+        ),
+    ],
+    storage_compression_type="LZ4",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([AzureBlobStorageSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1066,112 +1111,93 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[AzureEventHubsSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create azure event hubs collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_azure_event_hubs_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                AzureEventHubsSourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    hub_id="event-hub-1",
-                    offset_reset_policy="EARLIEST",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.create_azure_event_hubs_collection(
+    clustering_key=[
+        FieldPartition(
+            field_name="address.city.zipcode",
+            keys=["value1","value2"],
+            type="AUTO",
+        ),
+    ],
+    description="transactions from stores worldwide",
+    event_time_info=EventTimeInfo(
+        field="timestamp",
+        format="seconds_since_epoch",
+        time_zone="UTC",
+    ),
+    field_mapping_query=FieldMappingQuery(
+        sql="sql",
+    ),
+    name="global-transactions",
+    retention_secs=1000000,
+    sources=[
+        AzureEventHubsSourceWrapper(
+            format_params=FormatParams(
+                csv=CsvParams(
+                    column_names=["c1","c2","c3"],
+                    column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
+                    encoding="UTF-8",
+                    escape_char="\\",
+                    first_line_as_column_names=True,
+                    quote_char="\"",
+                    separator=",",
+                ),
+                json=True,
+                mssql_dms=True,
+                mysql_dms=True,
+                oracle_dms=True,
+                postgres_dms=True,
+                xml=XmlParams(
+                    attribute_prefix="_attr",
+                    doc_tag="row",
+                    encoding="UTF-8",
+                    root_tag="root",
+                    value_tag="value",
+                ),
+            ),
+            integration_name="aws-integration",
+            hub_id="event-hub-1",
+            offset_reset_policy="EARLIEST",
+        ),
+    ],
+    storage_compression_type="LZ4",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([AzureEventHubsSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1236,112 +1262,93 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[AzureServiceBusSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create azure service bus collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_azure_service_bus_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                AzureServiceBusSourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    subscription="rockset-subscription",
-                    topic="rockset-topic",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.create_azure_service_bus_collection(
+    clustering_key=[
+        FieldPartition(
+            field_name="address.city.zipcode",
+            keys=["value1","value2"],
+            type="AUTO",
+        ),
+    ],
+    description="transactions from stores worldwide",
+    event_time_info=EventTimeInfo(
+        field="timestamp",
+        format="seconds_since_epoch",
+        time_zone="UTC",
+    ),
+    field_mapping_query=FieldMappingQuery(
+        sql="sql",
+    ),
+    name="global-transactions",
+    retention_secs=1000000,
+    sources=[
+        AzureServiceBusSourceWrapper(
+            format_params=FormatParams(
+                csv=CsvParams(
+                    column_names=["c1","c2","c3"],
+                    column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
+                    encoding="UTF-8",
+                    escape_char="\\",
+                    first_line_as_column_names=True,
+                    quote_char="\"",
+                    separator=",",
+                ),
+                json=True,
+                mssql_dms=True,
+                mysql_dms=True,
+                oracle_dms=True,
+                postgres_dms=True,
+                xml=XmlParams(
+                    attribute_prefix="_attr",
+                    doc_tag="row",
+                    encoding="UTF-8",
+                    root_tag="root",
+                    value_tag="value",
+                ),
+            ),
+            integration_name="aws-integration",
+            subscription="rockset-subscription",
+            topic="rockset-topic",
+        ),
+    ],
+    storage_compression_type="LZ4",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([AzureServiceBusSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1406,114 +1413,95 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[DynamodbSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create dynamodb collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_dynamodb_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                DynamodbSourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    aws_region="us-east-2",
-                    rcu=1000,
-                    table_name="dynamodb_table_name",
-                    use_scan_api=True,
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.create_dynamodb_collection(
+    clustering_key=[
+        FieldPartition(
+            field_name="address.city.zipcode",
+            keys=["value1","value2"],
+            type="AUTO",
+        ),
+    ],
+    description="transactions from stores worldwide",
+    event_time_info=EventTimeInfo(
+        field="timestamp",
+        format="seconds_since_epoch",
+        time_zone="UTC",
+    ),
+    field_mapping_query=FieldMappingQuery(
+        sql="sql",
+    ),
+    name="global-transactions",
+    retention_secs=1000000,
+    sources=[
+        DynamodbSourceWrapper(
+            format_params=FormatParams(
+                csv=CsvParams(
+                    column_names=["c1","c2","c3"],
+                    column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
+                    encoding="UTF-8",
+                    escape_char="\\",
+                    first_line_as_column_names=True,
+                    quote_char="\"",
+                    separator=",",
+                ),
+                json=True,
+                mssql_dms=True,
+                mysql_dms=True,
+                oracle_dms=True,
+                postgres_dms=True,
+                xml=XmlParams(
+                    attribute_prefix="_attr",
+                    doc_tag="row",
+                    encoding="UTF-8",
+                    root_tag="root",
+                    value_tag="value",
+                ),
+            ),
+            integration_name="aws-integration",
+            aws_region="us-east-2",
+            rcu=1000,
+            table_name="dynamodb_table_name",
+            use_scan_api=True,
+        ),
+    ],
+    storage_compression_type="LZ4",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([DynamodbSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1578,113 +1566,94 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[FileUploadSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create file upload collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_file_upload_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                FileUploadSourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    file_name="file1.json",
-                    file_size=12345,
-                    file_upload_time="2019-01-15T21:48:23Z",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.create_file_upload_collection(
+    clustering_key=[
+        FieldPartition(
+            field_name="address.city.zipcode",
+            keys=["value1","value2"],
+            type="AUTO",
+        ),
+    ],
+    description="transactions from stores worldwide",
+    event_time_info=EventTimeInfo(
+        field="timestamp",
+        format="seconds_since_epoch",
+        time_zone="UTC",
+    ),
+    field_mapping_query=FieldMappingQuery(
+        sql="sql",
+    ),
+    name="global-transactions",
+    retention_secs=1000000,
+    sources=[
+        FileUploadSourceWrapper(
+            format_params=FormatParams(
+                csv=CsvParams(
+                    column_names=["c1","c2","c3"],
+                    column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
+                    encoding="UTF-8",
+                    escape_char="\\",
+                    first_line_as_column_names=True,
+                    quote_char="\"",
+                    separator=",",
+                ),
+                json=True,
+                mssql_dms=True,
+                mysql_dms=True,
+                oracle_dms=True,
+                postgres_dms=True,
+                xml=XmlParams(
+                    attribute_prefix="_attr",
+                    doc_tag="row",
+                    encoding="UTF-8",
+                    root_tag="root",
+                    value_tag="value",
+                ),
+            ),
+            integration_name="aws-integration",
+            file_name="file1.json",
+            file_size=12345,
+            file_upload_time="2019-01-15T21:48:23Z",
+        ),
+    ],
+    storage_compression_type="LZ4",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([FileUploadSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1749,113 +1718,94 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[GcsSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create gcs collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_gcs_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                GcsSourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    bucket="server-logs",
-                    pattern="prefix/to/**/keys/*.format",
-                    prefix="prefix/to/keys",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.create_gcs_collection(
+    clustering_key=[
+        FieldPartition(
+            field_name="address.city.zipcode",
+            keys=["value1","value2"],
+            type="AUTO",
+        ),
+    ],
+    description="transactions from stores worldwide",
+    event_time_info=EventTimeInfo(
+        field="timestamp",
+        format="seconds_since_epoch",
+        time_zone="UTC",
+    ),
+    field_mapping_query=FieldMappingQuery(
+        sql="sql",
+    ),
+    name="global-transactions",
+    retention_secs=1000000,
+    sources=[
+        GcsSourceWrapper(
+            format_params=FormatParams(
+                csv=CsvParams(
+                    column_names=["c1","c2","c3"],
+                    column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
+                    encoding="UTF-8",
+                    escape_char="\\",
+                    first_line_as_column_names=True,
+                    quote_char="\"",
+                    separator=",",
+                ),
+                json=True,
+                mssql_dms=True,
+                mysql_dms=True,
+                oracle_dms=True,
+                postgres_dms=True,
+                xml=XmlParams(
+                    attribute_prefix="_attr",
+                    doc_tag="row",
+                    encoding="UTF-8",
+                    root_tag="root",
+                    value_tag="value",
+                ),
+            ),
+            integration_name="aws-integration",
+            bucket="server-logs",
+            pattern="prefix/to/**/keys/*.format",
+            prefix="prefix/to/keys",
+        ),
+    ],
+    storage_compression_type="LZ4",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([GcsSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1920,114 +1870,95 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[KafkaSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create kafka collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_kafka_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                KafkaSourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    consumer_group_id="org-collection",
-                    kafka_topic_name="example-topic",
-                    offset_reset_policy="EARLIEST",
-                    use_v3=True,
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.create_kafka_collection(
+    clustering_key=[
+        FieldPartition(
+            field_name="address.city.zipcode",
+            keys=["value1","value2"],
+            type="AUTO",
+        ),
+    ],
+    description="transactions from stores worldwide",
+    event_time_info=EventTimeInfo(
+        field="timestamp",
+        format="seconds_since_epoch",
+        time_zone="UTC",
+    ),
+    field_mapping_query=FieldMappingQuery(
+        sql="sql",
+    ),
+    name="global-transactions",
+    retention_secs=1000000,
+    sources=[
+        KafkaSourceWrapper(
+            format_params=FormatParams(
+                csv=CsvParams(
+                    column_names=["c1","c2","c3"],
+                    column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
+                    encoding="UTF-8",
+                    escape_char="\\",
+                    first_line_as_column_names=True,
+                    quote_char="\"",
+                    separator=",",
+                ),
+                json=True,
+                mssql_dms=True,
+                mysql_dms=True,
+                oracle_dms=True,
+                postgres_dms=True,
+                xml=XmlParams(
+                    attribute_prefix="_attr",
+                    doc_tag="row",
+                    encoding="UTF-8",
+                    root_tag="root",
+                    value_tag="value",
+                ),
+            ),
+            integration_name="aws-integration",
+            consumer_group_id="org-collection",
+            kafka_topic_name="example-topic",
+            offset_reset_policy="EARLIEST",
+            use_v3=True,
+        ),
+    ],
+    storage_compression_type="LZ4",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([KafkaSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2092,116 +2023,97 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[KinesisSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create kinesis collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_kinesis_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                KinesisSourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    aws_region="us-east-2",
-                    dms_primary_key=[
-                        "dms_primary_key_example",
-                    ],
-                    offset_reset_policy="EARLIEST",
-                    stream_name="click_stream",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.create_kinesis_collection(
+    clustering_key=[
+        FieldPartition(
+            field_name="address.city.zipcode",
+            keys=["value1","value2"],
+            type="AUTO",
+        ),
+    ],
+    description="transactions from stores worldwide",
+    event_time_info=EventTimeInfo(
+        field="timestamp",
+        format="seconds_since_epoch",
+        time_zone="UTC",
+    ),
+    field_mapping_query=FieldMappingQuery(
+        sql="sql",
+    ),
+    name="global-transactions",
+    retention_secs=1000000,
+    sources=[
+        KinesisSourceWrapper(
+            format_params=FormatParams(
+                csv=CsvParams(
+                    column_names=["c1","c2","c3"],
+                    column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
+                    encoding="UTF-8",
+                    escape_char="\\",
+                    first_line_as_column_names=True,
+                    quote_char="\"",
+                    separator=",",
+                ),
+                json=True,
+                mssql_dms=True,
+                mysql_dms=True,
+                oracle_dms=True,
+                postgres_dms=True,
+                xml=XmlParams(
+                    attribute_prefix="_attr",
+                    doc_tag="row",
+                    encoding="UTF-8",
+                    root_tag="root",
+                    value_tag="value",
+                ),
+            ),
+            integration_name="aws-integration",
+            aws_region="us-east-2",
+            dms_primary_key=[
+                "dms_primary_key_example",
+            ],
+            offset_reset_policy="EARLIEST",
+            stream_name="click_stream",
+        ),
+    ],
+    storage_compression_type="LZ4",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([KinesisSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2266,112 +2178,94 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[MongodbSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create mongodb collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_mongodb_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                MongodbSourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    collection_name="my_collection",
-                    database_name="my_database",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.create_mongodb_collection(
+    clustering_key=[
+        FieldPartition(
+            field_name="address.city.zipcode",
+            keys=["value1","value2"],
+            type="AUTO",
+        ),
+    ],
+    description="transactions from stores worldwide",
+    event_time_info=EventTimeInfo(
+        field="timestamp",
+        format="seconds_since_epoch",
+        time_zone="UTC",
+    ),
+    field_mapping_query=FieldMappingQuery(
+        sql="sql",
+    ),
+    name="global-transactions",
+    retention_secs=1000000,
+    sources=[
+        MongodbSourceWrapper(
+            format_params=FormatParams(
+                csv=CsvParams(
+                    column_names=["c1","c2","c3"],
+                    column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
+                    encoding="UTF-8",
+                    escape_char="\\",
+                    first_line_as_column_names=True,
+                    quote_char="\"",
+                    separator=",",
+                ),
+                json=True,
+                mssql_dms=True,
+                mysql_dms=True,
+                oracle_dms=True,
+                postgres_dms=True,
+                xml=XmlParams(
+                    attribute_prefix="_attr",
+                    doc_tag="row",
+                    encoding="UTF-8",
+                    root_tag="root",
+                    value_tag="value",
+                ),
+            ),
+            integration_name="aws-integration",
+            collection_name="my_collection",
+            database_name="my_database",
+            retrieve_full_document=True,
+        ),
+    ],
+    storage_compression_type="LZ4",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([MongodbSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2436,114 +2330,95 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[S3SourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create s3 collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_s3_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                S3SourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    bucket="s3://customer-account-info",
-                    pattern="prefix/to/**/keys/*.format",
-                    prefix="prefix/to/keys",
-                    region="us-west-2",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.create_s3_collection(
+    clustering_key=[
+        FieldPartition(
+            field_name="address.city.zipcode",
+            keys=["value1","value2"],
+            type="AUTO",
+        ),
+    ],
+    description="transactions from stores worldwide",
+    event_time_info=EventTimeInfo(
+        field="timestamp",
+        format="seconds_since_epoch",
+        time_zone="UTC",
+    ),
+    field_mapping_query=FieldMappingQuery(
+        sql="sql",
+    ),
+    name="global-transactions",
+    retention_secs=1000000,
+    sources=[
+        S3SourceWrapper(
+            format_params=FormatParams(
+                csv=CsvParams(
+                    column_names=["c1","c2","c3"],
+                    column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
+                    encoding="UTF-8",
+                    escape_char="\\",
+                    first_line_as_column_names=True,
+                    quote_char="\"",
+                    separator=",",
+                ),
+                json=True,
+                mssql_dms=True,
+                mysql_dms=True,
+                oracle_dms=True,
+                postgres_dms=True,
+                xml=XmlParams(
+                    attribute_prefix="_attr",
+                    doc_tag="row",
+                    encoding="UTF-8",
+                    root_tag="root",
+                    value_tag="value",
+                ),
+            ),
+            integration_name="aws-integration",
+            bucket="s3://customer-account-info",
+            pattern="prefix/to/**/keys/*.format",
+            prefix="prefix/to/keys",
+            region="us-west-2",
+        ),
+    ],
+    storage_compression_type="LZ4",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([S3SourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2608,114 +2483,95 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[SnowflakeSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create snowflake collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_snowflake_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                SnowflakeSourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    database="NASDAQ",
-                    schema="PUBLIC",
-                    table_name="COMPANIES",
-                    warehouse="COMPUTE_XL",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.create_snowflake_collection(
+    clustering_key=[
+        FieldPartition(
+            field_name="address.city.zipcode",
+            keys=["value1","value2"],
+            type="AUTO",
+        ),
+    ],
+    description="transactions from stores worldwide",
+    event_time_info=EventTimeInfo(
+        field="timestamp",
+        format="seconds_since_epoch",
+        time_zone="UTC",
+    ),
+    field_mapping_query=FieldMappingQuery(
+        sql="sql",
+    ),
+    name="global-transactions",
+    retention_secs=1000000,
+    sources=[
+        SnowflakeSourceWrapper(
+            format_params=FormatParams(
+                csv=CsvParams(
+                    column_names=["c1","c2","c3"],
+                    column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
+                    encoding="UTF-8",
+                    escape_char="\\",
+                    first_line_as_column_names=True,
+                    quote_char="\"",
+                    separator=",",
+                ),
+                json=True,
+                mssql_dms=True,
+                mysql_dms=True,
+                oracle_dms=True,
+                postgres_dms=True,
+                xml=XmlParams(
+                    attribute_prefix="_attr",
+                    doc_tag="row",
+                    encoding="UTF-8",
+                    root_tag="root",
+                    value_tag="value",
+                ),
+            ),
+            integration_name="aws-integration",
+            database="NASDAQ",
+            schema="PUBLIC",
+            table_name="COMPANIES",
+            warehouse="COMPUTE_XL",
+        ),
+    ],
+    storage_compression_type="LZ4",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([SnowflakeSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2785,22 +2641,22 @@
     ) -> typing.Union[DeleteCollectionResponse, asyncio.Future]:
         """Delete Collection  # noqa: E501
 
         Delete a collection and all its documents from Rockset.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.delete(
-            collection="collection_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.delete(
+    collection="collection_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             collection (str): name of the collection. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -2874,22 +2730,22 @@
     ) -> typing.Union[GetCollectionResponse, asyncio.Future]:
         """Retrieve Collection  # noqa: E501
 
         Get details about a collection.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.get(
-            collection="collection_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.get(
+    collection="collection_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             collection (str): name of the collection. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -2950,31 +2806,130 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['workspace'] = \
             workspace
         kwargs['collection'] = \
             collection
         return self.get_endpoint.call_with_http_info(**kwargs)
 
+    def get_0(
+        self,
+        *,
+        collection: str,
+        description: str = None,
+        field_mapping_query: FieldMappingQuery = None,
+        workspace = "commons",
+        **kwargs
+    ) -> typing.Union[GetCollectionResponse, asyncio.Future]:
+        """Update Collection  # noqa: E501
+
+        Update details about a collection.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.get_0(
+    collection="collection_example",
+    description="transactions from stores worldwide",
+    field_mapping_query=FieldMappingQuery(
+        sql="sql",
+    ),
+    async_req=True,
+)
+result = await future
+```
+
+        Keyword Args:
+            workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
+            collection (str): name of the collection. [required]
+            description (str): Updated text describing the collection.. [optional]
+            field_mapping_query (FieldMappingQuery): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done on the data received from the server.
+                If False, the client will also not convert nested inner objects
+                into the respective model types (the outermost object
+                is still converted to the model).
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            GetCollectionResponse
+                If the method is called asynchronously, returns an asyncio.Future which resolves to the response.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['workspace'] = \
+            workspace
+        kwargs['collection'] = \
+            collection
+        kwargs['update_collection_request'] = \
+            kwargs['update_collection_request']
+        return self.get_0_endpoint.call_with_http_info(**kwargs)
+
     def list(
         self,
         **kwargs
     ) -> typing.Union[ListCollectionsResponse, asyncio.Future]:
         """List Collections  # noqa: E501
 
         Retrieve all collections in an organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.list(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.list(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -3041,21 +2996,21 @@
     ) -> typing.Union[ListCollectionsResponse, asyncio.Future]:
         """List Collections in Workspace  # noqa: E501
 
         Retrieve all collections in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.workspace_collections(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Collections.workspace_collections(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -3138,7 +3093,9 @@
     return_types_dict['create_kinesis_collection'] = KinesisCollectionCreationRequest
     body_params_dict['create_mongodb_collection'] = 'mongodb_collection_creation_request'
     return_types_dict['create_mongodb_collection'] = MongodbCollectionCreationRequest
     body_params_dict['create_s3_collection'] = 's3_collection_creation_request'
     return_types_dict['create_s3_collection'] = S3CollectionCreationRequest
     body_params_dict['create_snowflake_collection'] = 'snowflake_collection_creation_request'
     return_types_dict['create_snowflake_collection'] = SnowflakeCollectionCreationRequest
+    body_params_dict['get_0'] = 'update_collection_request'
+    return_types_dict['get_0'] = UpdateCollectionRequest
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/custom_roles_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/custom_roles_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.create_role_request import CreateRoleRequest
-from rockset.model.error_model import ErrorModel
-from rockset.model.list_roles_response import ListRolesResponse
-from rockset.model.role_response import RoleResponse
-from rockset.model.update_role_request import UpdateRoleRequest
-from rockset.models import *
+from rockset_v2.model.create_role_request import CreateRoleRequest
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.list_roles_response import ListRolesResponse
+from rockset_v2.model.role_response import RoleResponse
+from rockset_v2.model.update_role_request import UpdateRoleRequest
+from rockset_v2.models import *
 
 
 class CustomRoles(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -308,30 +308,30 @@
     ) -> typing.Union[RoleResponse, asyncio.Future]:
         """Create a Role  # noqa: E501
 
         Create a role for your organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.CustomRoles.create(
-            description="Role with read and write privileges to all collections.",
-            privileges=[
-                Privilege(
-                    action="CREATE_COLLECTION_WS",
-                    cluster="*ALL*",
-                    resource_name="commons",
-                ),
-            ],
-            role_name="read_write",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.CustomRoles.create(
+    description="Role with read and write privileges to all collections.",
+    privileges=[
+        Privilege(
+            action="CREATE_COLLECTION_WS",
+            cluster="*ALL*",
+            resource_name="commons",
+        ),
+    ],
+    role_name="read_write",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             description (str): Description for the role.. [optional]
             privileges ([Privilege]): List of privileges that will be associated with the role.. [optional]
             role_name (str): Unique identifier for the role.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -403,22 +403,22 @@
     ) -> typing.Union[RoleResponse, asyncio.Future]:
         """Delete a Role  # noqa: E501
 
         Delete a role for your organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.CustomRoles.delete(
-            role_name="roleName_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.CustomRoles.delete(
+    role_name="roleName_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             role_name (str): [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -488,22 +488,22 @@
     ) -> typing.Union[RoleResponse, asyncio.Future]:
         """Retrieve role  # noqa: E501
 
         Retrieve a role by name for your organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.CustomRoles.get(
-            role_name="roleName_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.CustomRoles.get(
+    role_name="roleName_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             role_name (str): [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -571,21 +571,21 @@
     ) -> typing.Union[ListRolesResponse, asyncio.Future]:
         """List Roles  # noqa: E501
 
         List all roles for your organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.CustomRoles.list(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.CustomRoles.list(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -654,30 +654,30 @@
     ) -> typing.Union[RoleResponse, asyncio.Future]:
         """Update a Role  # noqa: E501
 
         Update a role for your organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.CustomRoles.update(
-            role_name="roleName_example",
-            description="Role with read and write privileges to all collections.",
-            privileges=[
-                Privilege(
-                    action="CREATE_COLLECTION_WS",
-                    cluster="*ALL*",
-                    resource_name="commons",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.CustomRoles.update(
+    role_name="roleName_example",
+    description="Role with read and write privileges to all collections.",
+    privileges=[
+        Privilege(
+            action="CREATE_COLLECTION_WS",
+            cluster="*ALL*",
+            resource_name="commons",
+        ),
+    ],
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             role_name (str): [required]
             description (str): Description for the role.. [optional]
             privileges ([Privilege]): List of privileges that will be associated with the role.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/documents_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/documents_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.add_documents_request import AddDocumentsRequest
-from rockset.model.add_documents_response import AddDocumentsResponse
-from rockset.model.delete_documents_request import DeleteDocumentsRequest
-from rockset.model.delete_documents_response import DeleteDocumentsResponse
-from rockset.model.error_model import ErrorModel
-from rockset.model.patch_documents_request import PatchDocumentsRequest
-from rockset.model.patch_documents_response import PatchDocumentsResponse
-from rockset.models import *
+from rockset_v2.model.add_documents_request import AddDocumentsRequest
+from rockset_v2.model.add_documents_response import AddDocumentsResponse
+from rockset_v2.model.delete_documents_request import DeleteDocumentsRequest
+from rockset_v2.model.delete_documents_response import DeleteDocumentsResponse
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.patch_documents_request import PatchDocumentsRequest
+from rockset_v2.model.patch_documents_response import PatchDocumentsResponse
+from rockset_v2.models import *
 
 
 class Documents(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -245,23 +245,23 @@
     ) -> typing.Union[AddDocumentsResponse, asyncio.Future]:
         """Add Documents  # noqa: E501
 
         Add documents to a collection.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Documents.add_documents(
-            collection="collection_example",
-            data=[{"field":"value"}],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Documents.add_documents(
+    collection="collection_example",
+    data=[{"field":"value"}],
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): Name of the workspace.. [required] if omitted the server will use the default value of "commons"
             collection (str): Name of the collection.. [required]
             data ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): Array of documents to be added to the collection.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -339,27 +339,27 @@
     ) -> typing.Union[DeleteDocumentsResponse, asyncio.Future]:
         """Delete Documents  # noqa: E501
 
         Delete documents from a collection.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Documents.delete_documents(
-            collection="collection_example",
-            data=[
-                DeleteDocumentsRequestData(
-                    id="2cd61e3b",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Documents.delete_documents(
+    collection="collection_example",
+    data=[
+        DeleteDocumentsRequestData(
+            id="2cd61e3b",
+        ),
+    ],
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): Name of the workspace.. [required] if omitted the server will use the default value of "commons"
             collection (str): Name of the collection.. [required]
             data ([DeleteDocumentsRequestData]): Array of IDs of documents to be deleted.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -437,35 +437,35 @@
     ) -> typing.Union[PatchDocumentsResponse, asyncio.Future]:
         """Patch Documents  # noqa: E501
 
         Update existing documents in a collection.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Documents.patch_documents(
-            collection="collection_example",
-            data=[
-                PatchDocument(
-                    id="ca2d6832-1bfd-f88f-0620-d2aa27a5d86c",
-                    patch=[
-                        PatchOperation(
-                            _from="_from_example",
-                            op="ADD",
-                            path="/foo/bar",
-                            value={},
-                        ),
-                    ],
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Documents.patch_documents(
+    collection="collection_example",
+    data=[
+        PatchDocument(
+            id="ca2d6832-1bfd-f88f-0620-d2aa27a5d86c",
+            patch=[
+                PatchOperation(
+                    _from="_from_example",
+                    op="ADD",
+                    path="/foo/bar",
+                    value={},
                 ),
             ],
-            async_req=True,
-        )
-        result = await future
-        ```
+        ),
+    ],
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): Name of the workspace.. [required] if omitted the server will use the default value of "commons"
             collection (str): Name of the collection.. [required]
             data ([PatchDocument]): List of patches to be applied.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/integrations_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/integrations_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,39 +10,39 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.azure_blob_storage_integration_creation_request import AzureBlobStorageIntegrationCreationRequest
-from rockset.model.azure_event_hubs_integration_creation_request import AzureEventHubsIntegrationCreationRequest
-from rockset.model.create_integration_response import CreateIntegrationResponse
-from rockset.model.delete_integration_response import DeleteIntegrationResponse
-from rockset.model.dynamodb_integration_creation_request import DynamodbIntegrationCreationRequest
-from rockset.model.error_model import ErrorModel
-from rockset.model.gcs_integration_creation_request import GcsIntegrationCreationRequest
-from rockset.model.get_integration_response import GetIntegrationResponse
-from rockset.model.kafka_integration_creation_request import KafkaIntegrationCreationRequest
-from rockset.model.kinesis_integration_creation_request import KinesisIntegrationCreationRequest
-from rockset.model.list_integrations_response import ListIntegrationsResponse
-from rockset.model.mongodb_integration_creation_request import MongodbIntegrationCreationRequest
-from rockset.model.s3_integration_creation_request import S3IntegrationCreationRequest
-from rockset.model.snowflake_integration_creation_request import SnowflakeIntegrationCreationRequest
-from rockset.models import *
+from rockset_v2.model.azure_blob_storage_integration_creation_request import AzureBlobStorageIntegrationCreationRequest
+from rockset_v2.model.azure_event_hubs_integration_creation_request import AzureEventHubsIntegrationCreationRequest
+from rockset_v2.model.create_integration_response import CreateIntegrationResponse
+from rockset_v2.model.delete_integration_response import DeleteIntegrationResponse
+from rockset_v2.model.dynamodb_integration_creation_request import DynamodbIntegrationCreationRequest
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.gcs_integration_creation_request import GcsIntegrationCreationRequest
+from rockset_v2.model.get_integration_response import GetIntegrationResponse
+from rockset_v2.model.kafka_integration_creation_request import KafkaIntegrationCreationRequest
+from rockset_v2.model.kinesis_integration_creation_request import KinesisIntegrationCreationRequest
+from rockset_v2.model.list_integrations_response import ListIntegrationsResponse
+from rockset_v2.model.mongodb_integration_creation_request import MongodbIntegrationCreationRequest
+from rockset_v2.model.s3_integration_creation_request import S3IntegrationCreationRequest
+from rockset_v2.model.snowflake_integration_creation_request import SnowflakeIntegrationCreationRequest
+from rockset_v2.models import *
 
 
 class Integrations(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -668,27 +668,27 @@
     ) -> typing.Union[CreateIntegrationResponse, asyncio.Future]:
         """Create azure blob storage integration  # noqa: E501
 
         Create a new integration.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Integrations.create_azure_blob_storage_integration(
-            azure_blob_storage=AzureBlobStorageIntegration(
-                connection_string='''BlobEndpoint=https://<NamespaceName>.blob.core.windows.net;
-        SharedAccessSignature=<KeyValue>''',
-            ),
-            description="AWS account with event data for the data science team.",
-            name="event-logs",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Integrations.create_azure_blob_storage_integration(
+    azure_blob_storage=AzureBlobStorageIntegration(
+        connection_string='''BlobEndpoint=https://<NamespaceName>.blob.core.windows.net;
+SharedAccessSignature=<KeyValue>''',
+    ),
+    description="AWS account with event data for the data science team.",
+    name="event-logs",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             azure_blob_storage (AzureBlobStorageIntegration): [optional]
             description (str): Longer explanation for the integration.. [optional]
             name (str): Descriptive label.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -762,26 +762,26 @@
     ) -> typing.Union[CreateIntegrationResponse, asyncio.Future]:
         """Create azure event hubs integration  # noqa: E501
 
         Create a new integration.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Integrations.create_azure_event_hubs_integration(
-            azure_event_hubs=AzureEventHubsIntegration(
-                connection_string="Endpoint=sb://<NamespaceName>.servicebus.windows.net/;SharedAccessKeyName=<KeyName>;SharedAccessKey=<KeyValue>",
-            ),
-            description="AWS account with event data for the data science team.",
-            name="event-logs",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Integrations.create_azure_event_hubs_integration(
+    azure_event_hubs=AzureEventHubsIntegration(
+        connection_string="Endpoint=sb://<NamespaceName>.servicebus.windows.net/;SharedAccessKeyName=<KeyName>;SharedAccessKey=<KeyValue>",
+    ),
+    description="AWS account with event data for the data science team.",
+    name="event-logs",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             azure_event_hubs (AzureEventHubsIntegration): [optional]
             description (str): Longer explanation for the integration.. [optional]
             name (str): Descriptive label.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -855,34 +855,34 @@
     ) -> typing.Union[CreateIntegrationResponse, asyncio.Future]:
         """Create dynamodb integration  # noqa: E501
 
         Create a new integration.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Integrations.create_dynamodb_integration(
-            description="AWS account with event data for the data science team.",
-            dynamodb=DynamodbIntegration(
-                aws_access_key=AwsAccessKey(
-                    aws_access_key_id="AKIAIOSFODNN7EXAMPLE",
-                    aws_secret_access_key="wJal....",
-                ),
-                aws_role=AwsRole(
-                    aws_external_id="external id of aws",
-                    aws_role_arn="arn:aws:iam::2378964092:role/rockset-role",
-                ),
-                s3_export_bucket_name="s3_export_bucket_name_example",
-            ),
-            name="event-logs",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Integrations.create_dynamodb_integration(
+    description="AWS account with event data for the data science team.",
+    dynamodb=DynamodbIntegration(
+        aws_access_key=AwsAccessKey(
+            aws_access_key_id="AKIAIOSFODNN7EXAMPLE",
+            aws_secret_access_key="wJal....",
+        ),
+        aws_role=AwsRole(
+            aws_external_id="external id of aws",
+            aws_role_arn="arn:aws:iam::2378964092:role/rockset-role",
+        ),
+        s3_export_bucket_name="s3_export_bucket_name_example",
+    ),
+    name="event-logs",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             description (str): Longer explanation for the integration.. [optional]
             dynamodb (DynamodbIntegration): [optional]
             name (str): Descriptive label.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -956,28 +956,28 @@
     ) -> typing.Union[CreateIntegrationResponse, asyncio.Future]:
         """Create gcs integration  # noqa: E501
 
         Create a new integration.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Integrations.create_gcs_integration(
-            description="AWS account with event data for the data science team.",
-            gcs=GcsIntegration(
-                gcp_service_account=GcpServiceAccount(
-                    service_account_key_file_json="service_account_key_file_json_example",
-                ),
-            ),
-            name="event-logs",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Integrations.create_gcs_integration(
+    description="AWS account with event data for the data science team.",
+    gcs=GcsIntegration(
+        gcp_service_account=GcpServiceAccount(
+            service_account_key_file_json="service_account_key_file_json_example",
+        ),
+    ),
+    name="event-logs",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             description (str): Longer explanation for the integration.. [optional]
             gcs (GcsIntegration): [optional]
             name (str): Descriptive label.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -1051,45 +1051,45 @@
     ) -> typing.Union[CreateIntegrationResponse, asyncio.Future]:
         """Create kafka integration  # noqa: E501
 
         Create a new integration.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Integrations.create_kafka_integration(
-            description="AWS account with event data for the data science team.",
-            kafka=KafkaIntegration(
-                aws_role=AwsRole(
-                    aws_external_id="external id of aws",
-                    aws_role_arn="arn:aws:iam::2378964092:role/rockset-role",
-                ),
-                bootstrap_servers="localhost:9092",
-                connection_string="connection_string_example",
-                kafka_data_format="JSON",
-                kafka_topic_names=[
-                    "kafka_topic_names_example",
-                ],
-                schema_registry_config=SchemaRegistryConfig(
-                    key="key_example",
-                    secret="secret_example",
-                    url="url_example",
-                ),
-                security_config=KafkaV3SecurityConfig(
-                    api_key="api_key_example",
-                    secret="secret_example",
-                ),
-                use_v3=True,
-            ),
-            name="event-logs",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Integrations.create_kafka_integration(
+    description="AWS account with event data for the data science team.",
+    kafka=KafkaIntegration(
+        aws_role=AwsRole(
+            aws_external_id="external id of aws",
+            aws_role_arn="arn:aws:iam::2378964092:role/rockset-role",
+        ),
+        bootstrap_servers="localhost:9092",
+        connection_string="connection_string_example",
+        kafka_data_format="JSON",
+        kafka_topic_names=[
+            "kafka_topic_names_example",
+        ],
+        schema_registry_config=SchemaRegistryConfig(
+            key="key_example",
+            secret="secret_example",
+            url="url_example",
+        ),
+        security_config=KafkaV3SecurityConfig(
+            api_key="api_key_example",
+            secret="secret_example",
+        ),
+        use_v3=True,
+    ),
+    name="event-logs",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             description (str): Longer explanation for the integration.. [optional]
             kafka (KafkaIntegration): [optional]
             name (str): Descriptive label.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -1163,33 +1163,33 @@
     ) -> typing.Union[CreateIntegrationResponse, asyncio.Future]:
         """Create kinesis integration  # noqa: E501
 
         Create a new integration.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Integrations.create_kinesis_integration(
-            description="AWS account with event data for the data science team.",
-            kinesis=KinesisIntegration(
-                aws_access_key=AwsAccessKey(
-                    aws_access_key_id="AKIAIOSFODNN7EXAMPLE",
-                    aws_secret_access_key="wJal....",
-                ),
-                aws_role=AwsRole(
-                    aws_external_id="external id of aws",
-                    aws_role_arn="arn:aws:iam::2378964092:role/rockset-role",
-                ),
-            ),
-            name="event-logs",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Integrations.create_kinesis_integration(
+    description="AWS account with event data for the data science team.",
+    kinesis=KinesisIntegration(
+        aws_access_key=AwsAccessKey(
+            aws_access_key_id="AKIAIOSFODNN7EXAMPLE",
+            aws_secret_access_key="wJal....",
+        ),
+        aws_role=AwsRole(
+            aws_external_id="external id of aws",
+            aws_role_arn="arn:aws:iam::2378964092:role/rockset-role",
+        ),
+    ),
+    name="event-logs",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             description (str): Longer explanation for the integration.. [optional]
             kinesis (KinesisIntegration): [optional]
             name (str): Descriptive label.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -1263,26 +1263,26 @@
     ) -> typing.Union[CreateIntegrationResponse, asyncio.Future]:
         """Create mongodb integration  # noqa: E501
 
         Create a new integration.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Integrations.create_mongodb_integration(
-            description="AWS account with event data for the data science team.",
-            mongodb=MongoDbIntegration(
-                connection_uri="mongodb+srv://<username>:<password>@server.example.com/",
-            ),
-            name="event-logs",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Integrations.create_mongodb_integration(
+    description="AWS account with event data for the data science team.",
+    mongodb=MongoDbIntegration(
+        connection_uri="mongodb+srv://<username>:<password>@server.example.com/",
+    ),
+    name="event-logs",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             description (str): Longer explanation for the integration.. [optional]
             mongodb (MongoDbIntegration): [optional]
             name (str): Descriptive label.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -1356,33 +1356,33 @@
     ) -> typing.Union[CreateIntegrationResponse, asyncio.Future]:
         """Create s3 integration  # noqa: E501
 
         Create a new integration.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Integrations.create_s3_integration(
-            description="AWS account with event data for the data science team.",
-            name="event-logs",
-            s3=S3Integration(
-                aws_access_key=AwsAccessKey(
-                    aws_access_key_id="AKIAIOSFODNN7EXAMPLE",
-                    aws_secret_access_key="wJal....",
-                ),
-                aws_role=AwsRole(
-                    aws_external_id="external id of aws",
-                    aws_role_arn="arn:aws:iam::2378964092:role/rockset-role",
-                ),
-            ),
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Integrations.create_s3_integration(
+    description="AWS account with event data for the data science team.",
+    name="event-logs",
+    s3=S3Integration(
+        aws_access_key=AwsAccessKey(
+            aws_access_key_id="AKIAIOSFODNN7EXAMPLE",
+            aws_secret_access_key="wJal....",
+        ),
+        aws_role=AwsRole(
+            aws_external_id="external id of aws",
+            aws_role_arn="arn:aws:iam::2378964092:role/rockset-role",
+        ),
+    ),
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             description (str): Longer explanation for the integration.. [optional]
             name (str): Descriptive label.. [required]
             s3 (S3Integration): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -1456,39 +1456,39 @@
     ) -> typing.Union[CreateIntegrationResponse, asyncio.Future]:
         """Create snowflake integration  # noqa: E501
 
         Create a new integration.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Integrations.create_snowflake_integration(
-            description="AWS account with event data for the data science team.",
-            name="event-logs",
-            snowflake=SnowflakeIntegration(
-                aws_access_key=AwsAccessKey(
-                    aws_access_key_id="AKIAIOSFODNN7EXAMPLE",
-                    aws_secret_access_key="wJal....",
-                ),
-                aws_role=AwsRole(
-                    aws_external_id="external id of aws",
-                    aws_role_arn="arn:aws:iam::2378964092:role/rockset-role",
-                ),
-                default_warehouse="default_warehouse_example",
-                password="password_example",
-                s3_export_path="s3://bucket/prefix",
-                snowflake_url="acme-marketing-test-account.snowflakecomputing.com",
-                user_role="user_role_example",
-                username="username_example",
-            ),
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Integrations.create_snowflake_integration(
+    description="AWS account with event data for the data science team.",
+    name="event-logs",
+    snowflake=SnowflakeIntegration(
+        aws_access_key=AwsAccessKey(
+            aws_access_key_id="AKIAIOSFODNN7EXAMPLE",
+            aws_secret_access_key="wJal....",
+        ),
+        aws_role=AwsRole(
+            aws_external_id="external id of aws",
+            aws_role_arn="arn:aws:iam::2378964092:role/rockset-role",
+        ),
+        default_warehouse="default_warehouse_example",
+        password="password_example",
+        s3_export_path="s3://bucket/prefix",
+        snowflake_url="acme-marketing-test-account.snowflakecomputing.com",
+        user_role="user_role_example",
+        username="username_example",
+    ),
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             description (str): Longer explanation for the integration.. [optional]
             name (str): Descriptive label.. [required]
             snowflake (SnowflakeIntegration): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -1560,22 +1560,22 @@
     ) -> typing.Union[DeleteIntegrationResponse, asyncio.Future]:
         """Delete Integration  # noqa: E501
 
         Remove an integration.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Integrations.delete(
-            integration="integration_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Integrations.delete(
+    integration="integration_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             integration (str): name of the integration. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -1645,22 +1645,22 @@
     ) -> typing.Union[GetIntegrationResponse, asyncio.Future]:
         """Retrieve Integration  # noqa: E501
 
         Retrieve information about a single integration.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Integrations.get(
-            integration="integration_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Integrations.get(
+    integration="integration_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             integration (str): name of the integration. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -1728,21 +1728,21 @@
     ) -> typing.Union[ListIntegrationsResponse, asyncio.Future]:
         """List Integrations  # noqa: E501
 
         List all integrations in an organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Integrations.list(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Integrations.list(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/organizations_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/organizations_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.error_model import ErrorModel
-from rockset.model.organization_response import OrganizationResponse
-from rockset.models import *
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.organization_response import OrganizationResponse
+from rockset_v2.models import *
 
 
 class Organizations(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -91,21 +91,21 @@
     ) -> typing.Union[OrganizationResponse, asyncio.Future]:
         """Get Organization  # noqa: E501
 
         Retrieve information about current organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Organizations.get(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Organizations.get(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/queries_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/queries_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.cancel_query_response import CancelQueryResponse
-from rockset.model.error_model import ErrorModel
-from rockset.model.get_query_response import GetQueryResponse
-from rockset.model.list_queries_response import ListQueriesResponse
-from rockset.model.query_pagination_response import QueryPaginationResponse
-from rockset.model.query_request import QueryRequest
-from rockset.model.query_response import QueryResponse
-from rockset.model.validate_query_response import ValidateQueryResponse
-from rockset.models import *
+from rockset_v2.model.cancel_query_response import CancelQueryResponse
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.get_query_response import GetQueryResponse
+from rockset_v2.model.list_queries_response import ListQueriesResponse
+from rockset_v2.model.query_pagination_response import QueryPaginationResponse
+from rockset_v2.model.query_request import QueryRequest
+from rockset_v2.model.query_response import QueryResponse
+from rockset_v2.model.validate_query_response import ValidateQueryResponse
+from rockset_v2.models import *
 
 
 class Queries(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -369,22 +369,22 @@
     ) -> typing.Union[CancelQueryResponse, asyncio.Future]:
         """Cancel Query  # noqa: E501
 
         Attempts to cancel an actively-running query.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Queries.cancel_query(
-            query_id="queryId_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Queries.cancel_query(
+    query_id="queryId_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             query_id (str): [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -454,22 +454,22 @@
     ) -> typing.Union[GetQueryResponse, asyncio.Future]:
         """Retrieve Query  # noqa: E501
 
         Returns information about a query.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Queries.get_query(
-            query_id="queryId_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Queries.get_query(
+    query_id="queryId_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             query_id (str): [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -542,22 +542,22 @@
     ) -> typing.Union[QueryPaginationResponse, asyncio.Future]:
         """Retrieve Query Results Page  # noqa: E501
 
         Returns a page of query results.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Queries.get_query_results(
-            query_id="queryId_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Queries.get_query_results(
+    query_id="queryId_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             query_id (str): [required]
             cursor (str): Cursor to current page. If unset, will default to the first page.. [optional]
             docs (int): Number of documents to fetch.. [optional]
             offset (int): Offset from the cursor of the first document to be returned. [optional]
             _return_http_data_only (bool): response data without head status
@@ -637,21 +637,21 @@
     ) -> typing.Union[ListQueriesResponse, asyncio.Future]:
         """List Queries  # noqa: E501
 
         Lists actively queued and running queries.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Queries.list_active_queries(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Queries.list_active_queries(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -711,52 +711,54 @@
         return self.list_active_queries_endpoint.call_with_http_info(**kwargs)
 
     def query(
         self,
         *,
         sql: QueryRequestSql,
         async_options: AsyncQueryOptions = None,
+        timeout_ms: int = None,
         **kwargs
     ) -> typing.Union[QueryResponse, asyncio.Future]:
         """Execute SQL Query  # noqa: E501
 
         Make a SQL query to Rockset.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Queries.query(
-            async_options=AsyncQueryOptions(
-                client_timeout_ms=1,
-                max_initial_results=1,
-                timeout_ms=1,
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Queries.query(
+    async_options=AsyncQueryOptions(
+        client_timeout_ms=1,
+        max_initial_results=1,
+        timeout_ms=1,
+    ),
+    sql=QueryRequestSql(
+        default_row_limit=1,
+        generate_warnings=False,
+        initial_paginate_response_doc_count=1,
+        parameters=[
+            QueryParameter(
+                name="_id",
+                type="string",
+                value="85beb391",
             ),
-            sql=QueryRequestSql(
-                default_row_limit=1,
-                generate_warnings=False,
-                initial_paginate_response_doc_count=1,
-                paginate=True,
-                parameters=[
-                    QueryParameter(
-                        name="_id",
-                        type="string",
-                        value="85beb391",
-                    ),
-                ],
-                query="SELECT * FROM foo where _id = :_id",
-            ),
-            async_req=True,
-        )
-        result = await future
-        ```
+        ],
+        query="SELECT * FROM foo where _id = :_id",
+    ),
+    timeout_ms=1,
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             async_options (AsyncQueryOptions): [optional]
             sql (QueryRequestSql): [required]
+            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error. The maximum value for this timeout is 2 minutes. async_options.timeout_ms will override this timeout.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -816,52 +818,54 @@
         return self.query_endpoint.call_with_http_info(**kwargs)
 
     def validate(
         self,
         *,
         sql: QueryRequestSql,
         async_options: AsyncQueryOptions = None,
+        timeout_ms: int = None,
         **kwargs
     ) -> typing.Union[ValidateQueryResponse, asyncio.Future]:
         """Validate Query  # noqa: E501
 
         Validate a SQL query with Rockset's parser and planner.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Queries.validate(
-            async_options=AsyncQueryOptions(
-                client_timeout_ms=1,
-                max_initial_results=1,
-                timeout_ms=1,
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Queries.validate(
+    async_options=AsyncQueryOptions(
+        client_timeout_ms=1,
+        max_initial_results=1,
+        timeout_ms=1,
+    ),
+    sql=QueryRequestSql(
+        default_row_limit=1,
+        generate_warnings=False,
+        initial_paginate_response_doc_count=1,
+        parameters=[
+            QueryParameter(
+                name="_id",
+                type="string",
+                value="85beb391",
             ),
-            sql=QueryRequestSql(
-                default_row_limit=1,
-                generate_warnings=False,
-                initial_paginate_response_doc_count=1,
-                paginate=True,
-                parameters=[
-                    QueryParameter(
-                        name="_id",
-                        type="string",
-                        value="85beb391",
-                    ),
-                ],
-                query="SELECT * FROM foo where _id = :_id",
-            ),
-            async_req=True,
-        )
-        result = await future
-        ```
+        ],
+        query="SELECT * FROM foo where _id = :_id",
+    ),
+    timeout_ms=1,
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             async_options (AsyncQueryOptions): [optional]
             sql (QueryRequestSql): [required]
+            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error. The maximum value for this timeout is 2 minutes. async_options.timeout_ms will override this timeout.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/query_lambdas_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/query_lambdas_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,37 +10,37 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.create_query_lambda_request import CreateQueryLambdaRequest
-from rockset.model.create_query_lambda_tag_request import CreateQueryLambdaTagRequest
-from rockset.model.delete_query_lambda_response import DeleteQueryLambdaResponse
-from rockset.model.error_model import ErrorModel
-from rockset.model.execute_query_lambda_request import ExecuteQueryLambdaRequest
-from rockset.model.list_query_lambda_tags_response import ListQueryLambdaTagsResponse
-from rockset.model.list_query_lambda_versions_response import ListQueryLambdaVersionsResponse
-from rockset.model.list_query_lambdas_response import ListQueryLambdasResponse
-from rockset.model.query_lambda_tag_response import QueryLambdaTagResponse
-from rockset.model.query_lambda_version_response import QueryLambdaVersionResponse
-from rockset.model.query_response import QueryResponse
-from rockset.model.update_query_lambda_request import UpdateQueryLambdaRequest
-from rockset.models import *
+from rockset_v2.model.create_query_lambda_request import CreateQueryLambdaRequest
+from rockset_v2.model.create_query_lambda_tag_request import CreateQueryLambdaTagRequest
+from rockset_v2.model.delete_query_lambda_response import DeleteQueryLambdaResponse
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.execute_query_lambda_request import ExecuteQueryLambdaRequest
+from rockset_v2.model.list_query_lambda_tags_response import ListQueryLambdaTagsResponse
+from rockset_v2.model.list_query_lambda_versions_response import ListQueryLambdaVersionsResponse
+from rockset_v2.model.list_query_lambdas_response import ListQueryLambdasResponse
+from rockset_v2.model.query_lambda_tag_response import QueryLambdaTagResponse
+from rockset_v2.model.query_lambda_version_response import QueryLambdaVersionResponse
+from rockset_v2.model.query_response import QueryResponse
+from rockset_v2.model.update_query_lambda_request import UpdateQueryLambdaRequest
+from rockset_v2.models import *
 
 
 class QueryLambdas(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -907,34 +907,34 @@
     ) -> typing.Union[QueryLambdaVersionResponse, asyncio.Future]:
         """Create Query Lambda  # noqa: E501
 
         Create a Query Lambda in given workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.create_query_lambda(
-            description="production version foo",
-            is_public=True,
-            name="myQueryLambda",
-            sql=QueryLambdaSql(
-                default_parameters=[
-                    QueryParameter(
-                        name="_id",
-                        type="string",
-                        value="85beb391",
-                    ),
-                ],
-                query="SELECT 'Foo'",
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.create_query_lambda(
+    description="production version foo",
+    is_public=True,
+    name="myQueryLambda",
+    sql=QueryLambdaSql(
+        default_parameters=[
+            QueryParameter(
+                name="_id",
+                type="string",
+                value="85beb391",
             ),
-            async_req=True,
-        )
-        result = await future
-        ```
+        ],
+        query="SELECT 'Foo'",
+    ),
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             description (str): Optional description.. [optional]
             is_public (bool): [optional]
             name (str): Query Lambda name.. [required]
             sql (QueryLambdaSql): [optional]
@@ -1013,24 +1013,24 @@
     ) -> typing.Union[QueryLambdaTagResponse, asyncio.Future]:
         """Create Query Lambda Tag  # noqa: E501
 
         Create a tag for a specific Query Lambda version, or update that tag if it already exists.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.create_query_lambda_tag(
-            query_lambda="queryLambda_example",
-            tag_name="production",
-            version="123ABC",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.create_query_lambda_tag(
+    query_lambda="queryLambda_example",
+    tag_name="production",
+    version="123ABC",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             query_lambda (str): name of the Query Lambda. [required]
             tag_name (str): Name of Query Lambda tag.. [required]
             version (str): Hash identifying a Query Lambda tag.. [required]
             _return_http_data_only (bool): response data without head status
@@ -1108,22 +1108,22 @@
     ) -> typing.Union[DeleteQueryLambdaResponse, asyncio.Future]:
         """Delete Query Lambda  # noqa: E501
 
         Delete a Query Lambda.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.delete_query_lambda(
-            query_lambda="queryLambda_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.delete_query_lambda(
+    query_lambda="queryLambda_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             query_lambda (str): name of the Query Lambda. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -1198,23 +1198,23 @@
     ) -> typing.Union[QueryLambdaTagResponse, asyncio.Future]:
         """Delete Query Lambda Tag Version  # noqa: E501
 
         Delete a tag for a specific Query Lambda  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.delete_query_lambda_tag(
-            query_lambda="queryLambda_example",
-            tag="tag_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.delete_query_lambda_tag(
+    query_lambda="queryLambda_example",
+    tag="tag_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             query_lambda (str): name of the Query Lambda. [required]
             tag (str): name of the tag. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -1292,23 +1292,23 @@
     ) -> typing.Union[QueryLambdaVersionResponse, asyncio.Future]:
         """Delete Query Lambda Version  # noqa: E501
 
         Delete a Query Lambda version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.delete_query_lambda_version(
-            query_lambda="queryLambda_example",
-            version="version_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.delete_query_lambda_version(
+    query_lambda="queryLambda_example",
+    version="version_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             query_lambda (str): name of the Query Lambda. [required]
             version (str): version. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -1384,32 +1384,33 @@
         workspace = "commons",
         async_options: AsyncQueryOptions = None,
         default_row_limit: int = None,
         generate_warnings: bool = None,
         initial_paginate_response_doc_count: int = None,
         paginate: bool = None,
         parameters: typing.Sequence[QueryParameter] = None,
+        timeout_ms: int = None,
         virtual_instance_id: str = None,
         **kwargs
     ) -> typing.Union[QueryResponse, asyncio.Future]:
         """Execute Query Lambda By Version  # noqa: E501
 
         Execute a particular version of a Query Lambda.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.execute_query_lambda(
-            query_lambda="queryLambda_example",
-            version="version_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.execute_query_lambda(
+    query_lambda="queryLambda_example",
+    version="version_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             query_lambda (str): name of the Query Lambda. [required]
             version (str): version. [required]
             execute_query_lambda_request (ExecuteQueryLambdaRequest): JSON object. [optional]
             _return_http_data_only (bool): response data without head status
@@ -1486,32 +1487,33 @@
         workspace = "commons",
         async_options: AsyncQueryOptions = None,
         default_row_limit: int = None,
         generate_warnings: bool = None,
         initial_paginate_response_doc_count: int = None,
         paginate: bool = None,
         parameters: typing.Sequence[QueryParameter] = None,
+        timeout_ms: int = None,
         virtual_instance_id: str = None,
         **kwargs
     ) -> typing.Union[QueryResponse, asyncio.Future]:
         """Execute Query Lambda By Tag  # noqa: E501
 
         Execute the Query Lambda version associated with a given tag.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.execute_query_lambda_by_tag(
-            query_lambda="queryLambda_example",
-            tag="tag_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.execute_query_lambda_by_tag(
+    query_lambda="queryLambda_example",
+    tag="tag_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             query_lambda (str): name of the Query Lambda. [required]
             tag (str): tag. [required]
             execute_query_lambda_request (ExecuteQueryLambdaRequest): JSON object. [optional]
             _return_http_data_only (bool): response data without head status
@@ -1590,23 +1592,23 @@
     ) -> typing.Union[QueryLambdaTagResponse, asyncio.Future]:
         """Retrieve Query Lambda Tag  # noqa: E501
 
         Retrieve the Query Lambda version associated with a given tag.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.get_query_lambda_tag_version(
-            query_lambda="queryLambda_example",
-            tag="tag_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.get_query_lambda_tag_version(
+    query_lambda="queryLambda_example",
+    tag="tag_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             query_lambda (str): name of the Query Lambda. [required]
             tag (str): name of the tag. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -1684,23 +1686,23 @@
     ) -> typing.Union[QueryLambdaVersionResponse, asyncio.Future]:
         """Retrieve Query Lambda Version  # noqa: E501
 
         Retrieve details for a specified version of a Query Lambda.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.get_query_lambda_version(
-            query_lambda="queryLambda_example",
-            version="version_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.get_query_lambda_version(
+    query_lambda="queryLambda_example",
+    version="version_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             query_lambda (str): name of the Query Lambda. [required]
             version (str): version. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
@@ -1774,21 +1776,21 @@
     ) -> typing.Union[ListQueryLambdasResponse, asyncio.Future]:
         """List Query Lambdas  # noqa: E501
 
         List all Query Lambdas in an organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.list_all_query_lambdas(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.list_all_query_lambdas(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1856,22 +1858,22 @@
     ) -> typing.Union[ListQueryLambdaTagsResponse, asyncio.Future]:
         """List Query Lambda Tags  # noqa: E501
 
         List all tags associated with a Query Lambda  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.list_query_lambda_tags(
-            query_lambda="queryLambda_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.list_query_lambda_tags(
+    query_lambda="queryLambda_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             query_lambda (str): name of the Query Lambda. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -1945,22 +1947,22 @@
     ) -> typing.Union[ListQueryLambdaVersionsResponse, asyncio.Future]:
         """List Query Lambda Versions  # noqa: E501
 
         List all versions of a Query Lambda.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.list_query_lambda_versions(
-            query_lambda="queryLambda_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.list_query_lambda_versions(
+    query_lambda="queryLambda_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             query_lambda (str): name of the Query Lambda. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -2033,21 +2035,21 @@
     ) -> typing.Union[ListQueryLambdasResponse, asyncio.Future]:
         """List Query Lambdas in Workspace  # noqa: E501
 
         List all Query Lambdas under given workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.list_query_lambdas_in_workspace(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.list_query_lambdas_in_workspace(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -2122,34 +2124,34 @@
     ) -> typing.Union[QueryLambdaVersionResponse, asyncio.Future]:
         """Update Query Lambda  # noqa: E501
 
         Create a new version of a Query Lambda in given workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.QueryLambdas.update_query_lambda(
-            query_lambda="queryLambda_example",
-            description="production version foo",
-            is_public=True,
-            sql=QueryLambdaSql(
-                default_parameters=[
-                    QueryParameter(
-                        name="_id",
-                        type="string",
-                        value="85beb391",
-                    ),
-                ],
-                query="SELECT 'Foo'",
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.QueryLambdas.update_query_lambda(
+    query_lambda="queryLambda_example",
+    description="production version foo",
+    is_public=True,
+    sql=QueryLambdaSql(
+        default_parameters=[
+            QueryParameter(
+                name="_id",
+                type="string",
+                value="85beb391",
             ),
-            async_req=True,
-        )
-        result = await future
-        ```
+        ],
+        query="SELECT 'Foo'",
+    ),
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             query_lambda (str): name of the Query Lambda. [required]
             description (str): Optional description.. [optional]
             is_public (bool): [optional]
             sql (QueryLambdaSql): [optional]
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/shared_lambdas_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/shared_lambdas_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.error_model import ErrorModel
-from rockset.model.execute_public_query_lambda_request import ExecutePublicQueryLambdaRequest
-from rockset.model.query_response import QueryResponse
-from rockset.models import *
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.execute_public_query_lambda_request import ExecutePublicQueryLambdaRequest
+from rockset_v2.model.query_response import QueryResponse
+from rockset_v2.models import *
 
 
 class SharedLambdas(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -110,22 +110,22 @@
     ) -> typing.Union[QueryResponse, asyncio.Future]:
         """Execute a Public Query Lambda  # noqa: E501
 
         Execute a public query lambda (full version).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.SharedLambdas.execute_public_query_lambda_with_params(
-            public_access_id="public_access_id_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.SharedLambdas.execute_public_query_lambda_with_params(
+    public_access_id="public_access_id_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             public_access_id (str): public access ID of the query lambda. [required]
             execute_public_query_lambda_request (ExecutePublicQueryLambdaRequest): JSON object. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/users_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/users_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.create_user_request import CreateUserRequest
-from rockset.model.create_user_response import CreateUserResponse
-from rockset.model.delete_user_response import DeleteUserResponse
-from rockset.model.error_model import ErrorModel
-from rockset.model.list_unsubscribe_preferences_response import ListUnsubscribePreferencesResponse
-from rockset.model.list_users_response import ListUsersResponse
-from rockset.model.update_unsubscribe_preferences_request import UpdateUnsubscribePreferencesRequest
-from rockset.model.update_unsubscribe_preferences_response import UpdateUnsubscribePreferencesResponse
-from rockset.model.update_user_request import UpdateUserRequest
-from rockset.model.user import User
-from rockset.models import *
+from rockset_v2.model.create_user_request import CreateUserRequest
+from rockset_v2.model.create_user_response import CreateUserResponse
+from rockset_v2.model.delete_user_response import DeleteUserResponse
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.list_unsubscribe_preferences_response import ListUnsubscribePreferencesResponse
+from rockset_v2.model.list_users_response import ListUsersResponse
+from rockset_v2.model.update_unsubscribe_preferences_request import UpdateUnsubscribePreferencesRequest
+from rockset_v2.model.update_unsubscribe_preferences_response import UpdateUnsubscribePreferencesResponse
+from rockset_v2.model.update_user_request import UpdateUserRequest
+from rockset_v2.model.user import User
+from rockset_v2.models import *
 
 
 class Users(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -453,25 +453,25 @@
     ) -> typing.Union[CreateUserResponse, asyncio.Future]:
         """Create User  # noqa: E501
 
         Create a new user for an organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Users.create(
-            email="hello@rockset.com",
-            first_name="John",
-            last_name="Doe",
-            roles=["admin","member","read-only"],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Users.create(
+    email="hello@rockset.com",
+    first_name="John",
+    last_name="Doe",
+    roles=["admin","member","read-only"],
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             email (str): User email, must be unique.. [required]
             first_name (str): User first name.. [optional]
             last_name (str): User last name.. [optional]
             roles ([str]): List of roles for a given user.. [optional]
             _return_http_data_only (bool): response data without head status
@@ -544,22 +544,22 @@
     ) -> typing.Union[DeleteUserResponse, asyncio.Future]:
         """Delete User  # noqa: E501
 
         Delete a user from an organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Users.delete(
-            user="user_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Users.delete(
+    user="user_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             user (str): user email. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -629,22 +629,22 @@
     ) -> typing.Union[User, asyncio.Future]:
         """Retrieve User  # noqa: E501
 
         Retrieve user by email.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Users.get(
-            user="user_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Users.get(
+    user="user_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             user (str): user email. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -712,21 +712,21 @@
     ) -> typing.Union[User, asyncio.Future]:
         """Retrieve Current User  # noqa: E501
 
         Retrieve currently authenticated user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Users.get_current_user(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Users.get_current_user(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -791,21 +791,21 @@
     ) -> typing.Union[ListUsersResponse, asyncio.Future]:
         """List Users  # noqa: E501
 
         Retrieve all users for an organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Users.list(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Users.list(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -870,21 +870,21 @@
     ) -> typing.Union[ListUnsubscribePreferencesResponse, asyncio.Future]:
         """Retrieve Notification Preferences  # noqa: E501
 
         Get all notification preferences.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Users.list_unsubscribe_preferences(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Users.list_unsubscribe_preferences(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -954,25 +954,25 @@
     ) -> typing.Union[User, asyncio.Future]:
         """Update User  # noqa: E501
 
         Update a user in an organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Users.update(
-            user="user_example",
-            first_name="John",
-            last_name="Doe",
-            roles=["admin","member","read-only"],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Users.update(
+    user="user_example",
+    first_name="John",
+    last_name="Doe",
+    roles=["admin","member","read-only"],
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             user (str): email of the user to update. [required]
             first_name (str): User first name.. [optional]
             last_name (str): User last name.. [optional]
             roles ([str]): New list of roles for a given user.. [optional]
             _return_http_data_only (bool): response data without head status
@@ -1047,26 +1047,26 @@
     ) -> typing.Union[UpdateUnsubscribePreferencesResponse, asyncio.Future]:
         """Update Notification Preferences  # noqa: E501
 
         Update notification preference.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Users.update_unsubscribe_preferences(
-            data=[
-                UnsubscribePreference(
-                    notification_type="create_apikey",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Users.update_unsubscribe_preferences(
+    data=[
+        UnsubscribePreference(
+            notification_type="create_apikey",
+        ),
+    ],
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             data ([UnsubscribePreference]): List of notification preferences.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/views_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/views_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.create_view_request import CreateViewRequest
-from rockset.model.create_view_response import CreateViewResponse
-from rockset.model.delete_view_response import DeleteViewResponse
-from rockset.model.error_model import ErrorModel
-from rockset.model.get_view_response import GetViewResponse
-from rockset.model.list_views_response import ListViewsResponse
-from rockset.model.update_view_request import UpdateViewRequest
-from rockset.model.update_view_response import UpdateViewResponse
-from rockset.models import *
+from rockset_v2.model.create_view_request import CreateViewRequest
+from rockset_v2.model.create_view_response import CreateViewResponse
+from rockset_v2.model.delete_view_response import DeleteViewResponse
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.get_view_response import GetViewResponse
+from rockset_v2.model.list_views_response import ListViewsResponse
+from rockset_v2.model.update_view_request import UpdateViewRequest
+from rockset_v2.model.update_view_response import UpdateViewResponse
+from rockset_v2.models import *
 
 
 class Views(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -387,24 +387,24 @@
     ) -> typing.Union[CreateViewResponse, asyncio.Future]:
         """Create View  # noqa: E501
 
         Create a view  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Views.create(
-            description="view of awesome collection",
-            name="myAwesomeView",
-            query="SELECT * FROM foo",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Views.create(
+    description="view of awesome collection",
+    name="myAwesomeView",
+    query="SELECT * FROM foo",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             description (str): Optional description.. [optional]
             name (str): View name.. [required]
             query (str): SQL for this view.. [required]
             _return_http_data_only (bool): response data without head status
@@ -480,22 +480,22 @@
     ) -> typing.Union[DeleteViewResponse, asyncio.Future]:
         """Delete View  # noqa: E501
 
         Delete a view  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Views.delete(
-            view="view_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Views.delete(
+    view="view_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             view (str): name of the view. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -569,22 +569,22 @@
     ) -> typing.Union[GetViewResponse, asyncio.Future]:
         """Retrieve View  # noqa: E501
 
         Get details about a view  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Views.get(
-            view="view_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Views.get(
+    view="view_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             view (str): name of the view. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -655,21 +655,21 @@
     ) -> typing.Union[ListViewsResponse, asyncio.Future]:
         """List Views  # noqa: E501
 
         Retrieve all views in an organization  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Views.list(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Views.list(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -739,24 +739,24 @@
     ) -> typing.Union[UpdateViewResponse, asyncio.Future]:
         """Update View  # noqa: E501
 
         Update a view  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Views.update(
-            view="view_example",
-            description="view of awesome collection",
-            query="SELECT * FROM foo",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Views.update(
+    view="view_example",
+    description="view of awesome collection",
+    query="SELECT * FROM foo",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             view (str): name of the view. [required]
             description (str): Optional description.. [optional]
             query (str): SQL for this view.. [required]
             _return_http_data_only (bool): response data without head status
@@ -833,21 +833,21 @@
     ) -> typing.Union[ListViewsResponse, asyncio.Future]:
         """List Views in Workspace  # noqa: E501
 
         Retrieve all views in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Views.workspace_views(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Views.workspace_views(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/virtual_instances_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/virtual_instances_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.collection_mount_response import CollectionMountResponse
-from rockset.model.create_collection_mount_request import CreateCollectionMountRequest
-from rockset.model.create_collection_mounts_response import CreateCollectionMountsResponse
-from rockset.model.create_virtual_instance_request import CreateVirtualInstanceRequest
-from rockset.model.create_virtual_instance_response import CreateVirtualInstanceResponse
-from rockset.model.delete_virtual_instance_response import DeleteVirtualInstanceResponse
-from rockset.model.error_model import ErrorModel
-from rockset.model.get_virtual_instance_response import GetVirtualInstanceResponse
-from rockset.model.list_collection_mounts_response import ListCollectionMountsResponse
-from rockset.model.list_queries_response import ListQueriesResponse
-from rockset.model.list_virtual_instances_response import ListVirtualInstancesResponse
-from rockset.model.query_request import QueryRequest
-from rockset.model.query_response import QueryResponse
-from rockset.model.resume_virtual_instance_response import ResumeVirtualInstanceResponse
-from rockset.model.suspend_virtual_instance_response import SuspendVirtualInstanceResponse
-from rockset.model.update_virtual_instance_request import UpdateVirtualInstanceRequest
-from rockset.model.update_virtual_instance_response import UpdateVirtualInstanceResponse
-from rockset.models import *
+from rockset_v2.model.collection_mount_response import CollectionMountResponse
+from rockset_v2.model.create_collection_mount_request import CreateCollectionMountRequest
+from rockset_v2.model.create_collection_mounts_response import CreateCollectionMountsResponse
+from rockset_v2.model.create_virtual_instance_request import CreateVirtualInstanceRequest
+from rockset_v2.model.create_virtual_instance_response import CreateVirtualInstanceResponse
+from rockset_v2.model.delete_virtual_instance_response import DeleteVirtualInstanceResponse
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.get_virtual_instance_response import GetVirtualInstanceResponse
+from rockset_v2.model.list_collection_mounts_response import ListCollectionMountsResponse
+from rockset_v2.model.list_queries_response import ListQueriesResponse
+from rockset_v2.model.list_virtual_instances_response import ListVirtualInstancesResponse
+from rockset_v2.model.query_request import QueryRequest
+from rockset_v2.model.query_response import QueryResponse
+from rockset_v2.model.resume_virtual_instance_response import ResumeVirtualInstanceResponse
+from rockset_v2.model.suspend_virtual_instance_response import SuspendVirtualInstanceResponse
+from rockset_v2.model.update_virtual_instance_request import UpdateVirtualInstanceRequest
+from rockset_v2.model.update_virtual_instance_response import UpdateVirtualInstanceResponse
+from rockset_v2.models import *
 
 
 class VirtualInstances(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -744,38 +744,44 @@
 
     def create(
         self,
         *,
         name: str,
         auto_suspend_seconds: int = None,
         description: str = None,
+        enable_remount_on_resume: bool = None,
+        mount_refresh_interval_seconds: int = None,
         type: str = None,
         **kwargs
     ) -> typing.Union[CreateVirtualInstanceResponse, asyncio.Future]:
         """Create Virtual Instance  # noqa: E501
 
         [beta] Create virtual instance  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.create(
-            auto_suspend_seconds=3600,
-            description="VI serving prod traffic",
-            name="prod_vi",
-            type="LARGE",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.create(
+    auto_suspend_seconds=3600,
+    description="VI serving prod traffic",
+    enable_remount_on_resume=True,
+    mount_refresh_interval_seconds=3600,
+    name="prod_vi",
+    type="LARGE",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]
             description (str): Description of requested virtual instance.. [optional]
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]
+            mount_refresh_interval_seconds (int): Number of seconds between data refreshes for mounts on this Virtual Instance. A value of 0 means continuous refresh and a value of null means never refresh.. [optional]
             name (str): Unique identifier for virtual instance, can contain alphanumeric or dash characters.. [required]
             type (str): Requested virtual instance type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -844,22 +850,22 @@
     ) -> typing.Union[DeleteVirtualInstanceResponse, asyncio.Future]:
         """Delete Virtual Instance  # noqa: E501
 
         [beta] Delete a virtual instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.delete(
-            virtual_instance_id="virtualInstanceId_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.delete(
+    virtual_instance_id="virtualInstanceId_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -929,22 +935,22 @@
     ) -> typing.Union[GetVirtualInstanceResponse, asyncio.Future]:
         """Retrieve Virtual Instance  # noqa: E501
 
         Get details about a virtual instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.get(
-            virtual_instance_id="virtualInstanceId_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.get(
+    virtual_instance_id="virtualInstanceId_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -1011,27 +1017,27 @@
         *,
         virtual_instance_id: str,
         collection_path: str,
         **kwargs
     ) -> typing.Union[CollectionMountResponse, asyncio.Future]:
         """Get Collection Mount  # noqa: E501
 
-        [beta] Get a mount on this virtual instance.  # noqa: E501
+        [beta] Retrieve a mount on this virtual instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.get_collection_mount(
-            virtual_instance_id="virtualInstanceId_example",
-            collection_path="collectionPath_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.get_collection_mount(
+    virtual_instance_id="virtualInstanceId_example",
+    collection_path="collectionPath_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
             collection_path (str): [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -1104,22 +1110,22 @@
     ) -> typing.Union[ListQueriesResponse, asyncio.Future]:
         """List Queries  # noqa: E501
 
         [beta] Lists actively queued and running queries for a particular Virtual Instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.get_virtual_instance_queries(
-            virtual_instance_id="virtualInstanceId_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.get_virtual_instance_queries(
+    virtual_instance_id="virtualInstanceId_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -1187,21 +1193,21 @@
     ) -> typing.Union[ListVirtualInstancesResponse, asyncio.Future]:
         """List Virtual Instances  # noqa: E501
 
         Retrieve all virtual instances in an organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.list(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.list(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1268,22 +1274,22 @@
     ) -> typing.Union[ListCollectionMountsResponse, asyncio.Future]:
         """List Collection Mounts  # noqa: E501
 
         [beta] List collection mounts for a particular VI.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.list_collection_mounts(
-            virtual_instance_id="virtualInstanceId_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.list_collection_mounts(
+    virtual_instance_id="virtualInstanceId_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -1346,38 +1352,35 @@
         return self.list_collection_mounts_endpoint.call_with_http_info(**kwargs)
 
     def mount_collection(
         self,
         *,
         virtual_instance_id: str,
         collection_paths: typing.Sequence[str] = None,
-        type: str = None,
         **kwargs
     ) -> typing.Union[CreateCollectionMountsResponse, asyncio.Future]:
-        """Mount Collection  # noqa: E501
+        """Mount Collections  # noqa: E501
 
         [beta] Mount a collection to this virtual instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.mount_collection(
-            virtual_instance_id="virtualInstanceId_example",
-            collection_paths=["commons.foo","commons.bar"],
-            type="STATIC",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.mount_collection(
+    virtual_instance_id="virtualInstanceId_example",
+    collection_paths=["commons.foo","commons.bar"],
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
             collection_paths ([str]): Collections to mount.. [optional]
-            type (str): Mount type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1440,54 +1443,56 @@
 
     def query_virtual_instance(
         self,
         *,
         virtual_instance_id: str,
         sql: QueryRequestSql,
         async_options: AsyncQueryOptions = None,
+        timeout_ms: int = None,
         **kwargs
     ) -> typing.Union[QueryResponse, asyncio.Future]:
         """Execute SQL Query  # noqa: E501
 
         [beta] Make a SQL query to Rockset.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.query_virtual_instance(
-            virtual_instance_id="virtualInstanceId_example",
-            async_options=AsyncQueryOptions(
-                client_timeout_ms=1,
-                max_initial_results=1,
-                timeout_ms=1,
-            ),
-            sql=QueryRequestSql(
-                default_row_limit=1,
-                generate_warnings=False,
-                initial_paginate_response_doc_count=1,
-                paginate=True,
-                parameters=[
-                    QueryParameter(
-                        name="_id",
-                        type="string",
-                        value="85beb391",
-                    ),
-                ],
-                query="SELECT * FROM foo where _id = :_id",
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.query_virtual_instance(
+    virtual_instance_id="virtualInstanceId_example",
+    async_options=AsyncQueryOptions(
+        client_timeout_ms=1,
+        max_initial_results=1,
+        timeout_ms=1,
+    ),
+    sql=QueryRequestSql(
+        default_row_limit=1,
+        generate_warnings=False,
+        initial_paginate_response_doc_count=1,
+        parameters=[
+            QueryParameter(
+                name="_id",
+                type="string",
+                value="85beb391",
             ),
-            async_req=True,
-        )
-        result = await future
-        ```
+        ],
+        query="SELECT * FROM foo where _id = :_id",
+    ),
+    timeout_ms=1,
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
             async_options (AsyncQueryOptions): [optional]
             sql (QueryRequestSql): [required]
+            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error. The maximum value for this timeout is 2 minutes. async_options.timeout_ms will override this timeout.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1556,22 +1561,22 @@
     ) -> typing.Union[ResumeVirtualInstanceResponse, asyncio.Future]:
         """Resume Virtual Instance  # noqa: E501
 
         [beta] Resume a virtual instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.resume_virtual_instance(
-            virtual_instance_id="virtualInstanceId_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.resume_virtual_instance(
+    virtual_instance_id="virtualInstanceId_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -1641,22 +1646,22 @@
     ) -> typing.Union[SuspendVirtualInstanceResponse, asyncio.Future]:
         """Suspend Virtual Instance  # noqa: E501
 
         [beta] Suspend a virtual instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.suspend_virtual_instance(
-            virtual_instance_id="virtualInstanceId_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.suspend_virtual_instance(
+    virtual_instance_id="virtualInstanceId_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -1727,23 +1732,23 @@
     ) -> typing.Union[CollectionMountResponse, asyncio.Future]:
         """Unmount Collection  # noqa: E501
 
         [beta] Unmount a collection from this virtual instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.unmount_collection(
-            virtual_instance_id="virtualInstanceId_example",
-            collection_path="collectionPath_example",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.unmount_collection(
+    virtual_instance_id="virtualInstanceId_example",
+    collection_path="collectionPath_example",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
             collection_path (str): [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -1808,49 +1813,59 @@
             collection_path
         return self.unmount_collection_endpoint.call_with_http_info(**kwargs)
 
     def update(
         self,
         *,
         virtual_instance_id: str,
+        auto_scaling_policy: AutoScalingPolicy = None,
         auto_suspend_enabled: bool = None,
         auto_suspend_seconds: int = None,
         description: str = None,
-        monitoring_enabled: bool = None,
+        enable_remount_on_resume: bool = None,
+        mount_refresh_interval_seconds: int = None,
         name: str = None,
         new_size: str = None,
         **kwargs
     ) -> typing.Union[UpdateVirtualInstanceResponse, asyncio.Future]:
         """Update Virtual Instance  # noqa: E501
 
         Update the properties of a virtual instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.VirtualInstances.update(
-            virtual_instance_id="virtualInstanceId_example",
-            auto_suspend_enabled=True,
-            auto_suspend_seconds=3600,
-            description="VI for prod traffic",
-            monitoring_enabled=True,
-            name="prod_vi",
-            new_size="LARGE",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.VirtualInstances.update(
+    virtual_instance_id="virtualInstanceId_example",
+    auto_scaling_policy=AutoScalingPolicy(
+        enabled=True,
+        max_size="XLARGE2",
+        min_size="LARGE",
+    ),
+    auto_suspend_enabled=True,
+    auto_suspend_seconds=3600,
+    description="VI for prod traffic",
+    enable_remount_on_resume=True,
+    mount_refresh_interval_seconds=3600,
+    name="prod_vi",
+    new_size="LARGE",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
+            auto_scaling_policy (AutoScalingPolicy): [optional]
             auto_suspend_enabled (bool): Whether auto-suspend should be enabled for this Virtual Instance.. [optional]
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]
             description (str): New virtual instance description.. [optional]
-            monitoring_enabled (bool): [optional]
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]
+            mount_refresh_interval_seconds (int): Number of seconds between data refreshes for mounts on this Virtual Instance. A value of 0 means continuous refresh and a value of null means never refresh.. [optional]
             name (str): New virtual instance name.. [optional]
             new_size (str): Requested virtual instance size.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api/workspaces_api.py` & `rockset_v2_internal-2.0.2/rockset_v2/api/workspaces_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 
 import re  # noqa: F401
 import sys  # noqa: F401
 import typing  # noqa: F401
 
 import asyncio
 
-from rockset.api_client import ApiClient, Endpoint as _Endpoint
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.api_client import ApiClient, Endpoint as _Endpoint
+from rockset_v2.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from rockset.model.create_workspace_request import CreateWorkspaceRequest
-from rockset.model.create_workspace_response import CreateWorkspaceResponse
-from rockset.model.delete_workspace_response import DeleteWorkspaceResponse
-from rockset.model.error_model import ErrorModel
-from rockset.model.get_workspace_response import GetWorkspaceResponse
-from rockset.model.list_workspaces_response import ListWorkspacesResponse
-from rockset.models import *
+from rockset_v2.model.create_workspace_request import CreateWorkspaceRequest
+from rockset_v2.model.create_workspace_response import CreateWorkspaceResponse
+from rockset_v2.model.delete_workspace_response import DeleteWorkspaceResponse
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.get_workspace_response import GetWorkspaceResponse
+from rockset_v2.model.list_workspaces_response import ListWorkspacesResponse
+from rockset_v2.models import *
 
 
 class Workspaces(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -251,23 +251,23 @@
     ) -> typing.Union[CreateWorkspaceResponse, asyncio.Future]:
         """Create Workspace  # noqa: E501
 
         Create a new workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Workspaces.create(
-            description="Datasets of system logs for the ops team.",
-            name="event_logs",
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Workspaces.create(
+    description="Datasets of system logs for the ops team.",
+    name="event_logs",
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             description (str): Longer explanation for the workspace.. [optional]
             name (str): Descriptive label and unique identifier.. [required]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -338,21 +338,21 @@
     ) -> typing.Union[DeleteWorkspaceResponse, asyncio.Future]:
         """Delete Workspace  # noqa: E501
 
         Remove a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Workspaces.delete(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Workspaces.delete(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -422,21 +422,21 @@
     ) -> typing.Union[GetWorkspaceResponse, asyncio.Future]:
         """Retrieve Workspace  # noqa: E501
 
         Get information about a single workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Workspaces.get(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Workspaces.get(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -504,21 +504,21 @@
     ) -> typing.Union[ListWorkspacesResponse, asyncio.Future]:
         """List Workspaces  # noqa: E501
 
         List all workspaces in an organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Workspaces.list(
-            async_req=True,
-        )
-        result = await future
-        ```
+```python
+rs = RocksetClient(api_key=APIKEY)
+future = rs.Workspaces.list(
+    async_req=True,
+)
+result = await future
+```
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/api_client.py` & `rockset_v2_internal-2.0.2/rockset_v2/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 import re
 import typing
 from concurrent.futures import ThreadPoolExecutor
 from functools import wraps
 from urllib.parse import quote
 from urllib3.fields import RequestField
 
-from rockset import rest
-from rockset.configuration import Configuration
-from rockset.exceptions import ApiTypeError, ApiValueError, ApiException
-from rockset.model_utils import (
+from rockset_v2 import rest
+from rockset_v2.configuration import Configuration
+from rockset_v2.exceptions import ApiTypeError, ApiValueError, ApiException
+from rockset_v2.model_utils import (
     ModelNormal,
     ModelSimple,
     ModelComposed,
     check_allowed_values,
     check_validations,
     date,
     datetime,
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/apis/__init__.py` & `rockset_v2_internal-2.0.2/rockset_v2/apis/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 #
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
-from rockset.api.api_keys_api import APIKeys
-from rockset.api.aliases_api import Aliases
-from rockset.api.collections_api import Collections
-from rockset.api.custom_roles_api import CustomRoles
-from rockset.api.documents_api import Documents
-from rockset.api.integrations_api import Integrations
-from rockset.api.organizations_api import Organizations
-from rockset.api.queries_api import Queries
-from rockset.api.query_lambdas_api import QueryLambdas
-from rockset.api.shared_lambdas_api import SharedLambdas
-from rockset.api.users_api import Users
-from rockset.api.views_api import Views
-from rockset.api.virtual_instances_api import VirtualInstances
-from rockset.api.workspaces_api import Workspaces
+from rockset_v2.api.api_keys_api import APIKeys
+from rockset_v2.api.aliases_api import Aliases
+from rockset_v2.api.collections_api import Collections
+from rockset_v2.api.custom_roles_api import CustomRoles
+from rockset_v2.api.documents_api import Documents
+from rockset_v2.api.integrations_api import Integrations
+from rockset_v2.api.organizations_api import Organizations
+from rockset_v2.api.queries_api import Queries
+from rockset_v2.api.query_lambdas_api import QueryLambdas
+from rockset_v2.api.shared_lambdas_api import SharedLambdas
+from rockset_v2.api.users_api import Users
+from rockset_v2.api.views_api import Views
+from rockset_v2.api.virtual_instances_api import VirtualInstances
+from rockset_v2.api.workspaces_api import Workspaces
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/configuration.py` & `rockset_v2_internal-2.0.2/rockset_v2/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 from http import client as http_client
-from rockset.exceptions import ApiValueError
+from rockset_v2.exceptions import ApiValueError
 
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
@@ -70,15 +70,15 @@
     :param retries: int - Overrides the default number of retry attempts for the
       urllib3 PoolManager
 
     :Example:
 
     Requests to the Rockset API made from clients should use apikeys which are set in the authorization header with a prefix of 'apikey'.
 
-    conf = rockset.Configuration(
+    conf = rockset_v2.Configuration(
         api_key='abc123'
     )
 
     The following header will be added to the HTTP request:
        Authorization: apikey abc123
     """
 
@@ -118,15 +118,15 @@
         """
 
         self.discard_unknown_keys = discard_unknown_keys
         self.disabled_client_side_validations = disabled_client_side_validations
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("rockset")
+        self.logger["package_logger"] = logging.getLogger("rockset_v2")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/document.py` & `rockset_v2_internal-2.0.2/rockset_v2/document.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/exceptions.py` & `rockset_v2_internal-2.0.2/rockset_v2/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/add_documents_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/add_documents_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class AddDocumentsRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/add_documents_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/add_documents_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.document_status import DocumentStatus
+    from rockset_v2.model.document_status import DocumentStatus
     globals()['DocumentStatus'] = DocumentStatus
 
 
 class AddDocumentsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/alias.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/alias.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class Alias(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/api_key.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class ApiKey(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/async_query_options.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/async_query_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class AsyncQueryOptions(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -136,15 +136,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             client_timeout_ms (int): The maximum amount of time that the client is willing to wait for the query to complete. If the query is not complete by this timeout, a response will be returned with a `query_id` that can be used to check the status of the query and retrieve results once the query has completed.. [optional]  # noqa: E501
             max_initial_results (int): The maximum number of results you will receive as a client. If the query exceeds this limit, the remaining results can be requested using a returned pagination cursor. In addition, there is a maximum response size of 100MiB so fewer than `max_results` may be returned.. [optional]  # noqa: E501
-            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error.. [optional]  # noqa: E501
+            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error. This must be set to a value that is greater than or equal to the client timeout, and the maximum value of this timeout is 30 minutes.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,15 +190,15 @@
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
         """AsyncQueryOptions - a model defined in OpenAPI
 
         Keyword Args:
             client_timeout_ms (int): The maximum amount of time that the client is willing to wait for the query to complete. If the query is not complete by this timeout, a response will be returned with a `query_id` that can be used to check the status of the query and retrieve results once the query has completed.. [optional]  # noqa: E501
             max_initial_results (int): The maximum number of results you will receive as a client. If the query exceeds this limit, the remaining results can be requested using a returned pagination cursor. In addition, there is a maximum response size of 100MiB so fewer than `max_results` may be returned.. [optional]  # noqa: E501
-            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error.. [optional]  # noqa: E501
+            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error. This must be set to a value that is greater than or equal to the client timeout, and the maximum value of this timeout is 30 minutes.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/aws_access_key.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/aws_access_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class AwsAccessKey(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/aws_role.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/aws_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class AwsRole(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/azure_blob_storage_collection_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/file_upload_collection_creation_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,46 +7,44 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.azure_blob_storage_source_wrapper import AzureBlobStorageSourceWrapper
-    from rockset.model.event_time_info import EventTimeInfo
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
-    globals()['AzureBlobStorageSourceWrapper'] = AzureBlobStorageSourceWrapper
+    from rockset_v2.model.event_time_info import EventTimeInfo
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_partition import FieldPartition
+    from rockset_v2.model.file_upload_source_wrapper import FileUploadSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
+    globals()['FileUploadSourceWrapper'] = FileUploadSourceWrapper
 
 
-class AzureBlobStorageCollectionCreationRequest(ModelNormal):
+class FileUploadCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([AzureBlobStorageSourceWrapper], none_type),  # noqa: E501
+            'sources': ([FileUploadSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """AzureBlobStorageCollectionCreationRequest - a model defined in OpenAPI
+        """FileUploadCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([AzureBlobStorageSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([FileUploadSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """AzureBlobStorageCollectionCreationRequest - a model defined in OpenAPI
+        """FileUploadCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([AzureBlobStorageSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([FileUploadSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/azure_blob_storage_integration.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class AzureBlobStorageIntegration(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/azure_blob_storage_integration_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_integration_creation_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.azure_blob_storage_integration import AzureBlobStorageIntegration
+    from rockset_v2.model.azure_blob_storage_integration import AzureBlobStorageIntegration
     globals()['AzureBlobStorageIntegration'] = AzureBlobStorageIntegration
 
 
 class AzureBlobStorageIntegrationCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/azure_blob_storage_source_wrapper.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_source_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status import Status
+    from rockset_v2.model.format_params import FormatParams
+    from rockset_v2.model.status import Status
     globals()['FormatParams'] = FormatParams
     globals()['Status'] = Status
 
 
 class AzureBlobStorageSourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/azure_event_hubs_collection_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/kafka_collection_creation_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,46 +7,44 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.azure_event_hubs_source_wrapper import AzureEventHubsSourceWrapper
-    from rockset.model.event_time_info import EventTimeInfo
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
-    globals()['AzureEventHubsSourceWrapper'] = AzureEventHubsSourceWrapper
+    from rockset_v2.model.event_time_info import EventTimeInfo
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_partition import FieldPartition
+    from rockset_v2.model.kafka_source_wrapper import KafkaSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
+    globals()['KafkaSourceWrapper'] = KafkaSourceWrapper
 
 
-class AzureEventHubsCollectionCreationRequest(ModelNormal):
+class KafkaCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([AzureEventHubsSourceWrapper], none_type),  # noqa: E501
+            'sources': ([KafkaSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """AzureEventHubsCollectionCreationRequest - a model defined in OpenAPI
+        """KafkaCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([AzureEventHubsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([KafkaSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """AzureEventHubsCollectionCreationRequest - a model defined in OpenAPI
+        """KafkaCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([AzureEventHubsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([KafkaSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/azure_event_hubs_integration.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class AzureEventHubsIntegration(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/azure_event_hubs_integration_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_integration_creation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.azure_event_hubs_integration import AzureEventHubsIntegration
+    from rockset_v2.model.azure_event_hubs_integration import AzureEventHubsIntegration
     globals()['AzureEventHubsIntegration'] = AzureEventHubsIntegration
 
 
 class AzureEventHubsIntegrationCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/azure_event_hubs_source_wrapper.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_source_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status_azure_event_hubs import StatusAzureEventHubs
+    from rockset_v2.model.format_params import FormatParams
+    from rockset_v2.model.status_azure_event_hubs import StatusAzureEventHubs
     globals()['FormatParams'] = FormatParams
     globals()['StatusAzureEventHubs'] = StatusAzureEventHubs
 
 
 class AzureEventHubsSourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/azure_service_bus_collection_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/azure_blob_storage_collection_creation_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,46 +7,44 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.azure_service_bus_source_wrapper import AzureServiceBusSourceWrapper
-    from rockset.model.event_time_info import EventTimeInfo
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
-    globals()['AzureServiceBusSourceWrapper'] = AzureServiceBusSourceWrapper
+    from rockset_v2.model.azure_blob_storage_source_wrapper import AzureBlobStorageSourceWrapper
+    from rockset_v2.model.event_time_info import EventTimeInfo
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_partition import FieldPartition
+    globals()['AzureBlobStorageSourceWrapper'] = AzureBlobStorageSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
 
 
-class AzureServiceBusCollectionCreationRequest(ModelNormal):
+class AzureBlobStorageCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([AzureServiceBusSourceWrapper], none_type),  # noqa: E501
+            'sources': ([AzureBlobStorageSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """AzureServiceBusCollectionCreationRequest - a model defined in OpenAPI
+        """AzureBlobStorageCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([AzureServiceBusSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([AzureBlobStorageSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """AzureServiceBusCollectionCreationRequest - a model defined in OpenAPI
+        """AzureBlobStorageCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([AzureServiceBusSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([AzureBlobStorageSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/azure_service_bus_integration.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/azure_service_bus_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class AzureServiceBusIntegration(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/azure_service_bus_source_wrapper.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/azure_service_bus_source_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status_azure_service_bus import StatusAzureServiceBus
+    from rockset_v2.model.format_params import FormatParams
+    from rockset_v2.model.status_azure_service_bus import StatusAzureServiceBus
     globals()['FormatParams'] = FormatParams
     globals()['StatusAzureServiceBus'] = StatusAzureServiceBus
 
 
 class AzureServiceBusSourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/bulk_stats.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/bulk_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class BulkStats(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/cancel_query_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/cancel_query_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_info import QueryInfo
+    from rockset_v2.model.query_info import QueryInfo
     globals()['QueryInfo'] = QueryInfo
 
 
 class CancelQueryResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/cluster.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class Cluster(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/collection.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,40 +7,40 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.alias import Alias
-    from rockset.model.bulk_stats import BulkStats
-    from rockset.model.collection_stats import CollectionStats
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
-    from rockset.model.source import Source
+    from rockset_v2.model.alias import Alias
+    from rockset_v2.model.bulk_stats import BulkStats
+    from rockset_v2.model.collection_stats import CollectionStats
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_mapping_v2 import FieldMappingV2
+    from rockset_v2.model.field_partition import FieldPartition
+    from rockset_v2.model.source import Source
     globals()['Alias'] = Alias
     globals()['BulkStats'] = BulkStats
     globals()['CollectionStats'] = CollectionStats
     globals()['FieldMappingQuery'] = FieldMappingQuery
     globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
     globals()['Source'] = Source
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/collection_mount.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,38 +7,40 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.collection_mount_stats import CollectionMountStats
-    globals()['CollectionMountStats'] = CollectionMountStats
+    from rockset_v2.model.query_lambda_sql import QueryLambdaSql
+    from rockset_v2.model.query_lambda_stats import QueryLambdaStats
+    globals()['QueryLambdaSql'] = QueryLambdaSql
+    globals()['QueryLambdaStats'] = QueryLambdaStats
 
 
-class CollectionMount(ModelNormal):
+class QueryLambdaVersion(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,23 +58,16 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
         ('state',): {
-            'CREATING': "CREATING",
             'ACTIVE': "ACTIVE",
-            'REFRESHING': "REFRESHING",
-            'EXPIRED': "EXPIRED",
-            'DELETING': "DELETING",
-        },
-        ('type',): {
-            'STATIC': "STATIC",
-            'LIVE': "LIVE",
+            'INVALID_SQL': "INVALID_SQL",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -94,53 +89,55 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'collection_path': (str, none_type),  # noqa: E501
+            'collections': ([str], none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
-            'id': (str, none_type),  # noqa: E501
-            'rrn': (str, none_type),  # noqa: E501
-            'snapshot_expiration_time_millis': (int, none_type),  # noqa: E501
+            'created_by': (str, none_type),  # noqa: E501
+            'description': (str, none_type),  # noqa: E501
+            'name': (str, none_type),  # noqa: E501
+            'public_access_id': (str, none_type),  # noqa: E501
+            'sql': (QueryLambdaSql, none_type),  # noqa: E501
             'state': (str, none_type),  # noqa: E501
-            'stats': (CollectionMountStats, none_type),  # noqa: E501
-            'type': (str, none_type),  # noqa: E501
-            'virtual_instance_id': (str, none_type),  # noqa: E501
-            'virtual_instance_rrn': (str, none_type),  # noqa: E501
+            'stats': (QueryLambdaStats, none_type),  # noqa: E501
+            'version': (str, none_type),  # noqa: E501
+            'workspace': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'collection_path': 'collection_path',  # noqa: E501
+        'collections': 'collections',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
-        'id': 'id',  # noqa: E501
-        'rrn': 'rrn',  # noqa: E501
-        'snapshot_expiration_time_millis': 'snapshot_expiration_time_millis',  # noqa: E501
+        'created_by': 'created_by',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'public_access_id': 'public_access_id',  # noqa: E501
+        'sql': 'sql',  # noqa: E501
         'state': 'state',  # noqa: E501
         'stats': 'stats',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'virtual_instance_id': 'virtual_instance_id',  # noqa: E501
-        'virtual_instance_rrn': 'virtual_instance_rrn',  # noqa: E501
+        'version': 'version',  # noqa: E501
+        'workspace': 'workspace',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CollectionMount - a model defined in OpenAPI
+        """QueryLambdaVersion - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,24 +162,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            collection_path (str): Collection path.. [optional]  # noqa: E501
-            created_at (str): ISO-8601 date.. [optional]  # noqa: E501
-            id (str): Mount ID.. [optional]  # noqa: E501
-            rrn (str): Mount RRN.. [optional]  # noqa: E501
-            snapshot_expiration_time_millis (int): Time in millis at which the snapshot expires.. [optional]  # noqa: E501
-            state (str): Mount type.. [optional]  # noqa: E501
-            stats (CollectionMountStats): [optional]  # noqa: E501
-            type (str): Mount type.. [optional]  # noqa: E501
-            virtual_instance_id (str): Virtual instance ID.. [optional]  # noqa: E501
-            virtual_instance_rrn (str): Virtual Instance RRN.. [optional]  # noqa: E501
+            collections ([str]): Collections queried by underlying SQL query.. [optional]  # noqa: E501
+            created_at (str): ISO-8601 date of when Query Lambda was created.. [optional]  # noqa: E501
+            created_by (str): User that created this Query Lambda.. [optional]  # noqa: E501
+            description (str): Optional description.. [optional]  # noqa: E501
+            name (str): Query Lambda name.. [optional]  # noqa: E501
+            public_access_id (str): Public access ID associated with this QL version. [optional]  # noqa: E501
+            sql (QueryLambdaSql): [optional]  # noqa: E501
+            state (str): Status of this Query Lambda.. [optional]  # noqa: E501
+            stats (QueryLambdaStats): [optional]  # noqa: E501
+            version (str): Query Lambda version.. [optional]  # noqa: E501
+            workspace (str): Workspace of this Query Lambda.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -223,27 +221,28 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """CollectionMount - a model defined in OpenAPI
+        """QueryLambdaVersion - a model defined in OpenAPI
 
         Keyword Args:
-            collection_path (str): Collection path.. [optional]  # noqa: E501
-            created_at (str): ISO-8601 date.. [optional]  # noqa: E501
-            id (str): Mount ID.. [optional]  # noqa: E501
-            rrn (str): Mount RRN.. [optional]  # noqa: E501
-            snapshot_expiration_time_millis (int): Time in millis at which the snapshot expires.. [optional]  # noqa: E501
-            state (str): Mount type.. [optional]  # noqa: E501
-            stats (CollectionMountStats): [optional]  # noqa: E501
-            type (str): Mount type.. [optional]  # noqa: E501
-            virtual_instance_id (str): Virtual instance ID.. [optional]  # noqa: E501
-            virtual_instance_rrn (str): Virtual Instance RRN.. [optional]  # noqa: E501
+            collections ([str]): Collections queried by underlying SQL query.. [optional]  # noqa: E501
+            created_at (str): ISO-8601 date of when Query Lambda was created.. [optional]  # noqa: E501
+            created_by (str): User that created this Query Lambda.. [optional]  # noqa: E501
+            description (str): Optional description.. [optional]  # noqa: E501
+            name (str): Query Lambda name.. [optional]  # noqa: E501
+            public_access_id (str): Public access ID associated with this QL version. [optional]  # noqa: E501
+            sql (QueryLambdaSql): [optional]  # noqa: E501
+            state (str): Status of this Query Lambda.. [optional]  # noqa: E501
+            stats (QueryLambdaStats): [optional]  # noqa: E501
+            version (str): Query Lambda version.. [optional]  # noqa: E501
+            workspace (str): Workspace of this Query Lambda.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/collection_mount_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/collection_mount_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.collection_mount import CollectionMount
+    from rockset_v2.model.collection_mount import CollectionMount
     globals()['CollectionMount'] = CollectionMount
 
 
 class CollectionMountResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/collection_mount_stats.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/collection_mount_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class CollectionMountStats(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/collection_stats.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/collection_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class CollectionStats(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_alias_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_alias_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class CreateAliasRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_alias_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_alias_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.alias import Alias
+    from rockset_v2.model.alias import Alias
     globals()['Alias'] = Alias
 
 
 class CreateAliasResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_api_key_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_api_key_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class CreateApiKeyRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_api_key_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_api_key_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.api_key import ApiKey
+    from rockset_v2.model.api_key import ApiKey
     globals()['ApiKey'] = ApiKey
 
 
 class CreateApiKeyResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_collection_mount_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/get_collection_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,34 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rockset_v2.model.collection import Collection
+    globals()['Collection'] = Collection
 
-class CreateCollectionMountRequest(ModelNormal):
+
+class GetCollectionResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,67 +55,63 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
-        ('type',): {
-            'STATIC': "STATIC",
-            'LIVE': "LIVE",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'collection_paths': ([str], none_type),  # noqa: E501
-            'type': (str, none_type),  # noqa: E501
+            'data': (Collection, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'collection_paths': 'collection_paths',  # noqa: E501
-        'type': 'type',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CreateCollectionMountRequest - a model defined in OpenAPI
+        """GetCollectionResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,16 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            collection_paths ([str]): Collections to mount.. [optional]  # noqa: E501
-            type (str): Mount type.. [optional]  # noqa: E501
+            data (Collection): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,19 +185,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """CreateCollectionMountRequest - a model defined in OpenAPI
+        """GetCollectionResponse - a model defined in OpenAPI
 
         Keyword Args:
-            collection_paths ([str]): Collections to mount.. [optional]  # noqa: E501
-            type (str): Mount type.. [optional]  # noqa: E501
+            data (Collection): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_collection_mounts_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_mounts_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.collection_mount import CollectionMount
+    from rockset_v2.model.collection_mount import CollectionMount
     globals()['CollectionMount'] = CollectionMount
 
 
 class CreateCollectionMountsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_collection_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,40 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.event_time_info import EventTimeInfo
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
+    from rockset_v2.model.event_time_info import EventTimeInfo
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_partition import FieldPartition
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
 
 
 class CreateCollectionRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -61,14 +59,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -96,32 +98,32 @@
         """
         lazy_import()
         return {
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'name': (str, none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'name': 'name',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -161,17 +163,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -219,17 +221,17 @@
         """CreateCollectionRequest - a model defined in OpenAPI
 
         Keyword Args:
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_collection_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.collection import Collection
+    from rockset_v2.model.collection import Collection
     globals()['Collection'] = Collection
 
 
 class CreateCollectionResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_integration_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_integration_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,43 +7,43 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.azure_blob_storage_integration import AzureBlobStorageIntegration
-    from rockset.model.azure_event_hubs_integration import AzureEventHubsIntegration
-    from rockset.model.azure_service_bus_integration import AzureServiceBusIntegration
-    from rockset.model.dynamodb_integration import DynamodbIntegration
-    from rockset.model.gcs_integration import GcsIntegration
-    from rockset.model.kafka_integration import KafkaIntegration
-    from rockset.model.kinesis_integration import KinesisIntegration
-    from rockset.model.mongo_db_integration import MongoDbIntegration
-    from rockset.model.s3_integration import S3Integration
-    from rockset.model.snowflake_integration import SnowflakeIntegration
+    from rockset_v2.model.azure_blob_storage_integration import AzureBlobStorageIntegration
+    from rockset_v2.model.azure_event_hubs_integration import AzureEventHubsIntegration
+    from rockset_v2.model.azure_service_bus_integration import AzureServiceBusIntegration
+    from rockset_v2.model.dynamodb_integration import DynamodbIntegration
+    from rockset_v2.model.gcs_integration import GcsIntegration
+    from rockset_v2.model.kafka_integration import KafkaIntegration
+    from rockset_v2.model.kinesis_integration import KinesisIntegration
+    from rockset_v2.model.mongo_db_integration import MongoDbIntegration
+    from rockset_v2.model.s3_integration import S3Integration
+    from rockset_v2.model.snowflake_integration import SnowflakeIntegration
     globals()['AzureBlobStorageIntegration'] = AzureBlobStorageIntegration
     globals()['AzureEventHubsIntegration'] = AzureEventHubsIntegration
     globals()['AzureServiceBusIntegration'] = AzureServiceBusIntegration
     globals()['DynamodbIntegration'] = DynamodbIntegration
     globals()['GcsIntegration'] = GcsIntegration
     globals()['KafkaIntegration'] = KafkaIntegration
     globals()['KinesisIntegration'] = KinesisIntegration
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_integration_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_integration_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.integration import Integration
+    from rockset_v2.model.integration import Integration
     globals()['Integration'] = Integration
 
 
 class CreateIntegrationResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_query_lambda_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_query_lambda_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_lambda_sql import QueryLambdaSql
+    from rockset_v2.model.query_lambda_sql import QueryLambdaSql
     globals()['QueryLambdaSql'] = QueryLambdaSql
 
 
 class CreateQueryLambdaRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_query_lambda_tag_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_query_lambda_tag_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class CreateQueryLambdaTagRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_role_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_role_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.privilege import Privilege
+    from rockset_v2.model.privilege import Privilege
     globals()['Privilege'] = Privilege
 
 
 class CreateRoleRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_user_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class CreateUserRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_user_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_user_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.user import User
+    from rockset_v2.model.user import User
     globals()['User'] = User
 
 
 class CreateUserResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_view_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_view_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class CreateViewRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_view_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_view_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.view import View
+    from rockset_v2.model.view import View
     globals()['View'] = View
 
 
 class CreateViewResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_virtual_instance_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_query_lambda_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,34 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rockset_v2.model.query_lambda_sql import QueryLambdaSql
+    globals()['QueryLambdaSql'] = QueryLambdaSql
 
-class CreateVirtualInstanceRequest(ModelNormal):
+
+class UpdateQueryLambdaRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,84 +55,67 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
-        ('type',): {
-            'FREE': "FREE",
-            'NANO': "NANO",
-            'SHARED': "SHARED",
-            'MILLI': "MILLI",
-            'SMALL': "SMALL",
-            'MEDIUM': "MEDIUM",
-            'LARGE': "LARGE",
-            'XLARGE': "XLARGE",
-            'XLARGE2': "XLARGE2",
-            'XLARGE4': "XLARGE4",
-            'XLARGE8': "XLARGE8",
-            'XLARGE16': "XLARGE16",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'auto_suspend_seconds': (int, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
-            'type': (str, none_type),  # noqa: E501
+            'is_public': (bool, none_type),  # noqa: E501
+            'sql': (QueryLambdaSql, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'auto_suspend_seconds': 'auto_suspend_seconds',  # noqa: E501
         'description': 'description',  # noqa: E501
-        'type': 'type',  # noqa: E501
+        'is_public': 'is_public',  # noqa: E501
+        'sql': 'sql',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """CreateVirtualInstanceRequest - a model defined in OpenAPI
-
-        Args:
-            name (str): Unique identifier for virtual instance, can contain alphanumeric or dash characters.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """UpdateQueryLambdaRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -153,17 +140,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
-            description (str): Description of requested virtual instance.. [optional]  # noqa: E501
-            type (str): Requested virtual instance type.. [optional]  # noqa: E501
+            description (str): Optional description.. [optional]  # noqa: E501
+            is_public (bool): [optional]  # noqa: E501
+            sql (QueryLambdaSql): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +170,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -204,22 +190,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *, name, **kwargs):  # noqa: E501
-        """CreateVirtualInstanceRequest - a model defined in OpenAPI
+    def __init__(self, **kwargs):  # noqa: E501
+        """UpdateQueryLambdaRequest - a model defined in OpenAPI
 
         Keyword Args:
-            name (str): Unique identifier for virtual instance, can contain alphanumeric or dash characters.
-            auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
-            description (str): Description of requested virtual instance.. [optional]  # noqa: E501
-            type (str): Requested virtual instance type.. [optional]  # noqa: E501
+            description (str): Optional description.. [optional]  # noqa: E501
+            is_public (bool): [optional]  # noqa: E501
+            sql (QueryLambdaSql): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -268,15 +253,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_virtual_instance_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/suspend_virtual_instance_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.virtual_instance import VirtualInstance
+    from rockset_v2.model.virtual_instance import VirtualInstance
     globals()['VirtualInstance'] = VirtualInstance
 
 
-class CreateVirtualInstanceResponse(ModelNormal):
+class SuspendVirtualInstanceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -103,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CreateVirtualInstanceResponse - a model defined in OpenAPI
+        """SuspendVirtualInstanceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -185,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """CreateVirtualInstanceResponse - a model defined in OpenAPI
+        """SuspendVirtualInstanceResponse - a model defined in OpenAPI
 
         Keyword Args:
             data (VirtualInstance): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_workspace_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_workspace_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class CreateWorkspaceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/create_workspace_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_workspace_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.workspace import Workspace
+    from rockset_v2.model.workspace import Workspace
     globals()['Workspace'] = Workspace
 
 
 class CreateWorkspaceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/csv_params.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/csv_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class CsvParams(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/delete_alias_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/delete_alias_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.alias import Alias
+    from rockset_v2.model.alias import Alias
     globals()['Alias'] = Alias
 
 
 class DeleteAliasResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/delete_api_key_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/delete_api_key_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.api_key import ApiKey
+    from rockset_v2.model.api_key import ApiKey
     globals()['ApiKey'] = ApiKey
 
 
 class DeleteApiKeyResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/delete_collection_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/delete_collection_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.collection import Collection
+    from rockset_v2.model.collection import Collection
     globals()['Collection'] = Collection
 
 
 class DeleteCollectionResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/delete_documents_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/delete_documents_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.delete_documents_request_data import DeleteDocumentsRequestData
+    from rockset_v2.model.delete_documents_request_data import DeleteDocumentsRequestData
     globals()['DeleteDocumentsRequestData'] = DeleteDocumentsRequestData
 
 
 class DeleteDocumentsRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/delete_documents_request_data.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/delete_documents_request_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class DeleteDocumentsRequestData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/delete_documents_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/delete_documents_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.document_status import DocumentStatus
+    from rockset_v2.model.document_status import DocumentStatus
     globals()['DocumentStatus'] = DocumentStatus
 
 
 class DeleteDocumentsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/delete_integration_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_integration_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def lazy_import():
     from rockset.model.integration import Integration
     globals()['Integration'] = Integration
 
 
-class DeleteIntegrationResponse(ModelNormal):
+class UpdateIntegrationResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -103,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DeleteIntegrationResponse - a model defined in OpenAPI
+        """UpdateIntegrationResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -185,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """DeleteIntegrationResponse - a model defined in OpenAPI
+        """UpdateIntegrationResponse - a model defined in OpenAPI
 
         Keyword Args:
             data (Integration): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/delete_query_lambda_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/delete_query_lambda_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_lambda import QueryLambda
+    from rockset_v2.model.query_lambda import QueryLambda
     globals()['QueryLambda'] = QueryLambda
 
 
 class DeleteQueryLambdaResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/delete_user_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/delete_user_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.user import User
+    from rockset_v2.model.user import User
     globals()['User'] = User
 
 
 class DeleteUserResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/delete_view_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/delete_view_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.view import View
+    from rockset_v2.model.view import View
     globals()['View'] = View
 
 
 class DeleteViewResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/delete_virtual_instance_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/delete_virtual_instance_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.virtual_instance import VirtualInstance
+    from rockset_v2.model.virtual_instance import VirtualInstance
     globals()['VirtualInstance'] = VirtualInstance
 
 
 class DeleteVirtualInstanceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/delete_workspace_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/delete_workspace_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.workspace import Workspace
+    from rockset_v2.model.workspace import Workspace
     globals()['Workspace'] = Workspace
 
 
 class DeleteWorkspaceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/document_status.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/document_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.error_model import ErrorModel
+    from rockset_v2.model.error_model import ErrorModel
     globals()['ErrorModel'] = ErrorModel
 
 
 class DocumentStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/dynamodb_collection_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_collection_creation_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,42 +7,40 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.dynamodb_source_wrapper import DynamodbSourceWrapper
-    from rockset.model.event_time_info import EventTimeInfo
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
+    from rockset_v2.model.dynamodb_source_wrapper import DynamodbSourceWrapper
+    from rockset_v2.model.event_time_info import EventTimeInfo
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_partition import FieldPartition
     globals()['DynamodbSourceWrapper'] = DynamodbSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
 
 
 class DynamodbCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,33 +101,33 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
             'sources': ([DynamodbSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
             sources ([DynamodbSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -228,17 +230,17 @@
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
             sources ([DynamodbSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/dynamodb_integration.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.aws_access_key import AwsAccessKey
-    from rockset.model.aws_role import AwsRole
+    from rockset_v2.model.aws_access_key import AwsAccessKey
+    from rockset_v2.model.aws_role import AwsRole
     globals()['AwsAccessKey'] = AwsAccessKey
     globals()['AwsRole'] = AwsRole
 
 
 class DynamodbIntegration(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/dynamodb_integration_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_integration_creation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.dynamodb_integration import DynamodbIntegration
+    from rockset_v2.model.dynamodb_integration import DynamodbIntegration
     globals()['DynamodbIntegration'] = DynamodbIntegration
 
 
 class DynamodbIntegrationCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/dynamodb_source_wrapper.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/dynamodb_source_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,36 +7,36 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status_dynamo_db import StatusDynamoDb
-    from rockset.model.status_dynamo_db_v2 import StatusDynamoDbV2
+    from rockset_v2.model.format_params import FormatParams
+    from rockset_v2.model.status_dynamo_db import StatusDynamoDb
+    from rockset_v2.model.status_dynamo_db_v2 import StatusDynamoDbV2
     globals()['FormatParams'] = FormatParams
     globals()['StatusDynamoDb'] = StatusDynamoDb
     globals()['StatusDynamoDbV2'] = StatusDynamoDbV2
 
 
 class DynamodbSourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/error_model.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/error_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class ErrorModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/event_time_info.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/event_time_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class EventTimeInfo(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/execute_public_query_lambda_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/execute_public_query_lambda_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_parameter import QueryParameter
+    from rockset_v2.model.query_parameter import QueryParameter
     globals()['QueryParameter'] = QueryParameter
 
 
 class ExecutePublicQueryLambdaRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/execute_query_lambda_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/execute_query_lambda_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.async_query_options import AsyncQueryOptions
-    from rockset.model.query_parameter import QueryParameter
+    from rockset_v2.model.async_query_options import AsyncQueryOptions
+    from rockset_v2.model.query_parameter import QueryParameter
     globals()['AsyncQueryOptions'] = AsyncQueryOptions
     globals()['QueryParameter'] = QueryParameter
 
 
 class ExecuteQueryLambdaRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -91,14 +91,15 @@
         return {
             'async_options': (AsyncQueryOptions, none_type),  # noqa: E501
             'default_row_limit': (int, none_type),  # noqa: E501
             'generate_warnings': (bool, none_type),  # noqa: E501
             'initial_paginate_response_doc_count': (int, none_type),  # noqa: E501
             'paginate': (bool, none_type),  # noqa: E501
             'parameters': ([QueryParameter], none_type),  # noqa: E501
+            'timeout_ms': (int, none_type),  # noqa: E501
             'virtual_instance_id': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -106,14 +107,15 @@
     attribute_map = {
         'async_options': 'async_options',  # noqa: E501
         'default_row_limit': 'default_row_limit',  # noqa: E501
         'generate_warnings': 'generate_warnings',  # noqa: E501
         'initial_paginate_response_doc_count': 'initial_paginate_response_doc_count',  # noqa: E501
         'paginate': 'paginate',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
+        'timeout_ms': 'timeout_ms',  # noqa: E501
         'virtual_instance_id': 'virtual_instance_id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -156,14 +158,15 @@
                                 _visited_composed_classes = (Animal,)
             async_options (AsyncQueryOptions): [optional]  # noqa: E501
             default_row_limit (int): Row limit to use if no limit specified in the SQL query text.. [optional]  # noqa: E501
             generate_warnings (bool): Whether to generate warnings.. [optional]  # noqa: E501
             initial_paginate_response_doc_count (int): Number of documents to return in addition to paginating for this query call. Only relevant if `paginate` flag is also set.. [optional]  # noqa: E501
             paginate (bool): Flag to paginate and store the results of this query for later / sequential retrieval.. [optional]  # noqa: E501
             parameters ([QueryParameter]): List of named parameters.. [optional]  # noqa: E501
+            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error. The maximum value for this timeout is 2 minutes. async_options.timeout_ms will override this timeout.. [optional]  # noqa: E501
             virtual_instance_id (str): Virtual instance on which to run the query.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -214,14 +217,15 @@
         Keyword Args:
             async_options (AsyncQueryOptions): [optional]  # noqa: E501
             default_row_limit (int): Row limit to use if no limit specified in the SQL query text.. [optional]  # noqa: E501
             generate_warnings (bool): Whether to generate warnings.. [optional]  # noqa: E501
             initial_paginate_response_doc_count (int): Number of documents to return in addition to paginating for this query call. Only relevant if `paginate` flag is also set.. [optional]  # noqa: E501
             paginate (bool): Flag to paginate and store the results of this query for later / sequential retrieval.. [optional]  # noqa: E501
             parameters ([QueryParameter]): List of named parameters.. [optional]  # noqa: E501
+            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error. The maximum value for this timeout is 2 minutes. async_options.timeout_ms will override this timeout.. [optional]  # noqa: E501
             virtual_instance_id (str): Virtual instance on which to run the query.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/field_mapping_query.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/field_mapping_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class FieldMappingQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/field_mapping_v2.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/field_mapping_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.input_field import InputField
-    from rockset.model.output_field import OutputField
+    from rockset_v2.model.input_field import InputField
+    from rockset_v2.model.output_field import OutputField
     globals()['InputField'] = InputField
     globals()['OutputField'] = OutputField
 
 
 class FieldMappingV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/field_partition.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/field_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class FieldPartition(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/file_upload_collection_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/mongodb_collection_creation_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,46 +7,44 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.event_time_info import EventTimeInfo
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
-    from rockset.model.file_upload_source_wrapper import FileUploadSourceWrapper
+    from rockset_v2.model.event_time_info import EventTimeInfo
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_partition import FieldPartition
+    from rockset_v2.model.mongodb_source_wrapper import MongodbSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['FileUploadSourceWrapper'] = FileUploadSourceWrapper
+    globals()['MongodbSourceWrapper'] = MongodbSourceWrapper
 
 
-class FileUploadCollectionCreationRequest(ModelNormal):
+class MongodbCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([FileUploadSourceWrapper], none_type),  # noqa: E501
+            'sources': ([MongodbSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """FileUploadCollectionCreationRequest - a model defined in OpenAPI
+        """MongodbCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([FileUploadSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([MongodbSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """FileUploadCollectionCreationRequest - a model defined in OpenAPI
+        """MongodbCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([FileUploadSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([MongodbSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/file_upload_source_wrapper.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/file_upload_source_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status import Status
+    from rockset_v2.model.format_params import FormatParams
+    from rockset_v2.model.status import Status
     globals()['FormatParams'] = FormatParams
     globals()['Status'] = Status
 
 
 class FileUploadSourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/format_params.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/format_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.csv_params import CsvParams
-    from rockset.model.xml_params import XmlParams
+    from rockset_v2.model.csv_params import CsvParams
+    from rockset_v2.model.xml_params import XmlParams
     globals()['CsvParams'] = CsvParams
     globals()['XmlParams'] = XmlParams
 
 
 class FormatParams(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/gcp_service_account.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/gcp_service_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class GcpServiceAccount(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/gcs_collection_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_collection_creation_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,46 +7,44 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.event_time_info import EventTimeInfo
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
-    from rockset.model.gcs_source_wrapper import GcsSourceWrapper
+    from rockset_v2.model.event_time_info import EventTimeInfo
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_partition import FieldPartition
+    from rockset_v2.model.kinesis_source_wrapper import KinesisSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['GcsSourceWrapper'] = GcsSourceWrapper
+    globals()['KinesisSourceWrapper'] = KinesisSourceWrapper
 
 
-class GcsCollectionCreationRequest(ModelNormal):
+class KinesisCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([GcsSourceWrapper], none_type),  # noqa: E501
+            'sources': ([KinesisSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """GcsCollectionCreationRequest - a model defined in OpenAPI
+        """KinesisCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([GcsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([KinesisSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """GcsCollectionCreationRequest - a model defined in OpenAPI
+        """KinesisCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([GcsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([KinesisSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/gcs_integration.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/gcs_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.gcp_service_account import GcpServiceAccount
+    from rockset_v2.model.gcp_service_account import GcpServiceAccount
     globals()['GcpServiceAccount'] = GcpServiceAccount
 
 
 class GcsIntegration(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/gcs_integration_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/gcs_integration_creation_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.gcs_integration import GcsIntegration
+    from rockset_v2.model.gcs_integration import GcsIntegration
     globals()['GcsIntegration'] = GcsIntegration
 
 
 class GcsIntegrationCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/gcs_source_wrapper.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/gcs_source_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status import Status
+    from rockset_v2.model.format_params import FormatParams
+    from rockset_v2.model.status import Status
     globals()['FormatParams'] = FormatParams
     globals()['Status'] = Status
 
 
 class GcsSourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/get_alias_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/get_alias_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.alias import Alias
+    from rockset_v2.model.alias import Alias
     globals()['Alias'] = Alias
 
 
 class GetAliasResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/get_api_key_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/get_api_key_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.api_key import ApiKey
+    from rockset_v2.model.api_key import ApiKey
     globals()['ApiKey'] = ApiKey
 
 
 class GetApiKeyResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/get_collection_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_collection_mount_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,38 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rockset.model.collection import Collection
-    globals()['Collection'] = Collection
 
-
-class GetCollectionResponse(ModelNormal):
+class CreateCollectionMountRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,52 +62,50 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': (Collection, none_type),  # noqa: E501
+            'collection_paths': ([str], none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'collection_paths': 'collection_paths',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetCollectionResponse - a model defined in OpenAPI
+        """CreateCollectionMountRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (Collection): [optional]  # noqa: E501
+            collection_paths ([str]): Collections to mount.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,18 +179,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """GetCollectionResponse - a model defined in OpenAPI
+        """CreateCollectionMountRequest - a model defined in OpenAPI
 
         Keyword Args:
-            data (Collection): [optional]  # noqa: E501
+            collection_paths ([str]): Collections to mount.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/get_integration_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/get_integration_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.integration import Integration
+    from rockset_v2.model.integration import Integration
     globals()['Integration'] = Integration
 
 
 class GetIntegrationResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/get_query_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/get_query_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_info import QueryInfo
+    from rockset_v2.model.query_info import QueryInfo
     globals()['QueryInfo'] = QueryInfo
 
 
 class GetQueryResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/get_view_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/get_view_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.view import View
+    from rockset_v2.model.view import View
     globals()['View'] = View
 
 
 class GetViewResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/get_virtual_instance_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/resume_virtual_instance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.virtual_instance import VirtualInstance
+    from rockset_v2.model.virtual_instance import VirtualInstance
     globals()['VirtualInstance'] = VirtualInstance
 
 
-class GetVirtualInstanceResponse(ModelNormal):
+class ResumeVirtualInstanceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -103,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetVirtualInstanceResponse - a model defined in OpenAPI
+        """ResumeVirtualInstanceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -185,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """GetVirtualInstanceResponse - a model defined in OpenAPI
+        """ResumeVirtualInstanceResponse - a model defined in OpenAPI
 
         Keyword Args:
             data (VirtualInstance): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/get_workspace_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/role_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.workspace import Workspace
-    globals()['Workspace'] = Workspace
+    from rockset_v2.model.role import Role
+    globals()['Role'] = Role
 
 
-class GetWorkspaceResponse(ModelNormal):
+class RoleResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,15 +83,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (Workspace, none_type),  # noqa: E501
+            'data': (Role, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -103,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetWorkspaceResponse - a model defined in OpenAPI
+        """RoleResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (Workspace): [optional]  # noqa: E501
+            data (Role): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,18 +185,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """GetWorkspaceResponse - a model defined in OpenAPI
+        """RoleResponse - a model defined in OpenAPI
 
         Keyword Args:
-            data (Workspace): [optional]  # noqa: E501
+            data (Role): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/input_field.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/input_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class InputField(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/integration.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,44 +7,44 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.azure_blob_storage_integration import AzureBlobStorageIntegration
-    from rockset.model.azure_event_hubs_integration import AzureEventHubsIntegration
-    from rockset.model.azure_service_bus_integration import AzureServiceBusIntegration
-    from rockset.model.collection import Collection
-    from rockset.model.dynamodb_integration import DynamodbIntegration
-    from rockset.model.gcs_integration import GcsIntegration
-    from rockset.model.kafka_integration import KafkaIntegration
-    from rockset.model.kinesis_integration import KinesisIntegration
-    from rockset.model.mongo_db_integration import MongoDbIntegration
-    from rockset.model.s3_integration import S3Integration
-    from rockset.model.snowflake_integration import SnowflakeIntegration
+    from rockset_v2.model.azure_blob_storage_integration import AzureBlobStorageIntegration
+    from rockset_v2.model.azure_event_hubs_integration import AzureEventHubsIntegration
+    from rockset_v2.model.azure_service_bus_integration import AzureServiceBusIntegration
+    from rockset_v2.model.collection import Collection
+    from rockset_v2.model.dynamodb_integration import DynamodbIntegration
+    from rockset_v2.model.gcs_integration import GcsIntegration
+    from rockset_v2.model.kafka_integration import KafkaIntegration
+    from rockset_v2.model.kinesis_integration import KinesisIntegration
+    from rockset_v2.model.mongo_db_integration import MongoDbIntegration
+    from rockset_v2.model.s3_integration import S3Integration
+    from rockset_v2.model.snowflake_integration import SnowflakeIntegration
     globals()['AzureBlobStorageIntegration'] = AzureBlobStorageIntegration
     globals()['AzureEventHubsIntegration'] = AzureEventHubsIntegration
     globals()['AzureServiceBusIntegration'] = AzureServiceBusIntegration
     globals()['Collection'] = Collection
     globals()['DynamodbIntegration'] = DynamodbIntegration
     globals()['GcsIntegration'] = GcsIntegration
     globals()['KafkaIntegration'] = KafkaIntegration
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/kafka_collection_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/s3_collection_creation_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,46 +7,44 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.event_time_info import EventTimeInfo
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
-    from rockset.model.kafka_source_wrapper import KafkaSourceWrapper
+    from rockset_v2.model.event_time_info import EventTimeInfo
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_partition import FieldPartition
+    from rockset_v2.model.s3_source_wrapper import S3SourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['KafkaSourceWrapper'] = KafkaSourceWrapper
+    globals()['S3SourceWrapper'] = S3SourceWrapper
 
 
-class KafkaCollectionCreationRequest(ModelNormal):
+class S3CollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([KafkaSourceWrapper], none_type),  # noqa: E501
+            'sources': ([S3SourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """KafkaCollectionCreationRequest - a model defined in OpenAPI
+        """S3CollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([KafkaSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([S3SourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """KafkaCollectionCreationRequest - a model defined in OpenAPI
+        """S3CollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([KafkaSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([S3SourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/kafka_integration.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/kafka_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,37 +7,37 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.aws_role import AwsRole
-    from rockset.model.kafka_v3_security_config import KafkaV3SecurityConfig
-    from rockset.model.schema_registry_config import SchemaRegistryConfig
-    from rockset.model.status_kafka import StatusKafka
+    from rockset_v2.model.aws_role import AwsRole
+    from rockset_v2.model.kafka_v3_security_config import KafkaV3SecurityConfig
+    from rockset_v2.model.schema_registry_config import SchemaRegistryConfig
+    from rockset_v2.model.status_kafka import StatusKafka
     globals()['AwsRole'] = AwsRole
     globals()['KafkaV3SecurityConfig'] = KafkaV3SecurityConfig
     globals()['SchemaRegistryConfig'] = SchemaRegistryConfig
     globals()['StatusKafka'] = StatusKafka
 
 
 class KafkaIntegration(ModelNormal):
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/kafka_integration_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/kafka_integration_creation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.kafka_integration import KafkaIntegration
+    from rockset_v2.model.kafka_integration import KafkaIntegration
     globals()['KafkaIntegration'] = KafkaIntegration
 
 
 class KafkaIntegrationCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/kafka_source_wrapper.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/kafka_source_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status_kafka import StatusKafka
+    from rockset_v2.model.format_params import FormatParams
+    from rockset_v2.model.status_kafka import StatusKafka
     globals()['FormatParams'] = FormatParams
     globals()['StatusKafka'] = StatusKafka
 
 
 class KafkaSourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/kafka_v3_security_config.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/kafka_v3_security_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class KafkaV3SecurityConfig(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/kinesis_collection_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/azure_service_bus_collection_creation_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,46 +7,44 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.event_time_info import EventTimeInfo
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
-    from rockset.model.kinesis_source_wrapper import KinesisSourceWrapper
+    from rockset_v2.model.azure_service_bus_source_wrapper import AzureServiceBusSourceWrapper
+    from rockset_v2.model.event_time_info import EventTimeInfo
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_partition import FieldPartition
+    globals()['AzureServiceBusSourceWrapper'] = AzureServiceBusSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['KinesisSourceWrapper'] = KinesisSourceWrapper
 
 
-class KinesisCollectionCreationRequest(ModelNormal):
+class AzureServiceBusCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([KinesisSourceWrapper], none_type),  # noqa: E501
+            'sources': ([AzureServiceBusSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """KinesisCollectionCreationRequest - a model defined in OpenAPI
+        """AzureServiceBusCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([KinesisSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([AzureServiceBusSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """KinesisCollectionCreationRequest - a model defined in OpenAPI
+        """AzureServiceBusCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([KinesisSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([AzureServiceBusSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/kinesis_integration.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.aws_access_key import AwsAccessKey
-    from rockset.model.aws_role import AwsRole
+    from rockset_v2.model.aws_access_key import AwsAccessKey
+    from rockset_v2.model.aws_role import AwsRole
     globals()['AwsAccessKey'] = AwsAccessKey
     globals()['AwsRole'] = AwsRole
 
 
 class KinesisIntegration(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/kinesis_integration_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_integration_creation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.kinesis_integration import KinesisIntegration
+    from rockset_v2.model.kinesis_integration import KinesisIntegration
     globals()['KinesisIntegration'] = KinesisIntegration
 
 
 class KinesisIntegrationCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/kinesis_source_wrapper.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/kinesis_source_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status import Status
+    from rockset_v2.model.format_params import FormatParams
+    from rockset_v2.model.status import Status
     globals()['FormatParams'] = FormatParams
     globals()['Status'] = Status
 
 
 class KinesisSourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_aliases_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_aliases_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.alias import Alias
+    from rockset_v2.model.alias import Alias
     globals()['Alias'] = Alias
 
 
 class ListAliasesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_api_keys_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_api_keys_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.api_key import ApiKey
+    from rockset_v2.model.api_key import ApiKey
     globals()['ApiKey'] = ApiKey
 
 
 class ListApiKeysResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_collection_mounts_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_collection_mounts_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.collection_mount import CollectionMount
+    from rockset_v2.model.collection_mount import CollectionMount
     globals()['CollectionMount'] = CollectionMount
 
 
 class ListCollectionMountsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_collections_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_collections_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.collection import Collection
+    from rockset_v2.model.collection import Collection
     globals()['Collection'] = Collection
 
 
 class ListCollectionsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_integrations_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_integrations_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.integration import Integration
+    from rockset_v2.model.integration import Integration
     globals()['Integration'] = Integration
 
 
 class ListIntegrationsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_queries_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_queries_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_info import QueryInfo
+    from rockset_v2.model.query_info import QueryInfo
     globals()['QueryInfo'] = QueryInfo
 
 
 class ListQueriesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_query_lambda_tags_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_query_lambda_tags_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_lambda_tag import QueryLambdaTag
+    from rockset_v2.model.query_lambda_tag import QueryLambdaTag
     globals()['QueryLambdaTag'] = QueryLambdaTag
 
 
 class ListQueryLambdaTagsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_query_lambda_versions_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_query_lambda_versions_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_lambda_version import QueryLambdaVersion
+    from rockset_v2.model.query_lambda_version import QueryLambdaVersion
     globals()['QueryLambdaVersion'] = QueryLambdaVersion
 
 
 class ListQueryLambdaVersionsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_query_lambdas_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_query_lambdas_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_lambda import QueryLambda
+    from rockset_v2.model.query_lambda import QueryLambda
     globals()['QueryLambda'] = QueryLambda
 
 
 class ListQueryLambdasResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_roles_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_roles_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.role import Role
+    from rockset_v2.model.role import Role
     globals()['Role'] = Role
 
 
 class ListRolesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_unsubscribe_preferences_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_unsubscribe_preferences_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.unsubscribe_preference import UnsubscribePreference
+    from rockset_v2.model.unsubscribe_preference import UnsubscribePreference
     globals()['UnsubscribePreference'] = UnsubscribePreference
 
 
 class ListUnsubscribePreferencesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_users_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_users_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.user import User
+    from rockset_v2.model.user import User
     globals()['User'] = User
 
 
 class ListUsersResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_views_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_views_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.view import View
+    from rockset_v2.model.view import View
     globals()['View'] = View
 
 
 class ListViewsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_virtual_instances_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_virtual_instances_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.virtual_instance import VirtualInstance
+    from rockset_v2.model.virtual_instance import VirtualInstance
     globals()['VirtualInstance'] = VirtualInstance
 
 
 class ListVirtualInstancesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/list_workspaces_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/list_workspaces_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.workspace import Workspace
+    from rockset_v2.model.workspace import Workspace
     globals()['Workspace'] = Workspace
 
 
 class ListWorkspacesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/mongo_db_integration.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/mongo_db_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class MongoDbIntegration(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/mongodb_collection_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/azure_event_hubs_collection_creation_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,46 +7,44 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.event_time_info import EventTimeInfo
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
-    from rockset.model.mongodb_source_wrapper import MongodbSourceWrapper
+    from rockset_v2.model.azure_event_hubs_source_wrapper import AzureEventHubsSourceWrapper
+    from rockset_v2.model.event_time_info import EventTimeInfo
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_partition import FieldPartition
+    globals()['AzureEventHubsSourceWrapper'] = AzureEventHubsSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['MongodbSourceWrapper'] = MongodbSourceWrapper
 
 
-class MongodbCollectionCreationRequest(ModelNormal):
+class AzureEventHubsCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([MongodbSourceWrapper], none_type),  # noqa: E501
+            'sources': ([AzureEventHubsSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """MongodbCollectionCreationRequest - a model defined in OpenAPI
+        """AzureEventHubsCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([MongodbSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([AzureEventHubsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """MongodbCollectionCreationRequest - a model defined in OpenAPI
+        """AzureEventHubsCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([MongodbSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([AzureEventHubsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/mongodb_integration_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/mongodb_integration_creation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.mongo_db_integration import MongoDbIntegration
+    from rockset_v2.model.mongo_db_integration import MongoDbIntegration
     globals()['MongoDbIntegration'] = MongoDbIntegration
 
 
 class MongodbIntegrationCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/mongodb_source_wrapper.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,40 +7,40 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status_mongo_db import StatusMongoDb
+    from rockset_v2.model.format_params import FormatParams
+    from rockset_v2.model.status import Status
     globals()['FormatParams'] = FormatParams
-    globals()['StatusMongoDb'] = StatusMongoDb
+    globals()['Status'] = Status
 
 
-class MongodbSourceWrapper(ModelNormal):
+class Source(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,16 +55,15 @@
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
-    inner_field = "mongodb"
-    inner_properties = ["collection_name", "database_name", "status"]
+    
     allowed_values = {
     }
 
     validations = {
     }
 
     @cached_property
@@ -86,48 +85,40 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'collection_name': (str,),  # noqa: E501
-            'database_name': (str,),  # noqa: E501
             'format_params': (FormatParams, none_type),  # noqa: E501
             'integration_name': (str, none_type),  # noqa: E501
             'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'collection_name': 'collection_name',  # noqa: E501
-        'database_name': 'database_name',  # noqa: E501
         'format_params': 'format_params',  # noqa: E501
         'integration_name': 'integration_name',  # noqa: E501
         'status': 'status',  # noqa: E501
     }
 
     read_only_vars = {
         'status',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, collection_name, database_name, *args, **kwargs):  # noqa: E501
-        """MongodbSourceWrapper - a model defined in OpenAPI
-
-        Args:
-            collection_name (str): MongoDB collection name.
-            database_name (str): MongoDB database name containing this collection.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Source - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,16 +173,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.collection_name = collection_name
-        self.database_name = database_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -204,20 +193,18 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *, collection_name, database_name, **kwargs):  # noqa: E501
-        """MongodbSourceWrapper - a model defined in OpenAPI
+    def __init__(self, **kwargs):  # noqa: E501
+        """Source - a model defined in OpenAPI
 
         Keyword Args:
-            collection_name (str): MongoDB collection name.
-            database_name (str): MongoDB database name containing this collection.
             format_params (FormatParams): [optional]  # noqa: E501
             integration_name (str): Name of integration to use.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -268,16 +255,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.collection_name = collection_name
-        self.database_name = database_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/organization.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.cluster import Cluster
+    from rockset_v2.model.cluster import Cluster
     globals()['Cluster'] = Cluster
 
 
 class Organization(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/organization_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/organization_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.organization import Organization
+    from rockset_v2.model.organization import Organization
     globals()['Organization'] = Organization
 
 
 class OrganizationResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/output_field.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/output_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.sql_expression import SqlExpression
+    from rockset_v2.model.sql_expression import SqlExpression
     globals()['SqlExpression'] = SqlExpression
 
 
 class OutputField(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/pagination.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class Pagination(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/pagination_info.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/pagination_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class PaginationInfo(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/patch_document.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/patch_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.patch_operation import PatchOperation
+    from rockset_v2.model.patch_operation import PatchOperation
     globals()['PatchOperation'] = PatchOperation
 
 
 class PatchDocument(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/patch_documents_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/patch_documents_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.patch_document import PatchDocument
+    from rockset_v2.model.patch_document import PatchDocument
     globals()['PatchDocument'] = PatchDocument
 
 
 class PatchDocumentsRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/patch_documents_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/patch_documents_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.document_status import DocumentStatus
+    from rockset_v2.model.document_status import DocumentStatus
     globals()['DocumentStatus'] = DocumentStatus
 
 
 class PatchDocumentsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/patch_operation.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/patch_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class PatchOperation(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/privilege.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/privilege.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class Privilege(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_error.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class QueryError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_field_type.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_field_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class QueryFieldType(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_info.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,36 +7,36 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.pagination import Pagination
-    from rockset.model.query_error import QueryError
-    from rockset.model.stats import Stats
+    from rockset_v2.model.pagination import Pagination
+    from rockset_v2.model.query_error import QueryError
+    from rockset_v2.model.stats import Stats
     globals()['Pagination'] = Pagination
     globals()['QueryError'] = QueryError
     globals()['Stats'] = Stats
 
 
 class QueryInfo(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
@@ -100,14 +100,15 @@
         return {
             'executed_by': (str, none_type),  # noqa: E501
             'expires_at': (str, none_type),  # noqa: E501
             'last_offset': (str, none_type),  # noqa: E501
             'pagination': (Pagination, none_type),  # noqa: E501
             'query_errors': ([QueryError], none_type),  # noqa: E501
             'query_id': (str, none_type),  # noqa: E501
+            'sql': (str, none_type),  # noqa: E501
             'stats': (Stats, none_type),  # noqa: E501
             'status': (str, none_type),  # noqa: E501
             'submitted_at': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -117,14 +118,15 @@
     attribute_map = {
         'executed_by': 'executed_by',  # noqa: E501
         'expires_at': 'expires_at',  # noqa: E501
         'last_offset': 'last_offset',  # noqa: E501
         'pagination': 'pagination',  # noqa: E501
         'query_errors': 'query_errors',  # noqa: E501
         'query_id': 'query_id',  # noqa: E501
+        'sql': 'sql',  # noqa: E501
         'stats': 'stats',  # noqa: E501
         'status': 'status',  # noqa: E501
         'submitted_at': 'submitted_at',  # noqa: E501
     }
 
     read_only_vars = {
     }
@@ -169,14 +171,15 @@
                                 _visited_composed_classes = (Animal,)
             executed_by (str): User ID who executed the query.. [optional]  # noqa: E501
             expires_at (str): Time (UTC) that query results expire. Only populated if `status` is `COMPLETE`.. [optional]  # noqa: E501
             last_offset (str): The log offset that query results were written to in the destination collection. Only populated for INSERT INTO queries.. [optional]  # noqa: E501
             pagination (Pagination): [optional]  # noqa: E501
             query_errors ([QueryError]): Errors encountered while executing the query.. [optional]  # noqa: E501
             query_id (str): Unique Query ID.. [optional]  # noqa: E501
+            sql (str): The SQL query for this request. [optional]  # noqa: E501
             stats (Stats): [optional]  # noqa: E501
             status (str): Status of the query.. [optional]  # noqa: E501
             submitted_at (str): Time (UTC) the query request was first received and queued for execution.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -229,14 +232,15 @@
         Keyword Args:
             executed_by (str): User ID who executed the query.. [optional]  # noqa: E501
             expires_at (str): Time (UTC) that query results expire. Only populated if `status` is `COMPLETE`.. [optional]  # noqa: E501
             last_offset (str): The log offset that query results were written to in the destination collection. Only populated for INSERT INTO queries.. [optional]  # noqa: E501
             pagination (Pagination): [optional]  # noqa: E501
             query_errors ([QueryError]): Errors encountered while executing the query.. [optional]  # noqa: E501
             query_id (str): Unique Query ID.. [optional]  # noqa: E501
+            sql (str): The SQL query for this request. [optional]  # noqa: E501
             stats (Stats): [optional]  # noqa: E501
             status (str): Status of the query.. [optional]  # noqa: E501
             submitted_at (str): Time (UTC) the query request was first received and queued for execution.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_lambda_version import QueryLambdaVersion
+    from rockset_v2.model.query_lambda_version import QueryLambdaVersion
     globals()['QueryLambdaVersion'] = QueryLambdaVersion
 
 
 class QueryLambda(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda_sql.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_parameter import QueryParameter
+    from rockset_v2.model.query_parameter import QueryParameter
     globals()['QueryParameter'] = QueryParameter
 
 
 class QueryLambdaSql(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda_stats.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class QueryLambdaStats(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda_tag.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_lambda_version import QueryLambdaVersion
+    from rockset_v2.model.query_lambda_version import QueryLambdaVersion
     globals()['QueryLambdaVersion'] = QueryLambdaVersion
 
 
 class QueryLambdaTag(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda_tag_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_tag_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_lambda_tag import QueryLambdaTag
+    from rockset_v2.model.query_lambda_tag import QueryLambdaTag
     globals()['QueryLambdaTag'] = QueryLambdaTag
 
 
 class QueryLambdaTagResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda_version.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/collection_mount.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,40 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_lambda_sql import QueryLambdaSql
-    from rockset.model.query_lambda_stats import QueryLambdaStats
-    globals()['QueryLambdaSql'] = QueryLambdaSql
-    globals()['QueryLambdaStats'] = QueryLambdaStats
+    from rockset_v2.model.collection_mount_stats import CollectionMountStats
+    globals()['CollectionMountStats'] = CollectionMountStats
 
 
-class QueryLambdaVersion(ModelNormal):
+class CollectionMount(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -58,16 +56,22 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
         ('state',): {
+            'CREATING': "CREATING",
             'ACTIVE': "ACTIVE",
-            'INVALID_SQL': "INVALID_SQL",
+            'REFRESHING': "REFRESHING",
+            'EXPIRED': "EXPIRED",
+            'DELETING': "DELETING",
+            'SWITCHING_REFRESH_TYPE': "SWITCHING_REFRESH_TYPE",
+            'SUSPENDED': "SUSPENDED",
+            'SUSPENDING': "SUSPENDING",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -89,55 +93,53 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'collections': ([str], none_type),  # noqa: E501
+            'collection_path': (str, none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
-            'created_by': (str, none_type),  # noqa: E501
-            'description': (str, none_type),  # noqa: E501
-            'name': (str, none_type),  # noqa: E501
-            'public_access_id': (str, none_type),  # noqa: E501
-            'sql': (QueryLambdaSql, none_type),  # noqa: E501
+            'id': (str, none_type),  # noqa: E501
+            'last_refresh_time_millis': (int, none_type),  # noqa: E501
+            'rrn': (str, none_type),  # noqa: E501
+            'snapshot_expiration_time_millis': (int, none_type),  # noqa: E501
             'state': (str, none_type),  # noqa: E501
-            'stats': (QueryLambdaStats, none_type),  # noqa: E501
-            'version': (str, none_type),  # noqa: E501
-            'workspace': (str, none_type),  # noqa: E501
+            'stats': (CollectionMountStats, none_type),  # noqa: E501
+            'virtual_instance_id': (str, none_type),  # noqa: E501
+            'virtual_instance_rrn': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'collections': 'collections',  # noqa: E501
+        'collection_path': 'collection_path',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
-        'created_by': 'created_by',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'public_access_id': 'public_access_id',  # noqa: E501
-        'sql': 'sql',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'last_refresh_time_millis': 'last_refresh_time_millis',  # noqa: E501
+        'rrn': 'rrn',  # noqa: E501
+        'snapshot_expiration_time_millis': 'snapshot_expiration_time_millis',  # noqa: E501
         'state': 'state',  # noqa: E501
         'stats': 'stats',  # noqa: E501
-        'version': 'version',  # noqa: E501
-        'workspace': 'workspace',  # noqa: E501
+        'virtual_instance_id': 'virtual_instance_id',  # noqa: E501
+        'virtual_instance_rrn': 'virtual_instance_rrn',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """QueryLambdaVersion - a model defined in OpenAPI
+        """CollectionMount - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -162,25 +164,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            collections ([str]): Collections queried by underlying SQL query.. [optional]  # noqa: E501
-            created_at (str): ISO-8601 date of when Query Lambda was created.. [optional]  # noqa: E501
-            created_by (str): User that created this Query Lambda.. [optional]  # noqa: E501
-            description (str): Optional description.. [optional]  # noqa: E501
-            name (str): Query Lambda name.. [optional]  # noqa: E501
-            public_access_id (str): Public access ID associated with this QL version. [optional]  # noqa: E501
-            sql (QueryLambdaSql): [optional]  # noqa: E501
-            state (str): Status of this Query Lambda.. [optional]  # noqa: E501
-            stats (QueryLambdaStats): [optional]  # noqa: E501
-            version (str): Query Lambda version.. [optional]  # noqa: E501
-            workspace (str): Workspace of this Query Lambda.. [optional]  # noqa: E501
+            collection_path (str): Collection path.. [optional]  # noqa: E501
+            created_at (str): ISO-8601 date.. [optional]  # noqa: E501
+            id (str): Mount ID.. [optional]  # noqa: E501
+            last_refresh_time_millis (int): Unix timestamp of most recent refresh. Not applicable for live mounts.. [optional]  # noqa: E501
+            rrn (str): Mount RRN.. [optional]  # noqa: E501
+            snapshot_expiration_time_millis (int): Time in millis at which the snapshot expires.. [optional]  # noqa: E501
+            state (str): Mount type.. [optional]  # noqa: E501
+            stats (CollectionMountStats): [optional]  # noqa: E501
+            virtual_instance_id (str): Virtual instance ID.. [optional]  # noqa: E501
+            virtual_instance_rrn (str): Virtual Instance RRN.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -221,28 +222,27 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """QueryLambdaVersion - a model defined in OpenAPI
+        """CollectionMount - a model defined in OpenAPI
 
         Keyword Args:
-            collections ([str]): Collections queried by underlying SQL query.. [optional]  # noqa: E501
-            created_at (str): ISO-8601 date of when Query Lambda was created.. [optional]  # noqa: E501
-            created_by (str): User that created this Query Lambda.. [optional]  # noqa: E501
-            description (str): Optional description.. [optional]  # noqa: E501
-            name (str): Query Lambda name.. [optional]  # noqa: E501
-            public_access_id (str): Public access ID associated with this QL version. [optional]  # noqa: E501
-            sql (QueryLambdaSql): [optional]  # noqa: E501
-            state (str): Status of this Query Lambda.. [optional]  # noqa: E501
-            stats (QueryLambdaStats): [optional]  # noqa: E501
-            version (str): Query Lambda version.. [optional]  # noqa: E501
-            workspace (str): Workspace of this Query Lambda.. [optional]  # noqa: E501
+            collection_path (str): Collection path.. [optional]  # noqa: E501
+            created_at (str): ISO-8601 date.. [optional]  # noqa: E501
+            id (str): Mount ID.. [optional]  # noqa: E501
+            last_refresh_time_millis (int): Unix timestamp of most recent refresh. Not applicable for live mounts.. [optional]  # noqa: E501
+            rrn (str): Mount RRN.. [optional]  # noqa: E501
+            snapshot_expiration_time_millis (int): Time in millis at which the snapshot expires.. [optional]  # noqa: E501
+            state (str): Mount type.. [optional]  # noqa: E501
+            stats (CollectionMountStats): [optional]  # noqa: E501
+            virtual_instance_id (str): Virtual instance ID.. [optional]  # noqa: E501
+            virtual_instance_rrn (str): Virtual Instance RRN.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_lambda_version_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_lambda_version_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_lambda_version import QueryLambdaVersion
+    from rockset_v2.model.query_lambda_version import QueryLambdaVersion
     globals()['QueryLambdaVersion'] = QueryLambdaVersion
 
 
 class QueryLambdaVersionResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_pagination_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_pagination_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
-from rockset.document import Document
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.pagination_info import PaginationInfo
+    from rockset_v2.model.pagination_info import PaginationInfo
     globals()['PaginationInfo'] = PaginationInfo
 
 
 class QueryPaginationResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -178,17 +177,14 @@
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
-            if var_name == "results":
-                setattr(self, "results", [Document(doc) for doc in var_value])
-                continue
             setattr(self, var_name, var_value)
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
@@ -264,15 +260,12 @@
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
-            if var_name == "results":
-                setattr(self, "results", [Document(doc) for doc in var_value])
-                continue
             setattr(self, var_name, var_value)
             # todo: remove these comments - this stops the user from setting read only vars but we need this now to address a bug
             # if var_name in self.read_only_vars:
             #     raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
             #                          f"class with read only attributes.")
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_parameter.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class QueryParameter(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -105,15 +105,15 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, type, value, *args, **kwargs):  # noqa: E501
         """QueryParameter - a model defined in OpenAPI
 
         Args:
             name (str): Name of the field.
-            type (str): Data type of the field.
+            type (str): Deprecated. Data type of the field.
             value (str): Literal value of the field.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -194,15 +194,15 @@
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, type, value, **kwargs):  # noqa: E501
         """QueryParameter - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Name of the field.
-            type (str): Data type of the field.
+            type (str): Deprecated. Data type of the field.
             value (str): Literal value of the field.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_alias_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,40 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rockset.model.async_query_options import AsyncQueryOptions
-    from rockset.model.query_request_sql import QueryRequestSql
-    globals()['AsyncQueryOptions'] = AsyncQueryOptions
-    globals()['QueryRequestSql'] = QueryRequestSql
 
-
-class QueryRequest(ModelNormal):
+class UpdateAliasRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -68,57 +62,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'sql': (QueryRequestSql,),  # noqa: E501
-            'async_options': (AsyncQueryOptions, none_type),  # noqa: E501
+            'collections': ([str],),  # noqa: E501
+            'description': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'sql': 'sql',  # noqa: E501
-        'async_options': 'async_options',  # noqa: E501
+        'collections': 'collections',  # noqa: E501
+        'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, sql, *args, **kwargs):  # noqa: E501
-        """QueryRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, collections, *args, **kwargs):  # noqa: E501
+        """UpdateAliasRequest - a model defined in OpenAPI
 
         Args:
-            sql (QueryRequestSql):
+            collections ([str]): List of fully qualified collection names referenced by alias.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,15 +135,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            async_options (AsyncQueryOptions): [optional]  # noqa: E501
+            description (str): Optional description.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,15 +163,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.sql = sql
+        self.collections = collections
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,20 +184,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *, sql, **kwargs):  # noqa: E501
-        """QueryRequest - a model defined in OpenAPI
+    def __init__(self, *, collections, **kwargs):  # noqa: E501
+        """UpdateAliasRequest - a model defined in OpenAPI
 
         Keyword Args:
-            sql (QueryRequestSql):
-            async_options (AsyncQueryOptions): [optional]  # noqa: E501
+            collections ([str]): List of fully qualified collection names referenced by alias.
+            description (str): Optional description.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -254,15 +246,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.sql = sql
+        self.collections = collections
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_request_sql.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_request_sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_parameter import QueryParameter
+    from rockset_v2.model.query_parameter import QueryParameter
     globals()['QueryParameter'] = QueryParameter
 
 
 class QueryRequestSql(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -87,29 +87,27 @@
         """
         lazy_import()
         return {
             'query': (str,),  # noqa: E501
             'default_row_limit': (int, none_type),  # noqa: E501
             'generate_warnings': (bool, none_type),  # noqa: E501
             'initial_paginate_response_doc_count': (int, none_type),  # noqa: E501
-            'paginate': (bool, none_type),  # noqa: E501
             'parameters': ([QueryParameter], none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'query': 'query',  # noqa: E501
         'default_row_limit': 'default_row_limit',  # noqa: E501
         'generate_warnings': 'generate_warnings',  # noqa: E501
         'initial_paginate_response_doc_count': 'initial_paginate_response_doc_count',  # noqa: E501
-        'paginate': 'paginate',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -152,15 +150,14 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             default_row_limit (int): Row limit to use. Limits specified in the query text will override this default.. [optional]  # noqa: E501
             generate_warnings (bool): Flag to enable warnings. Warnings can help debug query issues but negatively affect performance.. [optional]  # noqa: E501
             initial_paginate_response_doc_count (int): Number of documents to return in addition to paginating for this query call. Only relevant if `paginate` flag is also set.. [optional]  # noqa: E501
-            paginate (bool): Flag to paginate and store the results of this query for later sequential retrieval.. [optional]  # noqa: E501
             parameters ([QueryParameter]): List of named parameters.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -210,15 +207,14 @@
         """QueryRequestSql - a model defined in OpenAPI
 
         Keyword Args:
             query (str): SQL query string.
             default_row_limit (int): Row limit to use. Limits specified in the query text will override this default.. [optional]  # noqa: E501
             generate_warnings (bool): Flag to enable warnings. Warnings can help debug query issues but negatively affect performance.. [optional]  # noqa: E501
             initial_paginate_response_doc_count (int): Number of documents to return in addition to paginating for this query call. Only relevant if `paginate` flag is also set.. [optional]  # noqa: E501
-            paginate (bool): Flag to paginate and store the results of this query for later sequential retrieval.. [optional]  # noqa: E501
             parameters ([QueryParameter]): List of named parameters.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 """
     REST API
 
     Rockset's REST API allows for creating and managing all resources in Rockset. Each supported endpoint is documented below.  All requests must be authorized with a Rockset API key, which can be created in the [Rockset console](https://console.rockset.com). The API key must be provided as `ApiKey <api_key>` in the `Authorization` request header. For example: ``` Authorization: ApiKey aB35kDjg93J5nsf4GjwMeErAVd832F7ad4vhsW1S02kfZiab42sTsfW5Sxt25asT ```  All endpoints are only accessible via https.  Build something awesome!  # noqa: E501
 
     The version of the OpenAPI document: v1
     Generated by: https://openapi-generator.tech
-    Not regenerated automatically
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
-    OpenApiModel,
+    OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
-from rockset.document import Document
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.pagination_info import PaginationInfo
-    from rockset.model.query_error import QueryError
-    from rockset.model.query_field_type import QueryFieldType
-    from rockset.model.query_response_stats import QueryResponseStats
-
-    globals()["PaginationInfo"] = PaginationInfo
-    globals()["QueryError"] = QueryError
-    globals()["QueryFieldType"] = QueryFieldType
-    globals()["QueryResponseStats"] = QueryResponseStats
+    from rockset_v2.model.pagination_info import PaginationInfo
+    from rockset_v2.model.query_error import QueryError
+    from rockset_v2.model.query_field_type import QueryFieldType
+    from rockset_v2.model.query_response_stats import QueryResponseStats
+    globals()['PaginationInfo'] = PaginationInfo
+    globals()['QueryError'] = QueryError
+    globals()['QueryFieldType'] = QueryFieldType
+    globals()['QueryResponseStats'] = QueryResponseStats
 
 
 class QueryResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -62,37 +59,29 @@
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
+    
+    allowed_values = {
+    }
 
-    allowed_values = {}
-
-    validations = {}
+    validations = {
+    }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
         lazy_import()
-        return (
-            bool,
-            date,
-            datetime,
-            dict,
-            float,
-            int,
-            list,
-            str,
-            none_type,
-        )  # noqa: E501
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -100,72 +89,61 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            "collections": ([str],),  # noqa: E501
-            "column_fields": ([QueryFieldType],),  # noqa: E501
-            "last_offset": (str,),  # noqa: E501
-            "pagination": (PaginationInfo,),  # noqa: E501
-            "query_errors": ([QueryError],),  # noqa: E501
-            "query_id": (str,),  # noqa: E501
-            "query_lambda_path": (str,),  # noqa: E501
-            "results": (
-                [{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],
-            ),  # noqa: E501
-            "results_total_doc_count": (int,),  # noqa: E501
-            "stats": (QueryResponseStats,),  # noqa: E501
-            "warnings": ([str],),  # noqa: E501
+            'collections': ([str], none_type),  # noqa: E501
+            'column_fields': ([QueryFieldType], none_type),  # noqa: E501
+            'last_offset': (str, none_type),  # noqa: E501
+            'pagination': (PaginationInfo, none_type),  # noqa: E501
+            'query_errors': ([QueryError], none_type),  # noqa: E501
+            'query_id': (str, none_type),  # noqa: E501
+            'query_lambda_path': (str, none_type),  # noqa: E501
+            'results': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}], none_type),  # noqa: E501
+            'results_total_doc_count': (int, none_type),  # noqa: E501
+            'stats': (QueryResponseStats, none_type),  # noqa: E501
+            'warnings': ([str], none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
+
     attribute_map = {
-        "collections": "collections",  # noqa: E501
-        "column_fields": "column_fields",  # noqa: E501
-        "last_offset": "last_offset",  # noqa: E501
-        "pagination": "pagination",  # noqa: E501
-        "query_errors": "query_errors",  # noqa: E501
-        "query_id": "query_id",  # noqa: E501
-        "query_lambda_path": "query_lambda_path",  # noqa: E501
-        "results": "results",  # noqa: E501
-        "results_total_doc_count": "results_total_doc_count",  # noqa: E501
-        "stats": "stats",  # noqa: E501
-        "warnings": "warnings",  # noqa: E501
+        'collections': 'collections',  # noqa: E501
+        'column_fields': 'column_fields',  # noqa: E501
+        'last_offset': 'last_offset',  # noqa: E501
+        'pagination': 'pagination',  # noqa: E501
+        'query_errors': 'query_errors',  # noqa: E501
+        'query_id': 'query_id',  # noqa: E501
+        'query_lambda_path': 'query_lambda_path',  # noqa: E501
+        'results': 'results',  # noqa: E501
+        'results_total_doc_count': 'results_total_doc_count',  # noqa: E501
+        'stats': 'stats',  # noqa: E501
+        'warnings': 'warnings',  # noqa: E501
     }
 
-    read_only_vars = {}
+    read_only_vars = {
+    }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """QueryResponse - a model defined in OpenAPI
 
         Keyword Args:
-            collections ([str]): List of collections referenced in the query.. [optional]  # noqa: E501
-            column_fields ([QueryFieldType]): Meta information about each column in the result set. Not populated in `SELECT *` queries.. [optional]  # noqa: E501
-            last_offset (str): If this was a write query, this is the log offset the query was written to. [optional]  # noqa: E501
-            pagination (PaginationInfo): [optional]  # noqa: E501
-            query_errors ([QueryError]): Errors encountered while executing the query.. [optional]  # noqa: E501
-            query_id (str): Unique ID for this query.. [optional]  # noqa: E501
-            query_lambda_path (str): The full path of the executed query lambda. Includes version information.. [optional]  # noqa: E501
-            results ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): Results from the query.. [optional]  # noqa: E501
-            results_total_doc_count (int): Number of results generated by the query. [optional]  # noqa: E501
-            stats (QueryResponseStats): [optional]  # noqa: E501
-            warnings ([str]): Warnings generated by the query. Only populated if `generate_warnings` is specified in the query request.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
-                                Defaults to False for performance
+                                Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
             _spec_property_naming (bool): True if the variable names in the input data
                                 are serialized names, as specified in the OpenAPI document.
                                 False if the variable names in the input data
                                 are pythonic names, e.g. snake case (default)
@@ -184,28 +162,38 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            collections ([str]): List of collections referenced in the query.. [optional]  # noqa: E501
+            column_fields ([QueryFieldType]): Meta information about each column in the result set. Not populated in `SELECT *` queries.. [optional]  # noqa: E501
+            last_offset (str): If this was a write query, this is the log offset the query was written to.. [optional]  # noqa: E501
+            pagination (PaginationInfo): [optional]  # noqa: E501
+            query_errors ([QueryError]): Errors encountered while executing the query.. [optional]  # noqa: E501
+            query_id (str): Unique ID for this query.. [optional]  # noqa: E501
+            query_lambda_path (str): The full path of the executed query lambda. Includes version information.. [optional]  # noqa: E501
+            results ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): Results from the query.. [optional]  # noqa: E501
+            results_total_doc_count (int): Number of results generated by the query.. [optional]  # noqa: E501
+            stats (QueryResponseStats): [optional]  # noqa: E501
+            warnings ([str]): Warnings generated by the query. Only populated if `generate_warnings` is specified in the query request.. [optional]  # noqa: E501
         """
 
-        _check_type = kwargs.pop("_check_type", False)
-        _spec_property_naming = kwargs.pop("_spec_property_naming", False)
-        _path_to_item = kwargs.pop("_path_to_item", ())
-        _configuration = kwargs.pop("_configuration", None)
-        _visited_composed_classes = kwargs.pop("_visited_composed_classes", ())
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
 
         if args:
             raise ApiTypeError(
-                "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments."
-                % (
+                "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
                     self.__class__.__name__,
                 ),
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
@@ -213,48 +201,52 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         for var_name, var_value in kwargs.items():
-            if (
-                var_name not in self.attribute_map
-                and self._configuration is not None
-                and self._configuration.discard_unknown_keys
-                and self.additional_properties_type is None
-            ):
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
-            if var_name == "results":
-                setattr(self, "results", [Document(doc) for doc in var_value])
-                continue
             setattr(self, var_name, var_value)
         return self
 
-    required_properties = set(
-        [
-            "_data_store",
-            "_check_type",
-            "_spec_property_naming",
-            "_path_to_item",
-            "_configuration",
-            "_visited_composed_classes",
-        ]
-    )
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, **kwargs):  # noqa: E501
         """QueryResponse - a model defined in OpenAPI
 
         Keyword Args:
+            collections ([str]): List of collections referenced in the query.. [optional]  # noqa: E501
+            column_fields ([QueryFieldType]): Meta information about each column in the result set. Not populated in `SELECT *` queries.. [optional]  # noqa: E501
+            last_offset (str): If this was a write query, this is the log offset the query was written to.. [optional]  # noqa: E501
+            pagination (PaginationInfo): [optional]  # noqa: E501
+            query_errors ([QueryError]): Errors encountered while executing the query.. [optional]  # noqa: E501
+            query_id (str): Unique ID for this query.. [optional]  # noqa: E501
+            query_lambda_path (str): The full path of the executed query lambda. Includes version information.. [optional]  # noqa: E501
+            results ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): Results from the query.. [optional]  # noqa: E501
+            results_total_doc_count (int): Number of results generated by the query.. [optional]  # noqa: E501
+            stats (QueryResponseStats): [optional]  # noqa: E501
+            warnings ([str]): Warnings generated by the query. Only populated if `generate_warnings` is specified in the query request.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
-                                Defaults to False for performance
+                                Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
             _spec_property_naming (bool): True if the variable names in the input data
                                 are serialized names, as specified in the OpenAPI document.
                                 False if the variable names in the input data
                                 are pythonic names, e.g. snake case (default)
@@ -273,37 +265,26 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            collections ([str]): List of collections referenced in the query.. [optional]  # noqa: E501
-            column_fields ([QueryFieldType]): Meta information about each column in the result set. Not populated in `SELECT *` queries.. [optional]  # noqa: E501
-            last_offset (str): If this was a write query, this is the log offset the query was written to. [optional]  # noqa: E501
-            pagination (PaginationInfo): [optional]  # noqa: E501
-            query_errors ([QueryError]): Errors encountered while executing the query.. [optional]  # noqa: E501
-            query_id (str): Unique ID for this query.. [optional]  # noqa: E501
-            query_lambda_path (str): The full path of the executed query lambda. Includes version information.. [optional]  # noqa: E501
-            results ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): Results from the query.. [optional]  # noqa: E501
-            results_total_doc_count (int): Number of results generated by the query. [optional]  # noqa: E501
-            stats (QueryResponseStats): [optional]  # noqa: E501
-            warnings ([str]): Warnings generated by the query. Only populated if `generate_warnings` is specified in the query request.. [optional]  # noqa: E501
         """
-
-        _check_type = kwargs.pop("_check_type", False)
-        _spec_property_naming = kwargs.pop("_spec_property_naming", False)
-        _path_to_item = kwargs.pop("_path_to_item", ())
-        _configuration = kwargs.pop("_configuration", None)
-        _visited_composed_classes = kwargs.pop("_visited_composed_classes", ())
+        
+        args = []
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             raise ApiTypeError(
-                "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments."
-                % (
+                "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
                     self.__class__.__name__,
                 ),
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
@@ -311,24 +292,18 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         for var_name, var_value in kwargs.items():
-            if (
-                var_name not in self.attribute_map
-                and self._configuration is not None
-                and self._configuration.discard_unknown_keys
-                and self.additional_properties_type is None
-            ):
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
-            if var_name == "results":
-                setattr(self, "results", [Document(doc) for doc in var_value])
-                continue
             setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(
-                    f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                    f"class with read only attributes."
-                )
+            # todo: remove these comments - this stops the user from setting read only vars but we need this now to address a bug
+            # if var_name in self.read_only_vars:
+            #     raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+            #                          f"class with read only attributes.")
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/query_response_stats.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_response_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class QueryResponseStats(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/resume_virtual_instance_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_virtual_instance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.virtual_instance import VirtualInstance
+    from rockset_v2.model.virtual_instance import VirtualInstance
     globals()['VirtualInstance'] = VirtualInstance
 
 
-class ResumeVirtualInstanceResponse(ModelNormal):
+class UpdateVirtualInstanceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -103,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResumeVirtualInstanceResponse - a model defined in OpenAPI
+        """UpdateVirtualInstanceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -185,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """ResumeVirtualInstanceResponse - a model defined in OpenAPI
+        """UpdateVirtualInstanceResponse - a model defined in OpenAPI
 
         Keyword Args:
             data (VirtualInstance): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/role.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.privilege import Privilege
+    from rockset_v2.model.privilege import Privilege
     globals()['Privilege'] = Privilege
 
 
 class Role(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/role_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_api_key_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,38 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rockset.model.role import Role
-    globals()['Role'] = Role
 
-
-class RoleResponse(ModelNormal):
+class UpdateApiKeyRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,63 +51,65 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('state',): {
+            'ACTIVE': "ACTIVE",
+            'SUSPENDED': "SUSPENDED",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': (Role, none_type),  # noqa: E501
+            'state': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'state': 'state',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RoleResponse - a model defined in OpenAPI
+        """UpdateApiKeyRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (Role): [optional]  # noqa: E501
+            state (str): State that the api key should be set to.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,18 +183,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """RoleResponse - a model defined in OpenAPI
+        """UpdateApiKeyRequest - a model defined in OpenAPI
 
         Keyword Args:
-            data (Role): [optional]  # noqa: E501
+            state (str): State that the api key should be set to.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/s3_collection_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_collection_creation_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,46 +7,44 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.event_time_info import EventTimeInfo
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
-    from rockset.model.s3_source_wrapper import S3SourceWrapper
+    from rockset_v2.model.event_time_info import EventTimeInfo
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_partition import FieldPartition
+    from rockset_v2.model.snowflake_source_wrapper import SnowflakeSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['S3SourceWrapper'] = S3SourceWrapper
+    globals()['SnowflakeSourceWrapper'] = SnowflakeSourceWrapper
 
 
-class S3CollectionCreationRequest(ModelNormal):
+class SnowflakeCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([S3SourceWrapper], none_type),  # noqa: E501
+            'sources': ([SnowflakeSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """S3CollectionCreationRequest - a model defined in OpenAPI
+        """SnowflakeCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([S3SourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([SnowflakeSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """S3CollectionCreationRequest - a model defined in OpenAPI
+        """SnowflakeCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([S3SourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([SnowflakeSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/s3_integration.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/s3_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.aws_access_key import AwsAccessKey
-    from rockset.model.aws_role import AwsRole
+    from rockset_v2.model.aws_access_key import AwsAccessKey
+    from rockset_v2.model.aws_role import AwsRole
     globals()['AwsAccessKey'] = AwsAccessKey
     globals()['AwsRole'] = AwsRole
 
 
 class S3Integration(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/s3_integration_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/s3_integration_creation_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.s3_integration import S3Integration
+    from rockset_v2.model.s3_integration import S3Integration
     globals()['S3Integration'] = S3Integration
 
 
 class S3IntegrationCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/s3_source_wrapper.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/s3_source_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status import Status
+    from rockset_v2.model.format_params import FormatParams
+    from rockset_v2.model.status import Status
     globals()['FormatParams'] = FormatParams
     globals()['Status'] = Status
 
 
 class S3SourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/schema_registry_config.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/schema_registry_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class SchemaRegistryConfig(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/segment_integration.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/segment_integration.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/segment_integration_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/segment_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/snowflake_collection_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/gcs_collection_creation_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,46 +7,44 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.event_time_info import EventTimeInfo
-    from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
-    from rockset.model.field_partition import FieldPartition
-    from rockset.model.snowflake_source_wrapper import SnowflakeSourceWrapper
+    from rockset_v2.model.event_time_info import EventTimeInfo
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    from rockset_v2.model.field_partition import FieldPartition
+    from rockset_v2.model.gcs_source_wrapper import GcsSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['SnowflakeSourceWrapper'] = SnowflakeSourceWrapper
+    globals()['GcsSourceWrapper'] = GcsSourceWrapper
 
 
-class SnowflakeCollectionCreationRequest(ModelNormal):
+class GcsCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([SnowflakeSourceWrapper], none_type),  # noqa: E501
+            'sources': ([GcsSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """SnowflakeCollectionCreationRequest - a model defined in OpenAPI
+        """GcsCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([SnowflakeSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([GcsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """SnowflakeCollectionCreationRequest - a model defined in OpenAPI
+        """GcsCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([SnowflakeSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([GcsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/snowflake_integration.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.aws_access_key import AwsAccessKey
-    from rockset.model.aws_role import AwsRole
+    from rockset_v2.model.aws_access_key import AwsAccessKey
+    from rockset_v2.model.aws_role import AwsRole
     globals()['AwsAccessKey'] = AwsAccessKey
     globals()['AwsRole'] = AwsRole
 
 
 class SnowflakeIntegration(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/snowflake_integration_creation_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_integration_creation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.snowflake_integration import SnowflakeIntegration
+    from rockset_v2.model.snowflake_integration import SnowflakeIntegration
     globals()['SnowflakeIntegration'] = SnowflakeIntegration
 
 
 class SnowflakeIntegrationCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/snowflake_source_wrapper.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/snowflake_source_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status_snowflake import StatusSnowflake
+    from rockset_v2.model.format_params import FormatParams
+    from rockset_v2.model.status_snowflake import StatusSnowflake
     globals()['FormatParams'] = FormatParams
     globals()['StatusSnowflake'] = StatusSnowflake
 
 
 class SnowflakeSourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/source.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source_azure_service_bus.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,40 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status import Status
-    globals()['FormatParams'] = FormatParams
-    globals()['Status'] = Status
+    from rockset_v2.model.status_azure_service_bus import StatusAzureServiceBus
+    globals()['StatusAzureServiceBus'] = StatusAzureServiceBus
 
 
-class Source(ModelNormal):
+class SourceAzureServiceBus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,40 +83,40 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'format_params': (FormatParams, none_type),  # noqa: E501
-            'integration_name': (str, none_type),  # noqa: E501
             'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
+            'subscription': (str, none_type),  # noqa: E501
+            'topic': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'format_params': 'format_params',  # noqa: E501
-        'integration_name': 'integration_name',  # noqa: E501
         'status': 'status',  # noqa: E501
+        'subscription': 'subscription',  # noqa: E501
+        'topic': 'topic',  # noqa: E501
     }
 
     read_only_vars = {
         'status',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Source - a model defined in OpenAPI
+        """SourceAzureServiceBus - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,17 +141,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            format_params (FormatParams): [optional]  # noqa: E501
-            integration_name (str): Name of integration to use.. [optional]  # noqa: E501
             status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            subscription (str): The subscription to read from the topic.. [optional]  # noqa: E501
+            topic (str): Name of the topic which rockset should ingest from.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -194,19 +192,19 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """Source - a model defined in OpenAPI
+        """SourceAzureServiceBus - a model defined in OpenAPI
 
         Keyword Args:
-            format_params (FormatParams): [optional]  # noqa: E501
-            integration_name (str): Name of integration to use.. [optional]  # noqa: E501
+            subscription (str): The subscription to read from the topic.. [optional]  # noqa: E501
+            topic (str): Name of the topic which rockset should ingest from.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/source_azure_blob_storage.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source_azure_blob_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class SourceAzureBlobStorage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/source_azure_event_hubs.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source_azure_event_hubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.status_azure_event_hubs import StatusAzureEventHubs
+    from rockset_v2.model.status_azure_event_hubs import StatusAzureEventHubs
     globals()['StatusAzureEventHubs'] = StatusAzureEventHubs
 
 
 class SourceAzureEventHubs(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/source_azure_service_bus.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_event_hubs_partition.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,38 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rockset.model.status_azure_service_bus import StatusAzureServiceBus
-    globals()['StatusAzureServiceBus'] = StatusAzureServiceBus
 
-
-class SourceAzureServiceBus(ModelNormal):
+class StatusAzureEventHubsPartition(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,57 +62,54 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
-            'subscription': (str, none_type),  # noqa: E501
-            'topic': (str, none_type),  # noqa: E501
+            'offset_lag': (int, none_type),  # noqa: E501
+            'partition_number': (int, none_type),  # noqa: E501
+            'partition_offset': (int, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'status': 'status',  # noqa: E501
-        'subscription': 'subscription',  # noqa: E501
-        'topic': 'topic',  # noqa: E501
+        'offset_lag': 'offset_lag',  # noqa: E501
+        'partition_number': 'partition_number',  # noqa: E501
+        'partition_offset': 'partition_offset',  # noqa: E501
     }
 
     read_only_vars = {
-        'status',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SourceAzureServiceBus - a model defined in OpenAPI
+        """StatusAzureEventHubsPartition - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,17 +134,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            subscription (str): The subscription to read from the topic.. [optional]  # noqa: E501
-            topic (str): Name of the topic which rockset should ingest from.. [optional]  # noqa: E501
+            offset_lag (int): Per partition lag for offset.. [optional]  # noqa: E501
+            partition_number (int): The number of this partition.. [optional]  # noqa: E501
+            partition_offset (int): Latest offset of partition.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,19 +185,20 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """SourceAzureServiceBus - a model defined in OpenAPI
+        """StatusAzureEventHubsPartition - a model defined in OpenAPI
 
         Keyword Args:
-            subscription (str): The subscription to read from the topic.. [optional]  # noqa: E501
-            topic (str): Name of the topic which rockset should ingest from.. [optional]  # noqa: E501
+            offset_lag (int): Per partition lag for offset.. [optional]  # noqa: E501
+            partition_number (int): The number of this partition.. [optional]  # noqa: E501
+            partition_offset (int): Latest offset of partition.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/source_dynamo_db.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source_dynamo_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.status_dynamo_db import StatusDynamoDb
-    from rockset.model.status_dynamo_db_v2 import StatusDynamoDbV2
+    from rockset_v2.model.status_dynamo_db import StatusDynamoDb
+    from rockset_v2.model.status_dynamo_db_v2 import StatusDynamoDbV2
     globals()['StatusDynamoDb'] = StatusDynamoDb
     globals()['StatusDynamoDbV2'] = StatusDynamoDbV2
 
 
 class SourceDynamoDb(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/source_file_upload.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source_file_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class SourceFileUpload(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/source_gcs.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source_gcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class SourceGcs(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/source_kafka.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source_kafka.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.status_kafka import StatusKafka
+    from rockset_v2.model.status_kafka import StatusKafka
     globals()['StatusKafka'] = StatusKafka
 
 
 class SourceKafka(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/source_kinesis.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source_kinesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class SourceKinesis(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/source_mongo_db.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source_mongo_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.status_mongo_db import StatusMongoDb
+    from rockset_v2.model.status_mongo_db import StatusMongoDb
     globals()['StatusMongoDb'] = StatusMongoDb
 
 
 class SourceMongoDb(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -85,25 +85,27 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'collection_name': (str,),  # noqa: E501
             'database_name': (str,),  # noqa: E501
+            'retrieve_full_document': (bool, none_type),  # noqa: E501
             'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'collection_name': 'collection_name',  # noqa: E501
         'database_name': 'database_name',  # noqa: E501
+        'retrieve_full_document': 'retrieve_full_document',  # noqa: E501
         'status': 'status',  # noqa: E501
     }
 
     read_only_vars = {
         'status',  # noqa: E501
     }
 
@@ -145,14 +147,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            retrieve_full_document (bool): Whether to get the full document from the MongoDB change stream to enable multi-field expression transformations. Selecting this option will increase load on your upstream MongoDB database.. [optional]  # noqa: E501
             status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -201,14 +204,15 @@
     @convert_js_args_to_python_args
     def __init__(self, *, collection_name, database_name, **kwargs):  # noqa: E501
         """SourceMongoDb - a model defined in OpenAPI
 
         Keyword Args:
             collection_name (str): MongoDB collection name.
             database_name (str): MongoDB database name containing this collection.
+            retrieve_full_document (bool): Whether to get the full document from the MongoDB change stream to enable multi-field expression transformations. Selecting this option will increase load on your upstream MongoDB database.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/source_s3.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source_s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class SourceS3(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/source_snowflake.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source_snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.status_snowflake import StatusSnowflake
+    from rockset_v2.model.status_snowflake import StatusSnowflake
     globals()['StatusSnowflake'] = StatusSnowflake
 
 
 class SourceSnowflake(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/sql_expression.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/sql_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class SqlExpression(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/stats.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class Stats(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/status.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class Status(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/status_azure_event_hubs.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_event_hubs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.status_azure_event_hubs_partition import StatusAzureEventHubsPartition
+    from rockset_v2.model.status_azure_event_hubs_partition import StatusAzureEventHubsPartition
     globals()['StatusAzureEventHubsPartition'] = StatusAzureEventHubsPartition
 
 
 class StatusAzureEventHubs(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/status_azure_event_hubs_partition.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/status_kafka_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
-class StatusAzureEventHubsPartition(ModelNormal):
+class StatusKafkaPartition(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -101,15 +101,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """StatusAzureEventHubsPartition - a model defined in OpenAPI
+        """StatusKafkaPartition - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -185,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """StatusAzureEventHubsPartition - a model defined in OpenAPI
+        """StatusKafkaPartition - a model defined in OpenAPI
 
         Keyword Args:
             offset_lag (int): Per partition lag for offset.. [optional]  # noqa: E501
             partition_number (int): The number of this partition.. [optional]  # noqa: E501
             partition_offset (int): Latest offset of partition.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/status_azure_service_bus.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_service_bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.status_azure_service_bus_session import StatusAzureServiceBusSession
+    from rockset_v2.model.status_azure_service_bus_session import StatusAzureServiceBusSession
     globals()['StatusAzureServiceBusSession'] = StatusAzureServiceBusSession
 
 
 class StatusAzureServiceBus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/status_azure_service_bus_session.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/status_azure_service_bus_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class StatusAzureServiceBusSession(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/status_dynamo_db.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/status_dynamo_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class StatusDynamoDb(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/status_dynamo_db_v2.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/status_dynamo_db_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class StatusDynamoDbV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/status_kafka.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/status_kafka.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.status_kafka_partition import StatusKafkaPartition
+    from rockset_v2.model.status_kafka_partition import StatusKafkaPartition
     globals()['StatusKafkaPartition'] = StatusKafkaPartition
 
 
 class StatusKafka(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/status_kafka_partition.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_view_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
-class StatusKafkaPartition(ModelNormal):
+class UpdateViewRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,39 +77,40 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'offset_lag': (int, none_type),  # noqa: E501
-            'partition_number': (int, none_type),  # noqa: E501
-            'partition_offset': (int, none_type),  # noqa: E501
+            'query': (str,),  # noqa: E501
+            'description': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'offset_lag': 'offset_lag',  # noqa: E501
-        'partition_number': 'partition_number',  # noqa: E501
-        'partition_offset': 'partition_offset',  # noqa: E501
+        'query': 'query',  # noqa: E501
+        'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """StatusKafkaPartition - a model defined in OpenAPI
+    def _from_openapi_data(cls, query, *args, **kwargs):  # noqa: E501
+        """UpdateViewRequest - a model defined in OpenAPI
+
+        Args:
+            query (str): SQL for this view.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,17 +135,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            offset_lag (int): Per partition lag for offset.. [optional]  # noqa: E501
-            partition_number (int): The number of this partition.. [optional]  # noqa: E501
-            partition_offset (int): Latest offset of partition.. [optional]  # noqa: E501
+            description (str): Optional description.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -164,14 +163,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.query = query
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -184,21 +184,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, **kwargs):  # noqa: E501
-        """StatusKafkaPartition - a model defined in OpenAPI
+    def __init__(self, *, query, **kwargs):  # noqa: E501
+        """UpdateViewRequest - a model defined in OpenAPI
 
         Keyword Args:
-            offset_lag (int): Per partition lag for offset.. [optional]  # noqa: E501
-            partition_number (int): The number of this partition.. [optional]  # noqa: E501
-            partition_offset (int): Latest offset of partition.. [optional]  # noqa: E501
+            query (str): SQL for this view.
+            description (str): Optional description.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -247,14 +246,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.query = query
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/status_mongo_db.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/status_mongo_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class StatusMongoDb(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/status_snowflake.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/status_snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class StatusSnowflake(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/suspend_virtual_instance_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_virtual_instance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.virtual_instance import VirtualInstance
+    from rockset_v2.model.virtual_instance import VirtualInstance
     globals()['VirtualInstance'] = VirtualInstance
 
 
-class SuspendVirtualInstanceResponse(ModelNormal):
+class CreateVirtualInstanceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -103,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SuspendVirtualInstanceResponse - a model defined in OpenAPI
+        """CreateVirtualInstanceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -185,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """SuspendVirtualInstanceResponse - a model defined in OpenAPI
+        """CreateVirtualInstanceResponse - a model defined in OpenAPI
 
         Keyword Args:
             data (VirtualInstance): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/unsubscribe_preference.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/unsubscribe_preference.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class UnsubscribePreference(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_alias_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_view_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,34 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rockset_v2.model.view import View
+    globals()['View'] = View
 
-class UpdateAliasRequest(ModelNormal):
+
+class UpdateViewResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,55 +66,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'collections': ([str],),  # noqa: E501
-            'description': (str, none_type),  # noqa: E501
+            'data': (View, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'collections': 'collections',  # noqa: E501
-        'description': 'description',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, collections, *args, **kwargs):  # noqa: E501
-        """UpdateAliasRequest - a model defined in OpenAPI
-
-        Args:
-            collections ([str]): List of fully qualified collection names referenced by alias.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """UpdateViewResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            description (str): Optional description.. [optional]  # noqa: E501
+            data (View): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -163,15 +164,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.collections = collections
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -184,20 +184,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *, collections, **kwargs):  # noqa: E501
-        """UpdateAliasRequest - a model defined in OpenAPI
+    def __init__(self, **kwargs):  # noqa: E501
+        """UpdateViewResponse - a model defined in OpenAPI
 
         Keyword Args:
-            collections ([str]): List of fully qualified collection names referenced by alias.
-            description (str): Optional description.. [optional]  # noqa: E501
+            data (View): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -246,15 +245,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.collections = collections
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_api_key_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_integration_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rockset.model.kafka_integration import KafkaIntegration
+    globals()['KafkaIntegration'] = KafkaIntegration
 
-class UpdateApiKeyRequest(ModelNormal):
+
+class UpdateIntegrationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,65 +55,63 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
-        ('state',): {
-            'ACTIVE': "ACTIVE",
-            'SUSPENDED': "SUSPENDED",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'state': (str, none_type),  # noqa: E501
+            'kafka': (KafkaIntegration, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'state': 'state',  # noqa: E501
+        'kafka': 'kafka',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateApiKeyRequest - a model defined in OpenAPI
+        """UpdateIntegrationRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            state (str): State that the api key should be set to.. [optional]  # noqa: E501
+            kafka (KafkaIntegration): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,18 +185,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """UpdateApiKeyRequest - a model defined in OpenAPI
+        """UpdateIntegrationRequest - a model defined in OpenAPI
 
         Keyword Args:
-            state (str): State that the api key should be set to.. [optional]  # noqa: E501
+            kafka (KafkaIntegration): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_api_key_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_api_key_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.api_key import ApiKey
+    from rockset_v2.model.api_key import ApiKey
     globals()['ApiKey'] = ApiKey
 
 
 class UpdateApiKeyResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_integration_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/delete_integration_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.kafka_integration import KafkaIntegration
-    globals()['KafkaIntegration'] = KafkaIntegration
+    from rockset_v2.model.integration import Integration
+    globals()['Integration'] = Integration
 
 
-class UpdateIntegrationRequest(ModelNormal):
+class DeleteIntegrationResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,35 +83,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'kafka': (KafkaIntegration, none_type),  # noqa: E501
+            'data': (Integration, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'kafka': 'kafka',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateIntegrationRequest - a model defined in OpenAPI
+        """DeleteIntegrationResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            kafka (KafkaIntegration): [optional]  # noqa: E501
+            data (Integration): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,18 +185,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """UpdateIntegrationRequest - a model defined in OpenAPI
+        """DeleteIntegrationResponse - a model defined in OpenAPI
 
         Keyword Args:
-            kafka (KafkaIntegration): [optional]  # noqa: E501
+            data (Integration): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_integration_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/get_workspace_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.integration import Integration
-    globals()['Integration'] = Integration
+    from rockset_v2.model.workspace import Workspace
+    globals()['Workspace'] = Workspace
 
 
-class UpdateIntegrationResponse(ModelNormal):
+class GetWorkspaceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,15 +83,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (Integration, none_type),  # noqa: E501
+            'data': (Workspace, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -103,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateIntegrationResponse - a model defined in OpenAPI
+        """GetWorkspaceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (Integration): [optional]  # noqa: E501
+            data (Workspace): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,18 +185,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """UpdateIntegrationResponse - a model defined in OpenAPI
+        """GetWorkspaceResponse - a model defined in OpenAPI
 
         Keyword Args:
-            data (Integration): [optional]  # noqa: E501
+            data (Workspace): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_query_lambda_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/source_system.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,38 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rockset.model.query_lambda_sql import QueryLambdaSql
-    globals()['QueryLambdaSql'] = QueryLambdaSql
 
-
-class UpdateQueryLambdaRequest(ModelNormal):
+class SourceSystem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,67 +51,64 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('type',): {
+            'QUERY_LOGS': "QUERY_LOGS",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'description': (str, none_type),  # noqa: E501
-            'is_public': (bool, none_type),  # noqa: E501
-            'sql': (QueryLambdaSql, none_type),  # noqa: E501
+            'type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'description': 'description',  # noqa: E501
-        'is_public': 'is_public',  # noqa: E501
-        'sql': 'sql',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateQueryLambdaRequest - a model defined in OpenAPI
+        """SourceSystem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +133,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            description (str): Optional description.. [optional]  # noqa: E501
-            is_public (bool): [optional]  # noqa: E501
-            sql (QueryLambdaSql): [optional]  # noqa: E501
+            type (str): The type of this system source.. [optional] if omitted the server will use the default value of "QUERY_LOGS"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,20 +182,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """UpdateQueryLambdaRequest - a model defined in OpenAPI
+        """SourceSystem - a model defined in OpenAPI
 
         Keyword Args:
-            description (str): Optional description.. [optional]  # noqa: E501
-            is_public (bool): [optional]  # noqa: E501
-            sql (QueryLambdaSql): [optional]  # noqa: E501
+            type (str): The type of this system source.. [optional] if omitted the server will use the default value of "QUERY_LOGS"  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_role_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_role_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.privilege import Privilege
+    from rockset_v2.model.privilege import Privilege
     globals()['Privilege'] = Privilege
 
 
 class UpdateRoleRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_unsubscribe_preferences_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_unsubscribe_preferences_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.unsubscribe_preference import UnsubscribePreference
+    from rockset_v2.model.unsubscribe_preference import UnsubscribePreference
     globals()['UnsubscribePreference'] = UnsubscribePreference
 
 
-class UpdateUnsubscribePreferencesRequest(ModelNormal):
+class UpdateUnsubscribePreferencesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -103,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateUnsubscribePreferencesRequest - a model defined in OpenAPI
+        """UpdateUnsubscribePreferencesResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -185,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """UpdateUnsubscribePreferencesRequest - a model defined in OpenAPI
+        """UpdateUnsubscribePreferencesResponse - a model defined in OpenAPI
 
         Keyword Args:
             data ([UnsubscribePreference]): List of notification preferences.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_unsubscribe_preferences_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_unsubscribe_preferences_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.unsubscribe_preference import UnsubscribePreference
+    from rockset_v2.model.unsubscribe_preference import UnsubscribePreference
     globals()['UnsubscribePreference'] = UnsubscribePreference
 
 
-class UpdateUnsubscribePreferencesResponse(ModelNormal):
+class UpdateUnsubscribePreferencesRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -103,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateUnsubscribePreferencesResponse - a model defined in OpenAPI
+        """UpdateUnsubscribePreferencesRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -185,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """UpdateUnsubscribePreferencesResponse - a model defined in OpenAPI
+        """UpdateUnsubscribePreferencesRequest - a model defined in OpenAPI
 
         Keyword Args:
             data ([UnsubscribePreference]): List of notification preferences.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_user_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_user_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class UpdateUserRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_view_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/get_virtual_instance_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,34 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rockset_v2.model.virtual_instance import VirtualInstance
+    globals()['VirtualInstance'] = VirtualInstance
 
-class UpdateViewRequest(ModelNormal):
+
+class GetVirtualInstanceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,55 +66,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'query': (str,),  # noqa: E501
-            'description': (str, none_type),  # noqa: E501
+            'data': (VirtualInstance, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'query': 'query',  # noqa: E501
-        'description': 'description',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, query, *args, **kwargs):  # noqa: E501
-        """UpdateViewRequest - a model defined in OpenAPI
-
-        Args:
-            query (str): SQL for this view.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """GetVirtualInstanceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            description (str): Optional description.. [optional]  # noqa: E501
+            data (VirtualInstance): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -163,15 +164,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.query = query
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -184,20 +184,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *, query, **kwargs):  # noqa: E501
-        """UpdateViewRequest - a model defined in OpenAPI
+    def __init__(self, **kwargs):  # noqa: E501
+        """GetVirtualInstanceResponse - a model defined in OpenAPI
 
         Keyword Args:
-            query (str): SQL for this view.
-            description (str): Optional description.. [optional]  # noqa: E501
+            data (VirtualInstance): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -246,15 +245,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.query = query
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_view_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/virtual_instance_stats.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,38 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rockset.model.view import View
-    globals()['View'] = View
 
-
-class UpdateViewResponse(ModelNormal):
+class VirtualInstanceStats(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,52 +62,50 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': (View, none_type),  # noqa: E501
+            'last_queried_ms': (int, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'last_queried_ms': 'last_queried_ms',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateViewResponse - a model defined in OpenAPI
+        """VirtualInstanceStats - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (View): [optional]  # noqa: E501
+            last_queried_ms (int): Milliseconds since Unix epoch Jan 1, 1970.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,18 +179,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """UpdateViewResponse - a model defined in OpenAPI
+        """VirtualInstanceStats - a model defined in OpenAPI
 
         Keyword Args:
-            data (View): [optional]  # noqa: E501
+            last_queried_ms (int): Milliseconds since Unix epoch Jan 1, 1970.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_virtual_instance_request.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/create_virtual_instance_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
-class UpdateVirtualInstanceRequest(ModelNormal):
+class CreateVirtualInstanceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,15 +51,15 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
-        ('new_size',): {
+        ('type',): {
             'FREE': "FREE",
             'NANO': "NANO",
             'SHARED': "SHARED",
             'MILLI': "MILLI",
             'SMALL': "SMALL",
             'MEDIUM': "MEDIUM",
             'LARGE': "LARGE",
@@ -91,45 +91,48 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'auto_suspend_enabled': (bool, none_type),  # noqa: E501
+            'name': (str,),  # noqa: E501
             'auto_suspend_seconds': (int, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
-            'monitoring_enabled': (bool, none_type),  # noqa: E501
-            'name': (str, none_type),  # noqa: E501
-            'new_size': (str, none_type),  # noqa: E501
+            'enable_remount_on_resume': (bool, none_type),  # noqa: E501
+            'mount_refresh_interval_seconds': (int, none_type),  # noqa: E501
+            'type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'auto_suspend_enabled': 'auto_suspend_enabled',  # noqa: E501
+        'name': 'name',  # noqa: E501
         'auto_suspend_seconds': 'auto_suspend_seconds',  # noqa: E501
         'description': 'description',  # noqa: E501
-        'monitoring_enabled': 'monitoring_enabled',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'new_size': 'new_size',  # noqa: E501
+        'enable_remount_on_resume': 'enable_remount_on_resume',  # noqa: E501
+        'mount_refresh_interval_seconds': 'mount_refresh_interval_seconds',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateVirtualInstanceRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """CreateVirtualInstanceRequest - a model defined in OpenAPI
+
+        Args:
+            name (str): Unique identifier for virtual instance, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -154,20 +157,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            auto_suspend_enabled (bool): Whether auto-suspend should be enabled for this Virtual Instance.. [optional]  # noqa: E501
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
-            description (str): New virtual instance description.. [optional]  # noqa: E501
-            monitoring_enabled (bool): [optional]  # noqa: E501
-            name (str): New virtual instance name.. [optional]  # noqa: E501
-            new_size (str): Requested virtual instance size.. [optional]  # noqa: E501
+            description (str): Description of requested virtual instance.. [optional]  # noqa: E501
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
+            mount_refresh_interval_seconds (int): Number of seconds between data refreshes for mounts on this Virtual Instance. A value of 0 means continuous refresh and a value of null means never refresh.. [optional]  # noqa: E501
+            type (str): Requested virtual instance type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,14 +189,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -207,24 +210,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, **kwargs):  # noqa: E501
-        """UpdateVirtualInstanceRequest - a model defined in OpenAPI
+    def __init__(self, *, name, **kwargs):  # noqa: E501
+        """CreateVirtualInstanceRequest - a model defined in OpenAPI
 
         Keyword Args:
-            auto_suspend_enabled (bool): Whether auto-suspend should be enabled for this Virtual Instance.. [optional]  # noqa: E501
+            name (str): Unique identifier for virtual instance, can contain alphanumeric or dash characters.
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
-            description (str): New virtual instance description.. [optional]  # noqa: E501
-            monitoring_enabled (bool): [optional]  # noqa: E501
-            name (str): New virtual instance name.. [optional]  # noqa: E501
-            new_size (str): Requested virtual instance size.. [optional]  # noqa: E501
+            description (str): Description of requested virtual instance.. [optional]  # noqa: E501
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
+            mount_refresh_interval_seconds (int): Number of seconds between data refreshes for mounts on this Virtual Instance. A value of 0 means continuous refresh and a value of null means never refresh.. [optional]  # noqa: E501
+            type (str): Requested virtual instance type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -273,14 +276,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/update_virtual_instance_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/query_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,38 +7,40 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.virtual_instance import VirtualInstance
-    globals()['VirtualInstance'] = VirtualInstance
+    from rockset_v2.model.async_query_options import AsyncQueryOptions
+    from rockset_v2.model.query_request_sql import QueryRequestSql
+    globals()['AsyncQueryOptions'] = AsyncQueryOptions
+    globals()['QueryRequestSql'] = QueryRequestSql
 
 
-class UpdateVirtualInstanceResponse(ModelNormal):
+class QueryRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,35 +85,42 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (VirtualInstance, none_type),  # noqa: E501
+            'sql': (QueryRequestSql,),  # noqa: E501
+            'async_options': (AsyncQueryOptions, none_type),  # noqa: E501
+            'timeout_ms': (int, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'sql': 'sql',  # noqa: E501
+        'async_options': 'async_options',  # noqa: E501
+        'timeout_ms': 'timeout_ms',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateVirtualInstanceResponse - a model defined in OpenAPI
+    def _from_openapi_data(cls, sql, *args, **kwargs):  # noqa: E501
+        """QueryRequest - a model defined in OpenAPI
+
+        Args:
+            sql (QueryRequestSql):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +145,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (VirtualInstance): [optional]  # noqa: E501
+            async_options (AsyncQueryOptions): [optional]  # noqa: E501
+            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error. The maximum value for this timeout is 2 minutes. async_options.timeout_ms will override this timeout.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -164,14 +174,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.sql = sql
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -184,19 +195,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, **kwargs):  # noqa: E501
-        """UpdateVirtualInstanceResponse - a model defined in OpenAPI
+    def __init__(self, *, sql, **kwargs):  # noqa: E501
+        """QueryRequest - a model defined in OpenAPI
 
         Keyword Args:
-            data (VirtualInstance): [optional]  # noqa: E501
+            sql (QueryRequestSql):
+            async_options (AsyncQueryOptions): [optional]  # noqa: E501
+            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error. The maximum value for this timeout is 2 minutes. async_options.timeout_ms will override this timeout.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -245,14 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.sql = sql
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/user.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class User(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/validate_query_response.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/validate_query_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class ValidateQueryResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/view.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class View(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/virtual_instance.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/virtual_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,34 +7,36 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.virtual_instance_stats import VirtualInstanceStats
+    from rockset_v2.model.auto_scaling_policy import AutoScalingPolicy
+    from rockset_v2.model.virtual_instance_stats import VirtualInstanceStats
+    globals()['AutoScalingPolicy'] = AutoScalingPolicy
     globals()['VirtualInstanceStats'] = VirtualInstanceStats
 
 
 class VirtualInstance(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -122,48 +124,54 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
+            'auto_scaling_policy': (AutoScalingPolicy, none_type),  # noqa: E501
             'auto_suspend_seconds': (int, none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
             'created_by': (str, none_type),  # noqa: E501
             'current_size': (str, none_type),  # noqa: E501
             'default_pod_count': (int, none_type),  # noqa: E501
             'default_vi': (bool, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'desired_size': (str, none_type),  # noqa: E501
+            'enable_remount_on_resume': (bool, none_type),  # noqa: E501
             'id': (str, none_type),  # noqa: E501
             'monitoring_enabled': (bool, none_type),  # noqa: E501
+            'mount_refresh_interval_seconds': (int, none_type),  # noqa: E501
             'resumed_at': (str, none_type),  # noqa: E501
             'rrn': (str, none_type),  # noqa: E501
             'scaled_pod_count': (int, none_type),  # noqa: E501
             'state': (str, none_type),  # noqa: E501
             'stats': (VirtualInstanceStats, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
+        'auto_scaling_policy': 'auto_scaling_policy',  # noqa: E501
         'auto_suspend_seconds': 'auto_suspend_seconds',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
         'created_by': 'created_by',  # noqa: E501
         'current_size': 'current_size',  # noqa: E501
         'default_pod_count': 'default_pod_count',  # noqa: E501
         'default_vi': 'default_vi',  # noqa: E501
         'description': 'description',  # noqa: E501
         'desired_size': 'desired_size',  # noqa: E501
+        'enable_remount_on_resume': 'enable_remount_on_resume',  # noqa: E501
         'id': 'id',  # noqa: E501
         'monitoring_enabled': 'monitoring_enabled',  # noqa: E501
+        'mount_refresh_interval_seconds': 'mount_refresh_interval_seconds',  # noqa: E501
         'resumed_at': 'resumed_at',  # noqa: E501
         'rrn': 'rrn',  # noqa: E501
         'scaled_pod_count': 'scaled_pod_count',  # noqa: E501
         'state': 'state',  # noqa: E501
         'stats': 'stats',  # noqa: E501
     }
 
@@ -209,24 +217,27 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            auto_scaling_policy (AutoScalingPolicy): [optional]  # noqa: E501
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
             created_at (str): ISO-8601 date of when virtual instance was created.. [optional]  # noqa: E501
             created_by (str): Creator of requested virtual instance.. [optional]  # noqa: E501
             current_size (str): Virtual instance current size.. [optional]  # noqa: E501
             default_pod_count (int): [optional]  # noqa: E501
             default_vi (bool): [optional]  # noqa: E501
             description (str): Virtual instance description.. [optional]  # noqa: E501
             desired_size (str): Virtual instance desired size.. [optional]  # noqa: E501
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
             id (str): Unique identifier for virtual instance.. [optional]  # noqa: E501
             monitoring_enabled (bool): [optional]  # noqa: E501
+            mount_refresh_interval_seconds (int): Number of seconds between data refreshes for mounts on this Virtual Instance. [optional]  # noqa: E501
             resumed_at (str): ISO-8601 date of when virtual instance was created.. [optional]  # noqa: E501
             rrn (str): Virtual Instance RRN.. [optional]  # noqa: E501
             scaled_pod_count (int): [optional]  # noqa: E501
             state (str): Virtual instance state.. [optional]  # noqa: E501
             stats (VirtualInstanceStats): [optional]  # noqa: E501
         """
 
@@ -277,22 +288,25 @@
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
         """VirtualInstance - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Virtual instance name.
+            auto_scaling_policy (AutoScalingPolicy): [optional]  # noqa: E501
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
             created_at (str): ISO-8601 date of when virtual instance was created.. [optional]  # noqa: E501
             created_by (str): Creator of requested virtual instance.. [optional]  # noqa: E501
             default_pod_count (int): [optional]  # noqa: E501
             default_vi (bool): [optional]  # noqa: E501
             description (str): Virtual instance description.. [optional]  # noqa: E501
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
             id (str): Unique identifier for virtual instance.. [optional]  # noqa: E501
             monitoring_enabled (bool): [optional]  # noqa: E501
+            mount_refresh_interval_seconds (int): Number of seconds between data refreshes for mounts on this Virtual Instance. [optional]  # noqa: E501
             resumed_at (str): ISO-8601 date of when virtual instance was created.. [optional]  # noqa: E501
             rrn (str): Virtual Instance RRN.. [optional]  # noqa: E501
             scaled_pod_count (int): [optional]  # noqa: E501
             state (str): Virtual instance state.. [optional]  # noqa: E501
             stats (VirtualInstanceStats): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/virtual_instance_stats.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/update_collection_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,34 +7,38 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rockset_v2.model.field_mapping_query import FieldMappingQuery
+    globals()['FieldMappingQuery'] = FieldMappingQuery
 
-class VirtualInstanceStats(ModelNormal):
+
+class UpdateCollectionRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,50 +66,54 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'last_queried_ms': (int, none_type),  # noqa: E501
+            'description': (str, none_type),  # noqa: E501
+            'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'last_queried_ms': 'last_queried_ms',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'field_mapping_query': 'field_mapping_query',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """VirtualInstanceStats - a model defined in OpenAPI
+        """UpdateCollectionRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            last_queried_ms (int): Milliseconds since Unix epoch Jan 1, 1970.. [optional]  # noqa: E501
+            description (str): Updated text describing the collection.. [optional]  # noqa: E501
+            field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -179,18 +188,19 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """VirtualInstanceStats - a model defined in OpenAPI
+        """UpdateCollectionRequest - a model defined in OpenAPI
 
         Keyword Args:
-            last_queried_ms (int): Milliseconds since Unix epoch Jan 1, 1970.. [optional]  # noqa: E501
+            description (str): Updated text describing the collection.. [optional]  # noqa: E501
+            field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/workspace.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class Workspace(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model/xml_params.py` & `rockset_v2_internal-2.0.2/rockset_v2/model/xml_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from rockset.model_utils import (  # noqa: F401
+from rockset_v2.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from rockset.exceptions import ApiAttributeError
+from rockset_v2.exceptions import ApiAttributeError
 
 
 
 class XmlParams(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/model_utils.py` & `rockset_v2_internal-2.0.2/rockset_v2/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import os
 import pprint
 import re
 import tempfile
 
 from dateutil.parser import parse
 
-from rockset.exceptions import (
+from rockset_v2.exceptions import (
     ApiKeyError,
     ApiAttributeError,
     ApiTypeError,
     ApiValueError,
 )
 
 none_type = type(None)
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/models/__init__.py` & `rockset_v2_internal-2.0.2/rockset_v2/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,213 +1,216 @@
 # flake8: noqa
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
-# from from rockset.model.pet import Pet
+# from from rockset_v2.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
-from rockset.model.add_documents_request import AddDocumentsRequest
-from rockset.model.add_documents_response import AddDocumentsResponse
-from rockset.model.alias import Alias
-from rockset.model.api_key import ApiKey
-from rockset.model.async_query_options import AsyncQueryOptions
-from rockset.model.aws_access_key import AwsAccessKey
-from rockset.model.aws_role import AwsRole
-from rockset.model.azure_blob_storage_collection_creation_request import AzureBlobStorageCollectionCreationRequest
-from rockset.model.azure_blob_storage_integration import AzureBlobStorageIntegration
-from rockset.model.azure_blob_storage_integration_creation_request import AzureBlobStorageIntegrationCreationRequest
-from rockset.model.azure_blob_storage_source_wrapper import AzureBlobStorageSourceWrapper
-from rockset.model.azure_event_hubs_collection_creation_request import AzureEventHubsCollectionCreationRequest
-from rockset.model.azure_event_hubs_integration import AzureEventHubsIntegration
-from rockset.model.azure_event_hubs_integration_creation_request import AzureEventHubsIntegrationCreationRequest
-from rockset.model.azure_event_hubs_source_wrapper import AzureEventHubsSourceWrapper
-from rockset.model.azure_service_bus_collection_creation_request import AzureServiceBusCollectionCreationRequest
-from rockset.model.azure_service_bus_integration import AzureServiceBusIntegration
-from rockset.model.azure_service_bus_source_wrapper import AzureServiceBusSourceWrapper
-from rockset.model.bulk_stats import BulkStats
-from rockset.model.cancel_query_response import CancelQueryResponse
-from rockset.model.cluster import Cluster
-from rockset.model.collection import Collection
-from rockset.model.collection_mount import CollectionMount
-from rockset.model.collection_mount_response import CollectionMountResponse
-from rockset.model.collection_mount_stats import CollectionMountStats
-from rockset.model.collection_stats import CollectionStats
-from rockset.model.create_alias_request import CreateAliasRequest
-from rockset.model.create_alias_response import CreateAliasResponse
-from rockset.model.create_api_key_request import CreateApiKeyRequest
-from rockset.model.create_api_key_response import CreateApiKeyResponse
-from rockset.model.create_collection_mount_request import CreateCollectionMountRequest
-from rockset.model.create_collection_mounts_response import CreateCollectionMountsResponse
-from rockset.model.create_collection_request import CreateCollectionRequest
-from rockset.model.create_collection_response import CreateCollectionResponse
-from rockset.model.create_integration_request import CreateIntegrationRequest
-from rockset.model.create_integration_response import CreateIntegrationResponse
-from rockset.model.create_query_lambda_request import CreateQueryLambdaRequest
-from rockset.model.create_query_lambda_tag_request import CreateQueryLambdaTagRequest
-from rockset.model.create_role_request import CreateRoleRequest
-from rockset.model.create_user_request import CreateUserRequest
-from rockset.model.create_user_response import CreateUserResponse
-from rockset.model.create_view_request import CreateViewRequest
-from rockset.model.create_view_response import CreateViewResponse
-from rockset.model.create_virtual_instance_request import CreateVirtualInstanceRequest
-from rockset.model.create_virtual_instance_response import CreateVirtualInstanceResponse
-from rockset.model.create_workspace_request import CreateWorkspaceRequest
-from rockset.model.create_workspace_response import CreateWorkspaceResponse
-from rockset.model.csv_params import CsvParams
-from rockset.model.delete_alias_response import DeleteAliasResponse
-from rockset.model.delete_api_key_response import DeleteApiKeyResponse
-from rockset.model.delete_collection_response import DeleteCollectionResponse
-from rockset.model.delete_documents_request import DeleteDocumentsRequest
-from rockset.model.delete_documents_request_data import DeleteDocumentsRequestData
-from rockset.model.delete_documents_response import DeleteDocumentsResponse
-from rockset.model.delete_integration_response import DeleteIntegrationResponse
-from rockset.model.delete_query_lambda_response import DeleteQueryLambdaResponse
-from rockset.model.delete_user_response import DeleteUserResponse
-from rockset.model.delete_view_response import DeleteViewResponse
-from rockset.model.delete_virtual_instance_response import DeleteVirtualInstanceResponse
-from rockset.model.delete_workspace_response import DeleteWorkspaceResponse
-from rockset.model.document_status import DocumentStatus
-from rockset.model.dynamodb_collection_creation_request import DynamodbCollectionCreationRequest
-from rockset.model.dynamodb_integration import DynamodbIntegration
-from rockset.model.dynamodb_integration_creation_request import DynamodbIntegrationCreationRequest
-from rockset.model.dynamodb_source_wrapper import DynamodbSourceWrapper
-from rockset.model.error_model import ErrorModel
-from rockset.model.event_time_info import EventTimeInfo
-from rockset.model.execute_public_query_lambda_request import ExecutePublicQueryLambdaRequest
-from rockset.model.execute_query_lambda_request import ExecuteQueryLambdaRequest
-from rockset.model.field_mapping_query import FieldMappingQuery
-from rockset.model.field_mapping_v2 import FieldMappingV2
-from rockset.model.field_partition import FieldPartition
-from rockset.model.file_upload_collection_creation_request import FileUploadCollectionCreationRequest
-from rockset.model.file_upload_source_wrapper import FileUploadSourceWrapper
-from rockset.model.format_params import FormatParams
-from rockset.model.gcp_service_account import GcpServiceAccount
-from rockset.model.gcs_collection_creation_request import GcsCollectionCreationRequest
-from rockset.model.gcs_integration import GcsIntegration
-from rockset.model.gcs_integration_creation_request import GcsIntegrationCreationRequest
-from rockset.model.gcs_source_wrapper import GcsSourceWrapper
-from rockset.model.get_alias_response import GetAliasResponse
-from rockset.model.get_api_key_response import GetApiKeyResponse
-from rockset.model.get_collection_response import GetCollectionResponse
-from rockset.model.get_integration_response import GetIntegrationResponse
-from rockset.model.get_query_response import GetQueryResponse
-from rockset.model.get_view_response import GetViewResponse
-from rockset.model.get_virtual_instance_response import GetVirtualInstanceResponse
-from rockset.model.get_workspace_response import GetWorkspaceResponse
-from rockset.model.input_field import InputField
-from rockset.model.integration import Integration
-from rockset.model.kafka_collection_creation_request import KafkaCollectionCreationRequest
-from rockset.model.kafka_integration import KafkaIntegration
-from rockset.model.kafka_integration_creation_request import KafkaIntegrationCreationRequest
-from rockset.model.kafka_source_wrapper import KafkaSourceWrapper
-from rockset.model.kafka_v3_security_config import KafkaV3SecurityConfig
-from rockset.model.kinesis_collection_creation_request import KinesisCollectionCreationRequest
-from rockset.model.kinesis_integration import KinesisIntegration
-from rockset.model.kinesis_integration_creation_request import KinesisIntegrationCreationRequest
-from rockset.model.kinesis_source_wrapper import KinesisSourceWrapper
-from rockset.model.list_aliases_response import ListAliasesResponse
-from rockset.model.list_api_keys_response import ListApiKeysResponse
-from rockset.model.list_collection_mounts_response import ListCollectionMountsResponse
-from rockset.model.list_collections_response import ListCollectionsResponse
-from rockset.model.list_integrations_response import ListIntegrationsResponse
-from rockset.model.list_queries_response import ListQueriesResponse
-from rockset.model.list_query_lambda_tags_response import ListQueryLambdaTagsResponse
-from rockset.model.list_query_lambda_versions_response import ListQueryLambdaVersionsResponse
-from rockset.model.list_query_lambdas_response import ListQueryLambdasResponse
-from rockset.model.list_roles_response import ListRolesResponse
-from rockset.model.list_unsubscribe_preferences_response import ListUnsubscribePreferencesResponse
-from rockset.model.list_users_response import ListUsersResponse
-from rockset.model.list_views_response import ListViewsResponse
-from rockset.model.list_virtual_instances_response import ListVirtualInstancesResponse
-from rockset.model.list_workspaces_response import ListWorkspacesResponse
-from rockset.model.mongo_db_integration import MongoDbIntegration
-from rockset.model.mongodb_collection_creation_request import MongodbCollectionCreationRequest
-from rockset.model.mongodb_integration_creation_request import MongodbIntegrationCreationRequest
-from rockset.model.mongodb_source_wrapper import MongodbSourceWrapper
-from rockset.model.organization import Organization
-from rockset.model.organization_response import OrganizationResponse
-from rockset.model.output_field import OutputField
-from rockset.model.pagination import Pagination
-from rockset.model.pagination_info import PaginationInfo
-from rockset.model.patch_document import PatchDocument
-from rockset.model.patch_documents_request import PatchDocumentsRequest
-from rockset.model.patch_documents_response import PatchDocumentsResponse
-from rockset.model.patch_operation import PatchOperation
-from rockset.model.privilege import Privilege
-from rockset.model.query_error import QueryError
-from rockset.model.query_field_type import QueryFieldType
-from rockset.model.query_info import QueryInfo
-from rockset.model.query_lambda import QueryLambda
-from rockset.model.query_lambda_sql import QueryLambdaSql
-from rockset.model.query_lambda_stats import QueryLambdaStats
-from rockset.model.query_lambda_tag import QueryLambdaTag
-from rockset.model.query_lambda_tag_response import QueryLambdaTagResponse
-from rockset.model.query_lambda_version import QueryLambdaVersion
-from rockset.model.query_lambda_version_response import QueryLambdaVersionResponse
-from rockset.model.query_pagination_response import QueryPaginationResponse
-from rockset.model.query_parameter import QueryParameter
-from rockset.model.query_request import QueryRequest
-from rockset.model.query_request_sql import QueryRequestSql
-from rockset.model.query_response import QueryResponse
-from rockset.model.query_response_stats import QueryResponseStats
-from rockset.model.resume_virtual_instance_response import ResumeVirtualInstanceResponse
-from rockset.model.role import Role
-from rockset.model.role_response import RoleResponse
-from rockset.model.s3_collection_creation_request import S3CollectionCreationRequest
-from rockset.model.s3_integration import S3Integration
-from rockset.model.s3_integration_creation_request import S3IntegrationCreationRequest
-from rockset.model.s3_source_wrapper import S3SourceWrapper
-from rockset.model.schema_registry_config import SchemaRegistryConfig
-from rockset.model.snowflake_collection_creation_request import SnowflakeCollectionCreationRequest
-from rockset.model.snowflake_integration import SnowflakeIntegration
-from rockset.model.snowflake_integration_creation_request import SnowflakeIntegrationCreationRequest
-from rockset.model.snowflake_source_wrapper import SnowflakeSourceWrapper
-from rockset.model.source import Source
-from rockset.model.source_azure_blob_storage import SourceAzureBlobStorage
-from rockset.model.source_azure_event_hubs import SourceAzureEventHubs
-from rockset.model.source_azure_service_bus import SourceAzureServiceBus
-from rockset.model.source_dynamo_db import SourceDynamoDb
-from rockset.model.source_file_upload import SourceFileUpload
-from rockset.model.source_gcs import SourceGcs
-from rockset.model.source_kafka import SourceKafka
-from rockset.model.source_kinesis import SourceKinesis
-from rockset.model.source_mongo_db import SourceMongoDb
-from rockset.model.source_s3 import SourceS3
-from rockset.model.source_snowflake import SourceSnowflake
-from rockset.model.sql_expression import SqlExpression
-from rockset.model.stats import Stats
-from rockset.model.status import Status
-from rockset.model.status_azure_event_hubs import StatusAzureEventHubs
-from rockset.model.status_azure_event_hubs_partition import StatusAzureEventHubsPartition
-from rockset.model.status_azure_service_bus import StatusAzureServiceBus
-from rockset.model.status_azure_service_bus_session import StatusAzureServiceBusSession
-from rockset.model.status_dynamo_db import StatusDynamoDb
-from rockset.model.status_dynamo_db_v2 import StatusDynamoDbV2
-from rockset.model.status_kafka import StatusKafka
-from rockset.model.status_kafka_partition import StatusKafkaPartition
-from rockset.model.status_mongo_db import StatusMongoDb
-from rockset.model.status_snowflake import StatusSnowflake
-from rockset.model.suspend_virtual_instance_response import SuspendVirtualInstanceResponse
-from rockset.model.unsubscribe_preference import UnsubscribePreference
-from rockset.model.update_alias_request import UpdateAliasRequest
-from rockset.model.update_api_key_request import UpdateApiKeyRequest
-from rockset.model.update_api_key_response import UpdateApiKeyResponse
-from rockset.model.update_query_lambda_request import UpdateQueryLambdaRequest
-from rockset.model.update_role_request import UpdateRoleRequest
-from rockset.model.update_unsubscribe_preferences_request import UpdateUnsubscribePreferencesRequest
-from rockset.model.update_unsubscribe_preferences_response import UpdateUnsubscribePreferencesResponse
-from rockset.model.update_user_request import UpdateUserRequest
-from rockset.model.update_view_request import UpdateViewRequest
-from rockset.model.update_view_response import UpdateViewResponse
-from rockset.model.update_virtual_instance_request import UpdateVirtualInstanceRequest
-from rockset.model.update_virtual_instance_response import UpdateVirtualInstanceResponse
-from rockset.model.user import User
-from rockset.model.validate_query_response import ValidateQueryResponse
-from rockset.model.view import View
-from rockset.model.virtual_instance import VirtualInstance
-from rockset.model.virtual_instance_stats import VirtualInstanceStats
-from rockset.model.workspace import Workspace
-from rockset.model.xml_params import XmlParams
+from rockset_v2.model.add_documents_request import AddDocumentsRequest
+from rockset_v2.model.add_documents_response import AddDocumentsResponse
+from rockset_v2.model.alias import Alias
+from rockset_v2.model.api_key import ApiKey
+from rockset_v2.model.async_query_options import AsyncQueryOptions
+from rockset_v2.model.auto_scaling_policy import AutoScalingPolicy
+from rockset_v2.model.aws_access_key import AwsAccessKey
+from rockset_v2.model.aws_role import AwsRole
+from rockset_v2.model.azure_blob_storage_collection_creation_request import AzureBlobStorageCollectionCreationRequest
+from rockset_v2.model.azure_blob_storage_integration import AzureBlobStorageIntegration
+from rockset_v2.model.azure_blob_storage_integration_creation_request import AzureBlobStorageIntegrationCreationRequest
+from rockset_v2.model.azure_blob_storage_source_wrapper import AzureBlobStorageSourceWrapper
+from rockset_v2.model.azure_event_hubs_collection_creation_request import AzureEventHubsCollectionCreationRequest
+from rockset_v2.model.azure_event_hubs_integration import AzureEventHubsIntegration
+from rockset_v2.model.azure_event_hubs_integration_creation_request import AzureEventHubsIntegrationCreationRequest
+from rockset_v2.model.azure_event_hubs_source_wrapper import AzureEventHubsSourceWrapper
+from rockset_v2.model.azure_service_bus_collection_creation_request import AzureServiceBusCollectionCreationRequest
+from rockset_v2.model.azure_service_bus_integration import AzureServiceBusIntegration
+from rockset_v2.model.azure_service_bus_source_wrapper import AzureServiceBusSourceWrapper
+from rockset_v2.model.bulk_stats import BulkStats
+from rockset_v2.model.cancel_query_response import CancelQueryResponse
+from rockset_v2.model.cluster import Cluster
+from rockset_v2.model.collection import Collection
+from rockset_v2.model.collection_mount import CollectionMount
+from rockset_v2.model.collection_mount_response import CollectionMountResponse
+from rockset_v2.model.collection_mount_stats import CollectionMountStats
+from rockset_v2.model.collection_stats import CollectionStats
+from rockset_v2.model.create_alias_request import CreateAliasRequest
+from rockset_v2.model.create_alias_response import CreateAliasResponse
+from rockset_v2.model.create_api_key_request import CreateApiKeyRequest
+from rockset_v2.model.create_api_key_response import CreateApiKeyResponse
+from rockset_v2.model.create_collection_mount_request import CreateCollectionMountRequest
+from rockset_v2.model.create_collection_mounts_response import CreateCollectionMountsResponse
+from rockset_v2.model.create_collection_request import CreateCollectionRequest
+from rockset_v2.model.create_collection_response import CreateCollectionResponse
+from rockset_v2.model.create_integration_request import CreateIntegrationRequest
+from rockset_v2.model.create_integration_response import CreateIntegrationResponse
+from rockset_v2.model.create_query_lambda_request import CreateQueryLambdaRequest
+from rockset_v2.model.create_query_lambda_tag_request import CreateQueryLambdaTagRequest
+from rockset_v2.model.create_role_request import CreateRoleRequest
+from rockset_v2.model.create_user_request import CreateUserRequest
+from rockset_v2.model.create_user_response import CreateUserResponse
+from rockset_v2.model.create_view_request import CreateViewRequest
+from rockset_v2.model.create_view_response import CreateViewResponse
+from rockset_v2.model.create_virtual_instance_request import CreateVirtualInstanceRequest
+from rockset_v2.model.create_virtual_instance_response import CreateVirtualInstanceResponse
+from rockset_v2.model.create_workspace_request import CreateWorkspaceRequest
+from rockset_v2.model.create_workspace_response import CreateWorkspaceResponse
+from rockset_v2.model.csv_params import CsvParams
+from rockset_v2.model.delete_alias_response import DeleteAliasResponse
+from rockset_v2.model.delete_api_key_response import DeleteApiKeyResponse
+from rockset_v2.model.delete_collection_response import DeleteCollectionResponse
+from rockset_v2.model.delete_documents_request import DeleteDocumentsRequest
+from rockset_v2.model.delete_documents_request_data import DeleteDocumentsRequestData
+from rockset_v2.model.delete_documents_response import DeleteDocumentsResponse
+from rockset_v2.model.delete_integration_response import DeleteIntegrationResponse
+from rockset_v2.model.delete_query_lambda_response import DeleteQueryLambdaResponse
+from rockset_v2.model.delete_user_response import DeleteUserResponse
+from rockset_v2.model.delete_view_response import DeleteViewResponse
+from rockset_v2.model.delete_virtual_instance_response import DeleteVirtualInstanceResponse
+from rockset_v2.model.delete_workspace_response import DeleteWorkspaceResponse
+from rockset_v2.model.document_status import DocumentStatus
+from rockset_v2.model.dynamodb_collection_creation_request import DynamodbCollectionCreationRequest
+from rockset_v2.model.dynamodb_integration import DynamodbIntegration
+from rockset_v2.model.dynamodb_integration_creation_request import DynamodbIntegrationCreationRequest
+from rockset_v2.model.dynamodb_source_wrapper import DynamodbSourceWrapper
+from rockset_v2.model.error_model import ErrorModel
+from rockset_v2.model.event_time_info import EventTimeInfo
+from rockset_v2.model.execute_public_query_lambda_request import ExecutePublicQueryLambdaRequest
+from rockset_v2.model.execute_query_lambda_request import ExecuteQueryLambdaRequest
+from rockset_v2.model.field_mapping_query import FieldMappingQuery
+from rockset_v2.model.field_mapping_v2 import FieldMappingV2
+from rockset_v2.model.field_partition import FieldPartition
+from rockset_v2.model.file_upload_collection_creation_request import FileUploadCollectionCreationRequest
+from rockset_v2.model.file_upload_source_wrapper import FileUploadSourceWrapper
+from rockset_v2.model.format_params import FormatParams
+from rockset_v2.model.gcp_service_account import GcpServiceAccount
+from rockset_v2.model.gcs_collection_creation_request import GcsCollectionCreationRequest
+from rockset_v2.model.gcs_integration import GcsIntegration
+from rockset_v2.model.gcs_integration_creation_request import GcsIntegrationCreationRequest
+from rockset_v2.model.gcs_source_wrapper import GcsSourceWrapper
+from rockset_v2.model.get_alias_response import GetAliasResponse
+from rockset_v2.model.get_api_key_response import GetApiKeyResponse
+from rockset_v2.model.get_collection_response import GetCollectionResponse
+from rockset_v2.model.get_integration_response import GetIntegrationResponse
+from rockset_v2.model.get_query_response import GetQueryResponse
+from rockset_v2.model.get_view_response import GetViewResponse
+from rockset_v2.model.get_virtual_instance_response import GetVirtualInstanceResponse
+from rockset_v2.model.get_workspace_response import GetWorkspaceResponse
+from rockset_v2.model.input_field import InputField
+from rockset_v2.model.integration import Integration
+from rockset_v2.model.kafka_collection_creation_request import KafkaCollectionCreationRequest
+from rockset_v2.model.kafka_integration import KafkaIntegration
+from rockset_v2.model.kafka_integration_creation_request import KafkaIntegrationCreationRequest
+from rockset_v2.model.kafka_source_wrapper import KafkaSourceWrapper
+from rockset_v2.model.kafka_v3_security_config import KafkaV3SecurityConfig
+from rockset_v2.model.kinesis_collection_creation_request import KinesisCollectionCreationRequest
+from rockset_v2.model.kinesis_integration import KinesisIntegration
+from rockset_v2.model.kinesis_integration_creation_request import KinesisIntegrationCreationRequest
+from rockset_v2.model.kinesis_source_wrapper import KinesisSourceWrapper
+from rockset_v2.model.list_aliases_response import ListAliasesResponse
+from rockset_v2.model.list_api_keys_response import ListApiKeysResponse
+from rockset_v2.model.list_collection_mounts_response import ListCollectionMountsResponse
+from rockset_v2.model.list_collections_response import ListCollectionsResponse
+from rockset_v2.model.list_integrations_response import ListIntegrationsResponse
+from rockset_v2.model.list_queries_response import ListQueriesResponse
+from rockset_v2.model.list_query_lambda_tags_response import ListQueryLambdaTagsResponse
+from rockset_v2.model.list_query_lambda_versions_response import ListQueryLambdaVersionsResponse
+from rockset_v2.model.list_query_lambdas_response import ListQueryLambdasResponse
+from rockset_v2.model.list_roles_response import ListRolesResponse
+from rockset_v2.model.list_unsubscribe_preferences_response import ListUnsubscribePreferencesResponse
+from rockset_v2.model.list_users_response import ListUsersResponse
+from rockset_v2.model.list_views_response import ListViewsResponse
+from rockset_v2.model.list_virtual_instances_response import ListVirtualInstancesResponse
+from rockset_v2.model.list_workspaces_response import ListWorkspacesResponse
+from rockset_v2.model.mongo_db_integration import MongoDbIntegration
+from rockset_v2.model.mongodb_collection_creation_request import MongodbCollectionCreationRequest
+from rockset_v2.model.mongodb_integration_creation_request import MongodbIntegrationCreationRequest
+from rockset_v2.model.mongodb_source_wrapper import MongodbSourceWrapper
+from rockset_v2.model.organization import Organization
+from rockset_v2.model.organization_response import OrganizationResponse
+from rockset_v2.model.output_field import OutputField
+from rockset_v2.model.pagination import Pagination
+from rockset_v2.model.pagination_info import PaginationInfo
+from rockset_v2.model.patch_document import PatchDocument
+from rockset_v2.model.patch_documents_request import PatchDocumentsRequest
+from rockset_v2.model.patch_documents_response import PatchDocumentsResponse
+from rockset_v2.model.patch_operation import PatchOperation
+from rockset_v2.model.privilege import Privilege
+from rockset_v2.model.query_error import QueryError
+from rockset_v2.model.query_field_type import QueryFieldType
+from rockset_v2.model.query_info import QueryInfo
+from rockset_v2.model.query_lambda import QueryLambda
+from rockset_v2.model.query_lambda_sql import QueryLambdaSql
+from rockset_v2.model.query_lambda_stats import QueryLambdaStats
+from rockset_v2.model.query_lambda_tag import QueryLambdaTag
+from rockset_v2.model.query_lambda_tag_response import QueryLambdaTagResponse
+from rockset_v2.model.query_lambda_version import QueryLambdaVersion
+from rockset_v2.model.query_lambda_version_response import QueryLambdaVersionResponse
+from rockset_v2.model.query_pagination_response import QueryPaginationResponse
+from rockset_v2.model.query_parameter import QueryParameter
+from rockset_v2.model.query_request import QueryRequest
+from rockset_v2.model.query_request_sql import QueryRequestSql
+from rockset_v2.model.query_response import QueryResponse
+from rockset_v2.model.query_response_stats import QueryResponseStats
+from rockset_v2.model.resume_virtual_instance_response import ResumeVirtualInstanceResponse
+from rockset_v2.model.role import Role
+from rockset_v2.model.role_response import RoleResponse
+from rockset_v2.model.s3_collection_creation_request import S3CollectionCreationRequest
+from rockset_v2.model.s3_integration import S3Integration
+from rockset_v2.model.s3_integration_creation_request import S3IntegrationCreationRequest
+from rockset_v2.model.s3_source_wrapper import S3SourceWrapper
+from rockset_v2.model.schema_registry_config import SchemaRegistryConfig
+from rockset_v2.model.snowflake_collection_creation_request import SnowflakeCollectionCreationRequest
+from rockset_v2.model.snowflake_integration import SnowflakeIntegration
+from rockset_v2.model.snowflake_integration_creation_request import SnowflakeIntegrationCreationRequest
+from rockset_v2.model.snowflake_source_wrapper import SnowflakeSourceWrapper
+from rockset_v2.model.source import Source
+from rockset_v2.model.source_azure_blob_storage import SourceAzureBlobStorage
+from rockset_v2.model.source_azure_event_hubs import SourceAzureEventHubs
+from rockset_v2.model.source_azure_service_bus import SourceAzureServiceBus
+from rockset_v2.model.source_dynamo_db import SourceDynamoDb
+from rockset_v2.model.source_file_upload import SourceFileUpload
+from rockset_v2.model.source_gcs import SourceGcs
+from rockset_v2.model.source_kafka import SourceKafka
+from rockset_v2.model.source_kinesis import SourceKinesis
+from rockset_v2.model.source_mongo_db import SourceMongoDb
+from rockset_v2.model.source_s3 import SourceS3
+from rockset_v2.model.source_snowflake import SourceSnowflake
+from rockset_v2.model.source_system import SourceSystem
+from rockset_v2.model.sql_expression import SqlExpression
+from rockset_v2.model.stats import Stats
+from rockset_v2.model.status import Status
+from rockset_v2.model.status_azure_event_hubs import StatusAzureEventHubs
+from rockset_v2.model.status_azure_event_hubs_partition import StatusAzureEventHubsPartition
+from rockset_v2.model.status_azure_service_bus import StatusAzureServiceBus
+from rockset_v2.model.status_azure_service_bus_session import StatusAzureServiceBusSession
+from rockset_v2.model.status_dynamo_db import StatusDynamoDb
+from rockset_v2.model.status_dynamo_db_v2 import StatusDynamoDbV2
+from rockset_v2.model.status_kafka import StatusKafka
+from rockset_v2.model.status_kafka_partition import StatusKafkaPartition
+from rockset_v2.model.status_mongo_db import StatusMongoDb
+from rockset_v2.model.status_snowflake import StatusSnowflake
+from rockset_v2.model.suspend_virtual_instance_response import SuspendVirtualInstanceResponse
+from rockset_v2.model.unsubscribe_preference import UnsubscribePreference
+from rockset_v2.model.update_alias_request import UpdateAliasRequest
+from rockset_v2.model.update_api_key_request import UpdateApiKeyRequest
+from rockset_v2.model.update_api_key_response import UpdateApiKeyResponse
+from rockset_v2.model.update_collection_request import UpdateCollectionRequest
+from rockset_v2.model.update_query_lambda_request import UpdateQueryLambdaRequest
+from rockset_v2.model.update_role_request import UpdateRoleRequest
+from rockset_v2.model.update_unsubscribe_preferences_request import UpdateUnsubscribePreferencesRequest
+from rockset_v2.model.update_unsubscribe_preferences_response import UpdateUnsubscribePreferencesResponse
+from rockset_v2.model.update_user_request import UpdateUserRequest
+from rockset_v2.model.update_view_request import UpdateViewRequest
+from rockset_v2.model.update_view_response import UpdateViewResponse
+from rockset_v2.model.update_virtual_instance_request import UpdateVirtualInstanceRequest
+from rockset_v2.model.update_virtual_instance_response import UpdateVirtualInstanceResponse
+from rockset_v2.model.user import User
+from rockset_v2.model.validate_query_response import ValidateQueryResponse
+from rockset_v2.model.view import View
+from rockset_v2.model.virtual_instance import VirtualInstance
+from rockset_v2.model.virtual_instance_stats import VirtualInstanceStats
+from rockset_v2.model.workspace import Workspace
+from rockset_v2.model.xml_params import XmlParams
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/query_paginator.py` & `rockset_v2_internal-2.0.2/rockset_v2/query_paginator.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/rest.py` & `rockset_v2_internal-2.0.2/rockset_v2/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import ssl
 from urllib.parse import urlencode
 from urllib.parse import urlparse
 from urllib.request import proxy_bypass_environment
 import urllib3
 import ipaddress
 
-from rockset.exceptions import ApiException, BadRequestException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+from rockset_v2.exceptions import ApiException, BadRequestException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/rockset_client.py` & `rockset_v2_internal-2.0.2/rockset_v2/rockset_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import inspect
 import re
 from enum import Enum
 from functools import wraps
 from types import FunctionType
 from typing import Any, Dict, Union
 
-from rockset.api_client import ApiClient
-from rockset.apis import (
+from rockset_v2.api_client import ApiClient
+from rockset_v2.apis import (
     Aliases,
     APIKeys,
     Collections,
     CustomRoles,
     Documents,
     Integrations,
     Organizations,
@@ -19,17 +19,17 @@
     QueryLambdas,
     SharedLambdas,
     Users,
     Views,
     VirtualInstances,
     Workspaces,
 )
-from rockset.configuration import Configuration
-from rockset.exceptions import ApiTypeError, ApiValueError, InitializationException
-from rockset.models import QueryParameter, QueryRequestSql, QueryResponse
+from rockset_v2.configuration import Configuration
+from rockset_v2.exceptions import ApiTypeError, ApiValueError, InitializationException
+from rockset_v2.models import QueryParameter, QueryRequestSql, QueryResponse
 
 
 APISERVER_PATTERN = re.compile(r"^https:\/\/(\w|-|\.)+\.rockset\.com$")
 
 
 class Regions(str, Enum):
     rs2 = "https://api.rs2.usw2.rockset.com"
```

### Comparing `rockset_v2_internal-2.0.1/rockset_v2/value.py` & `rockset_v2_internal-2.0.2/rockset_v2/value.py`

 * *Files identical despite different names*

### Comparing `rockset_v2_internal-2.0.1/PKG-INFO` & `rockset_v2_internal-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockset-v2-internal
-Version: 2.0.1
+Version: 2.0.2
 Summary: The python client for the Rockset API.
 Home-page: https://github.com/rockset/rockset-python-client
 License: Apache-2.0
 Author: Rockset
 Author-email: support@rockset.com
 Requires-Python: >=3.6,<4.0
 Classifier: Environment :: Console
```

