# Comparing `tmp/exchange_calendars_extensions-0.1.1.tar.gz` & `tmp/exchange_calendars_extensions-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_calendars_extensions-0.1.1.tar", max compression
+gzip compressed data, was "exchange_calendars_extensions-0.2.1.tar", max compression
```

## Comparing `exchange_calendars_extensions-0.1.1.tar` & `exchange_calendars_extensions-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-03-03 22:41:58.709034 exchange_calendars_extensions-0.1.1/LICENSE
--rw-r--r--   0        0        0     8258 2023-03-03 22:41:58.709034 exchange_calendars_extensions-0.1.1/README.md
--rw-r--r--   0        0        0     4553 2023-03-03 22:41:58.709034 exchange_calendars_extensions-0.1.1/exchange_calendars_extensions/__init__.py
--rw-r--r--   0        0        0     4691 2023-03-03 22:41:58.709034 exchange_calendars_extensions-0.1.1/exchange_calendars_extensions/holiday.py
--rw-r--r--   0        0        0    12970 2023-03-03 22:41:58.709034 exchange_calendars_extensions-0.1.1/exchange_calendars_extensions/holiday_calendar.py
--rw-r--r--   0        0        0     1363 2023-03-03 22:41:58.709034 exchange_calendars_extensions-0.1.1/exchange_calendars_extensions/observance.py
--rw-r--r--   0        0        0     4616 2023-03-03 22:41:58.709034 exchange_calendars_extensions-0.1.1/exchange_calendars_extensions/offset.py
--rw-r--r--   0        0        0     2344 2023-03-03 22:41:58.709034 exchange_calendars_extensions-0.1.1/exchange_calendars_extensions/util.py
--rw-r--r--   0        0        0     1436 2023-03-03 22:41:58.709034 exchange_calendars_extensions-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9680 1970-01-01 00:00:00.000000 exchange_calendars_extensions-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/LICENSE
+-rw-r--r--   0        0        0    22327 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/README.md
+-rw-r--r--   0        0        0    22374 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/__init__.py
+-rw-r--r--   0        0        0    27151 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/changeset.py
+-rw-r--r--   0        0        0     6780 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/holiday.py
+-rw-r--r--   0        0        0    37920 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/holiday_calendar.py
+-rw-r--r--   0        0        0     1674 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/observance.py
+-rw-r--r--   0        0        0     5720 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/offset.py
+-rw-r--r--   0        0        0     2611 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/util.py
+-rw-r--r--   0        0        0     1485 2023-05-31 11:16:28.649816 exchange_calendars_extensions-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    23639 1970-01-01 00:00:00.000000 exchange_calendars_extensions-0.2.1/PKG-INFO
```

### Comparing `exchange_calendars_extensions-0.1.1/LICENSE` & `exchange_calendars_extensions-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.1.1/exchange_calendars_extensions/observance.py` & `exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/observance.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,20 +2,31 @@
 
 import pandas as pd
 from exchange_calendars.exchange_calendar import HolidayCalendar
 
 
 def get_roll_backward_observance(calendar: HolidayCalendar) -> Callable[[pd.Timestamp], pd.Timestamp]:
     """
-        Return a function that rolls back a date to the last regular business day, according to a given holiday
-        calendar.
+    Return a function that rolls back a date to the last regular business day, according to a given holiday
+    calendar.
+
+    Regular business days are those days that are not defined as holidays by the given holiday calendar. This means,
+    for example, that the calendar also needs to define weekend days as holidays to avoid rolling a date back to
+    weekend day.
 
-        Regular business days are those days that are not defined as holidays by the given holiday calendar. This means,
-        for example, that the calendar must also define weekend days as holidays to avoid rolling the date back to a
-        such day.
+    Parameters
+    ----------
+    calendar : HolidayCalendar
+        The holiday calendar to use for determining holidays.
+
+    Returns
+    -------
+    Callable[[pd.Timestamp], pd.Timestamp]
+        A function that takes a date and returns the last business day on or before that date, according to the given
+        calendar.
     """
 
     def f(date: pd.Timestamp) -> pd.Timestamp:
         # Repeat until done.
         while True:
             # A date a few days in the past, relative to the current date.
             limit = date - pd.Timedelta(days=5)
