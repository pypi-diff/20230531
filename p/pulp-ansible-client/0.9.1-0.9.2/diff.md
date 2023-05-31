# Comparing `tmp/pulp_ansible-client-0.9.1.tar.gz` & `tmp/pulp_ansible-client-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_ansible-client-0.9.1.tar", last modified: Wed Aug 25 14:34:44 2021, max compression
+gzip compressed data, was "pulp_ansible-client-0.9.2.tar", last modified: Mon Oct  4 19:36:04 2021, max compression
```

## Comparing `pulp_ansible-client-0.9.1.tar` & `pulp_ansible-client-0.9.2.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:34:44.139558 pulp_ansible-client-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-08-25 14:34:44.139558 pulp_ansible-client-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17110 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:34:44.115557 pulp_ansible-client-0.9.1/pulp_ansible_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulp_ansible_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10054 2021-08-25 14:34:44.000000 pulp_ansible-client-0.9.1/pulp_ansible_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulp_ansible_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulp_ansible_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulp_ansible_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:34:44.115557 pulp_ansible-client-0.9.1/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:34:44.115557 pulp_ansible-client-0.9.1/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:34:44.115557 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/
--rw-r--r--   0 runner    (1001) docker     (121)     9752 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:34:44.119557 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14549 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/ansible_collections_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6199 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/ansible_copy_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    13384 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/api_collections_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     7340 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/api_roles_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     7292 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/collection_import_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    24931 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/content_collection_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    20370 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/content_roles_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    41591 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/distributions_ansible_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6749 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/galaxy_detail_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6217 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     8217 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v2_collections_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6467 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6598 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collection_versions_all_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     7334 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_all_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    21894 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    19308 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     8516 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_versions_docs_blob_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     8422 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_artifacts_collections_v3_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6947 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    42590 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/remotes_collection_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    41738 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/remotes_role_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    52775 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/repositories_ansible_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    32398 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/repositories_ansible_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    13823 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    26294 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13964 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:34:44.127558 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/
--rw-r--r--   0 runner    (1001) docker     (121)     6858 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8433 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_ansible_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)    11261 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_ansible_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     8427 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_ansible_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)    12124 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_ansible_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    28167 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_collection_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)    27280 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_collection_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4610 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_collection_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     8034 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_collection_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    30615 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_collection_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5387 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     5973 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_role.py
--rw-r--r--   0 runner    (1001) docker     (121)    23298 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_role_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)    22331 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_role_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     7708 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_role_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3388 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5108 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/artifact_ref_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3576 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     9860 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_import_detail_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    10209 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_metadata_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3528 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_namespace_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     7493 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_one_shot.py
--rw-r--r--   0 runner    (1001) docker     (121)     4818 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_ref_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     8391 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3658 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_version_docs_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    13173 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5175 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/content_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     5303 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3589 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/copy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5816 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/galaxy_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     8954 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/galaxy_collection_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     7522 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/galaxy_collection_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4877 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/galaxy_role_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4181 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/galaxy_role_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4990 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_collection_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5428 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_collection_response_list_links.py
--rw-r--r--   0 runner    (1001) docker     (121)     3458 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_collection_response_list_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     5123 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_collection_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5656 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_galaxy_collection_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5817 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_galaxy_collection_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5518 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_galaxy_role_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5679 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_galaxy_role_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5679 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5357 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_tag_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5886 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_ansible_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5840 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_ansible_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5817 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_collection_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5679 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_collection_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5840 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_collection_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5679 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_role_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5541 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_role_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     8316 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/patchedansible_ansible_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     8469 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/patchedansible_ansible_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)    28588 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/patchedansible_collection_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)    23607 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/patchedansible_role_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     2954 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     3592 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/repo_metadata_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6400 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     3702 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/repository_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     7919 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3246 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/tag_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12079 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/unpaginated_collection_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12315 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/rest.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-08-25 14:34:44.139558 pulp_ansible-client-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:34:44.139558 pulp_ansible-client-0.9.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_ansible_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_ansible_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_ansible_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_ansible_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_collection_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     2748 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_collection_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_collection_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_collection_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3960 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_collection_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_ansible_collections_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_ansible_copy_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_role_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_role_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_role_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_ansible_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_api_collections_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_api_roles_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_artifact_ref_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_collection_import_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2698 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_collection_import_detail_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_collection_metadata_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_collection_namespace_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_collection_one_shot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_collection_ref_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1882 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_collection_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_collection_version_docs_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_collection_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_content_collection_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_content_roles_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_content_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_distributions_ansible_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_galaxy_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_galaxy_collection_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3337 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_galaxy_collection_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)      873 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_galaxy_detail_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_galaxy_role_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_galaxy_role_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2758 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginated_collection_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginated_collection_response_list_links.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginated_collection_response_list_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginated_collection_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2593 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginated_galaxy_collection_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3367 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginated_galaxy_collection_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginated_galaxy_role_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginated_galaxy_role_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginated_tag_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginatedansible_ansible_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginatedansible_ansible_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3412 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginatedansible_collection_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginatedansible_collection_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3882 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginatedansible_collection_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginatedansible_role_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2287 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_paginatedansible_role_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1843 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_patchedansible_ansible_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_patchedansible_ansible_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     2543 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_patchedansible_collection_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_patchedansible_role_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)      887 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v2_collections_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v3_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v3_collection_versions_all_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v3_collections_all_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v3_collections_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v3_collections_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v3_collections_versions_docs_blob_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_pulp_ansible_artifacts_collections_v3_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_pulp_ansible_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_remotes_collection_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_remotes_role_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_repo_metadata_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1878 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_repositories_ansible_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_repositories_ansible_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_repository_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2399 2021-08-25 14:34:42.000000 pulp_ansible-client-0.9.1/test/test_unpaginated_collection_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2021-08-25 14:34:43.000000 pulp_ansible-client-0.9.1/test/test_versions_api.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:36:04.048354 pulp_ansible-client-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2021-10-04 19:36:04.048354 pulp_ansible-client-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    17110 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:36:04.020354 pulp_ansible-client-0.9.2/pulp_ansible_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulp_ansible_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10054 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulp_ansible_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulp_ansible_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulp_ansible_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulp_ansible_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:36:04.020354 pulp_ansible-client-0.9.2/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:36:04.020354 pulp_ansible-client-0.9.2/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:36:04.020354 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/
+-rw-r--r--   0 runner    (1001) docker     (121)     9752 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:36:04.024354 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     2447 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14549 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/ansible_collections_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6199 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/ansible_copy_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13384 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/api_collections_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7340 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/api_roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7292 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/collection_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24931 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/content_collection_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20370 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/content_roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41591 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/distributions_ansible_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6749 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/galaxy_detail_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6217 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8217 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v2_collections_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6467 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6598 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collection_versions_all_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7334 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_all_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21894 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19308 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8516 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_versions_docs_blob_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8422 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_artifacts_collections_v3_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6947 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42590 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/remotes_collection_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41738 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/remotes_role_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52775 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/repositories_ansible_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32398 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/repositories_ansible_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13823 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26294 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13964 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3769 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:36:04.032354 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     6858 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8433 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_ansible_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11261 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_ansible_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8427 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_ansible_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12124 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_ansible_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28167 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_collection_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27280 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_collection_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4610 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_collection_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8034 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_collection_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30615 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_collection_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5387 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5973 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_role.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23298 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_role_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22331 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_role_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7708 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3388 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5108 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/artifact_ref_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3576 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9860 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_import_detail_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10209 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_metadata_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3528 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_namespace_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7493 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_one_shot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4818 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_ref_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8391 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3658 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_version_docs_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13173 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5175 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/content_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5303 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3589 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5816 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/galaxy_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8954 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/galaxy_collection_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7522 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/galaxy_collection_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4877 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/galaxy_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4181 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/galaxy_role_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4990 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_collection_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5428 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_collection_response_list_links.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3458 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_collection_response_list_meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5123 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_collection_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5656 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_galaxy_collection_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5817 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_galaxy_collection_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5518 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_galaxy_role_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5679 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_galaxy_role_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5679 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5357 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_tag_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5886 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_ansible_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5840 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_ansible_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5817 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_collection_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5679 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_collection_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5840 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_collection_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5679 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_role_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5541 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_role_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8316 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/patchedansible_ansible_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8469 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/patchedansible_ansible_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28588 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/patchedansible_collection_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23607 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/patchedansible_role_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2954 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3592 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/repo_metadata_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6400 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3702 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/repository_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7919 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3246 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12079 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/unpaginated_collection_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12315 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/rest.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-10-04 19:36:04.048354 pulp_ansible-client-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:36:04.048354 pulp_ansible-client-0.9.2/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1827 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_ansible_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2153 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_ansible_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1852 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_ansible_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2225 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_ansible_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2521 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_collection_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2748 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_collection_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_collection_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1790 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_collection_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3960 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_collection_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_ansible_collections_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_ansible_copy_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1635 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_role_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2534 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_role_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1869 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1491 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_ansible_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_api_collections_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_api_roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_artifact_ref_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)      949 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_collection_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2698 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_collection_import_detail_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_collection_metadata_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1618 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_collection_namespace_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_collection_one_shot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1634 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_collection_ref_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1882 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_collection_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_collection_version_docs_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2341 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_collection_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_content_collection_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1149 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_content_roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1919 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_content_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2009 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1680 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_distributions_ansible_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_galaxy_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2199 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_galaxy_collection_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3337 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_galaxy_collection_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)      873 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_galaxy_detail_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1613 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_galaxy_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1629 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_galaxy_role_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2758 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginated_collection_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1785 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginated_collection_response_list_links.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginated_collection_response_list_meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3089 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginated_collection_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2593 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginated_galaxy_collection_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3367 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginated_galaxy_collection_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2069 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginated_galaxy_role_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2125 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginated_galaxy_role_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2381 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginated_tag_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2689 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginatedansible_ansible_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2798 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginatedansible_ansible_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3412 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginatedansible_collection_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginatedansible_collection_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3882 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginatedansible_collection_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3154 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginatedansible_role_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2287 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_paginatedansible_role_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1843 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_patchedansible_ansible_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1901 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_patchedansible_ansible_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2543 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_patchedansible_collection_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_patchedansible_role_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v2_collections_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v3_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v3_collection_versions_all_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v3_collections_all_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v3_collections_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v3_collections_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v3_collections_versions_docs_blob_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1053 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_pulp_ansible_artifacts_collections_v3_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_pulp_ansible_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_remotes_collection_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1567 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_remotes_role_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_repo_metadata_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1878 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_repositories_ansible_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1369 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_repositories_ansible_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1766 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_repository_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1826 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1412 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2399 2021-10-04 19:36:02.000000 pulp_ansible-client-0.9.2/test/test_unpaginated_collection_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)      931 2021-10-04 19:36:03.000000 pulp_ansible-client-0.9.2/test/test_versions_api.py
```

### Comparing `pulp_ansible-client-0.9.1/README.md` & `pulp_ansible-client-0.9.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_ansible-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 0.9.1
+- Package version: 0.9.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_ansible-client-0.9.1/pulp_ansible_client.egg-info/SOURCES.txt` & `pulp_ansible-client-0.9.2/pulp_ansible_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/__init__.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 # import apis into sdk package
 from pulpcore.client.pulp_ansible.api.ansible_collections_api import AnsibleCollectionsApi
 from pulpcore.client.pulp_ansible.api.ansible_copy_api import AnsibleCopyApi
 from pulpcore.client.pulp_ansible.api.api_collections_api import ApiCollectionsApi
 from pulpcore.client.pulp_ansible.api.api_roles_api import ApiRolesApi
 from pulpcore.client.pulp_ansible.api.collection_import_api import CollectionImportApi
