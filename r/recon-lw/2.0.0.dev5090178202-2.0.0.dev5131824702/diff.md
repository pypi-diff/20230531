# Comparing `tmp/recon_lw-2.0.0.dev5090178202.tar.gz` & `tmp/recon_lw-2.0.0.dev5131824702.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5090178202.tar", last modified: Fri May 26 11:13:05 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5131824702.tar", last modified: Wed May 31 10:38:02 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5090178202.tar` & `recon_lw-2.0.0.dev5131824702.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-26 11:12:39.000000 recon_lw-2.0.0.dev5090178202/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    29010 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15455 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-31 10:37:42.000000 recon_lw-2.0.0.dev5131824702/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30669 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15364 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:38:02.000000 recon_lw-2.0.0.dev5131824702/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-31 10:37:19.000000 recon_lw-2.0.0.dev5131824702/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5090178202/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5131824702/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5090178202/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5131824702/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5090178202/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5131824702/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5090178202/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5131824702/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5090178202/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5131824702/recon_lw/recon_ob.py`

 * *Files 2% similar despite different names*

```diff
@@ -533,14 +533,17 @@
 def ob_aggr_add_level(side: str, level: int, price: float, real_qty: int, real_num_orders: int, impl_qty: int,
                       impl_num_orders: int, str_time_of_event, order_book: dict):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
+    #is it purely implied
+    order_book["implied_only"] = (real_num_orders == 0)
+
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side + "_aggr"
     new_index = level - 1
     if not 0 <= new_index <= len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body, []
@@ -566,14 +569,17 @@
     result_body = {}
     side_key = side + "_aggr"
     del_index = level - 1
     if not 0 <= del_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body, []
 
+    #is it purely implied
+    order_book["implied_only"] = (order_book[side_key]["real_num_orders"] == 0)
+
     order_book[side_key].pop(del_index)
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
@@ -590,14 +596,19 @@
     max_levels = order_book["aggr_max_levels"]
     side_key = side + "_aggr"
     update_index = level - 1
     if not 0 <= update_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body, []
 
+    #is it purely implied
+    order_book["implied_only"] = (order_book[side_key]["real_num_orders"] == real_num_orders) and \
+                                 (order_book[side_key]["real_qty"] == real_qty)
+
+
     upd_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders,
                  "impl_qty": impl_qty, "impl_num_orders": impl_num_orders}
     order_book[side_key][update_index].update(upd_level)
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
 
@@ -647,14 +658,43 @@
                   bid_price: int, bid_real_qty: str, bid_impl_qty: str, bid_real_n_orders: int, bid_impl_n_orders: str,
                   str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
+    #is it purely implied
+    sell_implieds_only = False
+    if float(ask_price) == float(order_book["ask_price"]):
+        if ask_real_n_orders == order_book["ask_real_n_orders"]:
+            sell_implieds_only = True
+    if float(ask_price) > float(order_book["ask_price"]):
+        if ask_impl_n_orders != "0" and \
+                ask_real_n_orders == "0":
+            sell_implieds_only = True
+    if float(ask_price) < float(order_book["ask_price"]):
+        if order_book["ask_impl_n_orders"] != "0" and \
+                order_book["ask_real_n_orders"] == "0":
+            sell_implieds_only = True
+
+    buy_implieds_only = False
+    if float(bid_price) == float(order_book["bid_price"]):
+        if bid_real_n_orders == order_book["bid_real_n_orders"]:
+            buy_implieds_only = True
+    if float(bid_price) < float(order_book["bid_price"]):
+        if bid_impl_n_orders != "0" and \
+                bid_real_n_orders == "0":
+            buy_implieds_only = True
+    if float(bid_price) < float(order_book["bid_price"]):
+        if order_book["bid_impl_n_orders"] != "0" and \
+                order_book["bid_real_n_orders"] == "0":
+            buy_implieds_only = True
+    order_book["implied_only"] = sell_implieds_only and buy_implieds_only
+
+
     order_book["ask_price"] = ask_price
     order_book["ask_real_qty"] = ask_real_qty
     order_book["ask_impl_qty"] = ask_impl_qty
     order_book["ask_real_n_orders"] = ask_real_n_orders
     order_book["ask_impl_n_orders"] = ask_impl_n_orders
     order_book["bid_price"] = bid_price
     order_book["bid_real_qty"] = bid_real_qty
```

### Comparing `recon_lw-2.0.0.dev5090178202/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5131824702/recon_lw/recon_ob_cross_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     problems = []
     for side in ["ask", "bid"]:
         full_levels = list(full_book[side].keys())
         if side == "ask":
             full_levels.sort()
         else:
             full_levels.sort(reverse=True)
-        aggr_levels = aggr_book[side + "_aggr"]
+        aggr_levels = [level for level in aggr_book[side + "_aggr"] if level["real_num_orders"] != "0"]
         for i in range(aggr_book["aggr_max_levels"]):
             if i < len(full_levels) and i < len(aggr_levels):
                 price_condition = full_levels[i] == aggr_levels[i]["price"]
                 num_orders_condition = len(full_book[side][full_levels[i]]) == \
