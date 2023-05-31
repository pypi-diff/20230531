# Comparing `tmp/Pokie-0.4.2.tar.gz` & `tmp/Pokie-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pokie-0.4.2.tar", last modified: Mon May 29 17:00:53 2023, max compression
+gzip compressed data, was "Pokie-0.4.3.tar", last modified: Wed May 31 15:47:22 2023, max compression
```

## Comparing `Pokie-0.4.2.tar` & `Pokie-0.4.3.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-29 17:00:19.000000 Pokie-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-29 17:00:19.000000 Pokie-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-29 17:00:53.130009 Pokie-0.4.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/Pokie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-29 17:00:53.000000 Pokie-0.4.2/Pokie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-29 17:00:53.000000 Pokie-0.4.2/Pokie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:00:53.000000 Pokie-0.4.2/Pokie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:00:53.000000 Pokie-0.4.2/Pokie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 17:00:53.000000 Pokie-0.4.2/Pokie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 17:00:53.000000 Pokie-0.4.2/Pokie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-29 17:00:19.000000 Pokie-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/codegen/pg/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/pg/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/pg/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/pg/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/textfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/config/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/cli/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/dto/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/dto/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/dto/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/plugin/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/repository/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/repository/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/service/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/service/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/service/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/service/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/sql/001-auth-schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/view/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/db_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/tpl_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/dto/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/dto/records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/job/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/job/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/repository/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/repository/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/repository/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/repository/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/service/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/service/autorest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/service/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/service/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/service/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/sql/001-settings.sql
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/sql/002-fixtures.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/validators/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/validators/pk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/cli/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/dto/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/dto/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/job/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/job/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/repository/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/repository/repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/service/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/service/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/service/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/sql/001-mail.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/core/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/pokie/core/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/factories/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/factories/pgsql.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/factories/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/pokie/http/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/http/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/http/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/http/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/http/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/http/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/pokie/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/plugins/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/pokie/rest/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/rest/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/rest/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/pokie/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/util/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-29 17:00:53.130009 Pokie-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-29 17:00:19.000000 Pokie-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/tests/__init__.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.478436 Pokie-0.4.3/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1315 2023-05-22 13:10:12.000000 Pokie-0.4.3/LICENSE
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      125 2022-11-22 11:02:45.000000 Pokie-0.4.3/MANIFEST.in
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1865 2023-05-31 15:47:22.478436 Pokie-0.4.3/PKG-INFO
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.466436 Pokie-0.4.3/Pokie.egg-info/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1865 2023-05-31 15:47:22.000000 Pokie-0.4.3/Pokie.egg-info/PKG-INFO
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3406 2023-05-31 15:47:22.000000 Pokie-0.4.3/Pokie.egg-info/SOURCES.txt
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2023-05-31 15:47:22.000000 Pokie-0.4.3/Pokie.egg-info/dependency_links.txt
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2022-11-03 11:00:15.000000 Pokie-0.4.3/Pokie.egg-info/not-zip-safe
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      157 2023-05-31 15:47:22.000000 Pokie-0.4.3/Pokie.egg-info/requires.txt
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       12 2023-05-31 15:47:22.000000 Pokie-0.4.3/Pokie.egg-info/top_level.txt
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      619 2023-05-22 13:15:40.000000 Pokie-0.4.3/README.md
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.466436 Pokie-0.4.3/pokie/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       64 2022-11-03 10:59:50.000000 Pokie-0.4.3/pokie/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      116 2022-11-03 11:57:08.000000 Pokie-0.4.3/pokie/__main__.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/codegen/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-11-03 12:16:47.000000 Pokie-0.4.3/pokie/codegen/__init__.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/codegen/pg/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      104 2022-11-07 16:24:37.000000 Pokie-0.4.3/pokie/codegen/pg/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2044 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/codegen/pg/record.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4238 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/codegen/pg/request.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4111 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/codegen/pg/spec.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      405 2022-11-07 16:10:53.000000 Pokie-0.4.3/pokie/codegen/spec.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2585 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/codegen/template.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      590 2022-11-07 16:13:57.000000 Pokie-0.4.3/pokie/codegen/textfile.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/config/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-10-01 10:15:02.000000 Pokie-0.4.3/pokie/config/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1982 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/config/template.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1259 2023-05-31 15:18:34.000000 Pokie-0.4.3/pokie/constants.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-10-12 14:05:40.000000 Pokie-0.4.3/pokie/contrib/__init__.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-08-20 16:06:46.000000 Pokie-0.4.3/pokie/contrib/auth/__init__.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/cli/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      358 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/cli/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    11699 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/cli/acl.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    10570 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/cli/user.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       80 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/constants.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/dto/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       48 2022-10-13 10:50:07.000000 Pokie-0.4.3/pokie/contrib/auth/dto/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      654 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/dto/acl.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      410 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/dto/user.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1491 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/module.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/plugin/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       29 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/plugin/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2719 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/plugin/db.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/repository/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-08-20 16:09:00.000000 Pokie-0.4.3/pokie/contrib/auth/repository/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     8672 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/repository/acl.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      989 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/repository/user.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/service/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       88 2022-10-01 12:37:49.000000 Pokie-0.4.3/pokie/contrib/auth/service/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3396 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/service/acl.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2510 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/service/auth.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2998 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/service/user.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/sql/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1179 2023-05-30 08:22:14.000000 Pokie-0.4.3/pokie/contrib/auth/sql/001-auth-schema.sql
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/view/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-08-20 16:10:16.000000 Pokie-0.4.3/pokie/contrib/auth/view/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1660 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/view/account.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/base/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-10-01 14:59:52.000000 Pokie-0.4.3/pokie/contrib/base/__init__.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/base/cli/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      326 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5275 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/base.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     7245 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/db.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     6326 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/db_codegen.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3080 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/fixture.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2325 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/job.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      482 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/pytest.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1578 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/tpl_codegen.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      106 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/constants.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/base/dto/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       51 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/dto/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      329 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/dto/records.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/base/job/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       26 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/job/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      459 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/job/idle.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1776 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/module.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/base/repository/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       43 2022-10-12 13:28:57.000000 Pokie-0.4.3/pokie/contrib/base/repository/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      191 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/repository/fixture.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1985 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/repository/settings.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      807 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/repository/validator.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/base/service/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      128 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/service/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1025 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/service/autorest.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2098 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/service/fixture.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1125 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/service/settings.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2079 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/service/validator.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/base/sql/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      210 2022-11-02 00:49:04.000000 Pokie-0.4.3/pokie/contrib/base/sql/001-settings.sql
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      138 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/sql/002-fixtures.sql
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/base/validators/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       46 2022-10-12 13:46:20.000000 Pokie-0.4.3/pokie/contrib/base/validators/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1507 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/validators/pk.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/__init__.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/cli/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       46 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/cli/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1502 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/cli/queue.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       78 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/constants.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/dto/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       63 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/dto/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      728 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/dto/records.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1466 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/helpers.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/job/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       32 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/job/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2069 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/job/queue.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      661 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/module.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/repository/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       76 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/repository/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2823 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/repository/repositories.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/service/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       84 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/service/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1369 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/service/queue.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      939 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/service/template.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/sql/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      854 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/sql/001-mail.sql
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/core/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      139 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     7229 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/application.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      657 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/command.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/core/factories/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-10-01 12:07:49.000000 Pokie-0.4.3/pokie/core/factories/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      664 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/factories/login.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      887 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/factories/pgsql.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      848 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/factories/redis.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      475 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/module.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      813 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/signal.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/http/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       96 2022-11-22 11:02:45.000000 Pokie-0.4.3/pokie/http/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2045 2023-05-31 15:22:30.000000 Pokie-0.4.3/pokie/http/helpers.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      175 2022-10-31 14:57:32.000000 Pokie-0.4.3/pokie/http/response.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3129 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/http/rest.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2165 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/http/routes.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     9475 2023-05-29 17:32:51.000000 Pokie-0.4.3/pokie/http/view.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/plugins/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-10-14 15:27:51.000000 Pokie-0.4.3/pokie/plugins/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      731 2022-11-22 11:02:45.000000 Pokie-0.4.3/pokie/plugins/auth.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/rest/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       69 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/rest/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      652 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/rest/mixin.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2174 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/rest/service.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.478436 Pokie-0.4.3/pokie/util/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-10-01 18:39:00.000000 Pokie-0.4.3/pokie/util/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      775 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/util/cli_args.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1576 2023-05-31 15:47:22.478436 Pokie-0.4.3/setup.cfg
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       39 2022-11-03 10:58:29.000000 Pokie-0.4.3/setup.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.478436 Pokie-0.4.3/tests/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-11-22 11:02:45.000000 Pokie-0.4.3/tests/__init__.py
```

### Comparing `Pokie-0.4.2/LICENSE` & `Pokie-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/PKG-INFO` & `Pokie-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pokie
-Version: 0.4.2
+Version: 0.4.3
 Summary: A high-level Python REST web framework based on Flask, Rick and RickDb.
 Home-page: https://git.oddbit.org/OddBit/pokie
 Author: João Pinheiro
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.oddbit.org/pokie/
 Project-URL: Source, https://git.oddbit.org/OddBit/pokie
 Classifier: Environment :: Web Environment
