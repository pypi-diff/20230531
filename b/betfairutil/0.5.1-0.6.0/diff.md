# Comparing `tmp/betfairutil-0.5.1.tar.gz` & `tmp/betfairutil-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfairutil-0.5.1.tar", last modified: Sat Feb 25 08:36:13 2023, max compression
+gzip compressed data, was "betfairutil-0.6.0.tar", last modified: Wed May 31 11:58:05 2023, max compression
```

## Comparing `betfairutil-0.5.1.tar` & `betfairutil-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mberk     (1000) mberk     (1000)        0 2023-02-25 08:36:13.139433 betfairutil-0.5.1/
--rw-r--r--   0 mberk     (1000) mberk     (1000)     1062 2021-07-12 09:03:49.000000 betfairutil-0.5.1/LICENSE
--rw-rw-r--   0 mberk     (1000) mberk     (1000)     7231 2023-02-25 08:36:13.139433 betfairutil-0.5.1/PKG-INFO
--rw-rw-r--   0 mberk     (1000) mberk     (1000)     6693 2023-01-13 07:10:05.000000 betfairutil-0.5.1/README.md
-drwxrwxr-x   0 mberk     (1000) mberk     (1000)        0 2023-02-25 08:36:13.135433 betfairutil-0.5.1/betfairutil/
--rw-rw-r--   0 mberk     (1000) mberk     (1000)    84631 2023-02-25 08:36:01.000000 betfairutil-0.5.1/betfairutil/__init__.py
-drwxrwxr-x   0 mberk     (1000) mberk     (1000)        0 2023-02-25 08:36:13.139433 betfairutil-0.5.1/betfairutil.egg-info/
--rw-r--r--   0 mberk     (1000) mberk     (1000)     7231 2023-02-25 08:36:12.000000 betfairutil-0.5.1/betfairutil.egg-info/PKG-INFO
--rw-r--r--   0 mberk     (1000) mberk     (1000)      224 2023-02-25 08:36:13.000000 betfairutil-0.5.1/betfairutil.egg-info/SOURCES.txt
--rw-r--r--   0 mberk     (1000) mberk     (1000)        1 2023-02-25 08:36:12.000000 betfairutil-0.5.1/betfairutil.egg-info/dependency_links.txt
--rw-r--r--   0 mberk     (1000) mberk     (1000)       95 2023-02-25 08:36:13.000000 betfairutil-0.5.1/betfairutil.egg-info/requires.txt
--rw-r--r--   0 mberk     (1000) mberk     (1000)       12 2023-02-25 08:36:13.000000 betfairutil-0.5.1/betfairutil.egg-info/top_level.txt
--rw-rw-r--   0 mberk     (1000) mberk     (1000)       38 2023-02-25 08:36:13.139433 betfairutil-0.5.1/setup.cfg
--rw-rw-r--   0 mberk     (1000) mberk     (1000)      916 2023-02-25 08:36:01.000000 betfairutil-0.5.1/setup.py
+drwxrwxr-x   0 mberk     (1001) mberk     (1001)        0 2023-05-31 11:58:05.219445 betfairutil-0.6.0/
+-rw-r--r--   0 mberk     (1001) mberk     (1001)     1062 2021-07-12 09:03:49.000000 betfairutil-0.6.0/LICENSE
+-rw-rw-r--   0 mberk     (1001) mberk     (1001)     7231 2023-05-31 11:58:05.219445 betfairutil-0.6.0/PKG-INFO
+-rw-rw-r--   0 mberk     (1001) mberk     (1001)     6693 2023-01-13 07:10:05.000000 betfairutil-0.6.0/README.md
+drwxrwxr-x   0 mberk     (1001) mberk     (1001)        0 2023-05-31 11:58:05.215445 betfairutil-0.6.0/betfairutil/
+-rw-rw-r--   0 mberk     (1001) mberk     (1001)    95907 2023-05-31 11:29:19.000000 betfairutil-0.6.0/betfairutil/__init__.py
+drwxrwxr-x   0 mberk     (1001) mberk     (1001)        0 2023-05-31 11:58:05.219445 betfairutil-0.6.0/betfairutil.egg-info/
+-rw-r--r--   0 mberk     (1001) mberk     (1001)     7231 2023-05-31 11:58:04.000000 betfairutil-0.6.0/betfairutil.egg-info/PKG-INFO
+-rw-r--r--   0 mberk     (1001) mberk     (1001)      224 2023-05-31 11:58:05.000000 betfairutil-0.6.0/betfairutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 mberk     (1001) mberk     (1001)        1 2023-05-31 11:58:04.000000 betfairutil-0.6.0/betfairutil.egg-info/dependency_links.txt
+-rw-r--r--   0 mberk     (1001) mberk     (1001)       95 2023-05-31 11:58:04.000000 betfairutil-0.6.0/betfairutil.egg-info/requires.txt
+-rw-rw-r--   0 mberk     (1001) mberk     (1001)       12 2023-05-31 11:58:05.000000 betfairutil-0.6.0/betfairutil.egg-info/top_level.txt
+-rw-rw-r--   0 mberk     (1001) mberk     (1001)       38 2023-05-31 11:58:05.219445 betfairutil-0.6.0/setup.cfg
+-rw-r--r--   0 mberk     (1001) mberk     (1001)      916 2023-05-31 11:30:03.000000 betfairutil-0.6.0/setup.py
```

### Comparing `betfairutil-0.5.1/LICENSE` & `betfairutil-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `betfairutil-0.5.1/PKG-INFO` & `betfairutil-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfairutil
-Version: 0.5.1
+Version: 0.6.0
 Summary: Utility functions for working with Betfair data
 Home-page: https://github.com/mberk/betfairutil
 Author: Maurice Berk
 Author-email: maurice@mauriceberk.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betfairutil-0.5.1/README.md` & `betfairutil-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `betfairutil-0.5.1/betfairutil/__init__.py` & `betfairutil-0.6.0/betfairutil/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import datetime
 import enum
 import heapq
 import itertools
 import re
 from bisect import bisect_left
 from bisect import bisect_right
