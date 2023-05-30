# Comparing `tmp/nsj_rest_lib-0.2.1.tar.gz` & `tmp/nsj_rest_lib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-0.2.1.tar", last modified: Mon May 29 16:56:00 2023, max compression
+gzip compressed data, was "nsj_rest_lib-1.0.0.tar", last modified: Tue May 30 22:02:00 2023, max compression
```

## Comparing `nsj_rest_lib-0.2.1.tar` & `nsj_rest_lib-1.0.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.339509 nsj_rest_lib-0.2.1/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-05-29 16:56:00.339509 nsj_rest_lib-0.2.1/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2022-09-08 22:15:46.000000 nsj_rest_lib-0.2.1/README.md
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-05-29 16:56:00.339509 nsj_rest_lib-0.2.1/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.331509 nsj_rest_lib-0.2.1/src/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.331509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.335509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-01-06 22:06:31.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3131 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3700 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4349 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3684 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4094 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.335509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/dao/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    16639 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2022-12-19 18:04:42.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.335509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3987 2023-03-20 12:54:19.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/decorator/dto.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.335509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9033 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-01-02 23:27:01.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      195 2022-12-27 22:14:24.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.335509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/dto/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7290 2023-04-18 17:42:31.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.335509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/entity/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      772 2023-04-18 17:42:31.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2022-12-27 22:14:24.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2022-11-30 20:09:08.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-01-05 22:38:04.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2022-12-19 17:39:11.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.339509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/service/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    23200 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      582 2023-04-18 17:42:31.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.339509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/validator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/validator/validate_data.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.331509 nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-05-29 16:56:00.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1609 2023-05-29 16:56:00.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-05-29 16:56:00.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-05-29 16:56:00.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-05-29 16:56:00.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.150052 nsj_rest_lib-1.0.0/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-05-30 22:02:00.150052 nsj_rest_lib-1.0.0/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2022-09-08 22:15:46.000000 nsj_rest_lib-1.0.0/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-05-30 22:02:00.150052 nsj_rest_lib-1.0.0/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.134053 nsj_rest_lib-1.0.0/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.142053 nsj_rest_lib-1.0.0/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.142053 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-01-06 22:06:31.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3131 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3700 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4349 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3684 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4094 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.142053 nsj_rest_lib-1.0.0/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    16608 2023-05-30 22:01:35.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2022-12-19 18:04:42.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.146052 nsj_rest_lib-1.0.0/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3987 2023-03-20 12:54:19.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/decorator/dto.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.146052 nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9038 2023-05-30 22:01:35.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-01-02 23:27:01.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      195 2022-12-27 22:14:24.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.146052 nsj_rest_lib-1.0.0/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7290 2023-04-18 17:42:31.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.146052 nsj_rest_lib-1.0.0/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-05-30 22:01:35.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2022-12-27 22:14:24.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2022-11-30 20:09:08.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-01-05 22:38:04.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2022-12-19 17:39:11.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.146052 nsj_rest_lib-1.0.0/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    23264 2023-05-30 22:01:35.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      582 2023-04-18 17:42:31.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.146052 nsj_rest_lib-1.0.0/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/validator/validate_data.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.142053 nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-05-30 22:02:00.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1609 2023-05-30 22:02:00.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-05-30 22:02:00.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-05-30 22:02:00.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-05-30 22:02:00.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-0.2.1/PKG-INFO` & `nsj_rest_lib-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_rest_lib
-Version: 0.2.1
+Version: 1.0.0
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-0.2.1/setup.cfg` & `nsj_rest_lib-1.0.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 0.2.1
+version = 1.0.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/list_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/post_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/put_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/dao/dao_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,37 +66,37 @@
         # Building SQL fields
         if fields is None:
             fields = [f"t0.{k}" for k in entity.__dict__ if not callable(
                 getattr(entity, k, None)) and not k.startswith('_')]
 
         return ', '.join(fields)
 
-    def get(self, id: uuid.UUID, fields: List[str] = None, partition_fields=None) -> EntityBase:
+    def get(self, id: uuid.UUID, fields: List[str] = None, filters=None) -> EntityBase:
         """
         Returns an entity instance by its ID.
         """
 
         # Creating a entity instance
         entity = self._entity_class()
 
+        # Organizando o where dos filtros
+        filters_where, filter_values_map = self._make_filters_sql(filters)
+
         # Building query
         sql = f"""
         select
             {self._sql_fields(fields)}
         from
             {entity.get_table_name()} as t0
         where
-            t0.{entity.get_pk_column_name()} = :id
+            t0.{entity.get_pk_field()} = :id
+            {filters_where}
         """
         values = {"id": id}
-
-        if partition_fields is not None:
-            for field in partition_fields:
-                sql += f" \n and t0.{field} = :{field}"
-                values[field] = partition_fields[field]
+        values.update(filter_values_map)
                 
         # Running query
         resp = self._db.execute_query_to_model(
             sql,
             self._entity_class,
             **values
         )