```

### Comparing `Pokie-0.4.2/Pokie.egg-info/PKG-INFO` & `Pokie-0.4.3/Pokie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pokie
-Version: 0.4.2
+Version: 0.4.3
 Summary: A high-level Python REST web framework based on Flask, Rick and RickDb.
 Home-page: https://git.oddbit.org/OddBit/pokie
 Author: João Pinheiro
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.oddbit.org/pokie/
 Project-URL: Source, https://git.oddbit.org/OddBit/pokie
 Classifier: Environment :: Web Environment
```

### Comparing `Pokie-0.4.2/Pokie.egg-info/SOURCES.txt` & `Pokie-0.4.3/Pokie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/README.md` & `Pokie-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/codegen/pg/record.py` & `Pokie-0.4.3/pokie/codegen/pg/record.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/codegen/pg/request.py` & `Pokie-0.4.3/pokie/codegen/pg/request.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/codegen/pg/spec.py` & `Pokie-0.4.3/pokie/codegen/pg/spec.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/codegen/template.py` & `Pokie-0.4.3/pokie/codegen/template.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/codegen/textfile.py` & `Pokie-0.4.3/pokie/codegen/textfile.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/config/template.py` & `Pokie-0.4.3/pokie/config/template.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/constants.py` & `Pokie-0.4.3/pokie/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version
-POKIE_VERSION = ["0", "4", "2"]
+POKIE_VERSION = ["0", "4", "3"]
 
 
 def get_version():
     return ".".join(POKIE_VERSION)
 
 
 # Http Codes