+from collections import deque
 from copy import deepcopy
+from math import asin
+from math import cos
+from math import radians
+from math import sin
 from math import sqrt
 from pathlib import Path
 from typing import (
     Any,
     Dict,
     Generator,
     List,
     Mapping,
     Optional,
     Sequence,
+    Set,
     Tuple,
     TYPE_CHECKING,
     Union,
 )
 
 if TYPE_CHECKING:
     import pandas as pd
@@ -1441,14 +1447,15 @@
 EX_KEYS = ["availableToBack", "availableToLay", "tradedVolume"]
 MARKET_ID_PATTERN = re.compile(r"1\.\d{9}")
 EVENT_ID_PATTERN = re.compile(r"\d{8}")
 NUMBER_OF_METRES_IN_A_YARD = 0.9144
 RACE_ID_PATTERN = re.compile(r"\d{8}\.\d{4}")
 _INVERSE_GOLDEN_RATIO = 2.0 / (1 + sqrt(5.0))
 _ORIGINAL_OPEN = open
+_AVERAGE_EARTH_RADIUS_IN_METERS = 6371008.8
 
 
 class _OpenMocker:
     def __init__(self, path_to_file: str):
         self.path_to_file = path_to_file
 
     def open(self, file, *args, **kwargs):
@@ -1456,14 +1463,33 @@
             import smart_open
 
             return smart_open.open(file, *args, **kwargs)
         else:
             return _ORIGINAL_OPEN(file, *args, **kwargs)
 
 
+def _load_json_object(o: Union[Dict[str, Any], str, Path]) -> Dict[str, Any]:
+    """
+    Takes either a JSON object and simply returns it or a path to a JSON file containing a JSON
+    object in which case read that file and return the JSON object it contains
+
+    :param o: Either a JSON object or a path to a JSON file containing a JSON object
+    :return: If o is a JSON object then that object; otherwise the JSON object that the file
+        o refers to contains
+    """
+    if isinstance(o, (str, Path)):
+        import orjson
+        import smart_open
+
+        with smart_open.open(o, "r") as f:
+            o = orjson.loads(f.read())
+
+    return o
+
+
 class DataFrameFormatEnum(enum.Enum):
     FULL_LADDER = "FULL_LADDER"
     LAST_PRICE_TRADED = "LAST_PRICE_TRADED"
 
 
 class Side(enum.Enum):
     BACK = "Back"
