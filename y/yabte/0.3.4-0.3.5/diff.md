# Comparing `tmp/yabte-0.3.4.tar.gz` & `tmp/yabte-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yabte-0.3.4.tar", max compression
+gzip compressed data, was "yabte-0.3.5.tar", max compression
```

## Comparing `yabte-0.3.4.tar` & `yabte-0.3.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1072 2023-03-26 22:12:51.450315 yabte-0.3.4/LICENSE
--rw-r--r--   0        0        0     3220 2023-03-26 22:12:51.450315 yabte-0.3.4/README.md
--rw-r--r--   0        0        0      949 2023-03-26 22:12:51.458315 yabte-0.3.4/pyproject.toml
--rw-r--r--   0        0        0       30 2023-03-26 22:12:51.458315 yabte-0.3.4/yabte/__init__.py
--rw-r--r--   0        0        0      664 2023-03-26 22:12:51.458315 yabte-0.3.4/yabte/backtest/__init__.py
--rw-r--r--   0        0        0      670 2023-03-26 22:12:51.458315 yabte-0.3.4/yabte/backtest/_helpers.py
--rw-r--r--   0        0        0     2978 2023-03-26 22:12:51.458315 yabte-0.3.4/yabte/backtest/asset.py
--rw-r--r--   0        0        0     3992 2023-03-26 22:12:51.462315 yabte-0.3.4/yabte/backtest/book.py
--rw-r--r--   0        0        0    12669 2023-03-26 22:12:51.462315 yabte-0.3.4/yabte/backtest/order.py
--rw-r--r--   0        0        0    10872 2023-03-26 22:12:51.462315 yabte-0.3.4/yabte/backtest/strategy.py
--rw-r--r--   0        0        0     2036 2023-03-26 22:12:51.462315 yabte-0.3.4/yabte/backtest/transaction.py
--rw-r--r--   0        0        0        0 2023-03-26 22:12:51.462315 yabte-0.3.4/yabte/tests/__init__.py
--rw-r--r--   0        0        0      594 2023-03-26 22:12:51.462315 yabte-0.3.4/yabte/tests/_helpers.py
--rw-r--r--   0        0        0     1266 2023-03-26 22:12:51.462315 yabte-0.3.4/yabte/tests/_unittest_numpy_extensions.py
--rw-r--r--   0        0        0   137308 2023-03-26 22:12:51.462315 yabte-0.3.4/yabte/tests/data/nasdaq/AAPL.csv
--rw-r--r--   0        0        0   135665 2023-03-26 22:12:51.462315 yabte-0.3.4/yabte/tests/data/nasdaq/AMZN.csv
--rw-r--r--   0        0        0    90302 2023-03-26 22:12:51.462315 yabte-0.3.4/yabte/tests/data/nasdaq/GOOG.csv
--rw-r--r--   0        0        0   136484 2023-03-26 22:12:51.462315 yabte-0.3.4/yabte/tests/data/nasdaq/INTC.csv
--rw-r--r--   0        0        0   135802 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/tests/data/nasdaq/META.csv
--rw-r--r--   0        0        0    93835 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/tests/data/nasdaq/MSFT.csv
--rw-r--r--   0        0        0   130341 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/tests/data/nasdaq/NFLX.csv
--rw-r--r--   0        0        0   139249 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/tests/data/nasdaq/TSLA.csv
--rw-r--r--   0        0        0      799 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/tests/test_notebooks.py
--rw-r--r--   0        0        0     1676 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/tests/test_portopt.py
--rw-r--r--   0        0        0     4075 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/tests/test_simulation.py
--rw-r--r--   0        0        0    18624 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/tests/test_strategy_runner.py
--rw-r--r--   0        0        0     1560 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/tests/test_utilities.py
--rw-r--r--   0        0        0        0 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/__init__.py
--rw-r--r--   0        0        0     1179 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/lagrangian.py
--rw-r--r--   0        0        0     2353 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/pandas_extension.py
--rw-r--r--   0        0        0        0 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/plot/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/plot/matplotlib/__init__.py
--rw-r--r--   0        0        0     3360 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/plot/matplotlib/marker_updater.py
--rw-r--r--   0        0        0     5520 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/plot/matplotlib/strategy_runner.py
--rw-r--r--   0        0        0        0 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/portopt/__init__.py
--rw-r--r--   0        0        0     2332 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/portopt/hierarchical_risk_parity.py
--rw-r--r--   0        0        0      396 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/portopt/inverse_volatility.py
--rw-r--r--   0        0        0     1973 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/portopt/minimum_variance.py
--rw-r--r--   0        0        0        0 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/simulation/__init__.py
--rw-r--r--   0        0        0     1475 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/simulation/geometric_brownian_motion.py
--rw-r--r--   0        0        0     2098 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/simulation/heston.py
--rw-r--r--   0        0        0     1102 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/simulation/weiner.py
--rw-r--r--   0        0        0      397 2023-03-26 22:12:51.466315 yabte-0.3.4/yabte/utilities/strategy_helpers.py
--rw-r--r--   0        0        0     4211 1970-01-01 00:00:00.000000 yabte-0.3.4/setup.py
--rw-r--r--   0        0        0     3825 1970-01-01 00:00:00.000000 yabte-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-31 21:21:14.945726 yabte-0.3.5/LICENSE
+-rw-r--r--   0        0        0     3220 2023-05-31 21:21:14.945726 yabte-0.3.5/README.md
+-rw-r--r--   0        0        0     1115 2023-05-31 21:21:14.957726 yabte-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/__init__.py
+-rw-r--r--   0        0        0      859 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/__init__.py
+-rw-r--r--   0        0        0      670 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/_helpers.py
+-rw-r--r--   0        0        0     3123 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/asset.py
+-rw-r--r--   0        0        0     4004 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/book.py
+-rw-r--r--   0        0        0    12933 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/order.py
+-rw-r--r--   0        0        0    11687 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/strategy.py
+-rw-r--r--   0        0        0     2207 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/transaction.py
+-rw-r--r--   0        0        0        0 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/tests/__init__.py
+-rw-r--r--   0        0        0      594 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/tests/_helpers.py
+-rw-r--r--   0        0        0     1266 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/tests/_unittest_numpy_extensions.py
+-rw-r--r--   0        0        0   137308 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/tests/data/nasdaq/AAPL.csv
+-rw-r--r--   0        0        0   135665 2023-05-31 21:21:14.961726 yabte-0.3.5/yabte/tests/data/nasdaq/AMZN.csv
+-rw-r--r--   0        0        0    90302 2023-05-31 21:21:14.961726 yabte-0.3.5/yabte/tests/data/nasdaq/GOOG.csv
+-rw-r--r--   0        0        0   136484 2023-05-31 21:21:14.961726 yabte-0.3.5/yabte/tests/data/nasdaq/INTC.csv
+-rw-r--r--   0        0        0   135802 2023-05-31 21:21:14.961726 yabte-0.3.5/yabte/tests/data/nasdaq/META.csv
+-rw-r--r--   0        0        0    93835 2023-05-31 21:21:14.961726 yabte-0.3.5/yabte/tests/data/nasdaq/MSFT.csv
+-rw-r--r--   0        0        0   130341 2023-05-31 21:21:14.961726 yabte-0.3.5/yabte/tests/data/nasdaq/NFLX.csv
+-rw-r--r--   0        0        0   139249 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/tests/data/nasdaq/TSLA.csv
+-rw-r--r--   0        0        0      799 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1676 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/tests/test_portopt.py
+-rw-r--r--   0        0        0     4075 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/tests/test_simulation.py
+-rw-r--r--   0        0        0    18624 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/tests/test_strategy_runner.py
+-rw-r--r--   0        0        0     1560 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/tests/test_utilities.py
+-rw-r--r--   0        0        0        0 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/lagrangian.py
+-rw-r--r--   0        0        0     2353 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/pandas_extension.py
+-rw-r--r--   0        0        0        0 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/plot/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/plot/matplotlib/__init__.py
+-rw-r--r--   0        0        0     3360 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/plot/matplotlib/marker_updater.py
+-rw-r--r--   0        0        0     5520 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/plot/matplotlib/strategy_runner.py
+-rw-r--r--   0        0        0        0 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/portopt/__init__.py
+-rw-r--r--   0        0        0     2332 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/portopt/hierarchical_risk_parity.py
+-rw-r--r--   0        0        0      396 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/portopt/inverse_volatility.py
+-rw-r--r--   0        0        0     1973 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/portopt/minimum_variance.py
+-rw-r--r--   0        0        0        0 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/simulation/__init__.py
+-rw-r--r--   0        0        0     1475 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/simulation/geometric_brownian_motion.py
+-rw-r--r--   0        0        0     2098 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/simulation/heston.py
+-rw-r--r--   0        0        0     1102 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/simulation/weiner.py
+-rw-r--r--   0        0        0      397 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/strategy_helpers.py
+-rw-r--r--   0        0        0     4275 1970-01-01 00:00:00.000000 yabte-0.3.5/setup.py
+-rw-r--r--   0        0        0     3916 1970-01-01 00:00:00.000000 yabte-0.3.5/PKG-INFO
```

### Comparing `yabte-0.3.4/LICENSE` & `yabte-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/README.md` & `yabte-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/pyproject.toml` & `yabte-0.3.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 [tool.poetry]
 name = "yabte"
