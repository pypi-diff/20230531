# Comparing `tmp/iparapheur-provisioning-1.6.3.tar.gz` & `tmp/iparapheur-provisioning-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iparapheur-provisioning-1.6.3.tar", last modified: Thu May 25 16:17:12 2023, max compression
+gzip compressed data, was "iparapheur-provisioning-1.6.4.tar", last modified: Wed May 31 08:19:28 2023, max compression
```

## Comparing `iparapheur-provisioning-1.6.3.tar` & `iparapheur-provisioning-1.6.4.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.326281 iparapheur-provisioning-1.6.3/
--rw-r--r--   0 root         (0) root         (0)     1111 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      421 2023-05-25 16:17:12.326281 iparapheur-provisioning-1.6.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17390 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.254279 iparapheur-provisioning-1.6.3/iparapheur_provisioning/
--rw-r--r--   0 root         (0) root         (0)      907 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58620 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.258280 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4776 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.266280 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-05-25 16:15:34.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 16:15:34.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-25 16:15:29.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-05-25 16:15:29.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)     1089 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.270280 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-05-25 16:15:29.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tags/admin_all_users_api.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tags/admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-05-25 16:15:34.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tags/admin_tenant_api.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tags/admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)    15677 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.298281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-05-25 16:15:11.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    30320 2023-05-25 16:15:13.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/desk_dto.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-05-25 16:15:15.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-05-25 16:15:15.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/error_response.py
--rw-r--r--   0 root         (0) root         (0)     4891 2023-05-25 16:15:15.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     2680 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3284 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-05-25 16:15:17.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-25 16:15:17.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-05-25 16:15:17.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-05-25 16:15:17.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     9132 2023-05-25 16:15:18.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-05-25 16:15:18.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-05-25 16:15:18.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)     5251 2023-05-25 16:15:19.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-05-25 16:15:19.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-25 16:15:19.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-05-25 16:15:19.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/signature_format.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-05-25 16:15:19.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-05-25 16:15:19.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/sort_object.py
--rw-r--r--   0 root         (0) root         (0)    28616 2023-05-25 16:15:20.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-05-25 16:15:22.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-05-25 16:15:22.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-05-25 16:15:22.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-05-25 16:15:23.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     3274 2023-05-25 16:15:23.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-05-25 16:15:23.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-25 16:15:23.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     9365 2023-05-25 16:15:23.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/type_dto.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-05-25 16:15:24.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/type_representation.py
--rw-r--r--   0 root         (0) root         (0)     4436 2023-05-25 16:15:24.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/typology_representation.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-05-25 16:15:24.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    29666 2023-05-25 16:15:25.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/user_dto.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-05-25 16:15:26.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-05-25 16:15:26.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/user_representation.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-05-25 16:15:26.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-05-25 16:15:26.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.298281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/models/
--rw-r--r--   0 root         (0) root         (0)     3734 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.298281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.298281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-25 16:15:34.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13629 2023-05-25 16:15:32.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.302281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)      389 2023-05-25 16:15:34.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11083 2023-05-25 16:15:32.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11332 2023-05-25 16:15:32.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15808 2023-05-25 16:15:32.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.302281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15034 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
--rw-r--r--   0 root         (0) root         (0)    16302 2023-05-25 16:15:29.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.302281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-05-25 16:15:30.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11677 2023-05-25 16:15:30.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16545 2023-05-25 16:15:30.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.302281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14728 2023-05-25 16:15:39.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
--rw-r--r--   0 root         (0) root         (0)    15777 2023-05-25 16:15:38.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.302281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-05-25 16:15:38.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11590 2023-05-25 16:15:39.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15521 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.306281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)      449 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15050 2023-05-25 16:15:39.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.306281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)      471 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11672 2023-05-25 16:15:38.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11934 2023-05-25 16:15:38.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16645 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.306281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15944 2023-05-25 16:15:36.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
--rw-r--r--   0 root         (0) root         (0)    15781 2023-05-25 16:15:35.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.306281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-05-25 16:15:36.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11580 2023-05-25 16:15:35.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16046 2023-05-25 16:15:36.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.306281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-25 16:15:29.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13222 2023-05-25 16:15:28.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.306281 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-25 16:15:29.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11207 2023-05-25 16:15:27.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11978 2023-05-25 16:15:28.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15946 2023-05-25 16:15:28.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
--rw-r--r--   0 root         (0) root         (0)    10635 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/rest.py
--rw-r--r--   0 root         (0) root         (0)    97752 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.258280 iparapheur-provisioning-1.6.3/iparapheur_provisioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      421 2023-05-25 16:17:12.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13603 2023-05-25 16:17:12.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 16:17:12.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-25 16:17:12.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 16:17:12.000000 iparapheur-provisioning-1.6.3/iparapheur_provisioning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-25 16:17:12.326281 iparapheur-provisioning-1.6.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1322 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.246279 iparapheur-provisioning-1.6.3/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.318281 iparapheur-provisioning-1.6.3/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:41.000000 iparapheur-provisioning-1.6.3/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-05-25 16:15:11.000000 iparapheur-provisioning-1.6.3/test/test_models/test_delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-05-25 16:15:14.000000 iparapheur-provisioning-1.6.3/test/test_models/test_desk_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-25 16:15:15.000000 iparapheur-provisioning-1.6.3/test/test_models/test_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-25 16:15:15.000000 iparapheur-provisioning-1.6.3/test/test_models/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)      767 2023-05-25 16:15:15.000000 iparapheur-provisioning-1.6.3/test/test_models/test_external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/test/test_models/test_external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/test/test_models/test_external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/test/test_models/test_folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/test/test_models/test_internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/test/test_models/test_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/test/test_models/test_layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      661 2023-05-25 16:15:16.000000 iparapheur-provisioning-1.6.3/test/test_models/test_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-05-25 16:15:17.000000 iparapheur-provisioning-1.6.3/test/test_models/test_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-25 16:15:17.000000 iparapheur-provisioning-1.6.3/test/test_models/test_metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-05-25 16:15:17.000000 iparapheur-provisioning-1.6.3/test/test_models/test_metadata_type.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-05-25 16:15:17.000000 iparapheur-provisioning-1.6.3/test/test_models/test_page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-05-25 16:15:18.000000 iparapheur-provisioning-1.6.3/test/test_models/test_page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-05-25 16:15:18.000000 iparapheur-provisioning-1.6.3/test/test_models/test_page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-05-25 16:15:18.000000 iparapheur-provisioning-1.6.3/test/test_models/test_page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-05-25 16:15:19.000000 iparapheur-provisioning-1.6.3/test/test_models/test_pageable_object.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-25 16:15:19.000000 iparapheur-provisioning-1.6.3/test/test_models/test_pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-25 16:15:19.000000 iparapheur-provisioning-1.6.3/test/test_models/test_seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-05-25 16:15:19.000000 iparapheur-provisioning-1.6.3/test/test_models/test_signature_format.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-05-25 16:15:19.000000 iparapheur-provisioning-1.6.3/test/test_models/test_signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-25 16:15:19.000000 iparapheur-provisioning-1.6.3/test/test_models/test_sort_object.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-25 16:15:22.000000 iparapheur-provisioning-1.6.3/test/test_models/test_subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-05-25 16:15:22.000000 iparapheur-provisioning-1.6.3/test/test_models/test_subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-25 16:15:22.000000 iparapheur-provisioning-1.6.3/test/test_models/test_subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-25 16:15:23.000000 iparapheur-provisioning-1.6.3/test/test_models/test_subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-05-25 16:15:23.000000 iparapheur-provisioning-1.6.3/test/test_models/test_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      653 2023-05-25 16:15:23.000000 iparapheur-provisioning-1.6.3/test/test_models/test_tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-05-25 16:15:23.000000 iparapheur-provisioning-1.6.3/test/test_models/test_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-05-25 16:15:23.000000 iparapheur-provisioning-1.6.3/test/test_models/test_tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-05-25 16:15:24.000000 iparapheur-provisioning-1.6.3/test/test_models/test_type_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-25 16:15:24.000000 iparapheur-provisioning-1.6.3/test/test_models/test_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-05-25 16:15:24.000000 iparapheur-provisioning-1.6.3/test/test_models/test_typology_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-25 16:15:24.000000 iparapheur-provisioning-1.6.3/test/test_models/test_typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-05-25 16:15:25.000000 iparapheur-provisioning-1.6.3/test/test_models/test_user_dto.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-25 16:15:26.000000 iparapheur-provisioning-1.6.3/test/test_models/test_user_privilege.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-25 16:15:26.000000 iparapheur-provisioning-1.6.3/test/test_models/test_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-25 16:15:26.000000 iparapheur-provisioning-1.6.3/test/test_models/test_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-05-25 16:15:26.000000 iparapheur-provisioning-1.6.3/test/test_models/test_workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.318281 iparapheur-provisioning-1.6.3/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.318281 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:34.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-05-25 16:15:34.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.318281 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:34.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-05-25 16:15:34.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-05-25 16:15:34.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-05-25 16:15:34.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.318281 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.322281 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-05-25 16:15:31.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.322281 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.322281 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.322281 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.322281 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-05-25 16:15:40.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.326281 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.326281 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-05-25 16:15:37.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.326281 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:29.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-05-25 16:15:29.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:17:12.326281 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 16:15:29.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-05-25 16:15:29.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-05-25 16:15:29.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-05-25 16:15:29.000000 iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.344199 iparapheur-provisioning-1.6.4/
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      421 2023-05-31 08:19:28.344199 iparapheur-provisioning-1.6.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17390 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.304199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/
+-rw-r--r--   0 root         (0) root         (0)      907 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58620 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.304199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4776 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.308199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-31 08:16:53.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-31 08:16:53.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-05-31 08:16:51.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-05-31 08:16:51.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.308199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tags/
+-rw-r--r--   0 root         (0) root         (0)      475 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tags/admin_all_users_api.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-05-31 08:16:51.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tags/admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-05-31 08:16:54.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tags/admin_tenant_api.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tags/admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)    15677 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.312199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-05-31 08:16:33.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    30320 2023-05-31 08:16:34.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-05-31 08:16:35.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     4891 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     7233 2023-05-31 08:16:37.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-05-31 08:16:37.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-31 08:16:38.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-05-31 08:16:38.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-05-31 08:16:38.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-05-31 08:16:38.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-05-31 08:16:39.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-05-31 08:16:39.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-05-31 08:16:39.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-05-31 08:16:39.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-31 08:16:40.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-05-31 08:16:40.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-05-31 08:16:40.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-05-31 08:16:40.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/sort_object.py
+-rw-r--r--   0 root         (0) root         (0)    28616 2023-05-31 08:16:40.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-05-31 08:16:41.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-05-31 08:16:41.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-05-31 08:16:41.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-05-31 08:16:42.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-05-31 08:16:42.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-05-31 08:16:42.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-31 08:16:42.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     9365 2023-05-31 08:16:42.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-05-31 08:16:42.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4436 2023-05-31 08:16:43.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-05-31 08:16:43.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    29666 2023-05-31 08:16:43.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-05-31 08:16:44.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-05-31 08:16:45.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-05-31 08:16:45.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-05-31 08:16:45.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.312199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/models/
+-rw-r--r--   0 root         (0) root         (0)     3734 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.312199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.316199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-31 08:16:53.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13629 2023-05-31 08:16:52.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.316199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-31 08:16:53.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11083 2023-05-31 08:16:52.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11332 2023-05-31 08:16:53.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15808 2023-05-31 08:16:53.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.316199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 08:16:51.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15034 2023-05-31 08:16:50.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
+-rw-r--r--   0 root         (0) root         (0)    16302 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.316199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-31 08:16:51.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11677 2023-05-31 08:16:49.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16545 2023-05-31 08:16:49.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.316199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14728 2023-05-31 08:17:01.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
+-rw-r--r--   0 root         (0) root         (0)    15777 2023-05-31 08:16:59.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.324199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-05-31 08:17:00.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2023-05-31 08:17:01.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.324199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)      449 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15050 2023-05-31 08:17:01.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-05-31 08:16:58.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.324199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11672 2023-05-31 08:16:59.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11934 2023-05-31 08:17:00.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16645 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.324199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15944 2023-05-31 08:16:55.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
+-rw-r--r--   0 root         (0) root         (0)    15781 2023-05-31 08:16:54.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.328199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-05-31 08:16:56.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2023-05-31 08:16:55.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16046 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.328199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-05-31 08:16:46.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.328199 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11207 2023-05-31 08:16:46.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11978 2023-05-31 08:16:46.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-05-31 08:16:47.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
+-rw-r--r--   0 root         (0) root         (0)    10635 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/rest.py
+-rw-r--r--   0 root         (0) root         (0)    97752 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.304199 iparapheur-provisioning-1.6.4/iparapheur_provisioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-05-31 08:19:28.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13603 2023-05-31 08:19:28.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 08:19:28.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-31 08:19:28.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-31 08:19:28.000000 iparapheur-provisioning-1.6.4/iparapheur_provisioning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-31 08:19:28.344199 iparapheur-provisioning-1.6.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.300198 iparapheur-provisioning-1.6.4/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.336199 iparapheur-provisioning-1.6.4/test/test_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/test/test_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-05-31 08:16:33.000000 iparapheur-provisioning-1.6.4/test/test_models/test_delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-05-31 08:16:35.000000 iparapheur-provisioning-1.6.4/test/test_models/test_desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-31 08:16:35.000000 iparapheur-provisioning-1.6.4/test/test_models/test_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/test/test_models/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/test/test_models/test_external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/test/test_models/test_external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/test/test_models/test_external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/test/test_models/test_folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/test/test_models/test_internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/test/test_models/test_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-05-31 08:16:36.000000 iparapheur-provisioning-1.6.4/test/test_models/test_layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-31 08:16:37.000000 iparapheur-provisioning-1.6.4/test/test_models/test_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-05-31 08:16:37.000000 iparapheur-provisioning-1.6.4/test/test_models/test_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-31 08:16:38.000000 iparapheur-provisioning-1.6.4/test/test_models/test_metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-05-31 08:16:38.000000 iparapheur-provisioning-1.6.4/test/test_models/test_metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-05-31 08:16:38.000000 iparapheur-provisioning-1.6.4/test/test_models/test_page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-05-31 08:16:38.000000 iparapheur-provisioning-1.6.4/test/test_models/test_page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-05-31 08:16:39.000000 iparapheur-provisioning-1.6.4/test/test_models/test_page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-05-31 08:16:39.000000 iparapheur-provisioning-1.6.4/test/test_models/test_page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-05-31 08:16:39.000000 iparapheur-provisioning-1.6.4/test/test_models/test_pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-05-31 08:16:39.000000 iparapheur-provisioning-1.6.4/test/test_models/test_pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-31 08:16:40.000000 iparapheur-provisioning-1.6.4/test/test_models/test_seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-05-31 08:16:40.000000 iparapheur-provisioning-1.6.4/test/test_models/test_signature_format.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-05-31 08:16:40.000000 iparapheur-provisioning-1.6.4/test/test_models/test_signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-31 08:16:40.000000 iparapheur-provisioning-1.6.4/test/test_models/test_sort_object.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-31 08:16:41.000000 iparapheur-provisioning-1.6.4/test/test_models/test_subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-05-31 08:16:41.000000 iparapheur-provisioning-1.6.4/test/test_models/test_subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-31 08:16:41.000000 iparapheur-provisioning-1.6.4/test/test_models/test_subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-31 08:16:41.000000 iparapheur-provisioning-1.6.4/test/test_models/test_subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-05-31 08:16:42.000000 iparapheur-provisioning-1.6.4/test/test_models/test_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      653 2023-05-31 08:16:42.000000 iparapheur-provisioning-1.6.4/test/test_models/test_tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)      697 2023-05-31 08:16:42.000000 iparapheur-provisioning-1.6.4/test/test_models/test_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-05-31 08:16:42.000000 iparapheur-provisioning-1.6.4/test/test_models/test_tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-05-31 08:16:42.000000 iparapheur-provisioning-1.6.4/test/test_models/test_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-31 08:16:43.000000 iparapheur-provisioning-1.6.4/test/test_models/test_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-05-31 08:16:43.000000 iparapheur-provisioning-1.6.4/test/test_models/test_typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-31 08:16:43.000000 iparapheur-provisioning-1.6.4/test/test_models/test_typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-05-31 08:16:44.000000 iparapheur-provisioning-1.6.4/test/test_models/test_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-31 08:16:45.000000 iparapheur-provisioning-1.6.4/test/test_models/test_user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-31 08:16:45.000000 iparapheur-provisioning-1.6.4/test/test_models/test_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-31 08:16:45.000000 iparapheur-provisioning-1.6.4/test/test_models/test_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-05-31 08:16:45.000000 iparapheur-provisioning-1.6.4/test/test_models/test_workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.336199 iparapheur-provisioning-1.6.4/test/test_paths/
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.336199 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:16:53.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-05-31 08:16:53.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.336199 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:16:53.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-05-31 08:16:53.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-05-31 08:16:53.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-05-31 08:16:53.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.336199 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:16:51.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      924 2023-05-31 08:16:51.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-05-31 08:16:51.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.336199 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:16:51.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-31 08:16:51.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-31 08:16:51.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-05-31 08:16:51.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.336199 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.340199 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.340199 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.340199 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-05-31 08:17:02.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-05-31 08:17:03.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.340199 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.340199 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-05-31 08:16:57.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.340199 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 08:19:28.344199 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-05-31 08:16:48.000000 iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
```

### Comparing `iparapheur-provisioning-1.6.3/LICENSE.md` & `iparapheur-provisioning-1.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/README.md` & `iparapheur-provisioning-1.6.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The main link between every sub-services, integrating business code logic.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: DEVELOP
-- Package version: 1.6.3
+- Package version: 1.6.4
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://libriciel.fr](https://libriciel.fr)
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
```

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/__init__.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
     The version of the OpenAPI document: DEVELOP
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.6.3"
+__version__ = "1.6.4"
 
 # import ApiClient
 from iparapheur_provisioning.api_client import ApiClient
 
 # import Configuration
 from iparapheur_provisioning.configuration import Configuration
```

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/api_client.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.6.3/python'
+        self.user_agent = 'OpenAPI-Generator/1.6.4/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/path_to_api.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tag_to_api.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tags/admin_all_users_api.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tags/admin_all_users_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tags/admin_desk_api.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tags/admin_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tags/admin_tenant_api.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tags/admin_tenant_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/apis/tags/admin_typology_api.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/apis/tags/admin_typology_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/configuration.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: DEVELOP\n"\
-               "SDK Package Version: 1.6.3".\
+               "SDK Package Version: 1.6.4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/exceptions.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/exceptions.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/delegation_sort_by.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/desk_dto.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/desk_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/error_response.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/external_signature_config_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/external_signature_config_sort_by.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/external_signature_provider.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/folder_sort_by.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/internal_metadata.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/layer_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/layer_sort_by.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/metadata_dto.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/metadata_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/metadata_sort_by.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/metadata_type.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/page_desk_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/page_desk_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,33 +67,33 @@
                 def __getitem__(self, i: int) -> 'DeskRepresentation':
                     return super().__getitem__(i)
             number = schemas.Int32Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
