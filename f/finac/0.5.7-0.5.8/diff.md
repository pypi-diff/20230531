# Comparing `tmp/finac-0.5.7.tar.gz` & `tmp/finac-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/finac-0.5.7.tar", last modified: Tue Aug  3 21:22:27 2021, max compression
+gzip compressed data, was "finac-0.5.8.tar", last modified: Wed May 31 17:29:43 2023, max compression
```

## Comparing `finac-0.5.7.tar` & `finac-0.5.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 jenkins    (107) jenkins    (113)        0 2021-08-03 21:22:27.000000 finac-0.5.7/
--rw-r--r--   0 jenkins    (107) jenkins    (113)       38 2021-08-03 21:22:27.000000 finac-0.5.7/setup.cfg
--rw-r--r--   0 jenkins    (107) jenkins    (113)    10453 2021-08-03 21:21:03.000000 finac-0.5.7/README.md
-drwxr-xr-x   0 jenkins    (107) jenkins    (113)        0 2021-08-03 21:22:27.000000 finac-0.5.7/finac.egg-info/
--rw-r--r--   0 jenkins    (107) jenkins    (113)        1 2021-08-03 21:22:26.000000 finac-0.5.7/finac.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (107) jenkins    (113)      101 2021-08-03 21:22:26.000000 finac-0.5.7/finac.egg-info/requires.txt
--rw-r--r--   0 jenkins    (107) jenkins    (113)        6 2021-08-03 21:22:26.000000 finac-0.5.7/finac.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (107) jenkins    (113)    13668 2021-08-03 21:22:26.000000 finac-0.5.7/finac.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (107) jenkins    (113)      269 2021-08-03 21:22:27.000000 finac-0.5.7/finac.egg-info/SOURCES.txt
-drwxr-xr-x   0 jenkins    (107) jenkins    (113)        0 2021-08-03 21:22:27.000000 finac-0.5.7/finac/
--rw-r--r--   0 jenkins    (107) jenkins    (113)     2086 2021-08-03 21:21:03.000000 finac-0.5.7/finac/df.py
--rw-r--r--   0 jenkins    (107) jenkins    (113)     4760 2020-05-16 23:04:36.000000 finac-0.5.7/finac/db_set.py
--rw-r--r--   0 jenkins    (107) jenkins    (113)    12997 2021-08-03 21:21:03.000000 finac-0.5.7/finac/__init__.py
--rw-r--r--   0 jenkins    (107) jenkins    (113)     9958 2020-02-27 23:54:01.000000 finac-0.5.7/finac/currencies.py
--rw-r--r--   0 jenkins    (107) jenkins    (113)     2780 2021-08-03 21:21:03.000000 finac-0.5.7/finac/plot.py
--rw-r--r--   0 jenkins    (107) jenkins    (113)     8761 2020-05-05 02:28:29.000000 finac-0.5.7/finac/api.py
--rw-r--r--   0 jenkins    (107) jenkins    (113)    91601 2021-08-03 21:21:03.000000 finac-0.5.7/finac/core.py
--rw-r--r--   0 jenkins    (107) jenkins    (113)    13668 2021-08-03 21:22:27.000000 finac-0.5.7/PKG-INFO
--rw-r--r--   0 jenkins    (107) jenkins    (113)     1103 2021-08-03 21:21:03.000000 finac-0.5.7/setup.py
+drwxr-xr-x   0 rci        (999) rci        (999)        0 2023-05-31 17:29:43.184437 finac-0.5.8/
+-rw-r--r--   0 rci        (999) rci        (999)     1066 2023-05-31 17:26:30.000000 finac-0.5.8/LICENSE
+-rw-r--r--   0 rci        (999) rci        (999)    11281 2023-05-31 17:29:43.184437 finac-0.5.8/PKG-INFO
+-rw-r--r--   0 rci        (999) rci        (999)    10607 2023-05-31 17:26:30.000000 finac-0.5.8/README.md
+drwxr-xr-x   0 rci        (999) rci        (999)        0 2023-05-31 17:29:43.184437 finac-0.5.8/finac/
+-rw-r--r--   0 rci        (999) rci        (999)    12997 2023-05-31 17:26:30.000000 finac-0.5.8/finac/__init__.py
+-rw-r--r--   0 rci        (999) rci        (999)     8761 2023-05-31 17:26:30.000000 finac-0.5.8/finac/api.py
+-rw-r--r--   0 rci        (999) rci        (999)    91398 2023-05-31 17:26:30.000000 finac-0.5.8/finac/core.py
+-rw-r--r--   0 rci        (999) rci        (999)     9958 2023-05-31 17:26:30.000000 finac-0.5.8/finac/currencies.py
+-rw-r--r--   0 rci        (999) rci        (999)     4725 2023-05-31 17:26:30.000000 finac-0.5.8/finac/db_set.py
+-rw-r--r--   0 rci        (999) rci        (999)     2086 2023-05-31 17:26:30.000000 finac-0.5.8/finac/df.py
+-rw-r--r--   0 rci        (999) rci        (999)     2780 2023-05-31 17:26:30.000000 finac-0.5.8/finac/plot.py
+drwxr-xr-x   0 rci        (999) rci        (999)        0 2023-05-31 17:29:43.184437 finac-0.5.8/finac.egg-info/
+-rw-r--r--   0 rci        (999) rci        (999)    11281 2023-05-31 17:29:43.000000 finac-0.5.8/finac.egg-info/PKG-INFO
+-rw-r--r--   0 rci        (999) rci        (999)      277 2023-05-31 17:29:43.000000 finac-0.5.8/finac.egg-info/SOURCES.txt
+-rw-r--r--   0 rci        (999) rci        (999)        1 2023-05-31 17:29:43.000000 finac-0.5.8/finac.egg-info/dependency_links.txt
+-rw-r--r--   0 rci        (999) rci        (999)      103 2023-05-31 17:29:43.000000 finac-0.5.8/finac.egg-info/requires.txt
+-rw-r--r--   0 rci        (999) rci        (999)        6 2023-05-31 17:29:43.000000 finac-0.5.8/finac.egg-info/top_level.txt
+-rw-r--r--   0 rci        (999) rci        (999)       38 2023-05-31 17:29:43.184437 finac-0.5.8/setup.cfg
+-rw-r--r--   0 rci        (999) rci        (999)     1105 2023-05-31 17:26:30.000000 finac-0.5.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `finac-0.5.7/README.md` & `finac-0.5.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 
 Finac is a library and function set for Jupyter/ipython, which provides the
 double-entry bookkeeping database.
 
 Finac is simple, open and free. It can work with SQLite or any database
 supported by SQLAlchemy (tested: SQLite, MySQL, PostgreSQL).
 
-<img src="https://img.shields.io/pypi/v/finac.svg" /> <img src="https://img.shields.io/badge/license-MIT-green" /> <img src="https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-blue.svg" />
+WARNING: SQLAlchemy 2 is NOT SUPPORTED until stabilized. If SQLAlchemy 2 is
+required for other projects, run Finac in a dedicated virtual environment. 
+
+<img src="https://img.shields.io/pypi/v/finac.svg" /> <img src="https://img.shields.io/badge/license-MIT-green" /> <img src="https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg" />
 
 Finac can be used either in the interactive mode with
 [Jupyter](https://jupyter.org/), [Spyder-IDE](https://www.spyder-ide.org/),
 ipython or other similar environment or Finac library can be embedded into 3rd
 party projects. The library can be used in accounting applications and is
 useful for fin-tech services.
```