```

### Comparing `exchange_calendars_extensions-0.1.1/exchange_calendars_extensions/offset.py` & `exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/offset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime, date
+from typing import Type, Callable
 
 import pandas as pd
 from pandas._libs.tslibs import localize_pydatetime
 from pandas._libs.tslibs.offsets import Easter, apply_wraps
 
 from exchange_calendars_extensions.util import get_month_name, get_day_of_week_name, third_day_of_week_in_month, \
     last_day_in_month
@@ -15,20 +16,16 @@
         if dt.hour != 0 or dt.minute != 0 or dt.second != 0 or dt.microsecond != 0:
             # Regardless of whether dt is datetime vs Timestamp
             return False
         if isinstance(dt, pd.Timestamp):
             return dt.nanosecond == 0
         return True
 
-    """
-    Auxiliary class for DateOffset instances for the different holidays.
-    """
-
     @property
-    def holiday(self):
+    def holiday(self, year: int):
         """
         Return the Gregorian date for the holiday in a given Gregorian calendar
         year.
         """
         ...  # pragma: no cover
 
     @apply_wraps
@@ -61,27 +58,39 @@
 
     def is_on_offset(self, dt):
         if self.normalize and not AbstractHolidayOffset._is_normalized(dt):
             return False
         return date(dt.year, dt.month, dt.day) == self.holiday(dt.year).to_pydate()
 
 
-def get_third_day_of_week_in_month_offset_class(day_of_week: int, month: int) -> AbstractHolidayOffset:
+def get_third_day_of_week_in_month_offset_class(day_of_week: int, month: int) -> Type[AbstractHolidayOffset]:
     """
-    Return a new class that represents an offset that when applied to the first day of a year, results in the third given 
-    day of the week in the given month.
+    Return a new class that represents an offset that, when applied to the first day of a year, results in the third
+    given day of the week in the given month.
     
-    For example, to get the offset for the third Friday in June, call this function with day_of_week=4 and month=6. On many
-    exchanges, this will be the quadruple witching day for the second quarter of the year.
+    For example, to get the offset for the third Friday in June, call this function with day_of_week=4 and month=6. On
+    many exchanges, this will be the quadruple witching day for the second quarter of the year.
+
+    Parameters
+    ----------
+    day_of_week : int
+        The day of the week, where 0 is Monday and 6 is Sunday.
+    month : int
+        The month, where 1 is January and 12 is December.
+
+    Returns
+    -------
+    Type[AbstractHolidayOffset]
+        A new class that represents the offset.
     """
 
     @property
-    def holiday(self):
+    def holiday(self) -> Callable[[int], pd.Timestamp]:
         """
-            Return a function that returns the date of the day for a given year.
+        Return a function that returns the third instance of the given day of the week in the given month and year.
         """
         return lambda year: third_day_of_week_in_month(day_of_week, month, year)
 
     # Get name of day of week.
     day_of_week_name = get_day_of_week_name(day_of_week)
 
     # Get name of month.
@@ -92,33 +101,49 @@
         "holiday": holiday,
     })
 
     # Return the new class.
     return offset
 
 
-# A dictionary of dictionaries that maps day of week to month to corresponding offset class.
+# A dictionary of dictionaries that maps day of week and month to corresponding offset class as returned by
+# get_third_day_of_week_in_month_offset_class. Used as an internal cache to avoid unnecessarily creating classes with
+# the same parameters.
 #