-            first = schemas.BoolSchema
-            last = schemas.BoolSchema
             numberOfElements = schemas.Int32Schema
         
             @staticmethod
             def pageable() -> typing.Type['PageableObject']:
                 return PageableObject
+            first = schemas.BoolSchema
+            last = schemas.BoolSchema
             empty = schemas.BoolSchema
             __annotations__ = {
                 "totalElements": totalElements,
                 "totalPages": totalPages,
                 "size": size,
                 "content": content,
                 "number": number,
                 "sort": sort,
-                "first": first,
-                "last": last,
                 "numberOfElements": numberOfElements,
                 "pageable": pageable,
+                "first": first,
+                "last": last,
                 "empty": empty,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["totalElements"]) -> MetaOapg.properties.totalElements: ...
     
     @typing.overload
@@ -108,32 +108,32 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["number"]) -> MetaOapg.properties.number: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sort"]) -> 'SortObject': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
+    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
+    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
+    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
+    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["totalElements"]) -> typing.Union[MetaOapg.properties.totalElements, schemas.Unset]: ...
     
@@ -149,65 +149,65 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["number"]) -> typing.Union[MetaOapg.properties.number, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sort"]) -> typing.Union['SortObject', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         totalElements: typing.Union[MetaOapg.properties.totalElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         totalPages: typing.Union[MetaOapg.properties.totalPages, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         content: typing.Union[MetaOapg.properties.content, list, tuple, schemas.Unset] = schemas.unset,
         number: typing.Union[MetaOapg.properties.number, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         sort: typing.Union['SortObject', schemas.Unset] = schemas.unset,
-        first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
-        last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
         numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
+        first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
+        last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PageDeskRepresentation':
         return super().__new__(
             cls,
             *_args,
             totalElements=totalElements,
             totalPages=totalPages,
             size=size,
             content=content,
             number=number,
             sort=sort,
-            first=first,
-            last=last,
             numberOfElements=numberOfElements,
             pageable=pageable,
+            first=first,
+            last=last,
             empty=empty,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.desk_representation import DeskRepresentation
 from iparapheur_provisioning.model.pageable_object import PageableObject
```

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/page_subtype_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/page_subtype_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,33 +67,33 @@
                 def __getitem__(self, i: int) -> 'SubtypeRepresentation':
                     return super().__getitem__(i)
             number = schemas.Int32Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
-            first = schemas.BoolSchema
-            last = schemas.BoolSchema
             numberOfElements = schemas.Int32Schema
         
             @staticmethod
             def pageable() -> typing.Type['PageableObject']:
                 return PageableObject
+            first = schemas.BoolSchema
+            last = schemas.BoolSchema
             empty = schemas.BoolSchema
             __annotations__ = {
                 "totalElements": totalElements,
                 "totalPages": totalPages,
                 "size": size,
                 "content": content,
                 "number": number,
                 "sort": sort,
-                "first": first,
-                "last": last,
                 "numberOfElements": numberOfElements,
                 "pageable": pageable,
+                "first": first,
+                "last": last,
                 "empty": empty,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["totalElements"]) -> MetaOapg.properties.totalElements: ...
     
     @typing.overload
@@ -108,32 +108,32 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["number"]) -> MetaOapg.properties.number: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sort"]) -> 'SortObject': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
+    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
+    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
+    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
+    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["totalElements"]) -> typing.Union[MetaOapg.properties.totalElements, schemas.Unset]: ...
     
@@ -149,65 +149,65 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["number"]) -> typing.Union[MetaOapg.properties.number, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sort"]) -> typing.Union['SortObject', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         totalElements: typing.Union[MetaOapg.properties.totalElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         totalPages: typing.Union[MetaOapg.properties.totalPages, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         content: typing.Union[MetaOapg.properties.content, list, tuple, schemas.Unset] = schemas.unset,
         number: typing.Union[MetaOapg.properties.number, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         sort: typing.Union['SortObject', schemas.Unset] = schemas.unset,
-        first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
-        last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
         numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
+        first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
+        last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PageSubtypeRepresentation':
         return super().__new__(
             cls,
             *_args,
             totalElements=totalElements,
             totalPages=totalPages,
             size=size,
             content=content,
             number=number,
             sort=sort,
-            first=first,
-            last=last,
             numberOfElements=numberOfElements,
             pageable=pageable,
+            first=first,
+            last=last,
             empty=empty,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.pageable_object import PageableObject
 from iparapheur_provisioning.model.sort_object import SortObject
```

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/page_type_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/page_type_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,33 +67,33 @@
                 def __getitem__(self, i: int) -> 'TypeRepresentation':
                     return super().__getitem__(i)
             number = schemas.Int32Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
-            first = schemas.BoolSchema
-            last = schemas.BoolSchema
             numberOfElements = schemas.Int32Schema
         
             @staticmethod
             def pageable() -> typing.Type['PageableObject']:
                 return PageableObject
+            first = schemas.BoolSchema
+            last = schemas.BoolSchema
             empty = schemas.BoolSchema
             __annotations__ = {
                 "totalElements": totalElements,
                 "totalPages": totalPages,
                 "size": size,
                 "content": content,
                 "number": number,
                 "sort": sort,
-                "first": first,
-                "last": last,
                 "numberOfElements": numberOfElements,
                 "pageable": pageable,
+                "first": first,
+                "last": last,
                 "empty": empty,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["totalElements"]) -> MetaOapg.properties.totalElements: ...
     
     @typing.overload
@@ -108,32 +108,32 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["number"]) -> MetaOapg.properties.number: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sort"]) -> 'SortObject': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
+    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
+    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
+    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
+    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["totalElements"]) -> typing.Union[MetaOapg.properties.totalElements, schemas.Unset]: ...
     
@@ -149,65 +149,65 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["number"]) -> typing.Union[MetaOapg.properties.number, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sort"]) -> typing.Union['SortObject', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         totalElements: typing.Union[MetaOapg.properties.totalElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         totalPages: typing.Union[MetaOapg.properties.totalPages, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         content: typing.Union[MetaOapg.properties.content, list, tuple, schemas.Unset] = schemas.unset,
         number: typing.Union[MetaOapg.properties.number, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         sort: typing.Union['SortObject', schemas.Unset] = schemas.unset,
-        first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
-        last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
         numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
+        first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
+        last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PageTypeRepresentation':
         return super().__new__(
             cls,
             *_args,
             totalElements=totalElements,
             totalPages=totalPages,
             size=size,
             content=content,
             number=number,
             sort=sort,
-            first=first,
-            last=last,
             numberOfElements=numberOfElements,
             pageable=pageable,
+            first=first,
+            last=last,
             empty=empty,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.pageable_object import PageableObject
 from iparapheur_provisioning.model.sort_object import SortObject
```

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/page_user_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/page_user_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,33 +67,33 @@
                 def __getitem__(self, i: int) -> 'UserRepresentation':
                     return super().__getitem__(i)
             number = schemas.Int32Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
-            first = schemas.BoolSchema
-            last = schemas.BoolSchema
             numberOfElements = schemas.Int32Schema
         
             @staticmethod
             def pageable() -> typing.Type['PageableObject']:
                 return PageableObject
+            first = schemas.BoolSchema
+            last = schemas.BoolSchema
             empty = schemas.BoolSchema
             __annotations__ = {
                 "totalElements": totalElements,
                 "totalPages": totalPages,
                 "size": size,
                 "content": content,
                 "number": number,
                 "sort": sort,
-                "first": first,
-                "last": last,
                 "numberOfElements": numberOfElements,
                 "pageable": pageable,
+                "first": first,
+                "last": last,
                 "empty": empty,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["totalElements"]) -> MetaOapg.properties.totalElements: ...
     
     @typing.overload
@@ -108,32 +108,32 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["number"]) -> MetaOapg.properties.number: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sort"]) -> 'SortObject': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
+    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
+    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
+    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
+    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["totalElements"]) -> typing.Union[MetaOapg.properties.totalElements, schemas.Unset]: ...
     
@@ -149,65 +149,65 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["number"]) -> typing.Union[MetaOapg.properties.number, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sort"]) -> typing.Union['SortObject', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         totalElements: typing.Union[MetaOapg.properties.totalElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         totalPages: typing.Union[MetaOapg.properties.totalPages, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         content: typing.Union[MetaOapg.properties.content, list, tuple, schemas.Unset] = schemas.unset,
         number: typing.Union[MetaOapg.properties.number, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         sort: typing.Union['SortObject', schemas.Unset] = schemas.unset,
-        first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
-        last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
         numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
+        first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
+        last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PageUserRepresentation':
         return super().__new__(
             cls,
             *_args,
             totalElements=totalElements,
             totalPages=totalPages,
             size=size,
             content=content,
             number=number,
             sort=sort,
-            first=first,
-            last=last,
             numberOfElements=numberOfElements,
             pageable=pageable,
+            first=first,
+            last=last,
             empty=empty,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.pageable_object import PageableObject
 from iparapheur_provisioning.model.sort_object import SortObject
```

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/pageable_object.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/pdf_signature_position.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/seal_certificate_sort_by.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/signature_format.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/signature_protocol.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/sort_object.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/sort_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,66 +34,66 @@
     """
 
 
     class MetaOapg:
         
         class properties:
             empty = schemas.BoolSchema
-            sorted = schemas.BoolSchema
             unsorted = schemas.BoolSchema
+            sorted = schemas.BoolSchema
             __annotations__ = {
                 "empty": empty,
-                "sorted": sorted,
                 "unsorted": unsorted,
+                "sorted": sorted,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["sorted"]) -> MetaOapg.properties.sorted: ...
+    def __getitem__(self, name: typing_extensions.Literal["unsorted"]) -> MetaOapg.properties.unsorted: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["unsorted"]) -> MetaOapg.properties.unsorted: ...
+    def __getitem__(self, name: typing_extensions.Literal["sorted"]) -> MetaOapg.properties.sorted: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["empty", "sorted", "unsorted", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["empty", "unsorted", "sorted", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["sorted"]) -> typing.Union[MetaOapg.properties.sorted, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["unsorted"]) -> typing.Union[MetaOapg.properties.unsorted, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["unsorted"]) -> typing.Union[MetaOapg.properties.unsorted, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["sorted"]) -> typing.Union[MetaOapg.properties.sorted, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["empty", "sorted", "unsorted", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["empty", "unsorted", "sorted", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
-        sorted: typing.Union[MetaOapg.properties.sorted, bool, schemas.Unset] = schemas.unset,
         unsorted: typing.Union[MetaOapg.properties.unsorted, bool, schemas.Unset] = schemas.unset,
+        sorted: typing.Union[MetaOapg.properties.sorted, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'SortObject':
         return super().__new__(
             cls,
             *_args,
             empty=empty,
-            sorted=sorted,
             unsorted=unsorted,
+            sorted=sorted,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/subtype_dto.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/subtype_layer_association.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/subtype_layer_dto.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/subtype_metadata_dto.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/subtype_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/tenant_dto.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/tenant_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/tenant_sort_by.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/type_dto.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/type_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/typology_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/typology_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/typology_sort_by.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/user_dto.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/user_privilege.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/user_representation.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/user_sort_by.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/model/workflow_definition_sort_by.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/model/workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/models/__init__.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/models/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/__init__.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/rest.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/rest.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning/schemas.py` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning/schemas.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/iparapheur_provisioning.egg-info/SOURCES.txt` & `iparapheur-provisioning-1.6.4/iparapheur_provisioning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/setup.py` & `iparapheur-provisioning-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "iparapheur-provisioning"
-VERSION = "1.6.3"
+VERSION = "1.6.4"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_delegation_sort_by.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_desk_dto.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_desk_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_error_response.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_external_signature_config_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_external_signature_config_sort_by.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_external_signature_provider.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_folder_sort_by.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_internal_metadata.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_layer_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_layer_sort_by.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_metadata_dto.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_metadata_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_metadata_sort_by.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_metadata_type.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_page_desk_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_page_subtype_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_page_type_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_page_user_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_pageable_object.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_pdf_signature_position.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_seal_certificate_sort_by.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_signature_format.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_signature_protocol.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_sort_object.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_subtype_dto.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_subtype_layer_association.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_subtype_layer_dto.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_subtype_metadata_dto.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_subtype_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_tenant_dto.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_tenant_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_tenant_sort_by.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_type_dto.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_type_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_typology_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_typology_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_typology_sort_by.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_user_dto.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_user_privilege.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_user_representation.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_user_sort_by.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_models/test_workflow_definition_sort_by.py` & `iparapheur-provisioning-1.6.4/test/test_models/test_workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/__init__.py` & `iparapheur-provisioning-1.6.4/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py` & `iparapheur-provisioning-1.6.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py`

 * *Files identical despite different names*

