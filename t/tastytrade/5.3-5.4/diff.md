# Comparing `tmp/tastytrade-5.3.tar.gz` & `tmp/tastytrade-5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-5.3.tar", last modified: Tue May 30 18:57:37 2023, max compression
+gzip compressed data, was "tastytrade-5.4.tar", last modified: Wed May 31 19:22:00 2023, max compression
```

## Comparing `tastytrade-5.3.tar` & `tastytrade-5.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:57:37.089625 tastytrade-5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-30 18:57:26.000000 tastytrade-5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-30 18:57:37.085625 tastytrade-5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-05-30 18:57:26.000000 tastytrade-5.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:57:37.089625 tastytrade-5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-30 18:57:26.000000 tastytrade-5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:57:37.085625 tastytrade-5.3/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34247 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:57:37.085625 tastytrade-5.3/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/candle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/timeandsale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    20874 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:57:37.085625 tastytrade-5.3/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-30 18:57:37.000000 tastytrade-5.3/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-30 18:57:37.000000 tastytrade-5.3/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:57:37.000000 tastytrade-5.3/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-30 18:57:37.000000 tastytrade-5.3/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 18:57:37.000000 tastytrade-5.3/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:22:00.627303 tastytrade-5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-31 19:21:46.000000 tastytrade-5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-31 19:22:00.627303 tastytrade-5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-05-31 19:21:46.000000 tastytrade-5.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:22:00.627303 tastytrade-5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-31 19:21:46.000000 tastytrade-5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:22:00.623303 tastytrade-5.4/tastytrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34366 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:22:00.627303 tastytrade-5.4/tastytrade/dxfeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/timeandsale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:22:00.623303 tastytrade-5.4/tastytrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-31 19:22:00.000000 tastytrade-5.4/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-31 19:22:00.000000 tastytrade-5.4/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:22:00.000000 tastytrade-5.4/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-31 19:22:00.000000 tastytrade-5.4/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 19:22:00.000000 tastytrade-5.4/tastytrade.egg-info/top_level.txt
```

### Comparing `tastytrade-5.3/LICENSE` & `tastytrade-5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/PKG-INFO` & `tastytrade-5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.3
+Version: 5.4
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `tastytrade-5.3/README.rst` & `tastytrade-5.4/README.rst`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/setup.py` & `tastytrade-5.4/setup.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/account.py` & `tastytrade-5.4/tastytrade/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,25 +49,25 @@
     unsettled_cryptocurrency_fiat_amount: Decimal
     unsettled_cryptocurrency_fiat_effect: PriceEffect
     closed_loop_available_balance: Decimal
     equity_offering_margin_requirement: Decimal
     long_bond_value: Decimal
     bond_margin_requirement: Decimal
     snapshot_date: date
-    time_of_day: str
     reg_t_margin_requirement: Decimal
     futures_overnight_margin_requirement: Decimal
     futures_intraday_margin_requirement: Decimal
     maintenance_excess: Decimal
     pending_margin_interest: Decimal
     apex_starting_day_margin_equity: Decimal
     buying_power_adjustment: Decimal
     buying_power_adjustment_effect: PriceEffect
     effective_cryptocurrency_buying_power: Decimal
     updated_at: datetime
+    time_of_day: Optional[str] = None
 
 
 class AccountBalanceSnapshot(TastytradeJsonDataclass):
     """
     Dataclass containing account balance for a moment in time (snapshot).
     """
     account_number: str
@@ -119,34 +119,34 @@
     symbol: str
     instrument_type: InstrumentType
     underlying_symbol: str
     quantity: Decimal
     quantity_direction: str
     close_price: Decimal
     average_open_price: Decimal
-    average_yearly_market_close_price: Decimal
-    average_daily_market_close_price: Decimal
     multiplier: int
     cost_effect: str
     is_suppressed: bool
     is_frozen: bool
     realized_day_gain: Decimal
-    realized_day_gain_effect: PriceEffect
-    realized_day_gain_date: date
     realized_today: Decimal
