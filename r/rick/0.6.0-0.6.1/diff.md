# Comparing `tmp/rick-0.6.0.tar.gz` & `tmp/rick-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rick-0.6.0.tar", last modified: Sun May 21 19:03:31 2023, max compression
+gzip compressed data, was "rick-0.6.1.tar", last modified: Wed May 31 15:46:44 2023, max compression
```

## Comparing `rick-0.6.0.tar` & `rick-0.6.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.392892 rick-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-21 19:03:17.000000 rick-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-21 19:03:31.392892 rick-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-21 19:03:17.000000 rick-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.380892 rick-0.6.0/rick/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-21 19:03:17.000000 rick-0.6.0/rick/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/base/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-21 19:03:17.000000 rick-0.6.0/rick/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-21 19:03:17.000000 rick-0.6.0/rick/base/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-21 19:03:17.000000 rick-0.6.0/rick/base/di.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-21 19:03:17.000000 rick-0.6.0/rick/base/maploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-21 19:03:17.000000 rick-0.6.0/rick/base/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-21 19:03:17.000000 rick-0.6.0/rick/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-21 19:03:17.000000 rick-0.6.0/rick/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-21 19:03:17.000000 rick-0.6.0/rick/crypto/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-21 19:03:17.000000 rick-0.6.0/rick/crypto/fernet256.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/crypto/hasher/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-21 19:03:17.000000 rick-0.6.0/rick/crypto/hasher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-21 19:03:17.000000 rick-0.6.0/rick/crypto/hasher/bcrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-21 19:03:17.000000 rick-0.6.0/rick/crypto/hasher/hasher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/event/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-21 19:03:17.000000 rick-0.6.0/rick/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-21 19:03:17.000000 rick-0.6.0/rick/event/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-21 19:03:17.000000 rick-0.6.0/rick/event/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/filter/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-21 19:03:17.000000 rick-0.6.0/rick/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-21 19:03:17.000000 rick-0.6.0/rick/filter/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/form/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-21 19:03:17.000000 rick-0.6.0/rick/form/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-21 19:03:17.000000 rick-0.6.0/rick/form/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-21 19:03:17.000000 rick-0.6.0/rick/form/form.py
--rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-05-21 19:03:17.000000 rick-0.6.0/rick/form/requestrecord.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-21 19:03:17.000000 rick-0.6.0/rick/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-21 19:03:17.000000 rick-0.6.0/rick/mixin/injectable.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 19:03:17.000000 rick-0.6.0/rick/mixin/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 19:03:17.000000 rick-0.6.0/rick/mixin/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/resource/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/resource/config/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/config/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/config/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/resource/console/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/console/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/console/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/resource/file/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/file/filereader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/resource/redis/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/resource/stream/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/stream/multipart_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/rick/serializer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/serializer/json/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:03:17.000000 rick-0.6.0/rick/serializer/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-21 19:03:17.000000 rick-0.6.0/rick/serializer/json/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/rick/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/object.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/rick/validator/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/rick/validator/rules/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.380892 rick-0.6.0/rick.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-21 19:03:31.000000 rick-0.6.0/rick.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-21 19:03:31.000000 rick-0.6.0/rick.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:03:31.000000 rick-0.6.0/rick.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:03:31.000000 rick-0.6.0/rick.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-21 19:03:31.000000 rick-0.6.0/rick.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 19:03:31.000000 rick-0.6.0/rick.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-21 19:03:31.392892 rick-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:03:17.000000 rick-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-21 19:03:17.000000 rick-0.6.0/tests/base/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-21 19:03:17.000000 rick-0.6.0/tests/base/test_di.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-21 19:03:17.000000 rick-0.6.0/tests/base/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/crypto/hasher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/crypto/hasher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-21 19:03:17.000000 rick-0.6.0/tests/crypto/hasher/test_bcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-21 19:03:17.000000 rick-0.6.0/tests/event/test_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-21 19:03:17.000000 rick-0.6.0/tests/filter/test_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/form/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/form/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-21 19:03:17.000000 rick-0.6.0/tests/form/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-21 19:03:17.000000 rick-0.6.0/tests/form/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-21 19:03:17.000000 rick-0.6.0/tests/form/test_requestrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-21 19:03:17.000000 rick-0.6.0/tests/form/test_requestrecord_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-21 19:03:17.000000 rick-0.6.0/tests/form/test_requestrecord_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/resource/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/config/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/config/test_environment_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/resource/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/file/test_filereader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/resource/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/stream/test_multipart_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-21 19:03:17.000000 rick-0.6.0/tests/util/test_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.392892 rick-0.6.0/tests/validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-21 19:03:17.000000 rick-0.6.0/tests/validator/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-21 19:03:17.000000 rick-0.6.0/tests/validator/test_validator_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.720203 rick-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-31 15:46:32.000000 rick-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-31 15:46:44.720203 rick-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-31 15:46:32.000000 rick-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.712203 rick-0.6.1/rick/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-31 15:46:32.000000 rick-0.6.1/rick/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.712203 rick-0.6.1/rick/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-31 15:46:32.000000 rick-0.6.1/rick/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-31 15:46:32.000000 rick-0.6.1/rick/base/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-31 15:46:32.000000 rick-0.6.1/rick/base/di.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-31 15:46:32.000000 rick-0.6.1/rick/base/maploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-31 15:46:32.000000 rick-0.6.1/rick/base/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-31 15:46:32.000000 rick-0.6.1/rick/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.712203 rick-0.6.1/rick/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-31 15:46:32.000000 rick-0.6.1/rick/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-31 15:46:32.000000 rick-0.6.1/rick/crypto/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-31 15:46:32.000000 rick-0.6.1/rick/crypto/fernet256.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.712203 rick-0.6.1/rick/crypto/hasher/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 15:46:32.000000 rick-0.6.1/rick/crypto/hasher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-31 15:46:32.000000 rick-0.6.1/rick/crypto/hasher/bcrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-31 15:46:32.000000 rick-0.6.1/rick/crypto/hasher/hasher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 15:46:32.000000 rick-0.6.1/rick/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-31 15:46:32.000000 rick-0.6.1/rick/event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-31 15:46:32.000000 rick-0.6.1/rick/event/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 15:46:32.000000 rick-0.6.1/rick/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-31 15:46:32.000000 rick-0.6.1/rick/filter/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/form/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-31 15:46:32.000000 rick-0.6.1/rick/form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-31 15:46:32.000000 rick-0.6.1/rick/form/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-31 15:46:32.000000 rick-0.6.1/rick/form/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-05-31 15:46:32.000000 rick-0.6.1/rick/form/requestrecord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-31 15:46:32.000000 rick-0.6.1/rick/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-31 15:46:32.000000 rick-0.6.1/rick/mixin/injectable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-31 15:46:32.000000 rick-0.6.1/rick/mixin/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-31 15:46:32.000000 rick-0.6.1/rick/mixin/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/resource/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/config/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/config/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/resource/console/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/console/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/console/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/resource/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/file/filereader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/resource/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/resource/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-31 15:46:32.000000 rick-0.6.1/rick/resource/stream/multipart_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/rick/serializer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/serializer/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:46:32.000000 rick-0.6.1/rick/serializer/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-31 15:46:32.000000 rick-0.6.1/rick/serializer/json/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/rick/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-31 15:46:32.000000 rick-0.6.1/rick/util/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-31 15:46:32.000000 rick-0.6.1/rick/util/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-31 15:46:32.000000 rick-0.6.1/rick/util/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-31 15:46:32.000000 rick-0.6.1/rick/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-31 15:46:32.000000 rick-0.6.1/rick/util/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-31 15:46:32.000000 rick-0.6.1/rick/util/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-31 15:46:32.000000 rick-0.6.1/rick/validator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/rick/validator/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-31 15:46:32.000000 rick-0.6.1/rick/validator/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-31 15:46:32.000000 rick-0.6.1/rick/validator/rules/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-31 15:46:32.000000 rick-0.6.1/rick/validator/rules/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-31 15:46:32.000000 rick-0.6.1/rick/validator/rules/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-31 15:46:32.000000 rick-0.6.1/rick/validator/rules/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-31 15:46:32.000000 rick-0.6.1/rick/validator/rules/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-31 15:46:32.000000 rick-0.6.1/rick/validator/rules/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-31 15:46:32.000000 rick-0.6.1/rick/validator/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.712203 rick-0.6.1/rick.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-31 15:46:44.000000 rick-0.6.1/rick.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-31 15:46:44.000000 rick-0.6.1/rick.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:46:44.000000 rick-0.6.1/rick.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:46:44.000000 rick-0.6.1/rick.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 15:46:44.000000 rick-0.6.1/rick.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 15:46:44.000000 rick-0.6.1/rick.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-31 15:46:44.720203 rick-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:46:32.000000 rick-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/tests/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-31 15:46:32.000000 rick-0.6.1/tests/base/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-31 15:46:32.000000 rick-0.6.1/tests/base/test_di.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-31 15:46:32.000000 rick-0.6.1/tests/base/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.716203 rick-0.6.1/tests/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.720203 rick-0.6.1/tests/crypto/hasher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/crypto/hasher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-31 15:46:32.000000 rick-0.6.1/tests/crypto/hasher/test_bcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.720203 rick-0.6.1/tests/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-31 15:46:32.000000 rick-0.6.1/tests/event/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.720203 rick-0.6.1/tests/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-31 15:46:32.000000 rick-0.6.1/tests/filter/test_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.720203 rick-0.6.1/tests/form/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-31 15:46:32.000000 rick-0.6.1/tests/form/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-31 15:46:32.000000 rick-0.6.1/tests/form/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-31 15:46:32.000000 rick-0.6.1/tests/form/test_requestrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-31 15:46:32.000000 rick-0.6.1/tests/form/test_requestrecord_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-31 15:46:32.000000 rick-0.6.1/tests/form/test_requestrecord_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.720203 rick-0.6.1/tests/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.720203 rick-0.6.1/tests/resource/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/resource/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-31 15:46:32.000000 rick-0.6.1/tests/resource/config/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-31 15:46:32.000000 rick-0.6.1/tests/resource/config/test_environment_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.720203 rick-0.6.1/tests/resource/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/resource/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-31 15:46:32.000000 rick-0.6.1/tests/resource/file/test_filereader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.720203 rick-0.6.1/tests/resource/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/resource/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-31 15:46:32.000000 rick-0.6.1/tests/resource/stream/test_multipart_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.720203 rick-0.6.1/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-31 15:46:32.000000 rick-0.6.1/tests/util/test_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:44.720203 rick-0.6.1/tests/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 rick-0.6.1/tests/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-31 15:46:32.000000 rick-0.6.1/tests/validator/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-31 15:46:32.000000 rick-0.6.1/tests/validator/test_validator_list.py
```

### Comparing `rick-0.6.0/LICENSE` & `rick-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/PKG-INFO` & `rick-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rick
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python plumbing for micro-framework based applications
 Home-page: https://git.oddbit.org/OddBit/rick
 Author: João Pinheiro
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.oddbit.org/rick/
 Project-URL: Source, https://git.oddbit.org/OddBit/rick
 Classifier: Environment :: Web Environment