@@ -1536,14 +1562,45 @@
                 other_best_price_size = get_best_price_size(runner, side.other_side)
                 if other_best_price_size is not None:
                     implied_probabilities.append(1.0)
 
     return sum(implied_probabilities)
 
 
+def calculate_available_volume(
+    market_book: Union[Dict[str, Any], MarketBook],
+    side: Side,
+    max_book_percentage: float,
+) -> float:
+    """
+    Calculate the available volume up to a maximum book_percentage value.
+
+    :param market_book: A market book either as a dictionary or betfairlightweight MarketBook object
+    :param side: Indicate whether to get the available volume on the back or lay side.
+    :param max_book_percentage: Maximum book_percentage value to use for calculating the volume.
+    :return: Available total volume.
+    """
+    available_volume = 0
+    for depth in itertools.count():
+        book_percentage = 0
+        size = 0
+        for runner in market_book["runners"]:
+            runner_price_size = get_price_size_by_depth(
+                runner=runner, side=side, depth=depth
+            )
+            if runner_price_size:
+                book_percentage += 1.0 / runner_price_size["price"]
+                size += runner_price_size["size"]
+            else:
+                return available_volume
+
+        if book_percentage <= max_book_percentage:
+            available_volume += size
+
+
 def calculate_market_book_diff(
     current_market_book: Union[Dict[str, Any], MarketBook],
     previous_market_book: Union[Dict[str, Any], MarketBook],
 ) -> MarketBookDiff:
     """
     Calculate the size differences between amounts available to back, available to lay, and traded between two market books
 
@@ -1767,14 +1824,23 @@
 ) -> Optional[Union[Dict[str, Union[int, float]], PriceSize]]:
     if isinstance(runner, RunnerBook):
         return next(iter(getattr(runner.ex, side.ex_attribute)), None)
     else:
         return next(iter(runner.get("ex", {}).get(side.ex_key, [])), None)
 
 
+def get_mid_price(
+    runner: Union[Dict[str, Any], RunnerBook]
+) -> Optional[Union[int, float]]:
+    best_back = get_best_price(runner, Side.BACK)
+    best_lay = get_best_price(runner, Side.LAY)
+    if best_back is not None and best_lay is not None:
+        return (best_back + best_lay) / 2
+
+
 def get_best_price(
     runner: Union[Dict[str, Any], RunnerBook], side: Side
 ) -> Optional[Union[int, float]]:
     """
     Get the best price available on a runner on side Side. This is a convenience function which retrieves the best price/size pair using get_best_price_size then returns the price field
 
     :param runner: A runner book as either a betfairlightweight RunnerBook object or a dictionary