-    realized_today_effect: PriceEffect
-    realized_today_date: date
     created_at: datetime
     updated_at: datetime
     mark: Optional[Decimal] = None
     mark_price: Optional[Decimal] = None
     restricted_quantity: Optional[Decimal] = None
     expires_at: Optional[datetime] = None
     fixing_price: Optional[Decimal] = None
     deliverable_type: Optional[str] = None
+    average_yearly_market_close_price: Optional[Decimal] = None
+    average_daily_market_close_price: Optional[Decimal] = None
+    realized_day_gain_effect: Optional[PriceEffect] = None
+    realized_day_gain_date: Optional[date] = None
+    realized_today_effect: Optional[PriceEffect] = None
+    realized_today_date: Optional[date] = None
 
 
 class Lot(TastytradeJsonDataclass):
     """
     Dataclass containing information about the lot of a position.
     """
     id: str
```

### Comparing `tastytrade-5.3/tastytrade/dxfeed/candle.py` & `tastytrade-5.4/tastytrade/dxfeed/candle.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/dxfeed/event.py` & `tastytrade-5.4/tastytrade/dxfeed/event.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/dxfeed/greeks.py` & `tastytrade-5.4/tastytrade/dxfeed/greeks.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/dxfeed/profile.py` & `tastytrade-5.4/tastytrade/dxfeed/profile.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/dxfeed/quote.py` & `tastytrade-5.4/tastytrade/dxfeed/quote.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/dxfeed/summary.py` & `tastytrade-5.4/tastytrade/dxfeed/summary.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/dxfeed/theoprice.py` & `tastytrade-5.4/tastytrade/dxfeed/theoprice.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/dxfeed/timeandsale.py` & `tastytrade-5.4/tastytrade/dxfeed/timeandsale.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/dxfeed/trade.py` & `tastytrade-5.4/tastytrade/dxfeed/trade.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/instruments.py` & `tastytrade-5.4/tastytrade/instruments.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/metrics.py` & `tastytrade-5.4/tastytrade/metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/order.py` & `tastytrade-5.4/tastytrade/order.py`

 * *Files 15% similar despite different names*

```diff
@@ -323,7 +323,101 @@
     """
     buying_power_effect: BuyingPowerEffect
     fee_calculation: FeeCalculation
     order: Optional[PlacedOrder] = None
     complex_order: Optional[ComplexOrder] = None
     warnings: Optional[list[Message]] = None
     errors: Optional[list[Message]] = None
+
+
+class OrderChainEntry(TastytradeJsonDataclass):
+    """
+    Dataclass containing information about a single order in an order chain.
+    """
+    symbol: str
+    instrument_type: InstrumentType
+    quantity: str
+    quantity_type: str
+    quantity_numeric: Decimal
+
+
+class OrderChainLeg(TastytradeJsonDataclass):
+    """
+    Dataclass containing information about a single leg in an order from an order chain.
+    """
+    symbol: str
+    instrument_type: InstrumentType
+    action: OrderAction
+    fill_quantity: Decimal
+    order_quantity: Decimal
+
+
+class OrderChainNode(TastytradeJsonDataclass):
+    """
+    Dataclass containing information about a single node in an order chain.
+    """
+    node_type: str
+    id: str
+    description: str
+    occurred_at: Optional[datetime] = None
+    total_fees: Optional[Decimal] = None
+    total_fees_effect: Optional[PriceEffect] = None
+    total_fill_cost: Optional[Decimal] = None
+    total_fill_cost_effect: Optional[PriceEffect] = None
+    gcd_quantity: Optional[Decimal] = None
+    fill_cost_per_quantity: Optional[Decimal] = None
+    fill_cost_per_quantity_effect: Optional[PriceEffect] = None
+    order_fill_count: Optional[int] = None
+    roll: Optional[bool] = None
+    legs: Optional[list[OrderChainLeg]] = None
+    entries: Optional[list[OrderChainEntry]] = None
+
+
+class ComputedData(TastytradeJsonDataclass):
+    """
+    Dataclass containing computed data about an order chain.
+    """
+    open: bool
+    updated_at: datetime
+    total_fees: Decimal
+    total_fees_effect: PriceEffect
+    total_commissions: Decimal
+    total_commissions_effect: PriceEffect
+    realized_gain: Decimal
+    realized_gain_effect: PriceEffect
+    realized_gain_with_fees: Decimal
+    realized_gain_with_fees_effect: PriceEffect
+    winner_realized_and_closed: bool
+    winner_realized: bool
+    winner_realized_with_fees: bool
+    roll_count: int
+    opened_at: datetime
+    last_occurred_at: datetime
+    started_at_days_to_expiration: int
+    duration: int
+    total_opening_cost: Decimal
+    total_opening_cost_effect: PriceEffect
+    total_closing_cost: Decimal
+    total_closing_cost_effect: PriceEffect
+    total_cost: Decimal
+    total_cost_effect: PriceEffect
+    gcd_open_quantity: Decimal
+    fees_missing: bool
+    open_entries: list[OrderChainEntry]
+    total_cost_per_unit: Optional[Decimal] = None
+    total_cost_per_unit_effect: Optional[PriceEffect] = None
+
+
+class OrderChain(TastytradeJsonDataclass):
+    """
+    Dataclass containing information about an order chain: a group of orders for a
+    specific underlying, such as total P/L, rolls, current P/L in a symbol, etc.
+    """
+    id: int
+    updated_at: datetime
+    created_at: datetime
+    account_number: str
+    description: str
+    underlying_symbol: str
+    computed_data: ComputedData
+    lite_nodes_sizes: int
+    lite_nodes: list[OrderChainNode]
```

### Comparing `tastytrade-5.3/tastytrade/search.py` & `tastytrade-5.4/tastytrade/search.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/session.py` & `tastytrade-5.4/tastytrade/session.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/streamer.py` & `tastytrade-5.4/tastytrade/streamer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import json
 from asyncio import Lock, Queue
 from datetime import datetime
+from decimal import Decimal
 from enum import Enum
 from typing import Any, AsyncIterator, Optional, Union
 
 import requests
 import websockets
 
 from tastytrade import logger
@@ -17,22 +18,61 @@
 from tastytrade.dxfeed.greeks import Greeks
 from tastytrade.dxfeed.profile import Profile
 from tastytrade.dxfeed.quote import Quote
 from tastytrade.dxfeed.summary import Summary
 from tastytrade.dxfeed.theoprice import TheoPrice
 from tastytrade.dxfeed.timeandsale import TimeAndSale
 from tastytrade.dxfeed.trade import Trade
-from tastytrade.order import PlacedOrder
+from tastytrade.order import (InstrumentType, OrderChain, PlacedOrder,
+                              PriceEffect)
 from tastytrade.session import Session
-from tastytrade.utils import TastytradeError, validate_response
+from tastytrade.utils import (TastytradeError, TastytradeJsonDataclass,
+                              validate_response)
+from tastytrade.watchlists import Watchlist
 
 CERT_STREAMER_URL = 'wss://streamer.cert.tastyworks.com'
 STREAMER_URL = 'wss://streamer.tastyworks.com'
 
 
+class QuoteAlert(TastytradeJsonDataclass):
+    """
+    Dataclass that contains information about a quote alert
+    """
+    user_external_id: str
+    symbol: str
+    alert_external_id: str
+    expires_at: int
+    completed_at: datetime
+    created_at: datetime
+    triggered_at: datetime
+    field: str
+    operator: str
+    threshold: str
+    threshold_numeric: Decimal
+    dx_symbol: str
+
+
+class UnderlyingYearGainSummary(TastytradeJsonDataclass):
+    """
+    Dataclass that contains information about the yearly gainYloss for an underlying
+    """
+    year: int
+    account_number: str
+    symbol: str
+    instrument_type: InstrumentType
+    fees: Decimal
+    fees_effect: PriceEffect
+    commissions: Decimal
+    commissions_effect: PriceEffect
+    yearly_realized_gain: Decimal
+    yearly_realized_gain_effect: PriceEffect
+    realized_lot_gain: Decimal
+    realized_lot_gain_effect: PriceEffect
+
+
 class SubscriptionType(str, Enum):
     """
     This is an :class:`~enum.Enum` that contains the subscription types for the alert streamer.
     """
     ACCOUNT = 'account-subscribe'  # 'account-subscribe' may be deprecated in the future
     HEARTBEAT = 'heartbeat'
     PUBLIC_WATCHLISTS = 'public-watchlists-subscribe'
@@ -52,27 +92,25 @@
         session = Session('user', 'pass')
         streamer = await AlertStreamer.create(session)
         accounts = Account.get_accounts(session)
 
         await streamer.account_subscribe(accounts)
         await streamer.public_watchlists_subscribe()
         await streamer.quote_alerts_subscribe()
-        await streamer.user_message_subscribe(session)
 
         async for data in streamer.listen():
             print(data)
 
     """
     def __init__(self, session: Session):
         #: The active session used to initiate the streamer or make requests
         self.token: str = session.session_token
         #: The base url for the streamer websocket
         self.base_url: str = CERT_STREAMER_URL if session.is_certification else STREAMER_URL
 
