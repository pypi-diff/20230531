# Comparing `tmp/gyver-2.1.1.tar.gz` & `tmp/gyver-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver-2.1.1.tar", max compression
+gzip compressed data, was "gyver-2.1.2.tar", max compression
```

## Comparing `gyver-2.1.1.tar` & `gyver-2.1.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     1079 2023-03-29 07:24:24.843143 gyver-2.1.1/LICENSE
--rw-r--r--   0        0        0      993 2023-03-29 07:24:24.843143 gyver-2.1.1/README.md
--rw-r--r--   0        0        0      158 2023-05-13 16:49:41.026955 gyver-2.1.1/gyver/__init__.py
--rw-r--r--   0        0        0      359 2023-03-29 07:24:24.843143 gyver-2.1.1/gyver/cache/__init__.py
--rw-r--r--   0        0        0     1201 2023-04-14 08:44:43.823769 gyver-2.1.1/gyver/cache/asyncio.py
--rw-r--r--   0        0        0      237 2023-03-29 07:24:24.843143 gyver-2.1.1/gyver/cache/config.py
--rw-r--r--   0        0        0     1776 2023-03-29 07:24:24.843143 gyver-2.1.1/gyver/cache/interface.py
--rw-r--r--   0        0        0     1395 2023-03-29 07:24:24.843143 gyver-2.1.1/gyver/cache/mapper.py
--rw-r--r--   0        0        0     5993 2023-04-14 08:44:43.832774 gyver-2.1.1/gyver/cache/mock.py
--rw-r--r--   0        0        0     4283 2023-04-14 08:44:43.835775 gyver-2.1.1/gyver/cache/redis.py
--rw-r--r--   0        0        0     1128 2023-04-14 08:44:43.837776 gyver-2.1.1/gyver/cache/sync.py
--rw-r--r--   0        0        0      558 2023-03-29 07:33:58.431990 gyver-2.1.1/gyver/cache/utils.py
--rw-r--r--   0        0        0      498 2023-03-29 07:24:24.843143 gyver-2.1.1/gyver/config/__init__.py
--rw-r--r--   0        0        0       78 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/config/adapter/__init__.py
--rw-r--r--   0        0        0     1320 2023-04-14 08:44:43.858786 gyver-2.1.1/gyver/config/adapter/attrs.py
--rw-r--r--   0        0        0     1078 2023-04-14 08:44:43.860787 gyver-2.1.1/gyver/config/adapter/dataclass.py
--rw-r--r--   0        0        0     5886 2023-04-14 08:44:43.866790 gyver-2.1.1/gyver/config/adapter/factory.py
--rw-r--r--   0        0        0     1056 2023-04-14 08:44:43.871793 gyver-2.1.1/gyver/config/adapter/gattrs.py
--rw-r--r--   0        0        0     2107 2023-04-14 08:44:43.875795 gyver-2.1.1/gyver/config/adapter/interface.py
--rw-r--r--   0        0        0     1701 2023-04-14 08:44:43.878796 gyver-2.1.1/gyver/config/adapter/mark.py
--rw-r--r--   0        0        0     1091 2023-04-14 08:44:43.881798 gyver-2.1.1/gyver/config/adapter/pydantic.py
--rw-r--r--   0        0        0     3435 2023-04-14 08:44:43.847781 gyver-2.1.1/gyver/config/config.py
--rw-r--r--   0        0        0     2126 2023-04-14 08:44:43.849782 gyver-2.1.1/gyver/config/envconfig.py
--rw-r--r--   0        0        0      587 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/config/typedef.py
--rw-r--r--   0        0        0      473 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/config/utils.py
--rw-r--r--   0        0        0      419 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/context/__init__.py
--rw-r--r--   0        0        0      288 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/context/atomic_/__init__.py
--rw-r--r--   0        0        0     2317 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/context/atomic_/bound.py
--rw-r--r--   0        0        0     2493 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/context/atomic_/core.py
--rw-r--r--   0        0        0     1332 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/context/atomic_/resolver.py
--rw-r--r--   0        0        0     5659 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/context/context.py
--rw-r--r--   0        0        0      102 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/context/interfaces/__init__.py
--rw-r--r--   0        0        0     1525 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/context/interfaces/adapter.py
--rw-r--r--   0        0        0       39 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/context/typedef.py
--rw-r--r--   0        0        0      253 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/crypto/__init__.py
--rw-r--r--   0        0        0      133 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/crypto/config.py
--rw-r--r--   0        0        0      909 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/crypto/fernet.py
--rw-r--r--   0        0        0     1856 2023-04-14 08:44:43.914814 gyver-2.1.1/gyver/crypto/rsa.py
--rw-r--r--   0        0        0      749 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/database/__init__.py
--rw-r--r--   0        0        0     2136 2023-04-14 08:44:43.927820 gyver-2.1.1/gyver/database/adapter.py
--rw-r--r--   0        0        0     1233 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/database/config.py
--rw-r--r--   0        0        0      360 2023-03-29 07:24:24.844143 gyver-2.1.1/gyver/database/context/__init__.py
--rw-r--r--   0        0        0     3542 2023-04-14 08:44:42.980359 gyver-2.1.1/gyver/database/context/asyncio.py
--rw-r--r--   0        0        0     3349 2023-03-29 07:29:51.153084 gyver-2.1.1/gyver/database/context/sync.py
--rw-r--r--   0        0        0      170 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/database/drivers/__init__.py
--rw-r--r--   0        0        0      229 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/database/drivers/dialect.py
--rw-r--r--   0        0        0      224 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/database/drivers/interface.py
--rw-r--r--   0        0        0     1493 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/database/drivers/utils.py
--rw-r--r--   0        0        0     1076 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/database/entity.py
--rw-r--r--   0        0        0      498 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/database/entity.pyi
--rw-r--r--   0        0        0       50 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/database/metadata.py
--rw-r--r--   0        0        0     1012 2023-04-14 08:44:43.954833 gyver-2.1.1/gyver/database/query/__init__.py
--rw-r--r--   0        0        0     1692 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/database/query/_helpers.py
--rw-r--r--   0        0        0     2935 2023-04-14 08:44:43.960836 gyver-2.1.1/gyver/database/query/comp.py
--rw-r--r--   0        0        0      294 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/database/query/exc.py
--rw-r--r--   0        0        0     1353 2023-04-14 08:44:43.004370 gyver-2.1.1/gyver/database/query/interface.py
--rw-r--r--   0        0        0      279 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/database/query/null.py
--rw-r--r--   0        0        0     1270 2023-04-14 08:44:43.969841 gyver-2.1.1/gyver/database/query/order_by.py
--rw-r--r--   0        0        0     1239 2023-04-14 08:44:43.971842 gyver-2.1.1/gyver/database/query/paginate.py
--rw-r--r--   0        0        0      697 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/database/query/utils.py
--rw-r--r--   0        0        0     4613 2023-04-14 08:44:43.975844 gyver-2.1.1/gyver/database/query/where.py
--rw-r--r--   0        0        0      327 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/database/typedef.py
--rw-r--r--   0        0        0     4243 2023-04-14 08:44:43.080407 gyver-2.1.1/gyver/database/utils.py
--rw-r--r--   0        0        0     2030 2023-05-11 07:34:48.903992 gyver-2.1.1/gyver/exc.py
--rw-r--r--   0        0        0      857 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/model.py
--rw-r--r--   0        0        0      101 2023-05-08 11:52:12.095726 gyver-2.1.1/gyver/pools/__init__.py
--rw-r--r--   0        0        0     5764 2023-05-13 16:48:20.474968 gyver-2.1.1/gyver/pools/asyncio.py
--rw-r--r--   0        0        0     2225 2023-05-13 16:48:21.238958 gyver-2.1.1/gyver/pools/resource.py
--rw-r--r--   0        0        0     3855 2023-05-13 16:48:01.539206 gyver-2.1.1/gyver/pools/thread.py
--rw-r--r--   0        0        0        0 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/py.typed
--rw-r--r--   0        0        0      186 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/url/__init__.py
--rw-r--r--   0        0        0     3166 2023-05-13 16:48:22.167946 gyver-2.1.1/gyver/url/core.py
--rw-r--r--   0        0        0      423 2023-05-13 03:47:04.475970 gyver-2.1.1/gyver/url/encode.py
--rw-r--r--   0        0        0      664 2023-05-13 16:48:21.208958 gyver-2.1.1/gyver/url/fragment.py
--rw-r--r--   0        0        0     2834 2023-05-13 16:48:21.209958 gyver-2.1.1/gyver/url/netloc.py
--rw-r--r--   0        0        0     2795 2023-05-13 16:48:21.212958 gyver-2.1.1/gyver/url/path.py
--rw-r--r--   0        0        0     1711 2023-05-13 16:48:21.213958 gyver-2.1.1/gyver/url/query.py
--rw-r--r--   0        0        0      662 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/url/utils.py
--rw-r--r--   0        0        0      674 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/utils/__init__.py
--rw-r--r--   0        0        0      156 2023-03-29 07:24:24.845143 gyver-2.1.1/gyver/utils/exc.py
--rw-r--r--   0        0        0     7836 2023-04-14 08:44:44.001856 gyver-2.1.1/gyver/utils/finder.py
--rw-r--r--   0        0        0     1391 2023-04-14 08:44:44.003857 gyver-2.1.1/gyver/utils/helpers.py
--rw-r--r--   0        0        0      174 2023-03-29 07:24:24.846143 gyver-2.1.1/gyver/utils/json.py
--rw-r--r--   0        0        0     2610 2023-03-29 07:24:24.846143 gyver-2.1.1/gyver/utils/lazy.py
--rw-r--r--   0        0        0     1319 2023-04-14 08:44:44.010861 gyver-2.1.1/gyver/utils/singleton.py
--rw-r--r--   0        0        0     1718 2023-03-29 07:24:24.846143 gyver-2.1.1/gyver/utils/strings.py
--rw-r--r--   0        0        0      134 2023-03-29 07:24:24.846143 gyver-2.1.1/gyver/utils/timezone.py
--rw-r--r--   0        0        0     2418 2023-05-13 16:49:41.023955 gyver-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     2493 1970-01-01 00:00:00.000000 gyver-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-03-29 07:24:24.843143 gyver-2.1.2/LICENSE
+-rw-r--r--   0        0        0     1005 2023-05-13 16:51:07.121414 gyver-2.1.2/README.md
+-rw-r--r--   0        0        0      158 2023-05-31 11:18:06.211763 gyver-2.1.2/gyver/__init__.py
+-rw-r--r--   0        0        0      359 2023-03-29 07:24:24.843143 gyver-2.1.2/gyver/cache/__init__.py
+-rw-r--r--   0        0        0     1201 2023-04-14 08:44:43.823769 gyver-2.1.2/gyver/cache/asyncio.py
+-rw-r--r--   0        0        0      237 2023-03-29 07:24:24.843143 gyver-2.1.2/gyver/cache/config.py
+-rw-r--r--   0        0        0     1776 2023-03-29 07:24:24.843143 gyver-2.1.2/gyver/cache/interface.py
+-rw-r--r--   0        0        0     1395 2023-03-29 07:24:24.843143 gyver-2.1.2/gyver/cache/mapper.py
+-rw-r--r--   0        0        0     5993 2023-04-14 08:44:43.832774 gyver-2.1.2/gyver/cache/mock.py
+-rw-r--r--   0        0        0     4283 2023-04-14 08:44:43.835775 gyver-2.1.2/gyver/cache/redis.py
+-rw-r--r--   0        0        0     1128 2023-04-14 08:44:43.837776 gyver-2.1.2/gyver/cache/sync.py
+-rw-r--r--   0        0        0      558 2023-05-31 11:17:32.510186 gyver-2.1.2/gyver/cache/utils.py
+-rw-r--r--   0        0        0      498 2023-03-29 07:24:24.843143 gyver-2.1.2/gyver/config/__init__.py
+-rw-r--r--   0        0        0       78 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/config/adapter/__init__.py
+-rw-r--r--   0        0        0     1320 2023-04-14 08:44:43.858786 gyver-2.1.2/gyver/config/adapter/attrs.py
+-rw-r--r--   0        0        0     1078 2023-04-14 08:44:43.860787 gyver-2.1.2/gyver/config/adapter/dataclass.py
+-rw-r--r--   0        0        0     5886 2023-04-14 08:44:43.866790 gyver-2.1.2/gyver/config/adapter/factory.py
+-rw-r--r--   0        0        0     1056 2023-04-14 08:44:43.871793 gyver-2.1.2/gyver/config/adapter/gattrs.py
+-rw-r--r--   0        0        0     2107 2023-04-14 08:44:43.875795 gyver-2.1.2/gyver/config/adapter/interface.py
+-rw-r--r--   0        0        0     1701 2023-04-14 08:44:43.878796 gyver-2.1.2/gyver/config/adapter/mark.py
+-rw-r--r--   0        0        0     1091 2023-04-14 08:44:43.881798 gyver-2.1.2/gyver/config/adapter/pydantic.py
+-rw-r--r--   0        0        0     3435 2023-04-14 08:44:43.847781 gyver-2.1.2/gyver/config/config.py
+-rw-r--r--   0        0        0     2126 2023-04-14 08:44:43.849782 gyver-2.1.2/gyver/config/envconfig.py
+-rw-r--r--   0        0        0      587 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/config/typedef.py
+-rw-r--r--   0        0        0      473 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/config/utils.py
+-rw-r--r--   0        0        0      419 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/context/__init__.py
+-rw-r--r--   0        0        0      288 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/context/atomic_/__init__.py
+-rw-r--r--   0        0        0     2317 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/context/atomic_/bound.py
+-rw-r--r--   0        0        0     2493 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/context/atomic_/core.py
+-rw-r--r--   0        0        0     1332 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/context/atomic_/resolver.py
+-rw-r--r--   0        0        0     5659 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/context/context.py
+-rw-r--r--   0        0        0      102 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/context/interfaces/__init__.py
+-rw-r--r--   0        0        0     1525 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/context/interfaces/adapter.py
+-rw-r--r--   0        0        0       39 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/context/typedef.py
+-rw-r--r--   0        0        0      253 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/crypto/__init__.py
+-rw-r--r--   0        0        0      133 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/crypto/config.py
+-rw-r--r--   0        0        0      909 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/crypto/fernet.py
+-rw-r--r--   0        0        0     1856 2023-04-14 08:44:43.914814 gyver-2.1.2/gyver/crypto/rsa.py
+-rw-r--r--   0        0        0      749 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/database/__init__.py
+-rw-r--r--   0        0        0     2136 2023-04-14 08:44:43.927820 gyver-2.1.2/gyver/database/adapter.py
+-rw-r--r--   0        0        0     1233 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/database/config.py
+-rw-r--r--   0        0        0      360 2023-03-29 07:24:24.844143 gyver-2.1.2/gyver/database/context/__init__.py
+-rw-r--r--   0        0        0     3542 2023-04-14 08:44:42.980359 gyver-2.1.2/gyver/database/context/asyncio.py
+-rw-r--r--   0        0        0     3349 2023-03-29 07:29:51.153084 gyver-2.1.2/gyver/database/context/sync.py
+-rw-r--r--   0        0        0      170 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/database/drivers/__init__.py
+-rw-r--r--   0        0        0      229 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/database/drivers/dialect.py
+-rw-r--r--   0        0        0      224 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/database/drivers/interface.py
+-rw-r--r--   0        0        0     1493 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/database/drivers/utils.py
+-rw-r--r--   0        0        0     1076 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/database/entity.py
+-rw-r--r--   0        0        0      498 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/database/entity.pyi
+-rw-r--r--   0        0        0       50 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/database/metadata.py
+-rw-r--r--   0        0        0     1012 2023-04-14 08:44:43.954833 gyver-2.1.2/gyver/database/query/__init__.py
+-rw-r--r--   0        0        0     1692 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/database/query/_helpers.py
+-rw-r--r--   0        0        0     2935 2023-04-14 08:44:43.960836 gyver-2.1.2/gyver/database/query/comp.py
+-rw-r--r--   0        0        0      294 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/database/query/exc.py
+-rw-r--r--   0        0        0     1353 2023-04-14 08:44:43.004370 gyver-2.1.2/gyver/database/query/interface.py
+-rw-r--r--   0        0        0      279 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/database/query/null.py
+-rw-r--r--   0        0        0     1270 2023-04-14 08:44:43.969841 gyver-2.1.2/gyver/database/query/order_by.py
+-rw-r--r--   0        0        0     1239 2023-04-14 08:44:43.971842 gyver-2.1.2/gyver/database/query/paginate.py
+-rw-r--r--   0        0        0      697 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/database/query/utils.py
+-rw-r--r--   0        0        0     4613 2023-04-14 08:44:43.975844 gyver-2.1.2/gyver/database/query/where.py
+-rw-r--r--   0        0        0      327 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/database/typedef.py
+-rw-r--r--   0        0        0     4243 2023-04-14 08:44:43.080407 gyver-2.1.2/gyver/database/utils.py
+-rw-r--r--   0        0        0     2027 2023-05-31 11:17:46.118015 gyver-2.1.2/gyver/exc.py
+-rw-r--r--   0        0        0      857 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/model.py
+-rw-r--r--   0        0        0      101 2023-05-08 11:52:12.095726 gyver-2.1.2/gyver/pools/__init__.py
+-rw-r--r--   0        0        0     5764 2023-05-13 16:48:20.474968 gyver-2.1.2/gyver/pools/asyncio.py
+-rw-r--r--   0        0        0     2225 2023-05-13 16:48:21.238958 gyver-2.1.2/gyver/pools/resource.py
+-rw-r--r--   0        0        0     3855 2023-05-13 16:48:01.539206 gyver-2.1.2/gyver/pools/thread.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/py.typed
+-rw-r--r--   0        0        0      186 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/url/__init__.py
+-rw-r--r--   0        0        0     3166 2023-05-31 11:17:32.511186 gyver-2.1.2/gyver/url/core.py
+-rw-r--r--   0        0        0      423 2023-05-13 03:47:04.475970 gyver-2.1.2/gyver/url/encode.py
+-rw-r--r--   0        0        0      664 2023-05-13 16:48:21.208958 gyver-2.1.2/gyver/url/fragment.py
+-rw-r--r--   0        0        0     2834 2023-05-13 16:48:21.209958 gyver-2.1.2/gyver/url/netloc.py
+-rw-r--r--   0        0        0     2795 2023-05-13 16:48:21.212958 gyver-2.1.2/gyver/url/path.py
+-rw-r--r--   0        0        0     1711 2023-05-13 16:48:21.213958 gyver-2.1.2/gyver/url/query.py
+-rw-r--r--   0        0        0      662 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/url/utils.py
+-rw-r--r--   0        0        0      674 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/utils/__init__.py
+-rw-r--r--   0        0        0      156 2023-03-29 07:24:24.845143 gyver-2.1.2/gyver/utils/exc.py
+-rw-r--r--   0        0        0     7836 2023-04-14 08:44:44.001856 gyver-2.1.2/gyver/utils/finder.py
+-rw-r--r--   0        0        0     1391 2023-05-31 11:17:32.511186 gyver-2.1.2/gyver/utils/helpers.py
+-rw-r--r--   0        0        0      174 2023-03-29 07:24:24.846143 gyver-2.1.2/gyver/utils/json.py
+-rw-r--r--   0        0        0     2610 2023-03-29 07:24:24.846143 gyver-2.1.2/gyver/utils/lazy.py
+-rw-r--r--   0        0        0     1319 2023-04-14 08:44:44.010861 gyver-2.1.2/gyver/utils/singleton.py
+-rw-r--r--   0        0        0     1718 2023-03-29 07:24:24.846143 gyver-2.1.2/gyver/utils/strings.py
+-rw-r--r--   0        0        0      134 2023-03-29 07:24:24.846143 gyver-2.1.2/gyver/utils/timezone.py
+-rw-r--r--   0        0        0     2418 2023-05-31 11:18:06.209763 gyver-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 gyver-2.1.2/PKG-INFO
```

### Comparing `gyver-2.1.1/LICENSE` & `gyver-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/README.md` & `gyver-2.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 * [Pydantic](https://docs.pydantic.dev) for data handling.
 * [Typing Extensions](https://github.com/python/typing_extensions) for compatibility.
 * [Cryptography](https://cryptography.io) to handle encryption.
 
 ## Optional
 
 To use the database parts:
-* **Mysql/MariaDB:** AsyncMy, PyMySQL (use db-mysql or db-mariadb extras)
+* **Mysql/MariaDB:** AioMySQL, PyMySQL (use db-mysql or db-mariadb extras)
 * **Postgres:** AsyncPG, Psycopg2
 * **SQLite:** aiosqlite
 * **Redis:** redis
 * And **SQLAlchemy**
 
 ## Installation
 
 ```console
 $ pip install gyver
 ```
 
 ## Roadmap
 
-> Migrate from pydantic to dataclass/attrs for a lighter version of the library
+> Pack database code in a package specific "gyver-database" to make the gyver core lighter
 
 ##  License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `gyver-2.1.1/gyver/cache/asyncio.py` & `gyver-2.1.2/gyver/cache/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/cache/interface.py` & `gyver-2.1.2/gyver/cache/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/cache/mapper.py` & `gyver-2.1.2/gyver/cache/mapper.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/cache/mock.py` & `gyver-2.1.2/gyver/cache/mock.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/cache/redis.py` & `gyver-2.1.2/gyver/cache/redis.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/cache/sync.py` & `gyver-2.1.2/gyver/cache/sync.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/cache/utils.py` & `gyver-2.1.2/gyver/cache/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/config/adapter/attrs.py` & `gyver-2.1.2/gyver/config/adapter/attrs.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/config/adapter/dataclass.py` & `gyver-2.1.2/gyver/config/adapter/dataclass.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/config/adapter/factory.py` & `gyver-2.1.2/gyver/config/adapter/factory.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/config/adapter/gattrs.py` & `gyver-2.1.2/gyver/config/adapter/gattrs.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/config/adapter/interface.py` & `gyver-2.1.2/gyver/config/adapter/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/config/adapter/mark.py` & `gyver-2.1.2/gyver/config/adapter/mark.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/config/adapter/pydantic.py` & `gyver-2.1.2/gyver/config/adapter/pydantic.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/config/config.py` & `gyver-2.1.2/gyver/config/config.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/config/envconfig.py` & `gyver-2.1.2/gyver/config/envconfig.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/config/typedef.py` & `gyver-2.1.2/gyver/config/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/context/atomic_/bound.py` & `gyver-2.1.2/gyver/context/atomic_/bound.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/context/atomic_/core.py` & `gyver-2.1.2/gyver/context/atomic_/core.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/context/atomic_/resolver.py` & `gyver-2.1.2/gyver/context/atomic_/resolver.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/context/context.py` & `gyver-2.1.2/gyver/context/context.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/context/interfaces/adapter.py` & `gyver-2.1.2/gyver/context/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/crypto/fernet.py` & `gyver-2.1.2/gyver/crypto/fernet.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/crypto/rsa.py` & `gyver-2.1.2/gyver/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/__init__.py` & `gyver-2.1.2/gyver/database/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/adapter.py` & `gyver-2.1.2/gyver/database/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/config.py` & `gyver-2.1.2/gyver/database/config.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/context/asyncio.py` & `gyver-2.1.2/gyver/database/context/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/context/sync.py` & `gyver-2.1.2/gyver/database/context/sync.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/drivers/utils.py` & `gyver-2.1.2/gyver/database/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/entity.py` & `gyver-2.1.2/gyver/database/entity.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/query/__init__.py` & `gyver-2.1.2/gyver/database/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/query/_helpers.py` & `gyver-2.1.2/gyver/database/query/_helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/query/comp.py` & `gyver-2.1.2/gyver/database/query/comp.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/query/interface.py` & `gyver-2.1.2/gyver/database/query/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/query/order_by.py` & `gyver-2.1.2/gyver/database/query/order_by.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/query/paginate.py` & `gyver-2.1.2/gyver/database/query/paginate.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/query/utils.py` & `gyver-2.1.2/gyver/database/query/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/query/where.py` & `gyver-2.1.2/gyver/database/query/where.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/database/utils.py` & `gyver-2.1.2/gyver/database/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/exc.py` & `gyver-2.1.2/gyver/exc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from itertools import chain
 
-from pyparsing import Sequence
+from typing import Sequence
 
 
 class GyverError(Exception):
     """Base exception for all gyver exceptions"""
 
 
 class InvalidCast(GyverError):
```

### Comparing `gyver-2.1.1/gyver/model.py` & `gyver-2.1.2/gyver/model.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/pools/asyncio.py` & `gyver-2.1.2/gyver/pools/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/pools/resource.py` & `gyver-2.1.2/gyver/pools/resource.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/pools/thread.py` & `gyver-2.1.2/gyver/pools/thread.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/url/core.py` & `gyver-2.1.2/gyver/url/core.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/url/fragment.py` & `gyver-2.1.2/gyver/url/fragment.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/url/netloc.py` & `gyver-2.1.2/gyver/url/netloc.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/url/path.py` & `gyver-2.1.2/gyver/url/path.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/url/query.py` & `gyver-2.1.2/gyver/url/query.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/url/utils.py` & `gyver-2.1.2/gyver/url/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/utils/__init__.py` & `gyver-2.1.2/gyver/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/utils/finder.py` & `gyver-2.1.2/gyver/utils/finder.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/utils/helpers.py` & `gyver-2.1.2/gyver/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/utils/lazy.py` & `gyver-2.1.2/gyver/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/utils/singleton.py` & `gyver-2.1.2/gyver/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/gyver/utils/strings.py` & `gyver-2.1.2/gyver/utils/strings.py`

 * *Files identical despite different names*

### Comparing `gyver-2.1.1/pyproject.toml` & `gyver-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gyver"
-version = "2.1.1"
+version = "2.1.2"
 description = "Toolbox for web development"
 authors = ["Gustavo Correa <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/guscardvs/gyver"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gyver-2.1.1/PKG-INFO` & `gyver-2.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyver
-Version: 2.1.1
+Version: 2.1.2
 Summary: Toolbox for web development
 Home-page: https://github.com/guscardvs/gyver
 Author: Gustavo Correa
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -53,26 +53,26 @@
 * [Pydantic](https://docs.pydantic.dev) for data handling.
 * [Typing Extensions](https://github.com/python/typing_extensions) for compatibility.
 * [Cryptography](https://cryptography.io) to handle encryption.
 
 ## Optional
 
 To use the database parts:
-* **Mysql/MariaDB:** AsyncMy, PyMySQL (use db-mysql or db-mariadb extras)
+* **Mysql/MariaDB:** AioMySQL, PyMySQL (use db-mysql or db-mariadb extras)
 * **Postgres:** AsyncPG, Psycopg2
 * **SQLite:** aiosqlite
 * **Redis:** redis
 * And **SQLAlchemy**
 
 ## Installation
 
 ```console
 $ pip install gyver
 ```
 
 ## Roadmap
 
-> Migrate from pydantic to dataclass/attrs for a lighter version of the library
+> Pack database code in a package specific "gyver-database" to make the gyver core lighter
 
 ##  License
 
 This project is licensed under the terms of the MIT license.
```