@@ -453,15 +453,15 @@
         if filters is None or len(filters) <= 0:
             return None
 
         # Montando uma entity fake
         entity = self._entity_class()
 
         # Recuperando o campo de chave primária
-        pk_field = entity.get_pk_column_name()
+        pk_field = entity.get_pk_field()
 
         # Organizando o where dos filtros
         filters_where, filter_values_map = self._make_filters_sql(filters)
 
         # Montando a query
         sql = f"""
         select {pk_field} from {entity.get_table_name()} as t0 where true {filters_where}
```

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/decorator/dto.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,43 +138,44 @@
         # Montando expressões regulares para as validações
         matcher_uuid = re.compile(
             '^[A-Fa-f0-9]{8}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{12}$')
         matcher_datetime = re.compile(
             '^(\d\d\d\d)-(\d\d)-(\d\d)[T,t](\d\d):(\d\d):(\d\d)$')
         matcher_date = re.compile('^(\d\d\d\d)-(\d\d)-(\d\d)$')
 
-        # Validação por regex
-        if (
-            self.expected_type is datetime.datetime
-            or self.expected_type is datetime.date
-        ) and isinstance(value, str):
-            # Verificando se pode ser alterado de str para UUID
+        # Validação direta de tipos
+        erro_tipo = False
+        if self.expected_type is datetime.datetime and isinstance(value, str):
             match_datetime = matcher_datetime.search(value)
-            match_date = matcher_date.search(value)
 
             if match_datetime:
                 ano = int(match_datetime.group(1))
                 mes = int(match_datetime.group(2))
                 dia = int(match_datetime.group(3))
                 hora = int(match_datetime.group(4))
                 minuto = int(match_datetime.group(5))
                 segundo = int(match_datetime.group(6))
 
                 value = datetime.datetime(
                     year=ano, month=mes, day=dia, hour=hora, minute=minuto, second=segundo)
-            elif match_date:
+            else:
+                erro_tipo=True
+        elif self.expected_type is datetime.date and isinstance(value, str):
+
+            match_date = matcher_date.search(value)
+
+            if match_date:
                 ano = int(match_date.group(1))
                 mes = int(match_date.group(2))
                 dia = int(match_date.group(3))
 
                 value = datetime.date(year=ano, month=mes, day=dia)
-
-        # Validação direta de tipos
-        erro_tipo = False
-        if isinstance(self.expected_type, enum.EnumMeta):
+            else:
+                erro_tipo=True
+        elif isinstance(self.expected_type, enum.EnumMeta):
             # Enumerados
             try:
                 value = self.expected_type(value)
             except ValueError as e:
                 raise ValueError(
                     f"{self.storage_name} não é um {self.expected_type.__name__} válido. Valor recebido: {value}.")
         elif self.expected_type is bool and isinstance(value, int):
@@ -211,21 +212,21 @@
             try:
                 value = float(value)
             except:
                 erro_tipo = True
         elif self.expected_type is Decimal:
             # Int
             try:
-                value = str(value)
+                value = Decimal(value)
             except:
                 erro_tipo = True
         elif self.expected_type is str:
             # Int
             try:
-                value = Decimal(value)
+                value = str(value)
             except:
                 erro_tipo = True
         else:
             erro_tipo = True
 
         if erro_tipo:
             raise ValueError(
```

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/dto/dto_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/entity/entity_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 class EntityBase(abc.ABC):
 
     
     def initialize_fields(self):
         for annotation in self.__annotations__:
             self.__setattr__(annotation, None)  
 
-    def get_pk_column_name(self) -> str:
-        return 'id'
-
     @abc.abstractmethod
     def get_table_name(self) -> str:
         pass
 
     @abc.abstractmethod
     def get_default_order_fields(self) -> List[str]:
         pass
```

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/service/service_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,18 @@
     ) -> DTOBase:
         # Resolving fields
         fields = self._resolving_fields(fields)
 
         # Handling the fields to retrieve
         entity_fields = self._convert_to_entity_fields(fields['root'])
 
+        entity_filters = self._create_entity_filters(partition_fields)
+
         # Recuperando a entity
-        entity = self._dao.get(id, entity_fields, partition_fields)
+        entity = self._dao.get(id, entity_fields, entity_filters)
 
         # Convertendo para DTO
         dto = self._dto_class(entity)
 
         # Tratando das propriedades de lista
         if len(self._dto_class.list_fields_map) > 0:
             self._retrieve_related_lists([dto], fields)
@@ -547,15 +549,15 @@
         
 
         if entity_pk_value is None:
             return False
 
         # Searching entity in DB
         try:
-            self._dao.get(entity_pk_value, [entity.get_pk_column_name(
+            self._dao.get(entity_pk_value, [entity.get_pk_field(
             )], partition_fields)
         except NotFoundException as e:
             return False
 
         return True
 
     def _delete(
```

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-rest-lib
-Version: 0.2.1
+Version: 1.0.0
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

