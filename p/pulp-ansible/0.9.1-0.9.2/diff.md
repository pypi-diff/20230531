# Comparing `tmp/pulp-ansible-0.9.1.tar.gz` & `tmp/pulp-ansible-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-ansible-0.9.1.tar", last modified: Wed Aug 25 14:29:30 2021, max compression
+gzip compressed data, was "pulp-ansible-0.9.2.tar", last modified: Mon Oct  4 19:31:06 2021, max compression
```

## Comparing `pulp-ansible-0.9.1.tar` & `pulp-ansible-0.9.2.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.089864 pulp-ansible-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    27174 2021-08-25 14:29:28.000000 pulp-ansible-0.9.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (121)      540 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (121)    18046 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      319 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4357 2021-08-25 14:29:30.089864 pulp-ansible-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2943 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.081864 pulp-ansible-0.9.1/pulp_ansible/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.081864 pulp-ansible-0.9.1/pulp_ansible/app/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2021-08-25 14:29:29.000000 pulp-ansible-0.9.1/pulp_ansible/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     8419 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/downloaders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.081864 pulp-ansible-0.9.1/pulp_ansible/app/galaxy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/galaxy/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     5724 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/galaxy/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.081864 pulp-ansible-0.9.1/pulp_ansible/app/galaxy/v3/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/galaxy/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/galaxy/v3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4014 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/galaxy/v3/pagination.py
--rw-r--r--   0 runner    (1001) docker     (121)     7859 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/galaxy/v3/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)    18225 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/galaxy/v3/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     7433 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/galaxy/views.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/logutils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.085864 pulp-ansible-0.9.1/pulp_ansible/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0002_advanced_collections.py
--rw-r--r--   0 runner    (1001) docker     (121)     4021 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0003_add_tags_and_collectionversion_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0004_add_fulltext_search_indexes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0005_collectionversion_is_highest.py
--rw-r--r--   0 runner    (1001) docker     (121)      537 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0006_remove_whitelist_and_alter_collection_version_name.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0007_collectionversion_is_certified.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0008_collectionremote_requirements_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0009_collectionimport.py
--rw-r--r--   0 runner    (1001) docker     (121)     3537 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0010_ansible_related_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0011_collectionimport.py
--rw-r--r--   0 runner    (1001) docker     (121)      704 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0012_auto_20190906_2253.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0013_pulp_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      647 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0014_certification_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)      818 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0015_ansiblerepository.py
--rw-r--r--   0 runner    (1001) docker     (121)      889 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0016_add_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0017_increase_length_collectionversion_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0018_fix_collection_relative_path.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0019_collection_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0020_auto_20200810_1926.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0021_rename_role_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0022_URLField_to_CharField.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0023_alter_requirements_file_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0024_remove_collectionversion_certification.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0025_increase_collection_version_version_size.py
--rw-r--r--   0 runner    (1001) docker     (121)     2472 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0026_deprecation_per_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0027_tag_length.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0028_collectionversion_namespace_length.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0029_manifest_and_files_json_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0030_collectionversion_requires_ansible.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0031_ansiblerepository_last_synced_metadata_time.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0032_collectionremote_sync_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     3514 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/0033_swap_distribution_model.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2954 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/modelresource.py
--rw-r--r--   0 runner    (1001) docker     (121)    10305 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.085864 pulp-ansible-0.9.1/pulp_ansible/app/schema/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/schema/copy_config.json
--rw-r--r--   0 runner    (1001) docker     (121)    15770 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.085864 pulp-ansible-0.9.1/pulp_ansible/app/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    36570 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/tasks/collections.py
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/tasks/copy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5444 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/tasks/roles.py
--rw-r--r--   0 runner    (1001) docker     (121)     6792 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/tasks/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5102 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/tasks/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)    14032 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.085864 pulp-ansible-0.9.1/pulp_ansible/app/webserver_snippets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/webserver_snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/webserver_snippets/apache.conf
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/app/webserver_snippets/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.085864 pulp-ansible-0.9.1/pulp_ansible/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.085864 pulp-ansible-0.9.1/pulp_ansible/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/assets/func_test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.085864 pulp-ansible-0.9.1/pulp_ansible/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.085864 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.085864 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7329 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/test_crud_collection_versions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)    11784 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.085864 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10203 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v2/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v2/test_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.089864 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v3/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10281 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v3/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3383 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v3/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3948 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v3/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)    12246 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v3/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.089864 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/role/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/role/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6872 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/role/test_crd_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     4776 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/role/test_crud_remotes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3694 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/role/test_download_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     3217 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/role/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (121)     3550 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/role/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     5841 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/test_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     5521 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/test_import.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.089864 pulp-ansible-0.9.1/pulp_ansible/tests/functional/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/cli/test_collection_install.py
--rw-r--r--   0 runner    (1001) docker     (121)     5187 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/cli/test_collection_upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     2955 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/cli/test_role_install.py
--rw-r--r--   0 runner    (1001) docker     (121)     4472 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     8751 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.089864 pulp-ansible-0.9.1/pulp_ansible/tests/performance/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2293 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/performance/create_repos_with_collections.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/performance/fast_load_collections.py
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/performance/generate_collections.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/performance/promote.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.089864 pulp-ansible-0.9.1/pulp_ansible/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/unit/test_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.089864 pulp-ansible-0.9.1/pulp_ansible/tests/upgrade/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.089864 pulp-ansible-0.9.1/pulp_ansible/tests/upgrade/post/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/upgrade/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3458 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/upgrade/post/test_collection_install.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.089864 pulp-ansible-0.9.1/pulp_ansible/tests/upgrade/pre/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/upgrade/pre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3138 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pulp_ansible/tests/upgrade/pre/test_collection_install.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 14:29:30.081864 pulp-ansible-0.9.1/pulp_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4357 2021-08-25 14:29:30.000000 pulp-ansible-0.9.1/pulp_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5925 2021-08-25 14:29:30.000000 pulp-ansible-0.9.1/pulp_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-25 14:29:30.000000 pulp-ansible-0.9.1/pulp_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-08-25 14:29:30.000000 pulp-ansible-0.9.1/pulp_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-08-25 14:29:30.000000 pulp-ansible-0.9.1/pulp_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-08-25 14:29:30.000000 pulp-ansible-0.9.1/pulp_ansible.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      916 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-25 14:29:30.089864 pulp-ansible-0.9.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1493 2021-08-25 14:29:29.000000 pulp-ansible-0.9.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-08-25 14:29:17.000000 pulp-ansible-0.9.1/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.867350 pulp-ansible-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)    27396 2021-10-04 19:31:04.000000 pulp-ansible-0.9.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (121)    18046 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4357 2021-10-04 19:31:06.867350 pulp-ansible-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2943 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.847349 pulp-ansible-0.9.2/pulp_ansible/
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.851349 pulp-ansible-0.9.2/pulp_ansible/app/
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2021-10-04 19:31:06.000000 pulp-ansible-0.9.2/pulp_ansible/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8419 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/downloaders.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.851349 pulp-ansible-0.9.2/pulp_ansible/app/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/galaxy/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5724 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/galaxy/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.851349 pulp-ansible-0.9.2/pulp_ansible/app/galaxy/v3/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/galaxy/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1800 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/galaxy/v3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4014 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/galaxy/v3/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7859 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/galaxy/v3/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18225 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/galaxy/v3/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7433 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/galaxy/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/logutils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.859350 pulp-ansible-0.9.2/pulp_ansible/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     3125 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3489 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0002_advanced_collections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4021 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0003_add_tags_and_collectionversion_fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3132 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0004_add_fulltext_search_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0005_collectionversion_is_highest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0006_remove_whitelist_and_alter_collection_version_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0007_collectionversion_is_certified.py
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0008_collectionremote_requirements_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1333 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0009_collectionimport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3537 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0010_ansible_related_names.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0011_collectionimport.py
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0012_auto_20190906_2253.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1441 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0013_pulp_fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0014_certification_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0015_ansiblerepository.py
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0016_add_extension.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0017_increase_length_collectionversion_fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1187 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0018_fix_collection_relative_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0019_collection_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0020_auto_20200810_1926.py
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0021_rename_role_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0022_URLField_to_CharField.py
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0023_alter_requirements_file_field.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0024_remove_collectionversion_certification.py
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0025_increase_collection_version_version_size.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2472 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0026_deprecation_per_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0027_tag_length.py
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0028_collectionversion_namespace_length.py
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0029_manifest_and_files_json_fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3154 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0030_collectionversion_requires_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0031_ansiblerepository_last_synced_metadata_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0032_collectionremote_sync_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3514 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/0033_swap_distribution_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2954 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/modelresource.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10305 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.859350 pulp-ansible-0.9.2/pulp_ansible/app/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/schema/copy_config.json
+-rw-r--r--   0 runner    (1001) docker     (121)    15770 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.859350 pulp-ansible-0.9.2/pulp_ansible/app/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36606 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/tasks/collections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3023 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/tasks/copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5444 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/tasks/roles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6792 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/tasks/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5102 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/tasks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3336 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14032 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.859350 pulp-ansible-0.9.2/pulp_ansible/app/webserver_snippets/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/webserver_snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/webserver_snippets/apache.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/app/webserver_snippets/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.859350 pulp-ansible-0.9.2/pulp_ansible/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.859350 pulp-ansible-0.9.2/pulp_ansible/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/assets/func_test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.859350 pulp-ansible-0.9.2/pulp_ansible/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.859350 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.859350 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7308 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/test_crud_collection_versions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2991 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11784 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.859350 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v2/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10203 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v2/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2299 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v2/test_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.863350 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v3/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10281 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v3/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3371 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v3/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3930 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v3/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13637 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v3/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.863350 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/role/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/role/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6872 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/role/test_crd_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4776 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/role/test_crud_remotes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3694 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/role/test_download_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3217 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/role/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3550 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/role/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5841 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5521 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.863350 pulp-ansible-0.9.2/pulp_ansible/tests/functional/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3287 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/cli/test_collection_install.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5398 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/cli/test_collection_upload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2955 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/cli/test_role_install.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4472 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8751 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.863350 pulp-ansible-0.9.2/pulp_ansible/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2293 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/performance/create_repos_with_collections.py
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/performance/fast_load_collections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1408 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/performance/generate_collections.py
+-rw-r--r--   0 runner    (1001) docker     (121)      913 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/performance/promote.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.863350 pulp-ansible-0.9.2/pulp_ansible/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1821 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/unit/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.863350 pulp-ansible-0.9.2/pulp_ansible/tests/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.863350 pulp-ansible-0.9.2/pulp_ansible/tests/upgrade/post/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/upgrade/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3458 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/upgrade/post/test_collection_install.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.863350 pulp-ansible-0.9.2/pulp_ansible/tests/upgrade/pre/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/upgrade/pre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3138 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pulp_ansible/tests/upgrade/pre/test_collection_install.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 19:31:06.851349 pulp-ansible-0.9.2/pulp_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4357 2021-10-04 19:31:06.000000 pulp-ansible-0.9.2/pulp_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5925 2021-10-04 19:31:06.000000 pulp-ansible-0.9.2/pulp_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-04 19:31:06.000000 pulp-ansible-0.9.2/pulp_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-10-04 19:31:06.000000 pulp-ansible-0.9.2/pulp_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2021-10-04 19:31:06.000000 pulp-ansible-0.9.2/pulp_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-10-04 19:31:06.000000 pulp-ansible-0.9.2/pulp_ansible.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-04 19:31:06.867350 pulp-ansible-0.9.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1493 2021-10-04 19:31:06.000000 pulp-ansible-0.9.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-10-04 19:30:52.000000 pulp-ansible-0.9.2/unittest_requirements.txt
```

### Comparing `pulp-ansible-0.9.1/CHANGES.rst` & `pulp-ansible-0.9.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,28 @@
     To add a new change log entry, please see
     https://docs.pulpproject.org/en/3.0/nightly/contributing/git.html#changelog-update
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+0.9.2 (2021-10-04)
+==================
+
+Bugfixes
+--------
+
+- Fixed optimized mirror syncs erroneously removing all content in the repository.
+  (backported from #9476)
+  `#9480 <https://pulp.plan.io/issues/9480>`_
+
+
+----
+
+
 0.9.1 (2021-08-25)
 ==================
 
 Bugfixes
 --------
 
 - Improved performance on reporting progress on parsing collection metadata
```

### Comparing `pulp-ansible-0.9.1/COMMITMENT` & `pulp-ansible-0.9.2/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/COPYRIGHT` & `pulp-ansible-0.9.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/LICENSE` & `pulp-ansible-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/PKG-INFO` & `pulp-ansible-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-ansible
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pulp plugin to manage Ansible content, e.g. roles
 Home-page: https://github.com/pulp/pulp_ansible
 Author: Pulp Ansible Plugin Project Developers
 Author-email: pulp-dev@redhat.com
 License: GPLv2+
 Description: pulp_ansible
         ============
```

### Comparing `pulp-ansible-0.9.1/README.rst` & `pulp-ansible-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/downloaders.py` & `pulp-ansible-0.9.2/pulp_ansible/app/downloaders.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/galaxy/mixins.py` & `pulp-ansible-0.9.2/pulp_ansible/app/galaxy/mixins.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/galaxy/serializers.py` & `pulp-ansible-0.9.2/pulp_ansible/app/galaxy/serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/galaxy/v3/exceptions.py` & `pulp-ansible-0.9.2/pulp_ansible/app/galaxy/v3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/galaxy/v3/pagination.py` & `pulp-ansible-0.9.2/pulp_ansible/app/galaxy/v3/pagination.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/galaxy/v3/serializers.py` & `pulp-ansible-0.9.2/pulp_ansible/app/galaxy/v3/serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/galaxy/v3/views.py` & `pulp-ansible-0.9.2/pulp_ansible/app/galaxy/v3/views.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/galaxy/views.py` & `pulp-ansible-0.9.2/pulp_ansible/app/galaxy/views.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/logutils.py` & `pulp-ansible-0.9.2/pulp_ansible/app/logutils.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0001_initial.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0002_advanced_collections.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0002_advanced_collections.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0003_add_tags_and_collectionversion_fields.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0003_add_tags_and_collectionversion_fields.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0004_add_fulltext_search_indexes.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0004_add_fulltext_search_indexes.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0005_collectionversion_is_highest.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0005_collectionversion_is_highest.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0006_remove_whitelist_and_alter_collection_version_name.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0006_remove_whitelist_and_alter_collection_version_name.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0009_collectionimport.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0009_collectionimport.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0010_ansible_related_names.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0010_ansible_related_names.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0011_collectionimport.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0011_collectionimport.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0012_auto_20190906_2253.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0012_auto_20190906_2253.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0013_pulp_fields.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0013_pulp_fields.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0014_certification_enum.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0014_certification_enum.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0015_ansiblerepository.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0015_ansiblerepository.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0016_add_extension.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0016_add_extension.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0017_increase_length_collectionversion_fields.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0017_increase_length_collectionversion_fields.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0018_fix_collection_relative_path.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0018_fix_collection_relative_path.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0019_collection_token.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0019_collection_token.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0021_rename_role_remote.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0021_rename_role_remote.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0022_URLField_to_CharField.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0022_URLField_to_CharField.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0026_deprecation_per_repository.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0026_deprecation_per_repository.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0029_manifest_and_files_json_fields.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0029_manifest_and_files_json_fields.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0030_collectionversion_requires_ansible.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0030_collectionversion_requires_ansible.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/migrations/0033_swap_distribution_model.py` & `pulp-ansible-0.9.2/pulp_ansible/app/migrations/0033_swap_distribution_model.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/modelresource.py` & `pulp-ansible-0.9.2/pulp_ansible/app/modelresource.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/models.py` & `pulp-ansible-0.9.2/pulp_ansible/app/models.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/schema/copy_config.json` & `pulp-ansible-0.9.2/pulp_ansible/app/schema/copy_config.json`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/serializers.py` & `pulp-ansible-0.9.2/pulp_ansible/app/serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/settings.py` & `pulp-ansible-0.9.2/pulp_ansible/app/settings.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/tasks/collections.py` & `pulp-ansible-0.9.2/pulp_ansible/app/tasks/collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,18 @@
     remote = CollectionRemote.objects.get(pk=remote_pk)
     repository = AnsibleRepository.objects.get(pk=repository_pk)
 
     if not remote.url:
         raise ValueError(_("A CollectionRemote must have a 'url' specified to synchronize."))
 
     first_stage = CollectionSyncFirstStage(remote, repository, optimize)
+    if first_stage.should_sync is False:
+        log.debug(_("no-op: remote wasn't updated since last sync."))
+        return
+
     d_version = AnsibleDeclarativeVersion(first_stage, repository, mirror=mirror)
     repo_version = d_version.create()
 
     if not repo_version:
         return
 
     if first_stage.last_synced_metadata_time:
@@ -369,26 +373,30 @@
             repository (AnsibleRepository): The repository being syncedself.
             optimize (boolean): Whether to optimize sync or not.
 
         """
         super().__init__()
         self.remote = remote
         self.repository = repository
-        self.optimize = optimize
         self.collection_info = parse_collections_requirements_file(remote.requirements_file)
         self.deprecations = Q()
         self.add_dependents = self.collection_info and self.remote.sync_dependencies
         self.already_synced = set()
         self._unpaginated_collection_metadata = None
         self._unpaginated_collection_version_metadata = None
         self.last_synced_metadata_time = None
 
         # Interpret download policy
         self.deferred_download = self.remote.policy != Remote.IMMEDIATE
 
+        # Check if we should sync
+        self.should_sync = not optimize or asyncio.get_event_loop().run_until_complete(
+            self._should_we_sync()
+        )
+
     @alru_cache(maxsize=128)
     async def _get_root_api(self, root):
         """
         Returns the root api path and api version.
 
         Based on https://git.io/JTMxE.
         """
@@ -751,20 +759,14 @@
 
         return True
 
     async def run(self):
         """
         Build and emit `DeclarativeContent` from the ansible metadata.
         """
-        if self.optimize:
-            should_we_sync = await self._should_we_sync()
-            if should_we_sync is False:
-                log.debug(_("no-op: remote wasn't updated since last sync."))
-                return
-
         tasks = []
         loop = asyncio.get_event_loop()
 
         msg = _("Parsing CollectionVersion Metadata")
         with ProgressReport(message=msg, code="sync.parsing.metadata") as pb:
             self.parsing_metadata_progress_bar = pb
             await self._download_unpaginated_metadata()
```

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/tasks/copy.py` & `pulp-ansible-0.9.2/pulp_ansible/app/tasks/copy.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/tasks/roles.py` & `pulp-ansible-0.9.2/pulp_ansible/app/tasks/roles.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/tasks/test_tasks.py` & `pulp-ansible-0.9.2/pulp_ansible/app/tasks/test_tasks.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/tasks/utils.py` & `pulp-ansible-0.9.2/pulp_ansible/app/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/urls.py` & `pulp-ansible-0.9.2/pulp_ansible/app/urls.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/app/viewsets.py` & `pulp-ansible-0.9.2/pulp_ansible/app/viewsets.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/test_crud_collection_versions.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/test_crud_collection_versions.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,27 +92,27 @@
         cls.cv_content_api = ContentCollectionVersionsApi(gen_ansible_client())
 
     @classmethod
     def tearDownClass(cls):
         """Clean class-wide variable."""
         delete_orphans()
 
-    def upload_collection(self, namespace="pulp", name="pulp_installer", version="3.14.0"):
+    def upload_collection(self, namespace="pulp", name="squeezer", version="0.0.9"):
         """Upload collection."""
         url = f"https://galaxy.ansible.com/download/{namespace}-{name}-{version}.tar.gz"
         collection_content = http_get(url)
         with NamedTemporaryFile() as temp_file:
             temp_file.write(collection_content)
             return self.cv_content_api.create(
                 file=temp_file.name, namespace=namespace, name=name, version=version
             )
 
     def test_01_create_content_unit(self):
         """Create content unit."""
-        attrs = dict(namespace="pulp", name="pulp_installer", version="3.14.0")
+        attrs = dict(namespace="pulp", name="squeezer", version="0.0.9")
         response = self.upload_collection(**attrs)
         created_resources = monitor_task(response.task).created_resources
         content_unit = self.cv_content_api.read(created_resources[0])
         self.content_unit.update(content_unit.to_dict())
         for key, val in attrs.items():
             with self.subTest(key=key):
                 self.assertEqual(self.content_unit[key], val)
@@ -170,13 +170,13 @@
             self.cv_content_api.delete(self.content_unit["pulp_href"])
         msg = "object has no attribute 'delete'"
         self.assertIn(msg, exc.exception.args[0])
 
     @skip_if(bool, "content_unit", False)
     def test_05_duplicate_raise_error(self):
         """Attempt to create duplicate collection."""
-        attrs = dict(namespace="pulp", name="pulp_installer", version="3.14.0")
+        attrs = dict(namespace="pulp", name="squeezer", version="0.0.9")
         with self.assertRaises(ApiException) as ctx:
             self.upload_collection(**attrs)
         self.assertIn(
             "The fields namespace, name, version must make a unique set.", ctx.exception.body
         )
```

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/test_remote.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/test_remote.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/test_sync.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/test_sync.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v2/test_sync.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v2/test_sync.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v3/test_collection.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v3/test_collection.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v3/test_deprecation.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v3/test_deprecation.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class DeprecationTestCase(TestCaseUsingBindings, SyncHelpersMixin):
     """Test deprecation status sync."""
 
     def test_v3_deprecation(self):
         """Test sync  sync."""
         # Sync down two collections into a repo
         requirements = (
-            "collections:\n  - name: testing.k8s_demo_collection\n  - name: pulp.pulp_installer"
+            "collections:\n  - name: testing.k8s_demo_collection\n  - name: pulp.squeezer"
         )
 
         body = gen_ansible_remote(
             url="https://galaxy.ansible.com",
             requirements_file=requirements,
             sync_dependencies=False,
         )
@@ -56,15 +56,15 @@
             "k8s_demo_collection", "testing", first_distro.base_path, {"deprecated": False}
         )
         collections = self.collections_v3api.list(first_distro.base_path, namespace="testing")
         self.assertFalse(collections.data[0].deprecated)
 
         # Update the requirements to sync down both collections this time
         requirements = (
-            "collections:\n  - name: testing.k8s_demo_collection\n  - name: pulp.pulp_installer"
+            "collections:\n  - name: testing.k8s_demo_collection\n  - name: pulp.squeezer"
         )
         self.remote_collection_api.partial_update(
             second_remote.pulp_href, {"requirements_file": requirements}
         )
 
         # Sync the second repo again
         self._sync_repo(second_repo)
```

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v3/test_serializers.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v3/test_serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,43 +28,43 @@
         cls.collections_versions_api = ContentCollectionVersionsApi(cls.client)
         cls.collections_versions_v3api = PulpAnsibleApiV3CollectionsVersionsApi(cls.client)
 
     def test_v3_updated_at(self):
         """Test Collections V3 endpoint field: ``updated_at``."""
         body = gen_ansible_remote(
             url="https://galaxy.ansible.com",
-            requirements_file="collections:\n  - pulp.pulp_installer",
+            requirements_file="collections:\n  - pulp.squeezer",
             sync_dependencies=False,
         )
         remote = self.remote_collection_api.create(body)
         self.addCleanup(self.remote_collection_api.delete, remote.pulp_href)
 
         repo = self._create_repo_and_sync_with_remote(remote)
         distribution = self._create_distribution_from_repo(repo)
 
         collections = self.collections_api.list(distribution.base_path)
 
         original_highest_version = collections.data[0].highest_version["version"]
         original_updated_at = collections.data[0].updated_at
 
-        versions = self.collections_versions_api.list(version="3.6.4")
+        versions = self.collections_versions_api.list(version="0.0.7")
         original_total_versions = self.collections_versions_v3api.list(
-            "pulp_installer", "pulp", distribution.base_path
+            "squeezer", "pulp", distribution.base_path
         ).meta.count
 
         data = {"remove_content_units": [versions.results[0].pulp_href]}
         response = self.repo_api.modify(repo.pulp_href, data)
         monitor_task(response.task)
 
         collections = self.collections_api.list(distribution.base_path)
         highest_version = collections.data[0].highest_version["version"]
         updated_at = collections.data[0].updated_at
 
         total_versions = self.collections_versions_v3api.list(
-            "pulp_installer", "pulp", distribution.base_path
+            "squeezer", "pulp", distribution.base_path
         ).meta.count
 
         self.assertEqual(highest_version, original_highest_version)
         self.assertEqual(original_total_versions, total_versions + 1)
         self.assertGreater(updated_at, original_updated_at)
 
     def test_v3_collection_version_from_synced_data(self):
```

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/collection/v3/test_sync.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/collection/v3/test_sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -132,14 +132,43 @@
         second_repo = self.repo_api.read(second_repo.pulp_href)
         task = tasks.read(sync_response.task)
 
         msg = "no-op: {url} did not change since last sync".format(url=second_remote.url)
         messages = [r.message for r in task.progress_reports]
         self.assertIn(msg, str(messages))
 
+    def test_noop_resync_with_mirror_from_pulp(self):
+        """Test whether no-op sync with mirror=True doesn't remove repository content."""
+        second_body = gen_ansible_remote(
+            url=self.distribution.client_url,
+            requirements_file=self.requirements_file,
+            sync_dependencies=False,
+        )
+        second_remote = self.remote_collection_api.create(second_body)
+        self.addCleanup(self.remote_collection_api.delete, second_remote.pulp_href)
+
+        second_repo = self._create_repo_and_sync_with_remote(second_remote)
+
+        second_content = self.cv_api.list(repository_version=f"{second_repo.pulp_href}versions/1/")
+        self.assertGreaterEqual(len(second_content.results), 1)
+
+        # Resync
+        repository_sync_data = AnsibleRepositorySyncURL(
+            remote=second_remote.pulp_href, optimize=True, mirror=True
+        )
+        sync_response = self.repo_api.sync(second_repo.pulp_href, repository_sync_data)
+        monitor_task(sync_response.task)
+        second_repo = self.repo_api.read(second_repo.pulp_href)
+        self.assertEqual(int(second_repo.latest_version_href[-2]), 1)
+        task = tasks.read(sync_response.task)
+
+        msg = "no-op: {url} did not change since last sync".format(url=second_remote.url)
+        messages = [r.message for r in task.progress_reports]
+        self.assertIn(msg, str(messages))
+
     def test_update_requirements_file(self):
         """Test requirements_file update."""
         body = gen_ansible_remote(
             url=self.distribution.client_url,
             requirements_file=self.requirements_file,
             sync_dependencies=False,
         )
```

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/role/test_crd_distribution.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/role/test_crd_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/role/test_crud_remotes.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/role/test_crud_remotes.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/role/test_download_content.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/role/test_download_content.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/role/test_publish.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/role/test_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/role/test_sync.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/role/test_sync.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/test_export.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/test_export.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/api/test_import.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/api/test_import.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/cli/test_collection_install.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/cli/test_collection_install.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/cli/test_collection_upload.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/cli/test_collection_upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Tests that Collections can be uploaded to  Pulp with the ansible-galaxy CLI."""
 
 import random
 import string
 import subprocess
 import tempfile
-import unittest
 import os
 
 from pulpcore.client.pulp_ansible import (
     DistributionsAnsibleApi,
     PulpAnsibleApiV3CollectionsApi,
     PulpAnsibleApiV3CollectionsVersionsApi,
     RemotesCollectionApi,
     RepositoriesAnsibleApi,
     RepositoriesAnsibleVersionsApi,
 )
-from pulp_smash.pulp3.bindings import monitor_task
-from pulp_smash.pulp3.utils import delete_orphans, gen_distribution, gen_repo
+from pulp_smash.pulp3.bindings import delete_orphans, monitor_task, PulpTestCase
+from pulp_smash.pulp3.utils import gen_distribution, gen_repo
+from pulp_smash.utils import http_get, uuid4
 
 from pulp_ansible.tests.functional.utils import gen_ansible_client, wait_tasks
 from pulp_ansible.tests.functional.utils import set_up_module as setUpModule  # noqa:F401
 
 
-class InstallCollectionTestCase(unittest.TestCase):
+class InstallCollectionTestCase(PulpTestCase):
     """Test whether ansible-galaxy can upload a Collection to Pulp."""
 
     @classmethod
     def setUpClass(cls):
         """Create class-wide variables."""
         delete_orphans()
         cls.client = gen_ansible_client()
@@ -95,29 +95,33 @@
         distribution = self.distributions_api.read(created_resources[0])
 
         self.addCleanup(self.distributions_api.delete, distribution.pulp_href)
 
         collections = self.collections_v3api.list(distribution.base_path)
         self.assertEqual(collections.meta.count, 0)
 
-        colletion_path = os.path.join(
-            os.getcwd(), "pulp_ansible/tests/assets/collections/pulp-testing_asset-1.0.0.tar.gz"
-        )
+        temp_path = f"/tmp/{uuid4()}"
+        subprocess.run(f"mkdir -p {temp_path}".split())
+
+        content = http_get("https://galaxy.ansible.com/download/pulp-squeezer-0.0.9.tar.gz")
+        collection_path = f"{temp_path}/pulp-squeezer-0.0.9.tar.gz"
+        with open(collection_path, "wb") as f:
+            f.write(content)
 
         cmd = "ansible-galaxy collection publish -c -s {} {}".format(
-            distribution.client_url, colletion_path
+            distribution.client_url, collection_path
         )
         subprocess.run(cmd.split())
         wait_tasks()
 
         collections = self.collections_v3api.list(distribution.base_path)
         self.assertEqual(collections.meta.count, 1)
 
         repo = self.repo_api.read(repo.pulp_href)
         repo_version = self.repo_versions_api.read(repo.latest_version_href)
         self.assertEqual(repo_version.number, 1)  # We uploaded 1 collection
 
         version = self.collections_versions_v3api.read(
-            "testing_asset", "pulp", distribution.base_path, "1.0.0"
+            "squeezer", "pulp", distribution.base_path, "0.0.9"
         )
 
-        self.assertEqual(version.requires_ansible, ">=2.9.10,<2.11")
+        self.assertEqual(version.requires_ansible, ">=2.8")
```

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/cli/test_role_install.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/cli/test_role_install.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/constants.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/functional/utils.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/performance/create_repos_with_collections.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/performance/create_repos_with_collections.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/performance/fast_load_collections.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/performance/fast_load_collections.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/performance/generate_collections.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/performance/generate_collections.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/performance/promote.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/performance/promote.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/unit/test_serializers.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/unit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/upgrade/post/test_collection_install.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/upgrade/post/test_collection_install.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible/tests/upgrade/pre/test_collection_install.py` & `pulp-ansible-0.9.2/pulp_ansible/tests/upgrade/pre/test_collection_install.py`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pulp_ansible.egg-info/PKG-INFO` & `pulp-ansible-0.9.2/pulp_ansible.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-ansible
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pulp plugin to manage Ansible content, e.g. roles
 Home-page: https://github.com/pulp/pulp_ansible
 Author: Pulp Ansible Plugin Project Developers
 Author-email: pulp-dev@redhat.com
 License: GPLv2+
 Description: pulp_ansible
         ============
```

### Comparing `pulp-ansible-0.9.1/pulp_ansible.egg-info/SOURCES.txt` & `pulp-ansible-0.9.2/pulp_ansible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/pyproject.toml` & `pulp-ansible-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-ansible-0.9.1/setup.py` & `pulp-ansible-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = requirements.readlines()
 
 with open("README.rst") as f:
     long_description = f.read()
 
 setup(
     name="pulp-ansible",
-    version="0.9.1",
+    version="0.9.2",
     description="Pulp plugin to manage Ansible content, e.g. roles",
     long_description=long_description,
     license="GPLv2+",
     author="Pulp Ansible Plugin Project Developers",
     author_email="pulp-dev@redhat.com",
     url="https://github.com/pulp/pulp_ansible",
     install_requires=requirements,
```