-        self._done = False
         self._queue: Queue = Queue()
         self._websocket = None
 
         self._connect_task = asyncio.create_task(self._connect())
 
     @classmethod
     async def create(cls, session: Session) -> 'AlertStreamer':
@@ -95,64 +133,54 @@
         during initialization.
         """
         headers = {'Authorization': f'Bearer {self.token}'}
         async with websockets.connect(self.base_url, extra_headers=headers) as websocket:  # type: ignore
             self._websocket = websocket
             self._heartbeat_task = asyncio.create_task(self._heartbeat())
 
-            while not self._done:
+            while True:
                 raw_message = await self._websocket.recv()  # type: ignore
                 logger.debug('raw message: %s', raw_message)
                 await self._queue.put(json.loads(raw_message))
 
-    async def listen(self) -> AsyncIterator[Union[
-        AccountBalance,
-        CurrentPosition,
-        PlacedOrder,
-        TradingStatus,
-        dict  # some possible messages are not yet implemented
-    ]]:
+    async def listen(self) -> AsyncIterator[TastytradeJsonDataclass]:
         """
         Iterate over non-heartbeat messages received from the streamer,
         mapping them to their appropriate data class.
         """
         while True:
             data = await self._queue.get()
             type_str = data.get('type')
             if type_str is not None:
                 yield self._map_message(type_str, data['data'])
             elif data.get('action') != 'heartbeat':
                 logger.debug('subscription message: %s', data)
 
-    def _map_message(self, type_str: str, data: dict) -> Union[
-        AccountBalance,
-        CurrentPosition,
-        PlacedOrder,
-        TradingStatus,
-        dict  # some possible messages are not yet implemented
-    ]:
-        """
-        TODO: implement the following:
-        - OrderChain
-        - UnderlyingYearGainSummary
-        - User status related messages
-        - Watchlist related messages
-        - Quote alert messages
-        - Others?
+    def _map_message(self, type_str: str, data: dict) -> TastytradeJsonDataclass:
+        """
+        I'm not sure what the user-status messages look like, so they're absent.
         """
         if type_str == 'AccountBalance':
             return AccountBalance(**data)
         elif type_str == 'CurrentPosition':
             return CurrentPosition(**data)
         elif type_str == 'Order':
             return PlacedOrder(**data)
