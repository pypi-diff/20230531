# Comparing `tmp/appengine-python-standard-1.1.1.tar.gz` & `tmp/appengine-python-standard-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appengine-python-standard-1.1.1.tar", last modified: Mon Apr 24 23:22:38 2023, max compression
+gzip compressed data, was "appengine-python-standard-1.1.2.tar", last modified: Wed May 31 17:45:09 2023, max compression
```

## Comparing `appengine-python-standard-1.1.1.tar` & `appengine-python-standard-1.1.2.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.886088 appengine-python-standard-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-24 23:22:38.886088 appengine-python-standard-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 23:22:38.886088 appengine-python-standard-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.858088 appengine-python-standard-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.862088 appengine-python-standard-1.1.1/src/appengine_python_standard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-24 23:22:38.000000 appengine-python-standard-1.1.1/src/appengine_python_standard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-04-24 23:22:38.000000 appengine-python-standard-1.1.1/src/appengine_python_standard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:22:38.000000 appengine-python-standard-1.1.1/src/appengine_python_standard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 23:22:38.000000 appengine-python-standard-1.1.1/src/appengine_python_standard.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-24 23:22:38.000000 appengine-python-standard-1.1.1/src/appengine_python_standard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 23:22:38.000000 appengine-python-standard-1.1.1/src/appengine_python_standard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.862088 appengine-python-standard-1.1.1/src/google/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.862088 appengine-python-standard-1.1.1/src/google/appengine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.862088 appengine-python-standard-1.1.1/src/google/appengine/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.862088 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4766 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4565 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/dfa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5416 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/dottreegen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10171 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1004 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/extras.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6616 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40831 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/recognizers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34633 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/streams.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9197 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/tokens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55086 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/tree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15019 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/treewizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.866088 appengine-python-standard-1.1.1/src/google/appengine/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4326 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/api_base_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6637 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/api_testutil.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7038 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/apiproxy_rpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5483 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/apiproxy_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23020 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/apiproxy_stub_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.870088 appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1184 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2487 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/_metadata_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13352 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/app_identity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8066 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/app_identity_defaultcredentialsbased_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8537 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/app_identity_keybased_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9244 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/app_identity_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2728 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/app_identity_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8305 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/app_identity_stub_base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    92389 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/appinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5506 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/appinfo_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5858 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/backendinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.870088 appengine-python-standard-1.1.1/src/google/appengine/api/background_thread/
--rwxr-xr-x   0 runner    (1001) docker     (123)      705 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/background_thread/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4207 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/background_thread/background_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.870088 appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/
--rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17082 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/blobstore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8934 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/blobstore_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15313 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/blobstore_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2975 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/blobstore_stub_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1815 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/dict_blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4402 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/file_blob_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.870088 appengine-python-standard-1.1.1/src/google/appengine/api/capabilities/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6171 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/capabilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3227 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/capabilities/capability_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5127 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/capabilities/capability_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3816 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/cmp_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6304 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/croninfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    94133 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/datastore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2641 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/datastore_admin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12012 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/datastore_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4349 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/datastore_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23483 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/datastore_file_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    65487 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/datastore_types.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6643 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/dispatchinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3566 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/full_app_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.870088 appengine-python-standard-1.1.1/src/google/appengine/api/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)    76512 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/images/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2607 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/images/image_comparison.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/images/images_blob_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15751 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/images/images_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25149 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/images/images_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12487 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/lib_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    56706 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/mail.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/mail_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4303 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/mail_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16788 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/mail_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4871 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/mail_stub_service_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.870088 appengine-python-standard-1.1.1/src/google/appengine/api/memcache/
--rwxr-xr-x   0 runner    (1001) docker     (123)    54575 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/memcache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17524 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/memcache/memcache_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18037 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/memcache/memcache_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4122 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/memcache/memcache_stub_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5450 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/module_testutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.870088 appengine-python-standard-1.1.1/src/google/appengine/api/modules/
--rwxr-xr-x   0 runner    (1001) docker     (123)      678 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/modules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15352 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/modules/modules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10494 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/modules/modules_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5951 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/modules/modules_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.870088 appengine-python-standard-1.1.1/src/google/appengine/api/namespace_manager/
--rwxr-xr-x   0 runner    (1001) docker     (123)      711 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/namespace_manager/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2828 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/namespace_manager/namespace_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.874088 appengine-python-standard-1.1.1/src/google/appengine/api/oauth/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1061 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/oauth/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8589 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/oauth/oauth_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10946 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/queueinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24147 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/request_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.874088 appengine-python-standard-1.1.1/src/google/appengine/api/runtime/
--rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/runtime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3314 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/runtime/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.874088 appengine-python-standard-1.1.1/src/google/appengine/api/search/
--rwxr-xr-x   0 runner    (1001) docker     (123)    39873 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/ExpressionLexer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55393 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/ExpressionParser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28531 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/QueryLexer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    82233 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/QueryParser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5199 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/expression_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/geo_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8248 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/query_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   139421 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17321 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/search_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5749 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/search_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40299 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/simple_search_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.874088 appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/
--rwxr-xr-x   0 runner    (1001) docker     (123)      601 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18579 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/document_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20569 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/expression_evaluator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13705 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/simple_facet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5815 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/simple_tokenizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/tokens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2237 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/search/unicode_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1765 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/stublib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.874088 appengine-python-standard-1.1.1/src/google/appengine/api/system/
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/system/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5013 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/system/system_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/system/system_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.874088 appengine-python-standard-1.1.1/src/google/appengine/api/taskqueue/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1854 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/taskqueue/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    96230 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/taskqueue/taskqueue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39984 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/taskqueue/taskqueue_service_bytes_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   103352 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/taskqueue/taskqueue_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4393 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/titanoboa_request_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17484 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/urlfetch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/urlfetch_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5949 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/urlfetch_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18940 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/urlfetch_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6192 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/user_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7422 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/user_service_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9540 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47815 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/validation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13341 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/yaml_builder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2955 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/yaml_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8120 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/yaml_listener.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9368 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/yaml_object.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5539 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/api/yaml_test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.874088 appengine-python-standard-1.1.1/src/google/appengine/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/base/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3147 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/base/capabilities_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.878088 appengine-python-standard-1.1.1/src/google/appengine/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2996 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/action_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1835 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/cloud_datastore_v1_remote_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20288 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/cloud_datastore_v1_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38410 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/cloud_datastore_validator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31628 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_index.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6350 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_index_xml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_pb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57902 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_pbs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   110009 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    97472 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_rpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17779 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_stub_index.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   173811 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_stub_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36343 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_v3_bytes_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25116 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_v4_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14281 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_v4_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39296 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_v4_validator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6730 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/document_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19017 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/entity_bytes_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5968 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/entity_v4_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1990 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/snapshot_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17703 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/datastore/sortable_pb_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.878088 appengine-python-standard-1.1.1/src/google/appengine/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.878088 appengine-python-standard-1.1.1/src/google/appengine/ext/blobstore/
--rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/blobstore/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50088 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/blobstore/blobstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.882088 appengine-python-standard-1.1.1/src/google/appengine/ext/db/
--rwxr-xr-x   0 runner    (1001) docker     (123)   126163 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/db/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9980 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/db/metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12855 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/db/polymodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13730 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/db/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4993 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/db/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.882088 appengine-python-standard-1.1.1/src/google/appengine/ext/deferred/
--rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/deferred/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14355 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/deferred/deferred.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.882088 appengine-python-standard-1.1.1/src/google/appengine/ext/gql/
--rwxr-xr-x   0 runner    (1001) docker     (123)    44600 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.882088 appengine-python-standard-1.1.1/src/google/appengine/ext/key_range/
--rwxr-xr-x   0 runner    (1001) docker     (123)    27878 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/key_range/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.882088 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15403 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/blobstore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43446 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1995 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/django_middleware.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9344 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/eventloop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30714 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/key.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21525 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/key_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9859 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   130535 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8545 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/polymodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    66131 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14590 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37881 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/tasklets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6591 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/test_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5606 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.882088 appengine-python-standard-1.1.1/src/google/appengine/ext/remote_api/
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/remote_api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6866 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/remote_api/remote_api_bytes_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.882088 appengine-python-standard-1.1.1/src/google/appengine/ext/testbed/
--rwxr-xr-x   0 runner    (1001) docker     (123)    32956 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/ext/testbed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.886088 appengine-python-standard-1.1.1/src/google/appengine/runtime/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1607 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      798 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/apiproxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3096 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/apiproxy_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6655 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/background.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.886088 appengine-python-standard-1.1.1/src/google/appengine/runtime/context/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/context/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6143 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/context/ctx_test_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1875 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/context/gae_headers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1723 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/context/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10909 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/default_api_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5666 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/initialize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10837 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/middlewares.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4553 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/request_environment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4117 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/runtime/thread_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:38.886088 appengine-python-standard-1.1.1/src/google/appengine/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      904 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/tools/app_engine_config_exception.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1411 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/tools/os_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8563 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/tools/queue_xml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1774 2023-04-24 23:22:29.000000 appengine-python-standard-1.1.1/src/google/appengine/tools/xml_parser_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.468728 appengine-python-standard-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-31 17:45:09.468728 appengine-python-standard-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:45:09.468728 appengine-python-standard-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.408723 appengine-python-standard-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.420724 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-31 17:45:09.000000 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-05-31 17:45:09.000000 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:45:09.000000 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 17:45:09.000000 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-31 17:45:09.000000 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 17:45:09.000000 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.420724 appengine-python-standard-1.1.2/src/google/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.420724 appengine-python-standard-1.1.2/src/google/appengine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.420724 appengine-python-standard-1.1.2/src/google/appengine/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.424725 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4766 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4565 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/dfa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5416 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/dottreegen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10171 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1004 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/extras.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6616 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40831 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/recognizers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34633 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/streams.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9197 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/tokens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55086 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/tree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15019 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/treewizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.432725 appengine-python-standard-1.1.2/src/google/appengine/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4326 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/api_base_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6637 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/api_testutil.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7038 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/apiproxy_rpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5483 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/apiproxy_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23020 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/apiproxy_stub_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.436726 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1184 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2487 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/_metadata_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13352 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8066 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_defaultcredentialsbased_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8537 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_keybased_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9244 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2728 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8305 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_stub_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    92389 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/appinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5506 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/appinfo_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5858 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/backendinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.436726 appengine-python-standard-1.1.2/src/google/appengine/api/background_thread/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      705 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/background_thread/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4207 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/background_thread/background_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.436726 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17082 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8934 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15313 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2975 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore_stub_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1815 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/dict_blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4402 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/file_blob_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.436726 appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6171 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3227 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/capability_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5127 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/capability_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3816 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/cmp_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6304 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/croninfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    94133 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/datastore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2641 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/datastore_admin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12012 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/datastore_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4349 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/datastore_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23483 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/datastore_file_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    65487 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/datastore_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6643 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/dispatchinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3566 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/full_app_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.440726 appengine-python-standard-1.1.2/src/google/appengine/api/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    76512 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/images/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2607 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/images/image_comparison.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/images/images_blob_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15751 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/images/images_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25149 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/images/images_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12487 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/lib_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56706 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/mail.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/mail_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4303 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/mail_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16788 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/mail_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4871 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/mail_stub_service_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.440726 appengine-python-standard-1.1.2/src/google/appengine/api/memcache/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54575 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/memcache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17524 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/memcache/memcache_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18037 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/memcache/memcache_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4122 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/memcache/memcache_stub_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5450 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/module_testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.440726 appengine-python-standard-1.1.2/src/google/appengine/api/modules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      678 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/modules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15352 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/modules/modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10494 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/modules/modules_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5951 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/modules/modules_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.440726 appengine-python-standard-1.1.2/src/google/appengine/api/namespace_manager/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      711 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/namespace_manager/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2828 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/namespace_manager/namespace_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.440726 appengine-python-standard-1.1.2/src/google/appengine/api/oauth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1061 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/oauth/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8589 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/oauth/oauth_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10946 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/queueinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24147 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/request_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.440726 appengine-python-standard-1.1.2/src/google/appengine/api/runtime/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/runtime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3314 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/runtime/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.444726 appengine-python-standard-1.1.2/src/google/appengine/api/search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39873 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/ExpressionLexer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55393 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/ExpressionParser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28531 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/QueryLexer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    82233 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/QueryParser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5199 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/expression_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/geo_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8248 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/query_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   139421 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17321 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/search_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5749 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/search_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40299 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/simple_search_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.448727 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      601 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18579 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/document_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20569 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/expression_evaluator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13705 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/simple_facet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5815 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/simple_tokenizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/tokens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2237 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/unicode_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1765 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/stublib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.448727 appengine-python-standard-1.1.2/src/google/appengine/api/system/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/system/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5013 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/system/system_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/system/system_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.448727 appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1854 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    96230 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/taskqueue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39984 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/taskqueue_service_bytes_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   103352 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/taskqueue_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4393 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/titanoboa_request_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17484 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5949 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18940 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6192 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/user_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7422 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/user_service_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9540 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47815 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/validation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13341 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/yaml_builder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2955 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/yaml_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8120 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/yaml_listener.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9368 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/yaml_object.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5539 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/yaml_test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.448727 appengine-python-standard-1.1.2/src/google/appengine/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/base/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3147 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/base/capabilities_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.456727 appengine-python-standard-1.1.2/src/google/appengine/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2996 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/action_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1835 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/cloud_datastore_v1_remote_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20288 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/cloud_datastore_v1_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38410 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/cloud_datastore_validator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31628 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_index.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6350 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_index_xml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_pb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57902 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_pbs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   110009 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    97472 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_rpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17779 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_stub_index.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   173811 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_stub_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36343 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v3_bytes_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25116 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v4_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14281 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v4_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39296 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v4_validator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6730 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/document_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19017 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/entity_bytes_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5968 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/entity_v4_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1990 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/snapshot_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17703 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/sortable_pb_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.456727 appengine-python-standard-1.1.2/src/google/appengine/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.456727 appengine-python-standard-1.1.2/src/google/appengine/ext/blobstore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/blobstore/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50088 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/blobstore/blobstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.456727 appengine-python-standard-1.1.2/src/google/appengine/ext/db/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   126163 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/db/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9980 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/db/metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12855 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/db/polymodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13730 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/db/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4993 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/db/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.460728 appengine-python-standard-1.1.2/src/google/appengine/ext/deferred/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/deferred/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14355 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/deferred/deferred.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.460728 appengine-python-standard-1.1.2/src/google/appengine/ext/gql/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44600 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.460728 appengine-python-standard-1.1.2/src/google/appengine/ext/key_range/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27878 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/key_range/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.464728 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15403 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/blobstore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43446 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1995 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/django_middleware.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9344 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/eventloop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30714 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/key.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21525 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/key_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9859 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   130896 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8545 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/polymodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    66131 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14590 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37881 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/tasklets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6591 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/test_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5606 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.464728 appengine-python-standard-1.1.2/src/google/appengine/ext/remote_api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/remote_api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6866 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/remote_api/remote_api_bytes_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.464728 appengine-python-standard-1.1.2/src/google/appengine/ext/testbed/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32956 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/testbed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.464728 appengine-python-standard-1.1.2/src/google/appengine/runtime/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1607 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      798 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/apiproxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3096 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/apiproxy_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6655 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/background.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.468728 appengine-python-standard-1.1.2/src/google/appengine/runtime/context/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/context/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6143 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/context/ctx_test_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1875 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/context/gae_headers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1723 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/context/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10909 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/default_api_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5666 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/initialize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10837 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/middlewares.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4553 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/request_environment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4117 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/thread_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.468728 appengine-python-standard-1.1.2/src/google/appengine/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      904 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/tools/app_engine_config_exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1411 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/tools/os_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8563 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/tools/queue_xml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1774 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/tools/xml_parser_utils.py
```

### Comparing `appengine-python-standard-1.1.1/LICENSE` & `appengine-python-standard-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/PKG-INFO` & `appengine-python-standard-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appengine-python-standard
-Version: 1.1.1
+Version: 1.1.2
 Summary: Google App Engine services SDK for Python 3
 Home-page: https://github.com/GoogleCloudPlatform/appengine-python-standard
 Author: Google LLC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
```

### Comparing `appengine-python-standard-1.1.1/README.md` & `appengine-python-standard-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/setup.py` & `appengine-python-standard-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="appengine-python-standard",
-    version="1.1.1",
+    version="1.1.2",
     author="Google LLC",
     description="Google App Engine services SDK for Python 3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GoogleCloudPlatform/appengine-python-standard",
     packages=setuptools.find_packages(where="src"),
     namespace_packages=["google"],
```

### Comparing `appengine-python-standard-1.1.1/src/appengine_python_standard.egg-info/PKG-INFO` & `appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appengine-python-standard
-Version: 1.1.1
+Version: 1.1.2
 Summary: Google App Engine services SDK for Python 3
 Home-page: https://github.com/GoogleCloudPlatform/appengine-python-standard
 Author: Google LLC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
```

### Comparing `appengine-python-standard-1.1.1/src/appengine_python_standard.egg-info/SOURCES.txt` & `appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/__init__.py` & `appengine-python-standard-1.1.2/src/google/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/compat.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/compat.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/constants.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/constants.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/dfa.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/dfa.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/dottreegen.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/dottreegen.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/exceptions.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/exceptions.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/extras.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/extras.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/main.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/main.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/recognizers.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/recognizers.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/streams.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/streams.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/tokens.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/tokens.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/tree.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/tree.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/_internal/antlr3/treewizard.py` & `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/treewizard.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/api_base_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/api_base_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/api_testutil.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/api_testutil.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/apiproxy_rpc.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/apiproxy_rpc.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/apiproxy_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/apiproxy_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/apiproxy_stub_map.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/apiproxy_stub_map.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/_metadata_server.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/_metadata_server.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/app_identity.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/app_identity_defaultcredentialsbased_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_defaultcredentialsbased_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/app_identity_keybased_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_keybased_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/app_identity_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/app_identity_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/app_identity/app_identity_stub_base.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_stub_base.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/appinfo.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/appinfo.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/appinfo_errors.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/appinfo_errors.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/backendinfo.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/backendinfo.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/background_thread/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/background_thread/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/background_thread/background_thread.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/background_thread/background_thread.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/blob_storage.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blob_storage.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/blobstore.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/blobstore_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/blobstore_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/blobstore_stub_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore_stub_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/dict_blob_storage.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/dict_blob_storage.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/blobstore/file_blob_storage.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/file_blob_storage.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/capabilities/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/capabilities/capability_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/capability_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/capabilities/capability_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/capability_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/cmp_compat.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/cmp_compat.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/croninfo.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/croninfo.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/datastore.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/datastore.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/datastore_admin.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/datastore_admin.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/datastore_entities.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/datastore_entities.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/datastore_errors.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/datastore_errors.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/datastore_file_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/datastore_file_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/datastore_types.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/datastore_types.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/dispatchinfo.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/dispatchinfo.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/full_app_id.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/full_app_id.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/images/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/images/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/images/image_comparison.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/images/image_comparison.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/images/images_blob_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/images/images_blob_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/images/images_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/images/images_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/images/images_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/images/images_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/lib_config.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/lib_config.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/mail.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/mail.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/mail_errors.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/mail_errors.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/mail_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/mail_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/mail_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/mail_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/mail_stub_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/mail_stub_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/memcache/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/memcache/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/memcache/memcache_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/memcache/memcache_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/memcache/memcache_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/memcache/memcache_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/memcache/memcache_stub_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/memcache/memcache_stub_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/module_testutil.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/module_testutil.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/modules/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/modules/modules.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/modules/modules.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/modules/modules_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/modules/modules_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/modules/modules_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/modules/modules_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/namespace_manager/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/namespace_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/namespace_manager/namespace_manager.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/namespace_manager/namespace_manager.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/oauth/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/oauth/oauth_api.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/oauth/oauth_api.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/queueinfo.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/queueinfo.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/request_info.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/request_info.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/runtime/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/runtime/runtime.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/ExpressionLexer.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/ExpressionLexer.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/ExpressionParser.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/ExpressionParser.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/QueryLexer.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/QueryLexer.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/QueryParser.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/QueryParser.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/expression_parser.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/expression_parser.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/geo_util.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/geo_util.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/query_parser.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/query_parser.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/search.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/search.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/search_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/search_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/search_util.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/search_util.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/simple_search_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/simple_search_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/document_matcher.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/document_matcher.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/expression_evaluator.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/expression_evaluator.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/simple_facet.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/simple_facet.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/simple_tokenizer.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/stub/tokens.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/tokens.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/search/unicode_util.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/search/unicode_util.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/stublib.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/stublib.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/system/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/system/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/system/system_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/system/system_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/system/system_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/system/system_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/taskqueue/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/taskqueue/taskqueue.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/taskqueue.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/taskqueue/taskqueue_service_bytes_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/taskqueue_service_bytes_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/taskqueue/taskqueue_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/taskqueue_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/titanoboa_request_info.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/titanoboa_request_info.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/urlfetch.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/urlfetch_errors.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch_errors.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/urlfetch_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/urlfetch_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/user_service_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/user_service_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/user_service_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/users.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/users.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/validation.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/validation.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/yaml_builder.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/yaml_builder.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/yaml_errors.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/yaml_errors.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/yaml_listener.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/yaml_listener.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/yaml_object.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/yaml_object.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/api/yaml_test_util.py` & `appengine-python-standard-1.1.2/src/google/appengine/api/yaml_test_util.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/base/capabilities_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/base/capabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/action_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/action_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/cloud_datastore_v1_remote_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/cloud_datastore_v1_remote_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/cloud_datastore_v1_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/cloud_datastore_v1_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/cloud_datastore_validator.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/cloud_datastore_validator.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_index.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_index.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_index_xml.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_index_xml.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_pb.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_pb.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_pbs.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_pbs.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_query.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_query.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_rpc.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_rpc.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_stub_index.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_stub_index.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_stub_util.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_stub_util.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_v3_bytes_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v3_bytes_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_v4_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v4_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_v4_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v4_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/datastore_v4_validator.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v4_validator.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/document_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/document_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/entity_bytes_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/entity_bytes_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/entity_v4_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/entity_v4_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/snapshot_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/datastore/sortable_pb_encoder.py` & `appengine-python-standard-1.1.2/src/google/appengine/datastore/sortable_pb_encoder.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/blobstore/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/blobstore/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/blobstore/blobstore.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/blobstore/blobstore.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/db/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/db/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/db/metadata.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/db/metadata.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/db/polymodel.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/db/polymodel.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/db/stats.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/db/stats.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/db/sync.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/db/sync.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/deferred/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/deferred/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/deferred/deferred.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/deferred/deferred.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/gql/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/key_range/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/key_range/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/blobstore.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/blobstore.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/context.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/context.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/django_middleware.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/django_middleware.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/eventloop.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/eventloop.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/key.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/key.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/key_test.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/key_test.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/metadata.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/metadata.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/model.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -6118,2042 +6118,2064 @@
 00017e50: 6574 7572 6e20 6b77 6473 2e70 6f70 286b  eturn kwds.pop(k
 00017e60: 7764 290a 2020 2020 7265 7475 726e 204e  wd).    return N
 00017e70: 6f6e 650a 0a20 2064 6566 205f 5f67 6574  one..  def __get
 00017e80: 7374 6174 655f 5f28 7365 6c66 293a 0a20  state__(self):. 
 00017e90: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
 00017ea0: 746f 5f70 6228 292e 5365 7269 616c 697a  to_pb().Serializ
 00017eb0: 6554 6f53 7472 696e 6728 290a 0a20 2064  eToString()..  d
-00017ec0: 6566 205f 5f73 6574 7374 6174 655f 5f28  ef __setstate__(
-00017ed0: 7365 6c66 2c20 7365 7269 616c 697a 6564  self, serialized
-00017ee0: 5f70 6229 3a0a 2020 2020 7062 203d 2065  _pb):.    pb = e
-00017ef0: 6e74 6974 795f 7062 322e 456e 7469 7479  ntity_pb2.Entity
-00017f00: 5072 6f74 6f2e 4672 6f6d 5374 7269 6e67  Proto.FromString
-00017f10: 2873 6572 6961 6c69 7a65 645f 7062 290a  (serialized_pb).
-00017f20: 2020 2020 7365 6c66 2e5f 5f69 6e69 745f      self.__init_
-00017f30: 5f28 290a 2020 2020 7365 6c66 2e5f 5f63  _().    self.__c
-00017f40: 6c61 7373 5f5f 2e5f 6672 6f6d 5f70 6228  lass__._from_pb(
-00017f50: 7062 2c20 7365 745f 6b65 793d 4661 6c73  pb, set_key=Fals
-00017f60: 652c 2065 6e74 3d73 656c 6629 0a0a 2020  e, ent=self)..  
-00017f70: 6465 6620 5f70 6f70 756c 6174 6528 7365  def _populate(se
-00017f80: 6c66 2c20 2a2a 6b77 6473 293a 0a20 2020  lf, **kwds):.   
-00017f90: 2022 2222 506f 7075 6c61 7465 2061 6e20   """Populate an 
-00017fa0: 696e 7374 616e 6365 2066 726f 6d20 6b65  instance from ke
-00017fb0: 7977 6f72 6420 6172 6775 6d65 6e74 732e  yword arguments.
-00017fc0: 0a0a 2020 2020 4561 6368 206b 6579 776f  ..    Each keywo
-00017fd0: 7264 2061 7267 756d 656e 7420 7769 6c6c  rd argument will
-00017fe0: 2062 6520 7573 6564 2074 6f20 7365 7420   be used to set 
-00017ff0: 6120 636f 7272 6573 706f 6e64 696e 670a  a corresponding.
-00018000: 2020 2020 7072 6f70 6572 7479 2e20 204b      property.  K
-00018010: 6579 776f 7264 7320 6d75 7374 2072 6566  eywords must ref
-00018020: 6572 2074 6f20 7661 6c69 6420 7072 6f70  er to valid prop
-00018030: 6572 7479 206e 616d 652e 2020 5468 6973  erty name.  This
-00018040: 2069 730a 2020 2020 7369 6d69 6c61 7220   is.    similar 
-00018050: 746f 2070 6173 7369 6e67 206b 6579 776f  to passing keywo
-00018060: 7264 2061 7267 756d 656e 7473 2074 6f20  rd arguments to 
-00018070: 7468 6520 4d6f 6465 6c20 636f 6e73 7472  the Model constr
-00018080: 7563 746f 722c 0a20 2020 2065 7863 6570  uctor,.    excep
-00018090: 7420 7468 6174 206e 6f20 7072 6f76 6973  t that no provis
-000180a0: 696f 6e73 2066 6f72 206b 6579 2c20 6964  ions for key, id
-000180b0: 206f 7220 7061 7265 6e74 2061 7265 206d   or parent are m
-000180c0: 6164 652e 0a20 2020 2022 2222 0a20 2020  ade..    """.   
-000180d0: 2073 656c 662e 5f73 6574 5f61 7474 7269   self._set_attri
-000180e0: 6275 7465 7328 6b77 6473 290a 2020 706f  butes(kwds).  po
-000180f0: 7075 6c61 7465 203d 205f 706f 7075 6c61  pulate = _popula
-00018100: 7465 0a0a 2020 6465 6620 5f73 6574 5f61  te..  def _set_a
-00018110: 7474 7269 6275 7465 7328 7365 6c66 2c20  ttributes(self, 
-00018120: 6b77 6473 293a 0a20 2020 2022 2222 496e  kwds):.    """In
-00018130: 7465 726e 616c 2068 656c 7065 7220 746f  ternal helper to
-00018140: 2073 6574 2061 7474 7269 6275 7465 7320   set attributes 
-00018150: 6672 6f6d 206b 6579 776f 7264 2061 7267  from keyword arg
-00018160: 756d 656e 7473 2e0a 0a20 2020 2045 7870  uments...    Exp
-00018170: 616e 646f 206f 7665 7272 6964 6573 2074  ando overrides t
-00018180: 6869 732e 0a20 2020 2022 2222 0a20 2020  his..    """.   
-00018190: 2063 6c73 203d 2073 656c 662e 5f5f 636c   cls = self.__cl
-000181a0: 6173 735f 5f0a 2020 2020 666f 7220 6e61  ass__.    for na
-000181b0: 6d65 2c20 7661 6c75 6520 696e 2073 6978  me, value in six
-000181c0: 2e69 7465 7269 7465 6d73 286b 7764 7329  .iteritems(kwds)
-000181d0: 3a0a 2020 2020 2020 7072 6f70 203d 2067  :.      prop = g
-000181e0: 6574 6174 7472 2863 6c73 2c20 6e61 6d65  etattr(cls, name
-000181f0: 290a 2020 2020 2020 6966 206e 6f74 2069  ).      if not i
-00018200: 7369 6e73 7461 6e63 6528 7072 6f70 2c20  sinstance(prop, 
-00018210: 5072 6f70 6572 7479 293a 0a20 2020 2020  Property):.     
-00018220: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
-00018230: 6f72 2827 4361 6e6e 6f74 2073 6574 206e  or('Cannot set n
-00018240: 6f6e 2d70 726f 7065 7274 7920 2573 2720  on-property %s' 
-00018250: 2520 6e61 6d65 290a 2020 2020 2020 7072  % name).      pr
-00018260: 6f70 2e5f 7365 745f 7661 6c75 6528 7365  op._set_value(se
-00018270: 6c66 2c20 7661 6c75 6529 0a0a 2020 6465  lf, value)..  de
-00018280: 6620 5f66 696e 645f 756e 696e 6974 6961  f _find_uninitia
-00018290: 6c69 7a65 6428 7365 6c66 293a 0a20 2020  lized(self):.   
-000182a0: 2022 2222 496e 7465 726e 616c 2068 656c   """Internal hel
-000182b0: 7065 7220 746f 2066 696e 6420 756e 696e  per to find unin
-000182c0: 6974 6961 6c69 7a65 6420 7072 6f70 6572  itialized proper
-000182d0: 7469 6573 2e0a 0a20 2020 2052 6574 7572  ties...    Retur
-000182e0: 6e73 3a0a 2020 2020 2020 4120 7365 7420  ns:.      A set 
-000182f0: 6f66 2070 726f 7065 7274 7920 6e61 6d65  of property name
-00018300: 732e 0a20 2020 2022 2222 0a20 2020 2072  s..    """.    r
-00018310: 6574 7572 6e20 7365 7428 6e61 6d65 2066  eturn set(name f
-00018320: 6f72 206e 616d 652c 2070 726f 7020 696e  or name, prop in
-00018330: 2073 6978 2e69 7465 7269 7465 6d73 2873   six.iteritems(s
-00018340: 656c 662e 5f70 726f 7065 7274 6965 7329  elf._properties)
-00018350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018360: 6966 206e 6f74 2070 726f 702e 5f69 735f  if not prop._is_
-00018370: 696e 6974 6961 6c69 7a65 6428 7365 6c66  initialized(self
-00018380: 2929 0a0a 2020 6465 6620 5f63 6865 636b  ))..  def _check
-00018390: 5f69 6e69 7469 616c 697a 6564 2873 656c  _initialized(sel
-000183a0: 6629 3a0a 2020 2020 2222 2249 6e74 6572  f):.    """Inter
-000183b0: 6e61 6c20 6865 6c70 6572 2074 6f20 6368  nal helper to ch
-000183c0: 6563 6b20 666f 7220 756e 696e 6974 6961  eck for uninitia
-000183d0: 6c69 7a65 6420 7072 6f70 6572 7469 6573  lized properties
-000183e0: 2e0a 0a20 2020 2052 6169 7365 733a 0a20  ...    Raises:. 
-000183f0: 2020 2020 2042 6164 5661 6c75 6545 7272       BadValueErr
-00018400: 6f72 2069 6620 6974 2066 696e 6473 2061  or if it finds a
-00018410: 6e79 2e0a 2020 2020 2222 220a 2020 2020  ny..    """.    
-00018420: 6261 6464 6965 7320 3d20 7365 6c66 2e5f  baddies = self._
-00018430: 6669 6e64 5f75 6e69 6e69 7469 616c 697a  find_uninitializ
-00018440: 6564 2829 0a20 2020 2069 6620 6261 6464  ed().    if badd
-00018450: 6965 733a 0a20 2020 2020 2072 6169 7365  ies:.      raise
-00018460: 2064 6174 6173 746f 7265 5f65 7272 6f72   datastore_error
-00018470: 732e 4261 6456 616c 7565 4572 726f 7228  s.BadValueError(
-00018480: 0a20 2020 2020 2020 2020 2027 456e 7469  .          'Enti
-00018490: 7479 2068 6173 2075 6e69 6e69 7469 616c  ty has uninitial
-000184a0: 697a 6564 2070 726f 7065 7274 6965 733a  ized properties:
-000184b0: 2025 7327 2025 2027 2c20 272e 6a6f 696e   %s' % ', '.join
-000184c0: 2862 6164 6469 6573 2929 0a0a 2020 6465  (baddies))..  de
-000184d0: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
-000184e0: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
-000184f0: 616e 2075 6e61 6d62 6967 756f 7573 2073  an unambiguous s
-00018500: 7472 696e 6720 7265 7072 6573 656e 7461  tring representa
-00018510: 7469 6f6e 206f 6620 616e 2065 6e74 6974  tion of an entit
-00018520: 792e 2222 220a 2020 2020 6172 6773 203d  y.""".    args =
-00018530: 205b 5d0a 2020 2020 666f 7220 7072 6f70   [].    for prop
-00018540: 2069 6e20 7369 782e 6974 6572 7661 6c75   in six.itervalu
-00018550: 6573 2873 656c 662e 5f70 726f 7065 7274  es(self._propert
-00018560: 6965 7329 3a0a 2020 2020 2020 6966 2070  ies):.      if p
-00018570: 726f 702e 5f68 6173 5f76 616c 7565 2873  rop._has_value(s
-00018580: 656c 6629 3a0a 2020 2020 2020 2020 7661  elf):.        va
-00018590: 6c20 3d20 7072 6f70 2e5f 7265 7472 6965  l = prop._retrie
-000185a0: 7665 5f76 616c 7565 2873 656c 6629 0a20  ve_value(self). 
-000185b0: 2020 2020 2020 2069 6620 7661 6c20 6973         if val is
-000185c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000185d0: 2072 6570 203d 2027 4e6f 6e65 270a 2020   rep = 'None'.  
-000185e0: 2020 2020 2020 656c 6966 2070 726f 702e        elif prop.
-000185f0: 5f72 6570 6561 7465 643a 0a20 2020 2020  _repeated:.     
-00018600: 2020 2020 2072 6570 7273 203d 205b 7072       reprs = [pr
-00018610: 6f70 2e5f 7661 6c75 655f 746f 5f72 6570  op._value_to_rep
-00018620: 7228 7629 2066 6f72 2076 2069 6e20 7661  r(v) for v in va
-00018630: 6c5d 0a20 2020 2020 2020 2020 2069 6620  l].          if 
-00018640: 7265 7072 733a 0a20 2020 2020 2020 2020  reprs:.         
-00018650: 2020 2072 6570 7273 5b30 5d20 3d20 275b     reprs[0] = '[
-00018660: 2720 2b20 7265 7072 735b 305d 0a20 2020  ' + reprs[0].   
-00018670: 2020 2020 2020 2020 2072 6570 7273 5b2d           reprs[-
-00018680: 315d 203d 2072 6570 7273 5b2d 315d 202b  1] = reprs[-1] +
-00018690: 2027 5d27 0a20 2020 2020 2020 2020 2020   ']'.           
-000186a0: 2072 6570 203d 2027 2c20 272e 6a6f 696e   rep = ', '.join
-000186b0: 2872 6570 7273 290a 2020 2020 2020 2020  (reprs).        
-000186c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000186d0: 2020 2020 7265 7020 3d20 275b 5d27 0a20      rep = '[]'. 
-000186e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000186f0: 2020 2020 2020 2072 6570 203d 2070 726f         rep = pro
-00018700: 702e 5f76 616c 7565 5f74 6f5f 7265 7072  p._value_to_repr
-00018710: 2876 616c 290a 2020 2020 2020 2020 6172  (val).        ar
-00018720: 6773 2e61 7070 656e 6428 2725 733d 2573  gs.append('%s=%s
-00018730: 2720 2520 2870 726f 702e 5f63 6f64 655f  ' % (prop._code_
-00018740: 6e61 6d65 2c20 7265 7029 290a 2020 2020  name, rep)).    
-00018750: 6172 6773 2e73 6f72 7428 290a 2020 2020  args.sort().    
-00018760: 6966 2073 656c 662e 5f6b 6579 2069 7320  if self._key is 
-00018770: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00018780: 6172 6773 2e69 6e73 6572 7428 302c 2027  args.insert(0, '
-00018790: 6b65 793d 2572 2720 2520 7365 6c66 2e5f  key=%r' % self._
-000187a0: 6b65 7929 0a20 2020 2069 6620 7365 6c66  key).    if self
-000187b0: 2e5f 7072 6f6a 6563 7469 6f6e 3a0a 2020  ._projection:.  
-000187c0: 2020 2020 6172 6773 2e61 7070 656e 6428      args.append(
-000187d0: 275f 7072 6f6a 6563 7469 6f6e 3d25 7227  '_projection=%r'
-000187e0: 2025 2028 7365 6c66 2e5f 7072 6f6a 6563   % (self._projec
-000187f0: 7469 6f6e 2c29 290a 2020 2020 7320 3d20  tion,)).    s = 
-00018800: 2725 7328 2573 2927 2025 2028 7365 6c66  '%s(%s)' % (self
-00018810: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
-00018820: 655f 5f2c 2027 2c20 272e 6a6f 696e 2861  e__, ', '.join(a
-00018830: 7267 7329 290a 2020 2020 7265 7475 726e  rgs)).    return
-00018840: 2073 0a0a 2020 4063 6c61 7373 6d65 7468   s..  @classmeth
-00018850: 6f64 0a20 2064 6566 205f 6765 745f 6b69  od.  def _get_ki
-00018860: 6e64 2863 6c73 293a 0a20 2020 2022 2222  nd(cls):.    """
-00018870: 5265 7475 726e 2074 6865 206b 696e 6420  Return the kind 
-00018880: 6e61 6d65 2066 6f72 2074 6869 7320 636c  name for this cl
-00018890: 6173 732e 0a0a 2020 2020 5468 6973 2064  ass...    This d
-000188a0: 6566 6175 6c74 7320 746f 2063 6c73 2e5f  efaults to cls._
-000188b0: 5f6e 616d 655f 5f3b 2075 7365 7273 206d  _name__; users m
-000188c0: 6179 206f 7665 7272 6964 2074 6869 7320  ay overrid this 
-000188d0: 746f 2067 6976 6520 610a 2020 2020 636c  to give a.    cl
-000188e0: 6173 7320 6120 6469 6666 6572 656e 7420  ass a different 
-000188f0: 6f6e 2d64 6973 6b20 6e61 6d65 2074 6861  on-disk name tha
-00018900: 6e20 6974 7320 636c 6173 7320 6e61 6d65  n its class name
-00018910: 2e0a 2020 2020 2222 220a 2020 2020 7265  ..    """.    re
-00018920: 7475 726e 2063 6c73 2e5f 5f6e 616d 655f  turn cls.__name_
-00018930: 5f0a 0a20 2040 636c 6173 736d 6574 686f  _..  @classmetho
-00018940: 640a 2020 6465 6620 5f63 6c61 7373 5f6e  d.  def _class_n
-00018950: 616d 6528 636c 7329 3a0a 2020 2020 2222  ame(cls):.    ""
-00018960: 2241 2068 6f6f 6b20 666f 7220 706f 6c79  "A hook for poly
-00018970: 6d6f 6465 6c20 746f 206f 7665 7272 6964  model to overrid
-00018980: 652e 0a0a 2020 2020 466f 7220 7265 6775  e...    For regu
-00018990: 6c61 7220 6d6f 6465 6c73 2061 6e64 2065  lar models and e
-000189a0: 7870 616e 646f 7320 7468 6973 2069 7320  xpandos this is 
-000189b0: 6a75 7374 2061 6e20 616c 6961 7320 666f  just an alias fo
-000189c0: 720a 2020 2020 5f67 6574 5f6b 696e 6428  r.    _get_kind(
-000189d0: 292e 2020 466f 7220 506f 6c79 4d6f 6465  ).  For PolyMode
-000189e0: 6c20 7375 6263 6c61 7373 6573 2c20 6974  l subclasses, it
-000189f0: 2072 6574 7572 6e73 2074 6865 2063 6c61   returns the cla
-00018a00: 7373 206e 616d 650a 2020 2020 2861 7320  ss name.    (as 
-00018a10: 7365 7420 696e 2074 6865 2027 636c 6173  set in the 'clas
-00018a20: 7327 2061 7474 7269 6275 7465 2074 6865  s' attribute the
-00018a30: 7265 6f66 292c 2077 6865 7265 6173 205f  reof), whereas _
-00018a40: 6765 745f 6b69 6e64 2829 0a20 2020 2072  get_kind().    r
-00018a50: 6574 7572 6e73 2074 6865 206b 696e 6420  eturns the kind 
-00018a60: 2874 6865 2063 6c61 7373 206e 616d 6520  (the class name 
-00018a70: 6f66 2074 6865 2072 6f6f 7420 636c 6173  of the root clas
-00018a80: 7320 6f66 2061 2073 7065 6369 6669 630a  s of a specific.
-00018a90: 2020 2020 506f 6c79 4d6f 6465 6c20 6869      PolyModel hi
-00018aa0: 6572 6172 6368 7929 2e0a 2020 2020 2222  erarchy)..    ""
-00018ab0: 220a 2020 2020 7265 7475 726e 2063 6c73  ".    return cls
-00018ac0: 2e5f 6765 745f 6b69 6e64 2829 0a0a 2020  ._get_kind()..  
-00018ad0: 4063 6c61 7373 6d65 7468 6f64 0a20 2064  @classmethod.  d
-00018ae0: 6566 205f 6465 6661 756c 745f 6669 6c74  ef _default_filt
-00018af0: 6572 7328 636c 7329 3a0a 2020 2020 2222  ers(cls):.    ""
-00018b00: 2252 6574 7572 6e20 616e 2069 7465 7261  "Return an itera
-00018b10: 626c 6520 6f66 2066 696c 7465 7273 2074  ble of filters t
-00018b20: 6861 7420 6172 6520 616c 7761 7973 2074  hat are always t
-00018b30: 6f20 6265 2061 7070 6c69 6564 2e0a 0a20  o be applied... 
-00018b40: 2020 2054 6869 7320 6973 2075 7365 6420     This is used 
-00018b50: 6279 2050 6f6c 794d 6f64 656c 2074 6f20  by PolyModel to 
-00018b60: 7175 6965 746c 7920 696e 7365 7274 2061  quietly insert a
-00018b70: 2066 696c 7465 7220 666f 7220 7468 650a   filter for the.
-00018b80: 2020 2020 6375 7272 656e 7420 636c 6173      current clas
-00018b90: 7320 6e61 6d65 2e0a 2020 2020 2222 220a  s name..    """.
-00018ba0: 2020 2020 7265 7475 726e 2028 290a 0a20      return ().. 
-00018bb0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00018bc0: 6465 6620 5f72 6573 6574 5f6b 696e 645f  def _reset_kind_
-00018bd0: 6d61 7028 636c 7329 3a0a 2020 2020 2222  map(cls):.    ""
-00018be0: 2243 6c65 6172 2074 6865 206b 696e 6420  "Clear the kind 
-00018bf0: 6d61 702e 2020 5573 6566 756c 2066 6f72  map.  Useful for
-00018c00: 2074 6573 7469 6e67 2e22 2222 0a0a 2020   testing."""..  
-00018c10: 2020 6b65 6570 203d 207b 7d0a 2020 2020    keep = {}.    
-00018c20: 666f 7220 6e61 6d65 2c20 7661 6c75 6520  for name, value 
-00018c30: 696e 2073 6978 2e69 7465 7269 7465 6d73  in six.iteritems
-00018c40: 2863 6c73 2e5f 6b69 6e64 5f6d 6170 293a  (cls._kind_map):
-00018c50: 0a20 2020 2020 2069 6620 6e61 6d65 2e73  .      if name.s
-00018c60: 7461 7274 7377 6974 6828 275f 5f27 2920  tartswith('__') 
-00018c70: 616e 6420 6e61 6d65 2e65 6e64 7377 6974  and name.endswit
-00018c80: 6828 275f 5f27 293a 0a20 2020 2020 2020  h('__'):.       
-00018c90: 206b 6565 705b 6e61 6d65 5d20 3d20 7661   keep[name] = va
-00018ca0: 6c75 650a 2020 2020 636c 732e 5f6b 696e  lue.    cls._kin
-00018cb0: 645f 6d61 702e 636c 6561 7228 290a 2020  d_map.clear().  
-00018cc0: 2020 636c 732e 5f6b 696e 645f 6d61 702e    cls._kind_map.
-00018cd0: 7570 6461 7465 286b 6565 7029 0a0a 2020  update(keep)..  
-00018ce0: 4063 6c61 7373 6d65 7468 6f64 0a20 2064  @classmethod.  d
-00018cf0: 6566 205f 6c6f 6f6b 7570 5f6d 6f64 656c  ef _lookup_model
-00018d00: 2863 6c73 2c20 6b69 6e64 2c20 6465 6661  (cls, kind, defa
-00018d10: 756c 745f 6d6f 6465 6c3d 4e6f 6e65 293a  ult_model=None):
-00018d20: 0a20 2020 2022 2222 4765 7420 7468 6520  .    """Get the 
-00018d30: 6d6f 6465 6c20 636c 6173 7320 666f 7220  model class for 
-00018d40: 7468 6520 6b69 6e64 2e0a 0a20 2020 2041  the kind...    A
-00018d50: 7267 733a 0a20 2020 2020 206b 696e 643a  rgs:.      kind:
-00018d60: 2041 2073 7472 696e 6720 7265 7072 6573   A string repres
-00018d70: 656e 7469 6e67 2074 6865 206e 616d 6520  enting the name 
-00018d80: 6f66 2074 6865 206b 696e 6420 746f 206c  of the kind to l
-00018d90: 6f6f 6b75 702e 0a20 2020 2020 2064 6566  ookup..      def
-00018da0: 6175 6c74 5f6d 6f64 656c 3a20 5468 6520  ault_model: The 
-00018db0: 6d6f 6465 6c20 636c 6173 7320 746f 2075  model class to u
-00018dc0: 7365 2069 6620 7468 6520 6b69 6e64 2063  se if the kind c
-00018dd0: 616e 2774 2062 6520 666f 756e 642e 0a0a  an't be found...
-00018de0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00018df0: 2020 2054 6865 206d 6f64 656c 2063 6c61     The model cla
-00018e00: 7373 2066 6f72 2074 6865 2072 6571 7565  ss for the reque
-00018e10: 7374 6564 206b 696e 642e 0a20 2020 2052  sted kind..    R
-00018e20: 6169 7365 733a 0a20 2020 2020 204b 696e  aises:.      Kin
-00018e30: 6445 7272 6f72 3a20 5468 6520 6b69 6e64  dError: The kind
-00018e40: 2077 6173 206e 6f74 2066 6f75 6e64 2061   was not found a
-00018e50: 6e64 206e 6f20 6465 6661 756c 745f 6d6f  nd no default_mo
-00018e60: 6465 6c20 7761 7320 7072 6f76 6964 6564  del was provided
-00018e70: 2e0a 2020 2020 2222 220a 2020 2020 6d6f  ..    """.    mo
-00018e80: 6465 6c63 6c61 7373 203d 2063 6c73 2e5f  delclass = cls._
-00018e90: 6b69 6e64 5f6d 6170 2e67 6574 286b 696e  kind_map.get(kin
-00018ea0: 642c 2064 6566 6175 6c74 5f6d 6f64 656c  d, default_model
-00018eb0: 290a 2020 2020 6966 206d 6f64 656c 636c  ).    if modelcl
-00018ec0: 6173 7320 6973 204e 6f6e 653a 0a20 2020  ass is None:.   
-00018ed0: 2020 2072 6169 7365 204b 696e 6445 7272     raise KindErr
-00018ee0: 6f72 280a 2020 2020 2020 2020 2020 224e  or(.          "N
-00018ef0: 6f20 6d6f 6465 6c20 636c 6173 7320 666f  o model class fo
-00018f00: 756e 6420 666f 7220 6b69 6e64 2027 2573  und for kind '%s
-00018f10: 272e 2044 6964 2079 6f75 2066 6f72 6765  '. Did you forge
-00018f20: 7420 746f 2069 6d70 6f72 7420 6974 3f22  t to import it?"
-00018f30: 2025 0a20 2020 2020 2020 2020 206b 696e   %.          kin
-00018f40: 6429 0a20 2020 2072 6574 7572 6e20 6d6f  d).    return mo
-00018f50: 6465 6c63 6c61 7373 0a0a 2020 6465 6620  delclass..  def 
-00018f60: 5f68 6173 5f63 6f6d 706c 6574 655f 6b65  _has_complete_ke
-00018f70: 7928 7365 6c66 293a 0a20 2020 2022 2222  y(self):.    """
-00018f80: 5265 7475 726e 2077 6865 7468 6572 2074  Return whether t
-00018f90: 6869 7320 656e 7469 7479 2068 6173 2061  his entity has a
-00018fa0: 2063 6f6d 706c 6574 6520 6b65 792e 2222   complete key.""
-00018fb0: 220a 2020 2020 7265 7475 726e 2073 656c  ".    return sel
-00018fc0: 662e 5f6b 6579 2069 7320 6e6f 7420 4e6f  f._key is not No
-00018fd0: 6e65 2061 6e64 2073 656c 662e 5f6b 6579  ne and self._key
-00018fe0: 2e69 6428 2920 6973 206e 6f74 204e 6f6e  .id() is not Non
-00018ff0: 650a 2020 6861 735f 636f 6d70 6c65 7465  e.  has_complete
-00019000: 5f6b 6579 203d 205f 6861 735f 636f 6d70  _key = _has_comp
-00019010: 6c65 7465 5f6b 6579 0a0a 2020 6465 6620  lete_key..  def 
-00019020: 5f5f 6861 7368 5f5f 2873 656c 6629 3a0a  __hash__(self):.
-00019030: 2020 2020 2222 2244 756d 6d79 2068 6173      """Dummy has
-00019040: 6820 6675 6e63 7469 6f6e 2e0a 0a20 2020  h function...   
-00019050: 2052 6169 7365 733a 0a20 2020 2020 2041   Raises:.      A
-00019060: 6c77 6179 7320 5479 7065 4572 726f 7220  lways TypeError 
-00019070: 746f 2065 6d70 6861 7369 7a65 2074 6861  to emphasize tha
-00019080: 7420 656e 7469 7469 6573 2061 7265 206d  t entities are m
-00019090: 7574 6162 6c65 2e0a 2020 2020 2222 220a  utable..    """.
-000190a0: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
-000190b0: 726f 7228 274d 6f64 656c 2069 7320 6e6f  ror('Model is no
-000190c0: 7420 696d 6d75 7461 626c 6527 290a 0a0a  t immutable')...
-000190d0: 0a20 2064 6566 205f 5f65 715f 5f28 7365  .  def __eq__(se
-000190e0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
-000190f0: 2222 2243 6f6d 7061 7265 2074 776f 2065  """Compare two e
-00019100: 6e74 6974 6965 7320 6f66 2074 6865 2073  ntities of the s
-00019110: 616d 6520 636c 6173 7320 666f 7220 6571  ame class for eq
-00019120: 7561 6c69 7479 2e22 2222 0a20 2020 2069  uality.""".    i
-00019130: 6620 6f74 6865 722e 5f5f 636c 6173 735f  f other.__class_
-00019140: 5f20 6973 206e 6f74 2073 656c 662e 5f5f  _ is not self.__
-00019150: 636c 6173 735f 5f3a 0a20 2020 2020 2072  class__:.      r
-00019160: 6574 7572 6e20 4e6f 7449 6d70 6c65 6d65  eturn NotImpleme
-00019170: 6e74 6564 0a20 2020 2069 6620 7365 6c66  nted.    if self
-00019180: 2e5f 6b65 7920 213d 206f 7468 6572 2e5f  ._key != other._
-00019190: 6b65 793a 0a0a 0a20 2020 2020 2072 6574  key:...      ret
-000191a0: 7572 6e20 4661 6c73 650a 2020 2020 7265  urn False.    re
-000191b0: 7475 726e 2073 656c 662e 5f65 7175 6976  turn self._equiv
-000191c0: 616c 656e 7428 6f74 6865 7229 0a0a 2020  alent(other)..  
-000191d0: 6465 6620 5f65 7175 6976 616c 656e 7428  def _equivalent(
-000191e0: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
-000191f0: 2020 2222 2243 6f6d 7061 7265 2074 776f    """Compare two
-00019200: 2065 6e74 6974 6965 7320 6f66 2074 6865   entities of the
-00019210: 2073 616d 6520 636c 6173 732c 2065 7863   same class, exc
-00019220: 6c75 6469 6e67 206b 6579 732e 2222 220a  luding keys.""".
-00019230: 2020 2020 6966 206f 7468 6572 2e5f 5f63      if other.__c
-00019240: 6c61 7373 5f5f 2069 7320 6e6f 7420 7365  lass__ is not se
-00019250: 6c66 2e5f 5f63 6c61 7373 5f5f 3a0a 2020  lf.__class__:.  
-00019260: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-00019270: 6c65 6d65 6e74 6564 4572 726f 7228 2743  lementedError('C
-00019280: 616e 6e6f 7420 636f 6d70 6172 6520 6469  annot compare di
-00019290: 6666 6572 656e 7420 6d6f 6465 6c20 636c  fferent model cl
-000192a0: 6173 7365 732e 2027 0a20 2020 2020 2020  asses. '.       
-000192b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192c0: 2020 2020 2020 2020 2027 2573 2069 7320           '%s is 
-000192d0: 6e6f 7420 2573 2720 2520 2873 656c 662e  not %s' % (self.
-000192e0: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
-000192f0: 5f5f 2c0a 2020 2020 2020 2020 2020 2020  __,.            
-00019300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019320: 2020 2020 2020 6f74 6865 722e 5f5f 636c        other.__cl
-00019330: 6173 735f 2e5f 5f6e 616d 655f 5f29 290a  ass_.__name__)).
-00019340: 2020 2020 6966 2073 6574 2873 656c 662e      if set(self.
-00019350: 5f70 726f 6a65 6374 696f 6e29 2021 3d20  _projection) != 
-00019360: 7365 7428 6f74 6865 722e 5f70 726f 6a65  set(other._proje
-00019370: 6374 696f 6e29 3a0a 2020 2020 2020 7265  ction):.      re
-00019380: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
-00019390: 6966 206c 656e 2873 656c 662e 5f70 726f  if len(self._pro
-000193a0: 7065 7274 6965 7329 2021 3d20 6c65 6e28  perties) != len(
-000193b0: 6f74 6865 722e 5f70 726f 7065 7274 6965  other._propertie
-000193c0: 7329 3a0a 2020 2020 2020 7265 7475 726e  s):.      return
-000193d0: 2046 616c 7365 0a20 2020 206d 795f 7072   False.    my_pr
-000193e0: 6f70 5f6e 616d 6573 203d 2073 6574 2873  op_names = set(s
-000193f0: 6978 2e69 7465 726b 6579 7328 7365 6c66  ix.iterkeys(self
-00019400: 2e5f 7072 6f70 6572 7469 6573 2929 0a20  ._properties)). 
-00019410: 2020 2074 6865 6972 5f70 726f 705f 6e61     their_prop_na
-00019420: 6d65 7320 3d20 7365 7428 7369 782e 6974  mes = set(six.it
-00019430: 6572 6b65 7973 286f 7468 6572 2e5f 7072  erkeys(other._pr
-00019440: 6f70 6572 7469 6573 2929 0a20 2020 2069  operties)).    i
-00019450: 6620 6d79 5f70 726f 705f 6e61 6d65 7320  f my_prop_names 
-00019460: 213d 2074 6865 6972 5f70 726f 705f 6e61  != their_prop_na
-00019470: 6d65 733a 0a20 2020 2020 2072 6574 7572  mes:.      retur
-00019480: 6e20 4661 6c73 650a 2020 2020 6966 2073  n False.    if s
-00019490: 656c 662e 5f70 726f 6a65 6374 696f 6e3a  elf._projection:
-000194a0: 0a20 2020 2020 206d 795f 7072 6f70 5f6e  .      my_prop_n
-000194b0: 616d 6573 203d 2073 6574 2873 656c 662e  ames = set(self.
-000194c0: 5f70 726f 6a65 6374 696f 6e29 0a20 2020  _projection).   
-000194d0: 2066 6f72 206e 616d 6520 696e 206d 795f   for name in my_
-000194e0: 7072 6f70 5f6e 616d 6573 3a0a 2020 2020  prop_names:.    
-000194f0: 2020 6e61 6d65 203d 2073 6978 2e65 6e73    name = six.ens
-00019500: 7572 655f 7465 7874 286e 616d 6529 0a20  ure_text(name). 
-00019510: 2020 2020 2069 6620 272e 2720 696e 206e       if '.' in n
-00019520: 616d 653a 0a20 2020 2020 2020 206e 616d  ame:.        nam
-00019530: 652c 205f 203d 206e 616d 652e 7370 6c69  e, _ = name.spli
-00019540: 7428 272e 272c 2031 290a 2020 2020 2020  t('.', 1).      
-00019550: 6d79 5f76 616c 7565 203d 2073 656c 662e  my_value = self.
-00019560: 5f70 726f 7065 7274 6965 735b 6e61 6d65  _properties[name
-00019570: 5d2e 5f67 6574 5f76 616c 7565 2873 656c  ]._get_value(sel
-00019580: 6629 0a20 2020 2020 2074 6865 6972 5f76  f).      their_v
-00019590: 616c 7565 203d 206f 7468 6572 2e5f 7072  alue = other._pr
-000195a0: 6f70 6572 7469 6573 5b6e 616d 655d 2e5f  operties[name]._
-000195b0: 6765 745f 7661 6c75 6528 6f74 6865 7229  get_value(other)
-000195c0: 0a20 2020 2020 2069 6620 6d79 5f76 616c  .      if my_val
-000195d0: 7565 2021 3d20 7468 6569 725f 7661 6c75  ue != their_valu
-000195e0: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
-000195f0: 6e20 4661 6c73 650a 2020 2020 7265 7475  n False.    retu
-00019600: 726e 2054 7275 650a 0a20 2064 6566 205f  rn True..  def _
-00019610: 746f 5f70 6228 7365 6c66 2c20 7062 3d4e  to_pb(self, pb=N
-00019620: 6f6e 652c 2061 6c6c 6f77 5f70 6172 7469  one, allow_parti
-00019630: 616c 3d46 616c 7365 2c20 7365 745f 6b65  al=False, set_ke
-00019640: 793d 5472 7565 293a 0a20 2020 2022 2222  y=True):.    """
-00019650: 496e 7465 726e 616c 2068 656c 7065 7220  Internal helper 
-00019660: 746f 2074 7572 6e20 616e 2065 6e74 6974  to turn an entit
-00019670: 7920 696e 746f 2061 6e20 456e 7469 7479  y into an Entity
-00019680: 5072 6f74 6f20 7072 6f74 6f62 7566 2e22  Proto protobuf."
-00019690: 2222 0a20 2020 2069 6620 6e6f 7420 616c  "".    if not al
-000196a0: 6c6f 775f 7061 7274 6961 6c3a 0a20 2020  low_partial:.   
-000196b0: 2020 2073 656c 662e 5f63 6865 636b 5f69     self._check_i
-000196c0: 6e69 7469 616c 697a 6564 2829 0a20 2020  nitialized().   
-000196d0: 2069 6620 7062 2069 7320 4e6f 6e65 3a0a   if pb is None:.
-000196e0: 2020 2020 2020 7062 203d 2065 6e74 6974        pb = entit
-000196f0: 795f 7062 322e 456e 7469 7479 5072 6f74  y_pb2.EntityProt
-00019700: 6f28 290a 0a20 2020 2069 6620 7365 745f  o()..    if set_
-00019710: 6b65 793a 0a0a 2020 2020 2020 7365 6c66  key:..      self
-00019720: 2e5f 6b65 795f 746f 5f70 6228 7062 290a  ._key_to_pb(pb).
-00019730: 0a20 2020 2066 6f72 2075 6e75 7365 645f  .    for unused_
-00019740: 6e61 6d65 2c20 7072 6f70 2069 6e20 736f  name, prop in so
-00019750: 7274 6564 2873 6978 2e69 7465 7269 7465  rted(six.iterite
-00019760: 6d73 2873 656c 662e 5f70 726f 7065 7274  ms(self._propert
-00019770: 6965 7329 293a 0a20 2020 2020 2070 726f  ies)):.      pro
-00019780: 702e 5f73 6572 6961 6c69 7a65 2873 656c  p._serialize(sel
-00019790: 662c 2070 622c 2070 726f 6a65 6374 696f  f, pb, projectio
-000197a0: 6e3d 7365 6c66 2e5f 7072 6f6a 6563 7469  n=self._projecti
-000197b0: 6f6e 290a 0a20 2020 2072 6574 7572 6e20  on)..    return 
-000197c0: 7062 0a0a 2020 6465 6620 5f6b 6579 5f74  pb..  def _key_t
-000197d0: 6f5f 7062 2873 656c 662c 2070 6229 3a0a  o_pb(self, pb):.
-000197e0: 2020 2020 2222 2249 6e74 6572 6e61 6c20      """Internal 
-000197f0: 6865 6c70 6572 2074 6f20 636f 7079 2074  helper to copy t
-00019800: 6865 206b 6579 2069 6e74 6f20 6120 7072  he key into a pr
-00019810: 6f74 6f62 7566 2e22 2222 0a20 2020 206b  otobuf.""".    k
-00019820: 6579 203d 2073 656c 662e 5f6b 6579 0a20  ey = self._key. 
-00019830: 2020 2069 6620 6b65 7920 6973 204e 6f6e     if key is Non
-00019840: 653a 0a20 2020 2020 2070 6169 7273 203d  e:.      pairs =
-00019850: 205b 2873 656c 662e 5f67 6574 5f6b 696e   [(self._get_kin
-00019860: 6428 292c 204e 6f6e 6529 5d0a 2020 2020  d(), None)].    
-00019870: 2020 7265 6620 3d20 6b65 795f 6d6f 6475    ref = key_modu
-00019880: 6c65 2e5f 5265 6665 7265 6e63 6546 726f  le._ReferenceFro
-00019890: 6d50 6169 7273 2870 6169 7273 2c20 7265  mPairs(pairs, re
-000198a0: 6665 7265 6e63 653d 7062 2e6b 6579 290a  ference=pb.key).
-000198b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000198c0: 7265 6620 3d20 6b65 792e 7265 6665 7265  ref = key.refere
-000198d0: 6e63 6528 290a 2020 2020 2020 7062 2e6b  nce().      pb.k
-000198e0: 6579 2e43 6f70 7946 726f 6d28 7265 6629  ey.CopyFrom(ref)
-000198f0: 0a20 2020 2070 622e 656e 7469 7479 5f67  .    pb.entity_g
-00019900: 726f 7570 2e53 6574 496e 5061 7265 6e74  roup.SetInParent
-00019910: 2829 0a20 2020 2067 726f 7570 203d 2070  ().    group = p
-00019920: 622e 656e 7469 7479 5f67 726f 7570 0a0a  b.entity_group..
-00019930: 0a20 2020 2069 6620 6b65 7920 6973 206e  .    if key is n
-00019940: 6f74 204e 6f6e 6520 616e 6420 6b65 792e  ot None and key.
-00019950: 6964 2829 3a0a 2020 2020 2020 656c 656d  id():.      elem
-00019960: 203d 2072 6566 2e70 6174 682e 656c 656d   = ref.path.elem
-00019970: 656e 745b 305d 0a20 2020 2020 2069 6620  ent[0].      if 
-00019980: 656c 656d 2e69 6420 6f72 2065 6c65 6d2e  elem.id or elem.
-00019990: 6e61 6d65 3a0a 2020 2020 2020 2020 6772  name:.        gr
-000199a0: 6f75 702e 656c 656d 656e 742e 6164 6428  oup.element.add(
-000199b0: 292e 436f 7079 4672 6f6d 2865 6c65 6d29  ).CopyFrom(elem)
-000199c0: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
-000199d0: 0a20 2064 6566 205f 6672 6f6d 5f70 6228  .  def _from_pb(
-000199e0: 636c 732c 2070 622c 2073 6574 5f6b 6579  cls, pb, set_key
-000199f0: 3d54 7275 652c 2065 6e74 3d4e 6f6e 652c  =True, ent=None,
-00019a00: 206b 6579 3d4e 6f6e 6529 3a0a 2020 2020   key=None):.    
-00019a10: 2222 2249 6e74 6572 6e61 6c20 6865 6c70  """Internal help
-00019a20: 6572 2074 6f20 6372 6561 7465 2061 6e20  er to create an 
-00019a30: 656e 7469 7479 2066 726f 6d20 616e 2045  entity from an E
-00019a40: 6e74 6974 7950 726f 746f 2070 726f 746f  ntityProto proto
-00019a50: 6275 662e 2222 220a 2020 2020 6966 206e  buf.""".    if n
-00019a60: 6f74 2069 7369 6e73 7461 6e63 6528 7062  ot isinstance(pb
-00019a70: 2c20 656e 7469 7479 5f70 6232 2e45 6e74  , entity_pb2.Ent
-00019a80: 6974 7950 726f 746f 293a 0a20 2020 2020  ityProto):.     
-00019a90: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-00019aa0: 2827 7062 206d 7573 7420 6265 2061 2045  ('pb must be a E
-00019ab0: 6e74 6974 7950 726f 746f 3b20 7265 6365  ntityProto; rece
-00019ac0: 6976 6564 2025 7227 2025 2070 6229 0a20  ived %r' % pb). 
-00019ad0: 2020 2069 6620 656e 7420 6973 204e 6f6e     if ent is Non
-00019ae0: 653a 0a20 2020 2020 2065 6e74 203d 2063  e:.      ent = c
-00019af0: 6c73 2829 0a0a 0a20 2020 2069 6620 6b65  ls()...    if ke
-00019b00: 7920 6973 204e 6f6e 6520 616e 6420 6c65  y is None and le
-00019b10: 6e28 7062 2e6b 6579 2e70 6174 682e 656c  n(pb.key.path.el
-00019b20: 656d 656e 7429 3a0a 2020 2020 2020 6b65  ement):.      ke
-00019b30: 7920 3d20 4b65 7928 7265 6665 7265 6e63  y = Key(referenc
-00019b40: 653d 7062 2e6b 6579 290a 0a20 2020 2069  e=pb.key)..    i
-00019b50: 6620 6b65 7920 6973 206e 6f74 204e 6f6e  f key is not Non
-00019b60: 6520 616e 6420 2873 6574 5f6b 6579 206f  e and (set_key o
-00019b70: 7220 6b65 792e 6964 2829 206f 7220 6b65  r key.id() or ke
-00019b80: 792e 7061 7265 6e74 2829 293a 0a20 2020  y.parent()):.   
-00019b90: 2020 2065 6e74 2e5f 6b65 7920 3d20 6b65     ent._key = ke
-00019ba0: 790a 0a0a 0a0a 2020 2020 5f70 726f 7065  y.....    _prope
-00019bb0: 7274 795f 6d61 7020 3d20 7b7d 0a20 2020  rty_map = {}.   
-00019bc0: 2070 726f 6a65 6374 696f 6e20 3d20 5b5d   projection = []
-00019bd0: 0a20 2020 2066 6f72 2069 6e64 6578 6564  .    for indexed
-00019be0: 2c20 706c 6973 7420 696e 2028 2854 7275  , plist in ((Tru
-00019bf0: 652c 2070 622e 7072 6f70 6572 7479 292c  e, pb.property),
-00019c00: 2028 4661 6c73 652c 2070 622e 7261 775f   (False, pb.raw_
-00019c10: 7072 6f70 6572 7479 2929 3a0a 2020 2020  property)):.    
-00019c20: 2020 666f 7220 7020 696e 2070 6c69 7374    for p in plist
-00019c30: 3a0a 2020 2020 2020 2020 7072 6f70 5f6e  :.        prop_n
-00019c40: 616d 6520 3d20 7369 782e 656e 7375 7265  ame = six.ensure
-00019c50: 5f74 6578 7428 702e 6e61 6d65 290a 2020  _text(p.name).  
-00019c60: 2020 2020 2020 6966 2070 2e6d 6561 6e69        if p.meani
-00019c70: 6e67 203d 3d20 656e 7469 7479 5f70 6232  ng == entity_pb2
-00019c80: 2e50 726f 7065 7274 792e 494e 4445 585f  .Property.INDEX_
-00019c90: 5641 4c55 453a 0a20 2020 2020 2020 2020  VALUE:.         
-00019ca0: 2070 726f 6a65 6374 696f 6e2e 6170 7065   projection.appe
-00019cb0: 6e64 2870 726f 705f 6e61 6d65 290a 2020  nd(prop_name).  
-00019cc0: 2020 2020 2020 7072 6f70 6572 7479 5f6d        property_m
-00019cd0: 6170 5f6b 6579 203d 2028 7072 6f70 5f6e  ap_key = (prop_n
-00019ce0: 616d 652c 2069 6e64 6578 6564 290a 2020  ame, indexed).  
-00019cf0: 2020 2020 2020 6966 2070 726f 7065 7274        if propert
-00019d00: 795f 6d61 705f 6b65 7920 6e6f 7420 696e  y_map_key not in
-00019d10: 205f 7072 6f70 6572 7479 5f6d 6170 3a0a   _property_map:.
-00019d20: 2020 2020 2020 2020 2020 5f70 726f 7065            _prope
-00019d30: 7274 795f 6d61 705b 7072 6f70 6572 7479  rty_map[property
-00019d40: 5f6d 6170 5f6b 6579 5d20 3d20 656e 742e  _map_key] = ent.
-00019d50: 5f67 6574 5f70 726f 7065 7274 795f 666f  _get_property_fo
-00019d60: 7228 702c 2069 6e64 6578 6564 290a 2020  r(p, indexed).  
-00019d70: 2020 2020 2020 5f70 726f 7065 7274 795f        _property_
-00019d80: 6d61 705b 7072 6f70 6572 7479 5f6d 6170  map[property_map
-00019d90: 5f6b 6579 5d2e 5f64 6573 6572 6961 6c69  _key]._deseriali
-00019da0: 7a65 2865 6e74 2c20 7029 0a0a 2020 2020  ze(ent, p)..    
-00019db0: 656e 742e 5f73 6574 5f70 726f 6a65 6374  ent._set_project
-00019dc0: 696f 6e28 7072 6f6a 6563 7469 6f6e 290a  ion(projection).
-00019dd0: 2020 2020 7265 7475 726e 2065 6e74 0a0a      return ent..
-00019de0: 2020 6465 6620 5f73 6574 5f70 726f 6a65    def _set_proje
-00019df0: 6374 696f 6e28 7365 6c66 2c20 7072 6f6a  ction(self, proj
-00019e00: 6563 7469 6f6e 293a 0a20 2020 2062 795f  ection):.    by_
-00019e10: 7072 6566 6978 203d 207b 7d0a 2020 2020  prefix = {}.    
-00019e20: 666f 7220 7072 6f70 6e61 6d65 2069 6e20  for propname in 
-00019e30: 7072 6f6a 6563 7469 6f6e 3a0a 2020 2020  projection:.    
-00019e40: 2020 6966 2027 2e27 2069 6e20 7072 6f70    if '.' in prop
-00019e50: 6e61 6d65 3a0a 2020 2020 2020 2020 6865  name:.        he
-00019e60: 6164 2c20 7461 696c 203d 2070 726f 706e  ad, tail = propn
-00019e70: 616d 652e 7370 6c69 7428 272e 272c 2031  ame.split('.', 1
-00019e80: 290a 2020 2020 2020 2020 6966 2068 6561  ).        if hea
-00019e90: 6420 696e 2062 795f 7072 6566 6978 3a0a  d in by_prefix:.
-00019ea0: 2020 2020 2020 2020 2020 6279 5f70 7265            by_pre
-00019eb0: 6669 785b 6865 6164 5d2e 6170 7065 6e64  fix[head].append
-00019ec0: 2874 6169 6c29 0a20 2020 2020 2020 2065  (tail).        e
-00019ed0: 6c73 653a 0a20 2020 2020 2020 2020 2062  lse:.          b
-00019ee0: 795f 7072 6566 6978 5b68 6561 645d 203d  y_prefix[head] =
-00019ef0: 205b 7461 696c 5d0a 2020 2020 7365 6c66   [tail].    self
-00019f00: 2e5f 7072 6f6a 6563 7469 6f6e 203d 2074  ._projection = t
-00019f10: 7570 6c65 2870 726f 6a65 6374 696f 6e29  uple(projection)
-00019f20: 0a20 2020 2066 6f72 2070 726f 706e 616d  .    for propnam
-00019f30: 652c 2070 726f 6a20 696e 2073 6978 2e69  e, proj in six.i
-00019f40: 7465 7269 7465 6d73 2862 795f 7072 6566  teritems(by_pref
-00019f50: 6978 293a 0a20 2020 2020 2070 726f 7020  ix):.      prop 
-00019f60: 3d20 7365 6c66 2e5f 7072 6f70 6572 7469  = self._properti
-00019f70: 6573 2e67 6574 2870 726f 706e 616d 6529  es.get(propname)
-00019f80: 0a20 2020 2020 2073 7562 7661 6c20 3d20  .      subval = 
-00019f90: 7072 6f70 2e5f 6765 745f 6261 7365 5f76  prop._get_base_v
-00019fa0: 616c 7565 5f75 6e77 7261 7070 6564 5f61  alue_unwrapped_a
-00019fb0: 735f 6c69 7374 2873 656c 6629 0a20 2020  s_list(self).   
-00019fc0: 2020 2066 6f72 2069 7465 6d20 696e 2073     for item in s
-00019fd0: 7562 7661 6c3a 0a20 2020 2020 2020 2061  ubval:.        a
-00019fe0: 7373 6572 7420 6974 656d 2069 7320 6e6f  ssert item is no
-00019ff0: 7420 4e6f 6e65 0a20 2020 2020 2020 2069  t None.        i
-0001a000: 7465 6d2e 5f73 6574 5f70 726f 6a65 6374  tem._set_project
-0001a010: 696f 6e28 7072 6f6a 290a 0a20 2064 6566  ion(proj)..  def
-0001a020: 205f 6765 745f 7072 6f70 6572 7479 5f66   _get_property_f
-0001a030: 6f72 2873 656c 662c 2070 2c20 696e 6465  or(self, p, inde
-0001a040: 7865 643d 5472 7565 2c20 6465 7074 683d  xed=True, depth=
-0001a050: 3029 3a0a 2020 2020 2222 2249 6e74 6572  0):.    """Inter
-0001a060: 6e61 6c20 6865 6c70 6572 2074 6f20 6765  nal helper to ge
-0001a070: 7420 7468 6520 5072 6f70 6572 7479 2066  t the Property f
-0001a080: 6f72 2061 2070 726f 746f 6275 662d 6c65  or a protobuf-le
-0001a090: 7665 6c20 7072 6f70 6572 7479 2e22 2222  vel property."""
-0001a0a0: 0a20 2020 2070 6172 7473 203d 2070 2e6e  .    parts = p.n
-0001a0b0: 616d 652e 7370 6c69 7428 272e 2729 0a20  ame.split('.'). 
-0001a0c0: 2020 2069 6620 6c65 6e28 7061 7274 7329     if len(parts)
-0001a0d0: 203c 3d20 6465 7074 683a 0a0a 0a0a 0a0a   <= depth:......
-0001a0e0: 0a20 2020 2020 2072 6574 7572 6e20 4e6f  .      return No
-0001a0f0: 6e65 0a20 2020 206e 6578 7420 3d20 7061  ne.    next = pa
-0001a100: 7274 735b 6465 7074 685d 0a20 2020 2070  rts[depth].    p
-0001a110: 726f 7020 3d20 7365 6c66 2e5f 7072 6f70  rop = self._prop
-0001a120: 6572 7469 6573 2e67 6574 286e 6578 7429  erties.get(next)
-0001a130: 0a20 2020 2069 6620 7072 6f70 2069 7320  .    if prop is 
-0001a140: 4e6f 6e65 3a0a 2020 2020 2020 7072 6f70  None:.      prop
-0001a150: 203d 2073 656c 662e 5f66 616b 655f 7072   = self._fake_pr
-0001a160: 6f70 6572 7479 2870 2c20 6e65 7874 2c20  operty(p, next, 
-0001a170: 696e 6465 7865 6429 0a20 2020 2072 6574  indexed).    ret
-0001a180: 7572 6e20 7072 6f70 0a0a 2020 6465 6620  urn prop..  def 
-0001a190: 5f63 6c6f 6e65 5f70 726f 7065 7274 6965  _clone_propertie
-0001a1a0: 7328 7365 6c66 293a 0a20 2020 2022 2222  s(self):.    """
-0001a1b0: 496e 7465 726e 616c 2068 656c 7065 7220  Internal helper 
-0001a1c0: 746f 2063 6c6f 6e65 2073 656c 662e 5f70  to clone self._p
-0001a1d0: 726f 7065 7274 6965 7320 6966 206e 6563  roperties if nec
-0001a1e0: 6573 7361 7279 2e22 2222 0a20 2020 2063  essary.""".    c
-0001a1f0: 6c73 203d 2073 656c 662e 5f5f 636c 6173  ls = self.__clas
-0001a200: 735f 5f0a 2020 2020 6966 2073 656c 662e  s__.    if self.
-0001a210: 5f70 726f 7065 7274 6965 7320 6973 2063  _properties is c
-0001a220: 6c73 2e5f 7072 6f70 6572 7469 6573 3a0a  ls._properties:.
-0001a230: 2020 2020 2020 7365 6c66 2e5f 7072 6f70        self._prop
-0001a240: 6572 7469 6573 203d 2064 6963 7428 636c  erties = dict(cl
-0001a250: 732e 5f70 726f 7065 7274 6965 7329 0a0a  s._properties)..
-0001a260: 2020 6465 6620 5f66 616b 655f 7072 6f70    def _fake_prop
-0001a270: 6572 7479 2873 656c 662c 2070 2c20 6e65  erty(self, p, ne
-0001a280: 7874 2c20 696e 6465 7865 643d 5472 7565  xt, indexed=True
-0001a290: 293a 0a20 2020 2022 2222 496e 7465 726e  ):.    """Intern
-0001a2a0: 616c 2068 656c 7065 7220 746f 2063 7265  al helper to cre
-0001a2b0: 6174 6520 6120 6661 6b65 2050 726f 7065  ate a fake Prope
-0001a2c0: 7274 792e 2222 220a 2020 2020 7365 6c66  rty.""".    self
-0001a2d0: 2e5f 636c 6f6e 655f 7072 6f70 6572 7469  ._clone_properti
-0001a2e0: 6573 2829 0a20 2020 2069 6620 702e 6e61  es().    if p.na
-0001a2f0: 6d65 2021 3d20 6e65 7874 2061 6e64 206e  me != next and n
-0001a300: 6f74 2070 2e6e 616d 652e 656e 6473 7769  ot p.name.endswi
-0001a310: 7468 2827 2e27 202b 206e 6578 7429 3a0a  th('.' + next):.
-0001a320: 2020 2020 2020 7072 6f70 203d 2053 7472        prop = Str
-0001a330: 7563 7475 7265 6450 726f 7065 7274 7928  ucturedProperty(
-0001a340: 4578 7061 6e64 6f2c 206e 6578 7429 0a20  Expando, next). 
-0001a350: 2020 2020 2070 726f 702e 5f73 746f 7265       prop._store
-0001a360: 5f76 616c 7565 2873 656c 662c 205f 4261  _value(self, _Ba
-0001a370: 7365 5661 6c75 6528 4578 7061 6e64 6f28  seValue(Expando(
-0001a380: 2929 290a 2020 2020 656c 7365 3a0a 2020  ))).    else:.  
-0001a390: 2020 2020 636f 6d70 7265 7373 6564 203d      compressed =
-0001a3a0: 2070 2e6d 6561 6e69 6e67 5f75 7269 203d   p.meaning_uri =
-0001a3b0: 3d20 5f4d 4541 4e49 4e47 5f55 5249 5f43  = _MEANING_URI_C
-0001a3c0: 4f4d 5052 4553 5345 440a 2020 2020 2020  OMPRESSED.      
-0001a3d0: 7072 6f70 203d 2047 656e 6572 6963 5072  prop = GenericPr
-0001a3e0: 6f70 6572 7479 280a 2020 2020 2020 2020  operty(.        
-0001a3f0: 2020 6e65 7874 2c20 7265 7065 6174 6564    next, repeated
-0001a400: 3d70 2e6d 756c 7469 706c 652c 2069 6e64  =p.multiple, ind
-0001a410: 6578 6564 3d69 6e64 6578 6564 2c20 636f  exed=indexed, co
-0001a420: 6d70 7265 7373 6564 3d63 6f6d 7072 6573  mpressed=compres
-0001a430: 7365 6429 0a20 2020 2070 726f 702e 5f63  sed).    prop._c
-0001a440: 6f64 655f 6e61 6d65 203d 206e 6578 740a  ode_name = next.
-0001a450: 2020 2020 7365 6c66 2e5f 7072 6f70 6572      self._proper
-0001a460: 7469 6573 5b70 726f 702e 5f6e 616d 652e  ties[prop._name.
-0001a470: 6465 636f 6465 2827 7574 662d 3827 295d  decode('utf-8')]
-0001a480: 203d 2070 726f 700a 2020 2020 7265 7475   = prop.    retu
-0001a490: 726e 2070 726f 700a 0a20 2040 7574 696c  rn prop..  @util
-0001a4a0: 732e 706f 7369 7469 6f6e 616c 2831 290a  s.positional(1).
-0001a4b0: 2020 6465 6620 5f74 6f5f 6469 6374 2873    def _to_dict(s
-0001a4c0: 656c 662c 2069 6e63 6c75 6465 3d4e 6f6e  elf, include=Non
-0001a4d0: 652c 2065 7863 6c75 6465 3d4e 6f6e 6529  e, exclude=None)
-0001a4e0: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
-0001a4f0: 6120 6469 6374 2063 6f6e 7461 696e 696e  a dict containin
-0001a500: 6720 7468 6520 656e 7469 7479 2773 2070  g the entity's p
-0001a510: 726f 7065 7274 7920 7661 6c75 6573 2e0a  roperty values..
-0001a520: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-0001a530: 2069 6e63 6c75 6465 3a20 4f70 7469 6f6e   include: Option
-0001a540: 616c 2073 6574 206f 6620 7072 6f70 6572  al set of proper
-0001a550: 7479 206e 616d 6573 2074 6f20 696e 636c  ty names to incl
-0001a560: 7564 652c 2064 6566 6175 6c74 2061 6c6c  ude, default all
-0001a570: 2e0a 2020 2020 2020 6578 636c 7564 653a  ..      exclude:
-0001a580: 204f 7074 696f 6e61 6c20 7365 7420 6f66   Optional set of
-0001a590: 2070 726f 7065 7274 7920 6e61 6d65 7320   property names 
-0001a5a0: 746f 2073 6b69 702c 2064 6566 6175 6c74  to skip, default
-0001a5b0: 206e 6f6e 652e 0a20 2020 2020 2020 2041   none..        A
-0001a5c0: 206e 616d 6520 636f 6e74 6169 6e65 6420   name contained 
-0001a5d0: 696e 2062 6f74 6820 696e 636c 7564 6520  in both include 
-0001a5e0: 616e 6420 6578 636c 7564 6520 6973 2065  and exclude is e
-0001a5f0: 7863 6c75 6465 642e 0a20 2020 2022 2222  xcluded..    """
-0001a600: 0a20 2020 2069 6620 2869 6e63 6c75 6465  .    if (include
-0001a610: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0001a620: 0a20 2020 2020 2020 206e 6f74 2069 7369  .        not isi
-0001a630: 6e73 7461 6e63 6528 696e 636c 7564 652c  nstance(include,
-0001a640: 2028 6c69 7374 2c20 7475 706c 652c 2073   (list, tuple, s
-0001a650: 6574 2c20 6672 6f7a 656e 7365 7429 2929  et, frozenset)))
-0001a660: 3a0a 2020 2020 2020 7261 6973 6520 5479  :.      raise Ty
-0001a670: 7065 4572 726f 7228 2769 6e63 6c75 6465  peError('include
-0001a680: 2073 686f 756c 6420 6265 2061 206c 6973   should be a lis
-0001a690: 742c 2074 7570 6c65 206f 7220 7365 7427  t, tuple or set'
-0001a6a0: 290a 2020 2020 6966 2028 6578 636c 7564  ).    if (exclud
-0001a6b0: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
-0001a6c0: 640a 2020 2020 2020 2020 6e6f 7420 6973  d.        not is
-0001a6d0: 696e 7374 616e 6365 2865 7863 6c75 6465  instance(exclude
-0001a6e0: 2c20 286c 6973 742c 2074 7570 6c65 2c20  , (list, tuple, 
-0001a6f0: 7365 742c 2066 726f 7a65 6e73 6574 2929  set, frozenset))
-0001a700: 293a 0a20 2020 2020 2072 6169 7365 2054  ):.      raise T
-0001a710: 7970 6545 7272 6f72 2827 6578 636c 7564  ypeError('exclud
-0001a720: 6520 7368 6f75 6c64 2062 6520 6120 6c69  e should be a li
-0001a730: 7374 2c20 7475 706c 6520 6f72 2073 6574  st, tuple or set
-0001a740: 2729 0a20 2020 2076 616c 7565 7320 3d20  ').    values = 
-0001a750: 7b7d 0a20 2020 2066 6f72 2070 726f 7020  {}.    for prop 
-0001a760: 696e 2073 6978 2e69 7465 7276 616c 7565  in six.itervalue
-0001a770: 7328 7365 6c66 2e5f 7072 6f70 6572 7469  s(self._properti
-0001a780: 6573 293a 0a20 2020 2020 206e 616d 6520  es):.      name 
-0001a790: 3d20 7072 6f70 2e5f 636f 6465 5f6e 616d  = prop._code_nam
-0001a7a0: 650a 2020 2020 2020 6966 2069 6e63 6c75  e.      if inclu
-0001a7b0: 6465 2069 7320 6e6f 7420 4e6f 6e65 2061  de is not None a
-0001a7c0: 6e64 206e 616d 6520 6e6f 7420 696e 2069  nd name not in i
-0001a7d0: 6e63 6c75 6465 3a0a 2020 2020 2020 2020  nclude:.        
-0001a7e0: 636f 6e74 696e 7565 0a20 2020 2020 2069  continue.      i
-0001a7f0: 6620 6578 636c 7564 6520 6973 206e 6f74  f exclude is not
-0001a800: 204e 6f6e 6520 616e 6420 6e61 6d65 2069   None and name i
-0001a810: 6e20 6578 636c 7564 653a 0a20 2020 2020  n exclude:.     
-0001a820: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-0001a830: 2020 7472 793a 0a20 2020 2020 2020 2076    try:.        v
-0001a840: 616c 7565 735b 6e61 6d65 5d20 3d20 7072  alues[name] = pr
-0001a850: 6f70 2e5f 6765 745f 666f 725f 6469 6374  op._get_for_dict
-0001a860: 2873 656c 6629 0a20 2020 2020 2065 7863  (self).      exc
-0001a870: 6570 7420 556e 7072 6f6a 6563 7465 6450  ept UnprojectedP
-0001a880: 726f 7065 7274 7945 7272 6f72 3a0a 2020  ropertyError:.  
-0001a890: 2020 2020 2020 7061 7373 0a20 2020 2072        pass.    r
-0001a8a0: 6574 7572 6e20 7661 6c75 6573 0a20 2074  eturn values.  t
-0001a8b0: 6f5f 6469 6374 203d 205f 746f 5f64 6963  o_dict = _to_dic
-0001a8c0: 740a 0a20 2040 636c 6173 736d 6574 686f  t..  @classmetho
-0001a8d0: 640a 2020 6465 6620 5f66 6978 5f75 705f  d.  def _fix_up_
-0001a8e0: 7072 6f70 6572 7469 6573 2863 6c73 293a  properties(cls):
-0001a8f0: 0a20 2020 2022 2222 4669 7820 7570 2074  .    """Fix up t
-0001a900: 6865 2070 726f 7065 7274 6965 7320 6279  he properties by
-0001a910: 2063 616c 6c69 6e67 2074 6865 6972 205f   calling their _
-0001a920: 6669 785f 7570 2829 206d 6574 686f 642e  fix_up() method.
-0001a930: 0a0a 2020 2020 4e6f 7465 3a20 5468 6973  ..    Note: This
-0001a940: 2069 7320 6361 6c6c 6564 2062 7920 4d65   is called by Me
-0001a950: 7461 4d6f 6465 6c2c 2062 7574 206d 6179  taModel, but may
-0001a960: 2061 6c73 6f20 6265 2063 616c 6c65 6420   also be called 
-0001a970: 6d61 6e75 616c 6c79 0a20 2020 2061 6674  manually.    aft
-0001a980: 6572 2064 796e 616d 6963 616c 6c79 2075  er dynamically u
-0001a990: 7064 6174 696e 6720 6120 6d6f 6465 6c20  pdating a model 
-0001a9a0: 636c 6173 732e 0a20 2020 2022 2222 0a0a  class..    """..
-0001a9b0: 2020 2020 6b69 6e64 203d 2063 6c73 2e5f      kind = cls._
-0001a9c0: 6765 745f 6b69 6e64 2829 0a20 2020 2069  get_kind().    i
-0001a9d0: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-0001a9e0: 286b 696e 642c 2028 7369 782e 7465 7874  (kind, (six.text
-0001a9f0: 5f74 7970 652c 2073 6978 2e62 696e 6172  _type, six.binar
-0001aa00: 795f 7479 7065 2929 3a0a 2020 2020 2020  y_type)):.      
-0001aa10: 7261 6973 6520 4b69 6e64 4572 726f 7228  raise KindError(
-0001aa20: 2743 6c61 7373 2025 7320 6465 6669 6e65  'Class %s define
-0001aa30: 7320 6120 5f67 6574 5f6b 696e 6428 2920  s a _get_kind() 
-0001aa40: 6d65 7468 6f64 2074 6861 7420 7265 7475  method that retu
-0001aa50: 726e 7320 270a 2020 2020 2020 2020 2020  rns '.          
-0001aa60: 2020 2020 2020 2020 2020 2020 2761 206e              'a n
-0001aa70: 6f6e 2d73 7472 696e 6720 2825 7229 2720  on-string (%r)' 
-0001aa80: 2520 2863 6c73 2e5f 5f6e 616d 655f 5f2c  % (cls.__name__,
-0001aa90: 206b 696e 6429 290a 2020 2020 6966 2073   kind)).    if s
-0001aaa0: 6978 2e50 5932 2061 6e64 206e 6f74 2069  ix.PY2 and not i
-0001aab0: 7369 6e73 7461 6e63 6528 6b69 6e64 2c20  sinstance(kind, 
-0001aac0: 7369 782e 6269 6e61 7279 5f74 7970 6529  six.binary_type)
-0001aad0: 3a0a 2020 2020 2020 7472 793a 0a20 2020  :.      try:.   
-0001aae0: 2020 2020 206b 696e 6420 3d20 6b69 6e64       kind = kind
-0001aaf0: 2e65 6e63 6f64 6528 2761 7363 6969 2729  .encode('ascii')
-0001ab00: 0a20 2020 2020 2065 7863 6570 7420 556e  .      except Un
-0001ab10: 6963 6f64 6545 6e63 6f64 6545 7272 6f72  icodeEncodeError
-0001ab20: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-0001ab30: 4b69 6e64 4572 726f 7228 2743 6c61 7373  KindError('Class
-0001ab40: 2025 7320 6465 6669 6e65 7320 6120 5f67   %s defines a _g
-0001ab50: 6574 5f6b 696e 6428 2920 6d65 7468 6f64  et_kind() method
-0001ab60: 2074 6861 7420 7265 7475 726e 7320 270a   that returns '.
-0001ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab80: 2020 2020 2020 2020 2761 2055 6e69 636f          'a Unico
-0001ab90: 6465 2073 7472 696e 6720 2825 7229 3b20  de string (%r); 
-0001aba0: 706c 6561 7365 2065 6e63 6f64 6520 7573  please encode us
-0001abb0: 696e 6720 7574 662d 3827 2025 0a20 2020  ing utf-8' %.   
+00017ec0: 6566 205f 7079 325f 636f 6d70 6174 5f65  ef _py2_compat_e
+00017ed0: 6e63 6f64 6528 7365 6c66 2c20 7079 325f  ncode(self, py2_
+00017ee0: 7365 7269 616c 697a 6564 5f70 6229 3a0a  serialized_pb):.
+00017ef0: 2020 2020 7265 7475 726e 2062 7974 6573      return bytes
+00017f00: 2870 7932 5f73 6572 6961 6c69 7a65 645f  (py2_serialized_
+00017f10: 7062 2c20 276c 6174 696e 3127 290a 0a20  pb, 'latin1').. 
+00017f20: 2064 6566 205f 5f73 6574 7374 6174 655f   def __setstate_
+00017f30: 5f28 7365 6c66 2c20 7365 7269 616c 697a  _(self, serializ
+00017f40: 6564 5f70 6229 3a0a 2020 2020 6966 2069  ed_pb):.    if i
+00017f50: 7369 6e73 7461 6e63 6528 7365 7269 616c  sinstance(serial
+00017f60: 697a 6564 5f70 622c 2073 7472 293a 0a20  ized_pb, str):. 
+00017f70: 2020 2020 2023 2049 6620 2773 6572 6961       # If 'seria
+00017f80: 6c69 7a65 645f 7062 2720 7761 7320 7772  lized_pb' was wr
+00017f90: 6974 7465 6e20 6279 2061 2070 7974 686f  itten by a pytho
+00017fa0: 6e32 3720 636c 6f6e 652e 0a20 2020 2020  n27 clone..     
+00017fb0: 206c 6f67 6769 6e67 2e77 6172 6e69 6e67   logging.warning
+00017fc0: 280a 2020 2020 2020 2020 2020 2741 7373  (.          'Ass
+00017fd0: 756d 696e 6720 7079 7468 6f6e 3220 7069  uming python2 pi
+00017fe0: 636b 6c65 6420 7374 6174 652c 2063 6f6e  ckled state, con
+00017ff0: 7665 7274 696e 6720 746f 2070 7974 686f  verting to pytho
+00018000: 6e33 2074 7970 652e 270a 2020 2020 2020  n3 type.'.      
+00018010: 290a 2020 2020 2020 7365 7269 616c 697a  ).      serializ
+00018020: 6564 5f70 6220 3d20 7365 6c66 2e5f 7079  ed_pb = self._py
+00018030: 325f 636f 6d70 6174 5f65 6e63 6f64 6528  2_compat_encode(
+00018040: 7365 7269 616c 697a 6564 5f70 6229 0a20  serialized_pb). 
+00018050: 2020 2070 6220 3d20 656e 7469 7479 5f70     pb = entity_p
+00018060: 6232 2e45 6e74 6974 7950 726f 746f 2e46  b2.EntityProto.F
+00018070: 726f 6d53 7472 696e 6728 7365 7269 616c  romString(serial
+00018080: 697a 6564 5f70 6229 0a20 2020 2073 656c  ized_pb).    sel
+00018090: 662e 5f5f 696e 6974 5f5f 2829 0a20 2020  f.__init__().   
+000180a0: 2073 656c 662e 5f5f 636c 6173 735f 5f2e   self.__class__.
+000180b0: 5f66 726f 6d5f 7062 2870 622c 2073 6574  _from_pb(pb, set
+000180c0: 5f6b 6579 3d46 616c 7365 2c20 656e 743d  _key=False, ent=
+000180d0: 7365 6c66 290a 0a20 2064 6566 205f 706f  self)..  def _po
+000180e0: 7075 6c61 7465 2873 656c 662c 202a 2a6b  pulate(self, **k
+000180f0: 7764 7329 3a0a 2020 2020 2222 2250 6f70  wds):.    """Pop
+00018100: 756c 6174 6520 616e 2069 6e73 7461 6e63  ulate an instanc
+00018110: 6520 6672 6f6d 206b 6579 776f 7264 2061  e from keyword a
+00018120: 7267 756d 656e 7473 2e0a 0a20 2020 2045  rguments...    E
+00018130: 6163 6820 6b65 7977 6f72 6420 6172 6775  ach keyword argu
+00018140: 6d65 6e74 2077 696c 6c20 6265 2075 7365  ment will be use
+00018150: 6420 746f 2073 6574 2061 2063 6f72 7265  d to set a corre
+00018160: 7370 6f6e 6469 6e67 0a20 2020 2070 726f  sponding.    pro
+00018170: 7065 7274 792e 2020 4b65 7977 6f72 6473  perty.  Keywords
+00018180: 206d 7573 7420 7265 6665 7220 746f 2076   must refer to v
+00018190: 616c 6964 2070 726f 7065 7274 7920 6e61  alid property na
+000181a0: 6d65 2e20 2054 6869 7320 6973 0a20 2020  me.  This is.   
+000181b0: 2073 696d 696c 6172 2074 6f20 7061 7373   similar to pass
+000181c0: 696e 6720 6b65 7977 6f72 6420 6172 6775  ing keyword argu
+000181d0: 6d65 6e74 7320 746f 2074 6865 204d 6f64  ments to the Mod
+000181e0: 656c 2063 6f6e 7374 7275 6374 6f72 2c0a  el constructor,.
+000181f0: 2020 2020 6578 6365 7074 2074 6861 7420      except that 
+00018200: 6e6f 2070 726f 7669 7369 6f6e 7320 666f  no provisions fo
+00018210: 7220 6b65 792c 2069 6420 6f72 2070 6172  r key, id or par
+00018220: 656e 7420 6172 6520 6d61 6465 2e0a 2020  ent are made..  
+00018230: 2020 2222 220a 2020 2020 7365 6c66 2e5f    """.    self._
+00018240: 7365 745f 6174 7472 6962 7574 6573 286b  set_attributes(k
+00018250: 7764 7329 0a20 2070 6f70 756c 6174 6520  wds).  populate 
+00018260: 3d20 5f70 6f70 756c 6174 650a 0a20 2064  = _populate..  d
+00018270: 6566 205f 7365 745f 6174 7472 6962 7574  ef _set_attribut
+00018280: 6573 2873 656c 662c 206b 7764 7329 3a0a  es(self, kwds):.
+00018290: 2020 2020 2222 2249 6e74 6572 6e61 6c20      """Internal 
+000182a0: 6865 6c70 6572 2074 6f20 7365 7420 6174  helper to set at
+000182b0: 7472 6962 7574 6573 2066 726f 6d20 6b65  tributes from ke
+000182c0: 7977 6f72 6420 6172 6775 6d65 6e74 732e  yword arguments.
+000182d0: 0a0a 2020 2020 4578 7061 6e64 6f20 6f76  ..    Expando ov
+000182e0: 6572 7269 6465 7320 7468 6973 2e0a 2020  errides this..  
+000182f0: 2020 2222 220a 2020 2020 636c 7320 3d20    """.    cls = 
+00018300: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 0a20  self.__class__. 
+00018310: 2020 2066 6f72 206e 616d 652c 2076 616c     for name, val
+00018320: 7565 2069 6e20 7369 782e 6974 6572 6974  ue in six.iterit
+00018330: 656d 7328 6b77 6473 293a 0a20 2020 2020  ems(kwds):.     
+00018340: 2070 726f 7020 3d20 6765 7461 7474 7228   prop = getattr(
+00018350: 636c 732c 206e 616d 6529 0a20 2020 2020  cls, name).     
+00018360: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+00018370: 6365 2870 726f 702c 2050 726f 7065 7274  ce(prop, Propert
+00018380: 7929 3a0a 2020 2020 2020 2020 7261 6973  y):.        rais
+00018390: 6520 5479 7065 4572 726f 7228 2743 616e  e TypeError('Can
+000183a0: 6e6f 7420 7365 7420 6e6f 6e2d 7072 6f70  not set non-prop
+000183b0: 6572 7479 2025 7327 2025 206e 616d 6529  erty %s' % name)
+000183c0: 0a20 2020 2020 2070 726f 702e 5f73 6574  .      prop._set
+000183d0: 5f76 616c 7565 2873 656c 662c 2076 616c  _value(self, val
+000183e0: 7565 290a 0a20 2064 6566 205f 6669 6e64  ue)..  def _find
+000183f0: 5f75 6e69 6e69 7469 616c 697a 6564 2873  _uninitialized(s
+00018400: 656c 6629 3a0a 2020 2020 2222 2249 6e74  elf):.    """Int
+00018410: 6572 6e61 6c20 6865 6c70 6572 2074 6f20  ernal helper to 
+00018420: 6669 6e64 2075 6e69 6e69 7469 616c 697a  find uninitializ
+00018430: 6564 2070 726f 7065 7274 6965 732e 0a0a  ed properties...
+00018440: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00018450: 2020 2041 2073 6574 206f 6620 7072 6f70     A set of prop
+00018460: 6572 7479 206e 616d 6573 2e0a 2020 2020  erty names..    
+00018470: 2222 220a 2020 2020 7265 7475 726e 2073  """.    return s
+00018480: 6574 286e 616d 6520 666f 7220 6e61 6d65  et(name for name
+00018490: 2c20 7072 6f70 2069 6e20 7369 782e 6974  , prop in six.it
+000184a0: 6572 6974 656d 7328 7365 6c66 2e5f 7072  eritems(self._pr
+000184b0: 6f70 6572 7469 6573 290a 2020 2020 2020  operties).      
+000184c0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000184d0: 7072 6f70 2e5f 6973 5f69 6e69 7469 616c  prop._is_initial
+000184e0: 697a 6564 2873 656c 6629 290a 0a20 2064  ized(self))..  d
+000184f0: 6566 205f 6368 6563 6b5f 696e 6974 6961  ef _check_initia
+00018500: 6c69 7a65 6428 7365 6c66 293a 0a20 2020  lized(self):.   
+00018510: 2022 2222 496e 7465 726e 616c 2068 656c   """Internal hel
+00018520: 7065 7220 746f 2063 6865 636b 2066 6f72  per to check for
+00018530: 2075 6e69 6e69 7469 616c 697a 6564 2070   uninitialized p
+00018540: 726f 7065 7274 6965 732e 0a0a 2020 2020  roperties...    
+00018550: 5261 6973 6573 3a0a 2020 2020 2020 4261  Raises:.      Ba
+00018560: 6456 616c 7565 4572 726f 7220 6966 2069  dValueError if i
+00018570: 7420 6669 6e64 7320 616e 792e 0a20 2020  t finds any..   
+00018580: 2022 2222 0a20 2020 2062 6164 6469 6573   """.    baddies
+00018590: 203d 2073 656c 662e 5f66 696e 645f 756e   = self._find_un
+000185a0: 696e 6974 6961 6c69 7a65 6428 290a 2020  initialized().  
+000185b0: 2020 6966 2062 6164 6469 6573 3a0a 2020    if baddies:.  
+000185c0: 2020 2020 7261 6973 6520 6461 7461 7374      raise datast
+000185d0: 6f72 655f 6572 726f 7273 2e42 6164 5661  ore_errors.BadVa
+000185e0: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+000185f0: 2020 2020 2745 6e74 6974 7920 6861 7320      'Entity has 
+00018600: 756e 696e 6974 6961 6c69 7a65 6420 7072  uninitialized pr
+00018610: 6f70 6572 7469 6573 3a20 2573 2720 2520  operties: %s' % 
+00018620: 272c 2027 2e6a 6f69 6e28 6261 6464 6965  ', '.join(baddie
+00018630: 7329 290a 0a20 2064 6566 205f 5f72 6570  s))..  def __rep
+00018640: 725f 5f28 7365 6c66 293a 0a20 2020 2022  r__(self):.    "
+00018650: 2222 5265 7475 726e 2061 6e20 756e 616d  ""Return an unam
+00018660: 6269 6775 6f75 7320 7374 7269 6e67 2072  biguous string r
+00018670: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+00018680: 2061 6e20 656e 7469 7479 2e22 2222 0a20   an entity.""". 
+00018690: 2020 2061 7267 7320 3d20 5b5d 0a20 2020     args = [].   
+000186a0: 2066 6f72 2070 726f 7020 696e 2073 6978   for prop in six
+000186b0: 2e69 7465 7276 616c 7565 7328 7365 6c66  .itervalues(self
+000186c0: 2e5f 7072 6f70 6572 7469 6573 293a 0a20  ._properties):. 
+000186d0: 2020 2020 2069 6620 7072 6f70 2e5f 6861       if prop._ha
+000186e0: 735f 7661 6c75 6528 7365 6c66 293a 0a20  s_value(self):. 
+000186f0: 2020 2020 2020 2076 616c 203d 2070 726f         val = pro
+00018700: 702e 5f72 6574 7269 6576 655f 7661 6c75  p._retrieve_valu
+00018710: 6528 7365 6c66 290a 2020 2020 2020 2020  e(self).        
+00018720: 6966 2076 616c 2069 7320 4e6f 6e65 3a0a  if val is None:.
+00018730: 2020 2020 2020 2020 2020 7265 7020 3d20            rep = 
+00018740: 274e 6f6e 6527 0a20 2020 2020 2020 2065  'None'.        e
+00018750: 6c69 6620 7072 6f70 2e5f 7265 7065 6174  lif prop._repeat
+00018760: 6564 3a0a 2020 2020 2020 2020 2020 7265  ed:.          re
+00018770: 7072 7320 3d20 5b70 726f 702e 5f76 616c  prs = [prop._val
+00018780: 7565 5f74 6f5f 7265 7072 2876 2920 666f  ue_to_repr(v) fo
+00018790: 7220 7620 696e 2076 616c 5d0a 2020 2020  r v in val].    
+000187a0: 2020 2020 2020 6966 2072 6570 7273 3a0a        if reprs:.
+000187b0: 2020 2020 2020 2020 2020 2020 7265 7072              repr
+000187c0: 735b 305d 203d 2027 5b27 202b 2072 6570  s[0] = '[' + rep
+000187d0: 7273 5b30 5d0a 2020 2020 2020 2020 2020  rs[0].          
+000187e0: 2020 7265 7072 735b 2d31 5d20 3d20 7265    reprs[-1] = re
+000187f0: 7072 735b 2d31 5d20 2b20 275d 270a 2020  prs[-1] + ']'.  
+00018800: 2020 2020 2020 2020 2020 7265 7020 3d20            rep = 
+00018810: 272c 2027 2e6a 6f69 6e28 7265 7072 7329  ', '.join(reprs)
+00018820: 0a20 2020 2020 2020 2020 2065 6c73 653a  .          else:
+00018830: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
+00018840: 203d 2027 5b5d 270a 2020 2020 2020 2020   = '[]'.        
+00018850: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00018860: 7265 7020 3d20 7072 6f70 2e5f 7661 6c75  rep = prop._valu
+00018870: 655f 746f 5f72 6570 7228 7661 6c29 0a20  e_to_repr(val). 
+00018880: 2020 2020 2020 2061 7267 732e 6170 7065         args.appe
+00018890: 6e64 2827 2573 3d25 7327 2025 2028 7072  nd('%s=%s' % (pr
+000188a0: 6f70 2e5f 636f 6465 5f6e 616d 652c 2072  op._code_name, r
+000188b0: 6570 2929 0a20 2020 2061 7267 732e 736f  ep)).    args.so
+000188c0: 7274 2829 0a20 2020 2069 6620 7365 6c66  rt().    if self
+000188d0: 2e5f 6b65 7920 6973 206e 6f74 204e 6f6e  ._key is not Non
+000188e0: 653a 0a20 2020 2020 2061 7267 732e 696e  e:.      args.in
+000188f0: 7365 7274 2830 2c20 276b 6579 3d25 7227  sert(0, 'key=%r'
+00018900: 2025 2073 656c 662e 5f6b 6579 290a 2020   % self._key).  
+00018910: 2020 6966 2073 656c 662e 5f70 726f 6a65    if self._proje
+00018920: 6374 696f 6e3a 0a20 2020 2020 2061 7267  ction:.      arg
+00018930: 732e 6170 7065 6e64 2827 5f70 726f 6a65  s.append('_proje
+00018940: 6374 696f 6e3d 2572 2720 2520 2873 656c  ction=%r' % (sel
+00018950: 662e 5f70 726f 6a65 6374 696f 6e2c 2929  f._projection,))
+00018960: 0a20 2020 2073 203d 2027 2573 2825 7329  .    s = '%s(%s)
+00018970: 2720 2520 2873 656c 662e 5f5f 636c 6173  ' % (self.__clas
+00018980: 735f 5f2e 5f5f 6e61 6d65 5f5f 2c20 272c  s__.__name__, ',
+00018990: 2027 2e6a 6f69 6e28 6172 6773 2929 0a20   '.join(args)). 
+000189a0: 2020 2072 6574 7572 6e20 730a 0a20 2040     return s..  @
+000189b0: 636c 6173 736d 6574 686f 640a 2020 6465  classmethod.  de
+000189c0: 6620 5f67 6574 5f6b 696e 6428 636c 7329  f _get_kind(cls)
+000189d0: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
+000189e0: 7468 6520 6b69 6e64 206e 616d 6520 666f  the kind name fo
+000189f0: 7220 7468 6973 2063 6c61 7373 2e0a 0a20  r this class... 
+00018a00: 2020 2054 6869 7320 6465 6661 756c 7473     This defaults
+00018a10: 2074 6f20 636c 732e 5f5f 6e61 6d65 5f5f   to cls.__name__
+00018a20: 3b20 7573 6572 7320 6d61 7920 6f76 6572  ; users may over
+00018a30: 7269 6420 7468 6973 2074 6f20 6769 7665  rid this to give
+00018a40: 2061 0a20 2020 2063 6c61 7373 2061 2064   a.    class a d
+00018a50: 6966 6665 7265 6e74 206f 6e2d 6469 736b  ifferent on-disk
+00018a60: 206e 616d 6520 7468 616e 2069 7473 2063   name than its c
+00018a70: 6c61 7373 206e 616d 652e 0a20 2020 2022  lass name..    "
+00018a80: 2222 0a20 2020 2072 6574 7572 6e20 636c  "".    return cl
+00018a90: 732e 5f5f 6e61 6d65 5f5f 0a0a 2020 4063  s.__name__..  @c
+00018aa0: 6c61 7373 6d65 7468 6f64 0a20 2064 6566  lassmethod.  def
+00018ab0: 205f 636c 6173 735f 6e61 6d65 2863 6c73   _class_name(cls
+00018ac0: 293a 0a20 2020 2022 2222 4120 686f 6f6b  ):.    """A hook
+00018ad0: 2066 6f72 2070 6f6c 796d 6f64 656c 2074   for polymodel t
+00018ae0: 6f20 6f76 6572 7269 6465 2e0a 0a20 2020  o override...   
+00018af0: 2046 6f72 2072 6567 756c 6172 206d 6f64   For regular mod
+00018b00: 656c 7320 616e 6420 6578 7061 6e64 6f73  els and expandos
+00018b10: 2074 6869 7320 6973 206a 7573 7420 616e   this is just an
+00018b20: 2061 6c69 6173 2066 6f72 0a20 2020 205f   alias for.    _
+00018b30: 6765 745f 6b69 6e64 2829 2e20 2046 6f72  get_kind().  For
+00018b40: 2050 6f6c 794d 6f64 656c 2073 7562 636c   PolyModel subcl
+00018b50: 6173 7365 732c 2069 7420 7265 7475 726e  asses, it return
+00018b60: 7320 7468 6520 636c 6173 7320 6e61 6d65  s the class name
+00018b70: 0a20 2020 2028 6173 2073 6574 2069 6e20  .    (as set in 
+00018b80: 7468 6520 2763 6c61 7373 2720 6174 7472  the 'class' attr
+00018b90: 6962 7574 6520 7468 6572 656f 6629 2c20  ibute thereof), 
+00018ba0: 7768 6572 6561 7320 5f67 6574 5f6b 696e  whereas _get_kin
+00018bb0: 6428 290a 2020 2020 7265 7475 726e 7320  d().    returns 
+00018bc0: 7468 6520 6b69 6e64 2028 7468 6520 636c  the kind (the cl
+00018bd0: 6173 7320 6e61 6d65 206f 6620 7468 6520  ass name of the 
+00018be0: 726f 6f74 2063 6c61 7373 206f 6620 6120  root class of a 
+00018bf0: 7370 6563 6966 6963 0a20 2020 2050 6f6c  specific.    Pol
+00018c00: 794d 6f64 656c 2068 6965 7261 7263 6879  yModel hierarchy
+00018c10: 292e 0a20 2020 2022 2222 0a20 2020 2072  )..    """.    r
+00018c20: 6574 7572 6e20 636c 732e 5f67 6574 5f6b  eturn cls._get_k
+00018c30: 696e 6428 290a 0a20 2040 636c 6173 736d  ind()..  @classm
+00018c40: 6574 686f 640a 2020 6465 6620 5f64 6566  ethod.  def _def
+00018c50: 6175 6c74 5f66 696c 7465 7273 2863 6c73  ault_filters(cls
+00018c60: 293a 0a20 2020 2022 2222 5265 7475 726e  ):.    """Return
+00018c70: 2061 6e20 6974 6572 6162 6c65 206f 6620   an iterable of 
+00018c80: 6669 6c74 6572 7320 7468 6174 2061 7265  filters that are
+00018c90: 2061 6c77 6179 7320 746f 2062 6520 6170   always to be ap
+00018ca0: 706c 6965 642e 0a0a 2020 2020 5468 6973  plied...    This
+00018cb0: 2069 7320 7573 6564 2062 7920 506f 6c79   is used by Poly
+00018cc0: 4d6f 6465 6c20 746f 2071 7569 6574 6c79  Model to quietly
+00018cd0: 2069 6e73 6572 7420 6120 6669 6c74 6572   insert a filter
+00018ce0: 2066 6f72 2074 6865 0a20 2020 2063 7572   for the.    cur
+00018cf0: 7265 6e74 2063 6c61 7373 206e 616d 652e  rent class name.
+00018d00: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
+00018d10: 7572 6e20 2829 0a0a 2020 4063 6c61 7373  urn ()..  @class
+00018d20: 6d65 7468 6f64 0a20 2064 6566 205f 7265  method.  def _re
+00018d30: 7365 745f 6b69 6e64 5f6d 6170 2863 6c73  set_kind_map(cls
+00018d40: 293a 0a20 2020 2022 2222 436c 6561 7220  ):.    """Clear 
+00018d50: 7468 6520 6b69 6e64 206d 6170 2e20 2055  the kind map.  U
+00018d60: 7365 6675 6c20 666f 7220 7465 7374 696e  seful for testin
+00018d70: 672e 2222 220a 0a20 2020 206b 6565 7020  g."""..    keep 
+00018d80: 3d20 7b7d 0a20 2020 2066 6f72 206e 616d  = {}.    for nam
+00018d90: 652c 2076 616c 7565 2069 6e20 7369 782e  e, value in six.
+00018da0: 6974 6572 6974 656d 7328 636c 732e 5f6b  iteritems(cls._k
+00018db0: 696e 645f 6d61 7029 3a0a 2020 2020 2020  ind_map):.      
+00018dc0: 6966 206e 616d 652e 7374 6172 7473 7769  if name.startswi
+00018dd0: 7468 2827 5f5f 2729 2061 6e64 206e 616d  th('__') and nam
+00018de0: 652e 656e 6473 7769 7468 2827 5f5f 2729  e.endswith('__')
+00018df0: 3a0a 2020 2020 2020 2020 6b65 6570 5b6e  :.        keep[n
+00018e00: 616d 655d 203d 2076 616c 7565 0a20 2020  ame] = value.   
+00018e10: 2063 6c73 2e5f 6b69 6e64 5f6d 6170 2e63   cls._kind_map.c
+00018e20: 6c65 6172 2829 0a20 2020 2063 6c73 2e5f  lear().    cls._
+00018e30: 6b69 6e64 5f6d 6170 2e75 7064 6174 6528  kind_map.update(
+00018e40: 6b65 6570 290a 0a20 2040 636c 6173 736d  keep)..  @classm
+00018e50: 6574 686f 640a 2020 6465 6620 5f6c 6f6f  ethod.  def _loo
+00018e60: 6b75 705f 6d6f 6465 6c28 636c 732c 206b  kup_model(cls, k
+00018e70: 696e 642c 2064 6566 6175 6c74 5f6d 6f64  ind, default_mod
+00018e80: 656c 3d4e 6f6e 6529 3a0a 2020 2020 2222  el=None):.    ""
+00018e90: 2247 6574 2074 6865 206d 6f64 656c 2063  "Get the model c
+00018ea0: 6c61 7373 2066 6f72 2074 6865 206b 696e  lass for the kin
+00018eb0: 642e 0a0a 2020 2020 4172 6773 3a0a 2020  d...    Args:.  
+00018ec0: 2020 2020 6b69 6e64 3a20 4120 7374 7269      kind: A stri
+00018ed0: 6e67 2072 6570 7265 7365 6e74 696e 6720  ng representing 
+00018ee0: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
+00018ef0: 6b69 6e64 2074 6f20 6c6f 6f6b 7570 2e0a  kind to lookup..
+00018f00: 2020 2020 2020 6465 6661 756c 745f 6d6f        default_mo
+00018f10: 6465 6c3a 2054 6865 206d 6f64 656c 2063  del: The model c
+00018f20: 6c61 7373 2074 6f20 7573 6520 6966 2074  lass to use if t
+00018f30: 6865 206b 696e 6420 6361 6e27 7420 6265  he kind can't be
+00018f40: 2066 6f75 6e64 2e0a 0a20 2020 2052 6574   found...    Ret
+00018f50: 7572 6e73 3a0a 2020 2020 2020 5468 6520  urns:.      The 
+00018f60: 6d6f 6465 6c20 636c 6173 7320 666f 7220  model class for 
+00018f70: 7468 6520 7265 7175 6573 7465 6420 6b69  the requested ki
+00018f80: 6e64 2e0a 2020 2020 5261 6973 6573 3a0a  nd..    Raises:.
+00018f90: 2020 2020 2020 4b69 6e64 4572 726f 723a        KindError:
+00018fa0: 2054 6865 206b 696e 6420 7761 7320 6e6f   The kind was no
+00018fb0: 7420 666f 756e 6420 616e 6420 6e6f 2064  t found and no d
+00018fc0: 6566 6175 6c74 5f6d 6f64 656c 2077 6173  efault_model was
+00018fd0: 2070 726f 7669 6465 642e 0a20 2020 2022   provided..    "
+00018fe0: 2222 0a20 2020 206d 6f64 656c 636c 6173  "".    modelclas
+00018ff0: 7320 3d20 636c 732e 5f6b 696e 645f 6d61  s = cls._kind_ma
+00019000: 702e 6765 7428 6b69 6e64 2c20 6465 6661  p.get(kind, defa
+00019010: 756c 745f 6d6f 6465 6c29 0a20 2020 2069  ult_model).    i
+00019020: 6620 6d6f 6465 6c63 6c61 7373 2069 7320  f modelclass is 
+00019030: 4e6f 6e65 3a0a 2020 2020 2020 7261 6973  None:.      rais
+00019040: 6520 4b69 6e64 4572 726f 7228 0a20 2020  e KindError(.   
+00019050: 2020 2020 2020 2022 4e6f 206d 6f64 656c         "No model
+00019060: 2063 6c61 7373 2066 6f75 6e64 2066 6f72   class found for
+00019070: 206b 696e 6420 2725 7327 2e20 4469 6420   kind '%s'. Did 
+00019080: 796f 7520 666f 7267 6574 2074 6f20 696d  you forget to im
+00019090: 706f 7274 2069 743f 2220 250a 2020 2020  port it?" %.    
+000190a0: 2020 2020 2020 6b69 6e64 290a 2020 2020        kind).    
+000190b0: 7265 7475 726e 206d 6f64 656c 636c 6173  return modelclas
+000190c0: 730a 0a20 2064 6566 205f 6861 735f 636f  s..  def _has_co
+000190d0: 6d70 6c65 7465 5f6b 6579 2873 656c 6629  mplete_key(self)
+000190e0: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
+000190f0: 7768 6574 6865 7220 7468 6973 2065 6e74  whether this ent
+00019100: 6974 7920 6861 7320 6120 636f 6d70 6c65  ity has a comple
+00019110: 7465 206b 6579 2e22 2222 0a20 2020 2072  te key.""".    r
+00019120: 6574 7572 6e20 7365 6c66 2e5f 6b65 7920  eturn self._key 
+00019130: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00019140: 7365 6c66 2e5f 6b65 792e 6964 2829 2069  self._key.id() i
+00019150: 7320 6e6f 7420 4e6f 6e65 0a20 2068 6173  s not None.  has
+00019160: 5f63 6f6d 706c 6574 655f 6b65 7920 3d20  _complete_key = 
+00019170: 5f68 6173 5f63 6f6d 706c 6574 655f 6b65  _has_complete_ke
+00019180: 790a 0a20 2064 6566 205f 5f68 6173 685f  y..  def __hash_
+00019190: 5f28 7365 6c66 293a 0a20 2020 2022 2222  _(self):.    """
+000191a0: 4475 6d6d 7920 6861 7368 2066 756e 6374  Dummy hash funct
+000191b0: 696f 6e2e 0a0a 2020 2020 5261 6973 6573  ion...    Raises
+000191c0: 3a0a 2020 2020 2020 416c 7761 7973 2054  :.      Always T
+000191d0: 7970 6545 7272 6f72 2074 6f20 656d 7068  ypeError to emph
+000191e0: 6173 697a 6520 7468 6174 2065 6e74 6974  asize that entit
+000191f0: 6965 7320 6172 6520 6d75 7461 626c 652e  ies are mutable.
+00019200: 0a20 2020 2022 2222 0a20 2020 2072 6169  .    """.    rai
+00019210: 7365 2054 7970 6545 7272 6f72 2827 4d6f  se TypeError('Mo
+00019220: 6465 6c20 6973 206e 6f74 2069 6d6d 7574  del is not immut
+00019230: 6162 6c65 2729 0a0a 0a0a 2020 6465 6620  able')....  def 
+00019240: 5f5f 6571 5f5f 2873 656c 662c 206f 7468  __eq__(self, oth
+00019250: 6572 293a 0a20 2020 2022 2222 436f 6d70  er):.    """Comp
+00019260: 6172 6520 7477 6f20 656e 7469 7469 6573  are two entities
+00019270: 206f 6620 7468 6520 7361 6d65 2063 6c61   of the same cla
+00019280: 7373 2066 6f72 2065 7175 616c 6974 792e  ss for equality.
+00019290: 2222 220a 2020 2020 6966 206f 7468 6572  """.    if other
+000192a0: 2e5f 5f63 6c61 7373 5f5f 2069 7320 6e6f  .__class__ is no
+000192b0: 7420 7365 6c66 2e5f 5f63 6c61 7373 5f5f  t self.__class__
+000192c0: 3a0a 2020 2020 2020 7265 7475 726e 204e  :.      return N
+000192d0: 6f74 496d 706c 656d 656e 7465 640a 2020  otImplemented.  
+000192e0: 2020 6966 2073 656c 662e 5f6b 6579 2021    if self._key !
+000192f0: 3d20 6f74 6865 722e 5f6b 6579 3a0a 0a0a  = other._key:...
+00019300: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00019310: 7365 0a20 2020 2072 6574 7572 6e20 7365  se.    return se
+00019320: 6c66 2e5f 6571 7569 7661 6c65 6e74 286f  lf._equivalent(o
+00019330: 7468 6572 290a 0a20 2064 6566 205f 6571  ther)..  def _eq
+00019340: 7569 7661 6c65 6e74 2873 656c 662c 206f  uivalent(self, o
+00019350: 7468 6572 293a 0a20 2020 2022 2222 436f  ther):.    """Co
+00019360: 6d70 6172 6520 7477 6f20 656e 7469 7469  mpare two entiti
+00019370: 6573 206f 6620 7468 6520 7361 6d65 2063  es of the same c
+00019380: 6c61 7373 2c20 6578 636c 7564 696e 6720  lass, excluding 
+00019390: 6b65 7973 2e22 2222 0a20 2020 2069 6620  keys.""".    if 
+000193a0: 6f74 6865 722e 5f5f 636c 6173 735f 5f20  other.__class__ 
+000193b0: 6973 206e 6f74 2073 656c 662e 5f5f 636c  is not self.__cl
+000193c0: 6173 735f 5f3a 0a20 2020 2020 2072 6169  ass__:.      rai
+000193d0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
+000193e0: 6445 7272 6f72 2827 4361 6e6e 6f74 2063  dError('Cannot c
+000193f0: 6f6d 7061 7265 2064 6966 6665 7265 6e74  ompare different
+00019400: 206d 6f64 656c 2063 6c61 7373 6573 2e20   model classes. 
+00019410: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00019420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019430: 2020 2725 7320 6973 206e 6f74 2025 7327    '%s is not %s'
+00019440: 2025 2028 7365 6c66 2e5f 5f63 6c61 7373   % (self.__class
+00019450: 5f5f 2e5f 5f6e 616d 655f 5f2c 0a20 2020  __.__name__,.   
+00019460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019480: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00019490: 7468 6572 2e5f 5f63 6c61 7373 5f2e 5f5f  ther.__class_.__
+000194a0: 6e61 6d65 5f5f 2929 0a20 2020 2069 6620  name__)).    if 
+000194b0: 7365 7428 7365 6c66 2e5f 7072 6f6a 6563  set(self._projec
+000194c0: 7469 6f6e 2920 213d 2073 6574 286f 7468  tion) != set(oth
+000194d0: 6572 2e5f 7072 6f6a 6563 7469 6f6e 293a  er._projection):
+000194e0: 0a20 2020 2020 2072 6574 7572 6e20 4661  .      return Fa
+000194f0: 6c73 650a 0a20 2020 2069 6620 6c65 6e28  lse..    if len(
+00019500: 7365 6c66 2e5f 7072 6f70 6572 7469 6573  self._properties
+00019510: 2920 213d 206c 656e 286f 7468 6572 2e5f  ) != len(other._
+00019520: 7072 6f70 6572 7469 6573 293a 0a20 2020  properties):.   
+00019530: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00019540: 2020 2020 6d79 5f70 726f 705f 6e61 6d65      my_prop_name
+00019550: 7320 3d20 7365 7428 7369 782e 6974 6572  s = set(six.iter
+00019560: 6b65 7973 2873 656c 662e 5f70 726f 7065  keys(self._prope
+00019570: 7274 6965 7329 290a 2020 2020 7468 6569  rties)).    thei
+00019580: 725f 7072 6f70 5f6e 616d 6573 203d 2073  r_prop_names = s
+00019590: 6574 2873 6978 2e69 7465 726b 6579 7328  et(six.iterkeys(
+000195a0: 6f74 6865 722e 5f70 726f 7065 7274 6965  other._propertie
+000195b0: 7329 290a 2020 2020 6966 206d 795f 7072  s)).    if my_pr
+000195c0: 6f70 5f6e 616d 6573 2021 3d20 7468 6569  op_names != thei
+000195d0: 725f 7072 6f70 5f6e 616d 6573 3a0a 2020  r_prop_names:.  
+000195e0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000195f0: 0a20 2020 2069 6620 7365 6c66 2e5f 7072  .    if self._pr
+00019600: 6f6a 6563 7469 6f6e 3a0a 2020 2020 2020  ojection:.      
+00019610: 6d79 5f70 726f 705f 6e61 6d65 7320 3d20  my_prop_names = 
+00019620: 7365 7428 7365 6c66 2e5f 7072 6f6a 6563  set(self._projec
+00019630: 7469 6f6e 290a 2020 2020 666f 7220 6e61  tion).    for na
+00019640: 6d65 2069 6e20 6d79 5f70 726f 705f 6e61  me in my_prop_na
+00019650: 6d65 733a 0a20 2020 2020 206e 616d 6520  mes:.      name 
+00019660: 3d20 7369 782e 656e 7375 7265 5f74 6578  = six.ensure_tex
+00019670: 7428 6e61 6d65 290a 2020 2020 2020 6966  t(name).      if
+00019680: 2027 2e27 2069 6e20 6e61 6d65 3a0a 2020   '.' in name:.  
+00019690: 2020 2020 2020 6e61 6d65 2c20 5f20 3d20        name, _ = 
+000196a0: 6e61 6d65 2e73 706c 6974 2827 2e27 2c20  name.split('.', 
+000196b0: 3129 0a20 2020 2020 206d 795f 7661 6c75  1).      my_valu
+000196c0: 6520 3d20 7365 6c66 2e5f 7072 6f70 6572  e = self._proper
+000196d0: 7469 6573 5b6e 616d 655d 2e5f 6765 745f  ties[name]._get_
+000196e0: 7661 6c75 6528 7365 6c66 290a 2020 2020  value(self).    
+000196f0: 2020 7468 6569 725f 7661 6c75 6520 3d20    their_value = 
+00019700: 6f74 6865 722e 5f70 726f 7065 7274 6965  other._propertie
+00019710: 735b 6e61 6d65 5d2e 5f67 6574 5f76 616c  s[name]._get_val
+00019720: 7565 286f 7468 6572 290a 2020 2020 2020  ue(other).      
+00019730: 6966 206d 795f 7661 6c75 6520 213d 2074  if my_value != t
+00019740: 6865 6972 5f76 616c 7565 3a0a 2020 2020  heir_value:.    
+00019750: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00019760: 0a20 2020 2072 6574 7572 6e20 5472 7565  .    return True
+00019770: 0a0a 2020 6465 6620 5f74 6f5f 7062 2873  ..  def _to_pb(s
+00019780: 656c 662c 2070 623d 4e6f 6e65 2c20 616c  elf, pb=None, al
+00019790: 6c6f 775f 7061 7274 6961 6c3d 4661 6c73  low_partial=Fals
+000197a0: 652c 2073 6574 5f6b 6579 3d54 7275 6529  e, set_key=True)
+000197b0: 3a0a 2020 2020 2222 2249 6e74 6572 6e61  :.    """Interna
+000197c0: 6c20 6865 6c70 6572 2074 6f20 7475 726e  l helper to turn
+000197d0: 2061 6e20 656e 7469 7479 2069 6e74 6f20   an entity into 
+000197e0: 616e 2045 6e74 6974 7950 726f 746f 2070  an EntityProto p
+000197f0: 726f 746f 6275 662e 2222 220a 2020 2020  rotobuf.""".    
+00019800: 6966 206e 6f74 2061 6c6c 6f77 5f70 6172  if not allow_par
+00019810: 7469 616c 3a0a 2020 2020 2020 7365 6c66  tial:.      self
+00019820: 2e5f 6368 6563 6b5f 696e 6974 6961 6c69  ._check_initiali
+00019830: 7a65 6428 290a 2020 2020 6966 2070 6220  zed().    if pb 
+00019840: 6973 204e 6f6e 653a 0a20 2020 2020 2070  is None:.      p
+00019850: 6220 3d20 656e 7469 7479 5f70 6232 2e45  b = entity_pb2.E
+00019860: 6e74 6974 7950 726f 746f 2829 0a0a 2020  ntityProto()..  
+00019870: 2020 6966 2073 6574 5f6b 6579 3a0a 0a20    if set_key:.. 
+00019880: 2020 2020 2073 656c 662e 5f6b 6579 5f74       self._key_t
+00019890: 6f5f 7062 2870 6229 0a0a 2020 2020 666f  o_pb(pb)..    fo
+000198a0: 7220 756e 7573 6564 5f6e 616d 652c 2070  r unused_name, p
+000198b0: 726f 7020 696e 2073 6f72 7465 6428 7369  rop in sorted(si
+000198c0: 782e 6974 6572 6974 656d 7328 7365 6c66  x.iteritems(self
+000198d0: 2e5f 7072 6f70 6572 7469 6573 2929 3a0a  ._properties)):.
+000198e0: 2020 2020 2020 7072 6f70 2e5f 7365 7269        prop._seri
+000198f0: 616c 697a 6528 7365 6c66 2c20 7062 2c20  alize(self, pb, 
+00019900: 7072 6f6a 6563 7469 6f6e 3d73 656c 662e  projection=self.
+00019910: 5f70 726f 6a65 6374 696f 6e29 0a0a 2020  _projection)..  
+00019920: 2020 7265 7475 726e 2070 620a 0a20 2064    return pb..  d
+00019930: 6566 205f 6b65 795f 746f 5f70 6228 7365  ef _key_to_pb(se
+00019940: 6c66 2c20 7062 293a 0a20 2020 2022 2222  lf, pb):.    """
+00019950: 496e 7465 726e 616c 2068 656c 7065 7220  Internal helper 
+00019960: 746f 2063 6f70 7920 7468 6520 6b65 7920  to copy the key 
+00019970: 696e 746f 2061 2070 726f 746f 6275 662e  into a protobuf.
+00019980: 2222 220a 2020 2020 6b65 7920 3d20 7365  """.    key = se
+00019990: 6c66 2e5f 6b65 790a 2020 2020 6966 206b  lf._key.    if k
+000199a0: 6579 2069 7320 4e6f 6e65 3a0a 2020 2020  ey is None:.    
+000199b0: 2020 7061 6972 7320 3d20 5b28 7365 6c66    pairs = [(self
+000199c0: 2e5f 6765 745f 6b69 6e64 2829 2c20 4e6f  ._get_kind(), No
+000199d0: 6e65 295d 0a20 2020 2020 2072 6566 203d  ne)].      ref =
+000199e0: 206b 6579 5f6d 6f64 756c 652e 5f52 6566   key_module._Ref
+000199f0: 6572 656e 6365 4672 6f6d 5061 6972 7328  erenceFromPairs(
+00019a00: 7061 6972 732c 2072 6566 6572 656e 6365  pairs, reference
+00019a10: 3d70 622e 6b65 7929 0a20 2020 2065 6c73  =pb.key).    els
+00019a20: 653a 0a20 2020 2020 2072 6566 203d 206b  e:.      ref = k
+00019a30: 6579 2e72 6566 6572 656e 6365 2829 0a20  ey.reference(). 
+00019a40: 2020 2020 2070 622e 6b65 792e 436f 7079       pb.key.Copy
+00019a50: 4672 6f6d 2872 6566 290a 2020 2020 7062  From(ref).    pb
+00019a60: 2e65 6e74 6974 795f 6772 6f75 702e 5365  .entity_group.Se
+00019a70: 7449 6e50 6172 656e 7428 290a 2020 2020  tInParent().    
+00019a80: 6772 6f75 7020 3d20 7062 2e65 6e74 6974  group = pb.entit
+00019a90: 795f 6772 6f75 700a 0a0a 2020 2020 6966  y_group...    if
+00019aa0: 206b 6579 2069 7320 6e6f 7420 4e6f 6e65   key is not None
+00019ab0: 2061 6e64 206b 6579 2e69 6428 293a 0a20   and key.id():. 
+00019ac0: 2020 2020 2065 6c65 6d20 3d20 7265 662e       elem = ref.
+00019ad0: 7061 7468 2e65 6c65 6d65 6e74 5b30 5d0a  path.element[0].
+00019ae0: 2020 2020 2020 6966 2065 6c65 6d2e 6964        if elem.id
+00019af0: 206f 7220 656c 656d 2e6e 616d 653a 0a20   or elem.name:. 
+00019b00: 2020 2020 2020 2067 726f 7570 2e65 6c65         group.ele
+00019b10: 6d65 6e74 2e61 6464 2829 2e43 6f70 7946  ment.add().CopyF
+00019b20: 726f 6d28 656c 656d 290a 0a20 2040 636c  rom(elem)..  @cl
+00019b30: 6173 736d 6574 686f 640a 2020 6465 6620  assmethod.  def 
+00019b40: 5f66 726f 6d5f 7062 2863 6c73 2c20 7062  _from_pb(cls, pb
+00019b50: 2c20 7365 745f 6b65 793d 5472 7565 2c20  , set_key=True, 
+00019b60: 656e 743d 4e6f 6e65 2c20 6b65 793d 4e6f  ent=None, key=No
+00019b70: 6e65 293a 0a20 2020 2022 2222 496e 7465  ne):.    """Inte
+00019b80: 726e 616c 2068 656c 7065 7220 746f 2063  rnal helper to c
+00019b90: 7265 6174 6520 616e 2065 6e74 6974 7920  reate an entity 
+00019ba0: 6672 6f6d 2061 6e20 456e 7469 7479 5072  from an EntityPr
+00019bb0: 6f74 6f20 7072 6f74 6f62 7566 2e22 2222  oto protobuf."""
+00019bc0: 0a20 2020 2069 6620 6e6f 7420 6973 696e  .    if not isin
+00019bd0: 7374 616e 6365 2870 622c 2065 6e74 6974  stance(pb, entit
+00019be0: 795f 7062 322e 456e 7469 7479 5072 6f74  y_pb2.EntityProt
+00019bf0: 6f29 3a0a 2020 2020 2020 7261 6973 6520  o):.      raise 
+00019c00: 5479 7065 4572 726f 7228 2770 6220 6d75  TypeError('pb mu
+00019c10: 7374 2062 6520 6120 456e 7469 7479 5072  st be a EntityPr
+00019c20: 6f74 6f3b 2072 6563 6569 7665 6420 2572  oto; received %r
+00019c30: 2720 2520 7062 290a 2020 2020 6966 2065  ' % pb).    if e
+00019c40: 6e74 2069 7320 4e6f 6e65 3a0a 2020 2020  nt is None:.    
+00019c50: 2020 656e 7420 3d20 636c 7328 290a 0a0a    ent = cls()...
+00019c60: 2020 2020 6966 206b 6579 2069 7320 4e6f      if key is No
+00019c70: 6e65 2061 6e64 206c 656e 2870 622e 6b65  ne and len(pb.ke
+00019c80: 792e 7061 7468 2e65 6c65 6d65 6e74 293a  y.path.element):
+00019c90: 0a20 2020 2020 206b 6579 203d 204b 6579  .      key = Key
+00019ca0: 2872 6566 6572 656e 6365 3d70 622e 6b65  (reference=pb.ke
+00019cb0: 7929 0a0a 2020 2020 6966 206b 6579 2069  y)..    if key i
+00019cc0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2028  s not None and (
+00019cd0: 7365 745f 6b65 7920 6f72 206b 6579 2e69  set_key or key.i
+00019ce0: 6428 2920 6f72 206b 6579 2e70 6172 656e  d() or key.paren
+00019cf0: 7428 2929 3a0a 2020 2020 2020 656e 742e  t()):.      ent.
+00019d00: 5f6b 6579 203d 206b 6579 0a0a 0a0a 0a20  _key = key..... 
+00019d10: 2020 205f 7072 6f70 6572 7479 5f6d 6170     _property_map
+00019d20: 203d 207b 7d0a 2020 2020 7072 6f6a 6563   = {}.    projec
+00019d30: 7469 6f6e 203d 205b 5d0a 2020 2020 666f  tion = [].    fo
+00019d40: 7220 696e 6465 7865 642c 2070 6c69 7374  r indexed, plist
+00019d50: 2069 6e20 2828 5472 7565 2c20 7062 2e70   in ((True, pb.p
+00019d60: 726f 7065 7274 7929 2c20 2846 616c 7365  roperty), (False
+00019d70: 2c20 7062 2e72 6177 5f70 726f 7065 7274  , pb.raw_propert
+00019d80: 7929 293a 0a20 2020 2020 2066 6f72 2070  y)):.      for p
+00019d90: 2069 6e20 706c 6973 743a 0a20 2020 2020   in plist:.     
+00019da0: 2020 2070 726f 705f 6e61 6d65 203d 2073     prop_name = s
+00019db0: 6978 2e65 6e73 7572 655f 7465 7874 2870  ix.ensure_text(p
+00019dc0: 2e6e 616d 6529 0a20 2020 2020 2020 2069  .name).        i
+00019dd0: 6620 702e 6d65 616e 696e 6720 3d3d 2065  f p.meaning == e
+00019de0: 6e74 6974 795f 7062 322e 5072 6f70 6572  ntity_pb2.Proper
+00019df0: 7479 2e49 4e44 4558 5f56 414c 5545 3a0a  ty.INDEX_VALUE:.
+00019e00: 2020 2020 2020 2020 2020 7072 6f6a 6563            projec
+00019e10: 7469 6f6e 2e61 7070 656e 6428 7072 6f70  tion.append(prop
+00019e20: 5f6e 616d 6529 0a20 2020 2020 2020 2070  _name).        p
+00019e30: 726f 7065 7274 795f 6d61 705f 6b65 7920  roperty_map_key 
+00019e40: 3d20 2870 726f 705f 6e61 6d65 2c20 696e  = (prop_name, in
+00019e50: 6465 7865 6429 0a20 2020 2020 2020 2069  dexed).        i
+00019e60: 6620 7072 6f70 6572 7479 5f6d 6170 5f6b  f property_map_k
+00019e70: 6579 206e 6f74 2069 6e20 5f70 726f 7065  ey not in _prope
+00019e80: 7274 795f 6d61 703a 0a20 2020 2020 2020  rty_map:.       
+00019e90: 2020 205f 7072 6f70 6572 7479 5f6d 6170     _property_map
+00019ea0: 5b70 726f 7065 7274 795f 6d61 705f 6b65  [property_map_ke
+00019eb0: 795d 203d 2065 6e74 2e5f 6765 745f 7072  y] = ent._get_pr
+00019ec0: 6f70 6572 7479 5f66 6f72 2870 2c20 696e  operty_for(p, in
+00019ed0: 6465 7865 6429 0a20 2020 2020 2020 205f  dexed).        _
+00019ee0: 7072 6f70 6572 7479 5f6d 6170 5b70 726f  property_map[pro
+00019ef0: 7065 7274 795f 6d61 705f 6b65 795d 2e5f  perty_map_key]._
+00019f00: 6465 7365 7269 616c 697a 6528 656e 742c  deserialize(ent,
+00019f10: 2070 290a 0a20 2020 2065 6e74 2e5f 7365   p)..    ent._se
+00019f20: 745f 7072 6f6a 6563 7469 6f6e 2870 726f  t_projection(pro
+00019f30: 6a65 6374 696f 6e29 0a20 2020 2072 6574  jection).    ret
+00019f40: 7572 6e20 656e 740a 0a20 2064 6566 205f  urn ent..  def _
+00019f50: 7365 745f 7072 6f6a 6563 7469 6f6e 2873  set_projection(s
+00019f60: 656c 662c 2070 726f 6a65 6374 696f 6e29  elf, projection)
+00019f70: 3a0a 2020 2020 6279 5f70 7265 6669 7820  :.    by_prefix 
+00019f80: 3d20 7b7d 0a20 2020 2066 6f72 2070 726f  = {}.    for pro
+00019f90: 706e 616d 6520 696e 2070 726f 6a65 6374  pname in project
+00019fa0: 696f 6e3a 0a20 2020 2020 2069 6620 272e  ion:.      if '.
+00019fb0: 2720 696e 2070 726f 706e 616d 653a 0a20  ' in propname:. 
+00019fc0: 2020 2020 2020 2068 6561 642c 2074 6169         head, tai
+00019fd0: 6c20 3d20 7072 6f70 6e61 6d65 2e73 706c  l = propname.spl
+00019fe0: 6974 2827 2e27 2c20 3129 0a20 2020 2020  it('.', 1).     
+00019ff0: 2020 2069 6620 6865 6164 2069 6e20 6279     if head in by
+0001a000: 5f70 7265 6669 783a 0a20 2020 2020 2020  _prefix:.       
+0001a010: 2020 2062 795f 7072 6566 6978 5b68 6561     by_prefix[hea
+0001a020: 645d 2e61 7070 656e 6428 7461 696c 290a  d].append(tail).
+0001a030: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001a040: 2020 2020 2020 2020 6279 5f70 7265 6669          by_prefi
+0001a050: 785b 6865 6164 5d20 3d20 5b74 6169 6c5d  x[head] = [tail]
+0001a060: 0a20 2020 2073 656c 662e 5f70 726f 6a65  .    self._proje
+0001a070: 6374 696f 6e20 3d20 7475 706c 6528 7072  ction = tuple(pr
+0001a080: 6f6a 6563 7469 6f6e 290a 2020 2020 666f  ojection).    fo
+0001a090: 7220 7072 6f70 6e61 6d65 2c20 7072 6f6a  r propname, proj
+0001a0a0: 2069 6e20 7369 782e 6974 6572 6974 656d   in six.iteritem
+0001a0b0: 7328 6279 5f70 7265 6669 7829 3a0a 2020  s(by_prefix):.  
+0001a0c0: 2020 2020 7072 6f70 203d 2073 656c 662e      prop = self.
+0001a0d0: 5f70 726f 7065 7274 6965 732e 6765 7428  _properties.get(
+0001a0e0: 7072 6f70 6e61 6d65 290a 2020 2020 2020  propname).      
+0001a0f0: 7375 6276 616c 203d 2070 726f 702e 5f67  subval = prop._g
+0001a100: 6574 5f62 6173 655f 7661 6c75 655f 756e  et_base_value_un
+0001a110: 7772 6170 7065 645f 6173 5f6c 6973 7428  wrapped_as_list(
+0001a120: 7365 6c66 290a 2020 2020 2020 666f 7220  self).      for 
+0001a130: 6974 656d 2069 6e20 7375 6276 616c 3a0a  item in subval:.
+0001a140: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+0001a150: 7465 6d20 6973 206e 6f74 204e 6f6e 650a  tem is not None.
+0001a160: 2020 2020 2020 2020 6974 656d 2e5f 7365          item._se
+0001a170: 745f 7072 6f6a 6563 7469 6f6e 2870 726f  t_projection(pro
+0001a180: 6a29 0a0a 2020 6465 6620 5f67 6574 5f70  j)..  def _get_p
+0001a190: 726f 7065 7274 795f 666f 7228 7365 6c66  roperty_for(self
+0001a1a0: 2c20 702c 2069 6e64 6578 6564 3d54 7275  , p, indexed=Tru
+0001a1b0: 652c 2064 6570 7468 3d30 293a 0a20 2020  e, depth=0):.   
+0001a1c0: 2022 2222 496e 7465 726e 616c 2068 656c   """Internal hel
+0001a1d0: 7065 7220 746f 2067 6574 2074 6865 2050  per to get the P
+0001a1e0: 726f 7065 7274 7920 666f 7220 6120 7072  roperty for a pr
+0001a1f0: 6f74 6f62 7566 2d6c 6576 656c 2070 726f  otobuf-level pro
+0001a200: 7065 7274 792e 2222 220a 2020 2020 7061  perty.""".    pa
+0001a210: 7274 7320 3d20 702e 6e61 6d65 2e73 706c  rts = p.name.spl
+0001a220: 6974 2827 2e27 290a 2020 2020 6966 206c  it('.').    if l
+0001a230: 656e 2870 6172 7473 2920 3c3d 2064 6570  en(parts) <= dep
+0001a240: 7468 3a0a 0a0a 0a0a 0a0a 2020 2020 2020  th:.......      
+0001a250: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
+0001a260: 6e65 7874 203d 2070 6172 7473 5b64 6570  next = parts[dep
+0001a270: 7468 5d0a 2020 2020 7072 6f70 203d 2073  th].    prop = s
+0001a280: 656c 662e 5f70 726f 7065 7274 6965 732e  elf._properties.
+0001a290: 6765 7428 6e65 7874 290a 2020 2020 6966  get(next).    if
+0001a2a0: 2070 726f 7020 6973 204e 6f6e 653a 0a20   prop is None:. 
+0001a2b0: 2020 2020 2070 726f 7020 3d20 7365 6c66       prop = self
+0001a2c0: 2e5f 6661 6b65 5f70 726f 7065 7274 7928  ._fake_property(
+0001a2d0: 702c 206e 6578 742c 2069 6e64 6578 6564  p, next, indexed
+0001a2e0: 290a 2020 2020 7265 7475 726e 2070 726f  ).    return pro
+0001a2f0: 700a 0a20 2064 6566 205f 636c 6f6e 655f  p..  def _clone_
+0001a300: 7072 6f70 6572 7469 6573 2873 656c 6629  properties(self)
+0001a310: 3a0a 2020 2020 2222 2249 6e74 6572 6e61  :.    """Interna
+0001a320: 6c20 6865 6c70 6572 2074 6f20 636c 6f6e  l helper to clon
+0001a330: 6520 7365 6c66 2e5f 7072 6f70 6572 7469  e self._properti
+0001a340: 6573 2069 6620 6e65 6365 7373 6172 792e  es if necessary.
+0001a350: 2222 220a 2020 2020 636c 7320 3d20 7365  """.    cls = se
+0001a360: 6c66 2e5f 5f63 6c61 7373 5f5f 0a20 2020  lf.__class__.   
+0001a370: 2069 6620 7365 6c66 2e5f 7072 6f70 6572   if self._proper
+0001a380: 7469 6573 2069 7320 636c 732e 5f70 726f  ties is cls._pro
+0001a390: 7065 7274 6965 733a 0a20 2020 2020 2073  perties:.      s
+0001a3a0: 656c 662e 5f70 726f 7065 7274 6965 7320  elf._properties 
+0001a3b0: 3d20 6469 6374 2863 6c73 2e5f 7072 6f70  = dict(cls._prop
+0001a3c0: 6572 7469 6573 290a 0a20 2064 6566 205f  erties)..  def _
+0001a3d0: 6661 6b65 5f70 726f 7065 7274 7928 7365  fake_property(se
+0001a3e0: 6c66 2c20 702c 206e 6578 742c 2069 6e64  lf, p, next, ind
+0001a3f0: 6578 6564 3d54 7275 6529 3a0a 2020 2020  exed=True):.    
+0001a400: 2222 2249 6e74 6572 6e61 6c20 6865 6c70  """Internal help
+0001a410: 6572 2074 6f20 6372 6561 7465 2061 2066  er to create a f
+0001a420: 616b 6520 5072 6f70 6572 7479 2e22 2222  ake Property."""
+0001a430: 0a20 2020 2073 656c 662e 5f63 6c6f 6e65  .    self._clone
+0001a440: 5f70 726f 7065 7274 6965 7328 290a 2020  _properties().  
+0001a450: 2020 6966 2070 2e6e 616d 6520 213d 206e    if p.name != n
+0001a460: 6578 7420 616e 6420 6e6f 7420 702e 6e61  ext and not p.na
+0001a470: 6d65 2e65 6e64 7377 6974 6828 272e 2720  me.endswith('.' 
+0001a480: 2b20 6e65 7874 293a 0a20 2020 2020 2070  + next):.      p
+0001a490: 726f 7020 3d20 5374 7275 6374 7572 6564  rop = Structured
+0001a4a0: 5072 6f70 6572 7479 2845 7870 616e 646f  Property(Expando
+0001a4b0: 2c20 6e65 7874 290a 2020 2020 2020 7072  , next).      pr
+0001a4c0: 6f70 2e5f 7374 6f72 655f 7661 6c75 6528  op._store_value(
+0001a4d0: 7365 6c66 2c20 5f42 6173 6556 616c 7565  self, _BaseValue
+0001a4e0: 2845 7870 616e 646f 2829 2929 0a20 2020  (Expando())).   
+0001a4f0: 2065 6c73 653a 0a20 2020 2020 2063 6f6d   else:.      com
+0001a500: 7072 6573 7365 6420 3d20 702e 6d65 616e  pressed = p.mean
+0001a510: 696e 675f 7572 6920 3d3d 205f 4d45 414e  ing_uri == _MEAN
+0001a520: 494e 475f 5552 495f 434f 4d50 5245 5353  ING_URI_COMPRESS
+0001a530: 4544 0a20 2020 2020 2070 726f 7020 3d20  ED.      prop = 
+0001a540: 4765 6e65 7269 6350 726f 7065 7274 7928  GenericProperty(
+0001a550: 0a20 2020 2020 2020 2020 206e 6578 742c  .          next,
+0001a560: 2072 6570 6561 7465 643d 702e 6d75 6c74   repeated=p.mult
+0001a570: 6970 6c65 2c20 696e 6465 7865 643d 696e  iple, indexed=in
+0001a580: 6465 7865 642c 2063 6f6d 7072 6573 7365  dexed, compresse
+0001a590: 643d 636f 6d70 7265 7373 6564 290a 2020  d=compressed).  
+0001a5a0: 2020 7072 6f70 2e5f 636f 6465 5f6e 616d    prop._code_nam
+0001a5b0: 6520 3d20 6e65 7874 0a20 2020 2073 656c  e = next.    sel
+0001a5c0: 662e 5f70 726f 7065 7274 6965 735b 7072  f._properties[pr
+0001a5d0: 6f70 2e5f 6e61 6d65 2e64 6563 6f64 6528  op._name.decode(
+0001a5e0: 2775 7466 2d38 2729 5d20 3d20 7072 6f70  'utf-8')] = prop
+0001a5f0: 0a20 2020 2072 6574 7572 6e20 7072 6f70  .    return prop
+0001a600: 0a0a 2020 4075 7469 6c73 2e70 6f73 6974  ..  @utils.posit
+0001a610: 696f 6e61 6c28 3129 0a20 2064 6566 205f  ional(1).  def _
+0001a620: 746f 5f64 6963 7428 7365 6c66 2c20 696e  to_dict(self, in
+0001a630: 636c 7564 653d 4e6f 6e65 2c20 6578 636c  clude=None, excl
+0001a640: 7564 653d 4e6f 6e65 293a 0a20 2020 2022  ude=None):.    "
+0001a650: 2222 5265 7475 726e 2061 2064 6963 7420  ""Return a dict 
+0001a660: 636f 6e74 6169 6e69 6e67 2074 6865 2065  containing the e
+0001a670: 6e74 6974 7927 7320 7072 6f70 6572 7479  ntity's property
+0001a680: 2076 616c 7565 732e 0a0a 2020 2020 4172   values...    Ar
+0001a690: 6773 3a0a 2020 2020 2020 696e 636c 7564  gs:.      includ
+0001a6a0: 653a 204f 7074 696f 6e61 6c20 7365 7420  e: Optional set 
+0001a6b0: 6f66 2070 726f 7065 7274 7920 6e61 6d65  of property name
+0001a6c0: 7320 746f 2069 6e63 6c75 6465 2c20 6465  s to include, de
+0001a6d0: 6661 756c 7420 616c 6c2e 0a20 2020 2020  fault all..     
+0001a6e0: 2065 7863 6c75 6465 3a20 4f70 7469 6f6e   exclude: Option
+0001a6f0: 616c 2073 6574 206f 6620 7072 6f70 6572  al set of proper
+0001a700: 7479 206e 616d 6573 2074 6f20 736b 6970  ty names to skip
+0001a710: 2c20 6465 6661 756c 7420 6e6f 6e65 2e0a  , default none..
+0001a720: 2020 2020 2020 2020 4120 6e61 6d65 2063          A name c
+0001a730: 6f6e 7461 696e 6564 2069 6e20 626f 7468  ontained in both
+0001a740: 2069 6e63 6c75 6465 2061 6e64 2065 7863   include and exc
+0001a750: 6c75 6465 2069 7320 6578 636c 7564 6564  lude is excluded
+0001a760: 2e0a 2020 2020 2222 220a 2020 2020 6966  ..    """.    if
+0001a770: 2028 696e 636c 7564 6520 6973 206e 6f74   (include is not
+0001a780: 204e 6f6e 6520 616e 640a 2020 2020 2020   None and.      
+0001a790: 2020 6e6f 7420 6973 696e 7374 616e 6365    not isinstance
+0001a7a0: 2869 6e63 6c75 6465 2c20 286c 6973 742c  (include, (list,
+0001a7b0: 2074 7570 6c65 2c20 7365 742c 2066 726f   tuple, set, fro
+0001a7c0: 7a65 6e73 6574 2929 293a 0a20 2020 2020  zenset))):.     
+0001a7d0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+0001a7e0: 2827 696e 636c 7564 6520 7368 6f75 6c64  ('include should
+0001a7f0: 2062 6520 6120 6c69 7374 2c20 7475 706c   be a list, tupl
+0001a800: 6520 6f72 2073 6574 2729 0a20 2020 2069  e or set').    i
+0001a810: 6620 2865 7863 6c75 6465 2069 7320 6e6f  f (exclude is no
+0001a820: 7420 4e6f 6e65 2061 6e64 0a20 2020 2020  t None and.     
+0001a830: 2020 206e 6f74 2069 7369 6e73 7461 6e63     not isinstanc
+0001a840: 6528 6578 636c 7564 652c 2028 6c69 7374  e(exclude, (list
+0001a850: 2c20 7475 706c 652c 2073 6574 2c20 6672  , tuple, set, fr
+0001a860: 6f7a 656e 7365 7429 2929 3a0a 2020 2020  ozenset))):.    
+0001a870: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
+0001a880: 7228 2765 7863 6c75 6465 2073 686f 756c  r('exclude shoul
+0001a890: 6420 6265 2061 206c 6973 742c 2074 7570  d be a list, tup
+0001a8a0: 6c65 206f 7220 7365 7427 290a 2020 2020  le or set').    
+0001a8b0: 7661 6c75 6573 203d 207b 7d0a 2020 2020  values = {}.    
+0001a8c0: 666f 7220 7072 6f70 2069 6e20 7369 782e  for prop in six.
+0001a8d0: 6974 6572 7661 6c75 6573 2873 656c 662e  itervalues(self.
+0001a8e0: 5f70 726f 7065 7274 6965 7329 3a0a 2020  _properties):.  
+0001a8f0: 2020 2020 6e61 6d65 203d 2070 726f 702e      name = prop.
+0001a900: 5f63 6f64 655f 6e61 6d65 0a20 2020 2020  _code_name.     
+0001a910: 2069 6620 696e 636c 7564 6520 6973 206e   if include is n
+0001a920: 6f74 204e 6f6e 6520 616e 6420 6e61 6d65  ot None and name
+0001a930: 206e 6f74 2069 6e20 696e 636c 7564 653a   not in include:
+0001a940: 0a20 2020 2020 2020 2063 6f6e 7469 6e75  .        continu
+0001a950: 650a 2020 2020 2020 6966 2065 7863 6c75  e.      if exclu
+0001a960: 6465 2069 7320 6e6f 7420 4e6f 6e65 2061  de is not None a
+0001a970: 6e64 206e 616d 6520 696e 2065 7863 6c75  nd name in exclu
+0001a980: 6465 3a0a 2020 2020 2020 2020 636f 6e74  de:.        cont
+0001a990: 696e 7565 0a20 2020 2020 2074 7279 3a0a  inue.      try:.
+0001a9a0: 2020 2020 2020 2020 7661 6c75 6573 5b6e          values[n
+0001a9b0: 616d 655d 203d 2070 726f 702e 5f67 6574  ame] = prop._get
+0001a9c0: 5f66 6f72 5f64 6963 7428 7365 6c66 290a  _for_dict(self).
+0001a9d0: 2020 2020 2020 6578 6365 7074 2055 6e70        except Unp
+0001a9e0: 726f 6a65 6374 6564 5072 6f70 6572 7479  rojectedProperty
+0001a9f0: 4572 726f 723a 0a20 2020 2020 2020 2070  Error:.        p
+0001aa00: 6173 730a 2020 2020 7265 7475 726e 2076  ass.    return v
+0001aa10: 616c 7565 730a 2020 746f 5f64 6963 7420  alues.  to_dict 
+0001aa20: 3d20 5f74 6f5f 6469 6374 0a0a 2020 4063  = _to_dict..  @c
+0001aa30: 6c61 7373 6d65 7468 6f64 0a20 2064 6566  lassmethod.  def
+0001aa40: 205f 6669 785f 7570 5f70 726f 7065 7274   _fix_up_propert
+0001aa50: 6965 7328 636c 7329 3a0a 2020 2020 2222  ies(cls):.    ""
+0001aa60: 2246 6978 2075 7020 7468 6520 7072 6f70  "Fix up the prop
+0001aa70: 6572 7469 6573 2062 7920 6361 6c6c 696e  erties by callin
+0001aa80: 6720 7468 6569 7220 5f66 6978 5f75 7028  g their _fix_up(
+0001aa90: 2920 6d65 7468 6f64 2e0a 0a20 2020 204e  ) method...    N
+0001aaa0: 6f74 653a 2054 6869 7320 6973 2063 616c  ote: This is cal
+0001aab0: 6c65 6420 6279 204d 6574 614d 6f64 656c  led by MetaModel
+0001aac0: 2c20 6275 7420 6d61 7920 616c 736f 2062  , but may also b
+0001aad0: 6520 6361 6c6c 6564 206d 616e 7561 6c6c  e called manuall
+0001aae0: 790a 2020 2020 6166 7465 7220 6479 6e61  y.    after dyna
+0001aaf0: 6d69 6361 6c6c 7920 7570 6461 7469 6e67  mically updating
+0001ab00: 2061 206d 6f64 656c 2063 6c61 7373 2e0a   a model class..
+0001ab10: 2020 2020 2222 220a 0a20 2020 206b 696e      """..    kin
+0001ab20: 6420 3d20 636c 732e 5f67 6574 5f6b 696e  d = cls._get_kin
+0001ab30: 6428 290a 2020 2020 6966 206e 6f74 2069  d().    if not i
+0001ab40: 7369 6e73 7461 6e63 6528 6b69 6e64 2c20  sinstance(kind, 
+0001ab50: 2873 6978 2e74 6578 745f 7479 7065 2c20  (six.text_type, 
+0001ab60: 7369 782e 6269 6e61 7279 5f74 7970 6529  six.binary_type)
+0001ab70: 293a 0a20 2020 2020 2072 6169 7365 204b  ):.      raise K
+0001ab80: 696e 6445 7272 6f72 2827 436c 6173 7320  indError('Class 
+0001ab90: 2573 2064 6566 696e 6573 2061 205f 6765  %s defines a _ge
+0001aba0: 745f 6b69 6e64 2829 206d 6574 686f 6420  t_kind() method 
+0001abb0: 7468 6174 2072 6574 7572 6e73 2027 0a20  that returns '. 
 0001abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001abd0: 2020 2020 2028 636c 732e 5f5f 6e61 6d65       (cls.__name
-0001abe0: 5f5f 2c20 6b69 6e64 2929 0a20 2020 2063  __, kind)).    c
-0001abf0: 6c73 2e5f 7072 6f70 6572 7469 6573 203d  ls._properties =
-0001ac00: 207b 7d0a 2020 2020 6966 2063 6c73 2e5f   {}.    if cls._
-0001ac10: 5f6d 6f64 756c 655f 5f20 3d3d 205f 5f6e  _module__ == __n
-0001ac20: 616d 655f 5f3a 0a20 2020 2020 2072 6574  ame__:.      ret
-0001ac30: 7572 6e0a 2020 2020 666f 7220 6e61 6d65  urn.    for name
-0001ac40: 2069 6e20 7365 7428 6469 7228 636c 7329   in set(dir(cls)
-0001ac50: 293a 0a20 2020 2020 2061 7474 7220 3d20  ):.      attr = 
-0001ac60: 6765 7461 7474 7228 636c 732c 206e 616d  getattr(cls, nam
-0001ac70: 652c 204e 6f6e 6529 0a20 2020 2020 2069  e, None).      i
-0001ac80: 6620 6973 696e 7374 616e 6365 2861 7474  f isinstance(att
-0001ac90: 722c 204d 6f64 656c 4174 7472 6962 7574  r, ModelAttribut
-0001aca0: 6529 2061 6e64 206e 6f74 2069 7369 6e73  e) and not isins
-0001acb0: 7461 6e63 6528 6174 7472 2c20 4d6f 6465  tance(attr, Mode
-0001acc0: 6c4b 6579 293a 0a20 2020 2020 2020 2069  lKey):.        i
-0001acd0: 6620 6e61 6d65 2e73 7461 7274 7377 6974  f name.startswit
-0001ace0: 6828 275f 2729 3a0a 2020 2020 2020 2020  h('_'):.        
-0001acf0: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-0001ad00: 7228 274d 6f64 656c 4174 7472 6962 7574  r('ModelAttribut
-0001ad10: 6520 2573 2063 616e 6e6f 7420 6265 6769  e %s cannot begi
-0001ad20: 6e20 7769 7468 2061 6e20 756e 6465 7273  n with an unders
-0001ad30: 636f 7265 2027 0a20 2020 2020 2020 2020  core '.         
-0001ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad50: 2027 6368 6172 6163 7465 722e 205f 2070   'character. _ p
-0001ad60: 7265 6669 7865 6420 6174 7472 6962 7574  refixed attribut
-0001ad70: 6573 2061 7265 2072 6573 6572 7665 6420  es are reserved 
-0001ad80: 666f 7220 270a 2020 2020 2020 2020 2020  for '.          
-0001ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ada0: 2774 656d 706f 7261 7279 204d 6f64 656c  'temporary Model
-0001adb0: 2069 6e73 7461 6e63 6520 7661 6c75 6573   instance values
-0001adc0: 2e27 2025 206e 616d 6529 0a20 2020 2020  .' % name).     
-0001add0: 2020 2061 7474 722e 5f66 6978 5f75 7028     attr._fix_up(
-0001ade0: 636c 732c 206e 616d 6529 0a20 2020 2020  cls, name).     
-0001adf0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0001ae00: 2861 7474 722c 2050 726f 7065 7274 7929  (attr, Property)
-0001ae10: 3a0a 2020 2020 2020 2020 2020 6966 2028  :.          if (
-0001ae20: 6174 7472 2e5f 7265 7065 6174 6564 206f  attr._repeated o
-0001ae30: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-0001ae40: 2869 7369 6e73 7461 6e63 6528 6174 7472  (isinstance(attr
-0001ae50: 2c20 5374 7275 6374 7572 6564 5072 6f70  , StructuredProp
-0001ae60: 6572 7479 2920 616e 640a 2020 2020 2020  erty) and.      
-0001ae70: 2020 2020 2020 2020 2061 7474 722e 5f6d           attr._m
-0001ae80: 6f64 656c 636c 6173 732e 5f68 6173 5f72  odelclass._has_r
-0001ae90: 6570 6561 7465 6429 293a 0a20 2020 2020  epeated)):.     
-0001aea0: 2020 2020 2020 2063 6c73 2e5f 6861 735f         cls._has_
-0001aeb0: 7265 7065 6174 6564 203d 2054 7275 650a  repeated = True.
-0001aec0: 2020 2020 2020 2020 2020 636c 732e 5f70            cls._p
-0001aed0: 726f 7065 7274 6965 735b 7369 782e 656e  roperties[six.en
-0001aee0: 7375 7265 5f74 6578 7428 6174 7472 2e5f  sure_text(attr._
-0001aef0: 6e61 6d65 295d 203d 2061 7474 720a 2020  name)] = attr.  
-0001af00: 2020 636c 732e 5f75 7064 6174 655f 6b69    cls._update_ki
-0001af10: 6e64 5f6d 6170 2829 0a0a 2020 4063 6c61  nd_map()..  @cla
-0001af20: 7373 6d65 7468 6f64 0a20 2064 6566 205f  ssmethod.  def _
-0001af30: 7570 6461 7465 5f6b 696e 645f 6d61 7028  update_kind_map(
-0001af40: 636c 7329 3a0a 2020 2020 2222 2255 7064  cls):.    """Upd
-0001af50: 6174 6520 7468 6520 6b69 6e64 206d 6170  ate the kind map
-0001af60: 2074 6f20 696e 636c 7564 6520 7468 6973   to include this
-0001af70: 2063 6c61 7373 2e22 2222 0a20 2020 206b   class.""".    k
-0001af80: 203d 2063 6c73 2e5f 6765 745f 6b69 6e64   = cls._get_kind
-0001af90: 2829 0a20 2020 2063 6c73 2e5f 6b69 6e64  ().    cls._kind
-0001afa0: 5f6d 6170 5b6b 5d20 3d20 636c 730a 0a20  _map[k] = cls.. 
-0001afb0: 2064 6566 205f 7072 6570 6172 655f 666f   def _prepare_fo
-0001afc0: 725f 7075 7428 7365 6c66 293a 0a20 2020  r_put(self):.   
-0001afd0: 2069 6620 7365 6c66 2e5f 7072 6f70 6572   if self._proper
-0001afe0: 7469 6573 3a0a 2020 2020 2020 666f 7220  ties:.      for 
-0001aff0: 5f2c 2070 726f 7020 696e 2073 6f72 7465  _, prop in sorte
-0001b000: 6428 7369 782e 6974 6572 6974 656d 7328  d(six.iteritems(
-0001b010: 7365 6c66 2e5f 7072 6f70 6572 7469 6573  self._properties
-0001b020: 2929 3a0a 2020 2020 2020 2020 7072 6f70  )):.        prop
-0001b030: 2e5f 7072 6570 6172 655f 666f 725f 7075  ._prepare_for_pu
-0001b040: 7428 7365 6c66 290a 0a20 2040 636c 6173  t(self)..  @clas
-0001b050: 736d 6574 686f 640a 2020 6465 6620 5f63  smethod.  def _c
-0001b060: 6865 636b 5f70 726f 7065 7274 6965 7328  heck_properties(
-0001b070: 636c 732c 2070 726f 7065 7274 795f 6e61  cls, property_na
-0001b080: 6d65 732c 2072 6571 7569 7265 5f69 6e64  mes, require_ind
-0001b090: 6578 6564 3d54 7275 6529 3a0a 2020 2020  exed=True):.    
-0001b0a0: 2222 2249 6e74 6572 6e61 6c20 6865 6c70  """Internal help
-0001b0b0: 6572 2074 6f20 6368 6563 6b20 7468 6520  er to check the 
-0001b0c0: 6769 7665 6e20 7072 6f70 6572 7469 6573  given properties
-0001b0d0: 2065 7869 7374 2061 6e64 206d 6565 7420   exist and meet 
-0001b0e0: 7370 6563 6966 6965 640a 2020 2020 7265  specified.    re
-0001b0f0: 7175 6972 656d 656e 7473 2e0a 0a20 2020  quirements...   
-0001b100: 2043 616c 6c65 6420 6672 6f6d 2071 7565   Called from que
-0001b110: 7279 2e70 792e 0a0a 2020 2020 4172 6773  ry.py...    Args
-0001b120: 3a0a 2020 2020 2020 7072 6f70 6572 7479  :.      property
-0001b130: 5f6e 616d 6573 3a20 4c69 7374 206f 7220  _names: List or 
-0001b140: 7475 706c 6520 6f66 2070 726f 7065 7274  tuple of propert
-0001b150: 7920 6e61 6d65 7320 2d2d 2065 6163 6820  y names -- each 
-0001b160: 6265 696e 6720 6120 7374 7269 6e67 2c0a  being a string,.
-0001b170: 2020 2020 2020 2020 706f 7373 6962 6c79          possibly
-0001b180: 2063 6f6e 7461 696e 696e 6720 646f 7473   containing dots
-0001b190: 2028 746f 2061 6464 7265 7373 2073 7562   (to address sub
-0001b1a0: 7072 6f70 6572 7469 6573 206f 6620 7374  properties of st
-0001b1b0: 7275 6374 7572 6564 0a20 2020 2020 2020  ructured.       
-0001b1c0: 2070 726f 7065 7274 6965 7329 2e0a 0a20   properties)... 
-0001b1d0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-0001b1e0: 2049 6e76 616c 6964 5072 6f70 6572 7479   InvalidProperty
-0001b1f0: 4572 726f 7220 6966 206f 6e65 206f 6620  Error if one of 
-0001b200: 7468 6520 7072 6f70 6572 7469 6573 2069  the properties i
-0001b210: 7320 696e 7661 6c69 642e 0a20 2020 2020  s invalid..     
-0001b220: 2041 7373 6572 7469 6f6e 4572 726f 7220   AssertionError 
-0001b230: 6966 2074 6865 2061 7267 756d 656e 7420  if the argument 
-0001b240: 6973 206e 6f74 2061 206c 6973 7420 6f72  is not a list or
-0001b250: 2074 7570 6c65 206f 6620 7374 7269 6e67   tuple of string
-0001b260: 732e 0a20 2020 2022 2222 0a20 2020 2061  s..    """.    a
-0001b270: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-0001b280: 2870 726f 7065 7274 795f 6e61 6d65 732c  (property_names,
-0001b290: 2028 6c69 7374 2c20 7475 706c 6529 292c   (list, tuple)),
-0001b2a0: 2072 6570 7228 7072 6f70 6572 7479 5f6e   repr(property_n
-0001b2b0: 616d 6573 290a 2020 2020 666f 7220 6e61  ames).    for na
-0001b2c0: 6d65 2069 6e20 7072 6f70 6572 7479 5f6e  me in property_n
-0001b2d0: 616d 6573 3a0a 2020 2020 2020 6173 7365  ames:.      asse
-0001b2e0: 7274 2069 7369 6e73 7461 6e63 6528 6e61  rt isinstance(na
-0001b2f0: 6d65 2c20 2873 6978 2e74 6578 745f 7479  me, (six.text_ty
-0001b300: 7065 2c20 7369 782e 6269 6e61 7279 5f74  pe, six.binary_t
-0001b310: 7970 6529 292c 2072 6570 7228 6e61 6d65  ype)), repr(name
-0001b320: 290a 2020 2020 2020 6e61 6d65 203d 2073  ).      name = s
-0001b330: 6978 2e65 6e73 7572 655f 7465 7874 286e  ix.ensure_text(n
-0001b340: 616d 6529 0a20 2020 2020 2069 6620 272e  ame).      if '.
-0001b350: 2720 696e 206e 616d 653a 0a20 2020 2020  ' in name:.     
-0001b360: 2020 206e 616d 652c 2072 6573 7420 3d20     name, rest = 
-0001b370: 6e61 6d65 2e73 706c 6974 2827 2e27 2c20  name.split('.', 
-0001b380: 3129 0a20 2020 2020 2065 6c73 653a 0a20  1).      else:. 
-0001b390: 2020 2020 2020 2072 6573 7420 3d20 4e6f         rest = No
-0001b3a0: 6e65 0a20 2020 2020 2070 726f 7020 3d20  ne.      prop = 
-0001b3b0: 636c 732e 5f70 726f 7065 7274 6965 732e  cls._properties.
-0001b3c0: 6765 7428 6e61 6d65 290a 2020 2020 2020  get(name).      
-0001b3d0: 6966 2070 726f 7020 6973 204e 6f6e 653a  if prop is None:
-0001b3e0: 0a20 2020 2020 2020 2063 6c73 2e5f 756e  .        cls._un
-0001b3f0: 6b6e 6f77 6e5f 7072 6f70 6572 7479 286e  known_property(n
-0001b400: 616d 6529 0a20 2020 2020 2065 6c73 653a  ame).      else:
-0001b410: 0a20 2020 2020 2020 2070 726f 702e 5f63  .        prop._c
-0001b420: 6865 636b 5f70 726f 7065 7274 7928 7265  heck_property(re
-0001b430: 7374 2c20 7265 7175 6972 655f 696e 6465  st, require_inde
-0001b440: 7865 643d 7265 7175 6972 655f 696e 6465  xed=require_inde
-0001b450: 7865 6429 0a0a 2020 4063 6c61 7373 6d65  xed)..  @classme
-0001b460: 7468 6f64 0a20 2064 6566 205f 756e 6b6e  thod.  def _unkn
-0001b470: 6f77 6e5f 7072 6f70 6572 7479 2863 6c73  own_property(cls
-0001b480: 2c20 6e61 6d65 293a 0a20 2020 2022 2222  , name):.    """
-0001b490: 496e 7465 726e 616c 2068 656c 7065 7220  Internal helper 
-0001b4a0: 746f 2072 6169 7365 2061 6e20 6578 6365  to raise an exce
-0001b4b0: 7074 696f 6e20 666f 7220 616e 2075 6e6b  ption for an unk
-0001b4c0: 6e6f 776e 2070 726f 7065 7274 7920 6e61  nown property na
-0001b4d0: 6d65 2e0a 0a20 2020 2054 6869 7320 6973  me...    This is
-0001b4e0: 2063 616c 6c65 6420 6279 205f 6368 6563   called by _chec
-0001b4f0: 6b5f 7072 6f70 6572 7469 6573 2829 2e20  k_properties(). 
-0001b500: 2049 7420 6973 206f 7665 7272 6964 6465   It is overridde
-0001b510: 6e20 6279 0a20 2020 2045 7870 616e 646f  n by.    Expando
-0001b520: 2c20 7768 6572 6520 7468 6973 2069 7320  , where this is 
-0001b530: 6120 6e6f 2d6f 702e 0a0a 2020 2020 5261  a no-op...    Ra
-0001b540: 6973 6573 3a0a 2020 2020 2020 496e 7661  ises:.      Inva
-0001b550: 6c69 6450 726f 7065 7274 7945 7272 6f72  lidPropertyError
-0001b560: 2e0a 2020 2020 2222 220a 2020 2020 7261  ..    """.    ra
-0001b570: 6973 6520 496e 7661 6c69 6450 726f 7065  ise InvalidPrope
-0001b580: 7274 7945 7272 6f72 2827 556e 6b6e 6f77  rtyError('Unknow
-0001b590: 6e20 7072 6f70 6572 7479 2025 7327 2025  n property %s' %
-0001b5a0: 206e 616d 6529 0a0a 2020 6465 6620 5f76   name)..  def _v
-0001b5b0: 616c 6964 6174 655f 6b65 7928 7365 6c66  alidate_key(self
-0001b5c0: 2c20 6b65 7929 3a0a 2020 2020 2222 2256  , key):.    """V
-0001b5d0: 616c 6964 6174 696f 6e20 666f 7220 5f6b  alidation for _k
-0001b5e0: 6579 2061 7474 7269 6275 7465 2028 6465  ey attribute (de
-0001b5f0: 7369 676e 6564 2074 6f20 6265 206f 7665  signed to be ove
-0001b600: 7272 6964 6465 6e29 2e0a 0a20 2020 2041  rridden)...    A
-0001b610: 7267 733a 0a20 2020 2020 206b 6579 3a20  rgs:.      key: 
-0001b620: 5072 6f70 6f73 6564 204b 6579 2074 6f20  Proposed Key to 
-0001b630: 7573 6520 666f 7220 656e 7469 7479 2e0a  use for entity..
-0001b640: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-0001b650: 2020 2020 4120 7661 6c69 6420 6b65 792e      A valid key.
-0001b660: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
-0001b670: 7572 6e20 6b65 790a 0a0a 0a0a 2020 4063  urn key.....  @c
-0001b680: 6c61 7373 6d65 7468 6f64 0a20 2064 6566  lassmethod.  def
-0001b690: 205f 7175 6572 7928 636c 732c 202a 6172   _query(cls, *ar
-0001b6a0: 6773 2c20 2a2a 6b77 6473 293a 0a20 2020  gs, **kwds):.   
-0001b6b0: 2022 2222 4372 6561 7465 2061 2051 7565   """Create a Que
-0001b6c0: 7279 206f 626a 6563 7420 666f 7220 7468  ry object for th
-0001b6d0: 6973 2063 6c61 7373 2e0a 0a20 2020 2041  is class...    A
-0001b6e0: 7267 733a 0a20 2020 2020 2064 6973 7469  rgs:.      disti
-0001b6f0: 6e63 743a 204f 7074 696f 6e61 6c20 626f  nct: Optional bo
-0001b700: 6f6c 2c20 7368 6f72 7420 6861 6e64 2066  ol, short hand f
-0001b710: 6f72 2067 726f 7570 5f62 7920 3d20 7072  or group_by = pr
-0001b720: 6f6a 6563 7469 6f6e 2e0a 2020 2020 2020  ojection..      
-0001b730: 2a61 7267 733a 2055 7365 6420 746f 2061  *args: Used to a
-0001b740: 7070 6c79 2061 6e20 696e 6974 6961 6c20  pply an initial 
-0001b750: 6669 6c74 6572 0a20 2020 2020 202a 2a6b  filter.      **k
-0001b760: 7764 733a 2061 7265 2070 6173 7365 6420  wds: are passed 
-0001b770: 746f 2074 6865 2051 7565 7279 2829 2063  to the Query() c
-0001b780: 6f6e 7374 7275 6374 6f72 2e0a 0a20 2020  onstructor...   
-0001b790: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0001b7a0: 4120 5175 6572 7920 6f62 6a65 6374 2e0a  A Query object..
-0001b7b0: 2020 2020 2222 220a 0a20 2020 2069 6620      """..    if 
-0001b7c0: 2764 6973 7469 6e63 7427 2069 6e20 6b77  'distinct' in kw
-0001b7d0: 6473 3a0a 2020 2020 2020 6966 2027 6772  ds:.      if 'gr
-0001b7e0: 6f75 705f 6279 2720 696e 206b 7764 733a  oup_by' in kwds:
-0001b7f0: 0a20 2020 2020 2020 2072 6169 7365 2054  .        raise T
-0001b800: 7970 6545 7272 6f72 280a 2020 2020 2020  ypeError(.      
-0001b810: 2020 2020 2020 2763 616e 6e6f 7420 7573        'cannot us
-0001b820: 6520 6469 7374 696e 6374 3d20 616e 6420  e distinct= and 
-0001b830: 6772 6f75 705f 6279 3d20 6174 2074 6865  group_by= at the
-0001b840: 2073 616d 6520 7469 6d65 2729 0a20 2020   same time').   
-0001b850: 2020 2070 726f 6a65 6374 696f 6e20 3d20     projection = 
-0001b860: 6b77 6473 2e67 6574 2827 7072 6f6a 6563  kwds.get('projec
-0001b870: 7469 6f6e 2729 0a20 2020 2020 2069 6620  tion').      if 
-0001b880: 6e6f 7420 7072 6f6a 6563 7469 6f6e 3a0a  not projection:.
-0001b890: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
-0001b8a0: 7065 4572 726f 7228 0a20 2020 2020 2020  peError(.       
-0001b8b0: 2020 2020 2027 6361 6e6e 6f74 2075 7365       'cannot use
-0001b8c0: 2064 6973 7469 6e63 743d 2077 6974 686f   distinct= witho
-0001b8d0: 7574 2070 726f 6a65 6374 696f 6e3d 2729  ut projection=')
-0001b8e0: 0a20 2020 2020 2069 6620 6b77 6473 2e70  .      if kwds.p
-0001b8f0: 6f70 2827 6469 7374 696e 6374 2729 3a0a  op('distinct'):.
-0001b900: 2020 2020 2020 2020 6b77 6473 5b27 6772          kwds['gr
-0001b910: 6f75 705f 6279 275d 203d 2070 726f 6a65  oup_by'] = proje
-0001b920: 6374 696f 6e0a 0a0a 2020 2020 6672 6f6d  ction...    from
-0001b930: 2067 6f6f 676c 652e 6170 7065 6e67 696e   google.appengin
-0001b940: 652e 6578 742e 6e64 622e 7175 6572 7920  e.ext.ndb.query 
-0001b950: 696d 706f 7274 2051 7565 7279 0a20 2020  import Query.   
-0001b960: 2071 7279 203d 2051 7565 7279 286b 696e   qry = Query(kin
-0001b970: 643d 636c 732e 5f67 6574 5f6b 696e 6428  d=cls._get_kind(
-0001b980: 292c 202a 2a6b 7764 7329 0a20 2020 2071  ), **kwds).    q
-0001b990: 7279 203d 2071 7279 2e66 696c 7465 7228  ry = qry.filter(
-0001b9a0: 2a63 6c73 2e5f 6465 6661 756c 745f 6669  *cls._default_fi
-0001b9b0: 6c74 6572 7328 2929 0a20 2020 2071 7279  lters()).    qry
-0001b9c0: 203d 2071 7279 2e66 696c 7465 7228 2a61   = qry.filter(*a
-0001b9d0: 7267 7329 0a20 2020 2072 6574 7572 6e20  rgs).    return 
-0001b9e0: 7172 790a 2020 7175 6572 7920 3d20 5f71  qry.  query = _q
-0001b9f0: 7565 7279 0a0a 2020 4063 6c61 7373 6d65  uery..  @classme
-0001ba00: 7468 6f64 0a20 2064 6566 205f 6771 6c28  thod.  def _gql(
-0001ba10: 636c 732c 2071 7565 7279 5f73 7472 696e  cls, query_strin
-0001ba20: 672c 202a 6172 6773 2c20 2a2a 6b77 6473  g, *args, **kwds
-0001ba30: 293a 0a20 2020 2022 2222 5275 6e20 6120  ):.    """Run a 
-0001ba40: 4751 4c20 7175 6572 792e 2222 220a 2020  GQL query.""".  
-0001ba50: 2020 6672 6f6d 2067 6f6f 676c 652e 6170    from google.ap
-0001ba60: 7065 6e67 696e 652e 6578 742e 6e64 622e  pengine.ext.ndb.
-0001ba70: 7175 6572 7920 696d 706f 7274 2067 716c  query import gql
-0001ba80: 0a20 2020 2072 6574 7572 6e20 6771 6c28  .    return gql(
-0001ba90: 2753 454c 4543 5420 2a20 4652 4f4d 2025  'SELECT * FROM %
-0001baa0: 7320 2573 2720 2520 2863 6c73 2e5f 636c  s %s' % (cls._cl
-0001bab0: 6173 735f 6e61 6d65 2829 2c20 7175 6572  ass_name(), quer
-0001bac0: 795f 7374 7269 6e67 292c 0a20 2020 2020  y_string),.     
-0001bad0: 2020 2020 2020 2020 2020 2a61 7267 732c            *args,
-0001bae0: 202a 2a6b 7764 7329 0a20 2067 716c 203d   **kwds).  gql =
-0001baf0: 205f 6771 6c0a 0a20 2064 6566 205f 7075   _gql..  def _pu
-0001bb00: 7428 7365 6c66 2c20 2a2a 6374 785f 6f70  t(self, **ctx_op
-0001bb10: 7469 6f6e 7329 3a0a 2020 2020 2222 2257  tions):.    """W
-0001bb20: 7269 7465 2074 6869 7320 656e 7469 7479  rite this entity
-0001bb30: 2074 6f20 436c 6f75 6420 4461 7461 7374   to Cloud Datast
-0001bb40: 6f72 652e 0a0a 2020 2020 4966 2074 6865  ore...    If the
-0001bb50: 206f 7065 7261 7469 6f6e 2063 7265 6174   operation creat
-0001bb60: 6573 206f 7220 636f 6d70 6c65 7465 7320  es or completes 
-0001bb70: 6120 6b65 792c 2074 6865 2065 6e74 6974  a key, the entit
-0001bb80: 7927 7320 6b65 790a 2020 2020 6174 7472  y's key.    attr
-0001bb90: 6962 7574 6520 6973 2073 6574 2074 6f20  ibute is set to 
-0001bba0: 7468 6520 6e65 772c 2063 6f6d 706c 6574  the new, complet
-0001bbb0: 6520 6b65 792e 0a0a 2020 2020 5265 7475  e key...    Retu
-0001bbc0: 726e 733a 0a20 2020 2020 2054 6865 206b  rns:.      The k
-0001bbd0: 6579 2066 6f72 2074 6865 2065 6e74 6974  ey for the entit
-0001bbe0: 792e 2020 5468 6973 2069 7320 616c 7761  y.  This is alwa
-0001bbf0: 7973 2061 2063 6f6d 706c 6574 6520 6b65  ys a complete ke
-0001bc00: 792e 0a20 2020 2022 2222 0a20 2020 2072  y..    """.    r
-0001bc10: 6574 7572 6e20 7365 6c66 2e5f 7075 745f  eturn self._put_
-0001bc20: 6173 796e 6328 2a2a 6374 785f 6f70 7469  async(**ctx_opti
-0001bc30: 6f6e 7329 2e67 6574 5f72 6573 756c 7428  ons).get_result(
-0001bc40: 290a 2020 7075 7420 3d20 5f70 7574 0a0a  ).  put = _put..
-0001bc50: 2020 6465 6620 5f70 7574 5f61 7379 6e63    def _put_async
-0001bc60: 2873 656c 662c 202a 2a63 7478 5f6f 7074  (self, **ctx_opt
-0001bc70: 696f 6e73 293a 0a20 2020 2022 2222 5772  ions):.    """Wr
-0001bc80: 6974 6520 7468 6973 2065 6e74 6974 7920  ite this entity 
-0001bc90: 746f 2043 6c6f 7564 2044 6174 6173 746f  to Cloud Datasto
-0001bca0: 7265 2e0a 0a20 2020 2054 6869 7320 6973  re...    This is
-0001bcb0: 2074 6865 2061 7379 6e63 6872 6f6e 6f75   the asynchronou
-0001bcc0: 7320 7665 7273 696f 6e20 6f66 204d 6f64  s version of Mod
-0001bcd0: 656c 2e5f 7075 7428 292e 0a20 2020 2022  el._put()..    "
-0001bce0: 2222 0a20 2020 2069 6620 7365 6c66 2e5f  "".    if self._
-0001bcf0: 7072 6f6a 6563 7469 6f6e 3a0a 2020 2020  projection:.    
-0001bd00: 2020 7261 6973 6520 6461 7461 7374 6f72    raise datastor
-0001bd10: 655f 6572 726f 7273 2e42 6164 5265 7175  e_errors.BadRequ
-0001bd20: 6573 7445 7272 6f72 2827 4361 6e6e 6f74  estError('Cannot
-0001bd30: 2070 7574 2061 2070 6172 7469 616c 2065   put a partial e
-0001bd40: 6e74 6974 7927 290a 2020 2020 6672 6f6d  ntity').    from
-0001bd50: 2067 6f6f 676c 652e 6170 7065 6e67 696e   google.appengin
-0001bd60: 652e 6578 742e 6e64 6220 696d 706f 7274  e.ext.ndb import
-0001bd70: 2074 6173 6b6c 6574 730a 2020 2020 6374   tasklets.    ct
-0001bd80: 7820 3d20 7461 736b 6c65 7473 2e67 6574  x = tasklets.get
-0001bd90: 5f63 6f6e 7465 7874 2829 0a20 2020 2073  _context().    s
-0001bda0: 656c 662e 5f70 7265 7061 7265 5f66 6f72  elf._prepare_for
-0001bdb0: 5f70 7574 2829 0a20 2020 2069 6620 7365  _put().    if se
-0001bdc0: 6c66 2e5f 6b65 7920 6973 204e 6f6e 653a  lf._key is None:
-0001bdd0: 0a20 2020 2020 2073 656c 662e 5f6b 6579  .      self._key
-0001bde0: 203d 204b 6579 2873 656c 662e 5f67 6574   = Key(self._get
-0001bdf0: 5f6b 696e 6428 292c 204e 6f6e 6529 0a20  _kind(), None). 
-0001be00: 2020 2073 656c 662e 5f70 7265 5f70 7574     self._pre_put
-0001be10: 5f68 6f6f 6b28 290a 2020 2020 6675 7420  _hook().    fut 
-0001be20: 3d20 6374 782e 7075 7428 7365 6c66 2c20  = ctx.put(self, 
-0001be30: 2a2a 6374 785f 6f70 7469 6f6e 7329 0a20  **ctx_options). 
-0001be40: 2020 2070 6f73 745f 686f 6f6b 203d 2073     post_hook = s
-0001be50: 656c 662e 5f70 6f73 745f 7075 745f 686f  elf._post_put_ho
-0001be60: 6f6b 0a20 2020 2069 6620 6e6f 7420 7365  ok.    if not se
-0001be70: 6c66 2e5f 6973 5f64 6566 6175 6c74 5f68  lf._is_default_h
-0001be80: 6f6f 6b28 4d6f 6465 6c2e 5f64 6566 6175  ook(Model._defau
-0001be90: 6c74 5f70 6f73 745f 7075 745f 686f 6f6b  lt_post_put_hook
-0001bea0: 2c20 706f 7374 5f68 6f6f 6b29 3a0a 2020  , post_hook):.  
-0001beb0: 2020 2020 6675 742e 6164 645f 696d 6d65      fut.add_imme
-0001bec0: 6469 6174 655f 6361 6c6c 6261 636b 2870  diate_callback(p
-0001bed0: 6f73 745f 686f 6f6b 2c20 6675 7429 0a20  ost_hook, fut). 
-0001bee0: 2020 2072 6574 7572 6e20 6675 740a 2020     return fut.  
-0001bef0: 7075 745f 6173 796e 6320 3d20 5f70 7574  put_async = _put
-0001bf00: 5f61 7379 6e63 0a0a 2020 4063 6c61 7373  _async..  @class
-0001bf10: 6d65 7468 6f64 0a20 2064 6566 205f 6765  method.  def _ge
-0001bf20: 745f 6f72 5f69 6e73 6572 7428 2a61 7267  t_or_insert(*arg
-0001bf30: 732c 202a 2a6b 7764 7329 3a0a 2020 2020  s, **kwds):.    
-0001bf40: 2222 2254 7261 6e73 6163 7469 6f6e 616c  """Transactional
-0001bf50: 6c79 2072 6574 7269 6576 6573 2061 6e20  ly retrieves an 
-0001bf60: 6578 6973 7469 6e67 2065 6e74 6974 7920  existing entity 
-0001bf70: 6f72 2063 7265 6174 6573 2061 206e 6577  or creates a new
-0001bf80: 206f 6e65 2e0a 0a20 2020 2050 6f73 6974   one...    Posit
-0001bf90: 696f 6e61 6c20 4172 6773 3a0a 2020 2020  ional Args:.    
-0001bfa0: 2020 6e61 6d65 3a20 4b65 7920 6e61 6d65    name: Key name
-0001bfb0: 2074 6f20 7265 7472 6965 7665 206f 7220   to retrieve or 
-0001bfc0: 6372 6561 7465 2e0a 0a20 2020 204b 6579  create...    Key
-0001bfd0: 776f 7264 2041 7267 733a 0a20 2020 2020  word Args:.     
-0001bfe0: 206e 616d 6573 7061 6365 3a20 4f70 7469   namespace: Opti
-0001bff0: 6f6e 616c 206e 616d 6573 7061 6365 2e0a  onal namespace..
-0001c000: 2020 2020 2020 6170 703a 204f 7074 696f        app: Optio
-0001c010: 6e61 6c20 6170 7020 4944 2e0a 2020 2020  nal app ID..    
-0001c020: 2020 7061 7265 6e74 3a20 5061 7265 6e74    parent: Parent
-0001c030: 2065 6e74 6974 7920 6b65 792c 2069 6620   entity key, if 
-0001c040: 616e 792e 0a20 2020 2020 2063 6f6e 7465  any..      conte
-0001c050: 7874 5f6f 7074 696f 6e73 3a20 436f 6e74  xt_options: Cont
-0001c060: 6578 744f 7074 696f 6e73 206f 626a 6563  extOptions objec
-0001c070: 7420 286e 6f74 206b 6579 776f 7264 2061  t (not keyword a
-0001c080: 7267 7321 2920 6f72 204e 6f6e 652e 0a20  rgs!) or None.. 
-0001c090: 2020 2020 202a 2a6b 7764 733a 204b 6579       **kwds: Key
-0001c0a0: 776f 7264 2061 7267 756d 656e 7473 2074  word arguments t
-0001c0b0: 6f20 7061 7373 2074 6f20 7468 6520 636f  o pass to the co
-0001c0c0: 6e73 7472 7563 746f 7220 6f66 2074 6865  nstructor of the
-0001c0d0: 206d 6f64 656c 2063 6c61 7373 0a20 2020   model class.   
-0001c0e0: 2020 2020 2069 6620 616e 2069 6e73 7461       if an insta
-0001c0f0: 6e63 6520 666f 7220 7468 6520 7370 6563  nce for the spec
-0001c100: 6966 6965 6420 6b65 7920 6e61 6d65 2064  ified key name d
-0001c110: 6f65 7320 6e6f 7420 616c 7265 6164 7920  oes not already 
-0001c120: 6578 6973 742e 2049 660a 2020 2020 2020  exist. If.      
-0001c130: 2020 616e 2069 6e73 7461 6e63 6520 7769    an instance wi
-0001c140: 7468 2074 6865 2073 7570 706c 6965 6420  th the supplied 
-0001c150: 6b65 795f 6e61 6d65 2061 6e64 2070 6172  key_name and par
-0001c160: 656e 7420 616c 7265 6164 7920 6578 6973  ent already exis
-0001c170: 7473 2c0a 2020 2020 2020 2020 7468 6573  ts,.        thes
-0001c180: 6520 6172 6775 6d65 6e74 7320 7769 6c6c  e arguments will
-0001c190: 2062 6520 6469 7363 6172 6465 642e 0a0a   be discarded...
-0001c1a0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0001c1b0: 2020 2045 7869 7374 696e 6720 696e 7374     Existing inst
-0001c1c0: 616e 6365 206f 6620 4d6f 6465 6c20 636c  ance of Model cl
-0001c1d0: 6173 7320 7769 7468 2074 6865 2073 7065  ass with the spe
-0001c1e0: 6369 6669 6564 206b 6579 206e 616d 6520  cified key name 
-0001c1f0: 616e 6420 7061 7265 6e74 0a20 2020 2020  and parent.     
-0001c200: 206f 7220 6120 6e65 7720 6f6e 6520 7468   or a new one th
-0001c210: 6174 2068 6173 206a 7573 7420 6265 656e  at has just been
-0001c220: 2063 7265 6174 6564 2e0a 2020 2020 2222   created..    ""
-0001c230: 220a 2020 2020 636c 732c 2061 7267 7320  ".    cls, args 
-0001c240: 3d20 6172 6773 5b30 5d2c 2061 7267 735b  = args[0], args[
-0001c250: 313a 5d0a 2020 2020 7265 7475 726e 2063  1:].    return c
-0001c260: 6c73 2e5f 6765 745f 6f72 5f69 6e73 6572  ls._get_or_inser
-0001c270: 745f 6173 796e 6328 2a61 7267 732c 202a  t_async(*args, *
-0001c280: 2a6b 7764 7329 2e67 6574 5f72 6573 756c  *kwds).get_resul
-0001c290: 7428 290a 2020 6765 745f 6f72 5f69 6e73  t().  get_or_ins
-0001c2a0: 6572 7420 3d20 5f67 6574 5f6f 725f 696e  ert = _get_or_in
-0001c2b0: 7365 7274 0a0a 2020 4063 6c61 7373 6d65  sert..  @classme
-0001c2c0: 7468 6f64 0a20 2064 6566 205f 6765 745f  thod.  def _get_
-0001c2d0: 6f72 5f69 6e73 6572 745f 6173 796e 6328  or_insert_async(
-0001c2e0: 2a61 7267 732c 202a 2a6b 7764 7329 3a0a  *args, **kwds):.
-0001c2f0: 2020 2020 2222 2254 7261 6e73 6163 7469      """Transacti
-0001c300: 6f6e 616c 6c79 2072 6574 7269 6576 6573  onally retrieves
-0001c310: 2061 6e20 6578 6973 7469 6e67 2065 6e74   an existing ent
-0001c320: 6974 7920 6f72 2063 7265 6174 6573 2061  ity or creates a
-0001c330: 206e 6577 206f 6e65 2e0a 0a20 2020 2054   new one...    T
-0001c340: 6869 7320 6973 2074 6865 2061 7379 6e63  his is the async
-0001c350: 6872 6f6e 6f75 7320 7665 7273 696f 6e20  hronous version 
-0001c360: 6f66 204d 6f64 656c 2e5f 6765 745f 6f72  of Model._get_or
-0001c370: 5f69 6e73 6572 7428 292e 0a20 2020 2022  _insert()..    "
-0001c380: 2222 0a0a 0a20 2020 2066 726f 6d20 676f  ""...    from go
-0001c390: 6f67 6c65 2e61 7070 656e 6769 6e65 2e65  ogle.appengine.e
-0001c3a0: 7874 2e6e 6462 2069 6d70 6f72 7420 7461  xt.ndb import ta
-0001c3b0: 736b 6c65 7473 0a20 2020 2063 6c73 2c20  sklets.    cls, 
-0001c3c0: 6e61 6d65 203d 2061 7267 730a 2020 2020  name = args.    
-0001c3d0: 6765 745f 6172 6720 3d20 636c 732e 5f5f  get_arg = cls.__
-0001c3e0: 6765 745f 6172 670a 2020 2020 6170 7020  get_arg.    app 
-0001c3f0: 3d20 6765 745f 6172 6728 6b77 6473 2c20  = get_arg(kwds, 
-0001c400: 2761 7070 2729 0a20 2020 206e 616d 6573  'app').    names
-0001c410: 7061 6365 203d 2067 6574 5f61 7267 286b  pace = get_arg(k
-0001c420: 7764 732c 2027 6e61 6d65 7370 6163 6527  wds, 'namespace'
-0001c430: 290a 2020 2020 7061 7265 6e74 203d 2067  ).    parent = g
-0001c440: 6574 5f61 7267 286b 7764 732c 2027 7061  et_arg(kwds, 'pa
-0001c450: 7265 6e74 2729 0a20 2020 2063 6f6e 7465  rent').    conte
-0001c460: 7874 5f6f 7074 696f 6e73 203d 2067 6574  xt_options = get
-0001c470: 5f61 7267 286b 7764 732c 2027 636f 6e74  _arg(kwds, 'cont
-0001c480: 6578 745f 6f70 7469 6f6e 7327 290a 0a0a  ext_options')...
-0001c490: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-0001c4a0: 7461 6e63 6528 6e61 6d65 2c20 7369 782e  tance(name, six.
-0001c4b0: 7374 7269 6e67 5f74 7970 6573 293a 0a20  string_types):. 
-0001c4c0: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
-0001c4d0: 7272 6f72 2827 6e61 6d65 206d 7573 7420  rror('name must 
-0001c4e0: 6265 2061 2073 7472 696e 673b 2072 6563  be a string; rec
-0001c4f0: 6569 7665 6420 2572 2720 2520 6e61 6d65  eived %r' % name
-0001c500: 290a 2020 2020 656c 6966 206e 6f74 206e  ).    elif not n
-0001c510: 616d 653a 0a20 2020 2020 2072 6169 7365  ame:.      raise
-0001c520: 2056 616c 7565 4572 726f 7228 276e 616d   ValueError('nam
-0001c530: 6520 6361 6e6e 6f74 2062 6520 616e 2065  e cannot be an e
-0001c540: 6d70 7479 2073 7472 696e 672e 2729 0a20  mpty string.'). 
-0001c550: 2020 206b 6579 203d 204b 6579 2863 6c73     key = Key(cls
-0001c560: 2c20 6e61 6d65 2c20 6170 703d 6170 702c  , name, app=app,
-0001c570: 206e 616d 6573 7061 6365 3d6e 616d 6573   namespace=names
-0001c580: 7061 6365 2c20 7061 7265 6e74 3d70 6172  pace, parent=par
-0001c590: 656e 7429 0a0a 2020 2020 4074 6173 6b6c  ent)..    @taskl
-0001c5a0: 6574 732e 7461 736b 6c65 740a 2020 2020  ets.tasklet.    
-0001c5b0: 6465 6620 696e 7465 726e 616c 5f74 6173  def internal_tas
-0001c5c0: 6b6c 6574 2829 3a0a 2020 2020 2020 4074  klet():.      @t
-0001c5d0: 6173 6b6c 6574 732e 7461 736b 6c65 740a  asklets.tasklet.
-0001c5e0: 2020 2020 2020 6465 6620 7478 6e28 293a        def txn():
-0001c5f0: 0a20 2020 2020 2020 2065 6e74 203d 2079  .        ent = y
-0001c600: 6965 6c64 206b 6579 2e67 6574 5f61 7379  ield key.get_asy
-0001c610: 6e63 286f 7074 696f 6e73 3d63 6f6e 7465  nc(options=conte
-0001c620: 7874 5f6f 7074 696f 6e73 290a 2020 2020  xt_options).    
-0001c630: 2020 2020 6966 2065 6e74 2069 7320 4e6f      if ent is No
-0001c640: 6e65 3a0a 2020 2020 2020 2020 2020 656e  ne:.          en
-0001c650: 7420 3d20 636c 7328 2a2a 6b77 6473 290a  t = cls(**kwds).
-0001c660: 2020 2020 2020 2020 2020 656e 742e 5f6b            ent._k
-0001c670: 6579 203d 206b 6579 0a20 2020 2020 2020  ey = key.       
-0001c680: 2020 2079 6965 6c64 2065 6e74 2e70 7574     yield ent.put
-0001c690: 5f61 7379 6e63 286f 7074 696f 6e73 3d63  _async(options=c
-0001c6a0: 6f6e 7465 7874 5f6f 7074 696f 6e73 290a  ontext_options).
-0001c6b0: 2020 2020 2020 2020 7261 6973 6520 7461          raise ta
-0001c6c0: 736b 6c65 7473 2e52 6574 7572 6e28 656e  sklets.Return(en
-0001c6d0: 7429 0a20 2020 2020 2069 6620 696e 5f74  t).      if in_t
-0001c6e0: 7261 6e73 6163 7469 6f6e 2829 3a0a 0a20  ransaction():.. 
-0001c6f0: 2020 2020 2020 2065 6e74 203d 2079 6965         ent = yie
-0001c700: 6c64 2074 786e 2829 0a20 2020 2020 2065  ld txn().      e
-0001c710: 6c73 653a 0a0a 2020 2020 2020 2020 656e  lse:..        en
-0001c720: 7420 3d20 7969 656c 6420 6b65 792e 6765  t = yield key.ge
-0001c730: 745f 6173 796e 6328 6f70 7469 6f6e 733d  t_async(options=
-0001c740: 636f 6e74 6578 745f 6f70 7469 6f6e 7329  context_options)
-0001c750: 0a20 2020 2020 2020 2069 6620 656e 7420  .        if ent 
-0001c760: 6973 204e 6f6e 653a 0a0a 2020 2020 2020  is None:..      
-0001c770: 2020 2020 656e 7420 3d20 7969 656c 6420      ent = yield 
-0001c780: 7472 616e 7361 6374 696f 6e5f 6173 796e  transaction_asyn
-0001c790: 6328 7478 6e29 0a20 2020 2020 2072 6169  c(txn).      rai
-0001c7a0: 7365 2074 6173 6b6c 6574 732e 5265 7475  se tasklets.Retu
-0001c7b0: 726e 2865 6e74 290a 0a20 2020 2072 6574  rn(ent)..    ret
-0001c7c0: 7572 6e20 696e 7465 726e 616c 5f74 6173  urn internal_tas
-0001c7d0: 6b6c 6574 2829 0a0a 2020 6765 745f 6f72  klet()..  get_or
-0001c7e0: 5f69 6e73 6572 745f 6173 796e 6320 3d20  _insert_async = 
-0001c7f0: 5f67 6574 5f6f 725f 696e 7365 7274 5f61  _get_or_insert_a
-0001c800: 7379 6e63 0a0a 2020 4063 6c61 7373 6d65  sync..  @classme
-0001c810: 7468 6f64 0a20 2064 6566 205f 616c 6c6f  thod.  def _allo
-0001c820: 6361 7465 5f69 6473 2863 6c73 2c20 7369  cate_ids(cls, si
-0001c830: 7a65 3d4e 6f6e 652c 206d 6178 3d4e 6f6e  ze=None, max=Non
-0001c840: 652c 2070 6172 656e 743d 4e6f 6e65 2c20  e, parent=None, 
-0001c850: 2a2a 6374 785f 6f70 7469 6f6e 7329 3a0a  **ctx_options):.
-0001c860: 2020 2020 2222 2241 6c6c 6f63 6174 6573      """Allocates
-0001c870: 2061 2072 616e 6765 206f 6620 6b65 7920   a range of key 
-0001c880: 4944 7320 666f 7220 7468 6973 206d 6f64  IDs for this mod
-0001c890: 656c 2063 6c61 7373 2e0a 0a20 2020 2041  el class...    A
-0001c8a0: 7267 733a 0a20 2020 2020 2073 697a 653a  rgs:.      size:
-0001c8b0: 204e 756d 6265 7220 6f66 2049 4473 2074   Number of IDs t
-0001c8c0: 6f20 616c 6c6f 6361 7465 2e20 4569 7468  o allocate. Eith
-0001c8d0: 6572 2073 697a 6520 6f72 206d 6178 2063  er size or max c
-0001c8e0: 616e 2062 6520 7370 6563 6966 6965 642c  an be specified,
-0001c8f0: 0a20 2020 2020 2020 206e 6f74 2062 6f74  .        not bot
-0001c900: 682e 0a20 2020 2020 206d 6178 3a20 4d61  h..      max: Ma
-0001c910: 7869 6d75 6d20 4944 2074 6f20 616c 6c6f  ximum ID to allo
-0001c920: 6361 7465 2e20 4569 7468 6572 2073 697a  cate. Either siz
-0001c930: 6520 6f72 206d 6178 2063 616e 2062 6520  e or max can be 
-0001c940: 7370 6563 6966 6965 642c 0a20 2020 2020  specified,.     
-0001c950: 2020 206e 6f74 2062 6f74 682e 0a20 2020     not both..   
-0001c960: 2020 2070 6172 656e 743a 2050 6172 656e     parent: Paren
-0001c970: 7420 6b65 7920 666f 7220 7768 6963 6820  t key for which 
-0001c980: 7468 6520 4944 7320 7769 6c6c 2062 6520  the IDs will be 
-0001c990: 616c 6c6f 6361 7465 642e 0a20 2020 2020  allocated..     
-0001c9a0: 202a 2a63 7478 5f6f 7074 696f 6e73 3a20   **ctx_options: 
-0001c9b0: 436f 6e74 6578 7420 6f70 7469 6f6e 732e  Context options.
-0001c9c0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-0001c9d0: 2020 2020 2041 2074 7570 6c65 2077 6974       A tuple wit
-0001c9e0: 6820 2873 7461 7274 2c20 656e 6429 2066  h (start, end) f
-0001c9f0: 6f72 2074 6865 2061 6c6c 6f63 6174 6564  or the allocated
-0001ca00: 2072 616e 6765 2c20 696e 636c 7573 6976   range, inclusiv
-0001ca10: 652e 0a20 2020 2022 2222 0a20 2020 2072  e..    """.    r
-0001ca20: 6574 7572 6e20 636c 732e 5f61 6c6c 6f63  eturn cls._alloc
-0001ca30: 6174 655f 6964 735f 6173 796e 6328 7369  ate_ids_async(si
-0001ca40: 7a65 3d73 697a 652c 206d 6178 3d6d 6178  ze=size, max=max
-0001ca50: 2c20 7061 7265 6e74 3d70 6172 656e 742c  , parent=parent,
-0001ca60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca80: 2020 2020 2a2a 6374 785f 6f70 7469 6f6e      **ctx_option
-0001ca90: 7329 2e67 6574 5f72 6573 756c 7428 290a  s).get_result().
-0001caa0: 2020 616c 6c6f 6361 7465 5f69 6473 203d    allocate_ids =
-0001cab0: 205f 616c 6c6f 6361 7465 5f69 6473 0a0a   _allocate_ids..
-0001cac0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-0001cad0: 2064 6566 205f 616c 6c6f 6361 7465 5f69   def _allocate_i
-0001cae0: 6473 5f61 7379 6e63 2863 6c73 2c20 7369  ds_async(cls, si
-0001caf0: 7a65 3d4e 6f6e 652c 206d 6178 3d4e 6f6e  ze=None, max=Non
-0001cb00: 652c 2070 6172 656e 743d 4e6f 6e65 2c0a  e, parent=None,.
-0001cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cb20: 2020 2020 2020 2020 2020 2a2a 6374 785f            **ctx_
-0001cb30: 6f70 7469 6f6e 7329 3a0a 2020 2020 2222  options):.    ""
-0001cb40: 2241 6c6c 6f63 6174 6573 2061 2072 616e  "Allocates a ran
-0001cb50: 6765 206f 6620 6b65 7920 4944 7320 666f  ge of key IDs fo
-0001cb60: 7220 7468 6973 206d 6f64 656c 2063 6c61  r this model cla
-0001cb70: 7373 2e0a 0a20 2020 2054 6869 7320 6973  ss...    This is
-0001cb80: 2074 6865 2061 7379 6e63 6872 6f6e 6f75   the asynchronou
-0001cb90: 7320 7665 7273 696f 6e20 6f66 204d 6f64  s version of Mod
-0001cba0: 656c 2e5f 616c 6c6f 6361 7465 5f69 6473  el._allocate_ids
-0001cbb0: 2829 2e0a 2020 2020 2222 220a 2020 2020  ()..    """.    
-0001cbc0: 6672 6f6d 2067 6f6f 676c 652e 6170 7065  from google.appe
-0001cbd0: 6e67 696e 652e 6578 742e 6e64 6220 696d  ngine.ext.ndb im
-0001cbe0: 706f 7274 2074 6173 6b6c 6574 730a 2020  port tasklets.  
-0001cbf0: 2020 6374 7820 3d20 7461 736b 6c65 7473    ctx = tasklets
-0001cc00: 2e67 6574 5f63 6f6e 7465 7874 2829 0a20  .get_context(). 
-0001cc10: 2020 2063 6c73 2e5f 7072 655f 616c 6c6f     cls._pre_allo
-0001cc20: 6361 7465 5f69 6473 5f68 6f6f 6b28 7369  cate_ids_hook(si
-0001cc30: 7a65 2c20 6d61 782c 2070 6172 656e 7429  ze, max, parent)
-0001cc40: 0a20 2020 206b 6579 203d 204b 6579 2863  .    key = Key(c
-0001cc50: 6c73 2e5f 6765 745f 6b69 6e64 2829 2c20  ls._get_kind(), 
-0001cc60: 4e6f 6e65 2c20 7061 7265 6e74 3d70 6172  None, parent=par
-0001cc70: 656e 7429 0a20 2020 2066 7574 203d 2063  ent).    fut = c
-0001cc80: 7478 2e61 6c6c 6f63 6174 655f 6964 7328  tx.allocate_ids(
-0001cc90: 6b65 792c 2073 697a 653d 7369 7a65 2c20  key, size=size, 
-0001cca0: 6d61 783d 6d61 782c 202a 2a63 7478 5f6f  max=max, **ctx_o
-0001ccb0: 7074 696f 6e73 290a 2020 2020 706f 7374  ptions).    post
-0001ccc0: 5f68 6f6f 6b20 3d20 636c 732e 5f70 6f73  _hook = cls._pos
-0001ccd0: 745f 616c 6c6f 6361 7465 5f69 6473 5f68  t_allocate_ids_h
-0001cce0: 6f6f 6b0a 2020 2020 6966 206e 6f74 2063  ook.    if not c
-0001ccf0: 6c73 2e5f 6973 5f64 6566 6175 6c74 5f68  ls._is_default_h
-0001cd00: 6f6f 6b28 4d6f 6465 6c2e 5f64 6566 6175  ook(Model._defau
-0001cd10: 6c74 5f70 6f73 745f 616c 6c6f 6361 7465  lt_post_allocate
-0001cd20: 5f69 6473 5f68 6f6f 6b2c 0a20 2020 2020  _ids_hook,.     
-0001cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd40: 2020 2020 2020 2020 2020 2070 6f73 745f             post_
-0001cd50: 686f 6f6b 293a 0a20 2020 2020 2066 7574  hook):.      fut
-0001cd60: 2e61 6464 5f69 6d6d 6564 6961 7465 5f63  .add_immediate_c
-0001cd70: 616c 6c62 6163 6b28 706f 7374 5f68 6f6f  allback(post_hoo
-0001cd80: 6b2c 2073 697a 652c 206d 6178 2c20 7061  k, size, max, pa
-0001cd90: 7265 6e74 2c20 6675 7429 0a20 2020 2072  rent, fut).    r
-0001cda0: 6574 7572 6e20 6675 740a 2020 616c 6c6f  eturn fut.  allo
-0001cdb0: 6361 7465 5f69 6473 5f61 7379 6e63 203d  cate_ids_async =
-0001cdc0: 205f 616c 6c6f 6361 7465 5f69 6473 5f61   _allocate_ids_a
-0001cdd0: 7379 6e63 0a0a 2020 4063 6c61 7373 6d65  sync..  @classme
-0001cde0: 7468 6f64 0a20 2040 7574 696c 732e 706f  thod.  @utils.po
-0001cdf0: 7369 7469 6f6e 616c 2833 290a 2020 6465  sitional(3).  de
-0001ce00: 6620 5f67 6574 5f62 795f 6964 2863 6c73  f _get_by_id(cls
-0001ce10: 2c20 6964 2c20 7061 7265 6e74 3d4e 6f6e  , id, parent=Non
-0001ce20: 652c 202a 2a63 7478 5f6f 7074 696f 6e73  e, **ctx_options
-0001ce30: 293a 0a20 2020 2022 2222 5265 7475 726e  ):.    """Return
-0001ce40: 7320 616e 2069 6e73 7461 6e63 6520 6f66  s an instance of
-0001ce50: 204d 6f64 656c 2063 6c61 7373 2062 7920   Model class by 
-0001ce60: 4944 2e0a 0a20 2020 2054 6869 7320 6973  ID...    This is
-0001ce70: 2072 6561 6c6c 7920 6a75 7374 2061 2073   really just a s
-0001ce80: 686f 7274 6861 6e64 2066 6f72 204b 6579  horthand for Key
-0001ce90: 2863 6c73 2c20 6964 2c20 2e2e 2e29 2e67  (cls, id, ...).g
-0001cea0: 6574 2829 2e0a 0a20 2020 2041 7267 733a  et()...    Args:
-0001ceb0: 0a20 2020 2020 2069 643a 2041 2073 7472  .      id: A str
-0001cec0: 696e 6720 6f72 2069 6e74 6567 6572 206b  ing or integer k
-0001ced0: 6579 2049 442e 0a20 2020 2020 2070 6172  ey ID..      par
-0001cee0: 656e 743a 204f 7074 696f 6e61 6c20 7061  ent: Optional pa
-0001cef0: 7265 6e74 206b 6579 206f 6620 7468 6520  rent key of the 
-0001cf00: 6d6f 6465 6c20 746f 2067 6574 2e0a 2020  model to get..  
-0001cf10: 2020 2020 6e61 6d65 7370 6163 653a 204f      namespace: O
-0001cf20: 7074 696f 6e61 6c20 6e61 6d65 7370 6163  ptional namespac
-0001cf30: 652e 0a20 2020 2020 2061 7070 3a20 4f70  e..      app: Op
-0001cf40: 7469 6f6e 616c 2061 7070 2049 442e 0a20  tional app ID.. 
-0001cf50: 2020 2020 202a 2a63 7478 5f6f 7074 696f       **ctx_optio
-0001cf60: 6e73 3a20 436f 6e74 6578 7420 6f70 7469  ns: Context opti
-0001cf70: 6f6e 732e 0a0a 2020 2020 5265 7475 726e  ons...    Return
-0001cf80: 733a 0a20 2020 2020 2041 206d 6f64 656c  s:.      A model
-0001cf90: 2069 6e73 7461 6e63 6520 6f72 204e 6f6e   instance or Non
-0001cfa0: 6520 6966 206e 6f74 2066 6f75 6e64 2e0a  e if not found..
-0001cfb0: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
-0001cfc0: 726e 2063 6c73 2e5f 6765 745f 6279 5f69  rn cls._get_by_i
-0001cfd0: 645f 6173 796e 6328 6964 2c20 7061 7265  d_async(id, pare
-0001cfe0: 6e74 3d70 6172 656e 742c 202a 2a63 7478  nt=parent, **ctx
-0001cff0: 5f6f 7074 696f 6e73 292e 6765 745f 7265  _options).get_re
-0001d000: 7375 6c74 2829 0a20 2067 6574 5f62 795f  sult().  get_by_
-0001d010: 6964 203d 205f 6765 745f 6279 5f69 640a  id = _get_by_id.
-0001d020: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
-0001d030: 2020 4075 7469 6c73 2e70 6f73 6974 696f    @utils.positio
-0001d040: 6e61 6c28 3329 0a20 2064 6566 205f 6765  nal(3).  def _ge
-0001d050: 745f 6279 5f69 645f 6173 796e 6328 636c  t_by_id_async(cl
-0001d060: 732c 2069 642c 2070 6172 656e 743d 4e6f  s, id, parent=No
-0001d070: 6e65 2c20 6170 703d 4e6f 6e65 2c20 6e61  ne, app=None, na
-0001d080: 6d65 7370 6163 653d 4e6f 6e65 2c0a 2020  mespace=None,.  
-0001d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d0a0: 2020 2020 202a 2a63 7478 5f6f 7074 696f       **ctx_optio
-0001d0b0: 6e73 293a 0a20 2020 2022 2222 5265 7475  ns):.    """Retu
-0001d0c0: 726e 7320 616e 2069 6e73 7461 6e63 6520  rns an instance 
-0001d0d0: 6f66 204d 6f64 656c 2063 6c61 7373 2062  of Model class b
-0001d0e0: 7920 4944 2028 616e 6420 6170 702c 206e  y ID (and app, n
-0001d0f0: 616d 6573 7061 6365 292e 0a0a 2020 2020  amespace)...    
-0001d100: 5468 6973 2069 7320 7468 6520 6173 796e  This is the asyn
-0001d110: 6368 726f 6e6f 7573 2076 6572 7369 6f6e  chronous version
-0001d120: 206f 6620 4d6f 6465 6c2e 5f67 6574 5f62   of Model._get_b
-0001d130: 795f 6964 2829 2e0a 2020 2020 2222 220a  y_id()..    """.
-0001d140: 2020 2020 6b65 7920 3d20 4b65 7928 636c      key = Key(cl
-0001d150: 732e 5f67 6574 5f6b 696e 6428 292c 2069  s._get_kind(), i
-0001d160: 642c 2070 6172 656e 743d 7061 7265 6e74  d, parent=parent
-0001d170: 2c20 6170 703d 6170 702c 206e 616d 6573  , app=app, names
-0001d180: 7061 6365 3d6e 616d 6573 7061 6365 290a  pace=namespace).
-0001d190: 2020 2020 7265 7475 726e 206b 6579 2e67      return key.g
-0001d1a0: 6574 5f61 7379 6e63 282a 2a63 7478 5f6f  et_async(**ctx_o
-0001d1b0: 7074 696f 6e73 290a 2020 6765 745f 6279  ptions).  get_by
-0001d1c0: 5f69 645f 6173 796e 6320 3d20 5f67 6574  _id_async = _get
-0001d1d0: 5f62 795f 6964 5f61 7379 6e63 0a0a 0a0a  _by_id_async....
-0001d1e0: 0a0a 0a0a 0a0a 0a0a 0a0a 0a20 2040 636c  ...........  @cl
-0001d1f0: 6173 736d 6574 686f 640a 2020 6465 6620  assmethod.  def 
-0001d200: 5f70 7265 5f61 6c6c 6f63 6174 655f 6964  _pre_allocate_id
-0001d210: 735f 686f 6f6b 2863 6c73 2c20 7369 7a65  s_hook(cls, size
-0001d220: 2c20 6d61 782c 2070 6172 656e 7429 3a0a  , max, parent):.
-0001d230: 2020 2020 7061 7373 0a20 205f 6465 6661      pass.  _defa
-0001d240: 756c 745f 7072 655f 616c 6c6f 6361 7465  ult_pre_allocate
-0001d250: 5f69 6473 5f68 6f6f 6b20 3d20 5f70 7265  _ids_hook = _pre
-0001d260: 5f61 6c6c 6f63 6174 655f 6964 735f 686f  _allocate_ids_ho
-0001d270: 6f6b 0a0a 2020 4063 6c61 7373 6d65 7468  ok..  @classmeth
-0001d280: 6f64 0a20 2064 6566 205f 706f 7374 5f61  od.  def _post_a
-0001d290: 6c6c 6f63 6174 655f 6964 735f 686f 6f6b  llocate_ids_hook
-0001d2a0: 2863 6c73 2c20 7369 7a65 2c20 6d61 782c  (cls, size, max,
-0001d2b0: 2070 6172 656e 742c 2066 7574 7572 6529   parent, future)
-0001d2c0: 3a0a 2020 2020 7061 7373 0a20 205f 6465  :.    pass.  _de
-0001d2d0: 6661 756c 745f 706f 7374 5f61 6c6c 6f63  fault_post_alloc
-0001d2e0: 6174 655f 6964 735f 686f 6f6b 203d 205f  ate_ids_hook = _
-0001d2f0: 706f 7374 5f61 6c6c 6f63 6174 655f 6964  post_allocate_id
-0001d300: 735f 686f 6f6b 0a0a 2020 4063 6c61 7373  s_hook..  @class
-0001d310: 6d65 7468 6f64 0a20 2064 6566 205f 7072  method.  def _pr
-0001d320: 655f 6465 6c65 7465 5f68 6f6f 6b28 636c  e_delete_hook(cl
-0001d330: 732c 206b 6579 293a 0a20 2020 2070 6173  s, key):.    pas
-0001d340: 730a 2020 5f64 6566 6175 6c74 5f70 7265  s.  _default_pre
-0001d350: 5f64 656c 6574 655f 686f 6f6b 203d 205f  _delete_hook = _
-0001d360: 7072 655f 6465 6c65 7465 5f68 6f6f 6b0a  pre_delete_hook.
-0001d370: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
-0001d380: 2020 6465 6620 5f70 6f73 745f 6465 6c65    def _post_dele
-0001d390: 7465 5f68 6f6f 6b28 636c 732c 206b 6579  te_hook(cls, key
-0001d3a0: 2c20 6675 7475 7265 293a 0a20 2020 2070  , future):.    p
-0001d3b0: 6173 730a 2020 5f64 6566 6175 6c74 5f70  ass.  _default_p
-0001d3c0: 6f73 745f 6465 6c65 7465 5f68 6f6f 6b20  ost_delete_hook 
-0001d3d0: 3d20 5f70 6f73 745f 6465 6c65 7465 5f68  = _post_delete_h
-0001d3e0: 6f6f 6b0a 0a20 2040 636c 6173 736d 6574  ook..  @classmet
-0001d3f0: 686f 640a 2020 6465 6620 5f70 7265 5f67  hod.  def _pre_g
-0001d400: 6574 5f68 6f6f 6b28 636c 732c 206b 6579  et_hook(cls, key
-0001d410: 293a 0a20 2020 2070 6173 730a 2020 5f64  ):.    pass.  _d
-0001d420: 6566 6175 6c74 5f70 7265 5f67 6574 5f68  efault_pre_get_h
-0001d430: 6f6f 6b20 3d20 5f70 7265 5f67 6574 5f68  ook = _pre_get_h
-0001d440: 6f6f 6b0a 0a20 2040 636c 6173 736d 6574  ook..  @classmet
-0001d450: 686f 640a 2020 6465 6620 5f70 6f73 745f  hod.  def _post_
-0001d460: 6765 745f 686f 6f6b 2863 6c73 2c20 6b65  get_hook(cls, ke
-0001d470: 792c 2066 7574 7572 6529 3a0a 2020 2020  y, future):.    
-0001d480: 7061 7373 0a20 205f 6465 6661 756c 745f  pass.  _default_
-0001d490: 706f 7374 5f67 6574 5f68 6f6f 6b20 3d20  post_get_hook = 
-0001d4a0: 5f70 6f73 745f 6765 745f 686f 6f6b 0a0a  _post_get_hook..
-0001d4b0: 2020 6465 6620 5f70 7265 5f70 7574 5f68    def _pre_put_h
-0001d4c0: 6f6f 6b28 7365 6c66 293a 0a20 2020 2070  ook(self):.    p
-0001d4d0: 6173 730a 2020 5f64 6566 6175 6c74 5f70  ass.  _default_p
-0001d4e0: 7265 5f70 7574 5f68 6f6f 6b20 3d20 5f70  re_put_hook = _p
-0001d4f0: 7265 5f70 7574 5f68 6f6f 6b0a 0a20 2064  re_put_hook..  d
-0001d500: 6566 205f 706f 7374 5f70 7574 5f68 6f6f  ef _post_put_hoo
-0001d510: 6b28 7365 6c66 2c20 6675 7475 7265 293a  k(self, future):
-0001d520: 0a20 2020 2070 6173 730a 2020 5f64 6566  .    pass.  _def
-0001d530: 6175 6c74 5f70 6f73 745f 7075 745f 686f  ault_post_put_ho
-0001d540: 6f6b 203d 205f 706f 7374 5f70 7574 5f68  ok = _post_put_h
-0001d550: 6f6f 6b0a 0a20 2040 7374 6174 6963 6d65  ook..  @staticme
-0001d560: 7468 6f64 0a20 2064 6566 205f 6973 5f64  thod.  def _is_d
-0001d570: 6566 6175 6c74 5f68 6f6f 6b28 6465 6661  efault_hook(defa
-0001d580: 756c 745f 686f 6f6b 2c20 686f 6f6b 293a  ult_hook, hook):
-0001d590: 0a20 2020 2022 2222 4368 6563 6b73 2077  .    """Checks w
-0001d5a0: 6865 7468 6572 2061 2073 7065 6369 6669  hether a specifi
-0001d5b0: 6320 686f 6f6b 2069 7320 696e 2069 7473  c hook is in its
-0001d5c0: 2064 6566 6175 6c74 2073 7461 7465 2e0a   default state..
-0001d5d0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-0001d5e0: 2064 6566 6175 6c74 5f68 6f6f 6b3a 2043   default_hook: C
-0001d5f0: 616c 6c61 626c 6520 7370 6563 6966 6965  allable specifie
-0001d600: 6420 6279 206e 6462 2069 6e74 6572 6e61  d by ndb interna
-0001d610: 6c6c 7920 2864 6f20 6e6f 7420 6f76 6572  lly (do not over
-0001d620: 7269 6465 292e 0a20 2020 2020 2068 6f6f  ride)..      hoo
-0001d630: 6b3a 2054 6865 2068 6f6f 6b20 6465 6669  k: The hook defi
-0001d640: 6e65 6420 6279 2061 206d 6f64 656c 2063  ned by a model c
-0001d650: 6c61 7373 2075 7369 6e67 205f 706f 7374  lass using _post
-0001d660: 5f2a 5f68 6f6f 6b2e 0a0a 2020 2020 5261  _*_hook...    Ra
-0001d670: 6973 6573 3a0a 2020 2020 2020 5479 7065  ises:.      Type
-0001d680: 4572 726f 7220 6966 2065 6974 6865 7220  Error if either 
-0001d690: 7468 6520 6465 6661 756c 7420 686f 6f6b  the default hook
-0001d6a0: 206f 7220 7468 6520 7465 7374 6564 2068   or the tested h
-0001d6b0: 6f6f 6b20 6172 6520 6e6f 7420 6361 6c6c  ook are not call
-0001d6c0: 6162 6c65 2e0a 2020 2020 2222 220a 2020  able..    """.  
-0001d6d0: 2020 6966 206e 6f74 2068 6173 6174 7472    if not hasattr
-0001d6e0: 2864 6566 6175 6c74 5f68 6f6f 6b2c 2027  (default_hook, '
-0001d6f0: 5f5f 6361 6c6c 5f5f 2729 3a0a 2020 2020  __call__'):.    
-0001d700: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-0001d710: 7228 2744 6566 6175 6c74 2068 6f6f 6b73  r('Default hooks
-0001d720: 2066 6f72 206e 6462 2e6d 6f64 656c 2e4d   for ndb.model.M
-0001d730: 6f64 656c 206d 7573 7420 6265 2063 616c  odel must be cal
-0001d740: 6c61 626c 6527 290a 2020 2020 6966 206e  lable').    if n
-0001d750: 6f74 2068 6173 6174 7472 2868 6f6f 6b2c  ot hasattr(hook,
-0001d760: 2027 5f5f 6361 6c6c 5f5f 2729 3a0a 2020   '__call__'):.  
-0001d770: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
-0001d780: 726f 7228 2748 6f6f 6b73 206d 7573 7420  ror('Hooks must 
-0001d790: 6265 2063 616c 6c61 626c 6527 290a 0a0a  be callable')...
-0001d7a0: 0a0a 0a20 2020 2069 6620 6861 7361 7474  ...    if hasatt
-0001d7b0: 7228 6465 6661 756c 745f 686f 6f6b 2c20  r(default_hook, 
-0001d7c0: 275f 5f66 756e 635f 5f27 293a 0a20 2020  '__func__'):.   
-0001d7d0: 2020 2064 6566 6175 6c74 5f68 6f6f 6b20     default_hook 
-0001d7e0: 3d20 6465 6661 756c 745f 686f 6f6b 2e5f  = default_hook._
-0001d7f0: 5f66 756e 635f 5f0a 2020 2020 6966 2068  _func__.    if h
-0001d800: 6173 6174 7472 2868 6f6f 6b2c 2027 5f5f  asattr(hook, '__
-0001d810: 6675 6e63 5f5f 2729 3a0a 2020 2020 2020  func__'):.      
-0001d820: 686f 6f6b 203d 2068 6f6f 6b2e 5f5f 6675  hook = hook.__fu
-0001d830: 6e63 5f5f 0a0a 2020 2020 7265 7475 726e  nc__..    return
-0001d840: 2064 6566 6175 6c74 5f68 6f6f 6b20 6973   default_hook is
-0001d850: 2068 6f6f 6b0a 0a0a 636c 6173 7320 4578   hook...class Ex
-0001d860: 7061 6e64 6f28 4d6f 6465 6c29 3a0a 2020  pando(Model):.  
-0001d870: 2222 224d 6f64 656c 2073 7562 636c 6173  """Model subclas
-0001d880: 7320 746f 2073 7570 706f 7274 2064 796e  s to support dyn
-0001d890: 616d 6963 2050 726f 7065 7274 7920 6e61  amic Property na
-0001d8a0: 6d65 7320 616e 6420 7479 7065 732e 0a0a  mes and types...
-0001d8b0: 2020 5365 6520 7468 6520 6d6f 6475 6c65    See the module
-0001d8c0: 2064 6f63 7374 7269 6e67 2066 6f72 2064   docstring for d
-0001d8d0: 6574 6169 6c73 2e0a 2020 2222 220a 0a0a  etails..  """...
-0001d8e0: 0a20 205f 6465 6661 756c 745f 696e 6465  .  _default_inde
-0001d8f0: 7865 6420 3d20 5472 7565 0a0a 0a20 205f  xed = True...  _
-0001d900: 7772 6974 655f 656d 7074 795f 6c69 7374  write_empty_list
-0001d910: 5f66 6f72 5f64 796e 616d 6963 5f70 726f  _for_dynamic_pro
-0001d920: 7065 7274 6965 7320 3d20 4e6f 6e65 0a0a  perties = None..
-0001d930: 2020 6465 6620 5f73 6574 5f61 7474 7269    def _set_attri
-0001d940: 6275 7465 7328 7365 6c66 2c20 6b77 6473  butes(self, kwds
-0001d950: 293a 0a20 2020 2066 6f72 206e 616d 652c  ):.    for name,
-0001d960: 2076 616c 7565 2069 6e20 7369 782e 6974   value in six.it
-0001d970: 6572 6974 656d 7328 6b77 6473 293a 0a20  eritems(kwds):. 
-0001d980: 2020 2020 2073 6574 6174 7472 2873 656c       setattr(sel
-0001d990: 662c 206e 616d 652c 2076 616c 7565 290a  f, name, value).
-0001d9a0: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
-0001d9b0: 2020 6465 6620 5f75 6e6b 6e6f 776e 5f70    def _unknown_p
-0001d9c0: 726f 7065 7274 7928 636c 732c 206e 616d  roperty(cls, nam
-0001d9d0: 6529 3a0a 0a20 2020 2070 6173 730a 0a20  e):..    pass.. 
-0001d9e0: 2064 6566 205f 5f67 6574 6174 7472 5f5f   def __getattr__
-0001d9f0: 2873 656c 662c 206e 616d 6529 3a0a 2020  (self, name):.  
-0001da00: 2020 6966 206e 616d 652e 7374 6172 7473    if name.starts
-0001da10: 7769 7468 2827 5f27 293a 0a20 2020 2020  with('_'):.     
-0001da20: 2072 6574 7572 6e20 7375 7065 7228 4578   return super(Ex
-0001da30: 7061 6e64 6f2c 2073 656c 6629 2e5f 5f67  pando, self).__g
-0001da40: 6574 6174 7472 5f5f 286e 616d 6529 0a20  etattr__(name). 
-0001da50: 2020 2070 726f 7020 3d20 7365 6c66 2e5f     prop = self._
-0001da60: 7072 6f70 6572 7469 6573 2e67 6574 2873  properties.get(s
-0001da70: 6978 2e65 6e73 7572 655f 7465 7874 286e  ix.ensure_text(n
-0001da80: 616d 6529 290a 2020 2020 6966 2070 726f  ame)).    if pro
-0001da90: 7020 6973 204e 6f6e 653a 0a20 2020 2020  p is None:.     
-0001daa0: 2072 6574 7572 6e20 7375 7065 7228 4578   return super(Ex
-0001dab0: 7061 6e64 6f2c 2073 656c 6629 2e5f 5f67  pando, self).__g
-0001dac0: 6574 6174 7472 6962 7574 655f 5f28 6e61  etattribute__(na
-0001dad0: 6d65 290a 2020 2020 7265 7475 726e 2070  me).    return p
-0001dae0: 726f 702e 5f67 6574 5f76 616c 7565 2873  rop._get_value(s
-0001daf0: 656c 6629 0a0a 2020 6465 6620 5f5f 7365  elf)..  def __se
-0001db00: 7461 7474 725f 5f28 7365 6c66 2c20 6e61  tattr__(self, na
-0001db10: 6d65 2c20 7661 6c75 6529 3a0a 2020 2020  me, value):.    
-0001db20: 6966 2028 6e61 6d65 2e73 7461 7274 7377  if (name.startsw
-0001db30: 6974 6828 275f 2729 206f 720a 2020 2020  ith('_') or.    
-0001db40: 2020 2020 6973 696e 7374 616e 6365 2867      isinstance(g
-0001db50: 6574 6174 7472 2873 656c 662e 5f5f 636c  etattr(self.__cl
-0001db60: 6173 735f 5f2c 206e 616d 652c 204e 6f6e  ass__, name, Non
-0001db70: 6529 2c20 2850 726f 7065 7274 792c 2070  e), (Property, p
-0001db80: 726f 7065 7274 7929 2929 3a0a 2020 2020  roperty))):.    
-0001db90: 2020 7265 7475 726e 2073 7570 6572 2845    return super(E
-0001dba0: 7870 616e 646f 2c20 7365 6c66 292e 5f5f  xpando, self).__
-0001dbb0: 7365 7461 7474 725f 5f28 6e61 6d65 2c20  setattr__(name, 
-0001dbc0: 7661 6c75 6529 0a0a 2020 2020 7365 6c66  value)..    self
-0001dbd0: 2e5f 636c 6f6e 655f 7072 6f70 6572 7469  ._clone_properti
-0001dbe0: 6573 2829 0a20 2020 2069 6620 6973 696e  es().    if isin
-0001dbf0: 7374 616e 6365 2876 616c 7565 2c20 4d6f  stance(value, Mo
-0001dc00: 6465 6c29 3a0a 2020 2020 2020 7072 6f70  del):.      prop
-0001dc10: 203d 2053 7472 7563 7475 7265 6450 726f   = StructuredPro
-0001dc20: 7065 7274 7928 4d6f 6465 6c2c 206e 616d  perty(Model, nam
-0001dc30: 6529 0a20 2020 2065 6c69 6620 6973 696e  e).    elif isin
-0001dc40: 7374 616e 6365 2876 616c 7565 2c20 6469  stance(value, di
-0001dc50: 6374 293a 0a20 2020 2020 2070 726f 7020  ct):.      prop 
-0001dc60: 3d20 5374 7275 6374 7572 6564 5072 6f70  = StructuredProp
-0001dc70: 6572 7479 2845 7870 616e 646f 2c20 6e61  erty(Expando, na
-0001dc80: 6d65 290a 2020 2020 656c 7365 3a0a 0a20  me).    else:.. 
-0001dc90: 2020 2020 2070 726f 7020 3d20 4765 6e65       prop = Gene
-0001dca0: 7269 6350 726f 7065 7274 7928 0a20 2020  ricProperty(.   
-0001dcb0: 2020 2020 2020 206e 616d 652c 2072 6570         name, rep
-0001dcc0: 6561 7465 643d 6973 696e 7374 616e 6365  eated=isinstance
-0001dcd0: 2876 616c 7565 2c20 6c69 7374 292c 0a20  (value, list),. 
-0001dce0: 2020 2020 2020 2020 2069 6e64 6578 6564           indexed
-0001dcf0: 3d73 656c 662e 5f64 6566 6175 6c74 5f69  =self._default_i
-0001dd00: 6e64 6578 6564 2c0a 2020 2020 2020 2020  ndexed,.        
-0001dd10: 2020 7772 6974 655f 656d 7074 795f 6c69    write_empty_li
-0001dd20: 7374 3d73 656c 662e 5f77 7269 7465 5f65  st=self._write_e
-0001dd30: 6d70 7479 5f6c 6973 745f 666f 725f 6479  mpty_list_for_dy
-0001dd40: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
-0001dd50: 290a 2020 2020 7072 6f70 2e5f 636f 6465  ).    prop._code
-0001dd60: 5f6e 616d 6520 3d20 6e61 6d65 0a20 2020  _name = name.   
-0001dd70: 2073 656c 662e 5f70 726f 7065 7274 6965   self._propertie
-0001dd80: 735b 7369 782e 656e 7375 7265 5f74 6578  s[six.ensure_tex
-0001dd90: 7428 6e61 6d65 295d 203d 2070 726f 700a  t(name)] = prop.
-0001dda0: 2020 2020 7072 6f70 2e5f 7365 745f 7661      prop._set_va
-0001ddb0: 6c75 6528 7365 6c66 2c20 7661 6c75 6529  lue(self, value)
-0001ddc0: 0a0a 2020 6465 6620 5f5f 6465 6c61 7474  ..  def __delatt
-0001ddd0: 725f 5f28 7365 6c66 2c20 6e61 6d65 293a  r__(self, name):
-0001dde0: 0a20 2020 2069 6620 286e 616d 652e 7374  .    if (name.st
-0001ddf0: 6172 7473 7769 7468 2827 5f27 2920 6f72  artswith('_') or
-0001de00: 0a20 2020 2020 2020 2069 7369 6e73 7461  .        isinsta
-0001de10: 6e63 6528 6765 7461 7474 7228 7365 6c66  nce(getattr(self
-0001de20: 2e5f 5f63 6c61 7373 5f5f 2c20 6e61 6d65  .__class__, name
-0001de30: 2c20 4e6f 6e65 292c 2028 5072 6f70 6572  , None), (Proper
-0001de40: 7479 2c20 7072 6f70 6572 7479 2929 293a  ty, property))):
-0001de50: 0a20 2020 2020 2072 6574 7572 6e20 7375  .      return su
-0001de60: 7065 7228 4578 7061 6e64 6f2c 2073 656c  per(Expando, sel
-0001de70: 6629 2e5f 5f64 656c 6174 7472 5f5f 286e  f).__delattr__(n
-0001de80: 616d 6529 0a20 2020 2070 726f 705f 6e61  ame).    prop_na
-0001de90: 6d65 203d 2073 6978 2e65 6e73 7572 655f  me = six.ensure_
-0001dea0: 7465 7874 286e 616d 6529 0a20 2020 2070  text(name).    p
-0001deb0: 726f 7020 3d20 7365 6c66 2e5f 7072 6f70  rop = self._prop
-0001dec0: 6572 7469 6573 2e67 6574 2870 726f 705f  erties.get(prop_
-0001ded0: 6e61 6d65 290a 2020 2020 6966 206e 6f74  name).    if not
-0001dee0: 2069 7369 6e73 7461 6e63 6528 7072 6f70   isinstance(prop
-0001def0: 2c20 5072 6f70 6572 7479 293a 0a20 2020  , Property):.   
-0001df00: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
-0001df10: 6f72 2827 4d6f 6465 6c20 7072 6f70 6572  or('Model proper
-0001df20: 7469 6573 206d 7573 7420 6265 2050 726f  ties must be Pro
-0001df30: 7065 7274 7920 696e 7374 616e 6365 733b  perty instances;
-0001df40: 206e 6f74 2025 7227 2025 0a20 2020 2020   not %r' %.     
-0001df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001df60: 2070 726f 7029 0a20 2020 2070 726f 702e   prop).    prop.
-0001df70: 5f64 656c 6574 655f 7661 6c75 6528 7365  _delete_value(se
-0001df80: 6c66 290a 2020 2020 6966 2070 726f 705f  lf).    if prop_
-0001df90: 6e61 6d65 2069 6e20 7365 6c66 2e5f 5f63  name in self.__c
-0001dfa0: 6c61 7373 5f5f 2e5f 7072 6f70 6572 7469  lass__._properti
-0001dfb0: 6573 3a0a 2020 2020 2020 7261 6973 6520  es:.      raise 
-0001dfc0: 5275 6e74 696d 6545 7272 6f72 2827 5072  RuntimeError('Pr
-0001dfd0: 6f70 6572 7479 2025 7320 7374 696c 6c20  operty %s still 
-0001dfe0: 696e 2074 6865 206c 6973 7420 6f66 2070  in the list of p
-0001dff0: 726f 7065 7274 6965 7320 666f 7220 7468  roperties for th
-0001e000: 6520 270a 2020 2020 2020 2020 2020 2020  e '.            
-0001e010: 2020 2020 2020 2020 2020 2020 2027 6261               'ba
-0001e020: 7365 2063 6c61 7373 2e27 2025 206e 616d  se class.' % nam
-0001e030: 6529 0a20 2020 2064 656c 2073 656c 662e  e).    del self.
-0001e040: 5f70 726f 7065 7274 6965 735b 7072 6f70  _properties[prop
-0001e050: 5f6e 616d 655d 0a0a 0a40 7574 696c 732e  _name]...@utils.
-0001e060: 706f 7369 7469 6f6e 616c 2831 290a 6465  positional(1).de
-0001e070: 6620 7472 616e 7361 6374 696f 6e28 6361  f transaction(ca
-0001e080: 6c6c 6261 636b 2c20 2a2a 6374 785f 6f70  llback, **ctx_op
-0001e090: 7469 6f6e 7329 3a0a 2020 2222 2252 756e  tions):.  """Run
-0001e0a0: 2061 2063 616c 6c62 6163 6b20 696e 2061   a callback in a
-0001e0b0: 2074 7261 6e73 6163 7469 6f6e 2e0a 0a20   transaction... 
-0001e0c0: 2041 7267 733a 0a20 2020 2063 616c 6c62   Args:.    callb
-0001e0d0: 6163 6b3a 2041 2066 756e 6374 696f 6e20  ack: A function 
-0001e0e0: 6f72 2074 6173 6b6c 6574 2074 6f20 6265  or tasklet to be
-0001e0f0: 2063 616c 6c65 642e 0a20 2020 202a 2a63   called..    **c
-0001e100: 7478 5f6f 7074 696f 6e73 3a20 5472 616e  tx_options: Tran
-0001e110: 7361 6374 696f 6e20 6f70 7469 6f6e 732e  saction options.
-0001e120: 0a0a 2020 5573 6566 756c 206f 7074 696f  ..  Useful optio
-0001e130: 6e73 2069 6e63 6c75 6465 3a0a 2020 2020  ns include:.    
-0001e140: 7265 7472 6965 733d 4e3a 2052 6574 7279  retries=N: Retry
-0001e150: 2075 7020 746f 204e 2074 696d 6573 2028   up to N times (
-0001e160: 692e 652e 2074 7279 2075 7020 746f 204e  i.e. try up to N
-0001e170: 2b31 2074 696d 6573 290a 2020 2020 7072  +1 times).    pr
-0001e180: 6f70 6167 6174 696f 6e3d 3c66 6c61 673e  opagation=<flag>
-0001e190: 3a20 4465 7465 726d 696e 6573 2068 6f77  : Determines how
-0001e1a0: 2061 6e20 6578 6973 7469 6e67 2074 7261   an existing tra
-0001e1b0: 6e73 6163 7469 6f6e 2073 686f 756c 6420  nsaction should 
-0001e1c0: 6265 0a20 2020 2020 2070 726f 7061 6761  be.      propaga
-0001e1d0: 7465 642c 2077 6865 7265 203c 666c 6167  ted, where <flag
-0001e1e0: 3e20 6361 6e20 6265 206f 6e65 206f 6620  > can be one of 
-0001e1f0: 7468 6520 666f 6c6c 6f77 696e 673a 0a20  the following:. 
-0001e200: 2020 2020 2054 7261 6e73 6163 7469 6f6e       Transaction
-0001e210: 4f70 7469 6f6e 732e 4e45 5354 4544 3a20  Options.NESTED: 
-0001e220: 5374 6172 7420 6120 6e65 7374 6564 2074  Start a nested t
-0001e230: 7261 6e73 6163 7469 6f6e 2028 7468 6973  ransaction (this
-0001e240: 2069 7320 7468 650a 2020 2020 2020 2020   is the.        
-0001e250: 6465 6661 756c 743b 2062 7574 2061 6374  default; but act
-0001e260: 7561 6c20 6e65 7374 6564 2074 7261 6e73  ual nested trans
-0001e270: 6163 7469 6f6e 7320 6172 6520 6e6f 7420  actions are not 
-0001e280: 7965 7420 696d 706c 656d 656e 7465 642c  yet implemented,
-0001e290: 0a20 2020 2020 2020 2073 6f20 6566 6665  .        so effe
-0001e2a0: 6374 6976 656c 7920 796f 7520 6361 6e20  ctively you can 
-0001e2b0: 6f6e 6c79 2075 7365 2074 6869 7320 6f75  only use this ou
-0001e2c0: 7473 6964 6520 616e 2065 7869 7374 696e  tside an existin
-0001e2d0: 6720 7472 616e 7361 6374 696f 6e29 2e0a  g transaction)..
-0001e2e0: 2020 2020 2020 5472 616e 7361 6374 696f        Transactio
-0001e2f0: 6e4f 7074 696f 6e73 2e4d 414e 4441 544f  nOptions.MANDATO
-0001e300: 5259 3a20 4120 7472 616e 7361 6374 696f  RY: A transactio
-0001e310: 6e20 6d75 7374 2061 6c72 6561 6479 2062  n must already b
-0001e320: 6520 696e 2070 726f 6772 6573 732e 0a20  e in progress.. 
-0001e330: 2020 2020 2054 7261 6e73 6163 7469 6f6e       Transaction
-0001e340: 4f70 7469 6f6e 732e 414c 4c4f 5745 443a  Options.ALLOWED:
-0001e350: 2049 6620 6120 7472 616e 7361 6374 696f   If a transactio
-0001e360: 6e20 6973 2069 6e20 7072 6f67 7265 7373  n is in progress
-0001e370: 2c20 6a6f 696e 2069 742e 0a20 2020 2020  , join it..     
-0001e380: 2054 7261 6e73 6163 7469 6f6e 4f70 7469   TransactionOpti
-0001e390: 6f6e 732e 494e 4445 5045 4e44 454e 543a  ons.INDEPENDENT:
-0001e3a0: 2041 6c77 6179 7320 7374 6172 7420 6120   Always start a 
-0001e3b0: 6e65 7720 7061 7261 6c6c 656c 2074 7261  new parallel tra
-0001e3c0: 6e73 6163 7469 6f6e 2e0a 2020 2020 7867  nsaction..    xg
-0001e3d0: 3d54 7275 653a 204f 6e20 7468 6520 4869  =True: On the Hi
-0001e3e0: 6768 2052 6570 6c69 6361 7469 6f6e 2044  gh Replication D
-0001e3f0: 6174 6173 746f 7265 2c20 656e 6162 6c65  atastore, enable
-0001e400: 2063 726f 7373 2d67 726f 7570 0a20 2020   cross-group.   
-0001e410: 2020 2074 7261 6e73 6163 7469 6f6e 732c     transactions,
-0001e420: 2069 2e65 2e20 616c 6c6f 7720 7772 6974   i.e. allow writ
-0001e430: 696e 6720 746f 2075 7020 746f 2035 2065  ing to up to 5 e
-0001e440: 6e74 6974 7920 6772 6f75 7073 2e0a 2020  ntity groups..  
-0001e450: 2020 7265 6164 5f6f 6e6c 793d 5472 7565    read_only=True
-0001e460: 3a20 496e 6469 6361 7465 7320 6120 7472  : Indicates a tr
-0001e470: 616e 7361 6374 696f 6e20 7769 6c6c 206e  ansaction will n
-0001e480: 6f74 2064 6f20 616e 7920 7772 6974 6573  ot do any writes
-0001e490: 2c20 7768 6963 680a 2020 2020 2020 706f  , which.      po
-0001e4a0: 7465 6e74 6961 6c6c 7920 616c 6c6f 7773  tentially allows
-0001e4b0: 2066 6f72 206d 6f72 6520 7468 726f 7567   for more throug
-0001e4c0: 6870 7574 2e0a 0a20 2057 4152 4e49 4e47  hput...  WARNING
-0001e4d0: 3a20 5573 696e 6720 616e 7974 6869 6e67  : Using anything
-0001e4e0: 206f 7468 6572 2074 6861 6e20 4e45 5354   other than NEST
-0001e4f0: 4544 2066 6f72 2074 6865 2070 726f 7061  ED for the propa
-0001e500: 6761 7469 6f6e 2066 6c61 670a 2020 6361  gation flag.  ca
-0001e510: 6e20 6861 7665 2073 7472 616e 6765 2063  n have strange c
-0001e520: 6f6e 7365 7175 656e 6365 732e 2020 5768  onsequences.  Wh
-0001e530: 656e 2075 7369 6e67 2041 4c4c 4f57 4544  en using ALLOWED
-0001e540: 206f 7220 4d41 4e44 4154 4f52 592c 2069   or MANDATORY, i
-0001e550: 660a 2020 616e 2065 7863 6570 7469 6f6e  f.  an exception
-0001e560: 2069 7320 7261 6973 6564 2c20 7468 6520   is raised, the 
-0001e570: 7472 616e 7361 6374 696f 6e20 6973 206c  transaction is l
-0001e580: 696b 656c 7920 6e6f 7420 7361 6665 2074  ikely not safe t
-0001e590: 6f0a 2020 636f 6d6d 6974 2e20 2057 6865  o.  commit.  Whe
-0001e5a0: 6e20 7573 696e 6720 494e 4445 5045 4e44  n using INDEPEND
-0001e5b0: 454e 5420 6974 2069 7320 6e6f 7420 6765  ENT it is not ge
-0001e5c0: 6e65 7261 6c6c 7920 7361 6665 2074 6f20  nerally safe to 
-0001e5d0: 7265 7475 726e 0a20 2076 616c 7565 7320  return.  values 
-0001e5e0: 7265 6164 2074 6f20 7468 6520 6361 6c6c  read to the call
-0001e5f0: 6572 2028 6173 2074 6865 7920 7765 7265  er (as they were
-0001e600: 206e 6f74 2072 6561 6420 696e 2074 6865   not read in the
-0001e610: 2063 616c 6c65 7227 730a 2020 7472 616e   caller's.  tran
-0001e620: 7361 6374 696f 6e29 2e0a 0a20 2052 6574  saction)...  Ret
-0001e630: 7572 6e73 3a0a 2020 2020 5768 6174 6576  urns:.    Whatev
-0001e640: 6572 2063 616c 6c62 6163 6b28 2920 7265  er callback() re
-0001e650: 7475 726e 732e 0a0a 2020 5261 6973 6573  turns...  Raises
-0001e660: 3a0a 2020 2020 5768 6174 6576 6572 2063  :.    Whatever c
-0001e670: 616c 6c62 6163 6b28 2920 7261 6973 6573  allback() raises
-0001e680: 3b20 6461 7461 7374 6f72 655f 6572 726f  ; datastore_erro
-0001e690: 7273 2e54 7261 6e73 6163 7469 6f6e 4661  rs.TransactionFa
-0001e6a0: 696c 6564 4572 726f 720a 2020 2020 6966  iledError.    if
-0001e6b0: 2074 6865 2074 7261 6e73 6163 7469 6f6e   the transaction
-0001e6c0: 2066 6169 6c65 642e 0a0a 2020 4e6f 7465   failed...  Note
-0001e6d0: 3a0a 2020 2020 546f 2070 6173 7320 6172  :.    To pass ar
-0001e6e0: 6775 6d65 6e74 7320 746f 2061 2063 616c  guments to a cal
-0001e6f0: 6c62 6163 6b20 6675 6e63 7469 6f6e 2c20  lback function, 
-0001e700: 7573 6520 6120 6c61 6d62 6461 2c20 652e  use a lambda, e.
-0001e710: 672e 0a20 2020 2020 2064 6566 206d 795f  g..      def my_
-0001e720: 6361 6c6c 6261 636b 286b 6579 2c20 696e  callback(key, in
-0001e730: 6329 3a0a 2020 2020 2020 2020 2e2e 2e0a  c):.        ....
-0001e740: 2020 2020 2020 7472 616e 7361 6374 696f        transactio
-0001e750: 6e28 6c61 6d62 6461 3a20 6d79 5f63 616c  n(lambda: my_cal
-0001e760: 6c62 6163 6b28 4b65 7928 2e2e 2e29 2c20  lback(Key(...), 
-0001e770: 3129 290a 2020 2222 220a 2020 6675 7420  1)).  """.  fut 
-0001e780: 3d20 7472 616e 7361 6374 696f 6e5f 6173  = transaction_as
-0001e790: 796e 6328 6361 6c6c 6261 636b 2c20 2a2a  ync(callback, **
-0001e7a0: 6374 785f 6f70 7469 6f6e 7329 0a20 2072  ctx_options).  r
-0001e7b0: 6574 7572 6e20 6675 742e 6765 745f 7265  eturn fut.get_re
-0001e7c0: 7375 6c74 2829 0a0a 0a40 7574 696c 732e  sult()...@utils.
-0001e7d0: 706f 7369 7469 6f6e 616c 2831 290a 6465  positional(1).de
-0001e7e0: 6620 7472 616e 7361 6374 696f 6e5f 6173  f transaction_as
-0001e7f0: 796e 6328 6361 6c6c 6261 636b 2c20 2a2a  ync(callback, **
-0001e800: 6374 785f 6f70 7469 6f6e 7329 3a0a 2020  ctx_options):.  
-0001e810: 2222 2252 756e 2061 2063 616c 6c62 6163  """Run a callbac
-0001e820: 6b20 696e 2061 2074 7261 6e73 6163 7469  k in a transacti
-0001e830: 6f6e 2e0a 0a20 2054 6869 7320 6973 2074  on...  This is t
-0001e840: 6865 2061 7379 6e63 6872 6f6e 6f75 7320  he asynchronous 
-0001e850: 7665 7273 696f 6e20 6f66 2074 7261 6e73  version of trans
-0001e860: 6163 7469 6f6e 2829 2e0a 2020 2222 220a  action()..  """.
-0001e870: 2020 6672 6f6d 2067 6f6f 676c 652e 6170    from google.ap
-0001e880: 7065 6e67 696e 652e 6578 742e 6e64 6220  pengine.ext.ndb 
-0001e890: 696d 706f 7274 2074 6173 6b6c 6574 730a  import tasklets.
-0001e8a0: 2020 7265 7475 726e 2074 6173 6b6c 6574    return tasklet
-0001e8b0: 732e 6765 745f 636f 6e74 6578 7428 292e  s.get_context().
-0001e8c0: 7472 616e 7361 6374 696f 6e28 6361 6c6c  transaction(call
-0001e8d0: 6261 636b 2c20 2a2a 6374 785f 6f70 7469  back, **ctx_opti
-0001e8e0: 6f6e 7329 0a0a 0a64 6566 2069 6e5f 7472  ons)...def in_tr
-0001e8f0: 616e 7361 6374 696f 6e28 293a 0a20 2022  ansaction():.  "
-0001e900: 2222 5265 7475 726e 2077 6865 7468 6572  ""Return whether
-0001e910: 2061 2074 7261 6e73 6163 7469 6f6e 2069   a transaction i
-0001e920: 7320 6375 7272 656e 746c 7920 6163 7469  s currently acti
-0001e930: 7665 2e22 2222 0a20 2066 726f 6d20 676f  ve.""".  from go
-0001e940: 6f67 6c65 2e61 7070 656e 6769 6e65 2e65  ogle.appengine.e
-0001e950: 7874 2e6e 6462 2069 6d70 6f72 7420 7461  xt.ndb import ta
-0001e960: 736b 6c65 7473 0a20 2072 6574 7572 6e20  sklets.  return 
-0001e970: 7461 736b 6c65 7473 2e67 6574 5f63 6f6e  tasklets.get_con
-0001e980: 7465 7874 2829 2e69 6e5f 7472 616e 7361  text().in_transa
-0001e990: 6374 696f 6e28 290a 0a0a 4075 7469 6c73  ction()...@utils
-0001e9a0: 2e64 6563 6f72 6174 6f72 0a64 6566 2074  .decorator.def t
-0001e9b0: 7261 6e73 6163 7469 6f6e 616c 2866 756e  ransactional(fun
-0001e9c0: 632c 2061 7267 732c 206b 7764 732c 202a  c, args, kwds, *
-0001e9d0: 2a6f 7074 696f 6e73 293a 0a20 2022 2222  *options):.  """
-0001e9e0: 4465 636f 7261 746f 7220 746f 206d 616b  Decorator to mak
-0001e9f0: 6520 6120 6675 6e63 7469 6f6e 2061 7574  e a function aut
-0001ea00: 6f6d 6174 6963 616c 6c79 2072 756e 2069  omatically run i
-0001ea10: 6e20 6120 7472 616e 7361 6374 696f 6e2e  n a transaction.
-0001ea20: 0a0a 2020 4172 6773 3a0a 2020 2020 2a2a  ..  Args:.    **
-0001ea30: 6374 785f 6f70 7469 6f6e 733a 2054 7261  ctx_options: Tra
-0001ea40: 6e73 6163 7469 6f6e 206f 7074 696f 6e73  nsaction options
-0001ea50: 2028 7365 6520 7472 616e 7361 6374 696f   (see transactio
-0001ea60: 6e28 292c 2062 7574 2070 726f 7061 6761  n(), but propaga
-0001ea70: 7469 6f6e 0a20 2020 2020 2064 6566 6175  tion.      defau
-0001ea80: 6c74 2074 6f20 5472 616e 7361 6374 696f  lt to Transactio
-0001ea90: 6e4f 7074 696f 6e73 2e41 4c4c 4f57 4544  nOptions.ALLOWED
-0001eaa0: 292e 0a0a 2020 5468 6973 2073 7570 706f  )...  This suppo
-0001eab0: 7274 7320 7477 6f20 666f 726d 733a 0a0a  rts two forms:..
-0001eac0: 2020 2831 2920 5661 6e69 6c6c 613a 0a20    (1) Vanilla:. 
-0001ead0: 2020 2020 2040 7472 616e 7361 6374 696f       @transactio
-0001eae0: 6e61 6c0a 2020 2020 2020 6465 6620 6361  nal.      def ca
-0001eaf0: 6c6c 6261 636b 2861 7267 293a 0a20 2020  llback(arg):.   
-0001eb00: 2020 2020 202e 2e2e 0a0a 2020 2832 2920       .....  (2) 
-0001eb10: 5769 7468 206f 7074 696f 6e73 3a0a 2020  With options:.  
-0001eb20: 2020 2020 4074 7261 6e73 6163 7469 6f6e      @transaction
-0001eb30: 616c 2872 6574 7269 6573 3d31 290a 2020  al(retries=1).  
-0001eb40: 2020 2020 6465 6620 6361 6c6c 6261 636b      def callback
-0001eb50: 2861 7267 293a 0a20 2020 2020 2020 202e  (arg):.        .
-0001eb60: 2e2e 0a20 2022 2222 0a20 2072 6574 7572  ...  """.  retur
-0001eb70: 6e20 7472 616e 7361 6374 696f 6e61 6c5f  n transactional_
-0001eb80: 6173 796e 632e 7772 6170 7065 645f 6465  async.wrapped_de
-0001eb90: 636f 7261 746f 7228 0a20 2020 2020 2066  corator(.      f
-0001eba0: 756e 632c 2061 7267 732c 206b 7764 732c  unc, args, kwds,
-0001ebb0: 202a 2a6f 7074 696f 6e73 292e 6765 745f   **options).get_
-0001ebc0: 7265 7375 6c74 2829 0a0a 0a40 7574 696c  result()...@util
-0001ebd0: 732e 6465 636f 7261 746f 720a 6465 6620  s.decorator.def 
-0001ebe0: 7472 616e 7361 6374 696f 6e61 6c5f 6173  transactional_as
-0001ebf0: 796e 6328 6675 6e63 2c20 6172 6773 2c20  ync(func, args, 
-0001ec00: 6b77 6473 2c20 2a2a 6f70 7469 6f6e 7329  kwds, **options)
-0001ec10: 3a0a 2020 2222 2254 6865 2061 7379 6e63  :.  """The async
-0001ec20: 2076 6572 7369 6f6e 206f 6620 406e 6462   version of @ndb
-0001ec30: 2e74 7261 6e73 6163 7469 6f6e 2e22 2222  .transaction."""
-0001ec40: 0a20 206f 7074 696f 6e73 2e73 6574 6465  .  options.setde
-0001ec50: 6661 756c 7428 2770 726f 7061 6761 7469  fault('propagati
-0001ec60: 6f6e 272c 2064 6174 6173 746f 7265 5f72  on', datastore_r
-0001ec70: 7063 2e54 7261 6e73 6163 7469 6f6e 4f70  pc.TransactionOp
-0001ec80: 7469 6f6e 732e 414c 4c4f 5745 4429 0a20  tions.ALLOWED). 
-0001ec90: 2069 6620 6172 6773 206f 7220 6b77 6473   if args or kwds
-0001eca0: 3a0a 2020 2020 7265 7475 726e 2074 7261  :.    return tra
-0001ecb0: 6e73 6163 7469 6f6e 5f61 7379 6e63 286c  nsaction_async(l
-0001ecc0: 616d 6264 613a 2066 756e 6328 2a61 7267  ambda: func(*arg
-0001ecd0: 732c 202a 2a6b 7764 7329 2c20 2a2a 6f70  s, **kwds), **op
-0001ece0: 7469 6f6e 7329 0a20 2072 6574 7572 6e20  tions).  return 
-0001ecf0: 7472 616e 7361 6374 696f 6e5f 6173 796e  transaction_asyn
-0001ed00: 6328 6675 6e63 2c20 2a2a 6f70 7469 6f6e  c(func, **option
-0001ed10: 7329 0a0a 0a40 7574 696c 732e 6465 636f  s)...@utils.deco
-0001ed20: 7261 746f 720a 6465 6620 7472 616e 7361  rator.def transa
-0001ed30: 6374 696f 6e61 6c5f 7461 736b 6c65 7428  ctional_tasklet(
-0001ed40: 6675 6e63 2c20 6172 6773 2c20 6b77 6473  func, args, kwds
-0001ed50: 2c20 2a2a 6f70 7469 6f6e 7329 3a0a 2020  , **options):.  
-0001ed60: 2222 2254 6865 2061 7379 6e63 2076 6572  """The async ver
-0001ed70: 7369 6f6e 206f 6620 406e 6462 2e74 7261  sion of @ndb.tra
-0001ed80: 6e73 6163 7469 6f6e 2e0a 0a20 2057 696c  nsaction...  Wil
-0001ed90: 6c20 7265 7475 726e 2074 6865 2072 6573  l return the res
-0001eda0: 756c 7420 6f66 2074 6865 2077 7261 7070  ult of the wrapp
-0001edb0: 6564 2066 756e 6374 696f 6e20 6173 2061  ed function as a
-0001edc0: 2046 7574 7572 652e 0a20 2022 2222 0a20   Future..  """. 
-0001edd0: 2066 726f 6d20 676f 6f67 6c65 2e61 7070   from google.app
-0001ede0: 656e 6769 6e65 2e65 7874 2e6e 6462 2069  engine.ext.ndb i
-0001edf0: 6d70 6f72 7420 7461 736b 6c65 7473 0a20  mport tasklets. 
-0001ee00: 2066 756e 6320 3d20 7461 736b 6c65 7473   func = tasklets
-0001ee10: 2e74 6173 6b6c 6574 2866 756e 6329 0a20  .tasklet(func). 
-0001ee20: 2072 6574 7572 6e20 7472 616e 7361 6374   return transact
-0001ee30: 696f 6e61 6c5f 6173 796e 632e 7772 6170  ional_async.wrap
-0001ee40: 7065 645f 6465 636f 7261 746f 7228 6675  ped_decorator(fu
-0001ee50: 6e63 2c20 6172 6773 2c20 6b77 6473 2c20  nc, args, kwds, 
-0001ee60: 2a2a 6f70 7469 6f6e 7329 0a0a 0a40 7574  **options)...@ut
-0001ee70: 696c 732e 6465 636f 7261 746f 720a 6465  ils.decorator.de
-0001ee80: 6620 6e6f 6e5f 7472 616e 7361 6374 696f  f non_transactio
-0001ee90: 6e61 6c28 6675 6e63 2c20 6172 6773 2c20  nal(func, args, 
-0001eea0: 6b77 6473 2c20 616c 6c6f 775f 6578 6973  kwds, allow_exis
-0001eeb0: 7469 6e67 3d54 7275 6529 3a0a 2020 2222  ting=True):.  ""
-0001eec0: 2241 2064 6563 6f72 6174 6f72 2074 6861  "A decorator tha
-0001eed0: 7420 656e 7375 7265 7320 6120 6675 6e63  t ensures a func
-0001eee0: 7469 6f6e 2069 7320 7275 6e20 6f75 7473  tion is run outs
-0001eef0: 6964 6520 6120 7472 616e 7361 6374 696f  ide a transactio
-0001ef00: 6e2e 0a0a 2020 4966 2074 6865 7265 2069  n...  If there i
-0001ef10: 7320 616e 2065 7869 7374 696e 6720 7472  s an existing tr
-0001ef20: 616e 7361 6374 696f 6e20 2861 6e64 2061  ansaction (and a
-0001ef30: 6c6c 6f77 5f65 7869 7374 696e 673d 5472  llow_existing=Tr
-0001ef40: 7565 292c 2074 6865 0a20 2065 7869 7374  ue), the.  exist
-0001ef50: 696e 6720 7472 616e 7361 6374 696f 6e20  ing transaction 
-0001ef60: 6973 2070 6175 7365 6420 7768 696c 6520  is paused while 
-0001ef70: 7468 6520 6675 6e63 7469 6f6e 2069 7320  the function is 
-0001ef80: 6578 6563 7574 6564 2e0a 0a20 2041 7267  executed...  Arg
-0001ef90: 733a 0a20 2020 2061 6c6c 6f77 5f65 7869  s:.    allow_exi
-0001efa0: 7374 696e 673a 2049 6620 6661 6c73 652c  sting: If false,
-0001efb0: 2074 6872 6f77 2061 6e20 6578 6365 7074   throw an except
-0001efc0: 696f 6e20 6966 2063 616c 6c65 6420 6672  ion if called fr
-0001efd0: 6f6d 2077 6974 6869 6e0a 2020 2020 2020  om within.      
-0001efe0: 6120 7472 616e 7361 6374 696f 6e2e 2020  a transaction.  
-0001eff0: 4966 2074 7275 652c 2074 656d 706f 7261  If true, tempora
-0001f000: 7269 6c79 2072 652d 6573 7461 626c 6973  rily re-establis
-0001f010: 6820 7468 650a 2020 2020 2020 7072 6576  h the.      prev
-0001f020: 696f 7573 206e 6f6e 2d74 7261 6e73 6163  ious non-transac
-0001f030: 7469 6f6e 616c 2063 6f6e 7465 7874 2e20  tional context. 
-0001f040: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
-0001f050: 652e 0a0a 2020 5468 6973 2073 7570 706f  e...  This suppo
-0001f060: 7274 7320 7477 6f20 666f 726d 732c 2073  rts two forms, s
-0001f070: 696d 696c 6172 2074 6f20 7472 616e 7361  imilar to transa
-0001f080: 6374 696f 6e61 6c28 292e 0a0a 2020 5265  ctional()...  Re
-0001f090: 7475 726e 733a 0a20 2020 2041 2077 7261  turns:.    A wra
-0001f0a0: 7070 6572 2066 6f72 2074 6865 2064 6563  pper for the dec
-0001f0b0: 6f72 6174 6564 2066 756e 6374 696f 6e20  orated function 
-0001f0c0: 7468 6174 2065 6e73 7572 6573 2069 7420  that ensures it 
-0001f0d0: 7275 6e73 206f 7574 7369 6465 2061 0a20  runs outside a. 
-0001f0e0: 2020 2074 7261 6e73 6163 7469 6f6e 2e0a     transaction..
-0001f0f0: 2020 2222 220a 2020 6672 6f6d 2067 6f6f    """.  from goo
-0001f100: 676c 652e 6170 7065 6e67 696e 652e 6578  gle.appengine.ex
-0001f110: 742e 6e64 6220 696d 706f 7274 2074 6173  t.ndb import tas
-0001f120: 6b6c 6574 730a 2020 6374 7820 3d20 7461  klets.  ctx = ta
-0001f130: 736b 6c65 7473 2e67 6574 5f63 6f6e 7465  sklets.get_conte
-0001f140: 7874 2829 0a20 2069 6620 6e6f 7420 6374  xt().  if not ct
-0001f150: 782e 696e 5f74 7261 6e73 6163 7469 6f6e  x.in_transaction
-0001f160: 2829 3a0a 2020 2020 7265 7475 726e 2066  ():.    return f
-0001f170: 756e 6328 2a61 7267 732c 202a 2a6b 7764  unc(*args, **kwd
-0001f180: 7329 0a20 2069 6620 6e6f 7420 616c 6c6f  s).  if not allo
-0001f190: 775f 6578 6973 7469 6e67 3a0a 2020 2020  w_existing:.    
-0001f1a0: 7261 6973 6520 6461 7461 7374 6f72 655f  raise datastore_
-0001f1b0: 6572 726f 7273 2e42 6164 5265 7175 6573  errors.BadReques
-0001f1c0: 7445 7272 6f72 280a 2020 2020 2020 2020  tError(.        
-0001f1d0: 2725 7320 6361 6e6e 6f74 2062 6520 6361  '%s cannot be ca
-0001f1e0: 6c6c 6564 2077 6974 6869 6e20 6120 7472  lled within a tr
-0001f1f0: 616e 7361 6374 696f 6e2e 2720 2520 6675  ansaction.' % fu
-0001f200: 6e63 2e5f 5f6e 616d 655f 5f29 0a20 2073  nc.__name__).  s
-0001f210: 6176 655f 6374 7820 3d20 6374 780a 2020  ave_ctx = ctx.  
-0001f220: 7768 696c 6520 6374 782e 696e 5f74 7261  while ctx.in_tra
-0001f230: 6e73 6163 7469 6f6e 2829 3a0a 2020 2020  nsaction():.    
-0001f240: 6374 7820 3d20 6374 782e 5f70 6172 656e  ctx = ctx._paren
-0001f250: 745f 636f 6e74 6578 740a 2020 2020 6966  t_context.    if
-0001f260: 2063 7478 2069 7320 4e6f 6e65 3a0a 2020   ctx is None:.  
-0001f270: 2020 2020 7261 6973 6520 6461 7461 7374      raise datast
-0001f280: 6f72 655f 6572 726f 7273 2e42 6164 5265  ore_errors.BadRe
-0001f290: 7175 6573 7445 7272 6f72 280a 2020 2020  questError(.    
-0001f2a0: 2020 2020 2020 2743 6f6e 7465 7874 2077        'Context w
-0001f2b0: 6974 686f 7574 206e 6f6e 2d74 7261 6e73  ithout non-trans
-0001f2c0: 6163 7469 6f6e 616c 2061 6e63 6573 746f  actional ancesto
-0001f2d0: 7227 290a 2020 7361 7665 5f64 735f 636f  r').  save_ds_co
-0001f2e0: 6e6e 203d 2064 6174 6173 746f 7265 2e5f  nn = datastore._
-0001f2f0: 4765 7443 6f6e 6e65 6374 696f 6e28 290a  GetConnection().
-0001f300: 2020 7472 793a 0a20 2020 2069 6620 6861    try:.    if ha
-0001f310: 7361 7474 7228 7361 7665 5f63 7478 2c20  sattr(save_ctx, 
-0001f320: 275f 6f6c 645f 6473 5f63 6f6e 6e27 293a  '_old_ds_conn'):
-0001f330: 0a20 2020 2020 2064 6174 6173 746f 7265  .      datastore
-0001f340: 2e5f 5365 7443 6f6e 6e65 6374 696f 6e28  ._SetConnection(
-0001f350: 7361 7665 5f63 7478 2e5f 6f6c 645f 6473  save_ctx._old_ds
-0001f360: 5f63 6f6e 6e29 0a20 2020 2074 6173 6b6c  _conn).    taskl
-0001f370: 6574 732e 7365 745f 636f 6e74 6578 7428  ets.set_context(
-0001f380: 6374 7829 0a20 2020 2072 6574 7572 6e20  ctx).    return 
-0001f390: 6675 6e63 282a 6172 6773 2c20 2a2a 6b77  func(*args, **kw
-0001f3a0: 6473 290a 2020 6669 6e61 6c6c 793a 0a20  ds).  finally:. 
-0001f3b0: 2020 2074 6173 6b6c 6574 732e 7365 745f     tasklets.set_
-0001f3c0: 636f 6e74 6578 7428 7361 7665 5f63 7478  context(save_ctx
-0001f3d0: 290a 2020 2020 6461 7461 7374 6f72 652e  ).    datastore.
-0001f3e0: 5f53 6574 436f 6e6e 6563 7469 6f6e 2873  _SetConnection(s
-0001f3f0: 6176 655f 6473 5f63 6f6e 6e29 0a0a 0a64  ave_ds_conn)...d
-0001f400: 6566 2067 6574 5f6d 756c 7469 5f61 7379  ef get_multi_asy
-0001f410: 6e63 286b 6579 732c 202a 2a63 7478 5f6f  nc(keys, **ctx_o
-0001f420: 7074 696f 6e73 293a 0a20 2022 2222 4665  ptions):.  """Fe
-0001f430: 7463 6865 7320 6120 7365 7175 656e 6365  tches a sequence
-0001f440: 206f 6620 6b65 7973 2e0a 0a20 2041 7267   of keys...  Arg
-0001f450: 733a 0a20 2020 206b 6579 733a 2041 2073  s:.    keys: A s
-0001f460: 6571 7565 6e63 6520 6f66 206b 6579 732e  equence of keys.
-0001f470: 0a20 2020 202a 2a63 7478 5f6f 7074 696f  .    **ctx_optio
-0001f480: 6e73 3a20 436f 6e74 6578 7420 6f70 7469  ns: Context opti
-0001f490: 6f6e 732e 0a0a 2020 5265 7475 726e 733a  ons...  Returns:
-0001f4a0: 0a20 2020 2041 206c 6973 7420 6f66 2066  .    A list of f
-0001f4b0: 7574 7572 6573 2e0a 2020 2222 220a 2020  utures..  """.  
-0001f4c0: 7265 7475 726e 205b 6b65 792e 6765 745f  return [key.get_
-0001f4d0: 6173 796e 6328 2a2a 6374 785f 6f70 7469  async(**ctx_opti
-0001f4e0: 6f6e 7329 2066 6f72 206b 6579 2069 6e20  ons) for key in 
-0001f4f0: 6b65 7973 5d0a 0a0a 6465 6620 6765 745f  keys]...def get_
-0001f500: 6d75 6c74 6928 6b65 7973 2c20 2a2a 6374  multi(keys, **ct
-0001f510: 785f 6f70 7469 6f6e 7329 3a0a 2020 2222  x_options):.  ""
-0001f520: 2246 6574 6368 6573 2061 2073 6571 7565  "Fetches a seque
-0001f530: 6e63 6520 6f66 206b 6579 732e 0a0a 2020  nce of keys...  
-0001f540: 4172 6773 3a0a 2020 2020 6b65 7973 3a20  Args:.    keys: 
-0001f550: 4120 7365 7175 656e 6365 206f 6620 6b65  A sequence of ke
-0001f560: 7973 2e0a 2020 2020 2a2a 6374 785f 6f70  ys..    **ctx_op
-0001f570: 7469 6f6e 733a 2043 6f6e 7465 7874 206f  tions: Context o
-0001f580: 7074 696f 6e73 2e0a 0a20 2052 6574 7572  ptions...  Retur
-0001f590: 6e73 3a0a 2020 2020 4120 6c69 7374 2077  ns:.    A list w
-0001f5a0: 686f 7365 2069 7465 6d73 2061 7265 2065  hose items are e
-0001f5b0: 6974 6865 7220 6120 4d6f 6465 6c20 696e  ither a Model in
-0001f5c0: 7374 616e 6365 206f 7220 4e6f 6e65 2069  stance or None i
-0001f5d0: 6620 7468 6520 6b65 7920 7761 736e 2774  f the key wasn't
-0001f5e0: 0a20 2020 2066 6f75 6e64 2e0a 2020 2222  .    found..  ""
-0001f5f0: 220a 2020 7265 7475 726e 205b 6675 7475  ".  return [futu
-0001f600: 7265 2e67 6574 5f72 6573 756c 7428 290a  re.get_result().
-0001f610: 2020 2020 2020 2020 2020 666f 7220 6675            for fu
-0001f620: 7475 7265 2069 6e20 6765 745f 6d75 6c74  ture in get_mult
-0001f630: 695f 6173 796e 6328 6b65 7973 2c20 2a2a  i_async(keys, **
-0001f640: 6374 785f 6f70 7469 6f6e 7329 5d0a 0a0a  ctx_options)]...
-0001f650: 6465 6620 7075 745f 6d75 6c74 695f 6173  def put_multi_as
-0001f660: 796e 6328 656e 7469 7469 6573 2c20 2a2a  ync(entities, **
-0001f670: 6374 785f 6f70 7469 6f6e 7329 3a0a 2020  ctx_options):.  
-0001f680: 2222 2253 746f 7265 7320 6120 7365 7175  """Stores a sequ
-0001f690: 656e 6365 206f 6620 4d6f 6465 6c20 696e  ence of Model in
-0001f6a0: 7374 616e 6365 732e 0a0a 2020 4172 6773  stances...  Args
-0001f6b0: 3a0a 2020 2020 656e 7469 7469 6573 3a20  :.    entities: 
-0001f6c0: 4120 7365 7175 656e 6365 206f 6620 4d6f  A sequence of Mo
-0001f6d0: 6465 6c20 696e 7374 616e 6365 732e 0a20  del instances.. 
-0001f6e0: 2020 202a 2a63 7478 5f6f 7074 696f 6e73     **ctx_options
-0001f6f0: 3a20 436f 6e74 6578 7420 6f70 7469 6f6e  : Context option
-0001f700: 732e 0a0a 2020 5265 7475 726e 733a 0a20  s...  Returns:. 
-0001f710: 2020 2041 206c 6973 7420 6f66 2066 7574     A list of fut
-0001f720: 7572 6573 2e0a 2020 2222 220a 2020 7265  ures..  """.  re
-0001f730: 7475 726e 205b 656e 7469 7479 2e70 7574  turn [entity.put
-0001f740: 5f61 7379 6e63 282a 2a63 7478 5f6f 7074  _async(**ctx_opt
-0001f750: 696f 6e73 2920 666f 7220 656e 7469 7479  ions) for entity
-0001f760: 2069 6e20 656e 7469 7469 6573 5d0a 0a0a   in entities]...
-0001f770: 6465 6620 7075 745f 6d75 6c74 6928 656e  def put_multi(en
-0001f780: 7469 7469 6573 2c20 2a2a 6374 785f 6f70  tities, **ctx_op
-0001f790: 7469 6f6e 7329 3a0a 2020 2222 2253 746f  tions):.  """Sto
-0001f7a0: 7265 7320 6120 7365 7175 656e 6365 206f  res a sequence o
-0001f7b0: 6620 4d6f 6465 6c20 696e 7374 616e 6365  f Model instance
-0001f7c0: 732e 0a0a 2020 4172 6773 3a0a 2020 2020  s...  Args:.    
-0001f7d0: 656e 7469 7469 6573 3a20 4120 7365 7175  entities: A sequ
-0001f7e0: 656e 6365 206f 6620 4d6f 6465 6c20 696e  ence of Model in
-0001f7f0: 7374 616e 6365 732e 0a20 2020 202a 2a63  stances..    **c
-0001f800: 7478 5f6f 7074 696f 6e73 3a20 436f 6e74  tx_options: Cont
-0001f810: 6578 7420 6f70 7469 6f6e 732e 0a0a 2020  ext options...  
-0001f820: 5265 7475 726e 733a 0a20 2020 2041 206c  Returns:.    A l
-0001f830: 6973 7420 7769 7468 2074 6865 2073 746f  ist with the sto
-0001f840: 7265 6420 6b65 7973 2e0a 2020 2222 220a  red keys..  """.
-0001f850: 2020 7265 7475 726e 205b 6675 7475 7265    return [future
-0001f860: 2e67 6574 5f72 6573 756c 7428 290a 2020  .get_result().  
-0001f870: 2020 2020 2020 2020 666f 7220 6675 7475          for futu
-0001f880: 7265 2069 6e20 7075 745f 6d75 6c74 695f  re in put_multi_
-0001f890: 6173 796e 6328 656e 7469 7469 6573 2c20  async(entities, 
-0001f8a0: 2a2a 6374 785f 6f70 7469 6f6e 7329 5d0a  **ctx_options)].
-0001f8b0: 0a0a 6465 6620 6465 6c65 7465 5f6d 756c  ..def delete_mul
-0001f8c0: 7469 5f61 7379 6e63 286b 6579 732c 202a  ti_async(keys, *
-0001f8d0: 2a63 7478 5f6f 7074 696f 6e73 293a 0a20  *ctx_options):. 
-0001f8e0: 2022 2222 4465 6c65 7465 7320 6120 7365   """Deletes a se
-0001f8f0: 7175 656e 6365 206f 6620 6b65 7973 2e0a  quence of keys..
-0001f900: 0a20 2041 7267 733a 0a20 2020 206b 6579  .  Args:.    key
-0001f910: 733a 2041 2073 6571 7565 6e63 6520 6f66  s: A sequence of
-0001f920: 206b 6579 732e 0a20 2020 202a 2a63 7478   keys..    **ctx
-0001f930: 5f6f 7074 696f 6e73 3a20 436f 6e74 6578  _options: Contex
-0001f940: 7420 6f70 7469 6f6e 732e 0a0a 2020 5265  t options...  Re
-0001f950: 7475 726e 733a 0a20 2020 2041 206c 6973  turns:.    A lis
-0001f960: 7420 6f66 2066 7574 7572 6573 2e0a 2020  t of futures..  
-0001f970: 2222 220a 2020 7265 7475 726e 205b 6b65  """.  return [ke
-0001f980: 792e 6465 6c65 7465 5f61 7379 6e63 282a  y.delete_async(*
-0001f990: 2a63 7478 5f6f 7074 696f 6e73 2920 666f  *ctx_options) fo
-0001f9a0: 7220 6b65 7920 696e 206b 6579 735d 0a0a  r key in keys]..
-0001f9b0: 0a64 6566 2064 656c 6574 655f 6d75 6c74  .def delete_mult
-0001f9c0: 6928 6b65 7973 2c20 2a2a 6374 785f 6f70  i(keys, **ctx_op
-0001f9d0: 7469 6f6e 7329 3a0a 2020 2222 2244 656c  tions):.  """Del
-0001f9e0: 6574 6573 2061 2073 6571 7565 6e63 6520  etes a sequence 
-0001f9f0: 6f66 206b 6579 732e 0a0a 2020 4172 6773  of keys...  Args
-0001fa00: 3a0a 2020 2020 6b65 7973 3a20 4120 7365  :.    keys: A se
-0001fa10: 7175 656e 6365 206f 6620 6b65 7973 2e0a  quence of keys..
-0001fa20: 2020 2020 2a2a 6374 785f 6f70 7469 6f6e      **ctx_option
-0001fa30: 733a 2043 6f6e 7465 7874 206f 7074 696f  s: Context optio
-0001fa40: 6e73 2e0a 0a20 2052 6574 7572 6e73 3a0a  ns...  Returns:.
-0001fa50: 2020 2020 4120 6c69 7374 2077 686f 7365      A list whose
-0001fa60: 2069 7465 6d73 2061 7265 2061 6c6c 204e   items are all N
-0001fa70: 6f6e 652c 206f 6e65 2070 6572 2064 656c  one, one per del
-0001fa80: 6574 6564 206b 6579 2e0a 2020 2222 220a  eted key..  """.
-0001fa90: 2020 7265 7475 726e 205b 6675 7475 7265    return [future
-0001faa0: 2e67 6574 5f72 6573 756c 7428 290a 2020  .get_result().  
-0001fab0: 2020 2020 2020 2020 666f 7220 6675 7475          for futu
-0001fac0: 7265 2069 6e20 6465 6c65 7465 5f6d 756c  re in delete_mul
-0001fad0: 7469 5f61 7379 6e63 286b 6579 732c 202a  ti_async(keys, *
-0001fae0: 2a63 7478 5f6f 7074 696f 6e73 295d 0a0a  *ctx_options)]..
-0001faf0: 0a64 6566 2067 6574 5f69 6e64 6578 6573  .def get_indexes
-0001fb00: 5f61 7379 6e63 282a 2a63 7478 5f6f 7074  _async(**ctx_opt
-0001fb10: 696f 6e73 293a 0a20 2022 2222 4765 7420  ions):.  """Get 
-0001fb20: 6120 6461 7461 2073 7472 7563 7475 7265  a data structure
-0001fb30: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
-0001fb40: 6520 636f 6e66 6967 7572 6564 2069 6e64  e configured ind
-0001fb50: 6578 6573 2e0a 0a20 2041 7267 733a 0a20  exes...  Args:. 
-0001fb60: 2020 202a 2a63 7478 5f6f 7074 696f 6e73     **ctx_options
-0001fb70: 3a20 436f 6e74 6578 7420 6f70 7469 6f6e  : Context option
-0001fb80: 732e 0a0a 2020 5265 7475 726e 733a 0a20  s...  Returns:. 
-0001fb90: 2020 2041 2066 7574 7572 652e 0a20 2022     A future..  "
-0001fba0: 2222 0a20 2066 726f 6d20 676f 6f67 6c65  "".  from google
-0001fbb0: 2e61 7070 656e 6769 6e65 2e65 7874 2e6e  .appengine.ext.n
-0001fbc0: 6462 2069 6d70 6f72 7420 7461 736b 6c65  db import taskle
-0001fbd0: 7473 0a20 2063 7478 203d 2074 6173 6b6c  ts.  ctx = taskl
-0001fbe0: 6574 732e 6765 745f 636f 6e74 6578 7428  ets.get_context(
-0001fbf0: 290a 2020 7265 7475 726e 2063 7478 2e67  ).  return ctx.g
-0001fc00: 6574 5f69 6e64 6578 6573 282a 2a63 7478  et_indexes(**ctx
-0001fc10: 5f6f 7074 696f 6e73 290a 0a0a 6465 6620  _options)...def 
-0001fc20: 6765 745f 696e 6465 7865 7328 2a2a 6374  get_indexes(**ct
-0001fc30: 785f 6f70 7469 6f6e 7329 3a0a 2020 2222  x_options):.  ""
-0001fc40: 2247 6574 2061 2064 6174 6120 7374 7275  "Get a data stru
-0001fc50: 6374 7572 6520 7265 7072 6573 656e 7469  cture representi
-0001fc60: 6e67 2074 6865 2063 6f6e 6669 6775 7265  ng the configure
-0001fc70: 6420 696e 6465 7865 732e 0a0a 2020 4172  d indexes...  Ar
-0001fc80: 6773 3a0a 2020 2020 2a2a 6374 785f 6f70  gs:.    **ctx_op
-0001fc90: 7469 6f6e 733a 2043 6f6e 7465 7874 206f  tions: Context o
-0001fca0: 7074 696f 6e73 2e0a 0a20 2052 6574 7572  ptions...  Retur
-0001fcb0: 6e73 3a0a 2020 2020 4120 6c69 7374 206f  ns:.    A list o
-0001fcc0: 6620 496e 6465 7820 6f62 6a65 6374 732e  f Index objects.
-0001fcd0: 0a20 2022 2222 0a20 2072 6574 7572 6e20  .  """.  return 
-0001fce0: 6765 745f 696e 6465 7865 735f 6173 796e  get_indexes_asyn
-0001fcf0: 6328 2a2a 6374 785f 6f70 7469 6f6e 7329  c(**ctx_options)
-0001fd00: 2e67 6574 5f72 6573 756c 7428 290a 0a0a  .get_result()...
-0001fd10: 0a66 6f72 205f 6e61 6d65 2c20 5f6f 626a  .for _name, _obj
-0001fd20: 6563 7420 696e 206c 6973 7428 676c 6f62  ect in list(glob
-0001fd30: 616c 7328 292e 6974 656d 7328 2929 3a0a  als().items()):.
-0001fd40: 2020 6966 2028 285f 6e61 6d65 2e65 6e64    if ((_name.end
-0001fd50: 7377 6974 6828 2750 726f 7065 7274 7927  swith('Property'
-0001fd60: 2920 616e 6420 6973 7375 6263 6c61 7373  ) and issubclass
-0001fd70: 285f 6f62 6a65 6374 2c20 5072 6f70 6572  (_object, Proper
-0001fd80: 7479 2929 206f 720a 2020 2020 2020 285f  ty)) or.      (_
-0001fd90: 6e61 6d65 2e65 6e64 7377 6974 6828 2745  name.endswith('E
-0001fda0: 7272 6f72 2729 2061 6e64 2069 7373 7562  rror') and issub
-0001fdb0: 636c 6173 7328 5f6f 626a 6563 742c 2045  class(_object, E
-0001fdc0: 7863 6570 7469 6f6e 2929 293a 0a20 2020  xception))):.   
-0001fdd0: 205f 5f61 6c6c 5f5f 2e61 7070 656e 6428   __all__.append(
-0001fde0: 5f6e 616d 6529 0a                        _name).
+0001abd0: 2020 2020 2027 6120 6e6f 6e2d 7374 7269       'a non-stri
+0001abe0: 6e67 2028 2572 2927 2025 2028 636c 732e  ng (%r)' % (cls.
+0001abf0: 5f5f 6e61 6d65 5f5f 2c20 6b69 6e64 2929  __name__, kind))
+0001ac00: 0a20 2020 2069 6620 7369 782e 5059 3220  .    if six.PY2 
+0001ac10: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
+0001ac20: 6365 286b 696e 642c 2073 6978 2e62 696e  ce(kind, six.bin
+0001ac30: 6172 795f 7479 7065 293a 0a20 2020 2020  ary_type):.     
+0001ac40: 2074 7279 3a0a 2020 2020 2020 2020 6b69   try:.        ki
+0001ac50: 6e64 203d 206b 696e 642e 656e 636f 6465  nd = kind.encode
+0001ac60: 2827 6173 6369 6927 290a 2020 2020 2020  ('ascii').      
+0001ac70: 6578 6365 7074 2055 6e69 636f 6465 456e  except UnicodeEn
+0001ac80: 636f 6465 4572 726f 723a 0a20 2020 2020  codeError:.     
+0001ac90: 2020 2072 6169 7365 204b 696e 6445 7272     raise KindErr
+0001aca0: 6f72 2827 436c 6173 7320 2573 2064 6566  or('Class %s def
+0001acb0: 696e 6573 2061 205f 6765 745f 6b69 6e64  ines a _get_kind
+0001acc0: 2829 206d 6574 686f 6420 7468 6174 2072  () method that r
+0001acd0: 6574 7572 6e73 2027 0a20 2020 2020 2020  eturns '.       
+0001ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001acf0: 2027 6120 556e 6963 6f64 6520 7374 7269   'a Unicode stri
+0001ad00: 6e67 2028 2572 293b 2070 6c65 6173 6520  ng (%r); please 
+0001ad10: 656e 636f 6465 2075 7369 6e67 2075 7466  encode using utf
+0001ad20: 2d38 2720 250a 2020 2020 2020 2020 2020  -8' %.          
+0001ad30: 2020 2020 2020 2020 2020 2020 2020 2863                (c
+0001ad40: 6c73 2e5f 5f6e 616d 655f 5f2c 206b 696e  ls.__name__, kin
+0001ad50: 6429 290a 2020 2020 636c 732e 5f70 726f  d)).    cls._pro
+0001ad60: 7065 7274 6965 7320 3d20 7b7d 0a20 2020  perties = {}.   
+0001ad70: 2069 6620 636c 732e 5f5f 6d6f 6475 6c65   if cls.__module
+0001ad80: 5f5f 203d 3d20 5f5f 6e61 6d65 5f5f 3a0a  __ == __name__:.
+0001ad90: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0001ada0: 2066 6f72 206e 616d 6520 696e 2073 6574   for name in set
+0001adb0: 2864 6972 2863 6c73 2929 3a0a 2020 2020  (dir(cls)):.    
+0001adc0: 2020 6174 7472 203d 2067 6574 6174 7472    attr = getattr
+0001add0: 2863 6c73 2c20 6e61 6d65 2c20 4e6f 6e65  (cls, name, None
+0001ade0: 290a 2020 2020 2020 6966 2069 7369 6e73  ).      if isins
+0001adf0: 7461 6e63 6528 6174 7472 2c20 4d6f 6465  tance(attr, Mode
+0001ae00: 6c41 7474 7269 6275 7465 2920 616e 6420  lAttribute) and 
+0001ae10: 6e6f 7420 6973 696e 7374 616e 6365 2861  not isinstance(a
+0001ae20: 7474 722c 204d 6f64 656c 4b65 7929 3a0a  ttr, ModelKey):.
+0001ae30: 2020 2020 2020 2020 6966 206e 616d 652e          if name.
+0001ae40: 7374 6172 7473 7769 7468 2827 5f27 293a  startswith('_'):
+0001ae50: 0a20 2020 2020 2020 2020 2072 6169 7365  .          raise
+0001ae60: 2054 7970 6545 7272 6f72 2827 4d6f 6465   TypeError('Mode
+0001ae70: 6c41 7474 7269 6275 7465 2025 7320 6361  lAttribute %s ca
+0001ae80: 6e6e 6f74 2062 6567 696e 2077 6974 6820  nnot begin with 
+0001ae90: 616e 2075 6e64 6572 7363 6f72 6520 270a  an underscore '.
+0001aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aeb0: 2020 2020 2020 2020 2020 2763 6861 7261            'chara
+0001aec0: 6374 6572 2e20 5f20 7072 6566 6978 6564  cter. _ prefixed
+0001aed0: 2061 7474 7269 6275 7465 7320 6172 6520   attributes are 
+0001aee0: 7265 7365 7276 6564 2066 6f72 2027 0a20  reserved for '. 
+0001aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af00: 2020 2020 2020 2020 2027 7465 6d70 6f72           'tempor
+0001af10: 6172 7920 4d6f 6465 6c20 696e 7374 616e  ary Model instan
+0001af20: 6365 2076 616c 7565 732e 2720 2520 6e61  ce values.' % na
+0001af30: 6d65 290a 2020 2020 2020 2020 6174 7472  me).        attr
+0001af40: 2e5f 6669 785f 7570 2863 6c73 2c20 6e61  ._fix_up(cls, na
+0001af50: 6d65 290a 2020 2020 2020 2020 6966 2069  me).        if i
+0001af60: 7369 6e73 7461 6e63 6528 6174 7472 2c20  sinstance(attr, 
+0001af70: 5072 6f70 6572 7479 293a 0a20 2020 2020  Property):.     
+0001af80: 2020 2020 2069 6620 2861 7474 722e 5f72       if (attr._r
+0001af90: 6570 6561 7465 6420 6f72 0a20 2020 2020  epeated or.     
+0001afa0: 2020 2020 2020 2020 2028 6973 696e 7374           (isinst
+0001afb0: 616e 6365 2861 7474 722c 2053 7472 7563  ance(attr, Struc
+0001afc0: 7475 7265 6450 726f 7065 7274 7929 2061  turedProperty) a
+0001afd0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+0001afe0: 2020 6174 7472 2e5f 6d6f 6465 6c63 6c61    attr._modelcla
+0001aff0: 7373 2e5f 6861 735f 7265 7065 6174 6564  ss._has_repeated
+0001b000: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0001b010: 636c 732e 5f68 6173 5f72 6570 6561 7465  cls._has_repeate
+0001b020: 6420 3d20 5472 7565 0a20 2020 2020 2020  d = True.       
+0001b030: 2020 2063 6c73 2e5f 7072 6f70 6572 7469     cls._properti
+0001b040: 6573 5b73 6978 2e65 6e73 7572 655f 7465  es[six.ensure_te
+0001b050: 7874 2861 7474 722e 5f6e 616d 6529 5d20  xt(attr._name)] 
+0001b060: 3d20 6174 7472 0a20 2020 2063 6c73 2e5f  = attr.    cls._
+0001b070: 7570 6461 7465 5f6b 696e 645f 6d61 7028  update_kind_map(
+0001b080: 290a 0a20 2040 636c 6173 736d 6574 686f  )..  @classmetho
+0001b090: 640a 2020 6465 6620 5f75 7064 6174 655f  d.  def _update_
+0001b0a0: 6b69 6e64 5f6d 6170 2863 6c73 293a 0a20  kind_map(cls):. 
+0001b0b0: 2020 2022 2222 5570 6461 7465 2074 6865     """Update the
+0001b0c0: 206b 696e 6420 6d61 7020 746f 2069 6e63   kind map to inc
+0001b0d0: 6c75 6465 2074 6869 7320 636c 6173 732e  lude this class.
+0001b0e0: 2222 220a 2020 2020 6b20 3d20 636c 732e  """.    k = cls.
+0001b0f0: 5f67 6574 5f6b 696e 6428 290a 2020 2020  _get_kind().    
+0001b100: 636c 732e 5f6b 696e 645f 6d61 705b 6b5d  cls._kind_map[k]
+0001b110: 203d 2063 6c73 0a0a 2020 6465 6620 5f70   = cls..  def _p
+0001b120: 7265 7061 7265 5f66 6f72 5f70 7574 2873  repare_for_put(s
+0001b130: 656c 6629 3a0a 2020 2020 6966 2073 656c  elf):.    if sel
+0001b140: 662e 5f70 726f 7065 7274 6965 733a 0a20  f._properties:. 
+0001b150: 2020 2020 2066 6f72 205f 2c20 7072 6f70       for _, prop
+0001b160: 2069 6e20 736f 7274 6564 2873 6978 2e69   in sorted(six.i
+0001b170: 7465 7269 7465 6d73 2873 656c 662e 5f70  teritems(self._p
+0001b180: 726f 7065 7274 6965 7329 293a 0a20 2020  roperties)):.   
+0001b190: 2020 2020 2070 726f 702e 5f70 7265 7061       prop._prepa
+0001b1a0: 7265 5f66 6f72 5f70 7574 2873 656c 6629  re_for_put(self)
+0001b1b0: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
+0001b1c0: 0a20 2064 6566 205f 6368 6563 6b5f 7072  .  def _check_pr
+0001b1d0: 6f70 6572 7469 6573 2863 6c73 2c20 7072  operties(cls, pr
+0001b1e0: 6f70 6572 7479 5f6e 616d 6573 2c20 7265  operty_names, re
+0001b1f0: 7175 6972 655f 696e 6465 7865 643d 5472  quire_indexed=Tr
+0001b200: 7565 293a 0a20 2020 2022 2222 496e 7465  ue):.    """Inte
+0001b210: 726e 616c 2068 656c 7065 7220 746f 2063  rnal helper to c
+0001b220: 6865 636b 2074 6865 2067 6976 656e 2070  heck the given p
+0001b230: 726f 7065 7274 6965 7320 6578 6973 7420  roperties exist 
+0001b240: 616e 6420 6d65 6574 2073 7065 6369 6669  and meet specifi
+0001b250: 6564 0a20 2020 2072 6571 7569 7265 6d65  ed.    requireme
+0001b260: 6e74 732e 0a0a 2020 2020 4361 6c6c 6564  nts...    Called
+0001b270: 2066 726f 6d20 7175 6572 792e 7079 2e0a   from query.py..
+0001b280: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0001b290: 2070 726f 7065 7274 795f 6e61 6d65 733a   property_names:
+0001b2a0: 204c 6973 7420 6f72 2074 7570 6c65 206f   List or tuple o
+0001b2b0: 6620 7072 6f70 6572 7479 206e 616d 6573  f property names
+0001b2c0: 202d 2d20 6561 6368 2062 6569 6e67 2061   -- each being a
+0001b2d0: 2073 7472 696e 672c 0a20 2020 2020 2020   string,.       
+0001b2e0: 2070 6f73 7369 626c 7920 636f 6e74 6169   possibly contai
+0001b2f0: 6e69 6e67 2064 6f74 7320 2874 6f20 6164  ning dots (to ad
+0001b300: 6472 6573 7320 7375 6270 726f 7065 7274  dress subpropert
+0001b310: 6965 7320 6f66 2073 7472 7563 7475 7265  ies of structure
+0001b320: 640a 2020 2020 2020 2020 7072 6f70 6572  d.        proper
+0001b330: 7469 6573 292e 0a0a 2020 2020 5261 6973  ties)...    Rais
+0001b340: 6573 3a0a 2020 2020 2020 496e 7661 6c69  es:.      Invali
+0001b350: 6450 726f 7065 7274 7945 7272 6f72 2069  dPropertyError i
+0001b360: 6620 6f6e 6520 6f66 2074 6865 2070 726f  f one of the pro
+0001b370: 7065 7274 6965 7320 6973 2069 6e76 616c  perties is inval
+0001b380: 6964 2e0a 2020 2020 2020 4173 7365 7274  id..      Assert
+0001b390: 696f 6e45 7272 6f72 2069 6620 7468 6520  ionError if the 
+0001b3a0: 6172 6775 6d65 6e74 2069 7320 6e6f 7420  argument is not 
+0001b3b0: 6120 6c69 7374 206f 7220 7475 706c 6520  a list or tuple 
+0001b3c0: 6f66 2073 7472 696e 6773 2e0a 2020 2020  of strings..    
+0001b3d0: 2222 220a 2020 2020 6173 7365 7274 2069  """.    assert i
+0001b3e0: 7369 6e73 7461 6e63 6528 7072 6f70 6572  sinstance(proper
+0001b3f0: 7479 5f6e 616d 6573 2c20 286c 6973 742c  ty_names, (list,
+0001b400: 2074 7570 6c65 2929 2c20 7265 7072 2870   tuple)), repr(p
+0001b410: 726f 7065 7274 795f 6e61 6d65 7329 0a20  roperty_names). 
+0001b420: 2020 2066 6f72 206e 616d 6520 696e 2070     for name in p
+0001b430: 726f 7065 7274 795f 6e61 6d65 733a 0a20  roperty_names:. 
+0001b440: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
+0001b450: 7374 616e 6365 286e 616d 652c 2028 7369  stance(name, (si
+0001b460: 782e 7465 7874 5f74 7970 652c 2073 6978  x.text_type, six
+0001b470: 2e62 696e 6172 795f 7479 7065 2929 2c20  .binary_type)), 
+0001b480: 7265 7072 286e 616d 6529 0a20 2020 2020  repr(name).     
+0001b490: 206e 616d 6520 3d20 7369 782e 656e 7375   name = six.ensu
+0001b4a0: 7265 5f74 6578 7428 6e61 6d65 290a 2020  re_text(name).  
+0001b4b0: 2020 2020 6966 2027 2e27 2069 6e20 6e61      if '.' in na
+0001b4c0: 6d65 3a0a 2020 2020 2020 2020 6e61 6d65  me:.        name
+0001b4d0: 2c20 7265 7374 203d 206e 616d 652e 7370  , rest = name.sp
+0001b4e0: 6c69 7428 272e 272c 2031 290a 2020 2020  lit('.', 1).    
+0001b4f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001b500: 7265 7374 203d 204e 6f6e 650a 2020 2020  rest = None.    
+0001b510: 2020 7072 6f70 203d 2063 6c73 2e5f 7072    prop = cls._pr
+0001b520: 6f70 6572 7469 6573 2e67 6574 286e 616d  operties.get(nam
+0001b530: 6529 0a20 2020 2020 2069 6620 7072 6f70  e).      if prop
+0001b540: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0001b550: 2020 636c 732e 5f75 6e6b 6e6f 776e 5f70    cls._unknown_p
+0001b560: 726f 7065 7274 7928 6e61 6d65 290a 2020  roperty(name).  
+0001b570: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001b580: 2020 7072 6f70 2e5f 6368 6563 6b5f 7072    prop._check_pr
+0001b590: 6f70 6572 7479 2872 6573 742c 2072 6571  operty(rest, req
+0001b5a0: 7569 7265 5f69 6e64 6578 6564 3d72 6571  uire_indexed=req
+0001b5b0: 7569 7265 5f69 6e64 6578 6564 290a 0a20  uire_indexed).. 
+0001b5c0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+0001b5d0: 6465 6620 5f75 6e6b 6e6f 776e 5f70 726f  def _unknown_pro
+0001b5e0: 7065 7274 7928 636c 732c 206e 616d 6529  perty(cls, name)
+0001b5f0: 3a0a 2020 2020 2222 2249 6e74 6572 6e61  :.    """Interna
+0001b600: 6c20 6865 6c70 6572 2074 6f20 7261 6973  l helper to rais
+0001b610: 6520 616e 2065 7863 6570 7469 6f6e 2066  e an exception f
+0001b620: 6f72 2061 6e20 756e 6b6e 6f77 6e20 7072  or an unknown pr
+0001b630: 6f70 6572 7479 206e 616d 652e 0a0a 2020  operty name...  
+0001b640: 2020 5468 6973 2069 7320 6361 6c6c 6564    This is called
+0001b650: 2062 7920 5f63 6865 636b 5f70 726f 7065   by _check_prope
+0001b660: 7274 6965 7328 292e 2020 4974 2069 7320  rties().  It is 
+0001b670: 6f76 6572 7269 6464 656e 2062 790a 2020  overridden by.  
+0001b680: 2020 4578 7061 6e64 6f2c 2077 6865 7265    Expando, where
+0001b690: 2074 6869 7320 6973 2061 206e 6f2d 6f70   this is a no-op
+0001b6a0: 2e0a 0a20 2020 2052 6169 7365 733a 0a20  ...    Raises:. 
+0001b6b0: 2020 2020 2049 6e76 616c 6964 5072 6f70       InvalidProp
+0001b6c0: 6572 7479 4572 726f 722e 0a20 2020 2022  ertyError..    "
+0001b6d0: 2222 0a20 2020 2072 6169 7365 2049 6e76  "".    raise Inv
+0001b6e0: 616c 6964 5072 6f70 6572 7479 4572 726f  alidPropertyErro
+0001b6f0: 7228 2755 6e6b 6e6f 776e 2070 726f 7065  r('Unknown prope
+0001b700: 7274 7920 2573 2720 2520 6e61 6d65 290a  rty %s' % name).
+0001b710: 0a20 2064 6566 205f 7661 6c69 6461 7465  .  def _validate
+0001b720: 5f6b 6579 2873 656c 662c 206b 6579 293a  _key(self, key):
+0001b730: 0a20 2020 2022 2222 5661 6c69 6461 7469  .    """Validati
+0001b740: 6f6e 2066 6f72 205f 6b65 7920 6174 7472  on for _key attr
+0001b750: 6962 7574 6520 2864 6573 6967 6e65 6420  ibute (designed 
+0001b760: 746f 2062 6520 6f76 6572 7269 6464 656e  to be overridden
+0001b770: 292e 0a0a 2020 2020 4172 6773 3a0a 2020  )...    Args:.  
+0001b780: 2020 2020 6b65 793a 2050 726f 706f 7365      key: Propose
+0001b790: 6420 4b65 7920 746f 2075 7365 2066 6f72  d Key to use for
+0001b7a0: 2065 6e74 6974 792e 0a0a 2020 2020 5265   entity...    Re
+0001b7b0: 7475 726e 733a 0a20 2020 2020 2041 2076  turns:.      A v
+0001b7c0: 616c 6964 206b 6579 2e0a 2020 2020 2222  alid key..    ""
+0001b7d0: 220a 2020 2020 7265 7475 726e 206b 6579  ".    return key
+0001b7e0: 0a0a 0a0a 0a20 2040 636c 6173 736d 6574  .....  @classmet
+0001b7f0: 686f 640a 2020 6465 6620 5f71 7565 7279  hod.  def _query
+0001b800: 2863 6c73 2c20 2a61 7267 732c 202a 2a6b  (cls, *args, **k
+0001b810: 7764 7329 3a0a 2020 2020 2222 2243 7265  wds):.    """Cre
+0001b820: 6174 6520 6120 5175 6572 7920 6f62 6a65  ate a Query obje
+0001b830: 6374 2066 6f72 2074 6869 7320 636c 6173  ct for this clas
+0001b840: 732e 0a0a 2020 2020 4172 6773 3a0a 2020  s...    Args:.  
+0001b850: 2020 2020 6469 7374 696e 6374 3a20 4f70      distinct: Op
+0001b860: 7469 6f6e 616c 2062 6f6f 6c2c 2073 686f  tional bool, sho
+0001b870: 7274 2068 616e 6420 666f 7220 6772 6f75  rt hand for grou
+0001b880: 705f 6279 203d 2070 726f 6a65 6374 696f  p_by = projectio
+0001b890: 6e2e 0a20 2020 2020 202a 6172 6773 3a20  n..      *args: 
+0001b8a0: 5573 6564 2074 6f20 6170 706c 7920 616e  Used to apply an
+0001b8b0: 2069 6e69 7469 616c 2066 696c 7465 720a   initial filter.
+0001b8c0: 2020 2020 2020 2a2a 6b77 6473 3a20 6172        **kwds: ar
+0001b8d0: 6520 7061 7373 6564 2074 6f20 7468 6520  e passed to the 
+0001b8e0: 5175 6572 7928 2920 636f 6e73 7472 7563  Query() construc
+0001b8f0: 746f 722e 0a0a 2020 2020 5265 7475 726e  tor...    Return
+0001b900: 733a 0a20 2020 2020 2041 2051 7565 7279  s:.      A Query
+0001b910: 206f 626a 6563 742e 0a20 2020 2022 2222   object..    """
+0001b920: 0a0a 2020 2020 6966 2027 6469 7374 696e  ..    if 'distin
+0001b930: 6374 2720 696e 206b 7764 733a 0a20 2020  ct' in kwds:.   
+0001b940: 2020 2069 6620 2767 726f 7570 5f62 7927     if 'group_by'
+0001b950: 2069 6e20 6b77 6473 3a0a 2020 2020 2020   in kwds:.      
+0001b960: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
+0001b970: 7228 0a20 2020 2020 2020 2020 2020 2027  r(.            '
+0001b980: 6361 6e6e 6f74 2075 7365 2064 6973 7469  cannot use disti
+0001b990: 6e63 743d 2061 6e64 2067 726f 7570 5f62  nct= and group_b
+0001b9a0: 793d 2061 7420 7468 6520 7361 6d65 2074  y= at the same t
+0001b9b0: 696d 6527 290a 2020 2020 2020 7072 6f6a  ime').      proj
+0001b9c0: 6563 7469 6f6e 203d 206b 7764 732e 6765  ection = kwds.ge
+0001b9d0: 7428 2770 726f 6a65 6374 696f 6e27 290a  t('projection').
+0001b9e0: 2020 2020 2020 6966 206e 6f74 2070 726f        if not pro
+0001b9f0: 6a65 6374 696f 6e3a 0a20 2020 2020 2020  jection:.       
+0001ba00: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+0001ba10: 280a 2020 2020 2020 2020 2020 2020 2763  (.            'c
+0001ba20: 616e 6e6f 7420 7573 6520 6469 7374 696e  annot use distin
+0001ba30: 6374 3d20 7769 7468 6f75 7420 7072 6f6a  ct= without proj
+0001ba40: 6563 7469 6f6e 3d27 290a 2020 2020 2020  ection=').      
+0001ba50: 6966 206b 7764 732e 706f 7028 2764 6973  if kwds.pop('dis
+0001ba60: 7469 6e63 7427 293a 0a20 2020 2020 2020  tinct'):.       
+0001ba70: 206b 7764 735b 2767 726f 7570 5f62 7927   kwds['group_by'
+0001ba80: 5d20 3d20 7072 6f6a 6563 7469 6f6e 0a0a  ] = projection..
+0001ba90: 0a20 2020 2066 726f 6d20 676f 6f67 6c65  .    from google
+0001baa0: 2e61 7070 656e 6769 6e65 2e65 7874 2e6e  .appengine.ext.n
+0001bab0: 6462 2e71 7565 7279 2069 6d70 6f72 7420  db.query import 
+0001bac0: 5175 6572 790a 2020 2020 7172 7920 3d20  Query.    qry = 
+0001bad0: 5175 6572 7928 6b69 6e64 3d63 6c73 2e5f  Query(kind=cls._
+0001bae0: 6765 745f 6b69 6e64 2829 2c20 2a2a 6b77  get_kind(), **kw
+0001baf0: 6473 290a 2020 2020 7172 7920 3d20 7172  ds).    qry = qr
+0001bb00: 792e 6669 6c74 6572 282a 636c 732e 5f64  y.filter(*cls._d
+0001bb10: 6566 6175 6c74 5f66 696c 7465 7273 2829  efault_filters()
+0001bb20: 290a 2020 2020 7172 7920 3d20 7172 792e  ).    qry = qry.
+0001bb30: 6669 6c74 6572 282a 6172 6773 290a 2020  filter(*args).  
+0001bb40: 2020 7265 7475 726e 2071 7279 0a20 2071    return qry.  q
+0001bb50: 7565 7279 203d 205f 7175 6572 790a 0a20  uery = _query.. 
+0001bb60: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+0001bb70: 6465 6620 5f67 716c 2863 6c73 2c20 7175  def _gql(cls, qu
+0001bb80: 6572 795f 7374 7269 6e67 2c20 2a61 7267  ery_string, *arg
+0001bb90: 732c 202a 2a6b 7764 7329 3a0a 2020 2020  s, **kwds):.    
+0001bba0: 2222 2252 756e 2061 2047 514c 2071 7565  """Run a GQL que
+0001bbb0: 7279 2e22 2222 0a20 2020 2066 726f 6d20  ry.""".    from 
+0001bbc0: 676f 6f67 6c65 2e61 7070 656e 6769 6e65  google.appengine
+0001bbd0: 2e65 7874 2e6e 6462 2e71 7565 7279 2069  .ext.ndb.query i
+0001bbe0: 6d70 6f72 7420 6771 6c0a 2020 2020 7265  mport gql.    re
+0001bbf0: 7475 726e 2067 716c 2827 5345 4c45 4354  turn gql('SELECT
+0001bc00: 202a 2046 524f 4d20 2573 2025 7327 2025   * FROM %s %s' %
+0001bc10: 2028 636c 732e 5f63 6c61 7373 5f6e 616d   (cls._class_nam
+0001bc20: 6528 292c 2071 7565 7279 5f73 7472 696e  e(), query_strin
+0001bc30: 6729 2c0a 2020 2020 2020 2020 2020 2020  g),.            
+0001bc40: 2020 202a 6172 6773 2c20 2a2a 6b77 6473     *args, **kwds
+0001bc50: 290a 2020 6771 6c20 3d20 5f67 716c 0a0a  ).  gql = _gql..
+0001bc60: 2020 6465 6620 5f70 7574 2873 656c 662c    def _put(self,
+0001bc70: 202a 2a63 7478 5f6f 7074 696f 6e73 293a   **ctx_options):
+0001bc80: 0a20 2020 2022 2222 5772 6974 6520 7468  .    """Write th
+0001bc90: 6973 2065 6e74 6974 7920 746f 2043 6c6f  is entity to Clo
+0001bca0: 7564 2044 6174 6173 746f 7265 2e0a 0a20  ud Datastore... 
+0001bcb0: 2020 2049 6620 7468 6520 6f70 6572 6174     If the operat
+0001bcc0: 696f 6e20 6372 6561 7465 7320 6f72 2063  ion creates or c
+0001bcd0: 6f6d 706c 6574 6573 2061 206b 6579 2c20  ompletes a key, 
+0001bce0: 7468 6520 656e 7469 7479 2773 206b 6579  the entity's key
+0001bcf0: 0a20 2020 2061 7474 7269 6275 7465 2069  .    attribute i
+0001bd00: 7320 7365 7420 746f 2074 6865 206e 6577  s set to the new
+0001bd10: 2c20 636f 6d70 6c65 7465 206b 6579 2e0a  , complete key..
+0001bd20: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+0001bd30: 2020 2020 5468 6520 6b65 7920 666f 7220      The key for 
+0001bd40: 7468 6520 656e 7469 7479 2e20 2054 6869  the entity.  Thi
+0001bd50: 7320 6973 2061 6c77 6179 7320 6120 636f  s is always a co
+0001bd60: 6d70 6c65 7465 206b 6579 2e0a 2020 2020  mplete key..    
+0001bd70: 2222 220a 2020 2020 7265 7475 726e 2073  """.    return s
+0001bd80: 656c 662e 5f70 7574 5f61 7379 6e63 282a  elf._put_async(*
+0001bd90: 2a63 7478 5f6f 7074 696f 6e73 292e 6765  *ctx_options).ge
+0001bda0: 745f 7265 7375 6c74 2829 0a20 2070 7574  t_result().  put
+0001bdb0: 203d 205f 7075 740a 0a20 2064 6566 205f   = _put..  def _
+0001bdc0: 7075 745f 6173 796e 6328 7365 6c66 2c20  put_async(self, 
+0001bdd0: 2a2a 6374 785f 6f70 7469 6f6e 7329 3a0a  **ctx_options):.
+0001bde0: 2020 2020 2222 2257 7269 7465 2074 6869      """Write thi
+0001bdf0: 7320 656e 7469 7479 2074 6f20 436c 6f75  s entity to Clou
+0001be00: 6420 4461 7461 7374 6f72 652e 0a0a 2020  d Datastore...  
+0001be10: 2020 5468 6973 2069 7320 7468 6520 6173    This is the as
+0001be20: 796e 6368 726f 6e6f 7573 2076 6572 7369  ynchronous versi
+0001be30: 6f6e 206f 6620 4d6f 6465 6c2e 5f70 7574  on of Model._put
+0001be40: 2829 2e0a 2020 2020 2222 220a 2020 2020  ()..    """.    
+0001be50: 6966 2073 656c 662e 5f70 726f 6a65 6374  if self._project
+0001be60: 696f 6e3a 0a20 2020 2020 2072 6169 7365  ion:.      raise
+0001be70: 2064 6174 6173 746f 7265 5f65 7272 6f72   datastore_error
+0001be80: 732e 4261 6452 6571 7565 7374 4572 726f  s.BadRequestErro
+0001be90: 7228 2743 616e 6e6f 7420 7075 7420 6120  r('Cannot put a 
+0001bea0: 7061 7274 6961 6c20 656e 7469 7479 2729  partial entity')
+0001beb0: 0a20 2020 2066 726f 6d20 676f 6f67 6c65  .    from google
+0001bec0: 2e61 7070 656e 6769 6e65 2e65 7874 2e6e  .appengine.ext.n
+0001bed0: 6462 2069 6d70 6f72 7420 7461 736b 6c65  db import taskle
+0001bee0: 7473 0a20 2020 2063 7478 203d 2074 6173  ts.    ctx = tas
+0001bef0: 6b6c 6574 732e 6765 745f 636f 6e74 6578  klets.get_contex
+0001bf00: 7428 290a 2020 2020 7365 6c66 2e5f 7072  t().    self._pr
+0001bf10: 6570 6172 655f 666f 725f 7075 7428 290a  epare_for_put().
+0001bf20: 2020 2020 6966 2073 656c 662e 5f6b 6579      if self._key
+0001bf30: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0001bf40: 7365 6c66 2e5f 6b65 7920 3d20 4b65 7928  self._key = Key(
+0001bf50: 7365 6c66 2e5f 6765 745f 6b69 6e64 2829  self._get_kind()
+0001bf60: 2c20 4e6f 6e65 290a 2020 2020 7365 6c66  , None).    self
+0001bf70: 2e5f 7072 655f 7075 745f 686f 6f6b 2829  ._pre_put_hook()
+0001bf80: 0a20 2020 2066 7574 203d 2063 7478 2e70  .    fut = ctx.p
+0001bf90: 7574 2873 656c 662c 202a 2a63 7478 5f6f  ut(self, **ctx_o
+0001bfa0: 7074 696f 6e73 290a 2020 2020 706f 7374  ptions).    post
+0001bfb0: 5f68 6f6f 6b20 3d20 7365 6c66 2e5f 706f  _hook = self._po
+0001bfc0: 7374 5f70 7574 5f68 6f6f 6b0a 2020 2020  st_put_hook.    
+0001bfd0: 6966 206e 6f74 2073 656c 662e 5f69 735f  if not self._is_
+0001bfe0: 6465 6661 756c 745f 686f 6f6b 284d 6f64  default_hook(Mod
+0001bff0: 656c 2e5f 6465 6661 756c 745f 706f 7374  el._default_post
+0001c000: 5f70 7574 5f68 6f6f 6b2c 2070 6f73 745f  _put_hook, post_
+0001c010: 686f 6f6b 293a 0a20 2020 2020 2066 7574  hook):.      fut
+0001c020: 2e61 6464 5f69 6d6d 6564 6961 7465 5f63  .add_immediate_c
+0001c030: 616c 6c62 6163 6b28 706f 7374 5f68 6f6f  allback(post_hoo
+0001c040: 6b2c 2066 7574 290a 2020 2020 7265 7475  k, fut).    retu
+0001c050: 726e 2066 7574 0a20 2070 7574 5f61 7379  rn fut.  put_asy
+0001c060: 6e63 203d 205f 7075 745f 6173 796e 630a  nc = _put_async.
+0001c070: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
+0001c080: 2020 6465 6620 5f67 6574 5f6f 725f 696e    def _get_or_in
+0001c090: 7365 7274 282a 6172 6773 2c20 2a2a 6b77  sert(*args, **kw
+0001c0a0: 6473 293a 0a20 2020 2022 2222 5472 616e  ds):.    """Tran
+0001c0b0: 7361 6374 696f 6e61 6c6c 7920 7265 7472  sactionally retr
+0001c0c0: 6965 7665 7320 616e 2065 7869 7374 696e  ieves an existin
+0001c0d0: 6720 656e 7469 7479 206f 7220 6372 6561  g entity or crea
+0001c0e0: 7465 7320 6120 6e65 7720 6f6e 652e 0a0a  tes a new one...
+0001c0f0: 2020 2020 506f 7369 7469 6f6e 616c 2041      Positional A
+0001c100: 7267 733a 0a20 2020 2020 206e 616d 653a  rgs:.      name:
+0001c110: 204b 6579 206e 616d 6520 746f 2072 6574   Key name to ret
+0001c120: 7269 6576 6520 6f72 2063 7265 6174 652e  rieve or create.
+0001c130: 0a0a 2020 2020 4b65 7977 6f72 6420 4172  ..    Keyword Ar
+0001c140: 6773 3a0a 2020 2020 2020 6e61 6d65 7370  gs:.      namesp
+0001c150: 6163 653a 204f 7074 696f 6e61 6c20 6e61  ace: Optional na
+0001c160: 6d65 7370 6163 652e 0a20 2020 2020 2061  mespace..      a
+0001c170: 7070 3a20 4f70 7469 6f6e 616c 2061 7070  pp: Optional app
+0001c180: 2049 442e 0a20 2020 2020 2070 6172 656e   ID..      paren
+0001c190: 743a 2050 6172 656e 7420 656e 7469 7479  t: Parent entity
+0001c1a0: 206b 6579 2c20 6966 2061 6e79 2e0a 2020   key, if any..  
+0001c1b0: 2020 2020 636f 6e74 6578 745f 6f70 7469      context_opti
+0001c1c0: 6f6e 733a 2043 6f6e 7465 7874 4f70 7469  ons: ContextOpti
+0001c1d0: 6f6e 7320 6f62 6a65 6374 2028 6e6f 7420  ons object (not 
+0001c1e0: 6b65 7977 6f72 6420 6172 6773 2129 206f  keyword args!) o
+0001c1f0: 7220 4e6f 6e65 2e0a 2020 2020 2020 2a2a  r None..      **
+0001c200: 6b77 6473 3a20 4b65 7977 6f72 6420 6172  kwds: Keyword ar
+0001c210: 6775 6d65 6e74 7320 746f 2070 6173 7320  guments to pass 
+0001c220: 746f 2074 6865 2063 6f6e 7374 7275 6374  to the construct
+0001c230: 6f72 206f 6620 7468 6520 6d6f 6465 6c20  or of the model 
+0001c240: 636c 6173 730a 2020 2020 2020 2020 6966  class.        if
+0001c250: 2061 6e20 696e 7374 616e 6365 2066 6f72   an instance for
+0001c260: 2074 6865 2073 7065 6369 6669 6564 206b   the specified k
+0001c270: 6579 206e 616d 6520 646f 6573 206e 6f74  ey name does not
+0001c280: 2061 6c72 6561 6479 2065 7869 7374 2e20   already exist. 
+0001c290: 4966 0a20 2020 2020 2020 2061 6e20 696e  If.        an in
+0001c2a0: 7374 616e 6365 2077 6974 6820 7468 6520  stance with the 
+0001c2b0: 7375 7070 6c69 6564 206b 6579 5f6e 616d  supplied key_nam
+0001c2c0: 6520 616e 6420 7061 7265 6e74 2061 6c72  e and parent alr
+0001c2d0: 6561 6479 2065 7869 7374 732c 0a20 2020  eady exists,.   
+0001c2e0: 2020 2020 2074 6865 7365 2061 7267 756d       these argum
+0001c2f0: 656e 7473 2077 696c 6c20 6265 2064 6973  ents will be dis
+0001c300: 6361 7264 6564 2e0a 0a20 2020 2052 6574  carded...    Ret
+0001c310: 7572 6e73 3a0a 2020 2020 2020 4578 6973  urns:.      Exis
+0001c320: 7469 6e67 2069 6e73 7461 6e63 6520 6f66  ting instance of
+0001c330: 204d 6f64 656c 2063 6c61 7373 2077 6974   Model class wit
+0001c340: 6820 7468 6520 7370 6563 6966 6965 6420  h the specified 
+0001c350: 6b65 7920 6e61 6d65 2061 6e64 2070 6172  key name and par
+0001c360: 656e 740a 2020 2020 2020 6f72 2061 206e  ent.      or a n
+0001c370: 6577 206f 6e65 2074 6861 7420 6861 7320  ew one that has 
+0001c380: 6a75 7374 2062 6565 6e20 6372 6561 7465  just been create
+0001c390: 642e 0a20 2020 2022 2222 0a20 2020 2063  d..    """.    c
+0001c3a0: 6c73 2c20 6172 6773 203d 2061 7267 735b  ls, args = args[
+0001c3b0: 305d 2c20 6172 6773 5b31 3a5d 0a20 2020  0], args[1:].   
+0001c3c0: 2072 6574 7572 6e20 636c 732e 5f67 6574   return cls._get
+0001c3d0: 5f6f 725f 696e 7365 7274 5f61 7379 6e63  _or_insert_async
+0001c3e0: 282a 6172 6773 2c20 2a2a 6b77 6473 292e  (*args, **kwds).
+0001c3f0: 6765 745f 7265 7375 6c74 2829 0a20 2067  get_result().  g
+0001c400: 6574 5f6f 725f 696e 7365 7274 203d 205f  et_or_insert = _
+0001c410: 6765 745f 6f72 5f69 6e73 6572 740a 0a20  get_or_insert.. 
+0001c420: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+0001c430: 6465 6620 5f67 6574 5f6f 725f 696e 7365  def _get_or_inse
+0001c440: 7274 5f61 7379 6e63 282a 6172 6773 2c20  rt_async(*args, 
+0001c450: 2a2a 6b77 6473 293a 0a20 2020 2022 2222  **kwds):.    """
+0001c460: 5472 616e 7361 6374 696f 6e61 6c6c 7920  Transactionally 
+0001c470: 7265 7472 6965 7665 7320 616e 2065 7869  retrieves an exi
+0001c480: 7374 696e 6720 656e 7469 7479 206f 7220  sting entity or 
+0001c490: 6372 6561 7465 7320 6120 6e65 7720 6f6e  creates a new on
+0001c4a0: 652e 0a0a 2020 2020 5468 6973 2069 7320  e...    This is 
+0001c4b0: 7468 6520 6173 796e 6368 726f 6e6f 7573  the asynchronous
+0001c4c0: 2076 6572 7369 6f6e 206f 6620 4d6f 6465   version of Mode
+0001c4d0: 6c2e 5f67 6574 5f6f 725f 696e 7365 7274  l._get_or_insert
+0001c4e0: 2829 2e0a 2020 2020 2222 220a 0a0a 2020  ()..    """...  
+0001c4f0: 2020 6672 6f6d 2067 6f6f 676c 652e 6170    from google.ap
+0001c500: 7065 6e67 696e 652e 6578 742e 6e64 6220  pengine.ext.ndb 
+0001c510: 696d 706f 7274 2074 6173 6b6c 6574 730a  import tasklets.
+0001c520: 2020 2020 636c 732c 206e 616d 6520 3d20      cls, name = 
+0001c530: 6172 6773 0a20 2020 2067 6574 5f61 7267  args.    get_arg
+0001c540: 203d 2063 6c73 2e5f 5f67 6574 5f61 7267   = cls.__get_arg
+0001c550: 0a20 2020 2061 7070 203d 2067 6574 5f61  .    app = get_a
+0001c560: 7267 286b 7764 732c 2027 6170 7027 290a  rg(kwds, 'app').
+0001c570: 2020 2020 6e61 6d65 7370 6163 6520 3d20      namespace = 
+0001c580: 6765 745f 6172 6728 6b77 6473 2c20 276e  get_arg(kwds, 'n
+0001c590: 616d 6573 7061 6365 2729 0a20 2020 2070  amespace').    p
+0001c5a0: 6172 656e 7420 3d20 6765 745f 6172 6728  arent = get_arg(
+0001c5b0: 6b77 6473 2c20 2770 6172 656e 7427 290a  kwds, 'parent').
+0001c5c0: 2020 2020 636f 6e74 6578 745f 6f70 7469      context_opti
+0001c5d0: 6f6e 7320 3d20 6765 745f 6172 6728 6b77  ons = get_arg(kw
+0001c5e0: 6473 2c20 2763 6f6e 7465 7874 5f6f 7074  ds, 'context_opt
+0001c5f0: 696f 6e73 2729 0a0a 0a20 2020 2069 6620  ions')...    if 
+0001c600: 6e6f 7420 6973 696e 7374 616e 6365 286e  not isinstance(n
+0001c610: 616d 652c 2073 6978 2e73 7472 696e 675f  ame, six.string_
+0001c620: 7479 7065 7329 3a0a 2020 2020 2020 7261  types):.      ra
+0001c630: 6973 6520 5479 7065 4572 726f 7228 276e  ise TypeError('n
+0001c640: 616d 6520 6d75 7374 2062 6520 6120 7374  ame must be a st
+0001c650: 7269 6e67 3b20 7265 6365 6976 6564 2025  ring; received %
+0001c660: 7227 2025 206e 616d 6529 0a20 2020 2065  r' % name).    e
+0001c670: 6c69 6620 6e6f 7420 6e61 6d65 3a0a 2020  lif not name:.  
+0001c680: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0001c690: 7272 6f72 2827 6e61 6d65 2063 616e 6e6f  rror('name canno
+0001c6a0: 7420 6265 2061 6e20 656d 7074 7920 7374  t be an empty st
+0001c6b0: 7269 6e67 2e27 290a 2020 2020 6b65 7920  ring.').    key 
+0001c6c0: 3d20 4b65 7928 636c 732c 206e 616d 652c  = Key(cls, name,
+0001c6d0: 2061 7070 3d61 7070 2c20 6e61 6d65 7370   app=app, namesp
+0001c6e0: 6163 653d 6e61 6d65 7370 6163 652c 2070  ace=namespace, p
+0001c6f0: 6172 656e 743d 7061 7265 6e74 290a 0a20  arent=parent).. 
+0001c700: 2020 2040 7461 736b 6c65 7473 2e74 6173     @tasklets.tas
+0001c710: 6b6c 6574 0a20 2020 2064 6566 2069 6e74  klet.    def int
+0001c720: 6572 6e61 6c5f 7461 736b 6c65 7428 293a  ernal_tasklet():
+0001c730: 0a20 2020 2020 2040 7461 736b 6c65 7473  .      @tasklets
+0001c740: 2e74 6173 6b6c 6574 0a20 2020 2020 2064  .tasklet.      d
+0001c750: 6566 2074 786e 2829 3a0a 2020 2020 2020  ef txn():.      
+0001c760: 2020 656e 7420 3d20 7969 656c 6420 6b65    ent = yield ke
+0001c770: 792e 6765 745f 6173 796e 6328 6f70 7469  y.get_async(opti
+0001c780: 6f6e 733d 636f 6e74 6578 745f 6f70 7469  ons=context_opti
+0001c790: 6f6e 7329 0a20 2020 2020 2020 2069 6620  ons).        if 
+0001c7a0: 656e 7420 6973 204e 6f6e 653a 0a20 2020  ent is None:.   
+0001c7b0: 2020 2020 2020 2065 6e74 203d 2063 6c73         ent = cls
+0001c7c0: 282a 2a6b 7764 7329 0a20 2020 2020 2020  (**kwds).       
+0001c7d0: 2020 2065 6e74 2e5f 6b65 7920 3d20 6b65     ent._key = ke
+0001c7e0: 790a 2020 2020 2020 2020 2020 7969 656c  y.          yiel
+0001c7f0: 6420 656e 742e 7075 745f 6173 796e 6328  d ent.put_async(
+0001c800: 6f70 7469 6f6e 733d 636f 6e74 6578 745f  options=context_
+0001c810: 6f70 7469 6f6e 7329 0a20 2020 2020 2020  options).       
+0001c820: 2072 6169 7365 2074 6173 6b6c 6574 732e   raise tasklets.
+0001c830: 5265 7475 726e 2865 6e74 290a 2020 2020  Return(ent).    
+0001c840: 2020 6966 2069 6e5f 7472 616e 7361 6374    if in_transact
+0001c850: 696f 6e28 293a 0a0a 2020 2020 2020 2020  ion():..        
+0001c860: 656e 7420 3d20 7969 656c 6420 7478 6e28  ent = yield txn(
+0001c870: 290a 2020 2020 2020 656c 7365 3a0a 0a20  ).      else:.. 
+0001c880: 2020 2020 2020 2065 6e74 203d 2079 6965         ent = yie
+0001c890: 6c64 206b 6579 2e67 6574 5f61 7379 6e63  ld key.get_async
+0001c8a0: 286f 7074 696f 6e73 3d63 6f6e 7465 7874  (options=context
+0001c8b0: 5f6f 7074 696f 6e73 290a 2020 2020 2020  _options).      
+0001c8c0: 2020 6966 2065 6e74 2069 7320 4e6f 6e65    if ent is None
+0001c8d0: 3a0a 0a20 2020 2020 2020 2020 2065 6e74  :..          ent
+0001c8e0: 203d 2079 6965 6c64 2074 7261 6e73 6163   = yield transac
+0001c8f0: 7469 6f6e 5f61 7379 6e63 2874 786e 290a  tion_async(txn).
+0001c900: 2020 2020 2020 7261 6973 6520 7461 736b        raise task
+0001c910: 6c65 7473 2e52 6574 7572 6e28 656e 7429  lets.Return(ent)
+0001c920: 0a0a 2020 2020 7265 7475 726e 2069 6e74  ..    return int
+0001c930: 6572 6e61 6c5f 7461 736b 6c65 7428 290a  ernal_tasklet().
+0001c940: 0a20 2067 6574 5f6f 725f 696e 7365 7274  .  get_or_insert
+0001c950: 5f61 7379 6e63 203d 205f 6765 745f 6f72  _async = _get_or
+0001c960: 5f69 6e73 6572 745f 6173 796e 630a 0a20  _insert_async.. 
+0001c970: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+0001c980: 6465 6620 5f61 6c6c 6f63 6174 655f 6964  def _allocate_id
+0001c990: 7328 636c 732c 2073 697a 653d 4e6f 6e65  s(cls, size=None
+0001c9a0: 2c20 6d61 783d 4e6f 6e65 2c20 7061 7265  , max=None, pare
+0001c9b0: 6e74 3d4e 6f6e 652c 202a 2a63 7478 5f6f  nt=None, **ctx_o
+0001c9c0: 7074 696f 6e73 293a 0a20 2020 2022 2222  ptions):.    """
+0001c9d0: 416c 6c6f 6361 7465 7320 6120 7261 6e67  Allocates a rang
+0001c9e0: 6520 6f66 206b 6579 2049 4473 2066 6f72  e of key IDs for
+0001c9f0: 2074 6869 7320 6d6f 6465 6c20 636c 6173   this model clas
+0001ca00: 732e 0a0a 2020 2020 4172 6773 3a0a 2020  s...    Args:.  
+0001ca10: 2020 2020 7369 7a65 3a20 4e75 6d62 6572      size: Number
+0001ca20: 206f 6620 4944 7320 746f 2061 6c6c 6f63   of IDs to alloc
+0001ca30: 6174 652e 2045 6974 6865 7220 7369 7a65  ate. Either size
+0001ca40: 206f 7220 6d61 7820 6361 6e20 6265 2073   or max can be s
+0001ca50: 7065 6369 6669 6564 2c0a 2020 2020 2020  pecified,.      
+0001ca60: 2020 6e6f 7420 626f 7468 2e0a 2020 2020    not both..    
+0001ca70: 2020 6d61 783a 204d 6178 696d 756d 2049    max: Maximum I
+0001ca80: 4420 746f 2061 6c6c 6f63 6174 652e 2045  D to allocate. E
+0001ca90: 6974 6865 7220 7369 7a65 206f 7220 6d61  ither size or ma
+0001caa0: 7820 6361 6e20 6265 2073 7065 6369 6669  x can be specifi
+0001cab0: 6564 2c0a 2020 2020 2020 2020 6e6f 7420  ed,.        not 
+0001cac0: 626f 7468 2e0a 2020 2020 2020 7061 7265  both..      pare
+0001cad0: 6e74 3a20 5061 7265 6e74 206b 6579 2066  nt: Parent key f
+0001cae0: 6f72 2077 6869 6368 2074 6865 2049 4473  or which the IDs
+0001caf0: 2077 696c 6c20 6265 2061 6c6c 6f63 6174   will be allocat
+0001cb00: 6564 2e0a 2020 2020 2020 2a2a 6374 785f  ed..      **ctx_
+0001cb10: 6f70 7469 6f6e 733a 2043 6f6e 7465 7874  options: Context
+0001cb20: 206f 7074 696f 6e73 2e0a 0a20 2020 2052   options...    R
+0001cb30: 6574 7572 6e73 3a0a 2020 2020 2020 4120  eturns:.      A 
+0001cb40: 7475 706c 6520 7769 7468 2028 7374 6172  tuple with (star
+0001cb50: 742c 2065 6e64 2920 666f 7220 7468 6520  t, end) for the 
+0001cb60: 616c 6c6f 6361 7465 6420 7261 6e67 652c  allocated range,
+0001cb70: 2069 6e63 6c75 7369 7665 2e0a 2020 2020   inclusive..    
+0001cb80: 2222 220a 2020 2020 7265 7475 726e 2063  """.    return c
+0001cb90: 6c73 2e5f 616c 6c6f 6361 7465 5f69 6473  ls._allocate_ids
+0001cba0: 5f61 7379 6e63 2873 697a 653d 7369 7a65  _async(size=size
+0001cbb0: 2c20 6d61 783d 6d61 782c 2070 6172 656e  , max=max, paren
+0001cbc0: 743d 7061 7265 6e74 2c0a 2020 2020 2020  t=parent,.      
+0001cbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cbe0: 2020 2020 2020 2020 2020 2020 202a 2a63               **c
+0001cbf0: 7478 5f6f 7074 696f 6e73 292e 6765 745f  tx_options).get_
+0001cc00: 7265 7375 6c74 2829 0a20 2061 6c6c 6f63  result().  alloc
+0001cc10: 6174 655f 6964 7320 3d20 5f61 6c6c 6f63  ate_ids = _alloc
+0001cc20: 6174 655f 6964 730a 0a20 2040 636c 6173  ate_ids..  @clas
+0001cc30: 736d 6574 686f 640a 2020 6465 6620 5f61  smethod.  def _a
+0001cc40: 6c6c 6f63 6174 655f 6964 735f 6173 796e  llocate_ids_asyn
+0001cc50: 6328 636c 732c 2073 697a 653d 4e6f 6e65  c(cls, size=None
+0001cc60: 2c20 6d61 783d 4e6f 6e65 2c20 7061 7265  , max=None, pare
+0001cc70: 6e74 3d4e 6f6e 652c 0a20 2020 2020 2020  nt=None,.       
+0001cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cc90: 2020 202a 2a63 7478 5f6f 7074 696f 6e73     **ctx_options
+0001cca0: 293a 0a20 2020 2022 2222 416c 6c6f 6361  ):.    """Alloca
+0001ccb0: 7465 7320 6120 7261 6e67 6520 6f66 206b  tes a range of k
+0001ccc0: 6579 2049 4473 2066 6f72 2074 6869 7320  ey IDs for this 
+0001ccd0: 6d6f 6465 6c20 636c 6173 732e 0a0a 2020  model class...  
+0001cce0: 2020 5468 6973 2069 7320 7468 6520 6173    This is the as
+0001ccf0: 796e 6368 726f 6e6f 7573 2076 6572 7369  ynchronous versi
+0001cd00: 6f6e 206f 6620 4d6f 6465 6c2e 5f61 6c6c  on of Model._all
+0001cd10: 6f63 6174 655f 6964 7328 292e 0a20 2020  ocate_ids()..   
+0001cd20: 2022 2222 0a20 2020 2066 726f 6d20 676f   """.    from go
+0001cd30: 6f67 6c65 2e61 7070 656e 6769 6e65 2e65  ogle.appengine.e
+0001cd40: 7874 2e6e 6462 2069 6d70 6f72 7420 7461  xt.ndb import ta
+0001cd50: 736b 6c65 7473 0a20 2020 2063 7478 203d  sklets.    ctx =
+0001cd60: 2074 6173 6b6c 6574 732e 6765 745f 636f   tasklets.get_co
+0001cd70: 6e74 6578 7428 290a 2020 2020 636c 732e  ntext().    cls.
+0001cd80: 5f70 7265 5f61 6c6c 6f63 6174 655f 6964  _pre_allocate_id
+0001cd90: 735f 686f 6f6b 2873 697a 652c 206d 6178  s_hook(size, max
+0001cda0: 2c20 7061 7265 6e74 290a 2020 2020 6b65  , parent).    ke
+0001cdb0: 7920 3d20 4b65 7928 636c 732e 5f67 6574  y = Key(cls._get
+0001cdc0: 5f6b 696e 6428 292c 204e 6f6e 652c 2070  _kind(), None, p
+0001cdd0: 6172 656e 743d 7061 7265 6e74 290a 2020  arent=parent).  
+0001cde0: 2020 6675 7420 3d20 6374 782e 616c 6c6f    fut = ctx.allo
+0001cdf0: 6361 7465 5f69 6473 286b 6579 2c20 7369  cate_ids(key, si
+0001ce00: 7a65 3d73 697a 652c 206d 6178 3d6d 6178  ze=size, max=max
+0001ce10: 2c20 2a2a 6374 785f 6f70 7469 6f6e 7329  , **ctx_options)
+0001ce20: 0a20 2020 2070 6f73 745f 686f 6f6b 203d  .    post_hook =
+0001ce30: 2063 6c73 2e5f 706f 7374 5f61 6c6c 6f63   cls._post_alloc
+0001ce40: 6174 655f 6964 735f 686f 6f6b 0a20 2020  ate_ids_hook.   
+0001ce50: 2069 6620 6e6f 7420 636c 732e 5f69 735f   if not cls._is_
+0001ce60: 6465 6661 756c 745f 686f 6f6b 284d 6f64  default_hook(Mod
+0001ce70: 656c 2e5f 6465 6661 756c 745f 706f 7374  el._default_post
+0001ce80: 5f61 6c6c 6f63 6174 655f 6964 735f 686f  _allocate_ids_ho
+0001ce90: 6f6b 2c0a 2020 2020 2020 2020 2020 2020  ok,.            
+0001cea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ceb0: 2020 2020 706f 7374 5f68 6f6f 6b29 3a0a      post_hook):.
+0001cec0: 2020 2020 2020 6675 742e 6164 645f 696d        fut.add_im
+0001ced0: 6d65 6469 6174 655f 6361 6c6c 6261 636b  mediate_callback
+0001cee0: 2870 6f73 745f 686f 6f6b 2c20 7369 7a65  (post_hook, size
+0001cef0: 2c20 6d61 782c 2070 6172 656e 742c 2066  , max, parent, f
+0001cf00: 7574 290a 2020 2020 7265 7475 726e 2066  ut).    return f
+0001cf10: 7574 0a20 2061 6c6c 6f63 6174 655f 6964  ut.  allocate_id
+0001cf20: 735f 6173 796e 6320 3d20 5f61 6c6c 6f63  s_async = _alloc
+0001cf30: 6174 655f 6964 735f 6173 796e 630a 0a20  ate_ids_async.. 
+0001cf40: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+0001cf50: 4075 7469 6c73 2e70 6f73 6974 696f 6e61  @utils.positiona
+0001cf60: 6c28 3329 0a20 2064 6566 205f 6765 745f  l(3).  def _get_
+0001cf70: 6279 5f69 6428 636c 732c 2069 642c 2070  by_id(cls, id, p
+0001cf80: 6172 656e 743d 4e6f 6e65 2c20 2a2a 6374  arent=None, **ct
+0001cf90: 785f 6f70 7469 6f6e 7329 3a0a 2020 2020  x_options):.    
+0001cfa0: 2222 2252 6574 7572 6e73 2061 6e20 696e  """Returns an in
+0001cfb0: 7374 616e 6365 206f 6620 4d6f 6465 6c20  stance of Model 
+0001cfc0: 636c 6173 7320 6279 2049 442e 0a0a 2020  class by ID...  
+0001cfd0: 2020 5468 6973 2069 7320 7265 616c 6c79    This is really
+0001cfe0: 206a 7573 7420 6120 7368 6f72 7468 616e   just a shorthan
+0001cff0: 6420 666f 7220 4b65 7928 636c 732c 2069  d for Key(cls, i
+0001d000: 642c 202e 2e2e 292e 6765 7428 292e 0a0a  d, ...).get()...
+0001d010: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0001d020: 6964 3a20 4120 7374 7269 6e67 206f 7220  id: A string or 
+0001d030: 696e 7465 6765 7220 6b65 7920 4944 2e0a  integer key ID..
+0001d040: 2020 2020 2020 7061 7265 6e74 3a20 4f70        parent: Op
+0001d050: 7469 6f6e 616c 2070 6172 656e 7420 6b65  tional parent ke
+0001d060: 7920 6f66 2074 6865 206d 6f64 656c 2074  y of the model t
+0001d070: 6f20 6765 742e 0a20 2020 2020 206e 616d  o get..      nam
+0001d080: 6573 7061 6365 3a20 4f70 7469 6f6e 616c  espace: Optional
+0001d090: 206e 616d 6573 7061 6365 2e0a 2020 2020   namespace..    
+0001d0a0: 2020 6170 703a 204f 7074 696f 6e61 6c20    app: Optional 
+0001d0b0: 6170 7020 4944 2e0a 2020 2020 2020 2a2a  app ID..      **
+0001d0c0: 6374 785f 6f70 7469 6f6e 733a 2043 6f6e  ctx_options: Con
+0001d0d0: 7465 7874 206f 7074 696f 6e73 2e0a 0a20  text options... 
+0001d0e0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0001d0f0: 2020 4120 6d6f 6465 6c20 696e 7374 616e    A model instan
+0001d100: 6365 206f 7220 4e6f 6e65 2069 6620 6e6f  ce or None if no
+0001d110: 7420 666f 756e 642e 0a20 2020 2022 2222  t found..    """
+0001d120: 0a20 2020 2072 6574 7572 6e20 636c 732e  .    return cls.
+0001d130: 5f67 6574 5f62 795f 6964 5f61 7379 6e63  _get_by_id_async
+0001d140: 2869 642c 2070 6172 656e 743d 7061 7265  (id, parent=pare
+0001d150: 6e74 2c20 2a2a 6374 785f 6f70 7469 6f6e  nt, **ctx_option
+0001d160: 7329 2e67 6574 5f72 6573 756c 7428 290a  s).get_result().
+0001d170: 2020 6765 745f 6279 5f69 6420 3d20 5f67    get_by_id = _g
+0001d180: 6574 5f62 795f 6964 0a0a 2020 4063 6c61  et_by_id..  @cla
+0001d190: 7373 6d65 7468 6f64 0a20 2040 7574 696c  ssmethod.  @util
+0001d1a0: 732e 706f 7369 7469 6f6e 616c 2833 290a  s.positional(3).
+0001d1b0: 2020 6465 6620 5f67 6574 5f62 795f 6964    def _get_by_id
+0001d1c0: 5f61 7379 6e63 2863 6c73 2c20 6964 2c20  _async(cls, id, 
+0001d1d0: 7061 7265 6e74 3d4e 6f6e 652c 2061 7070  parent=None, app
+0001d1e0: 3d4e 6f6e 652c 206e 616d 6573 7061 6365  =None, namespace
+0001d1f0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+0001d200: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
+0001d210: 6374 785f 6f70 7469 6f6e 7329 3a0a 2020  ctx_options):.  
+0001d220: 2020 2222 2252 6574 7572 6e73 2061 6e20    """Returns an 
+0001d230: 696e 7374 616e 6365 206f 6620 4d6f 6465  instance of Mode
+0001d240: 6c20 636c 6173 7320 6279 2049 4420 2861  l class by ID (a
+0001d250: 6e64 2061 7070 2c20 6e61 6d65 7370 6163  nd app, namespac
+0001d260: 6529 2e0a 0a20 2020 2054 6869 7320 6973  e)...    This is
+0001d270: 2074 6865 2061 7379 6e63 6872 6f6e 6f75   the asynchronou
+0001d280: 7320 7665 7273 696f 6e20 6f66 204d 6f64  s version of Mod
+0001d290: 656c 2e5f 6765 745f 6279 5f69 6428 292e  el._get_by_id().
+0001d2a0: 0a20 2020 2022 2222 0a20 2020 206b 6579  .    """.    key
+0001d2b0: 203d 204b 6579 2863 6c73 2e5f 6765 745f   = Key(cls._get_
+0001d2c0: 6b69 6e64 2829 2c20 6964 2c20 7061 7265  kind(), id, pare
+0001d2d0: 6e74 3d70 6172 656e 742c 2061 7070 3d61  nt=parent, app=a
+0001d2e0: 7070 2c20 6e61 6d65 7370 6163 653d 6e61  pp, namespace=na
+0001d2f0: 6d65 7370 6163 6529 0a20 2020 2072 6574  mespace).    ret
+0001d300: 7572 6e20 6b65 792e 6765 745f 6173 796e  urn key.get_asyn
+0001d310: 6328 2a2a 6374 785f 6f70 7469 6f6e 7329  c(**ctx_options)
+0001d320: 0a20 2067 6574 5f62 795f 6964 5f61 7379  .  get_by_id_asy
+0001d330: 6e63 203d 205f 6765 745f 6279 5f69 645f  nc = _get_by_id_
+0001d340: 6173 796e 630a 0a0a 0a0a 0a0a 0a0a 0a0a  async...........
+0001d350: 0a0a 0a0a 2020 4063 6c61 7373 6d65 7468  ....  @classmeth
+0001d360: 6f64 0a20 2064 6566 205f 7072 655f 616c  od.  def _pre_al
+0001d370: 6c6f 6361 7465 5f69 6473 5f68 6f6f 6b28  locate_ids_hook(
+0001d380: 636c 732c 2073 697a 652c 206d 6178 2c20  cls, size, max, 
+0001d390: 7061 7265 6e74 293a 0a20 2020 2070 6173  parent):.    pas
+0001d3a0: 730a 2020 5f64 6566 6175 6c74 5f70 7265  s.  _default_pre
+0001d3b0: 5f61 6c6c 6f63 6174 655f 6964 735f 686f  _allocate_ids_ho
+0001d3c0: 6f6b 203d 205f 7072 655f 616c 6c6f 6361  ok = _pre_alloca
+0001d3d0: 7465 5f69 6473 5f68 6f6f 6b0a 0a20 2040  te_ids_hook..  @
+0001d3e0: 636c 6173 736d 6574 686f 640a 2020 6465  classmethod.  de
+0001d3f0: 6620 5f70 6f73 745f 616c 6c6f 6361 7465  f _post_allocate
+0001d400: 5f69 6473 5f68 6f6f 6b28 636c 732c 2073  _ids_hook(cls, s
+0001d410: 697a 652c 206d 6178 2c20 7061 7265 6e74  ize, max, parent
+0001d420: 2c20 6675 7475 7265 293a 0a20 2020 2070  , future):.    p
+0001d430: 6173 730a 2020 5f64 6566 6175 6c74 5f70  ass.  _default_p
+0001d440: 6f73 745f 616c 6c6f 6361 7465 5f69 6473  ost_allocate_ids
+0001d450: 5f68 6f6f 6b20 3d20 5f70 6f73 745f 616c  _hook = _post_al
+0001d460: 6c6f 6361 7465 5f69 6473 5f68 6f6f 6b0a  locate_ids_hook.
+0001d470: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
+0001d480: 2020 6465 6620 5f70 7265 5f64 656c 6574    def _pre_delet
+0001d490: 655f 686f 6f6b 2863 6c73 2c20 6b65 7929  e_hook(cls, key)
+0001d4a0: 3a0a 2020 2020 7061 7373 0a20 205f 6465  :.    pass.  _de
+0001d4b0: 6661 756c 745f 7072 655f 6465 6c65 7465  fault_pre_delete
+0001d4c0: 5f68 6f6f 6b20 3d20 5f70 7265 5f64 656c  _hook = _pre_del
+0001d4d0: 6574 655f 686f 6f6b 0a0a 2020 4063 6c61  ete_hook..  @cla
+0001d4e0: 7373 6d65 7468 6f64 0a20 2064 6566 205f  ssmethod.  def _
+0001d4f0: 706f 7374 5f64 656c 6574 655f 686f 6f6b  post_delete_hook
+0001d500: 2863 6c73 2c20 6b65 792c 2066 7574 7572  (cls, key, futur
+0001d510: 6529 3a0a 2020 2020 7061 7373 0a20 205f  e):.    pass.  _
+0001d520: 6465 6661 756c 745f 706f 7374 5f64 656c  default_post_del
+0001d530: 6574 655f 686f 6f6b 203d 205f 706f 7374  ete_hook = _post
+0001d540: 5f64 656c 6574 655f 686f 6f6b 0a0a 2020  _delete_hook..  
+0001d550: 4063 6c61 7373 6d65 7468 6f64 0a20 2064  @classmethod.  d
+0001d560: 6566 205f 7072 655f 6765 745f 686f 6f6b  ef _pre_get_hook
+0001d570: 2863 6c73 2c20 6b65 7929 3a0a 2020 2020  (cls, key):.    
+0001d580: 7061 7373 0a20 205f 6465 6661 756c 745f  pass.  _default_
+0001d590: 7072 655f 6765 745f 686f 6f6b 203d 205f  pre_get_hook = _
+0001d5a0: 7072 655f 6765 745f 686f 6f6b 0a0a 2020  pre_get_hook..  
+0001d5b0: 4063 6c61 7373 6d65 7468 6f64 0a20 2064  @classmethod.  d
+0001d5c0: 6566 205f 706f 7374 5f67 6574 5f68 6f6f  ef _post_get_hoo
+0001d5d0: 6b28 636c 732c 206b 6579 2c20 6675 7475  k(cls, key, futu
+0001d5e0: 7265 293a 0a20 2020 2070 6173 730a 2020  re):.    pass.  
+0001d5f0: 5f64 6566 6175 6c74 5f70 6f73 745f 6765  _default_post_ge
+0001d600: 745f 686f 6f6b 203d 205f 706f 7374 5f67  t_hook = _post_g
+0001d610: 6574 5f68 6f6f 6b0a 0a20 2064 6566 205f  et_hook..  def _
+0001d620: 7072 655f 7075 745f 686f 6f6b 2873 656c  pre_put_hook(sel
+0001d630: 6629 3a0a 2020 2020 7061 7373 0a20 205f  f):.    pass.  _
+0001d640: 6465 6661 756c 745f 7072 655f 7075 745f  default_pre_put_
+0001d650: 686f 6f6b 203d 205f 7072 655f 7075 745f  hook = _pre_put_
+0001d660: 686f 6f6b 0a0a 2020 6465 6620 5f70 6f73  hook..  def _pos
+0001d670: 745f 7075 745f 686f 6f6b 2873 656c 662c  t_put_hook(self,
+0001d680: 2066 7574 7572 6529 3a0a 2020 2020 7061   future):.    pa
+0001d690: 7373 0a20 205f 6465 6661 756c 745f 706f  ss.  _default_po
+0001d6a0: 7374 5f70 7574 5f68 6f6f 6b20 3d20 5f70  st_put_hook = _p
+0001d6b0: 6f73 745f 7075 745f 686f 6f6b 0a0a 2020  ost_put_hook..  
+0001d6c0: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+0001d6d0: 6465 6620 5f69 735f 6465 6661 756c 745f  def _is_default_
+0001d6e0: 686f 6f6b 2864 6566 6175 6c74 5f68 6f6f  hook(default_hoo
+0001d6f0: 6b2c 2068 6f6f 6b29 3a0a 2020 2020 2222  k, hook):.    ""
+0001d700: 2243 6865 636b 7320 7768 6574 6865 7220  "Checks whether 
+0001d710: 6120 7370 6563 6966 6963 2068 6f6f 6b20  a specific hook 
+0001d720: 6973 2069 6e20 6974 7320 6465 6661 756c  is in its defaul
+0001d730: 7420 7374 6174 652e 0a0a 2020 2020 4172  t state...    Ar
+0001d740: 6773 3a0a 2020 2020 2020 6465 6661 756c  gs:.      defaul
+0001d750: 745f 686f 6f6b 3a20 4361 6c6c 6162 6c65  t_hook: Callable
+0001d760: 2073 7065 6369 6669 6564 2062 7920 6e64   specified by nd
+0001d770: 6220 696e 7465 726e 616c 6c79 2028 646f  b internally (do
+0001d780: 206e 6f74 206f 7665 7272 6964 6529 2e0a   not override)..
+0001d790: 2020 2020 2020 686f 6f6b 3a20 5468 6520        hook: The 
+0001d7a0: 686f 6f6b 2064 6566 696e 6564 2062 7920  hook defined by 
+0001d7b0: 6120 6d6f 6465 6c20 636c 6173 7320 7573  a model class us
+0001d7c0: 696e 6720 5f70 6f73 745f 2a5f 686f 6f6b  ing _post_*_hook
+0001d7d0: 2e0a 0a20 2020 2052 6169 7365 733a 0a20  ...    Raises:. 
+0001d7e0: 2020 2020 2054 7970 6545 7272 6f72 2069       TypeError i
+0001d7f0: 6620 6569 7468 6572 2074 6865 2064 6566  f either the def
+0001d800: 6175 6c74 2068 6f6f 6b20 6f72 2074 6865  ault hook or the
+0001d810: 2074 6573 7465 6420 686f 6f6b 2061 7265   tested hook are
+0001d820: 206e 6f74 2063 616c 6c61 626c 652e 0a20   not callable.. 
+0001d830: 2020 2022 2222 0a20 2020 2069 6620 6e6f     """.    if no
+0001d840: 7420 6861 7361 7474 7228 6465 6661 756c  t hasattr(defaul
+0001d850: 745f 686f 6f6b 2c20 275f 5f63 616c 6c5f  t_hook, '__call_
+0001d860: 5f27 293a 0a20 2020 2020 2072 6169 7365  _'):.      raise
+0001d870: 2054 7970 6545 7272 6f72 2827 4465 6661   TypeError('Defa
+0001d880: 756c 7420 686f 6f6b 7320 666f 7220 6e64  ult hooks for nd
+0001d890: 622e 6d6f 6465 6c2e 4d6f 6465 6c20 6d75  b.model.Model mu
+0001d8a0: 7374 2062 6520 6361 6c6c 6162 6c65 2729  st be callable')
+0001d8b0: 0a20 2020 2069 6620 6e6f 7420 6861 7361  .    if not hasa
+0001d8c0: 7474 7228 686f 6f6b 2c20 275f 5f63 616c  ttr(hook, '__cal
+0001d8d0: 6c5f 5f27 293a 0a20 2020 2020 2072 6169  l__'):.      rai
+0001d8e0: 7365 2054 7970 6545 7272 6f72 2827 486f  se TypeError('Ho
+0001d8f0: 6f6b 7320 6d75 7374 2062 6520 6361 6c6c  oks must be call
+0001d900: 6162 6c65 2729 0a0a 0a0a 0a0a 2020 2020  able')......    
+0001d910: 6966 2068 6173 6174 7472 2864 6566 6175  if hasattr(defau
+0001d920: 6c74 5f68 6f6f 6b2c 2027 5f5f 6675 6e63  lt_hook, '__func
+0001d930: 5f5f 2729 3a0a 2020 2020 2020 6465 6661  __'):.      defa
+0001d940: 756c 745f 686f 6f6b 203d 2064 6566 6175  ult_hook = defau
+0001d950: 6c74 5f68 6f6f 6b2e 5f5f 6675 6e63 5f5f  lt_hook.__func__
+0001d960: 0a20 2020 2069 6620 6861 7361 7474 7228  .    if hasattr(
+0001d970: 686f 6f6b 2c20 275f 5f66 756e 635f 5f27  hook, '__func__'
+0001d980: 293a 0a20 2020 2020 2068 6f6f 6b20 3d20  ):.      hook = 
+0001d990: 686f 6f6b 2e5f 5f66 756e 635f 5f0a 0a20  hook.__func__.. 
+0001d9a0: 2020 2072 6574 7572 6e20 6465 6661 756c     return defaul
+0001d9b0: 745f 686f 6f6b 2069 7320 686f 6f6b 0a0a  t_hook is hook..
+0001d9c0: 0a63 6c61 7373 2045 7870 616e 646f 284d  .class Expando(M
+0001d9d0: 6f64 656c 293a 0a20 2022 2222 4d6f 6465  odel):.  """Mode
+0001d9e0: 6c20 7375 6263 6c61 7373 2074 6f20 7375  l subclass to su
+0001d9f0: 7070 6f72 7420 6479 6e61 6d69 6320 5072  pport dynamic Pr
+0001da00: 6f70 6572 7479 206e 616d 6573 2061 6e64  operty names and
+0001da10: 2074 7970 6573 2e0a 0a20 2053 6565 2074   types...  See t
+0001da20: 6865 206d 6f64 756c 6520 646f 6373 7472  he module docstr
+0001da30: 696e 6720 666f 7220 6465 7461 696c 732e  ing for details.
+0001da40: 0a20 2022 2222 0a0a 0a0a 2020 5f64 6566  .  """....  _def
+0001da50: 6175 6c74 5f69 6e64 6578 6564 203d 2054  ault_indexed = T
+0001da60: 7275 650a 0a0a 2020 5f77 7269 7465 5f65  rue...  _write_e
+0001da70: 6d70 7479 5f6c 6973 745f 666f 725f 6479  mpty_list_for_dy
+0001da80: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
+0001da90: 203d 204e 6f6e 650a 0a20 2064 6566 205f   = None..  def _
+0001daa0: 7365 745f 6174 7472 6962 7574 6573 2873  set_attributes(s
+0001dab0: 656c 662c 206b 7764 7329 3a0a 2020 2020  elf, kwds):.    
+0001dac0: 666f 7220 6e61 6d65 2c20 7661 6c75 6520  for name, value 
+0001dad0: 696e 2073 6978 2e69 7465 7269 7465 6d73  in six.iteritems
+0001dae0: 286b 7764 7329 3a0a 2020 2020 2020 7365  (kwds):.      se
+0001daf0: 7461 7474 7228 7365 6c66 2c20 6e61 6d65  tattr(self, name
+0001db00: 2c20 7661 6c75 6529 0a0a 2020 4063 6c61  , value)..  @cla
+0001db10: 7373 6d65 7468 6f64 0a20 2064 6566 205f  ssmethod.  def _
+0001db20: 756e 6b6e 6f77 6e5f 7072 6f70 6572 7479  unknown_property
+0001db30: 2863 6c73 2c20 6e61 6d65 293a 0a0a 2020  (cls, name):..  
+0001db40: 2020 7061 7373 0a0a 2020 6465 6620 5f5f    pass..  def __
+0001db50: 6765 7461 7474 725f 5f28 7365 6c66 2c20  getattr__(self, 
+0001db60: 6e61 6d65 293a 0a20 2020 2069 6620 6e61  name):.    if na
+0001db70: 6d65 2e73 7461 7274 7377 6974 6828 275f  me.startswith('_
+0001db80: 2729 3a0a 2020 2020 2020 7265 7475 726e  '):.      return
+0001db90: 2073 7570 6572 2845 7870 616e 646f 2c20   super(Expando, 
+0001dba0: 7365 6c66 292e 5f5f 6765 7461 7474 725f  self).__getattr_
+0001dbb0: 5f28 6e61 6d65 290a 2020 2020 7072 6f70  _(name).    prop
+0001dbc0: 203d 2073 656c 662e 5f70 726f 7065 7274   = self._propert
+0001dbd0: 6965 732e 6765 7428 7369 782e 656e 7375  ies.get(six.ensu
+0001dbe0: 7265 5f74 6578 7428 6e61 6d65 2929 0a20  re_text(name)). 
+0001dbf0: 2020 2069 6620 7072 6f70 2069 7320 4e6f     if prop is No
+0001dc00: 6e65 3a0a 2020 2020 2020 7265 7475 726e  ne:.      return
+0001dc10: 2073 7570 6572 2845 7870 616e 646f 2c20   super(Expando, 
+0001dc20: 7365 6c66 292e 5f5f 6765 7461 7474 7269  self).__getattri
+0001dc30: 6275 7465 5f5f 286e 616d 6529 0a20 2020  bute__(name).   
+0001dc40: 2072 6574 7572 6e20 7072 6f70 2e5f 6765   return prop._ge
+0001dc50: 745f 7661 6c75 6528 7365 6c66 290a 0a20  t_value(self).. 
+0001dc60: 2064 6566 205f 5f73 6574 6174 7472 5f5f   def __setattr__
+0001dc70: 2873 656c 662c 206e 616d 652c 2076 616c  (self, name, val
+0001dc80: 7565 293a 0a20 2020 2069 6620 286e 616d  ue):.    if (nam
+0001dc90: 652e 7374 6172 7473 7769 7468 2827 5f27  e.startswith('_'
+0001dca0: 2920 6f72 0a20 2020 2020 2020 2069 7369  ) or.        isi
+0001dcb0: 6e73 7461 6e63 6528 6765 7461 7474 7228  nstance(getattr(
+0001dcc0: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 2c20  self.__class__, 
+0001dcd0: 6e61 6d65 2c20 4e6f 6e65 292c 2028 5072  name, None), (Pr
+0001dce0: 6f70 6572 7479 2c20 7072 6f70 6572 7479  operty, property
+0001dcf0: 2929 293a 0a20 2020 2020 2072 6574 7572  ))):.      retur
+0001dd00: 6e20 7375 7065 7228 4578 7061 6e64 6f2c  n super(Expando,
+0001dd10: 2073 656c 6629 2e5f 5f73 6574 6174 7472   self).__setattr
+0001dd20: 5f5f 286e 616d 652c 2076 616c 7565 290a  __(name, value).
+0001dd30: 0a20 2020 2073 656c 662e 5f63 6c6f 6e65  .    self._clone
+0001dd40: 5f70 726f 7065 7274 6965 7328 290a 2020  _properties().  
+0001dd50: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0001dd60: 7661 6c75 652c 204d 6f64 656c 293a 0a20  value, Model):. 
+0001dd70: 2020 2020 2070 726f 7020 3d20 5374 7275       prop = Stru
+0001dd80: 6374 7572 6564 5072 6f70 6572 7479 284d  cturedProperty(M
+0001dd90: 6f64 656c 2c20 6e61 6d65 290a 2020 2020  odel, name).    
+0001dda0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+0001ddb0: 7661 6c75 652c 2064 6963 7429 3a0a 2020  value, dict):.  
+0001ddc0: 2020 2020 7072 6f70 203d 2053 7472 7563      prop = Struc
+0001ddd0: 7475 7265 6450 726f 7065 7274 7928 4578  turedProperty(Ex
+0001dde0: 7061 6e64 6f2c 206e 616d 6529 0a20 2020  pando, name).   
+0001ddf0: 2065 6c73 653a 0a0a 2020 2020 2020 7072   else:..      pr
+0001de00: 6f70 203d 2047 656e 6572 6963 5072 6f70  op = GenericProp
+0001de10: 6572 7479 280a 2020 2020 2020 2020 2020  erty(.          
+0001de20: 6e61 6d65 2c20 7265 7065 6174 6564 3d69  name, repeated=i
+0001de30: 7369 6e73 7461 6e63 6528 7661 6c75 652c  sinstance(value,
+0001de40: 206c 6973 7429 2c0a 2020 2020 2020 2020   list),.        
+0001de50: 2020 696e 6465 7865 643d 7365 6c66 2e5f    indexed=self._
+0001de60: 6465 6661 756c 745f 696e 6465 7865 642c  default_indexed,
+0001de70: 0a20 2020 2020 2020 2020 2077 7269 7465  .          write
+0001de80: 5f65 6d70 7479 5f6c 6973 743d 7365 6c66  _empty_list=self
+0001de90: 2e5f 7772 6974 655f 656d 7074 795f 6c69  ._write_empty_li
+0001dea0: 7374 5f66 6f72 5f64 796e 616d 6963 5f70  st_for_dynamic_p
+0001deb0: 726f 7065 7274 6965 7329 0a20 2020 2070  roperties).    p
+0001dec0: 726f 702e 5f63 6f64 655f 6e61 6d65 203d  rop._code_name =
+0001ded0: 206e 616d 650a 2020 2020 7365 6c66 2e5f   name.    self._
+0001dee0: 7072 6f70 6572 7469 6573 5b73 6978 2e65  properties[six.e
+0001def0: 6e73 7572 655f 7465 7874 286e 616d 6529  nsure_text(name)
+0001df00: 5d20 3d20 7072 6f70 0a20 2020 2070 726f  ] = prop.    pro
+0001df10: 702e 5f73 6574 5f76 616c 7565 2873 656c  p._set_value(sel
+0001df20: 662c 2076 616c 7565 290a 0a20 2064 6566  f, value)..  def
+0001df30: 205f 5f64 656c 6174 7472 5f5f 2873 656c   __delattr__(sel
+0001df40: 662c 206e 616d 6529 3a0a 2020 2020 6966  f, name):.    if
+0001df50: 2028 6e61 6d65 2e73 7461 7274 7377 6974   (name.startswit
+0001df60: 6828 275f 2729 206f 720a 2020 2020 2020  h('_') or.      
+0001df70: 2020 6973 696e 7374 616e 6365 2867 6574    isinstance(get
+0001df80: 6174 7472 2873 656c 662e 5f5f 636c 6173  attr(self.__clas
+0001df90: 735f 5f2c 206e 616d 652c 204e 6f6e 6529  s__, name, None)
+0001dfa0: 2c20 2850 726f 7065 7274 792c 2070 726f  , (Property, pro
+0001dfb0: 7065 7274 7929 2929 3a0a 2020 2020 2020  perty))):.      
+0001dfc0: 7265 7475 726e 2073 7570 6572 2845 7870  return super(Exp
+0001dfd0: 616e 646f 2c20 7365 6c66 292e 5f5f 6465  ando, self).__de
+0001dfe0: 6c61 7474 725f 5f28 6e61 6d65 290a 2020  lattr__(name).  
+0001dff0: 2020 7072 6f70 5f6e 616d 6520 3d20 7369    prop_name = si
+0001e000: 782e 656e 7375 7265 5f74 6578 7428 6e61  x.ensure_text(na
+0001e010: 6d65 290a 2020 2020 7072 6f70 203d 2073  me).    prop = s
+0001e020: 656c 662e 5f70 726f 7065 7274 6965 732e  elf._properties.
+0001e030: 6765 7428 7072 6f70 5f6e 616d 6529 0a20  get(prop_name). 
+0001e040: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+0001e050: 616e 6365 2870 726f 702c 2050 726f 7065  ance(prop, Prope
+0001e060: 7274 7929 3a0a 2020 2020 2020 7261 6973  rty):.      rais
+0001e070: 6520 5479 7065 4572 726f 7228 274d 6f64  e TypeError('Mod
+0001e080: 656c 2070 726f 7065 7274 6965 7320 6d75  el properties mu
+0001e090: 7374 2062 6520 5072 6f70 6572 7479 2069  st be Property i
+0001e0a0: 6e73 7461 6e63 6573 3b20 6e6f 7420 2572  nstances; not %r
+0001e0b0: 2720 250a 2020 2020 2020 2020 2020 2020  ' %.            
+0001e0c0: 2020 2020 2020 2020 2020 7072 6f70 290a            prop).
+0001e0d0: 2020 2020 7072 6f70 2e5f 6465 6c65 7465      prop._delete
+0001e0e0: 5f76 616c 7565 2873 656c 6629 0a20 2020  _value(self).   
+0001e0f0: 2069 6620 7072 6f70 5f6e 616d 6520 696e   if prop_name in
+0001e100: 2073 656c 662e 5f5f 636c 6173 735f 5f2e   self.__class__.
+0001e110: 5f70 726f 7065 7274 6965 733a 0a20 2020  _properties:.   
+0001e120: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
+0001e130: 4572 726f 7228 2750 726f 7065 7274 7920  Error('Property 
+0001e140: 2573 2073 7469 6c6c 2069 6e20 7468 6520  %s still in the 
+0001e150: 6c69 7374 206f 6620 7072 6f70 6572 7469  list of properti
+0001e160: 6573 2066 6f72 2074 6865 2027 0a20 2020  es for the '.   
+0001e170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e180: 2020 2020 2020 2762 6173 6520 636c 6173        'base clas
+0001e190: 732e 2720 2520 6e61 6d65 290a 2020 2020  s.' % name).    
+0001e1a0: 6465 6c20 7365 6c66 2e5f 7072 6f70 6572  del self._proper
+0001e1b0: 7469 6573 5b70 726f 705f 6e61 6d65 5d0a  ties[prop_name].
+0001e1c0: 0a0a 4075 7469 6c73 2e70 6f73 6974 696f  ..@utils.positio
+0001e1d0: 6e61 6c28 3129 0a64 6566 2074 7261 6e73  nal(1).def trans
+0001e1e0: 6163 7469 6f6e 2863 616c 6c62 6163 6b2c  action(callback,
+0001e1f0: 202a 2a63 7478 5f6f 7074 696f 6e73 293a   **ctx_options):
+0001e200: 0a20 2022 2222 5275 6e20 6120 6361 6c6c  .  """Run a call
+0001e210: 6261 636b 2069 6e20 6120 7472 616e 7361  back in a transa
+0001e220: 6374 696f 6e2e 0a0a 2020 4172 6773 3a0a  ction...  Args:.
+0001e230: 2020 2020 6361 6c6c 6261 636b 3a20 4120      callback: A 
+0001e240: 6675 6e63 7469 6f6e 206f 7220 7461 736b  function or task
+0001e250: 6c65 7420 746f 2062 6520 6361 6c6c 6564  let to be called
+0001e260: 2e0a 2020 2020 2a2a 6374 785f 6f70 7469  ..    **ctx_opti
+0001e270: 6f6e 733a 2054 7261 6e73 6163 7469 6f6e  ons: Transaction
+0001e280: 206f 7074 696f 6e73 2e0a 0a20 2055 7365   options...  Use
+0001e290: 6675 6c20 6f70 7469 6f6e 7320 696e 636c  ful options incl
+0001e2a0: 7564 653a 0a20 2020 2072 6574 7269 6573  ude:.    retries
+0001e2b0: 3d4e 3a20 5265 7472 7920 7570 2074 6f20  =N: Retry up to 
+0001e2c0: 4e20 7469 6d65 7320 2869 2e65 2e20 7472  N times (i.e. tr
+0001e2d0: 7920 7570 2074 6f20 4e2b 3120 7469 6d65  y up to N+1 time
+0001e2e0: 7329 0a20 2020 2070 726f 7061 6761 7469  s).    propagati
+0001e2f0: 6f6e 3d3c 666c 6167 3e3a 2044 6574 6572  on=<flag>: Deter
+0001e300: 6d69 6e65 7320 686f 7720 616e 2065 7869  mines how an exi
+0001e310: 7374 696e 6720 7472 616e 7361 6374 696f  sting transactio
+0001e320: 6e20 7368 6f75 6c64 2062 650a 2020 2020  n should be.    
+0001e330: 2020 7072 6f70 6167 6174 6564 2c20 7768    propagated, wh
+0001e340: 6572 6520 3c66 6c61 673e 2063 616e 2062  ere <flag> can b
+0001e350: 6520 6f6e 6520 6f66 2074 6865 2066 6f6c  e one of the fol
+0001e360: 6c6f 7769 6e67 3a0a 2020 2020 2020 5472  lowing:.      Tr
+0001e370: 616e 7361 6374 696f 6e4f 7074 696f 6e73  ansactionOptions
+0001e380: 2e4e 4553 5445 443a 2053 7461 7274 2061  .NESTED: Start a
+0001e390: 206e 6573 7465 6420 7472 616e 7361 6374   nested transact
+0001e3a0: 696f 6e20 2874 6869 7320 6973 2074 6865  ion (this is the
+0001e3b0: 0a20 2020 2020 2020 2064 6566 6175 6c74  .        default
+0001e3c0: 3b20 6275 7420 6163 7475 616c 206e 6573  ; but actual nes
+0001e3d0: 7465 6420 7472 616e 7361 6374 696f 6e73  ted transactions
+0001e3e0: 2061 7265 206e 6f74 2079 6574 2069 6d70   are not yet imp
+0001e3f0: 6c65 6d65 6e74 6564 2c0a 2020 2020 2020  lemented,.      
+0001e400: 2020 736f 2065 6666 6563 7469 7665 6c79    so effectively
+0001e410: 2079 6f75 2063 616e 206f 6e6c 7920 7573   you can only us
+0001e420: 6520 7468 6973 206f 7574 7369 6465 2061  e this outside a
+0001e430: 6e20 6578 6973 7469 6e67 2074 7261 6e73  n existing trans
+0001e440: 6163 7469 6f6e 292e 0a20 2020 2020 2054  action)..      T
+0001e450: 7261 6e73 6163 7469 6f6e 4f70 7469 6f6e  ransactionOption
+0001e460: 732e 4d41 4e44 4154 4f52 593a 2041 2074  s.MANDATORY: A t
+0001e470: 7261 6e73 6163 7469 6f6e 206d 7573 7420  ransaction must 
+0001e480: 616c 7265 6164 7920 6265 2069 6e20 7072  already be in pr
+0001e490: 6f67 7265 7373 2e0a 2020 2020 2020 5472  ogress..      Tr
+0001e4a0: 616e 7361 6374 696f 6e4f 7074 696f 6e73  ansactionOptions
+0001e4b0: 2e41 4c4c 4f57 4544 3a20 4966 2061 2074  .ALLOWED: If a t
+0001e4c0: 7261 6e73 6163 7469 6f6e 2069 7320 696e  ransaction is in
+0001e4d0: 2070 726f 6772 6573 732c 206a 6f69 6e20   progress, join 
+0001e4e0: 6974 2e0a 2020 2020 2020 5472 616e 7361  it..      Transa
+0001e4f0: 6374 696f 6e4f 7074 696f 6e73 2e49 4e44  ctionOptions.IND
+0001e500: 4550 454e 4445 4e54 3a20 416c 7761 7973  EPENDENT: Always
+0001e510: 2073 7461 7274 2061 206e 6577 2070 6172   start a new par
+0001e520: 616c 6c65 6c20 7472 616e 7361 6374 696f  allel transactio
+0001e530: 6e2e 0a20 2020 2078 673d 5472 7565 3a20  n..    xg=True: 
+0001e540: 4f6e 2074 6865 2048 6967 6820 5265 706c  On the High Repl
+0001e550: 6963 6174 696f 6e20 4461 7461 7374 6f72  ication Datastor
+0001e560: 652c 2065 6e61 626c 6520 6372 6f73 732d  e, enable cross-
+0001e570: 6772 6f75 700a 2020 2020 2020 7472 616e  group.      tran
+0001e580: 7361 6374 696f 6e73 2c20 692e 652e 2061  sactions, i.e. a
+0001e590: 6c6c 6f77 2077 7269 7469 6e67 2074 6f20  llow writing to 
+0001e5a0: 7570 2074 6f20 3520 656e 7469 7479 2067  up to 5 entity g
+0001e5b0: 726f 7570 732e 0a20 2020 2072 6561 645f  roups..    read_
+0001e5c0: 6f6e 6c79 3d54 7275 653a 2049 6e64 6963  only=True: Indic
+0001e5d0: 6174 6573 2061 2074 7261 6e73 6163 7469  ates a transacti
+0001e5e0: 6f6e 2077 696c 6c20 6e6f 7420 646f 2061  on will not do a
+0001e5f0: 6e79 2077 7269 7465 732c 2077 6869 6368  ny writes, which
+0001e600: 0a20 2020 2020 2070 6f74 656e 7469 616c  .      potential
+0001e610: 6c79 2061 6c6c 6f77 7320 666f 7220 6d6f  ly allows for mo
+0001e620: 7265 2074 6872 6f75 6768 7075 742e 0a0a  re throughput...
+0001e630: 2020 5741 524e 494e 473a 2055 7369 6e67    WARNING: Using
+0001e640: 2061 6e79 7468 696e 6720 6f74 6865 7220   anything other 
+0001e650: 7468 616e 204e 4553 5445 4420 666f 7220  than NESTED for 
+0001e660: 7468 6520 7072 6f70 6167 6174 696f 6e20  the propagation 
+0001e670: 666c 6167 0a20 2063 616e 2068 6176 6520  flag.  can have 
+0001e680: 7374 7261 6e67 6520 636f 6e73 6571 7565  strange conseque
+0001e690: 6e63 6573 2e20 2057 6865 6e20 7573 696e  nces.  When usin
+0001e6a0: 6720 414c 4c4f 5745 4420 6f72 204d 414e  g ALLOWED or MAN
+0001e6b0: 4441 544f 5259 2c20 6966 0a20 2061 6e20  DATORY, if.  an 
+0001e6c0: 6578 6365 7074 696f 6e20 6973 2072 6169  exception is rai
+0001e6d0: 7365 642c 2074 6865 2074 7261 6e73 6163  sed, the transac
+0001e6e0: 7469 6f6e 2069 7320 6c69 6b65 6c79 206e  tion is likely n
+0001e6f0: 6f74 2073 6166 6520 746f 0a20 2063 6f6d  ot safe to.  com
+0001e700: 6d69 742e 2020 5768 656e 2075 7369 6e67  mit.  When using
+0001e710: 2049 4e44 4550 454e 4445 4e54 2069 7420   INDEPENDENT it 
+0001e720: 6973 206e 6f74 2067 656e 6572 616c 6c79  is not generally
+0001e730: 2073 6166 6520 746f 2072 6574 7572 6e0a   safe to return.
+0001e740: 2020 7661 6c75 6573 2072 6561 6420 746f    values read to
+0001e750: 2074 6865 2063 616c 6c65 7220 2861 7320   the caller (as 
+0001e760: 7468 6579 2077 6572 6520 6e6f 7420 7265  they were not re
+0001e770: 6164 2069 6e20 7468 6520 6361 6c6c 6572  ad in the caller
+0001e780: 2773 0a20 2074 7261 6e73 6163 7469 6f6e  's.  transaction
+0001e790: 292e 0a0a 2020 5265 7475 726e 733a 0a20  )...  Returns:. 
+0001e7a0: 2020 2057 6861 7465 7665 7220 6361 6c6c     Whatever call
+0001e7b0: 6261 636b 2829 2072 6574 7572 6e73 2e0a  back() returns..
+0001e7c0: 0a20 2052 6169 7365 733a 0a20 2020 2057  .  Raises:.    W
+0001e7d0: 6861 7465 7665 7220 6361 6c6c 6261 636b  hatever callback
+0001e7e0: 2829 2072 6169 7365 733b 2064 6174 6173  () raises; datas
+0001e7f0: 746f 7265 5f65 7272 6f72 732e 5472 616e  tore_errors.Tran
+0001e800: 7361 6374 696f 6e46 6169 6c65 6445 7272  sactionFailedErr
+0001e810: 6f72 0a20 2020 2069 6620 7468 6520 7472  or.    if the tr
+0001e820: 616e 7361 6374 696f 6e20 6661 696c 6564  ansaction failed
+0001e830: 2e0a 0a20 204e 6f74 653a 0a20 2020 2054  ...  Note:.    T
+0001e840: 6f20 7061 7373 2061 7267 756d 656e 7473  o pass arguments
+0001e850: 2074 6f20 6120 6361 6c6c 6261 636b 2066   to a callback f
+0001e860: 756e 6374 696f 6e2c 2075 7365 2061 206c  unction, use a l
+0001e870: 616d 6264 612c 2065 2e67 2e0a 2020 2020  ambda, e.g..    
+0001e880: 2020 6465 6620 6d79 5f63 616c 6c62 6163    def my_callbac
+0001e890: 6b28 6b65 792c 2069 6e63 293a 0a20 2020  k(key, inc):.   
+0001e8a0: 2020 2020 202e 2e2e 0a20 2020 2020 2074       ....      t
+0001e8b0: 7261 6e73 6163 7469 6f6e 286c 616d 6264  ransaction(lambd
+0001e8c0: 613a 206d 795f 6361 6c6c 6261 636b 284b  a: my_callback(K
+0001e8d0: 6579 282e 2e2e 292c 2031 2929 0a20 2022  ey(...), 1)).  "
+0001e8e0: 2222 0a20 2066 7574 203d 2074 7261 6e73  "".  fut = trans
+0001e8f0: 6163 7469 6f6e 5f61 7379 6e63 2863 616c  action_async(cal
+0001e900: 6c62 6163 6b2c 202a 2a63 7478 5f6f 7074  lback, **ctx_opt
+0001e910: 696f 6e73 290a 2020 7265 7475 726e 2066  ions).  return f
+0001e920: 7574 2e67 6574 5f72 6573 756c 7428 290a  ut.get_result().
+0001e930: 0a0a 4075 7469 6c73 2e70 6f73 6974 696f  ..@utils.positio
+0001e940: 6e61 6c28 3129 0a64 6566 2074 7261 6e73  nal(1).def trans
+0001e950: 6163 7469 6f6e 5f61 7379 6e63 2863 616c  action_async(cal
+0001e960: 6c62 6163 6b2c 202a 2a63 7478 5f6f 7074  lback, **ctx_opt
+0001e970: 696f 6e73 293a 0a20 2022 2222 5275 6e20  ions):.  """Run 
+0001e980: 6120 6361 6c6c 6261 636b 2069 6e20 6120  a callback in a 
+0001e990: 7472 616e 7361 6374 696f 6e2e 0a0a 2020  transaction...  
+0001e9a0: 5468 6973 2069 7320 7468 6520 6173 796e  This is the asyn
+0001e9b0: 6368 726f 6e6f 7573 2076 6572 7369 6f6e  chronous version
+0001e9c0: 206f 6620 7472 616e 7361 6374 696f 6e28   of transaction(
+0001e9d0: 292e 0a20 2022 2222 0a20 2066 726f 6d20  )..  """.  from 
+0001e9e0: 676f 6f67 6c65 2e61 7070 656e 6769 6e65  google.appengine
+0001e9f0: 2e65 7874 2e6e 6462 2069 6d70 6f72 7420  .ext.ndb import 
+0001ea00: 7461 736b 6c65 7473 0a20 2072 6574 7572  tasklets.  retur
+0001ea10: 6e20 7461 736b 6c65 7473 2e67 6574 5f63  n tasklets.get_c
+0001ea20: 6f6e 7465 7874 2829 2e74 7261 6e73 6163  ontext().transac
+0001ea30: 7469 6f6e 2863 616c 6c62 6163 6b2c 202a  tion(callback, *
+0001ea40: 2a63 7478 5f6f 7074 696f 6e73 290a 0a0a  *ctx_options)...
+0001ea50: 6465 6620 696e 5f74 7261 6e73 6163 7469  def in_transacti
+0001ea60: 6f6e 2829 3a0a 2020 2222 2252 6574 7572  on():.  """Retur
+0001ea70: 6e20 7768 6574 6865 7220 6120 7472 616e  n whether a tran
+0001ea80: 7361 6374 696f 6e20 6973 2063 7572 7265  saction is curre
+0001ea90: 6e74 6c79 2061 6374 6976 652e 2222 220a  ntly active.""".
+0001eaa0: 2020 6672 6f6d 2067 6f6f 676c 652e 6170    from google.ap
+0001eab0: 7065 6e67 696e 652e 6578 742e 6e64 6220  pengine.ext.ndb 
+0001eac0: 696d 706f 7274 2074 6173 6b6c 6574 730a  import tasklets.
+0001ead0: 2020 7265 7475 726e 2074 6173 6b6c 6574    return tasklet
+0001eae0: 732e 6765 745f 636f 6e74 6578 7428 292e  s.get_context().
+0001eaf0: 696e 5f74 7261 6e73 6163 7469 6f6e 2829  in_transaction()
+0001eb00: 0a0a 0a40 7574 696c 732e 6465 636f 7261  ...@utils.decora
+0001eb10: 746f 720a 6465 6620 7472 616e 7361 6374  tor.def transact
+0001eb20: 696f 6e61 6c28 6675 6e63 2c20 6172 6773  ional(func, args
+0001eb30: 2c20 6b77 6473 2c20 2a2a 6f70 7469 6f6e  , kwds, **option
+0001eb40: 7329 3a0a 2020 2222 2244 6563 6f72 6174  s):.  """Decorat
+0001eb50: 6f72 2074 6f20 6d61 6b65 2061 2066 756e  or to make a fun
+0001eb60: 6374 696f 6e20 6175 746f 6d61 7469 6361  ction automatica
+0001eb70: 6c6c 7920 7275 6e20 696e 2061 2074 7261  lly run in a tra
+0001eb80: 6e73 6163 7469 6f6e 2e0a 0a20 2041 7267  nsaction...  Arg
+0001eb90: 733a 0a20 2020 202a 2a63 7478 5f6f 7074  s:.    **ctx_opt
+0001eba0: 696f 6e73 3a20 5472 616e 7361 6374 696f  ions: Transactio
+0001ebb0: 6e20 6f70 7469 6f6e 7320 2873 6565 2074  n options (see t
+0001ebc0: 7261 6e73 6163 7469 6f6e 2829 2c20 6275  ransaction(), bu
+0001ebd0: 7420 7072 6f70 6167 6174 696f 6e0a 2020  t propagation.  
+0001ebe0: 2020 2020 6465 6661 756c 7420 746f 2054      default to T
+0001ebf0: 7261 6e73 6163 7469 6f6e 4f70 7469 6f6e  ransactionOption
+0001ec00: 732e 414c 4c4f 5745 4429 2e0a 0a20 2054  s.ALLOWED)...  T
+0001ec10: 6869 7320 7375 7070 6f72 7473 2074 776f  his supports two
+0001ec20: 2066 6f72 6d73 3a0a 0a20 2028 3129 2056   forms:..  (1) V
+0001ec30: 616e 696c 6c61 3a0a 2020 2020 2020 4074  anilla:.      @t
+0001ec40: 7261 6e73 6163 7469 6f6e 616c 0a20 2020  ransactional.   
+0001ec50: 2020 2064 6566 2063 616c 6c62 6163 6b28     def callback(
+0001ec60: 6172 6729 3a0a 2020 2020 2020 2020 2e2e  arg):.        ..
+0001ec70: 2e0a 0a20 2028 3229 2057 6974 6820 6f70  ...  (2) With op
+0001ec80: 7469 6f6e 733a 0a20 2020 2020 2040 7472  tions:.      @tr
+0001ec90: 616e 7361 6374 696f 6e61 6c28 7265 7472  ansactional(retr
+0001eca0: 6965 733d 3129 0a20 2020 2020 2064 6566  ies=1).      def
+0001ecb0: 2063 616c 6c62 6163 6b28 6172 6729 3a0a   callback(arg):.
+0001ecc0: 2020 2020 2020 2020 2e2e 2e0a 2020 2222          ....  ""
+0001ecd0: 220a 2020 7265 7475 726e 2074 7261 6e73  ".  return trans
+0001ece0: 6163 7469 6f6e 616c 5f61 7379 6e63 2e77  actional_async.w
+0001ecf0: 7261 7070 6564 5f64 6563 6f72 6174 6f72  rapped_decorator
+0001ed00: 280a 2020 2020 2020 6675 6e63 2c20 6172  (.      func, ar
+0001ed10: 6773 2c20 6b77 6473 2c20 2a2a 6f70 7469  gs, kwds, **opti
+0001ed20: 6f6e 7329 2e67 6574 5f72 6573 756c 7428  ons).get_result(
+0001ed30: 290a 0a0a 4075 7469 6c73 2e64 6563 6f72  )...@utils.decor
+0001ed40: 6174 6f72 0a64 6566 2074 7261 6e73 6163  ator.def transac
+0001ed50: 7469 6f6e 616c 5f61 7379 6e63 2866 756e  tional_async(fun
+0001ed60: 632c 2061 7267 732c 206b 7764 732c 202a  c, args, kwds, *
+0001ed70: 2a6f 7074 696f 6e73 293a 0a20 2022 2222  *options):.  """
+0001ed80: 5468 6520 6173 796e 6320 7665 7273 696f  The async versio
+0001ed90: 6e20 6f66 2040 6e64 622e 7472 616e 7361  n of @ndb.transa
+0001eda0: 6374 696f 6e2e 2222 220a 2020 6f70 7469  ction.""".  opti
+0001edb0: 6f6e 732e 7365 7464 6566 6175 6c74 2827  ons.setdefault('
+0001edc0: 7072 6f70 6167 6174 696f 6e27 2c20 6461  propagation', da
+0001edd0: 7461 7374 6f72 655f 7270 632e 5472 616e  tastore_rpc.Tran
+0001ede0: 7361 6374 696f 6e4f 7074 696f 6e73 2e41  sactionOptions.A
+0001edf0: 4c4c 4f57 4544 290a 2020 6966 2061 7267  LLOWED).  if arg
+0001ee00: 7320 6f72 206b 7764 733a 0a20 2020 2072  s or kwds:.    r
+0001ee10: 6574 7572 6e20 7472 616e 7361 6374 696f  eturn transactio
+0001ee20: 6e5f 6173 796e 6328 6c61 6d62 6461 3a20  n_async(lambda: 
+0001ee30: 6675 6e63 282a 6172 6773 2c20 2a2a 6b77  func(*args, **kw
+0001ee40: 6473 292c 202a 2a6f 7074 696f 6e73 290a  ds), **options).
+0001ee50: 2020 7265 7475 726e 2074 7261 6e73 6163    return transac
+0001ee60: 7469 6f6e 5f61 7379 6e63 2866 756e 632c  tion_async(func,
+0001ee70: 202a 2a6f 7074 696f 6e73 290a 0a0a 4075   **options)...@u
+0001ee80: 7469 6c73 2e64 6563 6f72 6174 6f72 0a64  tils.decorator.d
+0001ee90: 6566 2074 7261 6e73 6163 7469 6f6e 616c  ef transactional
+0001eea0: 5f74 6173 6b6c 6574 2866 756e 632c 2061  _tasklet(func, a
+0001eeb0: 7267 732c 206b 7764 732c 202a 2a6f 7074  rgs, kwds, **opt
+0001eec0: 696f 6e73 293a 0a20 2022 2222 5468 6520  ions):.  """The 
+0001eed0: 6173 796e 6320 7665 7273 696f 6e20 6f66  async version of
+0001eee0: 2040 6e64 622e 7472 616e 7361 6374 696f   @ndb.transactio
+0001eef0: 6e2e 0a0a 2020 5769 6c6c 2072 6574 7572  n...  Will retur
+0001ef00: 6e20 7468 6520 7265 7375 6c74 206f 6620  n the result of 
+0001ef10: 7468 6520 7772 6170 7065 6420 6675 6e63  the wrapped func
+0001ef20: 7469 6f6e 2061 7320 6120 4675 7475 7265  tion as a Future
+0001ef30: 2e0a 2020 2222 220a 2020 6672 6f6d 2067  ..  """.  from g
+0001ef40: 6f6f 676c 652e 6170 7065 6e67 696e 652e  oogle.appengine.
+0001ef50: 6578 742e 6e64 6220 696d 706f 7274 2074  ext.ndb import t
+0001ef60: 6173 6b6c 6574 730a 2020 6675 6e63 203d  asklets.  func =
+0001ef70: 2074 6173 6b6c 6574 732e 7461 736b 6c65   tasklets.taskle
+0001ef80: 7428 6675 6e63 290a 2020 7265 7475 726e  t(func).  return
+0001ef90: 2074 7261 6e73 6163 7469 6f6e 616c 5f61   transactional_a
+0001efa0: 7379 6e63 2e77 7261 7070 6564 5f64 6563  sync.wrapped_dec
+0001efb0: 6f72 6174 6f72 2866 756e 632c 2061 7267  orator(func, arg
+0001efc0: 732c 206b 7764 732c 202a 2a6f 7074 696f  s, kwds, **optio
+0001efd0: 6e73 290a 0a0a 4075 7469 6c73 2e64 6563  ns)...@utils.dec
+0001efe0: 6f72 6174 6f72 0a64 6566 206e 6f6e 5f74  orator.def non_t
+0001eff0: 7261 6e73 6163 7469 6f6e 616c 2866 756e  ransactional(fun
+0001f000: 632c 2061 7267 732c 206b 7764 732c 2061  c, args, kwds, a
+0001f010: 6c6c 6f77 5f65 7869 7374 696e 673d 5472  llow_existing=Tr
+0001f020: 7565 293a 0a20 2022 2222 4120 6465 636f  ue):.  """A deco
+0001f030: 7261 746f 7220 7468 6174 2065 6e73 7572  rator that ensur
+0001f040: 6573 2061 2066 756e 6374 696f 6e20 6973  es a function is
+0001f050: 2072 756e 206f 7574 7369 6465 2061 2074   run outside a t
+0001f060: 7261 6e73 6163 7469 6f6e 2e0a 0a20 2049  ransaction...  I
+0001f070: 6620 7468 6572 6520 6973 2061 6e20 6578  f there is an ex
+0001f080: 6973 7469 6e67 2074 7261 6e73 6163 7469  isting transacti
+0001f090: 6f6e 2028 616e 6420 616c 6c6f 775f 6578  on (and allow_ex
+0001f0a0: 6973 7469 6e67 3d54 7275 6529 2c20 7468  isting=True), th
+0001f0b0: 650a 2020 6578 6973 7469 6e67 2074 7261  e.  existing tra
+0001f0c0: 6e73 6163 7469 6f6e 2069 7320 7061 7573  nsaction is paus
+0001f0d0: 6564 2077 6869 6c65 2074 6865 2066 756e  ed while the fun
+0001f0e0: 6374 696f 6e20 6973 2065 7865 6375 7465  ction is execute
+0001f0f0: 642e 0a0a 2020 4172 6773 3a0a 2020 2020  d...  Args:.    
+0001f100: 616c 6c6f 775f 6578 6973 7469 6e67 3a20  allow_existing: 
+0001f110: 4966 2066 616c 7365 2c20 7468 726f 7720  If false, throw 
+0001f120: 616e 2065 7863 6570 7469 6f6e 2069 6620  an exception if 
+0001f130: 6361 6c6c 6564 2066 726f 6d20 7769 7468  called from with
+0001f140: 696e 0a20 2020 2020 2061 2074 7261 6e73  in.      a trans
+0001f150: 6163 7469 6f6e 2e20 2049 6620 7472 7565  action.  If true
+0001f160: 2c20 7465 6d70 6f72 6172 696c 7920 7265  , temporarily re
+0001f170: 2d65 7374 6162 6c69 7368 2074 6865 0a20  -establish the. 
+0001f180: 2020 2020 2070 7265 7669 6f75 7320 6e6f       previous no
+0001f190: 6e2d 7472 616e 7361 6374 696f 6e61 6c20  n-transactional 
+0001f1a0: 636f 6e74 6578 742e 2020 4465 6661 756c  context.  Defaul
+0001f1b0: 7473 2074 6f20 5472 7565 2e0a 0a20 2054  ts to True...  T
+0001f1c0: 6869 7320 7375 7070 6f72 7473 2074 776f  his supports two
+0001f1d0: 2066 6f72 6d73 2c20 7369 6d69 6c61 7220   forms, similar 
+0001f1e0: 746f 2074 7261 6e73 6163 7469 6f6e 616c  to transactional
+0001f1f0: 2829 2e0a 0a20 2052 6574 7572 6e73 3a0a  ()...  Returns:.
+0001f200: 2020 2020 4120 7772 6170 7065 7220 666f      A wrapper fo
+0001f210: 7220 7468 6520 6465 636f 7261 7465 6420  r the decorated 
+0001f220: 6675 6e63 7469 6f6e 2074 6861 7420 656e  function that en
+0001f230: 7375 7265 7320 6974 2072 756e 7320 6f75  sures it runs ou
+0001f240: 7473 6964 6520 610a 2020 2020 7472 616e  tside a.    tran
+0001f250: 7361 6374 696f 6e2e 0a20 2022 2222 0a20  saction..  """. 
+0001f260: 2066 726f 6d20 676f 6f67 6c65 2e61 7070   from google.app
+0001f270: 656e 6769 6e65 2e65 7874 2e6e 6462 2069  engine.ext.ndb i
+0001f280: 6d70 6f72 7420 7461 736b 6c65 7473 0a20  mport tasklets. 
+0001f290: 2063 7478 203d 2074 6173 6b6c 6574 732e   ctx = tasklets.
+0001f2a0: 6765 745f 636f 6e74 6578 7428 290a 2020  get_context().  
+0001f2b0: 6966 206e 6f74 2063 7478 2e69 6e5f 7472  if not ctx.in_tr
+0001f2c0: 616e 7361 6374 696f 6e28 293a 0a20 2020  ansaction():.   
+0001f2d0: 2072 6574 7572 6e20 6675 6e63 282a 6172   return func(*ar
+0001f2e0: 6773 2c20 2a2a 6b77 6473 290a 2020 6966  gs, **kwds).  if
+0001f2f0: 206e 6f74 2061 6c6c 6f77 5f65 7869 7374   not allow_exist
+0001f300: 696e 673a 0a20 2020 2072 6169 7365 2064  ing:.    raise d
+0001f310: 6174 6173 746f 7265 5f65 7272 6f72 732e  atastore_errors.
+0001f320: 4261 6452 6571 7565 7374 4572 726f 7228  BadRequestError(
+0001f330: 0a20 2020 2020 2020 2027 2573 2063 616e  .        '%s can
+0001f340: 6e6f 7420 6265 2063 616c 6c65 6420 7769  not be called wi
+0001f350: 7468 696e 2061 2074 7261 6e73 6163 7469  thin a transacti
+0001f360: 6f6e 2e27 2025 2066 756e 632e 5f5f 6e61  on.' % func.__na
+0001f370: 6d65 5f5f 290a 2020 7361 7665 5f63 7478  me__).  save_ctx
+0001f380: 203d 2063 7478 0a20 2077 6869 6c65 2063   = ctx.  while c
+0001f390: 7478 2e69 6e5f 7472 616e 7361 6374 696f  tx.in_transactio
+0001f3a0: 6e28 293a 0a20 2020 2063 7478 203d 2063  n():.    ctx = c
+0001f3b0: 7478 2e5f 7061 7265 6e74 5f63 6f6e 7465  tx._parent_conte
+0001f3c0: 7874 0a20 2020 2069 6620 6374 7820 6973  xt.    if ctx is
+0001f3d0: 204e 6f6e 653a 0a20 2020 2020 2072 6169   None:.      rai
+0001f3e0: 7365 2064 6174 6173 746f 7265 5f65 7272  se datastore_err
+0001f3f0: 6f72 732e 4261 6452 6571 7565 7374 4572  ors.BadRequestEr
+0001f400: 726f 7228 0a20 2020 2020 2020 2020 2027  ror(.          '
+0001f410: 436f 6e74 6578 7420 7769 7468 6f75 7420  Context without 
+0001f420: 6e6f 6e2d 7472 616e 7361 6374 696f 6e61  non-transactiona
+0001f430: 6c20 616e 6365 7374 6f72 2729 0a20 2073  l ancestor').  s
+0001f440: 6176 655f 6473 5f63 6f6e 6e20 3d20 6461  ave_ds_conn = da
+0001f450: 7461 7374 6f72 652e 5f47 6574 436f 6e6e  tastore._GetConn
+0001f460: 6563 7469 6f6e 2829 0a20 2074 7279 3a0a  ection().  try:.
+0001f470: 2020 2020 6966 2068 6173 6174 7472 2873      if hasattr(s
+0001f480: 6176 655f 6374 782c 2027 5f6f 6c64 5f64  ave_ctx, '_old_d
+0001f490: 735f 636f 6e6e 2729 3a0a 2020 2020 2020  s_conn'):.      
+0001f4a0: 6461 7461 7374 6f72 652e 5f53 6574 436f  datastore._SetCo
+0001f4b0: 6e6e 6563 7469 6f6e 2873 6176 655f 6374  nnection(save_ct
+0001f4c0: 782e 5f6f 6c64 5f64 735f 636f 6e6e 290a  x._old_ds_conn).
+0001f4d0: 2020 2020 7461 736b 6c65 7473 2e73 6574      tasklets.set
+0001f4e0: 5f63 6f6e 7465 7874 2863 7478 290a 2020  _context(ctx).  
+0001f4f0: 2020 7265 7475 726e 2066 756e 6328 2a61    return func(*a
+0001f500: 7267 732c 202a 2a6b 7764 7329 0a20 2066  rgs, **kwds).  f
+0001f510: 696e 616c 6c79 3a0a 2020 2020 7461 736b  inally:.    task
+0001f520: 6c65 7473 2e73 6574 5f63 6f6e 7465 7874  lets.set_context
+0001f530: 2873 6176 655f 6374 7829 0a20 2020 2064  (save_ctx).    d
+0001f540: 6174 6173 746f 7265 2e5f 5365 7443 6f6e  atastore._SetCon
+0001f550: 6e65 6374 696f 6e28 7361 7665 5f64 735f  nection(save_ds_
+0001f560: 636f 6e6e 290a 0a0a 6465 6620 6765 745f  conn)...def get_
+0001f570: 6d75 6c74 695f 6173 796e 6328 6b65 7973  multi_async(keys
+0001f580: 2c20 2a2a 6374 785f 6f70 7469 6f6e 7329  , **ctx_options)
+0001f590: 3a0a 2020 2222 2246 6574 6368 6573 2061  :.  """Fetches a
+0001f5a0: 2073 6571 7565 6e63 6520 6f66 206b 6579   sequence of key
+0001f5b0: 732e 0a0a 2020 4172 6773 3a0a 2020 2020  s...  Args:.    
+0001f5c0: 6b65 7973 3a20 4120 7365 7175 656e 6365  keys: A sequence
+0001f5d0: 206f 6620 6b65 7973 2e0a 2020 2020 2a2a   of keys..    **
+0001f5e0: 6374 785f 6f70 7469 6f6e 733a 2043 6f6e  ctx_options: Con
+0001f5f0: 7465 7874 206f 7074 696f 6e73 2e0a 0a20  text options... 
+0001f600: 2052 6574 7572 6e73 3a0a 2020 2020 4120   Returns:.    A 
+0001f610: 6c69 7374 206f 6620 6675 7475 7265 732e  list of futures.
+0001f620: 0a20 2022 2222 0a20 2072 6574 7572 6e20  .  """.  return 
+0001f630: 5b6b 6579 2e67 6574 5f61 7379 6e63 282a  [key.get_async(*
+0001f640: 2a63 7478 5f6f 7074 696f 6e73 2920 666f  *ctx_options) fo
+0001f650: 7220 6b65 7920 696e 206b 6579 735d 0a0a  r key in keys]..
+0001f660: 0a64 6566 2067 6574 5f6d 756c 7469 286b  .def get_multi(k
+0001f670: 6579 732c 202a 2a63 7478 5f6f 7074 696f  eys, **ctx_optio
+0001f680: 6e73 293a 0a20 2022 2222 4665 7463 6865  ns):.  """Fetche
+0001f690: 7320 6120 7365 7175 656e 6365 206f 6620  s a sequence of 
+0001f6a0: 6b65 7973 2e0a 0a20 2041 7267 733a 0a20  keys...  Args:. 
+0001f6b0: 2020 206b 6579 733a 2041 2073 6571 7565     keys: A seque
+0001f6c0: 6e63 6520 6f66 206b 6579 732e 0a20 2020  nce of keys..   
+0001f6d0: 202a 2a63 7478 5f6f 7074 696f 6e73 3a20   **ctx_options: 
+0001f6e0: 436f 6e74 6578 7420 6f70 7469 6f6e 732e  Context options.
+0001f6f0: 0a0a 2020 5265 7475 726e 733a 0a20 2020  ..  Returns:.   
+0001f700: 2041 206c 6973 7420 7768 6f73 6520 6974   A list whose it
+0001f710: 656d 7320 6172 6520 6569 7468 6572 2061  ems are either a
+0001f720: 204d 6f64 656c 2069 6e73 7461 6e63 6520   Model instance 
+0001f730: 6f72 204e 6f6e 6520 6966 2074 6865 206b  or None if the k
+0001f740: 6579 2077 6173 6e27 740a 2020 2020 666f  ey wasn't.    fo
+0001f750: 756e 642e 0a20 2022 2222 0a20 2072 6574  und..  """.  ret
+0001f760: 7572 6e20 5b66 7574 7572 652e 6765 745f  urn [future.get_
+0001f770: 7265 7375 6c74 2829 0a20 2020 2020 2020  result().       
+0001f780: 2020 2066 6f72 2066 7574 7572 6520 696e     for future in
+0001f790: 2067 6574 5f6d 756c 7469 5f61 7379 6e63   get_multi_async
+0001f7a0: 286b 6579 732c 202a 2a63 7478 5f6f 7074  (keys, **ctx_opt
+0001f7b0: 696f 6e73 295d 0a0a 0a64 6566 2070 7574  ions)]...def put
+0001f7c0: 5f6d 756c 7469 5f61 7379 6e63 2865 6e74  _multi_async(ent
+0001f7d0: 6974 6965 732c 202a 2a63 7478 5f6f 7074  ities, **ctx_opt
+0001f7e0: 696f 6e73 293a 0a20 2022 2222 5374 6f72  ions):.  """Stor
+0001f7f0: 6573 2061 2073 6571 7565 6e63 6520 6f66  es a sequence of
+0001f800: 204d 6f64 656c 2069 6e73 7461 6e63 6573   Model instances
+0001f810: 2e0a 0a20 2041 7267 733a 0a20 2020 2065  ...  Args:.    e
+0001f820: 6e74 6974 6965 733a 2041 2073 6571 7565  ntities: A seque
+0001f830: 6e63 6520 6f66 204d 6f64 656c 2069 6e73  nce of Model ins
+0001f840: 7461 6e63 6573 2e0a 2020 2020 2a2a 6374  tances..    **ct
+0001f850: 785f 6f70 7469 6f6e 733a 2043 6f6e 7465  x_options: Conte
+0001f860: 7874 206f 7074 696f 6e73 2e0a 0a20 2052  xt options...  R
+0001f870: 6574 7572 6e73 3a0a 2020 2020 4120 6c69  eturns:.    A li
+0001f880: 7374 206f 6620 6675 7475 7265 732e 0a20  st of futures.. 
+0001f890: 2022 2222 0a20 2072 6574 7572 6e20 5b65   """.  return [e
+0001f8a0: 6e74 6974 792e 7075 745f 6173 796e 6328  ntity.put_async(
+0001f8b0: 2a2a 6374 785f 6f70 7469 6f6e 7329 2066  **ctx_options) f
+0001f8c0: 6f72 2065 6e74 6974 7920 696e 2065 6e74  or entity in ent
+0001f8d0: 6974 6965 735d 0a0a 0a64 6566 2070 7574  ities]...def put
+0001f8e0: 5f6d 756c 7469 2865 6e74 6974 6965 732c  _multi(entities,
+0001f8f0: 202a 2a63 7478 5f6f 7074 696f 6e73 293a   **ctx_options):
+0001f900: 0a20 2022 2222 5374 6f72 6573 2061 2073  .  """Stores a s
+0001f910: 6571 7565 6e63 6520 6f66 204d 6f64 656c  equence of Model
+0001f920: 2069 6e73 7461 6e63 6573 2e0a 0a20 2041   instances...  A
+0001f930: 7267 733a 0a20 2020 2065 6e74 6974 6965  rgs:.    entitie
+0001f940: 733a 2041 2073 6571 7565 6e63 6520 6f66  s: A sequence of
+0001f950: 204d 6f64 656c 2069 6e73 7461 6e63 6573   Model instances
+0001f960: 2e0a 2020 2020 2a2a 6374 785f 6f70 7469  ..    **ctx_opti
+0001f970: 6f6e 733a 2043 6f6e 7465 7874 206f 7074  ons: Context opt
+0001f980: 696f 6e73 2e0a 0a20 2052 6574 7572 6e73  ions...  Returns
+0001f990: 3a0a 2020 2020 4120 6c69 7374 2077 6974  :.    A list wit
+0001f9a0: 6820 7468 6520 7374 6f72 6564 206b 6579  h the stored key
+0001f9b0: 732e 0a20 2022 2222 0a20 2072 6574 7572  s..  """.  retur
+0001f9c0: 6e20 5b66 7574 7572 652e 6765 745f 7265  n [future.get_re
+0001f9d0: 7375 6c74 2829 0a20 2020 2020 2020 2020  sult().         
+0001f9e0: 2066 6f72 2066 7574 7572 6520 696e 2070   for future in p
+0001f9f0: 7574 5f6d 756c 7469 5f61 7379 6e63 2865  ut_multi_async(e
+0001fa00: 6e74 6974 6965 732c 202a 2a63 7478 5f6f  ntities, **ctx_o
+0001fa10: 7074 696f 6e73 295d 0a0a 0a64 6566 2064  ptions)]...def d
+0001fa20: 656c 6574 655f 6d75 6c74 695f 6173 796e  elete_multi_asyn
+0001fa30: 6328 6b65 7973 2c20 2a2a 6374 785f 6f70  c(keys, **ctx_op
+0001fa40: 7469 6f6e 7329 3a0a 2020 2222 2244 656c  tions):.  """Del
+0001fa50: 6574 6573 2061 2073 6571 7565 6e63 6520  etes a sequence 
+0001fa60: 6f66 206b 6579 732e 0a0a 2020 4172 6773  of keys...  Args
+0001fa70: 3a0a 2020 2020 6b65 7973 3a20 4120 7365  :.    keys: A se
+0001fa80: 7175 656e 6365 206f 6620 6b65 7973 2e0a  quence of keys..
+0001fa90: 2020 2020 2a2a 6374 785f 6f70 7469 6f6e      **ctx_option
+0001faa0: 733a 2043 6f6e 7465 7874 206f 7074 696f  s: Context optio
+0001fab0: 6e73 2e0a 0a20 2052 6574 7572 6e73 3a0a  ns...  Returns:.
+0001fac0: 2020 2020 4120 6c69 7374 206f 6620 6675      A list of fu
+0001fad0: 7475 7265 732e 0a20 2022 2222 0a20 2072  tures..  """.  r
+0001fae0: 6574 7572 6e20 5b6b 6579 2e64 656c 6574  eturn [key.delet
+0001faf0: 655f 6173 796e 6328 2a2a 6374 785f 6f70  e_async(**ctx_op
+0001fb00: 7469 6f6e 7329 2066 6f72 206b 6579 2069  tions) for key i
+0001fb10: 6e20 6b65 7973 5d0a 0a0a 6465 6620 6465  n keys]...def de
+0001fb20: 6c65 7465 5f6d 756c 7469 286b 6579 732c  lete_multi(keys,
+0001fb30: 202a 2a63 7478 5f6f 7074 696f 6e73 293a   **ctx_options):
+0001fb40: 0a20 2022 2222 4465 6c65 7465 7320 6120  .  """Deletes a 
+0001fb50: 7365 7175 656e 6365 206f 6620 6b65 7973  sequence of keys
+0001fb60: 2e0a 0a20 2041 7267 733a 0a20 2020 206b  ...  Args:.    k
+0001fb70: 6579 733a 2041 2073 6571 7565 6e63 6520  eys: A sequence 
+0001fb80: 6f66 206b 6579 732e 0a20 2020 202a 2a63  of keys..    **c
+0001fb90: 7478 5f6f 7074 696f 6e73 3a20 436f 6e74  tx_options: Cont
+0001fba0: 6578 7420 6f70 7469 6f6e 732e 0a0a 2020  ext options...  
+0001fbb0: 5265 7475 726e 733a 0a20 2020 2041 206c  Returns:.    A l
+0001fbc0: 6973 7420 7768 6f73 6520 6974 656d 7320  ist whose items 
+0001fbd0: 6172 6520 616c 6c20 4e6f 6e65 2c20 6f6e  are all None, on
+0001fbe0: 6520 7065 7220 6465 6c65 7465 6420 6b65  e per deleted ke
+0001fbf0: 792e 0a20 2022 2222 0a20 2072 6574 7572  y..  """.  retur
+0001fc00: 6e20 5b66 7574 7572 652e 6765 745f 7265  n [future.get_re
+0001fc10: 7375 6c74 2829 0a20 2020 2020 2020 2020  sult().         
+0001fc20: 2066 6f72 2066 7574 7572 6520 696e 2064   for future in d
+0001fc30: 656c 6574 655f 6d75 6c74 695f 6173 796e  elete_multi_asyn
+0001fc40: 6328 6b65 7973 2c20 2a2a 6374 785f 6f70  c(keys, **ctx_op
+0001fc50: 7469 6f6e 7329 5d0a 0a0a 6465 6620 6765  tions)]...def ge
+0001fc60: 745f 696e 6465 7865 735f 6173 796e 6328  t_indexes_async(
+0001fc70: 2a2a 6374 785f 6f70 7469 6f6e 7329 3a0a  **ctx_options):.
+0001fc80: 2020 2222 2247 6574 2061 2064 6174 6120    """Get a data 
+0001fc90: 7374 7275 6374 7572 6520 7265 7072 6573  structure repres
+0001fca0: 656e 7469 6e67 2074 6865 2063 6f6e 6669  enting the confi
+0001fcb0: 6775 7265 6420 696e 6465 7865 732e 0a0a  gured indexes...
+0001fcc0: 2020 4172 6773 3a0a 2020 2020 2a2a 6374    Args:.    **ct
+0001fcd0: 785f 6f70 7469 6f6e 733a 2043 6f6e 7465  x_options: Conte
+0001fce0: 7874 206f 7074 696f 6e73 2e0a 0a20 2052  xt options...  R
+0001fcf0: 6574 7572 6e73 3a0a 2020 2020 4120 6675  eturns:.    A fu
+0001fd00: 7475 7265 2e0a 2020 2222 220a 2020 6672  ture..  """.  fr
+0001fd10: 6f6d 2067 6f6f 676c 652e 6170 7065 6e67  om google.appeng
+0001fd20: 696e 652e 6578 742e 6e64 6220 696d 706f  ine.ext.ndb impo
+0001fd30: 7274 2074 6173 6b6c 6574 730a 2020 6374  rt tasklets.  ct
+0001fd40: 7820 3d20 7461 736b 6c65 7473 2e67 6574  x = tasklets.get
+0001fd50: 5f63 6f6e 7465 7874 2829 0a20 2072 6574  _context().  ret
+0001fd60: 7572 6e20 6374 782e 6765 745f 696e 6465  urn ctx.get_inde
+0001fd70: 7865 7328 2a2a 6374 785f 6f70 7469 6f6e  xes(**ctx_option
+0001fd80: 7329 0a0a 0a64 6566 2067 6574 5f69 6e64  s)...def get_ind
+0001fd90: 6578 6573 282a 2a63 7478 5f6f 7074 696f  exes(**ctx_optio
+0001fda0: 6e73 293a 0a20 2022 2222 4765 7420 6120  ns):.  """Get a 
+0001fdb0: 6461 7461 2073 7472 7563 7475 7265 2072  data structure r
+0001fdc0: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+0001fdd0: 636f 6e66 6967 7572 6564 2069 6e64 6578  configured index
+0001fde0: 6573 2e0a 0a20 2041 7267 733a 0a20 2020  es...  Args:.   
+0001fdf0: 202a 2a63 7478 5f6f 7074 696f 6e73 3a20   **ctx_options: 
+0001fe00: 436f 6e74 6578 7420 6f70 7469 6f6e 732e  Context options.
+0001fe10: 0a0a 2020 5265 7475 726e 733a 0a20 2020  ..  Returns:.   
+0001fe20: 2041 206c 6973 7420 6f66 2049 6e64 6578   A list of Index
+0001fe30: 206f 626a 6563 7473 2e0a 2020 2222 220a   objects..  """.
+0001fe40: 2020 7265 7475 726e 2067 6574 5f69 6e64    return get_ind
+0001fe50: 6578 6573 5f61 7379 6e63 282a 2a63 7478  exes_async(**ctx
+0001fe60: 5f6f 7074 696f 6e73 292e 6765 745f 7265  _options).get_re
+0001fe70: 7375 6c74 2829 0a0a 0a0a 666f 7220 5f6e  sult()....for _n
+0001fe80: 616d 652c 205f 6f62 6a65 6374 2069 6e20  ame, _object in 
+0001fe90: 6c69 7374 2867 6c6f 6261 6c73 2829 2e69  list(globals().i
+0001fea0: 7465 6d73 2829 293a 0a20 2069 6620 2828  tems()):.  if ((
+0001feb0: 5f6e 616d 652e 656e 6473 7769 7468 2827  _name.endswith('
+0001fec0: 5072 6f70 6572 7479 2729 2061 6e64 2069  Property') and i
+0001fed0: 7373 7562 636c 6173 7328 5f6f 626a 6563  ssubclass(_objec
+0001fee0: 742c 2050 726f 7065 7274 7929 2920 6f72  t, Property)) or
+0001fef0: 0a20 2020 2020 2028 5f6e 616d 652e 656e  .      (_name.en
+0001ff00: 6473 7769 7468 2827 4572 726f 7227 2920  dswith('Error') 
+0001ff10: 616e 6420 6973 7375 6263 6c61 7373 285f  and issubclass(_
+0001ff20: 6f62 6a65 6374 2c20 4578 6365 7074 696f  object, Exceptio
+0001ff30: 6e29 2929 3a0a 2020 2020 5f5f 616c 6c5f  n))):.    __all_
+0001ff40: 5f2e 6170 7065 6e64 285f 6e61 6d65 290a  _.append(_name).
```

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/polymodel.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/polymodel.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/query.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/query.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/stats.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/stats.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/tasklets.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/tasklets.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/test_utils.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/test_utils.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/ndb/utils.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/utils.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/remote_api/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/remote_api/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/remote_api/remote_api_bytes_pb2.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/remote_api/remote_api_bytes_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/ext/testbed/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/ext/testbed/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/apiproxy.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/apiproxy.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/apiproxy_errors.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/apiproxy_errors.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/background.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/background.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/callback.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/callback.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/context/__init__.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/context/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/context/ctx_test_util.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/context/ctx_test_util.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/context/gae_headers.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/context/gae_headers.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/context/wsgi.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/context/wsgi.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/default_api_stub.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/default_api_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/initialize.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/initialize.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/middlewares.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/middlewares.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/request_environment.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/request_environment.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/runtime/thread_hooks.py` & `appengine-python-standard-1.1.2/src/google/appengine/runtime/thread_hooks.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/tools/app_engine_config_exception.py` & `appengine-python-standard-1.1.2/src/google/appengine/tools/app_engine_config_exception.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/tools/os_compat.py` & `appengine-python-standard-1.1.2/src/google/appengine/tools/os_compat.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/tools/queue_xml_parser.py` & `appengine-python-standard-1.1.2/src/google/appengine/tools/queue_xml_parser.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.1/src/google/appengine/tools/xml_parser_utils.py` & `appengine-python-standard-1.1.2/src/google/appengine/tools/xml_parser_utils.py`

 * *Files identical despite different names*

