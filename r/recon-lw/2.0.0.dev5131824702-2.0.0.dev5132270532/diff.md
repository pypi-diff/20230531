# Comparing `tmp/recon_lw-2.0.0.dev5131824702.tar.gz` & `tmp/recon_lw-2.0.0.dev5132270532.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5131824702.tar", last modified: Wed May 31 10:38:02 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5132270532.tar", last modified: Wed May 31 11:29:16 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5131824702.tar` & `recon_lw-2.0.0.dev5132270532.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-31 10:37:42.000000 recon_lw-2.0.0.dev5131824702/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    30669 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15364 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-31 11:28:55.000000 recon_lw-2.0.0.dev5132270532/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32005 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22181 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5131824702/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5132270532/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5131824702/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5132270532/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5131824702/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5132270532/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5131824702/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5132270532/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5131824702/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5132270532/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,17 @@
                     r["body"]["operation_params"] = initial_parameters
                     r["body"]["initial_book"] = initial_book
                 r["body"]["operation"] = operation.__name__
                 r["body"]["book_id"] = book_id
                 r["parentEventId"] = parent_event["eventId"]
                 r["attachedMessageIds"] = [mess["messageId"]]
                 events.append(r)
+        book["last_operation"] = operation.__name__
+        book["last_params"] = initial_parameters
+
 
     dbg_event = recon_lw.create_event("DebugEvent",
                                       "DebugEvent",
                                       event_sequence,
                                       ok=True,
                                       body={"operations": [(op[0], op[2]["messageId"]) for op in operations_batch],
                                             "len(batch)": len(operations_batch),
@@ -307,18 +310,20 @@
     save_events_func(dupl_events)
     duplicates.clear()
     flush_sequence_clear_cache(n_processed, rule_settings["sequence_cache"])
 
 
 def init_aggr_seq(order_book: dict) -> None:
     order_book["aggr_seq"] = {"top_v": 0, "top_delta": 0, "limit_v": 0, "limit_delta": 0, "limit_v2" : 0, "top_v2" : 0, "affected_side": "na", "affected_level": -1}
+    order_book["implied_only"] = False
 
 
 def reset_aggr_seq(order_book):
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0, "affected_side": "na", "affected_level": -1})
+    order_book["implied_only"] = False
 
 
 def reflect_price_update_in_version(side: str, price: float,str_time_of_event,order_book: dict):
     level = get_price_level(side, price, order_book)
     order_book["aggr_seq"]["affected_side"] = side
     order_book["aggr_seq"]["affected_level"] = level
 
@@ -570,15 +575,15 @@
     side_key = side + "_aggr"
     del_index = level - 1
     if not 0 <= del_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body, []
 
     #is it purely implied
-    order_book["implied_only"] = (order_book[side_key]["real_num_orders"] == 0)
+    order_book["implied_only"] = (order_book[side_key][del_index]["real_num_orders"] == 0)
 
     order_book[side_key].pop(del_index)
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     return {}, [copy.deepcopy(order_book)]
@@ -597,16 +602,16 @@
     side_key = side + "_aggr"
     update_index = level - 1
     if not 0 <= update_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body, []
 
     #is it purely implied