+        elif type_str == 'OrderChain':
+            return OrderChain(**data)
+        elif type_str == 'QuoteAlert':
+            return QuoteAlert(**data)
         elif type_str == 'TradingStatus':
             return TradingStatus(**data)
+        elif type_str == 'UnderlyingYearGainSummary':
+            return UnderlyingYearGainSummary(**data)
+        elif type_str == 'PublicWatchlists':
+            return Watchlist(**data)
         else:
-            return data
+            raise TastytradeError(f'Unknown message type: {type_str}\n{data}')
 
     async def account_subscribe(self, accounts: list[Account]) -> None:
         """
         Subscribes to account-level updates (balances, orders, positions).
 
         :param accounts: list of :class:`tastytrade.account.Account`s to subscribe to updates for
         """
@@ -168,31 +196,31 @@
         """
         Subscribes to quote alerts (which are configured at a user level).
         """
         await self._subscribe(SubscriptionType.QUOTE_ALERTS)
 
     async def user_message_subscribe(self, session: Session) -> None:
         """
-        Subscribes to user-level messages.
+        Subscribes to user-level messages, e.g. new account creation.
         """
         external_id = session.user['external-id']
         await self._subscribe(SubscriptionType.USER_MESSAGE, value=external_id)
 
-    async def close(self) -> None:
+    def close(self) -> None:
         """
         Closes the websocket connection and cancels the heartbeat task.
         """
