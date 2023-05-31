# Comparing `tmp/nonebot_plugin_sqlalchemy-0.2.0.tar.gz` & `tmp/nonebot_plugin_sqlalchemy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sqlalchemy-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_sqlalchemy-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_sqlalchemy-0.2.0.tar` & `nonebot_plugin_sqlalchemy-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1085 2022-12-23 11:30:13.292518 nonebot_plugin_sqlalchemy-0.2.0/LICENSE
--rw-r--r--   0        0        0      637 2023-03-13 10:50:41.512528 nonebot_plugin_sqlalchemy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4292 2023-03-13 11:20:25.427869 nonebot_plugin_sqlalchemy-0.2.0/README.MD
--rw-r--r--   0        0        0     3402 2023-03-11 14:52:31.259575 nonebot_plugin_sqlalchemy-0.2.0/src/nonebot_plugin_sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5072 1970-01-01 00:00:00.000000 nonebot_plugin_sqlalchemy-0.2.0/setup.py
--rw-r--r--   0        0        0     4869 1970-01-01 00:00:00.000000 nonebot_plugin_sqlalchemy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-12-23 11:30:13.292518 nonebot_plugin_sqlalchemy-0.2.1/LICENSE
+-rw-r--r--   0        0        0      637 2023-05-31 06:20:08.021876 nonebot_plugin_sqlalchemy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4292 2023-03-13 11:20:25.427869 nonebot_plugin_sqlalchemy-0.2.1/README.MD
+-rw-r--r--   0        0        0     4394 2023-05-31 06:22:57.386026 nonebot_plugin_sqlalchemy-0.2.1/src/nonebot_plugin_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     4869 1970-01-01 00:00:00.000000 nonebot_plugin_sqlalchemy-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_sqlalchemy-0.2.0/LICENSE` & `nonebot_plugin_sqlalchemy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sqlalchemy-0.2.0/pyproject.toml` & `nonebot_plugin_sqlalchemy-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-sqlalchemy"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.MD"
 license = "MIT"
 repository = "https://github.com/ssttkkl/nonebot-plugin-sqlalchemy"
 packages = [
     { include = "nonebot_plugin_sqlalchemy", from = "src" },
```

### Comparing `nonebot_plugin_sqlalchemy-0.2.0/README.MD` & `nonebot_plugin_sqlalchemy-0.2.1/README.MD`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sqlalchemy-0.2.0/src/nonebot_plugin_sqlalchemy/__init__.py` & `nonebot_plugin_sqlalchemy-0.2.1/src/nonebot_plugin_sqlalchemy/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from asyncio import gather
 from inspect import isawaitable
-from typing import Callable, Awaitable, Union
+from typing import Callable, Awaitable, Union, List
+from urllib.parse import urlparse
 
 from nonebot import logger, Driver
 from nonebot.internal.matcher import current_matcher
 from nonebot.message import run_postprocessor
 from sqlalchemy.ext.asyncio import AsyncSession, AsyncEngine, create_async_engine, async_scoped_session
 from sqlalchemy.orm import registry
 from sqlalchemy.orm import sessionmaker
 
 T_OnReadyCallback = Union[Callable[[], None], Callable[[], Awaitable[None]]]
 
 T_OnEngineCreatedCallback = Union[Callable[[AsyncEngine], None], Callable[[AsyncEngine], Awaitable[None]]]
 
+T_OnRemoveSession = Union[Callable[[], None], Callable[[], Awaitable[None]]]
+
+T_OnSessionRemoved = Union[Callable[[], None], Callable[[], Awaitable[None]]]
+
 
 async def _fire(callbacks, args=None, kwargs=None):
     if args is None:
         args = []
     if kwargs is None:
         kwargs = {}
 
@@ -26,22 +31,34 @@
 
 
 class DataSourceNotReadyError(RuntimeError):
     pass
 
 
 class DataSource:
+    @staticmethod
+    def _detect_dialect(url: str):
+        parsed_url = urlparse(url)
+        if '+' in parsed_url.scheme:
+            return parsed_url.scheme.split('+')[0]
+        else:
+            return parsed_url.scheme
+
     def __init__(self, driver: Driver, url: str, **kwargs):
         self._engine = None
         self._session = None
 
         self._registry = registry()
 
-        self._on_engine_created_callback = []
-        self._on_ready_callback = []
+        self._on_engine_created_callback: List[T_OnEngineCreatedCallback] = []
+        self._on_ready_callback: List[T_OnReadyCallback] = []
+        self._on_remove_session_callback: List[T_OnRemoveSession] = []
+        self._on_session_removed_callback: List[T_OnSessionRemoved] = []
+
+        self.dialect = self._detect_dialect(url)
 
         # 仅当trace模式时回显sql语句
         kwargs.setdefault("echo", driver.config.log_level.lower() == 'TRACE')
         kwargs.setdefault("future", True)
 
         @driver.on_startup
         async def on_startup():
@@ -70,16 +87,18 @@
             self._session = None
 
             logger.success("data source disposed")
 
         @run_postprocessor
         async def postprocessor():
             if self._session is not None:
+                await _fire(self._on_remove_session_callback)
                 await self._session.remove()
                 logger.trace("session removed")
+                await _fire(self._on_session_removed_callback)
 
     @property
     def engine(self) -> AsyncEngine:
         if self._engine is None:
             raise DataSourceNotReadyError()
         return self._engine
 
@@ -90,16 +109,20 @@
     @property
     def session(self) -> async_scoped_session:
         if self._session is None:
             raise DataSourceNotReadyError()
         return self._session
 
     def on_engine_created(self, action: T_OnEngineCreatedCallback):
-        logger.trace("engine created")
         self._on_engine_created_callback.append(action)
 
     def on_ready(self, action: T_OnReadyCallback):
-        logger.trace("ready")
         self._on_ready_callback.append(action)
 
+    def on_remove_session(self, action: T_OnRemoveSession):
+        self._on_remove_session_callback.append(action)
+
+    def on_session_removed(self, action: T_OnRemoveSession):
+        self._on_session_removed_callback.append(action)
+
 
 __all__ = ("DataSource", "DataSourceNotReadyError")
```

### Comparing `nonebot_plugin_sqlalchemy-0.2.0/setup.py` & `nonebot_plugin_sqlalchemy-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,317 +1,305 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 655f 6469  etup..package_di
-00000040: 7220 3d20 5c0a 7b27 273a 2027 7372 6327  r = \.{'': 'src'
-00000050: 7d0a 0a70 6163 6b61 6765 7320 3d20 5c0a  }..packages = \.
-00000060: 5b27 6e6f 6e65 626f 745f 706c 7567 696e  ['nonebot_plugin
-00000070: 5f73 716c 616c 6368 656d 7927 5d0a 0a70  _sqlalchemy']..p
-00000080: 6163 6b61 6765 5f64 6174 6120 3d20 5c0a  ackage_data = \.
-00000090: 7b27 273a 205b 272a 275d 7d0a 0a69 6e73  {'': ['*']}..ins
-000000a0: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-000000b0: 5c0a 5b27 6e6f 6e65 626f 7432 3e3d 322e  \.['nonebot2>=2.
-000000c0: 302e 302d 7263 2e33 2c3c 332e 302e 3027  0.0-rc.3,<3.0.0'
-000000d0: 2c20 2773 716c 616c 6368 656d 795b 6173  , 'sqlalchemy[as
-000000e0: 796e 6369 6f5d 3e3d 322e 302e 302c 3c33  yncio]>=2.0.0,<3
-000000f0: 2e30 2e30 275d 0a0a 7365 7475 705f 6b77  .0.0']..setup_kw
-00000100: 6172 6773 203d 207b 0a20 2020 2027 6e61  args = {.    'na
-00000110: 6d65 273a 2027 6e6f 6e65 626f 742d 706c  me': 'nonebot-pl
-00000120: 7567 696e 2d73 716c 616c 6368 656d 7927  ugin-sqlalchemy'
-00000130: 2c0a 2020 2020 2776 6572 7369 6f6e 273a  ,.    'version':
-00000140: 2027 302e 322e 3027 2c0a 2020 2020 2764   '0.2.0',.    'd
-00000150: 6573 6372 6970 7469 6f6e 273a 2027 272c  escription': '',
-00000160: 0a20 2020 2027 6c6f 6e67 5f64 6573 6372  .    'long_descr
-00000170: 6970 7469 6f6e 273a 2027 3c21 2d2d 206d  iption': '<!-- m
-00000180: 6172 6b64 6f77 6e6c 696e 742d 6469 7361  arkdownlint-disa
-00000190: 626c 6520 4d44 3033 3320 4d44 3033 3620  ble MD033 MD036 
-000001a0: 4d44 3034 3120 2d2d 3e5c 6e5c 6e3c 7020  MD041 -->\n\n<p 
-000001b0: 616c 6967 6e3d 2263 656e 7465 7222 3e5c  align="center">\
-000001c0: 6e20 203c 6120 6872 6566 3d22 6874 7470  n  <a href="http
-000001d0: 733a 2f2f 7632 2e6e 6f6e 6562 6f74 2e64  s://v2.nonebot.d
-000001e0: 6576 2f22 3e3c 696d 6720 7372 633d 2268  ev/"><img src="h
-000001f0: 7474 7073 3a2f 2f76 322e 6e6f 6e65 626f  ttps://v2.nonebo
-00000200: 742e 6465 762f 6c6f 676f 2e70 6e67 2220  t.dev/logo.png" 
-00000210: 7769 6474 683d 2232 3030 2220 6865 6967  width="200" heig
-00000220: 6874 3d22 3230 3022 2061 6c74 3d22 6e6f  ht="200" alt="no
-00000230: 6e65 626f 7422 3e3c 2f61 3e5c 6e3c 2f70  nebot"></a>\n</p
-00000240: 3e5c 6e5c 6e3c 6469 7620 616c 6967 6e3d  >\n\n<div align=
-00000250: 2263 656e 7465 7222 3e5c 6e5c 6e6e 6f6e  "center">\n\nnon
-00000260: 6562 6f74 2d70 6c75 6769 6e2d 7371 6c61  ebot-plugin-sqla
-00000270: 6c63 6865 6d79 5c6e 3d3d 3d3d 3d3d 3d3d  lchemy\n========
-00000280: 3d3d 3d3d 5c6e 5c6e 5fe2 9ca8 204e 6f6e  ====\n\n_... Non
-00000290: 6542 6f74 2053 514c 416c 6368 656d 7920  eBot SQLAlchemy 
-000002a0: e5b0 81e8 a385 e68f 92e4 bbb6 20e2 9ca8  ............ ...
-000002b0: 5f5c 6e5c 6e3c 2f64 6976 3e5c 6e5c 6e3c  _\n\n</div>\n\n<
-000002c0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-000002d0: 3e5c 6e20 203c 6120 6872 6566 3d22 6874  >\n  <a href="ht
-000002e0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-000002f0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000300: 7373 7474 6b6b 6c2f 6e6f 6e65 626f 742d  ssttkkl/nonebot-
-00000310: 706c 7567 696e 2d73 716c 616c 6368 656d  plugin-sqlalchem
-00000320: 792f 6d61 7374 6572 2f4c 4943 454e 5345  y/master/LICENSE
-00000330: 223e 5c6e 2020 2020 3c69 6d67 2073 7263  ">\n    <img src
-00000340: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000350: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000360: 6c69 6365 6e73 652f 7373 7474 6b6b 6c2f  license/ssttkkl/
-00000370: 6e6f 6e65 626f 742d 706c 7567 696e 2d73  nonebot-plugin-s
-00000380: 716c 616c 6368 656d 792e 7376 6722 2061  qlalchemy.svg" a
-00000390: 6c74 3d22 6c69 6365 6e73 6522 3e5c 6e20  lt="license">\n 
-000003a0: 203c 2f61 3e5c 6e20 203c 6120 6872 6566   </a>\n  <a href
-000003b0: 3d22 6874 7470 733a 2f2f 7079 7069 2e70  ="https://pypi.p
-000003c0: 7974 686f 6e2e 6f72 672f 7079 7069 2f6e  ython.org/pypi/n
-000003d0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 7371  onebot-plugin-sq
-000003e0: 6c61 6c63 6865 6d79 223e 5c6e 2020 2020  lalchemy">\n    
-000003f0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000400: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000410: 2f70 7970 692f 762f 6e6f 6e65 626f 742d  /pypi/v/nonebot-
-00000420: 706c 7567 696e 2d73 716c 616c 6368 656d  plugin-sqlalchem
-00000430: 792e 7376 6722 2061 6c74 3d22 7079 7069  y.svg" alt="pypi
-00000440: 223e 5c6e 2020 3c2f 613e 5c6e 2020 3c69  ">\n  </a>\n  <i
-00000450: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000460: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000470: 6164 6765 2f70 7974 686f 6e2d 332e 392b  adge/python-3.9+
-00000480: 2d62 6c75 652e 7376 6722 2061 6c74 3d22  -blue.svg" alt="
-00000490: 7079 7468 6f6e 223e 5c6e 3c2f 703e 5c6e  python">\n</p>\n
-000004a0: 5c6e e4b8 bae6 8f92 e4bb b6e5 b081 e8a3  \n..............
-000004b0: 8553 514c 416c 6368 656d 79e6 95b0 e68d  .SQLAlchemy.....
-000004c0: aee5 ba93 e8ae bfe9 97ae efbc 8ce4 b880  ................
-000004d0: e4b8 aae6 8f92 e4bb b6e4 bdbf e794 a8e4  ................
-000004e0: b880 e4b8 aae6 95b0 e68d aee5 ba93 e380  ................
-000004f0: 825c 6e5c 6ee5 afb9 e4ba 8ee6 95b0 e68d  .\n\n...........
-00000500: aee5 ad98 e582 a8e8 be83 e7ae 80e5 8d95  ................
-00000510: e79a 84e5 9cba e699 afef bc8c e68e a8e8  ................
-00000520: 8d90 e4bd bfe7 94a8 5b68 6530 3131 392f  ........[he0119/
-00000530: 6e6f 6e65 626f 742d 706c 7567 696e 2d64  nonebot-plugin-d
-00000540: 6174 6173 746f 7265 5d28 6874 7470 733a  atastore](https:
-00000550: 2f2f 6769 7468 7562 2e63 6f6d 2f68 6530  //github.com/he0
-00000560: 3131 392f 6e6f 6e65 626f 742d 706c 7567  119/nonebot-plug
-00000570: 696e 2d64 6174 6173 746f 7265 295c 6e5c  in-datastore)\n\
-00000580: 6e23 2320 4765 7420 5374 6172 7465 645c  n## Get Started\
-00000590: 6e5c 6e23 2323 2031 e380 81e5 ae9a e4b9  n\n### 1........
-000005a0: 8964 6174 615f 736f 7572 6365 5c6e 5c6e  .data_source\n\n
-000005b0: 6060 6070 7974 686f 6e5c 6e66 726f 6d20  ```python\nfrom 
-000005c0: 6e6f 6e65 626f 7420 696d 706f 7274 2067  nonebot import g
-000005d0: 6574 5f64 7269 7665 722c 2072 6571 7569  et_driver, requi
-000005e0: 7265 5c6e 5c6e 2320 e6b3 a8e6 848f e5bf  re\n\n# ........
-000005f0: 85e9 a1bb e585 8872 6571 7569 7265 e586  .......require..
-00000600: 8d69 6d70 6f72 745c 6e72 6571 7569 7265  .import\nrequire
-00000610: 2822 6e6f 6e65 626f 745f 706c 7567 696e  ("nonebot_plugin
-00000620: 5f73 716c 616c 6368 656d 7922 295c 6e66  _sqlalchemy")\nf
-00000630: 726f 6d20 6e6f 6e65 626f 745f 706c 7567  rom nonebot_plug
-00000640: 696e 5f73 716c 616c 6368 656d 7920 696d  in_sqlalchemy im
-00000650: 706f 7274 2044 6174 6153 6f75 7263 655c  port DataSource\
-00000660: 6e5c 6e23 20e5 bf85 e9a1 bbe4 bdbf e794  n\n# ...........
-00000670: a8e6 94af e68c 8161 7379 6e63 696f e79a  .......asyncio..
-00000680: 84e9 a9b1 e58a a8e5 99a8 5c6e 6462 5f63  ..........\ndb_c
-00000690: 6f6e 6e5f 7572 6c20 3d20 2270 6f73 7467  onn_url = "postg
-000006a0: 7265 7371 6c2b 6173 796e 6370 673a 2f2f  resql+asyncpg://
-000006b0: 7573 6572 6e61 6d65 3a70 6173 7377 6f72  username:passwor
-000006c0: 6440 6c6f 6361 6c68 6f73 743a 3534 3332  d@localhost:5432
-000006d0: 2f64 6174 6162 6173 6522 5c6e 6461 7461  /database"\ndata
-000006e0: 5f73 6f75 7263 6520 3d20 4461 7461 536f  _source = DataSo
-000006f0: 7572 6365 2867 6574 5f64 7269 7665 7228  urce(get_driver(
-00000700: 292c 2064 625f 636f 6e6e 5f75 726c 295c  ), db_conn_url)\
-00000710: 6e60 6060 5c6e 5c6e 2323 2320 32e3 8081  n```\n\n### 2...
-00000720: e5ae 9ae4 b989 e698 a0e5 b084 5c6e 6060  ............\n``
-00000730: 6070 7974 686f 6e5c 6e66 726f 6d20 7371  `python\nfrom sq
-00000740: 6c61 6c63 6865 6d79 2e6f 726d 2069 6d70  lalchemy.orm imp
-00000750: 6f72 7420 6d61 7070 6564 5f63 6f6c 756d  ort mapped_colum
-00000760: 6e5c 6e5c 6e40 6461 7461 5f73 6f75 7263  n\n\n@data_sourc
-00000770: 652e 7265 6769 7374 7279 2e6d 6170 7065  e.registry.mappe
-00000780: 645c 6e63 6c61 7373 2055 7365 724f 726d  d\nclass UserOrm
-00000790: 3a5c 6e20 2020 205f 5f74 6162 6c65 6e61  :\n    __tablena
-000007a0: 6d65 5f5f 203d 205c 2775 7365 7273 5c27  me__ = \'users\'
-000007b0: 5c6e 5c6e 2020 2020 6964 3a20 696e 7420  \n\n    id: int 
-000007c0: 3d20 6d61 7070 6564 5f63 6f6c 756d 6e28  = mapped_column(
-000007d0: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
-000007e0: 2c20 6175 746f 696e 6372 656d 656e 743d  , autoincrement=
-000007f0: 5472 7565 295c 6e20 2020 2075 7365 726e  True)\n    usern
-00000800: 616d 653a 2073 7472 5c6e 2020 2020 7061  ame: str\n    pa
-00000810: 7373 776f 7264 3a20 7374 725c 6e20 2020  ssword: str\n   
-00000820: 206e 6963 6b6e 616d 653a 2073 7472 5c6e   nickname: str\n
-00000830: 6060 605c 6e5c 6e23 2323 2033 e380 81e5  ```\n\n### 3....
-00000840: 9ca8 4d61 7463 6865 72e4 b8ad e4bd bfe7  ..Matcher.......
-00000850: 94a8 5c6e 5c6e 6060 6070 7974 686f 6e5c  ..\n\n```python\
-00000860: 6e66 726f 6d20 6e6f 6e65 626f 7420 696d  nfrom nonebot im
-00000870: 706f 7274 206f 6e5f 636f 6d6d 616e 645c  port on_command\
-00000880: 6e66 726f 6d20 6e6f 6e65 626f 742e 6164  nfrom nonebot.ad
-00000890: 6170 7465 7273 2e6f 6e65 626f 742e 7631  apters.onebot.v1
-000008a0: 3120 696d 706f 7274 204d 6573 7361 6765  1 import Message
-000008b0: 4576 656e 745c 6e66 726f 6d20 6e6f 6e65  Event\nfrom none
-000008c0: 626f 742e 696e 7465 726e 616c 2e6d 6174  bot.internal.mat
-000008d0: 6368 6572 2069 6d70 6f72 7420 4d61 7463  cher import Matc
-000008e0: 6865 725c 6e66 726f 6d20 7371 6c61 6c63  her\nfrom sqlalc
-000008f0: 6865 6d79 2069 6d70 6f72 7420 7365 6c65  hemy import sele
-00000900: 6374 5c6e 5c6e 6c6f 6769 6e5f 6d61 7463  ct\n\nlogin_matc
-00000910: 6865 7220 3d20 6f6e 5f63 6f6d 6d61 6e64  her = on_command
-00000920: 2822 6c6f 6769 6e22 295c 6e5c 6e5c 6e40  ("login")\n\n\n@
-00000930: 6c6f 6769 6e5f 6d61 7463 6865 722e 6861  login_matcher.ha
-00000940: 6e64 6c65 2829 5c6e 6173 796e 6320 6465  ndle()\nasync de
-00000950: 6620 6861 6e64 6c65 7228 6576 656e 743a  f handler(event:
-00000960: 204d 6573 7361 6765 4576 656e 742c 206d   MessageEvent, m
-00000970: 6174 6368 6572 3a20 4d61 7463 6865 7229  atcher: Matcher)
-00000980: 3a5c 6e20 2020 2075 7365 726e 616d 652c  :\n    username,
-00000990: 2070 6173 7377 6f72 6420 3d20 6576 656e   password = even
-000009a0: 742e 6765 745f 706c 6169 6e74 6578 7428  t.get_plaintext(
-000009b0: 292e 7370 6c69 7428 2220 2229 5c6e 5c6e  ).split(" ")\n\n
-000009c0: 2020 2020 7365 7373 696f 6e20 3d20 6461      session = da
-000009d0: 7461 5f73 6f75 7263 652e 7365 7373 696f  ta_source.sessio
-000009e0: 6e28 295c 6e20 2020 205c 6e20 2020 2073  n()\n    \n    s
-000009f0: 746d 7420 3d20 7365 6c65 6374 2855 7365  tmt = select(Use
-00000a00: 724f 726d 292e 7768 6572 6528 5573 6572  rOrm).where(User
-00000a10: 4f72 6d2e 7573 6572 6e61 6d65 203d 3d20  Orm.username == 
-00000a20: 7573 6572 6e61 6d65 2c20 5573 6572 4f72  username, UserOr
-00000a30: 6d2e 7061 7373 776f 7264 203d 3d20 7061  m.password == pa
-00000a40: 7373 776f 7264 295c 6e20 2020 2072 6573  ssword)\n    res
-00000a50: 756c 7420 3d20 6177 6169 7420 7365 7373  ult = await sess
-00000a60: 696f 6e2e 6578 6563 7574 6528 7374 6d74  ion.execute(stmt
-00000a70: 295c 6e20 2020 2075 7365 7220 3d20 7265  )\n    user = re
-00000a80: 7375 6c74 2e73 6361 6c61 725f 6f6e 655f  sult.scalar_one_
-00000a90: 6f72 5f6e 6f6e 6528 295c 6e5c 6e20 2020  or_none()\n\n   
-00000aa0: 2069 6620 7573 6572 2069 7320 6e6f 7420   if user is not 
-00000ab0: 4e6f 6e65 3a5c 6e20 2020 2020 2020 2061  None:\n        a
-00000ac0: 7761 6974 206d 6174 6368 6572 2e73 656e  wait matcher.sen
-00000ad0: 6428 6622 4865 6c6c 6f2c 207b 7573 6572  d(f"Hello, {user
-00000ae0: 2e6e 6963 6b6e 616d 657d 2229 5c6e 6060  .nickname}")\n``
-00000af0: 605c 6e5c 6ee9 809a e8bf 8760 6461 7461  `\n\n......`data
-00000b00: 5f73 6f75 7263 652e 7365 7373 696f 6e28  _source.session(
-00000b10: 2960 e88e b7e5 8f96 4173 796e 6353 6573  )`......AsyncSes
-00000b20: 7369 6f6e e5af b9e8 b1a1 efbc 8ce6 ada4  sion............
-00000b30: e5a4 84e8 8eb7 e58f 96e7 9a84 7365 7373  ............sess
-00000b40: 696f 6ee5 ae9e e999 85e4 b88a e698 af61  ion............a
-00000b50: 7379 6e63 5f73 636f 7065 645f 7365 7373  sync_scoped_sess
-00000b60: 696f 6ee3 8082 5c6e 5c6e e59c a84d 6174  ion...\n\n...Mat
-00000b70: 6368 6572 e79a 84e4 b880 e6ac a1e6 89a7  cher............
-00000b80: e8a1 8ce8 bf87 e7a8 8be4 b8ad efbc 8ce5  ................
-00000b90: a49a e6ac a1e8 b083 e794 a860 6461 7461  ...........`data
-00000ba0: 5f73 6f75 7263 652e 7365 7373 696f 6e28  _source.session(
-00000bb0: 2960 e88e b7e5 be97 e79a 84e6 98af e590  )`..............
-00000bc0: 8ce4 b880 e4b8 aa73 6573 7369 6f6e efbc  .......session..
-00000bd0: 8ce5 b9b6 e4b8 94e4 bc9a e59c a84d 6174  .............Mat
-00000be0: 6368 6572 e689 a7e8 a18c e5ae 8ce6 af95  cher............
-00000bf0: e590 8ee8 87aa e58a a8e5 85b3 e997 ade3  ................
-00000c00: 8082 e4b9 9fe5 b0b1 e698 afe8 afb4 e688  ................
-00000c10: 91e4 bbac e58f afe4 bba5 e583 8fe4 b88b  ................
-00000c20: e99d a2e8 bf99 e6a0 b7e4 bdbf e794 a8ef  ................
-00000c30: bc9a 5c6e 5c6e 6060 6070 7974 686f 6e5c  ..\n\n```python\
-00000c40: 6e66 726f 6d20 6e6f 6e65 626f 7420 696d  nfrom nonebot im
-00000c50: 706f 7274 206f 6e5f 636f 6d6d 616e 645c  port on_command\
-00000c60: 6e66 726f 6d20 6e6f 6e65 626f 742e 6164  nfrom nonebot.ad
-00000c70: 6170 7465 7273 2e6f 6e65 626f 742e 7631  apters.onebot.v1
-00000c80: 3120 696d 706f 7274 204d 6573 7361 6765  1 import Message
-00000c90: 4576 656e 745c 6e66 726f 6d20 6e6f 6e65  Event\nfrom none
-00000ca0: 626f 742e 696e 7465 726e 616c 2e6d 6174  bot.internal.mat
-00000cb0: 6368 6572 2069 6d70 6f72 7420 4d61 7463  cher import Matc
-00000cc0: 6865 725c 6e66 726f 6d20 7371 6c61 6c63  her\nfrom sqlalc
-00000cd0: 6865 6d79 2069 6d70 6f72 7420 7365 6c65  hemy import sele
-00000ce0: 6374 5c6e 6672 6f6d 2074 7970 696e 6720  ct\nfrom typing 
-00000cf0: 696d 706f 7274 204f 7074 696f 6e61 6c5c  import Optional\
-00000d00: 6e5c 6e61 7379 6e63 2064 6566 206c 6f67  n\nasync def log
-00000d10: 696e 2875 7365 726e 616d 653a 2073 7472  in(username: str
-00000d20: 2c20 7061 7373 776f 7264 3a20 7374 7229  , password: str)
-00000d30: 202d 3e20 4f70 7469 6f6e 616c 5b55 7365   -> Optional[Use
-00000d40: 725d 3a5c 6e20 2020 2073 6573 7369 6f6e  r]:\n    session
-00000d50: 203d 2064 6174 615f 736f 7572 6365 2e73   = data_source.s
-00000d60: 6573 7369 6f6e 2829 5c6e 2020 2020 5c6e  ession()\n    \n
-00000d70: 2020 2020 7374 6d74 203d 2073 656c 6563      stmt = selec
-00000d80: 7428 5573 6572 4f72 6d29 2e77 6865 7265  t(UserOrm).where
-00000d90: 2855 7365 724f 726d 2e75 7365 726e 616d  (UserOrm.usernam
-00000da0: 6520 3d3d 2075 7365 726e 616d 652c 2055  e == username, U
-00000db0: 7365 724f 726d 2e70 6173 7377 6f72 6420  serOrm.password 
-00000dc0: 3d3d 2070 6173 7377 6f72 6429 5c6e 2020  == password)\n  
-00000dd0: 2020 7265 7375 6c74 203d 2061 7761 6974    result = await
-00000de0: 2073 6573 7369 6f6e 2e65 7865 6375 7465   session.execute
-00000df0: 2873 746d 7429 5c6e 2020 2020 7573 6572  (stmt)\n    user
-00000e00: 203d 2072 6573 756c 742e 7363 616c 6172   = result.scalar
-00000e10: 5f6f 6e65 5f6f 725f 6e6f 6e65 2829 5c6e  _one_or_none()\n
-00000e20: 5c6e 2020 2020 7265 7475 726e 2075 7365  \n    return use
-00000e30: 725c 6e5c 6e5c 6e6c 6f67 696e 5f6d 6174  r\n\n\nlogin_mat
-00000e40: 6368 6572 203d 206f 6e5f 636f 6d6d 616e  cher = on_comman
-00000e50: 6428 226c 6f67 696e 2229 5c6e 5c6e 5c6e  d("login")\n\n\n
-00000e60: 406c 6f67 696e 5f6d 6174 6368 6572 2e68  @login_matcher.h
-00000e70: 616e 646c 6528 295c 6e61 7379 6e63 2064  andle()\nasync d
-00000e80: 6566 2068 616e 646c 6572 2865 7665 6e74  ef handler(event
-00000e90: 3a20 4d65 7373 6167 6545 7665 6e74 2c20  : MessageEvent, 
-00000ea0: 6d61 7463 6865 723a 204d 6174 6368 6572  matcher: Matcher
-00000eb0: 293a 5c6e 2020 2020 7573 6572 6e61 6d65  ):\n    username
-00000ec0: 2c20 7061 7373 776f 7264 203d 2065 7665  , password = eve
-00000ed0: 6e74 2e67 6574 5f70 6c61 696e 7465 7874  nt.get_plaintext
-00000ee0: 2829 2e73 706c 6974 2822 2022 295c 6e20  ().split(" ")\n 
-00000ef0: 2020 2075 7365 7220 3d20 6177 6169 7420     user = await 
-00000f00: 6c6f 6769 6e28 7573 6572 6e61 6d65 2c20  login(username, 
-00000f10: 7061 7373 776f 7264 295c 6e20 2020 2069  password)\n    i
-00000f20: 6620 7573 6572 2069 7320 6e6f 7420 4e6f  f user is not No
-00000f30: 6e65 3a5c 6e20 2020 2020 2020 2061 7761  ne:\n        awa
-00000f40: 6974 206d 6174 6368 6572 2e73 656e 6428  it matcher.send(
-00000f50: 6622 4865 6c6c 6f2c 207b 7573 6572 2e6e  f"Hello, {user.n
-00000f60: 6963 6b6e 616d 657d 2229 5c6e 6060 605c  ickname}")\n```\
-00000f70: 6e5c 6ee5 8f82 e880 83ef bc9a 6874 7470  n\n.........http
-00000f80: 733a 2f2f 646f 6373 2e73 716c 616c 6368  s://docs.sqlalch
-00000f90: 656d 792e 6f72 672f 656e 2f31 342f 6f72  emy.org/en/14/or
-00000fa0: 6d2f 6578 7465 6e73 696f 6e73 2f61 7379  m/extensions/asy
-00000fb0: 6e63 696f 2e68 746d 6c23 7573 696e 672d  ncio.html#using-
-00000fc0: 6173 796e 6369 6f2d 7363 6f70 6564 2d73  asyncio-scoped-s
-00000fd0: 6573 7369 6f6e 5c6e 5c6e e6b3 a8e6 848f  ession\n\n......
-00000fe0: efbc 9ae5 8aa1 e5bf 85e4 bf9d e8af 81e4  ................
-00000ff0: b880 e6ac a14d 6174 6368 6572 e689 a7e8  .....Matcher....
-00001000: a18c e8bf 87e7 a88b e4b8 8de4 bc9a e59c  ................
-00001010: a8e4 b88d e590 8ce7 9a84 5461 736b e4b8  ..........Task..
-00001020: ade8 b083 e794 a860 6461 7461 5f73 6f75  .......`data_sou
-00001030: 7263 652e 7365 7373 696f 6e28 2960 e88e  rce.session()`..
-00001040: b7e5 8f96 7365 7373 696f 6eef bc88 e58d  ....session.....
-00001050: b3e4 b88d e8a6 81e4 bdbf e794 a860 6372  .............`cr
-00001060: 6561 7465 5f74 6173 6b28 2960 e688 9660  eate_task()`...`
-00001070: 656e 7375 7265 5f66 7574 7572 6528 2960  ensure_future()`
-00001080: e588 9be5 bbba 5461 736b efbc 89ef bc8c  ......Task......
-00001090: e590 a6e5 8899 e58f afe8 83bd e587 bae7  ................
-000010a0: 8eb0 e994 99e8 afaf e380 82e8 8ba5 e69c  ................
-000010b0: 89e8 bf99 e6a0 b7e7 9a84 e99c 80e6 b182  ................
-000010c0: efbc 8ce8 afb7 e58f 82e8 8083 e4b8 8be6  ................
-000010d0: 9687 e79a 84e6 96b9 e6b3 95e6 898b e58a  ................
-000010e0: a8e5 889b e5bb bae5 b9b6 e7ae a1e7 9086  ................
-000010f0: 7365 7373 696f 6ee3 8082 5c6e 5c6e 5c6e  session...\n\n\n
-00001100: 2323 2320 34e3 8081 e59c a84d 6174 6368  ### 4......Match
-00001110: 6572 e4b9 8be5 a496 e4bd bfe7 94a8 5c6e  er............\n
-00001120: 5c6e e59c a84d 6174 6368 6572 e4b9 8be5  \n...Matcher....
-00001130: a496 efbc 88e5 a682 6f6e 5f62 6f74 5f63  ........on_bot_c
-00001140: 6f6e 6e65 6374 e7ad 89e9 92a9 e5ad 90e5  onnect..........
-00001150: 87bd e695 b0e4 b8ad efbc 8ce6 8896 e880  ................
-00001160: 85e6 98af 4150 5363 6865 6475 6c65 72e7  ....APScheduler.
-00001170: 9a84 e5ae 9ae6 97b6 e4bb bbe5 8aa1 e4b8  ................
-00001180: adef bc89 e588 99e5 bf85 e9a1 bbe9 809a  ................
-00001190: e8bf 8760 4173 796e 6353 6573 7369 6f6e  ...`AsyncSession
-000011a0: 2864 6174 615f 736f 7572 6365 2e65 6e67  (data_source.eng
-000011b0: 696e 6529 60e5 889b e5bb ba73 6573 7369  ine)`......sessi
-000011c0: 6f6e e380 825c 6e5c 6e60 6060 7079 7468  on...\n\n```pyth
-000011d0: 6f6e 5c6e 6173 796e 6320 6465 6620 646f  on\nasync def do
-000011e0: 5f73 6f6d 6574 6869 6e67 2829 3a5c 6e20  _something():\n 
-000011f0: 2020 2061 7379 6e63 2077 6974 6820 4173     async with As
-00001200: 796e 6353 6573 7369 6f6e 2864 6174 615f  yncSession(data_
-00001210: 736f 7572 6365 2e65 6e67 696e 6529 2061  source.engine) a
-00001220: 7320 7365 7373 696f 6e3a 5c6e 2020 2020  s session:\n    
-00001230: 2020 2020 2320 2e2e 2e5c 6e60 6060 5c6e      # ...\n```\n
-00001240: 272c 0a20 2020 2027 6175 7468 6f72 273a  ',.    'author':
-00001250: 2027 7373 7474 6b6b 6c27 2c0a 2020 2020   'ssttkkl',.    
-00001260: 2761 7574 686f 725f 656d 6169 6c27 3a20  'author_email': 
-00001270: 2768 7561 6e67 2e77 656e 2e6c 6f6e 6740  'huang.wen.long@
-00001280: 686f 746d 6169 6c2e 636f 6d27 2c0a 2020  hotmail.com',.  
-00001290: 2020 276d 6169 6e74 6169 6e65 7227 3a20    'maintainer': 
-000012a0: 274e 6f6e 6527 2c0a 2020 2020 276d 6169  'None',.    'mai
-000012b0: 6e74 6169 6e65 725f 656d 6169 6c27 3a20  ntainer_email': 
-000012c0: 274e 6f6e 6527 2c0a 2020 2020 2775 726c  'None',.    'url
-000012d0: 273a 2027 6874 7470 733a 2f2f 6769 7468  ': 'https://gith
-000012e0: 7562 2e63 6f6d 2f73 7374 746b 6b6c 2f6e  ub.com/ssttkkl/n
-000012f0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 7371  onebot-plugin-sq
-00001300: 6c61 6c63 6865 6d79 272c 0a20 2020 2027  lalchemy',.    '
-00001310: 7061 636b 6167 655f 6469 7227 3a20 7061  package_dir': pa
-00001320: 636b 6167 655f 6469 722c 0a20 2020 2027  ckage_dir,.    '
-00001330: 7061 636b 6167 6573 273a 2070 6163 6b61  packages': packa
-00001340: 6765 732c 0a20 2020 2027 7061 636b 6167  ges,.    'packag
-00001350: 655f 6461 7461 273a 2070 6163 6b61 6765  e_data': package
-00001360: 5f64 6174 612c 0a20 2020 2027 696e 7374  _data,.    'inst
-00001370: 616c 6c5f 7265 7175 6972 6573 273a 2069  all_requires': i
-00001380: 6e73 7461 6c6c 5f72 6571 7569 7265 732c  nstall_requires,
-00001390: 0a20 2020 2027 7079 7468 6f6e 5f72 6571  .    'python_req
-000013a0: 7569 7265 7327 3a20 273e 3d33 2e39 2c3c  uires': '>=3.9,<
-000013b0: 342e 3027 2c0a 7d0a 0a0a 7365 7475 7028  4.0',.}...setup(
-000013c0: 2a2a 7365 7475 705f 6b77 6172 6773 290a  **setup_kwargs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6e6f 6e65  : 2.1.Name: none
+00000020: 626f 742d 706c 7567 696e 2d73 716c 616c  bot-plugin-sqlal
+00000030: 6368 656d 790a 5665 7273 696f 6e3a 2030  chemy.Version: 0
+00000040: 2e32 2e31 0a53 756d 6d61 7279 3a20 0a48  .2.1.Summary: .H
+00000050: 6f6d 652d 7061 6765 3a20 6874 7470 733a  ome-page: https:
+00000060: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7374  //github.com/sst
+00000070: 746b 6b6c 2f6e 6f6e 6562 6f74 2d70 6c75  tkkl/nonebot-plu
+00000080: 6769 6e2d 7371 6c61 6c63 6865 6d79 0a4c  gin-sqlalchemy.L
+00000090: 6963 656e 7365 3a20 4d49 540a 4175 7468  icense: MIT.Auth
+000000a0: 6f72 3a20 7373 7474 6b6b 6c0a 4175 7468  or: ssttkkl.Auth
+000000b0: 6f72 2d65 6d61 696c 3a20 6875 616e 672e  or-email: huang.
+000000c0: 7765 6e2e 6c6f 6e67 4068 6f74 6d61 696c  wen.long@hotmail
+000000d0: 2e63 6f6d 0a52 6571 7569 7265 732d 5079  .com.Requires-Py
+000000e0: 7468 6f6e 3a20 3e3d 332e 392c 3c34 2e30  thon: >=3.9,<4.0
+000000f0: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+00000100: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000110: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+00000120: 6e73 650a 436c 6173 7369 6669 6572 3a20  nse.Classifier: 
+00000130: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000140: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000150: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
+00000160: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000170: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000180: 3a20 332e 390a 436c 6173 7369 6669 6572  : 3.9.Classifier
+00000190: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000001a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001b0: 203a 3a20 332e 3130 0a43 6c61 7373 6966   :: 3.10.Classif
+000001c0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000001d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001e0: 686f 6e20 3a3a 2033 2e31 310a 5265 7175  hon :: 3.11.Requ
+000001f0: 6972 6573 2d44 6973 743a 206e 6f6e 6562  ires-Dist: noneb
+00000200: 6f74 3220 283e 3d32 2e30 2e30 2d72 632e  ot2 (>=2.0.0-rc.
+00000210: 332c 3c33 2e30 2e30 290a 5265 7175 6972  3,<3.0.0).Requir
+00000220: 6573 2d44 6973 743a 2073 716c 616c 6368  es-Dist: sqlalch
+00000230: 656d 795b 6173 796e 6369 6f5d 2028 3e3d  emy[asyncio] (>=
+00000240: 322e 302e 302c 3c33 2e30 2e30 290a 5072  2.0.0,<3.0.0).Pr
+00000250: 6f6a 6563 742d 5552 4c3a 2052 6570 6f73  oject-URL: Repos
+00000260: 6974 6f72 792c 2068 7474 7073 3a2f 2f67  itory, https://g
+00000270: 6974 6875 622e 636f 6d2f 7373 7474 6b6b  ithub.com/ssttkk
+00000280: 6c2f 6e6f 6e65 626f 742d 706c 7567 696e  l/nonebot-plugin
+00000290: 2d73 716c 616c 6368 656d 790a 4465 7363  -sqlalchemy.Desc
+000002a0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+000002b0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
+000002c0: 0a0a 3c21 2d2d 206d 6172 6b64 6f77 6e6c  ..<!-- markdownl
+000002d0: 696e 742d 6469 7361 626c 6520 4d44 3033  int-disable MD03
+000002e0: 3320 4d44 3033 3620 4d44 3034 3120 2d2d  3 MD036 MD041 --
+000002f0: 3e0a 0a3c 7020 616c 6967 6e3d 2263 656e  >..<p align="cen
+00000300: 7465 7222 3e0a 2020 3c61 2068 7265 663d  ter">.  <a href=
+00000310: 2268 7474 7073 3a2f 2f76 322e 6e6f 6e65  "https://v2.none
+00000320: 626f 742e 6465 762f 223e 3c69 6d67 2073  bot.dev/"><img s
+00000330: 7263 3d22 6874 7470 733a 2f2f 7632 2e6e  rc="https://v2.n
+00000340: 6f6e 6562 6f74 2e64 6576 2f6c 6f67 6f2e  onebot.dev/logo.
+00000350: 706e 6722 2077 6964 7468 3d22 3230 3022  png" width="200"
+00000360: 2068 6569 6768 743d 2232 3030 2220 616c   height="200" al
+00000370: 743d 226e 6f6e 6562 6f74 223e 3c2f 613e  t="nonebot"></a>
+00000380: 0a3c 2f70 3e0a 0a3c 6469 7620 616c 6967  .</p>..<div alig
+00000390: 6e3d 2263 656e 7465 7222 3e0a 0a6e 6f6e  n="center">..non
+000003a0: 6562 6f74 2d70 6c75 6769 6e2d 7371 6c61  ebot-plugin-sqla
+000003b0: 6c63 6865 6d79 0a3d 3d3d 3d3d 3d3d 3d3d  lchemy.=========
+000003c0: 3d3d 3d0a 0a5f e29c a820 4e6f 6e65 426f  ===.._... NoneBo
+000003d0: 7420 5351 4c41 6c63 6865 6d79 20e5 b081  t SQLAlchemy ...
+000003e0: e8a3 85e6 8f92 e4bb b620 e29c a85f 0a0a  ......... ..._..
+000003f0: 3c2f 6469 763e 0a0a 3c70 2061 6c69 676e  </div>..<p align
+00000400: 3d22 6365 6e74 6572 223e 0a20 203c 6120  ="center">.  <a 
+00000410: 6872 6566 3d22 6874 7470 733a 2f2f 7261  href="https://ra
+00000420: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00000430: 656e 742e 636f 6d2f 7373 7474 6b6b 6c2f  ent.com/ssttkkl/
+00000440: 6e6f 6e65 626f 742d 706c 7567 696e 2d73  nonebot-plugin-s
+00000450: 716c 616c 6368 656d 792f 6d61 7374 6572  qlalchemy/master
+00000460: 2f4c 4943 454e 5345 223e 0a20 2020 203c  /LICENSE">.    <
+00000470: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000480: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000490: 6769 7468 7562 2f6c 6963 656e 7365 2f73  github/license/s
+000004a0: 7374 746b 6b6c 2f6e 6f6e 6562 6f74 2d70  sttkkl/nonebot-p
+000004b0: 6c75 6769 6e2d 7371 6c61 6c63 6865 6d79  lugin-sqlalchemy
+000004c0: 2e73 7667 2220 616c 743d 226c 6963 656e  .svg" alt="licen
+000004d0: 7365 223e 0a20 203c 2f61 3e0a 2020 3c61  se">.  </a>.  <a
+000004e0: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+000004f0: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
+00000500: 7970 692f 6e6f 6e65 626f 742d 706c 7567  ypi/nonebot-plug
+00000510: 696e 2d73 716c 616c 6368 656d 7922 3e0a  in-sqlalchemy">.
+00000520: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000530: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000540: 732e 696f 2f70 7970 692f 762f 6e6f 6e65  s.io/pypi/v/none
+00000550: 626f 742d 706c 7567 696e 2d73 716c 616c  bot-plugin-sqlal
+00000560: 6368 656d 792e 7376 6722 2061 6c74 3d22  chemy.svg" alt="
+00000570: 7079 7069 223e 0a20 203c 2f61 3e0a 2020  pypi">.  </a>.  
+00000580: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000590: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000005a0: 2f62 6164 6765 2f70 7974 686f 6e2d 332e  /badge/python-3.
+000005b0: 392b 2d62 6c75 652e 7376 6722 2061 6c74  9+-blue.svg" alt
+000005c0: 3d22 7079 7468 6f6e 223e 0a3c 2f70 3e0a  ="python">.</p>.
+000005d0: 0ae4 b8ba e68f 92e4 bbb6 e5b0 81e8 a385  ................
+000005e0: 5351 4c41 6c63 6865 6d79 e695 b0e6 8dae  SQLAlchemy......
+000005f0: e5ba 93e8 aebf e997 aeef bc8c e4b8 80e4  ................
+00000600: b8aa e68f 92e4 bbb6 e4bd bfe7 94a8 e4b8  ................
+00000610: 80e4 b8aa e695 b0e6 8dae e5ba 93e3 8082  ................
+00000620: 0a0a e5af b9e4 ba8e e695 b0e6 8dae e5ad  ................
+00000630: 98e5 82a8 e8be 83e7 ae80 e58d 95e7 9a84  ................
+00000640: e59c bae6 99af efbc 8ce6 8ea8 e88d 90e4  ................
+00000650: bdbf e794 a85b 6865 3031 3139 2f6e 6f6e  .....[he0119/non
+00000660: 6562 6f74 2d70 6c75 6769 6e2d 6461 7461  ebot-plugin-data
+00000670: 7374 6f72 655d 2868 7474 7073 3a2f 2f67  store](https://g
+00000680: 6974 6875 622e 636f 6d2f 6865 3031 3139  ithub.com/he0119
+00000690: 2f6e 6f6e 6562 6f74 2d70 6c75 6769 6e2d  /nonebot-plugin-
+000006a0: 6461 7461 7374 6f72 6529 0a0a 2323 2047  datastore)..## G
+000006b0: 6574 2053 7461 7274 6564 0a0a 2323 2320  et Started..### 
+000006c0: 31e3 8081 e5ae 9ae4 b989 6461 7461 5f73  1.........data_s
+000006d0: 6f75 7263 650a 0a60 6060 7079 7468 6f6e  ource..```python
+000006e0: 0a66 726f 6d20 6e6f 6e65 626f 7420 696d  .from nonebot im
+000006f0: 706f 7274 2067 6574 5f64 7269 7665 722c  port get_driver,
+00000700: 2072 6571 7569 7265 0a0a 2320 e6b3 a8e6   require..# ....
+00000710: 848f e5bf 85e9 a1bb e585 8872 6571 7569  ...........requi
+00000720: 7265 e586 8d69 6d70 6f72 740a 7265 7175  re...import.requ
+00000730: 6972 6528 226e 6f6e 6562 6f74 5f70 6c75  ire("nonebot_plu
+00000740: 6769 6e5f 7371 6c61 6c63 6865 6d79 2229  gin_sqlalchemy")
+00000750: 0a66 726f 6d20 6e6f 6e65 626f 745f 706c  .from nonebot_pl
+00000760: 7567 696e 5f73 716c 616c 6368 656d 7920  ugin_sqlalchemy 
+00000770: 696d 706f 7274 2044 6174 6153 6f75 7263  import DataSourc
+00000780: 650a 0a23 20e5 bf85 e9a1 bbe4 bdbf e794  e..# ...........
+00000790: a8e6 94af e68c 8161 7379 6e63 696f e79a  .......asyncio..
+000007a0: 84e9 a9b1 e58a a8e5 99a8 0a64 625f 636f  ...........db_co
+000007b0: 6e6e 5f75 726c 203d 2022 706f 7374 6772  nn_url = "postgr
+000007c0: 6573 716c 2b61 7379 6e63 7067 3a2f 2f75  esql+asyncpg://u
+000007d0: 7365 726e 616d 653a 7061 7373 776f 7264  sername:password
+000007e0: 406c 6f63 616c 686f 7374 3a35 3433 322f  @localhost:5432/
+000007f0: 6461 7461 6261 7365 220a 6461 7461 5f73  database".data_s
+00000800: 6f75 7263 6520 3d20 4461 7461 536f 7572  ource = DataSour
+00000810: 6365 2867 6574 5f64 7269 7665 7228 292c  ce(get_driver(),
+00000820: 2064 625f 636f 6e6e 5f75 726c 290a 6060   db_conn_url).``
+00000830: 600a 0a23 2323 2032 e380 81e5 ae9a e4b9  `..### 2........
+00000840: 89e6 98a0 e5b0 840a 6060 6070 7974 686f  ........```pytho
+00000850: 6e0a 6672 6f6d 2073 716c 616c 6368 656d  n.from sqlalchem
+00000860: 792e 6f72 6d20 696d 706f 7274 206d 6170  y.orm import map
+00000870: 7065 645f 636f 6c75 6d6e 0a0a 4064 6174  ped_column..@dat
+00000880: 615f 736f 7572 6365 2e72 6567 6973 7472  a_source.registr
+00000890: 792e 6d61 7070 6564 0a63 6c61 7373 2055  y.mapped.class U
+000008a0: 7365 724f 726d 3a0a 2020 2020 5f5f 7461  serOrm:.    __ta
+000008b0: 626c 656e 616d 655f 5f20 3d20 2775 7365  blename__ = 'use
+000008c0: 7273 270a 0a20 2020 2069 643a 2069 6e74  rs'..    id: int
+000008d0: 203d 206d 6170 7065 645f 636f 6c75 6d6e   = mapped_column
+000008e0: 2870 7269 6d61 7279 5f6b 6579 3d54 7275  (primary_key=Tru
+000008f0: 652c 2061 7574 6f69 6e63 7265 6d65 6e74  e, autoincrement
+00000900: 3d54 7275 6529 0a20 2020 2075 7365 726e  =True).    usern
+00000910: 616d 653a 2073 7472 0a20 2020 2070 6173  ame: str.    pas
+00000920: 7377 6f72 643a 2073 7472 0a20 2020 206e  sword: str.    n
+00000930: 6963 6b6e 616d 653a 2073 7472 0a60 6060  ickname: str.```
+00000940: 0a0a 2323 2320 33e3 8081 e59c a84d 6174  ..### 3......Mat
+00000950: 6368 6572 e4b8 ade4 bdbf e794 a80a 0a60  cher...........`
+00000960: 6060 7079 7468 6f6e 0a66 726f 6d20 6e6f  ``python.from no
+00000970: 6e65 626f 7420 696d 706f 7274 206f 6e5f  nebot import on_
+00000980: 636f 6d6d 616e 640a 6672 6f6d 206e 6f6e  command.from non
+00000990: 6562 6f74 2e61 6461 7074 6572 732e 6f6e  ebot.adapters.on
+000009a0: 6562 6f74 2e76 3131 2069 6d70 6f72 7420  ebot.v11 import 
+000009b0: 4d65 7373 6167 6545 7665 6e74 0a66 726f  MessageEvent.fro
+000009c0: 6d20 6e6f 6e65 626f 742e 696e 7465 726e  m nonebot.intern
+000009d0: 616c 2e6d 6174 6368 6572 2069 6d70 6f72  al.matcher impor
+000009e0: 7420 4d61 7463 6865 720a 6672 6f6d 2073  t Matcher.from s
+000009f0: 716c 616c 6368 656d 7920 696d 706f 7274  qlalchemy import
+00000a00: 2073 656c 6563 740a 0a6c 6f67 696e 5f6d   select..login_m
+00000a10: 6174 6368 6572 203d 206f 6e5f 636f 6d6d  atcher = on_comm
+00000a20: 616e 6428 226c 6f67 696e 2229 0a0a 0a40  and("login")...@
+00000a30: 6c6f 6769 6e5f 6d61 7463 6865 722e 6861  login_matcher.ha
+00000a40: 6e64 6c65 2829 0a61 7379 6e63 2064 6566  ndle().async def
+00000a50: 2068 616e 646c 6572 2865 7665 6e74 3a20   handler(event: 
+00000a60: 4d65 7373 6167 6545 7665 6e74 2c20 6d61  MessageEvent, ma
+00000a70: 7463 6865 723a 204d 6174 6368 6572 293a  tcher: Matcher):
+00000a80: 0a20 2020 2075 7365 726e 616d 652c 2070  .    username, p
+00000a90: 6173 7377 6f72 6420 3d20 6576 656e 742e  assword = event.
+00000aa0: 6765 745f 706c 6169 6e74 6578 7428 292e  get_plaintext().
+00000ab0: 7370 6c69 7428 2220 2229 0a0a 2020 2020  split(" ")..    
+00000ac0: 7365 7373 696f 6e20 3d20 6461 7461 5f73  session = data_s
+00000ad0: 6f75 7263 652e 7365 7373 696f 6e28 290a  ource.session().
+00000ae0: 2020 2020 0a20 2020 2073 746d 7420 3d20      .    stmt = 
+00000af0: 7365 6c65 6374 2855 7365 724f 726d 292e  select(UserOrm).
+00000b00: 7768 6572 6528 5573 6572 4f72 6d2e 7573  where(UserOrm.us
+00000b10: 6572 6e61 6d65 203d 3d20 7573 6572 6e61  ername == userna
+00000b20: 6d65 2c20 5573 6572 4f72 6d2e 7061 7373  me, UserOrm.pass
+00000b30: 776f 7264 203d 3d20 7061 7373 776f 7264  word == password
+00000b40: 290a 2020 2020 7265 7375 6c74 203d 2061  ).    result = a
+00000b50: 7761 6974 2073 6573 7369 6f6e 2e65 7865  wait session.exe
+00000b60: 6375 7465 2873 746d 7429 0a20 2020 2075  cute(stmt).    u
+00000b70: 7365 7220 3d20 7265 7375 6c74 2e73 6361  ser = result.sca
+00000b80: 6c61 725f 6f6e 655f 6f72 5f6e 6f6e 6528  lar_one_or_none(
+00000b90: 290a 0a20 2020 2069 6620 7573 6572 2069  )..    if user i
+00000ba0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00000bb0: 2020 2020 6177 6169 7420 6d61 7463 6865      await matche
+00000bc0: 722e 7365 6e64 2866 2248 656c 6c6f 2c20  r.send(f"Hello, 
+00000bd0: 7b75 7365 722e 6e69 636b 6e61 6d65 7d22  {user.nickname}"
+00000be0: 290a 6060 600a 0ae9 809a e8bf 8760 6461  ).```........`da
+00000bf0: 7461 5f73 6f75 7263 652e 7365 7373 696f  ta_source.sessio
+00000c00: 6e28 2960 e88e b7e5 8f96 4173 796e 6353  n()`......AsyncS
+00000c10: 6573 7369 6f6e e5af b9e8 b1a1 efbc 8ce6  ession..........
+00000c20: ada4 e5a4 84e8 8eb7 e58f 96e7 9a84 7365  ..............se
+00000c30: 7373 696f 6ee5 ae9e e999 85e4 b88a e698  ssion...........
+00000c40: af61 7379 6e63 5f73 636f 7065 645f 7365  .async_scoped_se
+00000c50: 7373 696f 6ee3 8082 0a0a e59c a84d 6174  ssion........Mat
+00000c60: 6368 6572 e79a 84e4 b880 e6ac a1e6 89a7  cher............
+00000c70: e8a1 8ce8 bf87 e7a8 8be4 b8ad efbc 8ce5  ................
+00000c80: a49a e6ac a1e8 b083 e794 a860 6461 7461  ...........`data
+00000c90: 5f73 6f75 7263 652e 7365 7373 696f 6e28  _source.session(
+00000ca0: 2960 e88e b7e5 be97 e79a 84e6 98af e590  )`..............
+00000cb0: 8ce4 b880 e4b8 aa73 6573 7369 6f6e efbc  .......session..
+00000cc0: 8ce5 b9b6 e4b8 94e4 bc9a e59c a84d 6174  .............Mat
+00000cd0: 6368 6572 e689 a7e8 a18c e5ae 8ce6 af95  cher............
+00000ce0: e590 8ee8 87aa e58a a8e5 85b3 e997 ade3  ................
+00000cf0: 8082 e4b9 9fe5 b0b1 e698 afe8 afb4 e688  ................
+00000d00: 91e4 bbac e58f afe4 bba5 e583 8fe4 b88b  ................
+00000d10: e99d a2e8 bf99 e6a0 b7e4 bdbf e794 a8ef  ................
+00000d20: bc9a 0a0a 6060 6070 7974 686f 6e0a 6672  ....```python.fr
+00000d30: 6f6d 206e 6f6e 6562 6f74 2069 6d70 6f72  om nonebot impor
+00000d40: 7420 6f6e 5f63 6f6d 6d61 6e64 0a66 726f  t on_command.fro
+00000d50: 6d20 6e6f 6e65 626f 742e 6164 6170 7465  m nonebot.adapte
+00000d60: 7273 2e6f 6e65 626f 742e 7631 3120 696d  rs.onebot.v11 im
+00000d70: 706f 7274 204d 6573 7361 6765 4576 656e  port MessageEven
+00000d80: 740a 6672 6f6d 206e 6f6e 6562 6f74 2e69  t.from nonebot.i
+00000d90: 6e74 6572 6e61 6c2e 6d61 7463 6865 7220  nternal.matcher 
+00000da0: 696d 706f 7274 204d 6174 6368 6572 0a66  import Matcher.f
+00000db0: 726f 6d20 7371 6c61 6c63 6865 6d79 2069  rom sqlalchemy i
+00000dc0: 6d70 6f72 7420 7365 6c65 6374 0a66 726f  mport select.fro
+00000dd0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00000de0: 4f70 7469 6f6e 616c 0a0a 6173 796e 6320  Optional..async 
+00000df0: 6465 6620 6c6f 6769 6e28 7573 6572 6e61  def login(userna
+00000e00: 6d65 3a20 7374 722c 2070 6173 7377 6f72  me: str, passwor
+00000e10: 643a 2073 7472 2920 2d3e 204f 7074 696f  d: str) -> Optio
+00000e20: 6e61 6c5b 5573 6572 5d3a 0a20 2020 2073  nal[User]:.    s
+00000e30: 6573 7369 6f6e 203d 2064 6174 615f 736f  ession = data_so
+00000e40: 7572 6365 2e73 6573 7369 6f6e 2829 0a20  urce.session(). 
+00000e50: 2020 200a 2020 2020 7374 6d74 203d 2073     .    stmt = s
+00000e60: 656c 6563 7428 5573 6572 4f72 6d29 2e77  elect(UserOrm).w
+00000e70: 6865 7265 2855 7365 724f 726d 2e75 7365  here(UserOrm.use
+00000e80: 726e 616d 6520 3d3d 2075 7365 726e 616d  rname == usernam
+00000e90: 652c 2055 7365 724f 726d 2e70 6173 7377  e, UserOrm.passw
+00000ea0: 6f72 6420 3d3d 2070 6173 7377 6f72 6429  ord == password)
+00000eb0: 0a20 2020 2072 6573 756c 7420 3d20 6177  .    result = aw
+00000ec0: 6169 7420 7365 7373 696f 6e2e 6578 6563  ait session.exec
+00000ed0: 7574 6528 7374 6d74 290a 2020 2020 7573  ute(stmt).    us
+00000ee0: 6572 203d 2072 6573 756c 742e 7363 616c  er = result.scal
+00000ef0: 6172 5f6f 6e65 5f6f 725f 6e6f 6e65 2829  ar_one_or_none()
+00000f00: 0a0a 2020 2020 7265 7475 726e 2075 7365  ..    return use
+00000f10: 720a 0a0a 6c6f 6769 6e5f 6d61 7463 6865  r...login_matche
+00000f20: 7220 3d20 6f6e 5f63 6f6d 6d61 6e64 2822  r = on_command("
+00000f30: 6c6f 6769 6e22 290a 0a0a 406c 6f67 696e  login")...@login
+00000f40: 5f6d 6174 6368 6572 2e68 616e 646c 6528  _matcher.handle(
+00000f50: 290a 6173 796e 6320 6465 6620 6861 6e64  ).async def hand
+00000f60: 6c65 7228 6576 656e 743a 204d 6573 7361  ler(event: Messa
+00000f70: 6765 4576 656e 742c 206d 6174 6368 6572  geEvent, matcher
+00000f80: 3a20 4d61 7463 6865 7229 3a0a 2020 2020  : Matcher):.    
+00000f90: 7573 6572 6e61 6d65 2c20 7061 7373 776f  username, passwo
+00000fa0: 7264 203d 2065 7665 6e74 2e67 6574 5f70  rd = event.get_p
+00000fb0: 6c61 696e 7465 7874 2829 2e73 706c 6974  laintext().split
+00000fc0: 2822 2022 290a 2020 2020 7573 6572 203d  (" ").    user =
+00000fd0: 2061 7761 6974 206c 6f67 696e 2875 7365   await login(use
+00000fe0: 726e 616d 652c 2070 6173 7377 6f72 6429  rname, password)
+00000ff0: 0a20 2020 2069 6620 7573 6572 2069 7320  .    if user is 
+00001000: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00001010: 2020 6177 6169 7420 6d61 7463 6865 722e    await matcher.
+00001020: 7365 6e64 2866 2248 656c 6c6f 2c20 7b75  send(f"Hello, {u
+00001030: 7365 722e 6e69 636b 6e61 6d65 7d22 290a  ser.nickname}").
+00001040: 6060 600a 0ae5 8f82 e880 83ef bc9a 6874  ```...........ht
+00001050: 7470 733a 2f2f 646f 6373 2e73 716c 616c  tps://docs.sqlal
+00001060: 6368 656d 792e 6f72 672f 656e 2f31 342f  chemy.org/en/14/
+00001070: 6f72 6d2f 6578 7465 6e73 696f 6e73 2f61  orm/extensions/a
+00001080: 7379 6e63 696f 2e68 746d 6c23 7573 696e  syncio.html#usin
+00001090: 672d 6173 796e 6369 6f2d 7363 6f70 6564  g-asyncio-scoped
+000010a0: 2d73 6573 7369 6f6e 0a0a e6b3 a8e6 848f  -session........
+000010b0: efbc 9ae5 8aa1 e5bf 85e4 bf9d e8af 81e4  ................
+000010c0: b880 e6ac a14d 6174 6368 6572 e689 a7e8  .....Matcher....
+000010d0: a18c e8bf 87e7 a88b e4b8 8de4 bc9a e59c  ................
+000010e0: a8e4 b88d e590 8ce7 9a84 5461 736b e4b8  ..........Task..
+000010f0: ade8 b083 e794 a860 6461 7461 5f73 6f75  .......`data_sou
+00001100: 7263 652e 7365 7373 696f 6e28 2960 e88e  rce.session()`..
+00001110: b7e5 8f96 7365 7373 696f 6eef bc88 e58d  ....session.....
+00001120: b3e4 b88d e8a6 81e4 bdbf e794 a860 6372  .............`cr
+00001130: 6561 7465 5f74 6173 6b28 2960 e688 9660  eate_task()`...`
+00001140: 656e 7375 7265 5f66 7574 7572 6528 2960  ensure_future()`
+00001150: e588 9be5 bbba 5461 736b efbc 89ef bc8c  ......Task......
+00001160: e590 a6e5 8899 e58f afe8 83bd e587 bae7  ................
+00001170: 8eb0 e994 99e8 afaf e380 82e8 8ba5 e69c  ................
+00001180: 89e8 bf99 e6a0 b7e7 9a84 e99c 80e6 b182  ................
+00001190: efbc 8ce8 afb7 e58f 82e8 8083 e4b8 8be6  ................
+000011a0: 9687 e79a 84e6 96b9 e6b3 95e6 898b e58a  ................
+000011b0: a8e5 889b e5bb bae5 b9b6 e7ae a1e7 9086  ................
+000011c0: 7365 7373 696f 6ee3 8082 0a0a 0a23 2323  session......###
+000011d0: 2034 e380 81e5 9ca8 4d61 7463 6865 72e4   4......Matcher.
+000011e0: b98b e5a4 96e4 bdbf e794 a80a 0ae5 9ca8  ................
+000011f0: 4d61 7463 6865 72e4 b98b e5a4 96ef bc88  Matcher.........
+00001200: e5a6 826f 6e5f 626f 745f 636f 6e6e 6563  ...on_bot_connec
+00001210: 74e7 ad89 e992 a9e5 ad90 e587 bde6 95b0  t...............
+00001220: e4b8 adef bc8c e688 96e8 8085 e698 af41  ...............A
+00001230: 5053 6368 6564 756c 6572 e79a 84e5 ae9a  PScheduler......
+00001240: e697 b6e4 bbbb e58a a1e4 b8ad efbc 89e5  ................
+00001250: 8899 e5bf 85e9 a1bb e980 9ae8 bf87 6041  ..............`A
+00001260: 7379 6e63 5365 7373 696f 6e28 6461 7461  syncSession(data
+00001270: 5f73 6f75 7263 652e 656e 6769 6e65 2960  _source.engine)`
+00001280: e588 9be5 bbba 7365 7373 696f 6ee3 8082  ......session...
+00001290: 0a0a 6060 6070 7974 686f 6e0a 6173 796e  ..```python.asyn
+000012a0: 6320 6465 6620 646f 5f73 6f6d 6574 6869  c def do_somethi
+000012b0: 6e67 2829 3a0a 2020 2020 6173 796e 6320  ng():.    async 
+000012c0: 7769 7468 2041 7379 6e63 5365 7373 696f  with AsyncSessio
+000012d0: 6e28 6461 7461 5f73 6f75 7263 652e 656e  n(data_source.en
+000012e0: 6769 6e65 2920 6173 2073 6573 7369 6f6e  gine) as session
+000012f0: 3a0a 2020 2020 2020 2020 2320 2e2e 2e0a  :.        # ....
+00001300: 6060 600a 0a                             ```..
```