```

### Comparing `Pokie-0.4.2/pokie/contrib/auth/cli/acl.py` & `Pokie-0.4.3/pokie/contrib/auth/cli/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/auth/cli/user.py` & `Pokie-0.4.3/pokie/contrib/auth/cli/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/auth/dto/acl.py` & `Pokie-0.4.3/pokie/contrib/auth/dto/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/auth/module.py` & `Pokie-0.4.3/pokie/contrib/auth/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/auth/plugin/db.py` & `Pokie-0.4.3/pokie/contrib/auth/plugin/db.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/auth/repository/acl.py` & `Pokie-0.4.3/pokie/contrib/auth/repository/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/auth/repository/user.py` & `Pokie-0.4.3/pokie/contrib/auth/repository/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/auth/service/acl.py` & `Pokie-0.4.3/pokie/contrib/auth/service/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/auth/service/auth.py` & `Pokie-0.4.3/pokie/contrib/auth/service/auth.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/auth/service/user.py` & `Pokie-0.4.3/pokie/contrib/auth/service/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/auth/sql/001-auth-schema.sql` & `Pokie-0.4.3/pokie/contrib/auth/sql/001-auth-schema.sql`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 CREATE TABLE "user"(
     id_user SERIAL NOT NULL PRIMARY KEY,
     active BOOL DEFAULT True,
     admin BOOL DEFAULT False,
     username VARCHAR(200) NOT NULL UNIQUE,
-    first_name VARCHAR(100),
-    last_name VARCHAR(100),
-    email VARCHAR(200),
+    first_name VARCHAR(100) DEFAULT '',
+    last_name VARCHAR(100) DEFAULT '',
+    email VARCHAR(200) DEFAULT '',
     password TEXT NOT NULL,
     creation_date timestamp with time zone default NOW(),
     last_login TIMESTAMP WITH TIME ZONE default NULL,
     external BOOL DEFAULT False,
     attributes JSONB DEFAULT '{}'
 );
```