```

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/__init__.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/ansible_collections_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/ansible_collections_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/ansible_copy_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/ansible_copy_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/api_collections_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/api_collections_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/api_roles_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/api_roles_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/collection_import_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/collection_import_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/content_collection_versions_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/content_collection_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/content_roles_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/content_roles_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/distributions_ansible_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/distributions_ansible_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/galaxy_detail_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/galaxy_detail_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v2_collections_versions_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v2_collections_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collection_versions_all_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collection_versions_all_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_all_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_all_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_versions_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_versions_docs_blob_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_api_v3_collections_versions_docs_blob_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_artifacts_collections_v3_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_artifacts_collections_v3_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/pulp_ansible_tags_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/pulp_ansible_tags_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/remotes_collection_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/remotes_collection_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/remotes_role_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/remotes_role_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/repositories_ansible_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/repositories_ansible_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/repositories_ansible_versions_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/repositories_ansible_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api/versions_api.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api/versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/api_client.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.9.1/python'
+        self.user_agent = 'OpenAPI-Generator/0.9.2/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/configuration.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 0.9.1".\
+               "SDK Package Version: 0.9.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/exceptions.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/__init__.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_ansible_distribution.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_ansible_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_ansible_distribution_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_ansible_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_ansible_repository.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_ansible_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_ansible_repository_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_ansible_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_collection_remote.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_collection_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_collection_remote_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_collection_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_collection_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_collection_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_collection_version.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_collection_version.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_collection_version_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_collection_version_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'artifact': 'str',
         'pulp_created': 'datetime',
         'pulp_href': 'str',
+        'artifact': 'str',
         'md5': 'str',
         'sha1': 'str',
         'sha224': 'str',
         'sha256': 'str',
         'sha384': 'str',
         'sha512': 'str',
         'id': 'str',
@@ -60,17 +60,17 @@
         'repository': 'str',
         'tags': 'list[AnsibleTagResponse]',
         'version': 'str',
         'requires_ansible': 'str'
     }
 
     attribute_map = {
-        'artifact': 'artifact',
         'pulp_created': 'pulp_created',
         'pulp_href': 'pulp_href',
+        'artifact': 'artifact',
         'md5': 'md5',
         'sha1': 'sha1',
         'sha224': 'sha224',
         'sha256': 'sha256',
         'sha384': 'sha384',
         'sha512': 'sha512',
         'id': 'id',
@@ -89,23 +89,23 @@
         'namespace': 'namespace',
         'repository': 'repository',
         'tags': 'tags',
         'version': 'version',
         'requires_ansible': 'requires_ansible'
     }
 
-    def __init__(self, artifact=None, pulp_created=None, pulp_href=None, md5=None, sha1=None, sha224=None, sha256=None, sha384=None, sha512=None, id=None, authors=None, contents=None, dependencies=None, description=None, docs_blob=None, manifest=None, files=None, documentation=None, homepage=None, issues=None, license=None, name=None, namespace=None, repository=None, tags=None, version=None, requires_ansible=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_created=None, pulp_href=None, artifact=None, md5=None, sha1=None, sha224=None, sha256=None, sha384=None, sha512=None, id=None, authors=None, contents=None, dependencies=None, description=None, docs_blob=None, manifest=None, files=None, documentation=None, homepage=None, issues=None, license=None, name=None, namespace=None, repository=None, tags=None, version=None, requires_ansible=None, local_vars_configuration=None):  # noqa: E501
         """AnsibleCollectionVersionResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._artifact = None
         self._pulp_created = None
         self._pulp_href = None
+        self._artifact = None
         self._md5 = None
         self._sha1 = None
         self._sha224 = None
         self._sha256 = None
         self._sha384 = None
         self._sha512 = None
         self._id = None
@@ -124,19 +124,19 @@
         self._namespace = None
         self._repository = None
         self._tags = None
         self._version = None
         self._requires_ansible = None
         self.discriminator = None
 
-        self.artifact = artifact
         if pulp_created is not None:
             self.pulp_created = pulp_created
         if pulp_href is not None:
             self.pulp_href = pulp_href
+        self.artifact = artifact
         if md5 is not None:
             self.md5 = md5
         if sha1 is not None:
             self.sha1 = sha1
         if sha224 is not None:
             self.sha224 = sha224
         if sha256 is not None:
@@ -162,39 +162,14 @@
         self.repository = repository
         if tags is not None:
             self.tags = tags
         self.version = version
         self.requires_ansible = requires_ansible
 
     @property
-    def artifact(self):
-        """Gets the artifact of this AnsibleCollectionVersionResponse.  # noqa: E501
-
-        Artifact file representing the physical content  # noqa: E501
-
-        :return: The artifact of this AnsibleCollectionVersionResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._artifact
-
-    @artifact.setter
-    def artifact(self, artifact):
-        """Sets the artifact of this AnsibleCollectionVersionResponse.
-
-        Artifact file representing the physical content  # noqa: E501
-
-        :param artifact: The artifact of this AnsibleCollectionVersionResponse.  # noqa: E501
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and artifact is None:  # noqa: E501
-            raise ValueError("Invalid value for `artifact`, must not be `None`")  # noqa: E501
-
-        self._artifact = artifact
-
-    @property
     def pulp_created(self):
         """Gets the pulp_created of this AnsibleCollectionVersionResponse.  # noqa: E501
 
         Timestamp of creation.  # noqa: E501
 
         :return: The pulp_created of this AnsibleCollectionVersionResponse.  # noqa: E501
         :rtype: datetime
@@ -231,14 +206,39 @@
         :param pulp_href: The pulp_href of this AnsibleCollectionVersionResponse.  # noqa: E501
         :type: str
         """
 
         self._pulp_href = pulp_href
 
     @property
+    def artifact(self):
+        """Gets the artifact of this AnsibleCollectionVersionResponse.  # noqa: E501
+
+        Artifact file representing the physical content  # noqa: E501
+
+        :return: The artifact of this AnsibleCollectionVersionResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._artifact
+
+    @artifact.setter
+    def artifact(self, artifact):
+        """Sets the artifact of this AnsibleCollectionVersionResponse.
+
+        Artifact file representing the physical content  # noqa: E501
+
+        :param artifact: The artifact of this AnsibleCollectionVersionResponse.  # noqa: E501
+        :type: str
+        """
+        if self.local_vars_configuration.client_side_validation and artifact is None:  # noqa: E501
+            raise ValueError("Invalid value for `artifact`, must not be `None`")  # noqa: E501
+
+        self._artifact = artifact
+
+    @property
     def md5(self):
         """Gets the md5 of this AnsibleCollectionVersionResponse.  # noqa: E501
 
         The MD5 checksum if available.  # noqa: E501
 
         :return: The md5 of this AnsibleCollectionVersionResponse.  # noqa: E501
         :rtype: str
```

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_repository_sync_url.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_role.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_role.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_role_remote.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_role_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_role_remote_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_role_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_role_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_role_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,80 +30,55 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'artifact': 'str',
         'pulp_created': 'datetime',
         'pulp_href': 'str',