-                                       (aggr_levels[i]["real_num_orders"] + aggr_levels[i]["impl_num_orders"])
+                                       (aggr_levels[i]["real_num_orders"])
                 size_condition = sum(full_book[side][full_levels[i]].values()) == \
-                                 (aggr_levels[i]["real_qty"] + aggr_levels[i]["impl_qty"])
+                                 (aggr_levels[i]["real_qty"])
                 if not (price_condition and num_orders_condition and size_condition):
                     problems.append({"synopsys": synopsys(price_condition, num_orders_condition, size_condition),
                                      "side": side,
                                      "level": i + 1})
             elif i >= len(full_levels) and i >= len(aggr_levels):
                 break
             elif i >= len(full_levels):
@@ -47,58 +47,58 @@
 
     return problems
 
 
 def compare_full_vs_top(full_book: dict, top_book: dict):
     problems = []
     if len(full_book["ask"]) > 0:
-        if top_book["ask_real_qty"] == 0 and top_book["ask_impl_qty"] == 0:
+        if top_book["ask_real_qty"] == 0:
             problems.append({"synopsys": "top_miss_level", "side": "ask"})
         else:
             top_p = min(full_book["ask"].keys())
             price_condition = top_p == top_book["ask_price"]
             num_orders_condition = len(full_book["ask"][top_p]) == \
-                                   (top_book["ask_impl_n_orders"] + top_book["ask_real_n_orders"])
-            size_condition = sum(full_book["ask"][top_p].values()) == (
-                    top_book["ask_real_qty"] + top_book["ask_impl_qty"])
+                                   (top_book["ask_real_n_orders"])
+            size_condition = sum(full_book["ask"][top_p].values()) == (top_book["ask_real_qty"])
             if not (price_condition and num_orders_condition and size_condition):
                 problems.append({"synopsys": synopsys(price_condition, num_orders_condition, size_condition),
                                  "side": "ask"})
     else:
-        if top_book["ask_real_qty"] != 0 or top_book["ask_impl_qty"] != 0:
+        if top_book["ask_real_qty"] != 0:
             problems.append({"synopsys": "full_miss_level", "side": "ask"})
 
     if len(full_book["bid"]) > 0:
-        if top_book["bid_real_qty"] == 0 and top_book["bid_impl_qty"] == 0:
+        if top_book["bid_real_qty"] == 0:
             problems.append({"synopsys": "top_miss_level", "side": "bid"})
         else:
             top_p = max(full_book["bid"].keys())
             price_condition = top_p == top_book["bid_price"]
             num_orders_condition = len(full_book["bid"][top_p]) == \
-                                   (top_book["bid_impl_n_orders"] + top_book["bid_real_n_orders"])
-            size_condition = sum(full_book["bid"][top_p].values()) == (
-                    top_book["bid_real_qty"] + top_book["bid_impl_qty"])
+                                   (top_book["bid_real_n_orders"])
+            size_condition = sum(full_book["bid"][top_p].values()) == (top_book["bid_real_qty"])
             if not (price_condition and num_orders_condition and size_condition):
                 problems.append({"synopsys": synopsys(price_condition, num_orders_condition, size_condition),
                                  "side": "bid"})
     else:
-        if top_book["bid_real_qty"] != 0 or top_book["bid_impl_qty"] != 0:
+        if top_book["bid_real_qty"] != 0:
             problems.append({"synopsys": "full_miss_level", "side": "bid"})
     return problems
 
 
 def ob_compare_get_timestamp_key1_key2_aggr(o, custom_settings):
     if o["body"]["aggr_seq"]["limit_delta"] not in [1, 2]:
         return None, None, None
     if o["body"]["sessionId"] == custom_settings["full_session"]:
         return o["body"]["timestamp"], "{0}_{1}_{2}".format(o["body"]["book_id"],
                                                             o["body"]["time_of_event"],
                                                             o["body"]["aggr_seq"]["limit_v2"]), None
 
     if o["body"]["sessionId"] == custom_settings["comp_session"]:
+        if "implied_only" in o["body"] and o["body"]["implied_only"]:
+            return None, None, None
         return o["body"]["timestamp"], None, "{0}_{1}_{2}".format(o["body"]["book_id"],
                                                                   o["body"]["time_of_event"],
                                                                   o["body"]["aggr_seq"]["limit_v2"])
 
     return None, None, None
 
 
@@ -108,14 +108,16 @@
 
     if o["body"]["sessionId"] == custom_settings["full_session"]:
         return o["body"]["timestamp"], "{0}_{1}_{2}".format(o["body"]["book_id"],
                                                             o["body"]["time_of_event"],
                                                             o["body"]["aggr_seq"]["top_v2"]), None
 
     if o["body"]["sessionId"] == custom_settings["comp_session"]:
+        if "implied_only" in o["body"] and o["body"]["implied_only"]:
+            return None, None, None
         return o["body"]["timestamp"], None, "{0}_{1}_{2}".format(o["body"]["book_id"],
                                                                   o["body"]["time_of_event"],
                                                                   o["body"]["aggr_seq"]["top_v2"])
 
     return None, None, None
```

### Comparing `recon_lw-2.0.0.dev5090178202/setup.py` & `recon_lw-2.0.0.dev5131824702/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5090178202/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5131824702/test/test_recon_ob.py`

 * *Files identical despite different names*