-# For example, to get the offset class for the third Friday in June, use the following: OffsetClasses[4][6]. To
-# instantiate the offset, use the following: OffsetClasses[4][6]().
+# For example, to get the offset class for the third Friday in June, use the following: OffsetClasses[4][6], where 4
+# represents Friday (zero-based offset starting with 0 = Monday) and 6 represents June (one-based offset starting with
+# 1 = January). To instantiate the offset, use the following: OffsetClasses[4][6]().
 #
-# The offset classes can be used to define typical expiry days (options, futures, et cetera) on exchanges which
-# happen on the third Friday or Thursday in a month on most exchanges. The quarterly expiry days in months March, June,
-# September, and December are also called quadruple witching.
+# The offset classes can be used to define typical expiry days (options, futures, et cetera) on exchanges which often
+# happen on the third Friday or Thursday in a month. The quarterly expiry days in months March, June, September, and
+# December are also called quadruple witching.
 #
-# Currently, includes only Thursdays and Fridays to avoid unnecessarily creating classes that will never be used. Add
-# more days here, if required.
+# Currently, includes cases for Monday to Friday which should cover all real-world scenarios.
 ThirdDayOfWeekInMonthOffsetClasses = {day_of_week: {month: get_third_day_of_week_in_month_offset_class(day_of_week, month) for month in range(1, 13)} for day_of_week in range(5)}
 
 
-def get_last_day_of_month_offset_class(month: int) -> AbstractHolidayOffset:
+def get_last_day_of_month_offset_class(month: int) -> Type[AbstractHolidayOffset]:
+    """
+    Return a new class that represents an offset that, when applied to the first day of a year, results in the last
+    day of the given month.
+
+    Parameters
+    ----------
+    month : int
+        The month, where 1 is January and 12 is December.
+
+    Returns
+    -------
+    Type[AbstractHolidayOffset]
+        A new class that represents the offset.
+    """
     @property
-    def holiday(self):
+    def holiday(self) -> Callable[[int], pd.Timestamp]:
         """
-            Return a function that returns the last day of the month for a given year.
+        Return a function that returns the last day of the month for a given year.
         """
         return lambda year: last_day_in_month(month, year)
 
     # Get name of month.
     month_name = get_month_name(month)
 
     # Create the new class.
@@ -126,9 +151,10 @@
         "holiday": holiday,
     })
 
     # Return the new class.
     return offset
 
 
-# A dictionary that maps month to corresponding offset class.
+# A dictionary that maps month to corresponding offset class as returned by get_last_day_of_month_offset_class. Used
+# as an internal cache to avoid unnecessarily creating classes with the same parameters.
 LastDayOfMonthOffsetClasses = {month: get_last_day_of_month_offset_class(month) for month in range(1, 13)}
```

### Comparing `exchange_calendars_extensions-0.1.1/pyproject.toml` & `exchange_calendars_extensions-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "exchange-calendars-extensions"
-version = "0.1.1"
-description = "Extensions of the exchange_calendars package"
+version = "0.2.1"
+description = "Extensions of the exchange-calendars package"
 license = "Apache-2.0"
 authors = ["Jens Keiner <jens.keiner@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jenskeiner/exchange_calendars_extensions/"
 repository = "https://github.com/jenskeiner/exchange_calendars_extensions/"
 documentation = "https://github.com/jenskeiner/exchange_calendars_extensions/tree/main/docs/"
 keywords = ["exchange", "calendar", "trading", "holidays"]
@@ -27,14 +27,16 @@
     "Operating System :: OS Independent",
 ]
 packages = [{include = "exchange_calendars_extensions"}]
 
 [tool.poetry.dependencies]
 python = "~=3.8"
 exchange-calendars = ">=4.0.1"
+schema = "~=0.7.5"
+typing-extensions = "~=4.6.2"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "~=7.2.1"
-pytest-cov = "~=4.0.0"
+pytest = "~=7.3.1"
+pytest-cov = "~=4.1.0"
 
 [tool.pytest.ini_options]
 addopts = "--cov=exchange_calendars_extensions --cov-report=term-missing"
```