+        'artifact': 'str',
         'version': 'str',
         'name': 'str',
         'namespace': 'str'
     }
 
     attribute_map = {
-        'artifact': 'artifact',
         'pulp_created': 'pulp_created',
         'pulp_href': 'pulp_href',
+        'artifact': 'artifact',
         'version': 'version',
         'name': 'name',
         'namespace': 'namespace'
     }
 
-    def __init__(self, artifact=None, pulp_created=None, pulp_href=None, version=None, name=None, namespace=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_created=None, pulp_href=None, artifact=None, version=None, name=None, namespace=None, local_vars_configuration=None):  # noqa: E501
         """AnsibleRoleResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._artifact = None
         self._pulp_created = None
         self._pulp_href = None
+        self._artifact = None
         self._version = None
         self._name = None
         self._namespace = None
         self.discriminator = None
 
-        self.artifact = artifact
         if pulp_created is not None:
             self.pulp_created = pulp_created
         if pulp_href is not None:
             self.pulp_href = pulp_href
+        self.artifact = artifact
         self.version = version
         self.name = name
         self.namespace = namespace
 
     @property
-    def artifact(self):
-        """Gets the artifact of this AnsibleRoleResponse.  # noqa: E501
-
-        Artifact file representing the physical content  # noqa: E501
-
-        :return: The artifact of this AnsibleRoleResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._artifact
-
-    @artifact.setter
-    def artifact(self, artifact):
-        """Sets the artifact of this AnsibleRoleResponse.
-
-        Artifact file representing the physical content  # noqa: E501
-
-        :param artifact: The artifact of this AnsibleRoleResponse.  # noqa: E501
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and artifact is None:  # noqa: E501
-            raise ValueError("Invalid value for `artifact`, must not be `None`")  # noqa: E501
-
-        self._artifact = artifact
-
-    @property
     def pulp_created(self):
         """Gets the pulp_created of this AnsibleRoleResponse.  # noqa: E501
 
         Timestamp of creation.  # noqa: E501
 
         :return: The pulp_created of this AnsibleRoleResponse.  # noqa: E501
         :rtype: datetime