### Comparing `Pokie-0.4.2/pokie/contrib/auth/view/account.py` & `Pokie-0.4.3/pokie/contrib/auth/view/account.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/cli/base.py` & `Pokie-0.4.3/pokie/contrib/base/cli/base.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/cli/db.py` & `Pokie-0.4.3/pokie/contrib/base/cli/db.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/cli/db_codegen.py` & `Pokie-0.4.3/pokie/contrib/base/cli/db_codegen.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/cli/fixture.py` & `Pokie-0.4.3/pokie/contrib/base/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/cli/job.py` & `Pokie-0.4.3/pokie/contrib/base/cli/job.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/cli/tpl_codegen.py` & `Pokie-0.4.3/pokie/contrib/base/cli/tpl_codegen.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/module.py` & `Pokie-0.4.3/pokie/contrib/base/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/repository/settings.py` & `Pokie-0.4.3/pokie/contrib/base/repository/settings.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/repository/validator.py` & `Pokie-0.4.3/pokie/contrib/base/repository/validator.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/service/autorest.py` & `Pokie-0.4.3/pokie/contrib/base/service/autorest.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/service/fixture.py` & `Pokie-0.4.3/pokie/contrib/base/service/fixture.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/service/settings.py` & `Pokie-0.4.3/pokie/contrib/base/service/settings.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/service/validator.py` & `Pokie-0.4.3/pokie/contrib/base/service/validator.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/base/validators/pk.py` & `Pokie-0.4.3/pokie/contrib/base/validators/pk.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/mail/cli/queue.py` & `Pokie-0.4.3/pokie/contrib/mail/cli/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/mail/dto/records.py` & `Pokie-0.4.3/pokie/contrib/mail/dto/records.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/mail/helpers.py` & `Pokie-0.4.3/pokie/contrib/mail/helpers.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/mail/job/queue.py` & `Pokie-0.4.3/pokie/contrib/mail/job/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/mail/module.py` & `Pokie-0.4.3/pokie/contrib/mail/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/mail/repository/repositories.py` & `Pokie-0.4.3/pokie/contrib/mail/repository/repositories.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/mail/service/queue.py` & `Pokie-0.4.3/pokie/contrib/mail/service/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/mail/service/template.py` & `Pokie-0.4.3/pokie/contrib/mail/service/template.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/contrib/mail/sql/001-mail.sql` & `Pokie-0.4.3/pokie/contrib/mail/sql/001-mail.sql`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/core/application.py` & `Pokie-0.4.3/pokie/core/application.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/core/command.py` & `Pokie-0.4.3/pokie/core/command.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/core/factories/login.py` & `Pokie-0.4.3/pokie/core/factories/login.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/core/factories/pgsql.py` & `Pokie-0.4.3/pokie/core/factories/pgsql.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/core/factories/redis.py` & `Pokie-0.4.3/pokie/core/factories/redis.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/core/signal.py` & `Pokie-0.4.3/pokie/core/signal.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/http/helpers.py` & `Pokie-0.4.3/pokie/http/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-from rick.util.misc import optional
-
-
 class ParseListError(Exception):
     pass
 
 
 def parse_list_parameters(args, record):
-    search_text = optional("search", args, None)
-    match_fields = optional("match", args, None)
-    offset = optional("offset", args, None)
-    limit = optional("limit", args, None)
-    sort = optional("sort", args, None)
+    search_text = args.get("search")
+    match_fields = args.get("match")
+    offset = args.get("offset")
+    limit = args.get("limit")
+    sort = args.get("sort")
 
     # match fields
     if match_fields is not None:
         match_fields = match_fields.split("|")
         # convert field names to column names
         result = {}
         for f in match_fields:
```

### Comparing `Pokie-0.4.2/pokie/http/rest.py` & `Pokie-0.4.3/pokie/http/rest.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/http/routes.py` & `Pokie-0.4.3/pokie/http/routes.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/http/view.py` & `Pokie-0.4.3/pokie/http/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     def exception_handler(self, e) -> ResponseReturnValue:
         """
         Generic exception handler for dispatch
         :param e:
         :return:
         """
         if e is not None:
-            logging.error(e)
+            logging.exception(e)
         if request.is_json:
             return self.error("bad request")
         return (
             "<!doctype html>\n<html lang=en>\n<title>{code} {err}</title>\n<h1>{err}</h1>\n".format(
                 code=HTTP_BADREQ, err="Bad Request"
             ),
             HTTP_BADREQ,
```

### Comparing `Pokie-0.4.2/pokie/plugins/auth.py` & `Pokie-0.4.3/pokie/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/rest/mixin.py` & `Pokie-0.4.3/pokie/rest/mixin.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/rest/service.py` & `Pokie-0.4.3/pokie/rest/service.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/pokie/util/cli_args.py` & `Pokie-0.4.3/pokie/util/cli_args.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.2/setup.cfg` & `Pokie-0.4.3/setup.cfg`

 * *Files identical despite different names*