### Comparing `finac-0.5.7/finac/df.py` & `finac-0.5.8/finac/df.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = 'Altertech, https://www.altertech.com/'
 __copyright__ = 'Copyright (C) 2019 Altertech'
 __license__ = 'MIT'
 
-__version__ = '0.5.7'
+__version__ = '0.5.8'
 
 from . import core
 
 
 def df(fn, *args, **kwargs):
     """
     Get Finac DB data as Pandas DataFrame
```

### Comparing `finac-0.5.7/finac/db_set.py` & `finac-0.5.8/finac/db_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,14 @@
                      Column('account_credit_id', Integer,
                             ForeignKey('account.id', ondelete='SET NULL')),
                      Column('account_debit_id', Integer,
                             ForeignKey('account.id', ondelete='SET NULL')),
                      Column('amount', Float(precision=32), nullable=False),
                      Column('tag', String(20)),
                      Index('transact_tag', 'tag'),
-                     Column('note', String(20)),
                      Column('note', String(1024), server_default=''),
                      Column('d_created',
                             DateTime(timezone=True),
                             nullable=False),
                      Column('d', DateTime(timezone=True)),
                      Index('transact_account_credit_id', 'account_credit_id'),
                      Index('transact_account_debit_id', 'account_debit_id'),
@@ -91,12 +90,13 @@
                      mysql_engine='InnoDB',
                      mysql_charset='utf8mb4')
 
     meta.create_all(engine)
     conn = engine.connect()
     for cur in ('EUR', 'USD'):
         try:
-            conn.execute(sql("""
+            conn.execute(
+                sql("""
                 INSERT INTO asset(code, precs) VALUES(:code, 2)"""),
-                         code=cur)
+                dict(code=cur))
         except IntegrityError:
             pass