-        self._done = True
-        await asyncio.gather(self._connect_task, self._heartbeat_task)
+        self._connect_task.cancel()
+        self._heartbeat_task.cancel()
 
     async def _heartbeat(self) -> None:
         """
         Sends a heartbeat message every 10 seconds to keep the connection alive.
         """
-        while not self._done:
+        while True:
             await self._subscribe(SubscriptionType.HEARTBEAT, '')
             # send the heartbeat every 10 seconds
             await asyncio.sleep(10)
 
     async def _subscribe(self, subscription: SubscriptionType, value: Union[Optional[str], list[str]] = '') -> None:
         """
         Subscribes to one of the :class:`SubscriptionType`s. Depending on the kind of
@@ -227,15 +255,14 @@
         #: The active session used to initiate the streamer or make requests
         self.session: Session = session
 
         self._counter = 0
         self._lock: Lock = Lock()
         self._queue: Queue = Queue()
         self._queue_candle: Queue = Queue()
-        self._done = False
         #: The unique client identifier received from the server
         self.client_id: Optional[str] = None
 
         response = requests.get(f'{session.base_url}/quote-streamer-tokens', headers=session.headers)
         validate_response(response)
         logger.debug('response %s', json.dumps(response.json()))
         self._auth_token = response.json()['data']['token']
@@ -293,15 +320,16 @@
                 if message['channel'] == Channel.HANDSHAKE:
                     if message['successful']:
                         self.client_id = message['clientId']
                         self._heartbeat_task = asyncio.create_task(self._heartbeat())
                     else:
                         raise TastytradeError('Handshake failed')
 
-            while not self._done:
+            # main loop
+            while True:
                 raw_message = await self._websocket.recv()
                 message = json.loads(raw_message)[0]
 
                 if message['channel'] == Channel.DATA:
                     logger.debug('data received: %s', message)
                     await self._queue.put(message['data'])
                 elif message['channel'] == Channel.CANDLE:
@@ -334,41 +362,41 @@
     async def listen(self) -> AsyncIterator[Event]:
         """
         Using the existing subscriptions, pulls :class:`~tastytrade.dxfeed.event.Event`s and yield returns
         them. Never exits unless there's an error or the channel is closed.
         """
         while True:
             raw_data = await self._queue.get()
-            messages = _map_message(raw_data)
+            messages = self._map_message(raw_data)
             for message in messages:
                 yield message
 
     async def listen_candle(self) -> AsyncIterator[Candle]:
         """
         Using the existing subscriptions, pulls candles and yield returns them.
         Never exits unless there's an error or the channel is closed.
         """
         while True:
             raw_data = await self._queue_candle.get()
-            messages = _map_message(raw_data)
+            messages = self._map_message(raw_data)
             for message in messages:
                 yield message  # type: ignore
 
-    async def close(self) -> None:
+    def close(self) -> None:
         """
         Closes the websocket connection and cancels the heartbeat task.
         """
-        self._done = True
-        await asyncio.gather(self._connect_task, self._heartbeat_task)
+        self._connect_task.cancel()
+        self._heartbeat_task.cancel()
 
     async def _heartbeat(self) -> None:
         """
         Sends a heartbeat message every 10 seconds to keep the connection alive.
         """
-        while not self._done:
+        while True:
             id = await self._next_id()
             message = {
                 'id': id,
                 'channel': Channel.HEARTBEAT,
                 'clientId': self.client_id,
                 'connectionType': 'websocket'
             }
@@ -507,41 +535,38 @@
             if candle.time <= start_time.timestamp() * 1000:
                 break
         await self.unsubscribe_candle(ticker, interval)
 
         candles.reverse()
         return candles
 
-
-def _map_message(message) -> list[Event]:
-    """
-    Takes the raw JSON data and returns a list of parsed :class:`~tastytrade.dxfeed.event.Event` objects.
-    """
-    # the first time around, types are shown
-    if isinstance(message[0], str):
-        msg_type = message[0]
-    else:
-        msg_type = message[0][0]
-    # regardless, the second element will be the raw data
-    data = message[1]
-
-    # parse type or warn for unknown type
-    if msg_type == EventType.CANDLE:
-        res = Candle.from_stream(data)
-    elif msg_type == EventType.GREEKS:
-        res = Greeks.from_stream(data)
-    elif msg_type == EventType.PROFILE:
-        res = Profile.from_stream(data)
-    elif msg_type == EventType.QUOTE:
-        res = Quote.from_stream(data)
-    elif msg_type == EventType.SUMMARY:
-        res = Summary.from_stream(data)
-    elif msg_type == EventType.THEO_PRICE:
-        res = TheoPrice.from_stream(data)
-    elif msg_type == EventType.TIME_AND_SALE:
-        res = TimeAndSale.from_stream(data)
-    elif msg_type == EventType.TRADE:
-        res = Trade.from_stream(data)
-    else:
-        raise TastytradeError(f'Unknown message type received from streamer: {message}')
-
-    return res
+    def _map_message(self, message) -> list[Event]:
+        """
+        Takes the raw JSON data and returns a list of parsed :class:`~tastytrade.dxfeed.event.Event` objects.
+        """
+        # the first time around, types are shown
+        if isinstance(message[0], str):
+            msg_type = message[0]
+        else:
+            msg_type = message[0][0]
+        # regardless, the second element will be the raw data
+        data = message[1]
+
+        # parse type or warn for unknown type
+        if msg_type == EventType.CANDLE:
+            return Candle.from_stream(data)
+        elif msg_type == EventType.GREEKS:
+            return Greeks.from_stream(data)
+        elif msg_type == EventType.PROFILE:
+            return Profile.from_stream(data)
+        elif msg_type == EventType.QUOTE:
+            return Quote.from_stream(data)
+        elif msg_type == EventType.SUMMARY:
+            return Summary.from_stream(data)
+        elif msg_type == EventType.THEO_PRICE:
+            return TheoPrice.from_stream(data)
+        elif msg_type == EventType.TIME_AND_SALE:
+            return TimeAndSale.from_stream(data)
+        elif msg_type == EventType.TRADE:
+            return Trade.from_stream(data)
+        else:
+            raise TastytradeError(f'Unknown message type received from streamer: {message}')
```

### Comparing `tastytrade-5.3/tastytrade/utils.py` & `tastytrade-5.4/tastytrade/utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade/watchlists.py` & `tastytrade-5.4/tastytrade/watchlists.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.3/tastytrade.egg-info/PKG-INFO` & `tastytrade-5.4/tastytrade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.3
+Version: 5.4
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `tastytrade-5.3/tastytrade.egg-info/SOURCES.txt` & `tastytrade-5.4/tastytrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