-version = "0.3.4"
+version = "0.3.5"
 description = "Yet another backtesting engine"
 authors = ["Blair Azzopardi <blairuk@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bsdz/yabte"
 
+[tool.poetry.build]
+script = "build.py"
+generate-setup-file = true
+
 [tool.poetry.dependencies]
 python = "^3.10,<3.12"
 pandas = "^1.5.2"
 scipy = "^1.10.0"
+pandas-stubs = "^2.0.0.230412"
+mypy = "^1.3.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^0.991"
 isort = "^5.11.4"
 black = {extras = ["jupyter"], version = "^23.1.0"}
 docformatter = "^1.5.1"
 coverage = "^7.2.1"
 
 [tool.poetry.group.docs]
 optional = true
@@ -38,9 +43,9 @@
 pyfeng = "^0.2.5"
 nbconvert = "^7.2.9"
 
 [tool.isort]
 profile = "black"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.0.0", "setuptools==67.8.0", "mypy==1.3.0", "pandas-stubs==2.0.0.230412"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `yabte-0.3.4/yabte/backtest/_helpers.py` & `yabte-0.3.5/yabte/backtest/_helpers.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/backtest/asset.py` & `yabte-0.3.5/yabte/backtest/asset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from dataclasses import dataclass
 from decimal import Decimal
-from typing import Sequence
+from typing import Sequence, TypeAlias
 
 import pandas as pd
+from mypy_extensions import mypyc_attr
 
 __all__ = ["Asset"]
 
 
-class AssetName(str):
-    """Asset name string."""
+AssetName: TypeAlias = str
+"""Asset name string."""
 
 
+@mypyc_attr(allow_interpreted_subclasses=True)
 @dataclass(kw_only=True)
 class AssetBase:
     """Anything that has a price."""
 
     name: AssetName
     """Name string."""
 
@@ -56,14 +58,15 @@
 
     def check_and_fix_data(self, data: pd.DataFrame) -> pd.DataFrame:
         """Checks dataframe `data` has correct fields and fixes columns where
         necessary."""
         raise NotImplementedError("The apply methods needs to be implemented.")
 
 
+@mypyc_attr(allow_interpreted_subclasses=True)
 @dataclass(kw_only=True)
 class Asset(AssetBase):
     """Assets whose price history is represented by High, Low, Open, Close and
     Volume fields."""
 
     @property
     def fields_available_at_open(self) -> Sequence[str]:
```

### Comparing `yabte-0.3.4/yabte/backtest/book.py` & `yabte-0.3.5/yabte/backtest/book.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from collections import defaultdict
 from dataclasses import dataclass, field
 from decimal import Decimal
 from itertools import groupby
-from typing import Any, Dict, List, Sequence
+from typing import Any, Dict, List, Sequence, TypeAlias
 
 import pandas as pd
 
 from ._helpers import ensure_decimal
 from .asset import Asset, AssetName
 from .transaction import CashTransaction, Trade, Transaction
 
@@ -19,16 +19,16 @@
 
 @dataclass(kw_only=True)
 class BookMandate:
     def check(self, current_pos, quantity) -> bool:
         raise NotImplementedError()
 
 
-class BookName(str):
-    """Book name string."""
+BookName: TypeAlias = str
+"""Book name string."""
 
 
 @dataclass(kw_only=True)
 class Book:
     """Record of asset trades and positions including cash.
 
     A `name` can be provided and the default `cash` value can be changed
```

### Comparing `yabte-0.3.4/yabte/backtest/order.py` & `yabte-0.3.5/yabte/backtest/order.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass, field
 from decimal import Decimal
 from enum import Enum
-from typing import Callable, Dict, List, Optional, Tuple
+from typing import Dict, List, Optional, Tuple
 
 import pandas as pd
+from mypy_extensions import mypyc_attr
 
 from ._helpers import ensure_decimal, ensure_enum
 from .asset import Asset, AssetName
 from .book import Book, BookName
 from .transaction import Trade
 
 logger = logging.getLogger(__name__)
@@ -46,14 +47,15 @@
     NOTIONAL = 2
     """Size represent notional amount."""
 
     BOOK_PERCENT = 3
     """Size is a percentage of book value."""
 
 
+@mypyc_attr(allow_interpreted_subclasses=True)
 @dataclass(kw_only=True)
 class OrderBase:
     """Base class for all orders."""
 
     status: OrderStatus = OrderStatus.OPEN
     """Status of order."""
 
@@ -101,14 +103,15 @@
         self, ts: pd.Timestamp, day_data: pd.DataFrame, asset_map: Dict[str, Asset]
     ):
         """Applies order to `self.book` for time `ts` using provided `day_data`
         and dictionary of asset information `asset_map`."""
         raise NotImplementedError("The apply methods needs to be implemented.")
 
 
+@mypyc_attr(allow_interpreted_subclasses=True)
 @dataclass(kw_only=True)
 class Order(OrderBase):
     """Simple market order."""
 
     asset_name: AssetName
     """Asset name for order."""
 
@@ -183,14 +186,15 @@
 
 
 class PositionalOrderCheckType(Enum):
     POS_TQ_DIFFER = 1
     ZERO_POS = 2
 
 
+@mypyc_attr(allow_interpreted_subclasses=True)
 @dataclass(kw_only=True)
 class PositionalOrder(Order):
     """Ensures current position is `size` and will close out existing positions
     to achieve this."""
 
     check_type: PositionalOrderCheckType = PositionalOrderCheckType.POS_TQ_DIFFER
     """Condition type to determine if a trade is required."""
@@ -244,14 +248,15 @@
                         order_label=self.label,
                     )
                 )
 
         self._book_trades(trades)
 
 
+@mypyc_attr(allow_interpreted_subclasses=True)
 @dataclass
 class BasketOrder(OrderBase):
     """Combine multiple assets into a single order."""
 
     asset_names: List[AssetName]
     """List of asset names in basket."""
 
@@ -327,14 +332,15 @@
             )
             for an, (tq, tp) in zip(self.asset_names, trade_quantity_prices)
         ]
 
         self._book_trades(trades)
 
 
+@mypyc_attr(allow_interpreted_subclasses=True)
 @dataclass(kw_only=True)
 class PositionalBasketOrder(BasketOrder):
     """Similar to a :py:class:`BasketOrder` but will close out existing
     positions if they do not match requested weights."""
 
     check_type: PositionalOrderCheckType = PositionalOrderCheckType.POS_TQ_DIFFER
```

### Comparing `yabte-0.3.4/yabte/backtest/strategy.py` & `yabte-0.3.5/yabte/backtest/strategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,80 @@
 import logging
 from collections import Counter, deque
 from copy import deepcopy
 from dataclasses import dataclass, field
 from itertools import chain, product
-from typing import Any, Dict, List, Optional, Type
+from typing import Any, Dict, Iterable, List, Optional, Type
 
-import numpy as np
 import pandas as pd
+from mypy_extensions import mypyc_attr
+
+# TODO: use explicit imports until mypyc fixes attribute lookups in dataclass
+# (https://github.com/mypyc/mypyc/issues/1000)
+from pandas import DataFrame, Series, Timestamp  # type: ignore
 
 from .asset import Asset, AssetName
 from .book import Book, BookMandate, BookName
-from .order import Order, OrderStatus
+from .order import Order, OrderBase, OrderStatus
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["Strategy", "StrategyRunner"]
 
 
-class Orders(deque):
+class Orders:
+    def __init__(self):
+        self.deque = deque()
+
+    def __len__(self):
+        return len(self.deque)
+
+    def __iter__(self):
+        return iter(self.deque)
+
+    def popleft(self):
+        return self.deque.popleft()
+
+    def append(self, order: OrderBase):
+        return self.deque.append(order)
+
+    def extend(self, orders: Iterable[OrderBase]):
+        return self.deque.extend(orders)
+
     def sort_by_priority(self):
         """Sorts orders by order priority."""
-        ou_sorted = sorted(self, key=lambda o: o.priority, reverse=True)
-        self.clear()
-        self.extend(ou_sorted)
+        ou_sorted = sorted(self.deque, key=lambda o: o.priority, reverse=True)
+        self.deque.clear()
+        self.deque.extend(ou_sorted)
 
-    def remove_duplicate_keys(self) -> List[Order]:
+    def remove_duplicate_keys(self) -> List[OrderBase]:
         """Remove older orders with same key.
 
         Returns a list of orders than were removed with status set to
         REPLACED.
         """
         removed = []
-        cntr = Counter(o.key for o in self if o.key is not None)
+        cntr = Counter(o.key for o in self.deque if o.key is not None)
         if any(v > 1 for v in cntr.values()):
             kept = []
-            while self:
-                o = self.popleft()
+            while self.deque:
+                o = self.deque.popleft()
                 if o.key in cntr and cntr[o.key] > 1:
                     o.status = OrderStatus.REPLACED
                     removed.append(o)
                     cntr[o.key] -= 1
                 else:
                     kept.append(o)
-            self.clear()
-            self.extend(kept)
+            self.deque.clear()
+            self.deque.extend(kept)
 
         return removed
 
 
+@mypyc_attr(allow_interpreted_subclasses=True)
 @dataclass(kw_only=True)
 class Strategy:
     """Trading strategy base class.
 
     This class should be derived from and will be instantiated by
     :py:class:`StrategyRunner`.
     """
@@ -64,24 +87,24 @@
 
     books: Dict[BookName, Book]
     """Dictionary of books."""
 
     assets: Dict[AssetName, Asset]
     """Dictionary of assets."""
 
-    _ts = None
-    _data_lock = True
-    _mask_open = False
+    _ts: pd.Timestamp | None = None
+    _data_lock: bool = True
+    _mask_open: bool = False
 
     @property
-    def ts(self):
+    def ts(self) -> pd.Timestamp | None:
         """Stores the current timestamp."""
         return self._ts
 
-    def _set_ts(self, ts):
+    def _set_ts(self, ts: pd.Timestamp):
         """Internal method to update timestep to current `ts`"""
         self._ts = ts
 
     def _get_col_indexer(self):
         # cache this call for hopefully a small speed up
         if not hasattr(self, "_col_indexer"):
             mix = pd.MultiIndex.from_tuples(
@@ -99,15 +122,15 @@
     def data(self) -> pd.DataFrame:
         """Provides window of data available up to current timestamp `self.ts`
         and masks out data not availble at open (like high, low, close,
         volume)."""
         if not self.ts:
             return self._data
         else:
-            df_t = self._data.loc[: self.ts, :]
+            df_t = self._data.loc[: self.ts, :]  # type: ignore[misc]
             if not self._mask_open:
                 data = df_t
             else:
                 row_indexer = df_t.index == df_t.index[-1]
                 # generate mask from asset instances, some assets
                 # might support different field masks
                 col_indexer = self._get_col_indexer()
```

### Comparing `yabte-0.3.4/yabte/backtest/transaction.py` & `yabte-0.3.5/yabte/backtest/transaction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import logging
 from dataclasses import dataclass
 from decimal import Decimal
 
 import pandas as pd
 
+# TODO: use explicit imports until mypyc fixes attribute lookups in dataclass
+# (https://github.com/mypyc/mypyc/issues/1000)
+from pandas import Timestamp  # type: ignore
+
 from .asset import AssetName
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["CashTransaction"]
```

### Comparing `yabte-0.3.4/yabte/tests/_helpers.py` & `yabte-0.3.5/yabte/tests/_helpers.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/_unittest_numpy_extensions.py` & `yabte-0.3.5/yabte/tests/_unittest_numpy_extensions.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/data/nasdaq/AAPL.csv` & `yabte-0.3.5/yabte/tests/data/nasdaq/AAPL.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/data/nasdaq/AMZN.csv` & `yabte-0.3.5/yabte/tests/data/nasdaq/AMZN.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/data/nasdaq/GOOG.csv` & `yabte-0.3.5/yabte/tests/data/nasdaq/GOOG.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/data/nasdaq/INTC.csv` & `yabte-0.3.5/yabte/tests/data/nasdaq/INTC.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/data/nasdaq/META.csv` & `yabte-0.3.5/yabte/tests/data/nasdaq/META.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/data/nasdaq/MSFT.csv` & `yabte-0.3.5/yabte/tests/data/nasdaq/MSFT.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/data/nasdaq/NFLX.csv` & `yabte-0.3.5/yabte/tests/data/nasdaq/NFLX.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/data/nasdaq/TSLA.csv` & `yabte-0.3.5/yabte/tests/data/nasdaq/TSLA.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/test_notebooks.py` & `yabte-0.3.5/yabte/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/test_portopt.py` & `yabte-0.3.5/yabte/tests/test_portopt.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/test_simulation.py` & `yabte-0.3.5/yabte/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/test_strategy_runner.py` & `yabte-0.3.5/yabte/tests/test_strategy_runner.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/tests/test_utilities.py` & `yabte-0.3.5/yabte/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/utilities/lagrangian.py` & `yabte-0.3.5/yabte/utilities/lagrangian.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/utilities/pandas_extension.py` & `yabte-0.3.5/yabte/utilities/pandas_extension.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/utilities/plot/matplotlib/marker_updater.py` & `yabte-0.3.5/yabte/utilities/plot/matplotlib/marker_updater.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/utilities/plot/matplotlib/strategy_runner.py` & `yabte-0.3.5/yabte/utilities/plot/matplotlib/strategy_runner.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/utilities/portopt/hierarchical_risk_parity.py` & `yabte-0.3.5/yabte/utilities/portopt/hierarchical_risk_parity.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/utilities/portopt/minimum_variance.py` & `yabte-0.3.5/yabte/utilities/portopt/minimum_variance.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/utilities/simulation/geometric_brownian_motion.py` & `yabte-0.3.5/yabte/utilities/simulation/geometric_brownian_motion.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/utilities/simulation/heston.py` & `yabte-0.3.5/yabte/utilities/simulation/heston.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/yabte/utilities/simulation/weiner.py` & `yabte-0.3.5/yabte/utilities/simulation/weiner.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.4/setup.py` & `yabte-0.3.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,22 @@
  'yabte.utilities.portopt',
  'yabte.utilities.simulation']
 
 package_data = \
 {'': ['*'], 'yabte.tests': ['data/nasdaq/*']}
 
 install_requires = \
-['pandas>=1.5.2,<2.0.0', 'scipy>=1.10.0,<2.0.0']
+['mypy>=1.3.0,<2.0.0',
+ 'pandas-stubs>=2.0.0.230412,<3.0.0.0',
+ 'pandas>=1.5.2,<2.0.0',
+ 'scipy>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'yabte',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': 'Yet another backtesting engine',
     'long_description': '# yabte - Yet Another BackTesting Engine\n\nPython module for backtesting trading strategies.\n\nSupport event driven backtesting, ie `on_open`, `on_close`, etc. Also supports multiple assets.\n\nVery basic statistics like book cash, mtm and total value. Currently, everything else needs to be deferred to a 3rd party module like `empyrical`.\n\nThere are some basic tests but use at your own peril. It\'s not production level code.\n\n## Core dependencies\n\nThe core module uses pandas and scipy.\n\n## Installation\n\n```bash\npip install yatbe\n```\n\n## Usage\n\nBelow is an example usage (the performance of the example strategy won\'t be good).\n\n```python\nimport pandas as pd\n\nfrom yabte.backtest import Strategy, StrategyRunner, Order, Book\nfrom yabte.utilities.plot.matplotlib.strategy_runner import plot_strategy_runner\nfrom yabte.utilities.strategy_helpers import crossover\nfrom yabte.tests._helpers import generate_nasdaq_dataset\n\n\nclass SMAXO(Strategy):\n    def init(self):\n        # enhance data with simple moving averages\n\n        p = self.params\n        days_short = p.get("days_short", 10)\n        days_long = p.get("days_long", 20)\n\n        close_sma_short = (\n            self.data.loc[:, (slice(None), "Close")]\n            .rolling(days_short)\n            .mean()\n            .rename({"Close": "CloseSMAShort"}, axis=1, level=1)\n        )\n        close_sma_long = (\n            self.data.loc[:, (slice(None), "Close")]\n            .rolling(days_long)\n            .mean()\n            .rename({"Close": "CloseSMALong"}, axis=1, level=1)\n        )\n        self.data = pd.concat(\n            [self.data, close_sma_short, close_sma_long], axis=1\n        ).sort_index(axis=1)\n\n    def on_close(self):\n        # create some orders\n\n        for symbol in ["GOOG", "MSFT"]:\n            df = self.data[symbol]\n            ix_2d = df.index[-2:]\n            data = df.loc[ix_2d, ("CloseSMAShort", "CloseSMALong")].dropna()\n            if len(data) == 2:\n                if crossover(data.CloseSMAShort, data.CloseSMALong):\n                    self.orders.append(Order(asset_name=symbol, size=-100))\n                elif crossover(data.CloseSMALong, data.CloseSMAShort):\n                    self.orders.append(Order(asset_name=symbol, size=100))\n\n\n# load some data\nassets, df_combined = generate_nasdaq_dataset()\n\n# create a book with 100000 cash\nbook = Book(name="Main", cash="100000")\n\n# run our strategy\nsr = StrategyRunner(\n    data=df_combined,\n    assets=assets,\n    strat_classes=[SMAXO],\n    books=[book],\n)\nsr.run()\n\n# see the trades or book history\nth = sr.transaction_history\nbch = sr.book_history.loc[:, (slice(None), "cash")]\n\n# plot the trades against book value\nplot_strategy_runner(sr);\n\n```\n\n![Output from code](https://raw.githubusercontent.com/bsdz/yabte/main/readme_image.png)\n\n## Examples\n\nJupyter notebook examples can be found under the [notebooks folder](https://github.com/bsdz/yabte/tree/main/notebooks).\n\n## Documentation\n\nDocumentation can be found on [Read the Docs](https://yabte.readthedocs.io/en/latest/).\n\n\n## Development\n\nBefore commit run following format commands in project folder:\n\n```bash\npoetry run black .\npoetry run isort . --profile black\npoetry run docformatter . --recursive --in-place\n```\n',
     'author': 'Blair Azzopardi',
     'author_email': 'blairuk@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bsdz/yabte',
```

### Comparing `yabte-0.3.4/PKG-INFO` & `yabte-0.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: yabte
-Version: 0.3.4
+Version: 0.3.5
 Summary: Yet another backtesting engine
 Home-page: https://github.com/bsdz/yabte
 License: MIT
 Author: Blair Azzopardi
 Author-email: blairuk@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: mypy (>=1.3.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pandas-stubs (>=2.0.0.230412,<3.0.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://github.com/bsdz/yabte
 Description-Content-Type: text/markdown
 
 # yabte - Yet Another BackTesting Engine
 
 Python module for backtesting trading strategies.
```