@@ -21,18 +21,21 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Provides-Extra: redis
 License-File: LICENSE
 
 # rick
+
+
 [![Tests](https://github.com/oddbit-project/rick/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick/actions)
 [![pypi](https://img.shields.io/pypi/v/rick.svg)](https://pypi.org/project/rick/)
 [![license](https://img.shields.io/pypi/l/rick.svg)](https://git.oddbit.org/OddBit/rick/src/branch/master/LICENSE)
 
+
 Python plumbing for micro-framework based applications
 
 **Note**: This library is still under development; things may change place or be rewritten with a different spec between
 releases.
 
 
 ## Documentation
```

### Comparing `rick-0.6.0/README.md` & `rick-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # rick
+
+
 [![Tests](https://github.com/oddbit-project/rick/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick/actions)
 [![pypi](https://img.shields.io/pypi/v/rick.svg)](https://pypi.org/project/rick/)
 [![license](https://img.shields.io/pypi/l/rick.svg)](https://git.oddbit.org/OddBit/rick/src/branch/master/LICENSE)
 
+
 Python plumbing for micro-framework based applications
 
 **Note**: This library is still under development; things may change place or be rewritten with a different spec between
 releases.
 
 
 ## Documentation
```

### Comparing `rick-0.6.0/rick/base/container.py` & `rick-0.6.1/rick/base/container.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/base/di.py` & `rick-0.6.1/rick/base/di.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/base/maploader.py` & `rick-0.6.1/rick/base/maploader.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/base/registry.py` & `rick-0.6.1/rick/base/registry.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/crypto/buffer.py` & `rick-0.6.1/rick/crypto/buffer.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/crypto/fernet256.py` & `rick-0.6.1/rick/crypto/fernet256.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/crypto/hasher/bcrypt.py` & `rick-0.6.1/rick/crypto/hasher/bcrypt.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/event/manager.py` & `rick-0.6.1/rick/event/manager.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/filter/filter.py` & `rick-0.6.1/rick/filter/filter.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/form/field.py` & `rick-0.6.1/rick/form/field.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/form/form.py` & `rick-0.6.1/rick/form/form.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/form/requestrecord.py` & `rick-0.6.1/rick/form/requestrecord.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/resource/config/environment.py` & `rick-0.6.1/rick/resource/config/environment.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/resource/console/color.py` & `rick-0.6.1/rick/resource/console/color.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/resource/console/console.py` & `rick-0.6.1/rick/resource/console/console.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/resource/file/filereader.py` & `rick-0.6.1/rick/resource/file/filereader.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/resource/redis/redis.py` & `rick-0.6.1/rick/resource/redis/redis.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/resource/stream/multipart_reader.py` & `rick-0.6.1/rick/resource/stream/multipart_reader.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/serializer/json/json.py` & `rick-0.6.1/rick/serializer/json/json.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/util/loader.py` & `rick-0.6.1/rick/util/loader.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/util/object.py` & `rick-0.6.1/rick/util/object.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/validator/rules/hash.py` & `rick-0.6.1/rick/validator/rules/hash.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/validator/rules/misc.py` & `rick-0.6.1/rick/validator/rules/misc.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/validator/rules/net.py` & `rick-0.6.1/rick/validator/rules/net.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/validator/rules/numeric.py` & `rick-0.6.1/rick/validator/rules/numeric.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/validator/rules/rule.py` & `rick-0.6.1/rick/validator/rules/rule.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/validator/rules/strings.py` & `rick-0.6.1/rick/validator/rules/strings.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick/validator/validator.py` & `rick-0.6.1/rick/validator/validator.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/rick.egg-info/PKG-INFO` & `rick-0.6.1/rick.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rick
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python plumbing for micro-framework based applications
 Home-page: https://git.oddbit.org/OddBit/rick
 Author: João Pinheiro
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.oddbit.org/rick/
 Project-URL: Source, https://git.oddbit.org/OddBit/rick
 Classifier: Environment :: Web Environment
@@ -21,18 +21,21 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Provides-Extra: redis
 License-File: LICENSE
 
 # rick
+
+
 [![Tests](https://github.com/oddbit-project/rick/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick/actions)
 [![pypi](https://img.shields.io/pypi/v/rick.svg)](https://pypi.org/project/rick/)
 [![license](https://img.shields.io/pypi/l/rick.svg)](https://git.oddbit.org/OddBit/rick/src/branch/master/LICENSE)
 
+
 Python plumbing for micro-framework based applications
 
 **Note**: This library is still under development; things may change place or be rewritten with a different spec between
 releases.
 
 
 ## Documentation
```

### Comparing `rick-0.6.0/rick.egg-info/SOURCES.txt` & `rick-0.6.1/rick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/setup.cfg` & `rick-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/base/test_container.py` & `rick-0.6.1/tests/base/test_container.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/base/test_di.py` & `rick-0.6.1/tests/base/test_di.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/base/test_registry.py` & `rick-0.6.1/tests/base/test_registry.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/crypto/hasher/test_bcrypt.py` & `rick-0.6.1/tests/crypto/hasher/test_bcrypt.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/event/test_manager.py` & `rick-0.6.1/tests/event/test_manager.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/filter/test_filter.py` & `rick-0.6.1/tests/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/form/test_field.py` & `rick-0.6.1/tests/form/test_field.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/form/test_form.py` & `rick-0.6.1/tests/form/test_form.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/form/test_requestrecord.py` & `rick-0.6.1/tests/form/test_requestrecord.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/form/test_requestrecord_field.py` & `rick-0.6.1/tests/form/test_requestrecord_field.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/form/test_requestrecord_record.py` & `rick-0.6.1/tests/form/test_requestrecord_record.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/resource/config/test_environment.py` & `rick-0.6.1/tests/resource/config/test_environment.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/resource/config/test_environment_wrap.py` & `rick-0.6.1/tests/resource/config/test_environment_wrap.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/resource/file/test_filereader.py` & `rick-0.6.1/tests/resource/file/test_filereader.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/resource/stream/test_multipart_reader.py` & `rick-0.6.1/tests/resource/stream/test_multipart_reader.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/validator/test_validator.py` & `rick-0.6.1/tests/validator/test_validator.py`

 * *Files identical despite different names*

### Comparing `rick-0.6.0/tests/validator/test_validator_list.py` & `rick-0.6.1/tests/validator/test_validator_list.py`

 * *Files identical despite different names*