@@ -140,14 +115,39 @@
         :param pulp_href: The pulp_href of this AnsibleRoleResponse.  # noqa: E501
         :type: str
         """
 
         self._pulp_href = pulp_href
 
     @property
+    def artifact(self):
+        """Gets the artifact of this AnsibleRoleResponse.  # noqa: E501
+
+        Artifact file representing the physical content  # noqa: E501
+
+        :return: The artifact of this AnsibleRoleResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._artifact
+
+    @artifact.setter
+    def artifact(self, artifact):
+        """Sets the artifact of this AnsibleRoleResponse.
+
+        Artifact file representing the physical content  # noqa: E501
+
+        :param artifact: The artifact of this AnsibleRoleResponse.  # noqa: E501
+        :type: str
+        """
+        if self.local_vars_configuration.client_side_validation and artifact is None:  # noqa: E501
+            raise ValueError("Invalid value for `artifact`, must not be `None`")  # noqa: E501
+
+        self._artifact = artifact
+
+    @property
     def version(self):
         """Gets the version of this AnsibleRoleResponse.  # noqa: E501
 
 
         :return: The version of this AnsibleRoleResponse.  # noqa: E501
         :rtype: str
         """
```

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/ansible_tag_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/ansible_tag_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/artifact_ref_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/artifact_ref_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/async_operation_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_import_detail_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_import_detail_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_metadata_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_metadata_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_namespace_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_namespace_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_one_shot.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_one_shot.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_ref_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_ref_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_version_docs_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_version_docs_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/collection_version_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/collection_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/content_summary.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/content_summary.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/content_summary_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/copy.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/copy.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/galaxy_collection.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/galaxy_collection.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/galaxy_collection_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/galaxy_collection_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/galaxy_collection_version_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/galaxy_collection_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/galaxy_role_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/galaxy_role_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/galaxy_role_version_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/galaxy_role_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_collection_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_collection_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_collection_response_list_links.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_collection_response_list_links.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_collection_response_list_meta.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_collection_response_list_meta.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_collection_version_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_collection_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_galaxy_collection_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_galaxy_collection_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_galaxy_collection_version_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_galaxy_collection_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_galaxy_role_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_galaxy_role_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_galaxy_role_version_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_galaxy_role_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_repository_version_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginated_tag_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginated_tag_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_ansible_distribution_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_ansible_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_ansible_repository_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_ansible_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_collection_remote_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_collection_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_collection_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_collection_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_collection_version_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_collection_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_role_remote_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_role_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/paginatedansible_role_response_list.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/paginatedansible_role_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/patchedansible_ansible_distribution.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/patchedansible_ansible_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/patchedansible_ansible_repository.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/patchedansible_ansible_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/patchedansible_collection_remote.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/patchedansible_collection_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/patchedansible_role_remote.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/patchedansible_role_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/policy_enum.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/repo_metadata_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/repo_metadata_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/repository_add_remove_content.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/repository_version.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/repository_version.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/repository_version_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/tag_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/tag_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/models/unpaginated_collection_version_response.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/models/unpaginated_collection_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/pulpcore/client/pulp_ansible/rest.py` & `pulp_ansible-client-0.9.2/pulpcore/client/pulp_ansible/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/setup.py` & `pulp_ansible-client-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_ansible-client"
-VERSION = "0.9.1"
+VERSION = "0.9.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_ansible_distribution.py` & `pulp_ansible-client-0.9.2/test/test_ansible_ansible_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_ansible_distribution_response.py` & `pulp_ansible-client-0.9.2/test/test_ansible_ansible_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_ansible_repository.py` & `pulp_ansible-client-0.9.2/test/test_ansible_ansible_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_ansible_repository_response.py` & `pulp_ansible-client-0.9.2/test/test_ansible_ansible_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_collection_remote.py` & `pulp_ansible-client-0.9.2/test/test_ansible_collection_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_collection_remote_response.py` & `pulp_ansible-client-0.9.2/test/test_ansible_collection_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_collection_response.py` & `pulp_ansible-client-0.9.2/test/test_ansible_collection_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_collection_version.py` & `pulp_ansible-client-0.9.2/test/test_ansible_collection_version.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_collection_version_response.py` & `pulp_ansible-client-0.9.2/test/test_ansible_collection_version_response.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,17 +33,17 @@
         """Test AnsibleCollectionVersionResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = pulpcore.client.pulp_ansible.models.ansible_collection_version_response.AnsibleCollectionVersionResponse()  # noqa: E501
         if include_optional :
             return AnsibleCollectionVersionResponse(
-                artifact = '0', 
                 pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 pulp_href = '0', 
+                artifact = '0', 
                 md5 = '0', 
                 sha1 = '0', 
                 sha224 = '0', 
                 sha256 = '0', 
                 sha384 = '0', 
                 sha512 = '0', 
                 id = '0',
```

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_collections_api.py` & `pulp_ansible-client-0.9.2/test/test_ansible_collections_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_copy_api.py` & `pulp_ansible-client-0.9.2/test/test_ansible_copy_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_repository_sync_url.py` & `pulp_ansible-client-0.9.2/test/test_ansible_repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_role.py` & `pulp_ansible-client-0.9.2/test/test_ansible_role.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_role_remote.py` & `pulp_ansible-client-0.9.2/test/test_ansible_role_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_role_remote_response.py` & `pulp_ansible-client-0.9.2/test/test_ansible_role_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_role_response.py` & `pulp_ansible-client-0.9.2/test/test_ansible_role_response.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,17 +33,17 @@
         """Test AnsibleRoleResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = pulpcore.client.pulp_ansible.models.ansible_role_response.AnsibleRoleResponse()  # noqa: E501
         if include_optional :
             return AnsibleRoleResponse(
-                artifact = '0', 
                 pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 pulp_href = '0', 
+                artifact = '0', 
                 version = '0', 
                 name = '0', 
                 namespace = '0'
             )
         else :
             return AnsibleRoleResponse(
                 artifact = '0',
```

### Comparing `pulp_ansible-client-0.9.1/test/test_ansible_tag_response.py` & `pulp_ansible-client-0.9.2/test/test_ansible_tag_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_api_collections_api.py` & `pulp_ansible-client-0.9.2/test/test_api_collections_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_api_roles_api.py` & `pulp_ansible-client-0.9.2/test/test_api_roles_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_artifact_ref_response.py` & `pulp_ansible-client-0.9.2/test/test_artifact_ref_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_async_operation_response.py` & `pulp_ansible-client-0.9.2/test/test_async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_collection_import_api.py` & `pulp_ansible-client-0.9.2/test/test_collection_import_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_collection_import_detail_response.py` & `pulp_ansible-client-0.9.2/test/test_collection_import_detail_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_collection_metadata_response.py` & `pulp_ansible-client-0.9.2/test/test_collection_metadata_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_collection_namespace_response.py` & `pulp_ansible-client-0.9.2/test/test_collection_namespace_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_collection_one_shot.py` & `pulp_ansible-client-0.9.2/test/test_collection_one_shot.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_collection_ref_response.py` & `pulp_ansible-client-0.9.2/test/test_collection_ref_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_collection_response.py` & `pulp_ansible-client-0.9.2/test/test_collection_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_collection_version_docs_response.py` & `pulp_ansible-client-0.9.2/test/test_collection_version_docs_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_collection_version_response.py` & `pulp_ansible-client-0.9.2/test/test_collection_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_content_collection_versions_api.py` & `pulp_ansible-client-0.9.2/test/test_content_collection_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_content_roles_api.py` & `pulp_ansible-client-0.9.2/test/test_content_roles_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_content_summary.py` & `pulp_ansible-client-0.9.2/test/test_content_summary.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_content_summary_response.py` & `pulp_ansible-client-0.9.2/test/test_content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_copy.py` & `pulp_ansible-client-0.9.2/test/test_copy.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_distributions_ansible_api.py` & `pulp_ansible-client-0.9.2/test/test_distributions_ansible_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_galaxy_collection.py` & `pulp_ansible-client-0.9.2/test/test_galaxy_collection.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_galaxy_collection_response.py` & `pulp_ansible-client-0.9.2/test/test_galaxy_collection_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_galaxy_collection_version_response.py` & `pulp_ansible-client-0.9.2/test/test_galaxy_collection_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_galaxy_detail_api.py` & `pulp_ansible-client-0.9.2/test/test_galaxy_detail_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_galaxy_role_response.py` & `pulp_ansible-client-0.9.2/test/test_galaxy_role_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_galaxy_role_version_response.py` & `pulp_ansible-client-0.9.2/test/test_galaxy_role_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginated_collection_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginated_collection_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginated_collection_response_list_links.py` & `pulp_ansible-client-0.9.2/test/test_paginated_collection_response_list_links.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginated_collection_response_list_meta.py` & `pulp_ansible-client-0.9.2/test/test_paginated_collection_response_list_meta.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginated_collection_version_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginated_collection_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginated_galaxy_collection_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginated_galaxy_collection_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginated_galaxy_collection_version_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginated_galaxy_collection_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginated_galaxy_role_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginated_galaxy_role_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginated_galaxy_role_version_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginated_galaxy_role_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginated_repository_version_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginated_tag_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginated_tag_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginatedansible_ansible_distribution_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginatedansible_ansible_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginatedansible_ansible_repository_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginatedansible_ansible_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginatedansible_collection_remote_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginatedansible_collection_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginatedansible_collection_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginatedansible_collection_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginatedansible_collection_version_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginatedansible_collection_version_response_list.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,17 @@
         if include_optional :
             return PaginatedansibleCollectionVersionResponseList(
                 count = 123, 
                 next = 'http://api.example.org/accounts/?offset=400&limit=100', 
                 previous = 'http://api.example.org/accounts/?offset=200&limit=100', 
                 results = [
                     pulpcore.client.pulp_ansible.models.ansible/collection_version_response.ansible.CollectionVersionResponse(
-                        artifact = '0', 
                         pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         pulp_href = '0', 
+                        artifact = '0', 
                         md5 = '0', 
                         sha1 = '0', 
                         sha224 = '0', 
                         sha256 = '0', 
                         sha384 = '0', 
                         sha512 = '0', 
                         id = '0',
```

### Comparing `pulp_ansible-client-0.9.1/test/test_paginatedansible_role_remote_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginatedansible_role_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_paginatedansible_role_response_list.py` & `pulp_ansible-client-0.9.2/test/test_paginatedansible_role_response_list.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,17 @@
         if include_optional :
             return PaginatedansibleRoleResponseList(
                 count = 123, 
                 next = 'http://api.example.org/accounts/?offset=400&limit=100', 
                 previous = 'http://api.example.org/accounts/?offset=200&limit=100', 
                 results = [
                     pulpcore.client.pulp_ansible.models.ansible/role_response.ansible.RoleResponse(
-                        artifact = '0', 
                         pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         pulp_href = '0', 
+                        artifact = '0', 
                         version = '0', 
                         name = '0', 
                         namespace = '0', )
                     ]
             )
         else :
             return PaginatedansibleRoleResponseList(
```

### Comparing `pulp_ansible-client-0.9.1/test/test_patchedansible_ansible_distribution.py` & `pulp_ansible-client-0.9.2/test/test_patchedansible_ansible_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_patchedansible_ansible_repository.py` & `pulp_ansible-client-0.9.2/test/test_patchedansible_ansible_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_patchedansible_collection_remote.py` & `pulp_ansible-client-0.9.2/test/test_patchedansible_collection_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_patchedansible_role_remote.py` & `pulp_ansible-client-0.9.2/test/test_patchedansible_role_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_policy_enum.py` & `pulp_ansible-client-0.9.2/test/test_policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_api.py` & `pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v2_collections_versions_api.py` & `pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v2_collections_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v3_api.py` & `pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v3_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v3_collection_versions_all_api.py` & `pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v3_collection_versions_all_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v3_collections_all_api.py` & `pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v3_collections_all_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v3_collections_api.py` & `pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v3_collections_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v3_collections_versions_api.py` & `pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v3_collections_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_pulp_ansible_api_v3_collections_versions_docs_blob_api.py` & `pulp_ansible-client-0.9.2/test/test_pulp_ansible_api_v3_collections_versions_docs_blob_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_pulp_ansible_artifacts_collections_v3_api.py` & `pulp_ansible-client-0.9.2/test/test_pulp_ansible_artifacts_collections_v3_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_pulp_ansible_tags_api.py` & `pulp_ansible-client-0.9.2/test/test_pulp_ansible_tags_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_remotes_collection_api.py` & `pulp_ansible-client-0.9.2/test/test_remotes_collection_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_remotes_role_api.py` & `pulp_ansible-client-0.9.2/test/test_remotes_role_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_repo_metadata_response.py` & `pulp_ansible-client-0.9.2/test/test_repo_metadata_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_repositories_ansible_api.py` & `pulp_ansible-client-0.9.2/test/test_repositories_ansible_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_repositories_ansible_versions_api.py` & `pulp_ansible-client-0.9.2/test/test_repositories_ansible_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_repository_add_remove_content.py` & `pulp_ansible-client-0.9.2/test/test_repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_repository_version.py` & `pulp_ansible-client-0.9.2/test/test_repository_version.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_repository_version_response.py` & `pulp_ansible-client-0.9.2/test/test_repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_tag_response.py` & `pulp_ansible-client-0.9.2/test/test_tag_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_unpaginated_collection_version_response.py` & `pulp_ansible-client-0.9.2/test/test_unpaginated_collection_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ansible-client-0.9.1/test/test_versions_api.py` & `pulp_ansible-client-0.9.2/test/test_versions_api.py`

 * *Files identical despite different names*