@@ -2007,21 +2073,23 @@
 
     :param path_to_prices_file: The prices file to search
     :return: None if there are no market definitions in the file, otherwise the last one found, as a dictionary
     """
     import orjson
     import smart_open
 
-    market_definition = None
+    the_line = None
     with smart_open.open(path_to_prices_file, "rb") as f:
         for line in f:
             if b"marketDefinition" in line:
-                market_definition = orjson.loads(line)["mc"][0]["marketDefinition"]
+                the_line = line
 
-    return market_definition
+    if the_line is not None:
+        market_definition = orjson.loads(the_line)["mc"][0]["marketDefinition"]
+        return market_definition
 
 
 def create_market_definition_generator_from_prices_file(
     path_to_prices_file: Union[str, Path]
 ) -> Generator[Tuple[int, Dict[str, Any]], None, None]:
     import orjson
     import smart_open
@@ -2051,28 +2119,111 @@
     _, market_definition = next(
         create_market_definition_generator_from_prices_file(path_to_prices_file),
         (None, None),
     )
     return market_definition
 
 
-def get_pre_event_volume_traded_from_prices_file(
-    path_to_prices_file: Union[str, Path],
-) -> Optional[Union[int, float]]:
+def get_last_pre_event_market_book_from_prices_file(
+    path_to_prices_file: Union[str, Path], filter_suspended: bool = True
+) -> Optional[Dict[str, Any]]:
+    """
+    Search a prices file for the last market book before the market turned in play
+
+    :param path_to_prices_file: The prices file to search
+    :param filter_suspended: Optionally ignore any pre-event market books where the market status is SUSPENDED
+    :return: The last pre-event market book, where the status is not SUSPENDED if filter_suspended has been set to True, provided one such market book exists in the prices file. If not then None will be returned
+    """
     g = create_market_book_generator_from_prices_file(path_to_prices_file)
     pre_event_market_book = None
     for market_book in g:
         if market_book["inplay"]:
-            break
-        pre_event_market_book = market_book
+            return pre_event_market_book
+        if not filter_suspended or market_book["status"] != "SUSPENDED":
+            pre_event_market_book = market_book
+
+
+def get_pre_event_volume_traded_from_prices_file(
+    path_to_prices_file: Union[str, Path],
+) -> Optional[Union[int, float]]:
+    pre_event_market_book = get_last_pre_event_market_book_from_prices_file(
+        path_to_prices_file,
+        filter_suspended=False,
+    )
     if pre_event_market_book is not None:
         pre_event_volume_traded = calculate_total_matched(pre_event_market_book)
         return pre_event_volume_traded
 
 
+def get_inplay_publish_time_from_prices_file(
+    path_to_prices_file: Union[str, Path], as_datetime: bool = False
+) -> Optional[Union[int, datetime.datetime]]:
+    g = create_market_book_generator_from_prices_file(path_to_prices_file)
+    for market_book in g:
+        if market_book["inplay"]:
+            publish_time = market_book["publishTime"]
+            if as_datetime:
+                publish_time = publish_time_to_datetime(publish_time)
+            return publish_time
+
+
+def get_total_volume_traded_from_prices_file(
+    path_to_prices_file: Union[str, Path], deque_len: Optional[int] = 8
+) -> Optional[Union[int, float]]:
+    """
+    Working out the total volume traded on a market is surprisingly tricky given Betfair's shenanigans around the market
+    closure. Specifically, the last few updates in the price stream result in data getting zeroed out which means if you
+    were to just look at the last available market book it would look like the total volume traded was zero. In fact, it
+    appears there is no consistency as to how many price stream updates are involved in this zeroing of data and so it's
+    not as simple as having a rule such as "look at the second to last market book available".
+
+    If memory usage is not an issue then the most robust method would be to read the entire set of market books into
+    memory then iterate them in reverse order looking for the first market book that has a non-zero total volume traded.
+    However, in many use cases memory usage is a significant concern. For example, if you want to process tens of
+    thousands of markets and use parallel processing to speed this up then you end up needing to hold the entire set of
+    market books for multiple markets in memory simultaneously and, depending on the number of cores your machine has
+    and the number of parallel processes you use, it is easy to exhaust the total memory available.
+
+    The solution presented here is to use a deque
+    (https://docs.python.org/3/library/collections.html#collections.deque). Think of this as a limited length list
+    where when a new item is appended to the list, another item is removed for the start of the list. This is used when
+    reading the prices file to leave us with the X last market books which can then be iterated in reverse order to find
+    the last one which has a non-zero volume traded. Based on my own analysis of prices files I have settled on a
+    default maximum length of the deque of 8 - i.e. at most this function will store 8 market books in memory at any one
+    time. This is a trade-off between giving correct results and drastically cutting down on memory usage versus reading
+    the entire set of market books into memory. If memory usage is not of concern to you then you can simply set the
+    deque_len argument to None and the function will read the entire set of market books into memory ensuring
+    correctness. If you observe any prices files where a deque of length 8 doesn't give correct results then please
+    create a GitHub issue here: https://github.com/mberk/betfairutil/issues so I can investigate.
+
+    :param path_to_prices_file: Where the Betfair prices file to be processed is located. This can be a local file, one
+        stored in AWS S3, or any of the other options that can be handled by the smart_open package. The file can be
+        compressed or uncompressed
+    :param deque_len: The length of the deque used to limit memory usage when working out the total volume traded. See
+        discussion above. This can be set to None to use the entire set of market books which should ensure correctness
+        but dramatically increase memory usage
+    :return: The calculated total volume traded if it is available or None if the market was pulled by Betfair (i.e. all
+        runners have a status of "REMOVED")
+    """
+    g = create_market_book_generator_from_prices_file(path_to_prices_file)
+    market_books = deque(g, deque_len)
+    for market_book in reversed(market_books):
+        volume_traded = calculate_total_matched(market_book)
+        if volume_traded > 0:
+            return volume_traded
+        if all(
+            runner["status"] == "REMOVED"
+            for runner in market_book["marketDefinition"]["runners"]
+        ):
+            return None
+
+    if len(market_books) > 0:
+        return 0
+
+
 def _is_exchange_win_market(d: Dict[str, Any]) -> bool:
     return d["marketType"] == "WIN" and d["marketId"].startswith("1.")
 
 
 def get_bsp_from_race_result(
     race_result: Union[Dict[str, Any], str, Path]
 ) -> Dict[int, Optional[Union[int, float]]]:
@@ -2081,20 +2232,15 @@
     undocumented RaceCard endpoint (see
     https://github.com/betcode-org/betfair/blob/master/betfairlightweight/endpoints/racecard.py)
 
     :param race_result: Either the race result object as a dictionary or the path to a JSON file containing the race
         result object
     :return: a dictionary mapping selection ID to Betfair starting price
     """
-    if isinstance(race_result, (str, Path)):
-        import orjson
-        import smart_open
-
-        with smart_open.open(race_result, "r") as f:
-            race_result = orjson.loads(f.read())
+    race_result = _load_json_object(race_result)
 
     bsp = {}
     for runner in race_result["runners"]:
         for selection in runner.get("selections", []):
             if _is_exchange_win_market(selection):
                 selection_id = int(selection["selectionId"])
                 bsp[selection_id] = selection["bsp"]
@@ -2129,23 +2275,53 @@
         for selection in runner.get("selections", []):
             if _is_exchange_win_market(selection):
                 winning_selection_ids.append(int(selection["selectionId"]))
 
     return winning_selection_ids
 
 
-def get_race_distance_in_metres_from_race_card(race_card: Dict[str, Any]) -> float:
+def get_race_distance_in_metres_from_race_card(
+    race_card: Union[Dict[str, Any], str, Path]
+) -> float:
+    """
+    Extract the race distance from a race card object in yards then convert it to metres
+
+    :param race_card: Either the race card object as a dictionary or the path to a JSON file
+        containing the race card object
+    :return: the race distance in metres
+    """
+    race_card = _load_json_object(race_card)
     distance_in_yards = race_card["race"]["distance"]
     distance_in_metres = convert_yards_to_metres(distance_in_yards)
     return distance_in_metres
 
 
+def get_is_jump_from_race_card(race_card: Union[Dict[str, Any], str, Path]) -> bool:
+    race_card = _load_json_object(race_card)
+    race_type = race_card["race"]["raceType"]["full"]
+    return race_type in ("Chase", "Hurdle")
+
+
 def get_win_market_id_from_race_card(
-    race_card: Dict[str, Any], as_integer: bool = False
+    race_card: Union[Dict[str, Any], str, Path], as_integer: bool = False
 ) -> Optional[Union[int, str]]:
+    """
+    Search the markets contained in a race card for the one corresponding to the Exchange WIN
+    market and return its market ID
+
+    :param race_card: Either the race card object as a dictionary or the path to a JSON file
+        containing the race card object
+    :param as_integer: Should the market ID be returned as is - in the standard string form
+        provided by Betfair that starts "1." - or an integer where the "1." prefix has been
+        discarded
+    :return: The market ID corresponding to the Exchange WIN market, as either an integer or
+        a string according to as_integer, if such a market can be found in the race card
+        otherwise None
+    """
+    race_card = _load_json_object(race_card)
     for market in race_card["race"]["markets"]:
         market_id = market["marketId"]
         if market["marketType"] == "WIN" and market_id.startswith("1."):
             if as_integer:
                 market_id = int(market_id[2:])
             return market_id
 
@@ -2979,7 +3155,68 @@
     if not isinstance(i, int) or i <= 0:
         raise ValueError(f"{i} is not a positive integer")
 
     return (0.5 + _INVERSE_GOLDEN_RATIO * i) % 1
 
 
 random_from_event_id = random_from_positive_int
+
+
+def calculate_haversine_distance_between_runners(
+    rrc_a: Dict[str, Any], rrc_b: Dict[str, Any]
+) -> float:
+    """
+    Given two rrc objects from the Betfair race stream, calculate the approximate distance
+    between the horses in metres using the haversine formula
+
+    :param rrc_a: A rrc object from the Betfair race stream as a dictionary
+    :param rrc_b: Another rrc object from the Betfair race stream as a dictionary
+    :return: The approximate distance between the two horses in metres
+    """
+    delta_longitude = radians(rrc_a["long"]) - radians(rrc_b["long"])
+    delta_latitude = radians(rrc_a["lat"]) - radians(rrc_b["lat"])
+    d = (
+        sin(delta_latitude * 0.5) ** 2
+        + cos(radians(rrc_a["lat"]))
+        * cos(radians(rrc_b["lat"]))
+        * sin(delta_longitude * 0.5) ** 2
+    )
+
+    return 2 * _AVERAGE_EARTH_RADIUS_IN_METERS * asin(sqrt(d))
+
+
+def get_number_of_jumps_remaining(rc: Dict[str, Any]) -> Optional[int]:
+    """
+    Given a race change object, work out how many jumps there are between the _leader_ and the
+    finishing line. If there are no jump locations present in the race change object, either
+    because this is a flat race or because it comes from older data that lacks the jump
+    locations, then None will be returned
+
+    :param rc: A Betfair race change object as a Python dictionary
+    :return: The number of jumps between the leader and the finishing line unless there are no
+        jump locations present in the race change object in which case None
+    """
+    distance_remaining = (rc.get("rpc") or {}).get("prg")
+    jumps = (rc.get("rpc") or {}).get("J") or []
+    if distance_remaining is not None and len(jumps) > 0:
+        return sum(j["L"] < distance_remaining for j in jumps)
+
+
+def get_race_leaders(rc: Dict[str, Any]) -> Set[int]:
+    """
+    Given a race change object, return the set of selection IDs of horses which are closest to
+    the finishing line
+
+    :param rc: A Betfair race change object as a Python dictionary
+    :return: A set containing the selection IDs corresponding to the horses which are in the
+        lead. The size of the set may exceed 1 if multiple horses are tied for the lead
+    """
+    distances_remaining = sorted(rrc["prg"] for rrc in (rc.get("rrc") or []))
+    if len(distances_remaining) > 0:
+        leader_distance_remaining = distances_remaining[0]
+        return {
+            rrc["id"]
+            for rrc in (rc.get("rrc") or [])
+            if rrc["prg"] == leader_distance_remaining
+        }
+    else:
+        return set()
```

### Comparing `betfairutil-0.5.1/betfairutil.egg-info/PKG-INFO` & `betfairutil-0.6.0/betfairutil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfairutil
-Version: 0.5.1
+Version: 0.6.0
 Summary: Utility functions for working with Betfair data
 Home-page: https://github.com/mberk/betfairutil
 Author: Maurice Berk
 Author-email: maurice@mauriceberk.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betfairutil-0.5.1/setup.py` & `betfairutil-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 requires = ["betfairlightweight"]
 tests_require = ["pytest"]
 
 setup(
     name="betfairutil",
-    version="0.5.1",
+    version="0.6.0",
     description="Utility functions for working with Betfair data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Maurice Berk",
     author_email="maurice@mauriceberk.com",
     url="https://github.com/mberk/betfairutil",
     packages=["betfairutil"],
```