```

### Comparing `finac-0.5.7/finac/__init__.py` & `finac-0.5.8/finac/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = 'Altertech, https://www.altertech.com/'
 __copyright__ = 'Copyright (C) 2019 Altertech'
 __license__ = 'MIT'
 
-__version__ = '0.5.7'
+__version__ = '0.5.8'
 
 import rapidtables
 import neotermcolor
 import datetime, time
 
 from functools import partial
 from collections import OrderedDict
```

### Comparing `finac-0.5.7/finac/currencies.py` & `finac-0.5.8/finac/currencies.py`

 * *Files identical despite different names*

### Comparing `finac-0.5.7/finac/plot.py` & `finac-0.5.8/finac/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = 'Altertech, https://www.altertech.com/'
 __copyright__ = 'Copyright (C) 2019 Altertech'
 __license__ = 'MIT'
 
-__version__ = '0.5.7'
+__version__ = '0.5.8'
 
 from . import core
 
 
 def account_plot(account=None,
                  tp=None,
                  start=None,
```

### Comparing `finac-0.5.7/finac/api.py` & `finac-0.5.8/finac/api.py`

 * *Files identical despite different names*

### Comparing `finac-0.5.7/finac/core.py` & `finac-0.5.8/finac/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = 'Altertech, https://www.altertech.com/'
 __copyright__ = 'Copyright (C) 2019 Altertech'
 __license__ = 'MIT'
 
-__version__ = '0.5.7'
+__version__ = '0.5.8'
 
 from sqlalchemy.exc import IntegrityError
 from cachetools import TTLCache
 from itertools import groupby
 from .currencies import currencies
 from types import SimpleNamespace
 from concurrent.futures import ThreadPoolExecutor
@@ -356,15 +356,15 @@
 
 @core_method
 def _asset_precision(asset=None):
     if asset:
         if asset in _asset_precision_cache:
             return _asset_precision_cache[asset]
         d = get_db().execute(sql('select precs from asset where code=:code'),
-                             code=asset.upper()).fetchone()
+                             dict(code=asset.upper())).fetchone()
         if not d:
             raise ResourceNotFound
         precs = int(d.precs)
         _asset_precision_cache[asset] = precs
         return precs
     else:
 
@@ -655,18 +655,18 @@
     asset = asset.upper()
     if restrict_assets_to_currencies:
         if asset not in [c['cc'] for c in currencies]:
             logger.error('Currency {} not found'.format(asset))
             raise ResourceNotFound
     logger.info('Creating asset {}'.format(asset))
     try:
-        get_db().execute(sql("""
+        get_db().execute(
+            sql("""
         insert into asset(code, precs) values(:code, :precision)"""),
-                         code=asset,
-                         precision=precision)
+            dict(code=asset, precision=precision))
     except IntegrityError:
         raise ResourceAlreadyExists(asset)
 
 
 @core_method
 def asset_list():
     """
@@ -728,15 +728,16 @@
                 join asset as ct on asset_to_id = ct.id
                     where {cond} order by d
         """.format(cond=cond)))
     else:
         d = parse_date(end, return_timestamp=False,
                        ms=_time_ms) if end else parse_date(
                            return_timestamp=False)
-        r = get_db().execute(sql("""
+        r = get_db().execute(
+            sql("""
             select
                 a1.code as asset_from,
                 a2.code as asset_to,
                 ar.value as value, m as d
             from
                 (select
                     as1.asset_from_id as fr,
@@ -746,16 +747,15 @@
                 where as1.d<=:d group by fr, t)
             as s1
                 join asset as a1 on a1.id=fr
                 join asset as a2 on a2.id=t
                 join asset_rate as ar on ar.asset_from_id=fr
                     and ar.asset_to_id=t and ar.d=m
                 order by asset_from, asset_to
-                    """),
-                             d=d)
+                    """), dict(d=d))
     while True:
         d = r.fetchone()
         if not d:
             break
         row = OrderedDict()
         row['asset_from'] = d.asset_from
         row['asset_to'] = d.asset_to
@@ -770,16 +770,15 @@
     """
     Delete asset
 
     Warning: all accounts linked to this asset will be deleted as well
     """
     logger.warning('Deleting asset {}'.format(asset.upper()))
     if not get_db().execute(sql("""
-    delete from asset where code=:code"""),
-                            code=asset.upper()).rowcount:
+    delete from asset where code=:code"""), dict(code=asset.upper())).rowcount:
         logger.error('Asset {} not found'.format(asset.upper()))
         raise ResourceNotFound
 
 
 @core_method
 def asset_set_rate(asset_from, asset_to=None, value=None, date=None):
     """
@@ -805,28 +804,29 @@
         date = parse_date(return_timestamp=False)
     else:
         date = parse_date(date, return_timestamp=False)
     if asset_from.find('/') != -1 and asset_to is None:
         asset_from, asset_to = asset_from.split('/')
     logger.info('Setting rate for {}/{} to {} for {}'.format(
         asset_from.upper(), asset_to.upper(), value, format_date(date)))
-    get_db().execute(sql("""
+    get_db().execute(
+        sql("""
     insert into asset_rate (asset_from_id, asset_to_id, d, value)
     values
     (
         (select id from asset where code=:f),
         (select id from asset where code=:t),
         :d,
         :value
     )
     """),
-                     f=asset_from.upper(),
-                     t=asset_to.upper(),
-                     d=date,
-                     value=_multiply(value))
+        dict(f=asset_from.upper(),
+             t=asset_to.upper(),
+             d=date,
+             value=_multiply(value)))
 
 
 @deletion_method
 @core_method
 def asset_delete_rate(asset_from, asset_to=None, date=None):
     """
     Delete currrency rate
@@ -835,24 +835,22 @@
         raise ValueError('asset rate date not specified')
     if asset_from.find('/') != -1 and asset_to is None:
         asset_from, asset_to = asset_from.split('/')
     date = parse_date(date, return_timestamp=False)
     logger.info('Deleting rate for {}/{} for {}'.format(asset_from.upper(),
                                                         asset_to.upper(),
                                                         format_date(date)))
-    if not get_db().execute(sql("""
+    if not get_db().execute(
+            sql("""
     delete from asset_rate where
         asset_from_id=(select id from asset where code=:f)
         and
         asset_to_id=(select id from asset where code=:t)
         and d=:d
-        """),
-                            f=asset_from.upper(),
-                            t=asset_to.upper(),
-                            d=date).rowcount:
+        """), dict(f=asset_from.upper(), t=asset_to.upper(), d=date)).rowcount:
         logger.error('Asset rate {}/{} for {} not found'.format(
             asset_from.upper(), asset_to.upper(), format_date(date)))
         raise ResourceNotFound
 
 
 def _parse_asset_pair(asset_from, asset_to):
     if asset_from is None:
@@ -901,24 +899,22 @@
     db = get_db()
 
     def _get_rate(cf, ct, d):
         key = _format_ttlcache_key(d, config.rate_cache_ttl)
         try:
             return _cache.rate[(cf, ct, key)]
         except _CacheRateKeyError:
-            r = db.execute(sql("""
+            r = db.execute(
+                sql("""
                 select value from asset_rate
                     join asset as cfrom on asset_from_id=cfrom.id
                     join asset as cto on asset_to_id=cto.id
                 where d <= :d and cfrom.code = :f and cto.code = :t
                 order by d desc limit 1
-                """),
-                           d=date,
-                           f=cf,
-                           t=ct)
+                """), dict(d=date, f=cf, t=ct))
             d = r.fetchone()
             if d:
                 value = _demultiply(d.value)
                 _cache.rate[(cf, ct, key)] = value
                 return value
             else:
                 return None
@@ -1011,33 +1007,34 @@
         passive = True
     else:
         passive = val_to_boolean(passive)
     db = get_db()
     account = account.upper()
     asset = asset.upper()
     if not db.execute(sql("""select id from asset where code=:code"""),
-                      code=asset).fetchone():
+                      dict(code=asset)).fetchone():
         raise ResourceNotFound('asset {}'.format(asset))
     dbt = db.begin()
     logger.info('Creating account {}, asset: {}'.format(account, asset))
     try:
-        r = db.execute(sql("""
+        r = db.execute(
+            sql("""
         insert into account(code, note, tp, passive, asset_id, max_overdraft,
         max_balance) values
         (:code, :note, :tp, :passive,
             (select id from asset where code=:asset),
             :max_overdraft, :max_balance) {}""".format(
-            '' if _db.use_lastrowid else 'returning id')),
-                       code=account,
-                       note=note,
-                       tp=tp_id,
-                       passive=passive,
-                       asset=asset,
-                       max_overdraft=_multiply(max_overdraft),
-                       max_balance=_multiply(max_balance))
+                '' if _db.use_lastrowid else 'returning id')),
+            dict(code=account,
+                 note=note,
+                 tp=tp_id,
+                 passive=passive,
+                 asset=asset,
+                 max_overdraft=_multiply(max_overdraft),
+                 max_balance=_multiply(max_balance)))
         acc_id = r.lastrowid if _db.use_lastrowid else r.fetchone().id
         db.execute(sql("""
             INSERT INTO transact
                 (account_debit_id, amount, d_created, d, service)
             VALUES
                 (:account_id, 0, :d, :d, :s)
             """),
@@ -1177,15 +1174,15 @@
     import yaml
     try:
         yaml.warnings({'YAMLLoadWarning': False})
     except:
         pass
     result = []
     with open(fname) as fh:
-        transactions = yaml.load(fh)['transactions']
+        transactions = yaml.safe_load(fh)['transactions']
     for t in transactions:
         if 'account' in t:
             result.append(transaction_create(**t))
         else:
             result.append(transaction_move(**t))
     return result
```

### Comparing `finac-0.5.7/setup.py` & `finac-0.5.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.5.7'
+__version__ = '0.5.8'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
@@ -13,15 +13,15 @@
     description='Financial accounting library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/alttch/finac',
     packages=setuptools.find_packages(),
     license='MIT',
     install_requires=[
-        'rapidtables', 'python-dateutil', 'neotermcolor', 'sqlalchemy',
+        'rapidtables', 'python-dateutil', 'neotermcolor', 'sqlalchemy<2',
         'pyyaml', 'cachetools', 'flask', 'requests', 'pyaltt2>=0.0.89'
     ],
     classifiers=('Programming Language :: Python :: 3',
                  'License :: OSI Approved :: MIT License',
                  'Topic :: Software Development :: Libraries',
                  'Intended Audience :: Financial and Insurance Industry',
                  'Topic :: Office/Business :: Financial',
```