-    order_book["implied_only"] = (order_book[side_key]["real_num_orders"] == real_num_orders) and \
-                                 (order_book[side_key]["real_qty"] == real_qty)
+    order_book["implied_only"] = (order_book[side_key][update_index]["real_num_orders"] == real_num_orders) and \
+                                 (order_book[side_key][update_index]["real_qty"] == real_qty)
 
 
     upd_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders,
                  "impl_qty": impl_qty, "impl_num_orders": impl_num_orders}
     order_book[side_key][update_index].update(upd_level)
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
@@ -650,51 +655,87 @@
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 1
     order_book["aggr_seq"]["top_v"] += 1
 
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_top_update(ask_price: str, ask_real_qty: str, ask_impl_qty: str, ask_real_n_orders: str, ask_impl_n_orders: str,
-                  bid_price: int, bid_real_qty: str, bid_impl_qty: str, bid_real_n_orders: int, bid_impl_n_orders: str,
+def ob_indicative_market_data_trade(trade_price: float, str_time_of_event, order_book: dict):
+    if "aggr_seq" not in order_book:
+        init_aggr_seq(order_book)
+    else:
+        reset_aggr_seq(order_book)
+
+    order_book["last_price"] = trade_price
+    if trade_price > order_book["max_price"]:
+        order_book["max_price"] = trade_price
+    if trade_price < order_book["min_price"]:
+        order_book["min_price"] = trade_price
+
+    update_time_and_version(str_time_of_event, order_book)
+    order_book["aggr_seq"]["top_delta"] = 0
+    order_book["aggr_seq"]["limit_delta"] = 0
+
+    return {}, [copy.deepcopy(order_book)]
+
+
+def ob_indicative_open_price(opening_price: float, str_time_of_event, order_book: dict):
+    if "aggr_seq" not in order_book:
+        init_aggr_seq(order_book)
+    else:
+        reset_aggr_seq(order_book)
+
+    order_book["open_price"] = opening_price
+    order_book["last_price"] = opening_price
+    order_book["max_price"] = opening_price
+    order_book["min_price"] = opening_price
+
+    update_time_and_version(str_time_of_event, order_book)
+    order_book["aggr_seq"]["top_delta"] = 0
+    order_book["aggr_seq"]["limit_delta"] = 0
+
+    return {}, [copy.deepcopy(order_book)]
+
+
+def ob_top_update(ask_price: float, ask_real_qty: int, ask_impl_qty: int, ask_real_n_orders: int, ask_impl_n_orders: int,
+                  bid_price: float, bid_real_qty: int, bid_impl_qty: int, bid_real_n_orders: int, bid_impl_n_orders: int,
                   str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     #is it purely implied
     sell_implieds_only = False
-    if float(ask_price) == float(order_book["ask_price"]):
+    if ask_price == order_book["ask_price"]:
         if ask_real_n_orders == order_book["ask_real_n_orders"]:
             sell_implieds_only = True
-    if float(ask_price) > float(order_book["ask_price"]):
-        if ask_impl_n_orders != "0" and \
-                ask_real_n_orders == "0":
+    if ask_price > order_book["ask_price"]:
+        if ask_impl_n_orders != 0 and \
+                ask_real_n_orders == 0:
             sell_implieds_only = True
-    if float(ask_price) < float(order_book["ask_price"]):
-        if order_book["ask_impl_n_orders"] != "0" and \
-                order_book["ask_real_n_orders"] == "0":
+    if ask_price < order_book["ask_price"]:
+        if order_book["ask_impl_n_orders"] != 0 and \
+                order_book["ask_real_n_orders"] == 0:
             sell_implieds_only = True
 
     buy_implieds_only = False
-    if float(bid_price) == float(order_book["bid_price"]):
+    if bid_price == order_book["bid_price"]:
         if bid_real_n_orders == order_book["bid_real_n_orders"]:
             buy_implieds_only = True
-    if float(bid_price) < float(order_book["bid_price"]):
-        if bid_impl_n_orders != "0" and \
-                bid_real_n_orders == "0":
+    if bid_price < order_book["bid_price"]:
+        if bid_impl_n_orders != 0 and \
+                bid_real_n_orders == 0:
             buy_implieds_only = True
-    if float(bid_price) < float(order_book["bid_price"]):
-        if order_book["bid_impl_n_orders"] != "0" and \
-                order_book["bid_real_n_orders"] == "0":
+    if bid_price < order_book["bid_price"]:
+        if order_book["bid_impl_n_orders"] != 0 and \
+                order_book["bid_real_n_orders"] == 0:
             buy_implieds_only = True
     order_book["implied_only"] = sell_implieds_only and buy_implieds_only
 
-
     order_book["ask_price"] = ask_price
     order_book["ask_real_qty"] = ask_real_qty
     order_book["ask_impl_qty"] = ask_impl_qty
     order_book["ask_real_n_orders"] = ask_real_n_orders
     order_book["ask_impl_n_orders"] = ask_impl_n_orders
     order_book["bid_price"] = bid_price
     order_book["bid_real_qty"] = bid_real_qty
```

### Comparing `recon_lw-2.0.0.dev5131824702/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5132270532/recon_lw/recon_ob_cross_stream.py`

 * *Files 17% similar despite different names*

```diff
@@ -44,14 +44,60 @@
                 problems.append({"synopsys": " full_miss_level", "side": side, "level": i + 1})
             elif i >= len(aggr_levels):
                 problems.append({"synopsys": " aggr_miss_level", "side": side, "level": i + 1})
 
     return problems
 
 
+def compare_aggr_vs_top(aggr_book: dict, top_book: dict):
+    problems = []
+    if len(aggr_book["ask_aggr"]) > 0:
+        if top_book["ask_real_qty"] == 0 and top_book["ask_impl_qty"] == 0:
+            problems.append({"synopsys": "top_miss_level", "side": "ask"})
+        else:
+            price_condition = aggr_book["ask_aggr"][0]["price"] == top_book["ask_price"]
+            num_orders_condition1 = (aggr_book["ask_aggr"][0]["real_num_orders"]) == \
+                                    (top_book["ask_real_n_orders"])
+            num_orders_condition2 = (aggr_book["ask_aggr"][0]["impl_num_orders"]) == \
+                                    (top_book["ask_impl_n_orders"])
+            size_condition1 = aggr_book["ask_aggr"][0]["real_qty"] == (top_book["ask_real_qty"])
+            size_condition2 = aggr_book["ask_aggr"][0]["impl_qty"] == (top_book["ask_impl_qty"])
+            if not (price_condition and num_orders_condition1
+                    and num_orders_condition2 and size_condition1 and size_condition2):
+                problems.append({"synopsys": synopsys(price_condition,
+                                                      num_orders_condition1 and num_orders_condition2,
+                                                      size_condition1 and size_condition2),
+                                 "side": "ask"})
+    else:
+        if top_book["ask_real_qty"] != 0 or top_book["ask_impl_qty"] != 0:
+            problems.append({"synopsys": "aggr_miss_level", "side": "ask"})
+
+    if len(aggr_book["bid_aggr"]) > 0:
+        if top_book["bid_real_qty"] == 0 and top_book["bid_impl_qty"] == 0:
+            problems.append({"synopsys": "top_miss_level", "side": "bid"})
+        else:
+            price_condition = aggr_book["bid_aggr"][0]["price"] == top_book["bid_price"]
+            num_orders_condition1 = (aggr_book["bid_aggr"][0]["real_num_orders"]) == \
+                                    (top_book["bid_real_n_orders"])
+            num_orders_condition2 = (aggr_book["bid_aggr"][0]["impl_num_orders"]) == \
+                                    (top_book["bid_impl_n_orders"])
+            size_condition1 = aggr_book["bid_aggr"][0]["real_qty"] == (top_book["bid_real_qty"])
+            size_condition2 = aggr_book["bid_aggr"][0]["impl_qty"] == (top_book["bid_impl_qty"])
+            if not (price_condition and num_orders_condition1
+                    and num_orders_condition2 and size_condition1 and size_condition2):
+                problems.append({"synopsys": synopsys(price_condition,
+                                                      num_orders_condition1 and num_orders_condition2,
+                                                      size_condition1 and size_condition2),
+                                 "side": "bid"})
+    else:
+        if top_book["bid_real_qty"] != 0 or top_book["bid_impl_qty"] != 0:
+            problems.append({"synopsys": "full_miss_level", "side": "bid"})
+    return problems
+
+
 def compare_full_vs_top(full_book: dict, top_book: dict):
     problems = []
     if len(full_book["ask"]) > 0:
         if top_book["ask_real_qty"] == 0:
             problems.append({"synopsys": "top_miss_level", "side": "ask"})
         else:
             top_p = min(full_book["ask"].keys())
@@ -117,14 +163,31 @@
         return o["body"]["timestamp"], None, "{0}_{1}_{2}".format(o["body"]["book_id"],
                                                                   o["body"]["time_of_event"],
                                                                   o["body"]["aggr_seq"]["top_v2"])
 
     return None, None, None
 
 
+def ob_compare_get_timestamp_key1_key2_top_aggr(o, custom_settings):
+    if o["body"]["aggr_seq"]["top_delta"] not in [1, 2]:
+        return None, None, None
+
+    if o["body"]["sessionId"] == custom_settings["top_session"]:
+        return o["body"]["timestamp"], "{0}_{1}_{2}".format(o["body"]["book_id"],
+                                                            o["body"]["time_of_event"],
+                                                            o["body"]["aggr_seq"]["top_v2"]), None
+
+    if o["body"]["sessionId"] == custom_settings["aggr_session"]:
+        return o["body"]["timestamp"], None, "{0}_{1}_{2}".format(o["body"]["book_id"],
+                                                                  o["body"]["time_of_event"],
+                                                                  o["body"]["aggr_seq"]["limit_v2"])
+
+    return None, None, None
+
+
 def ob_compare_interpret_match_aggr(match, custom_settings, create_event, save_events):
     if match[0] is not None and match[1] is not None:
         comp_res = compare_full_vs_aggr(match[0]["body"], match[1]["body"])
         if len(comp_res) > 0:
             error_event = create_event("StreamMismatchAggr",
                                        "StreamMismatchAggr",
                                        False,
@@ -191,14 +254,50 @@
                                     "book_id": match[1]["body"]["book_id"],
                                     "time_of_event": match[1]["body"]["time_of_event"],
                                     "top_v2": match[1]["body"]["aggr_seq"]["top_v2"],
                                     "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
 
 
+def ob_compare_interpret_match_top_aggr(match, custom_settings, create_event, save_events):
+    if match[0] is not None and match[1] is not None:
+        comp_res = compare_aggr_vs_top(match[1]["body"], match[0]["body"])
+        if len(comp_res) > 0:
+            error_event = create_event("StreamMismatchTopAggr",
+                                       "StreamMismatchTopAggr",
+                                       False,
+                                       {"top_book_event": match[0]["eventId"],
+                                        "aggr_book_event": match[1]["eventId"],
+                                        "book_id": match[0]["body"]["book_id"],
+                                        "time_of_event": match[0]["body"]["time_of_event"],
+                                        "top_v2": match[0]["body"]["aggr_seq"]["top_v2"],
+                                        "errors": comp_res})
+            save_events([error_event])
+    elif match[0] is not None:
+        error_event = create_event("StreamMismatchNoAggrVsTop",
+                                   "StreamMismatchNoAggrVsTop",
+                                   False,
+                                   {"top_book_event": match[0]["eventId"],
+                                    "book_id": match[0]["body"]["book_id"],
+                                    "time_of_event": match[0]["body"]["time_of_event"],
+                                    "top_v2": match[0]["body"]["aggr_seq"]["top_v2"],
+                                    "sessionId": match[0]["body"]["sessionId"]})
+        save_events([error_event])
+    elif match[1] is not None:
+        error_event = create_event("StreamMismatchNoTopVsAggr",
+                                   "StreamMismatchNoTopVsAggr",
+                                   False,
+                                   {"aggr_book_event": match[1]["eventId"],
+                                    "book_id": match[1]["body"]["book_id"],
+                                    "time_of_event": match[1]["body"]["time_of_event"],
+                                    "limit_v2": match[1]["body"]["aggr_seq"]["limit_v2"],
+                                    "sessionId": match[1]["body"]["sessionId"]})
+        save_events([error_event])
+
+
 def split_every(n, data):
     iterable = iter(data)
     while 1:
         piece = list(islice(iterable, n))
         if not piece:
             break
         yield piece
@@ -235,14 +334,28 @@
                 ob_compare_interpret_match_top,
                 {"full_session": full_session, "comp_session": top_session},
                 lambda name, ev_type, ok, body: events_saver.create_event(
                     name, ev_type, ok, body, parentId=rule_root_event["eventId"]),
                 lambda ev_batch: events_saver.save_events(ev_batch)
             )
             processors.append(processor_top)
+        if "top_session" in rule_params and "aggr_session" in rule_params:
+            aggr_session = rule_params["aggr_session"]
+            top_session = rule_params["top_session"]
+            processor_top_aggr = TimeCacheMatcher(
+                rule_params["horizon_delay"],
+                ob_compare_get_timestamp_key1_key2_top_aggr,
+                ob_compare_interpret_match_top_aggr,
+                {"top_session": top_session, "aggr_session": aggr_session},
+                lambda name, ev_type, ok, body: events_saver.create_event(
+                    name, ev_type, ok, body, parentId=rule_root_event["eventId"]),
+                lambda ev_batch: events_saver.save_events(ev_batch)
+            )
+            processors.append(processor_top_aggr)
+
 
     # order_books_events = source_events.filter(lambda e: e["eventType"] == "OrderBook")
 
     # buffers = split_every(100, order_books_events)
     streams = recon_lw.open_scoped_events_streams(source_events_path, lambda n: "default_" not in n)
     message_buffer = [None] * 100
     buffer_len = 100
```

### Comparing `recon_lw-2.0.0.dev5131824702/setup.py` & `recon_lw-2.0.0.dev5132270532/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5131824702/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5132270532/test/test_recon_ob.py`

 * *Files identical despite different names*

