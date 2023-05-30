# Comparing `tmp/autobean-format-0.1.3.tar.gz` & `tmp/autobean-format-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobean-format-0.1.3.tar", last modified: Tue Apr  4 15:25:09 2023, max compression
+gzip compressed data, was "autobean-format-0.1.4.tar", last modified: Tue May 30 22:30:36 2023, max compression
```

## Comparing `autobean-format-0.1.3.tar` & `autobean-format-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1065 2023-04-04 15:24:54.942840 autobean-format-0.1.3/LICENSE
--rw-r--r--   0        0        0     1312 2023-04-04 15:24:54.942840 autobean-format-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/__init__.py
--rw-r--r--   0        0        0      460 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/formatter.py
--rw-r--r--   0        0        0      183 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/formatters/__init__.py
--rw-r--r--   0        0        0      966 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/formatters/balance.py
--rw-r--r--   0        0        0     1690 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/formatters/base.py
--rw-r--r--   0        0        0      822 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/formatters/cost.py
--rw-r--r--   0        0        0     2620 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/formatters/file.py
--rw-r--r--   0        0        0      567 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/formatters/number.py
--rw-r--r--   0        0        0     1008 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/formatters/open.py
--rw-r--r--   0        0        0     1573 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/formatters/posting.py
--rw-r--r--   0        0        0      969 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/formatters/price.py
--rw-r--r--   0        0        0     1301 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/formatters/tokens.py
--rw-r--r--   0        0        0        0 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/internal/__init__.py
--rw-r--r--   0        0        0      655 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/internal/alignment.py
--rw-r--r--   0        0        0     1080 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/internal/chrono.py
--rw-r--r--   0        0        0      926 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/internal/iterating.py
--rw-r--r--   0        0        0    12645 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/internal/sorting.py
--rw-r--r--   0        0        0     2788 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/main.py
--rw-r--r--   0        0        0     2623 2023-04-04 15:24:54.942840 autobean-format-0.1.3/autobean_format/options_lib.py
--rw-r--r--   0        0        0      665 2023-04-04 15:24:54.942840 autobean-format-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 autobean-format-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-30 22:30:17.066224 autobean-format-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3634 2023-05-30 22:30:17.066224 autobean-format-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/__init__.py
+-rw-r--r--   0        0        0      460 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/formatter.py
+-rw-r--r--   0        0        0      183 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/formatters/__init__.py
+-rw-r--r--   0        0        0      966 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/formatters/balance.py
+-rw-r--r--   0        0        0     1690 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/formatters/base.py
+-rw-r--r--   0        0        0      822 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/formatters/cost.py
+-rw-r--r--   0        0        0     2620 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/formatters/file.py
+-rw-r--r--   0        0        0      567 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/formatters/number.py
+-rw-r--r--   0        0        0     1008 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/formatters/open.py
+-rw-r--r--   0        0        0     1573 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/formatters/posting.py
+-rw-r--r--   0        0        0      969 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/formatters/price.py
+-rw-r--r--   0        0        0     1301 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/formatters/tokens.py
+-rw-r--r--   0        0        0        0 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/internal/__init__.py
+-rw-r--r--   0        0        0      655 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/internal/alignment.py
+-rw-r--r--   0        0        0     1080 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/internal/chrono.py
+-rw-r--r--   0        0        0      926 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/internal/iterating.py
+-rw-r--r--   0        0        0    13810 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/internal/sorting.py
+-rw-r--r--   0        0        0     2788 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/main.py
+-rw-r--r--   0        0        0     2623 2023-05-30 22:30:17.066224 autobean-format-0.1.4/autobean_format/options_lib.py
+-rw-r--r--   0        0        0      665 2023-05-30 22:30:17.070224 autobean-format-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3861 1970-01-01 00:00:00.000000 autobean-format-0.1.4/PKG-INFO
```

### Comparing `autobean-format-0.1.3/LICENSE` & `autobean-format-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/formatters/balance.py` & `autobean-format-0.1.4/autobean_format/formatters/balance.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/formatters/base.py` & `autobean-format-0.1.4/autobean_format/formatters/base.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/formatters/cost.py` & `autobean-format-0.1.4/autobean_format/formatters/cost.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/formatters/file.py` & `autobean-format-0.1.4/autobean_format/formatters/file.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/formatters/number.py` & `autobean-format-0.1.4/autobean_format/formatters/number.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/formatters/open.py` & `autobean-format-0.1.4/autobean_format/formatters/open.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/formatters/posting.py` & `autobean-format-0.1.4/autobean_format/formatters/posting.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/formatters/price.py` & `autobean-format-0.1.4/autobean_format/formatters/price.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/formatters/tokens.py` & `autobean-format-0.1.4/autobean_format/formatters/tokens.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/internal/alignment.py` & `autobean-format-0.1.4/autobean_format/internal/alignment.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/internal/chrono.py` & `autobean-format-0.1.4/autobean_format/internal/chrono.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/internal/iterating.py` & `autobean-format-0.1.4/autobean_format/internal/iterating.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/internal/sorting.py` & `autobean-format-0.1.4/autobean_format/internal/sorting.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,61 +38,73 @@
 `poptag #foo`, but we don't do it as it may be over-complexing due to possibly interleaving pushes.
 
 Instead of sorting out-of-order entities with simple sort, we could recurse with the same method, but we don't do it
 as it may be over-complexing and degraded performance.
 """
 
 import abc
+import bisect
 import decimal
 import functools
 import heapq
 import itertools
 from typing import TYPE_CHECKING, Any, Generic, Iterable, Iterator, Optional, Self, Sequence, TypeAlias, TypeVar, cast, get_args
 
 from autobean_refactor import models
 from . import chrono
 if TYPE_CHECKING:
     from _typeshed import SupportsDunderLT, SupportsDunderGT
 
 _T = TypeVar('_T')
 _O = TypeVar('_O', bound='_Ordered')
-_Entry: TypeAlias = models.Balance | models.Close | models.Commodity | models.Pad | models.Event | models.Query | models.Price | models.Note | models.Document | models.Custom | models.Transaction
+_Entry: TypeAlias = models.Balance | models.Open | models.Close | models.Commodity | models.Pad | models.Event | models.Query | models.Price | models.Note | models.Document | models.Custom | models.Transaction
 _CompartmentSplitter: TypeAlias = models.Pushtag | models.Poptag | models.Pushmeta | models.Popmeta | models.BlockComment
 _TopLevelEntitiy = models.Directive | models.BlockComment
 
 
 class _Ordered(Generic[_T], abc.ABC):
 
     def __init__(self, value: _T) -> None:
         self.value = value
 
-    # Note: a < b may not imply !(b <= a)
+    # Note: a.more_successor_permissive_than(b) may not imply !(b.can_go_before(a))
     @abc.abstractmethod
-    def __lt__(self, other: object) -> bool:
-        ...
+    def more_successor_permissive_than(self, other: Self) -> bool:
+        """Tests if successors permitted by this entity forms a proper superset of those permitted by the other entity."""
 
-    # Note: <= may not be transitive
+    # Note: may not be transitive
     @abc.abstractmethod
-    def __le__(self, other: object) -> bool:
-        ...
+    def can_go_before(self, other: Self) -> bool:
+        """Tests if this entity can go before the other entity."""
 
     @classmethod
     @abc.abstractmethod
     def min(cls, a: Self, b: Self) -> Self:
-        ...
+        """An associative function to summarize the lower bound for can_go_before.
+        
+        Formally:
+        forall x: x.can_go_before(a) && x.can_go_before(b) <=> x.can_go_before(min(a, b))
+        """
 
     @classmethod
     @abc.abstractmethod
     def max(cls, a: Self, b: Self) -> Self:
-        ...
+        """An associative function to summarize the upper bound for can_go_before.
+
+        Formally:
+        forall x: a.can_go_before(x) && b.can_go_before(x) <=> max(a, b).can_go_before(x)
+        """
 
     @classmethod
     @abc.abstractmethod
     def merge(cls, sorted: list[Self], unsorted: list[Self]) -> Iterable[Self]:
-        ...
+        """Merges a sorted list with an unsorted list into a sorted list.
+
+        The original order of `sorted` must be preserved.
+        """
 
     @classmethod
     def sort(cls, values: list[Self]) -> list[Self]:
         if _is_ordered(values):
             return values
         sorted, unsorted = _split_sorted_unsorted(values)
         return list(cls.merge(sorted, unsorted))
@@ -100,47 +112,55 @@
 
 def _is_ordered(entities: Sequence[_Ordered[_T]]) -> bool:
     if not entities:
         return True
     it = iter(entities)
     running_max = next(it)
     for entity in it:
-        if not running_max <= entity:
+        if not running_max.can_go_before(entity):
             return False
         running_max = running_max.max(running_max, entity)
     return True
 
 
 def _split_sorted_unsorted(
     entities: Sequence[_O],
 ) -> tuple[list[_O], list[_O]]:
+    # (running max index, entity index) -> (prev running max index, prev entity index)
+    p = dict[tuple[int, int], tuple[int, int]]()
+    m = list[tuple[int, int]]()  # length -> (running max index, last entity index)
+
+    for i, entity in enumerate(entities):
+        # first element we cannot go after
+        j = bisect.bisect_left(m, True, key=lambda item: not entities[item[0]].can_go_before(entity))
+        while j >= 0 and (j == len(m) or entity.more_successor_permissive_than(entities[m[j][0]])):
+            running_max = i
+            if j:
+                if entity.max(entity, entities[m[j - 1][0]]) is not entity:
+                    running_max = m[j - 1][0]
+                p[(running_max, i)] = m[j - 1]
+            m[j:j+1] = [(running_max, i)]
+            j -= 1
+        
+    last = m[-1] if m else None
+    sorted_i, sorted, unsorted = [], [], []
+    while last:
+        sorted_i.append(last[1])
+        last = p.get(last)
+    sorted_i.reverse()
 
-    # (length, running_max, prev)
-    l = [(1, entity, -1) for entity in entities]
-    sorted, unsorted = [], []
-    max_len, last = 0, -1
+    sorted = [entities[i] for i in sorted_i]
+    j = 0
     for i in range(len(entities)):
-        for j in range(i):
-            length, running_max, _ = l[j]
-            if not running_max <= entities[i] or length + 1 < l[i][0]:
-                continue
-            running_max = running_max.max(running_max, entities[i])
-            if length + 1 > l[i][0] or running_max < l[i][1]:
-                l[i] = (length + 1, running_max, j)
-        if l[i][0] > max_len:
-            max_len = l[i][0]
-            last = i
-    unsorted.append(entities[last+1:])
-    while last >= 0:
-        sorted.append(entities[last])
-        prev = l[last][2]
-        unsorted.append(entities[prev + 1:last])
-        last = prev
-    sorted.reverse()
-    return sorted, list(itertools.chain.from_iterable(reversed(unsorted)))
+        if j < len(sorted_i) and i == sorted_i[j]:
+            j += 1
+        else:
+            unsorted.append(entities[i])
+
+    return sorted, unsorted
 
 
 def _get_entry_time(entry: _Entry) -> int | None:
     time = entry.meta.get('time')
     if isinstance(time, str):
         return chrono.try_normalize_timestring(entry.date, time)
     elif isinstance(time, decimal.Decimal):
@@ -158,22 +178,22 @@
 
 
 def _merge_entries(sorted: Sequence['_OrderedEntry'], unsorted: Sequence['_OrderedEntry']) -> Iterator[Sequence['_OrderedEntry']]:
     cursor_sorted, cursor_unsorted = 0, 0
     reversed_running_min_unsorted = _build_reversed_running_min(unsorted)
     while cursor_sorted < len(sorted) and cursor_unsorted < len(unsorted):
         prev_cursor_sorted = cursor_sorted
-        while cursor_sorted < len(sorted) and sorted[cursor_sorted] <= reversed_running_min_unsorted[cursor_unsorted]:
+        while cursor_sorted < len(sorted) and sorted[cursor_sorted].can_go_before(reversed_running_min_unsorted[cursor_unsorted]):
             cursor_sorted += 1
         if cursor_sorted > prev_cursor_sorted:
             yield sorted[prev_cursor_sorted:cursor_sorted]
         if cursor_sorted == len(sorted):
             break
         prev_cursor_unsorted = cursor_unsorted
-        while cursor_unsorted < len(unsorted) and reversed_running_min_unsorted[cursor_unsorted] < sorted[cursor_sorted]:
+        while cursor_unsorted < len(unsorted) and not sorted[cursor_sorted].can_go_before(reversed_running_min_unsorted[cursor_unsorted]):
             cursor_unsorted += 1
         yield unsorted[prev_cursor_unsorted:cursor_unsorted]
     if cursor_sorted < len(sorted):
         yield sorted[cursor_sorted:]
     if cursor_unsorted < len(unsorted):
         yield unsorted[cursor_unsorted:]
 
@@ -181,25 +201,22 @@
 class _OrderedEntry(_Ordered[_Entry]):
 
     def __init__(self, entry: _Entry) -> None:
         super().__init__(entry)
         self.date = entry.date
         self.time = _get_entry_time(entry)
 
-    def __lt__(self, other: object) -> bool:
-        if not isinstance(other, _OrderedEntry):
-            return NotImplemented
-        return self.date < other.date or (
-            self.date == other.date and self.time is not None and other.time is not None and self.time < other.time
-        )
-
-    def __le__(self, other: object) -> bool:
-        if not isinstance(other, _OrderedEntry):
-            return NotImplemented
-        return not other < self
+    def more_successor_permissive_than(self, other: Self) -> bool:
+        return self.date < other.date or (self.date == other.date and (
+            self.time is None and other.time is not None or
+            self.time is not None and other.time is not None and self.time < other.time))
+
+    def can_go_before(self, other: Self) -> bool:
+        return self.date < other.date or (self.date == other.date and (
+            self.time is None or other.time is None or self.time <= other.time))
 
     @classmethod
     def min(cls, a: Self, b: Self) -> Self:
         if a.date < b.date or (a.date == b.date and (
                 b.time is None or (a.time is not None and a.time < b.time))):
             return a
         return b
@@ -208,15 +225,15 @@
     def max(cls, a: Self, b: Self) -> Self:
         if a.date < b.date or (a.date == b.date and (
                 a.time is None or (b.time is not None and a.time < b.time))):
             return b
         return a
 
     def simple_sort_key(self) -> Any:
-        return (self.date, self.time)
+        return (self.date, self.time or 0)
 
     @classmethod
     def merge(cls, sorted: list['_OrderedEntry'], unsorted: list['_OrderedEntry']) -> Iterator['_OrderedEntry']:
         unsorted.sort(key=lambda x: x.simple_sort_key())
         return itertools.chain.from_iterable(_merge_entries(sorted, unsorted))
 
 
@@ -247,66 +264,63 @@
     def _min(self) -> Optional['_OrderedEntry']:
         if not self.entries:
             return None
         return functools.reduce(_OrderedEntry.min, self.entries)
 
     @classmethod
     def min(cls, a: Self, b: Self) -> Self:
-        if not b._min or not b._max or (a._min and a._max and (
-                a._min < b._min or a._min <= b._min and a._max <= b._max)):
+        if (not b._min or (a._min and _OrderedEntry.min(a._min, b._min) is a._min)):
             return a
         return b
 
     @classmethod
     def max(cls, a: Self, b: Self) -> Self:
-        if not a._min or not a._max or (b._min and b._max and (
-                a._min < b._min or a._min <= b._min and a._max <= b._max)):
+        if (not a._max or (b._max and _OrderedEntry.max(a._max, b._max) is b._max)):
             return b
         return a
 
-    def __lt__(self, other: object) -> bool:
-        if not isinstance(other, _OrderedBlock):
-            return NotImplemented
+    def more_successor_permissive_than(self, other: Self) -> bool:
         return bool(
-            self._min and self._max and other._min and other._max and
-            self._max <= other._min and other._max > self._min)
+            not self._max and other._max or  # undated is more permissive than dated
+            self._max and other._max and self._max.more_successor_permissive_than(other._max)
+        )
 
-    def __le__(self, other: object) -> bool:
-        if not isinstance(other, _OrderedBlock):
-            return NotImplemented
-        return bool(not self._max or not other._min or self._max <= other._min)
+    def can_go_before(self, other: Self) -> bool:
+        return bool(not self._max or not other._min or self._max.can_go_before(other._min))
 
     def simple_sort_key(self) -> Any:
-        return (self._min and self._min.simple_sort_key(), self._max and self._max.simple_sort_key())
+        assert self._min and self._max  # undated blocks must be part of sorted
+        return (self._min.simple_sort_key(), self._max.simple_sort_key())
 
     @classmethod
     def merge(cls, sorted: list['_OrderedBlock'], unsorted: list['_OrderedBlock']) -> Iterator['_OrderedBlock']:
-        keyed_unsorted = [(block.simple_sort_key(), block) for block in unsorted]
+        keyed_unsorted = [(block.simple_sort_key(), i, block) for i, block in enumerate(unsorted)]
         heapq.heapify(keyed_unsorted)
         cursor_sorted = 0
         while cursor_sorted < len(sorted) and keyed_unsorted:
-            if sorted[cursor_sorted] <= keyed_unsorted[0][1]:
+            if sorted[cursor_sorted].can_go_before(keyed_unsorted[0][2]):
                 yield sorted[cursor_sorted]
                 cursor_sorted += 1
-            elif keyed_unsorted[0][1] <= sorted[cursor_sorted]:
-                yield heapq.heappop(keyed_unsorted)[1]
+            elif keyed_unsorted[0][2].can_go_before(sorted[cursor_sorted]):
+                yield heapq.heappop(keyed_unsorted)[2]
             else:
                 sorted_head_entries = sorted[cursor_sorted].entries
                 cursor_sorted += 1
-                unsorted_head_entries = heapq.heappop(keyed_unsorted)[1].entries
+                unsorted_block = heapq.heappop(keyed_unsorted)
+                unsorted_head_entries = unsorted_block[2].entries
                 assert sorted_head_entries is not None
                 assert unsorted_head_entries is not None
                 split_blocks = _merge_entries(sorted_head_entries, unsorted_head_entries)
                 for block in split_blocks:
                     ordered_block = _OrderedBlock(block)
-                    heapq.heappush(keyed_unsorted, (ordered_block.simple_sort_key(), ordered_block))
+                    heapq.heappush(keyed_unsorted, (ordered_block.simple_sort_key(), unsorted_block[1], ordered_block))
         if cursor_sorted < len(sorted):
             yield from sorted[cursor_sorted:]
         while keyed_unsorted:
-            yield heapq.heappop(keyed_unsorted)[1]
+            yield heapq.heappop(keyed_unsorted)[2]
 
 
 def _sort_compartment(blocks: list[_OrderedBlock]) -> list[Sequence[_TopLevelEntitiy]]:
     blocks = _OrderedBlock.sort(blocks)
 
     sorted_blocks = list[Sequence[_TopLevelEntitiy]]()
     for ordered_block in blocks:
```

### Comparing `autobean-format-0.1.3/autobean_format/main.py` & `autobean-format-0.1.4/autobean_format/main.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/autobean_format/options_lib.py` & `autobean-format-0.1.4/autobean_format/options_lib.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.3/pyproject.toml` & `autobean-format-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "autobean-format"
-version = "0.1.3"
+version = "0.1.4"
 description = "Yet another formatter for beancount"
 authors = [
     { name = "SEIAROTg", email = "seiarotg@gmail.com" },
 ]
 dependencies = [
     "autobean-refactor>=0.2.3",
 ]
```

