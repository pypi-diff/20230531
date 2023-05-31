# Comparing `tmp/econoplots-0.1.1.tar.gz` & `tmp/econoplots-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econoplots-0.1.1.tar", last modified: Fri May 19 14:51:10 2023, max compression
+gzip compressed data, was "econoplots-0.1.2.tar", last modified: Wed May 31 13:28:56 2023, max compression
```

## Comparing `econoplots-0.1.1.tar` & `econoplots-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-05-19 14:51:10.948466 econoplots-0.1.1/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1053 2023-05-19 14:19:37.000000 econoplots-0.1.1/LICENSE
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-05-19 14:51:10.948466 econoplots-0.1.1/PKG-INFO
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      799 2023-05-19 14:40:50.000000 econoplots-0.1.1/README.md
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-05-19 14:51:10.948466 econoplots-0.1.1/econoplots/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       22 2023-05-19 14:50:33.000000 econoplots-0.1.1/econoplots/__init__.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     4945 2023-05-10 21:36:54.000000 econoplots-0.1.1/econoplots/_standalone_plotters.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2356 2023-05-10 18:46:47.000000 econoplots-0.1.1/econoplots/colors.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1191 2023-05-18 20:41:58.000000 econoplots-0.1.1/econoplots/converter.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      907 2023-05-18 21:06:22.000000 econoplots-0.1.1/econoplots/params.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     8284 2023-05-18 20:42:24.000000 econoplots-0.1.1/econoplots/utils.py
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-05-19 14:51:10.948466 econoplots-0.1.1/econoplots.egg-info/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-05-19 14:51:10.000000 econoplots-0.1.1/econoplots.egg-info/PKG-INFO
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      431 2023-05-19 14:51:10.000000 econoplots-0.1.1/econoplots.egg-info/SOURCES.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-05-19 14:51:10.000000 econoplots-0.1.1/econoplots.egg-info/dependency_links.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-05-10 17:37:10.000000 econoplots-0.1.1/econoplots.egg-info/not-zip-safe
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       40 2023-05-19 14:51:10.000000 econoplots-0.1.1/econoplots.egg-info/requires.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       11 2023-05-19 14:51:10.000000 econoplots-0.1.1/econoplots.egg-info/top_level.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1336 2023-05-19 14:48:39.000000 econoplots-0.1.1/pyproject.toml
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       38 2023-05-19 14:51:10.948466 econoplots-0.1.1/setup.cfg
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       60 2023-05-10 17:07:57.000000 econoplots-0.1.1/setup.py
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-05-19 14:51:10.948466 econoplots-0.1.1/tests/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      496 2023-05-18 20:40:21.000000 econoplots-0.1.1/tests/test_converter.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      734 2023-05-18 20:49:32.000000 econoplots-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-05-31 13:28:56.748229 econoplots-0.1.2/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1053 2023-05-19 14:19:37.000000 econoplots-0.1.2/LICENSE
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-05-31 13:28:56.748229 econoplots-0.1.2/PKG-INFO
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      799 2023-05-19 14:40:50.000000 econoplots-0.1.2/README.md
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-05-31 13:28:56.748229 econoplots-0.1.2/econoplots/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       22 2023-05-31 13:27:50.000000 econoplots-0.1.2/econoplots/__init__.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     4945 2023-05-10 21:36:54.000000 econoplots-0.1.2/econoplots/_standalone_plotters.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2029 2023-05-10 18:47:46.000000 econoplots-0.1.2/econoplots/color_map.json
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2392 2023-05-19 15:01:31.000000 econoplots-0.1.2/econoplots/colors.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1375 2023-05-23 14:35:40.000000 econoplots-0.1.2/econoplots/converter.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      878 2023-05-22 17:38:56.000000 econoplots-0.1.2/econoplots/params.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    11934 2023-05-31 13:26:26.000000 econoplots-0.1.2/econoplots/utils.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-05-31 13:28:56.748229 econoplots-0.1.2/econoplots.egg-info/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-05-31 13:28:56.000000 econoplots-0.1.2/econoplots.egg-info/PKG-INFO
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      457 2023-05-31 13:28:56.000000 econoplots-0.1.2/econoplots.egg-info/SOURCES.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-05-31 13:28:56.000000 econoplots-0.1.2/econoplots.egg-info/dependency_links.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-05-10 17:37:10.000000 econoplots-0.1.2/econoplots.egg-info/not-zip-safe
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       40 2023-05-31 13:28:56.000000 econoplots-0.1.2/econoplots.egg-info/requires.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       11 2023-05-31 13:28:56.000000 econoplots-0.1.2/econoplots.egg-info/top_level.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1336 2023-05-22 17:38:24.000000 econoplots-0.1.2/pyproject.toml
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       38 2023-05-31 13:28:56.748229 econoplots-0.1.2/setup.cfg
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       60 2023-05-10 17:07:57.000000 econoplots-0.1.2/setup.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-05-31 13:28:56.748229 econoplots-0.1.2/tests/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      681 2023-05-23 15:37:46.000000 econoplots-0.1.2/tests/test_converter.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      734 2023-05-18 20:49:32.000000 econoplots-0.1.2/tests/test_utils.py
```

### Comparing `econoplots-0.1.1/LICENSE` & `econoplots-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `econoplots-0.1.1/PKG-INFO` & `econoplots-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econoplots
-Version: 0.1.1
+Version: 0.1.2
 Summary: Formats Matplotlib plots into the style of The Economist
 Author-email: Dylan Penn <dylan.penn@vt.edu>
 License: Copyright (c) 2022 Dylan Penn
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

### Comparing `econoplots-0.1.1/README.md` & `econoplots-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `econoplots-0.1.1/econoplots/_standalone_plotters.py` & `econoplots-0.1.2/econoplots/_standalone_plotters.py`

 * *Files identical despite different names*

### Comparing `econoplots-0.1.1/econoplots/colors.py` & `econoplots-0.1.2/econoplots/colors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Colors."""
+"""Run this script to generate color_map.json."""
 # %% Imports
 # Standard Library Imports
 import json
 
 # %% Colors and parameters
 colors_web_dict = {
     "econ_red": "#E3120B",
```

### Comparing `econoplots-0.1.1/econoplots/converter.py` & `econoplots-0.1.2/econoplots/converter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 """Module for converting input figure into Econoplots style."""
 # %% Imports
+
 # Standard Library Imports
-import json
+from copy import deepcopy
 
 # Third Party Imports
 from matplotlib import pyplot as plt  # noqa
 from matplotlib.axes import Axes
 
-# econoplots Imports
+# Econoplots Imports
 from econoplots.params import setRCParams
 from econoplots.utils import (
+    loadColorMap,
     makePatchSpinesInvisible,
     replaceAxesMinusGlyphs,
     setDefaultLineColors,
     setDefaultXAxisParams,
     setDefaultYAxisParams,
 )
 
 # %% Load color map and set parameters
 setRCParams()
 
-with open("econoplots/color_map.json") as json_file:
-    color_map = json.load(json_file)
+# with open("econoplots/color_map.json") as json_file:
+#     color_map = json.load(json_file)
 
 # %% Functions
 
 
 def convert2Econo(ax: Axes) -> Axes:
     assert isinstance(ax, Axes)
+    color_map = loadColorMap()
 
     # Change axis color
     ax.grid(
         which="major",
         axis="y",
         color=color_map["grid"]["grid_gray"],
         zorder=1,
     )
 
     # Change line colors
     setDefaultLineColors(ax)
 
     # set axis params
+    y_offset_text = ax.yaxis.get_offset_text().get_text()
+    x_offset_text = ax.xaxis.get_offset_text().get_text()
     replaceAxesMinusGlyphs(ax)
     setDefaultYAxisParams(ax, side="right", label_location="right")
     setDefaultXAxisParams(ax, pad_side="right", minor_ticks_on=True)
 
     # delete top, right, left spines
     makePatchSpinesInvisible(ax, ["top", "right", "left"])
```

### Comparing `econoplots-0.1.1/econoplots/params.py` & `econoplots-0.1.2/econoplots/params.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """Set global parameters of matplotlib."""
 # %% Imports
 from __future__ import annotations
 
-# Standard Library Imports
-import json
-
 # Third Party Imports
 import matplotlib as mpl
 from cycler import cycler
 
-# %% Load color map
-with open("econoplots/color_map.json") as json_file:
-    color_map = json.load(json_file)
+# Econoplots Imports
+from econoplots.utils import loadColorMap
 
 
 # %% Set Params
 def setRCParams():
+    color_map = loadColorMap()
+
     mpl.rcParams["font.sans-serif"] = [
         "CMU Bright",
     ]
     mpl.rcParams["font.family"] = "sans-serif"
     mpl.rcParams.update(
         {
             "font.size": 14,
-            "font.weight": "bold",
+            # "font.weight": "bold",
         }
     )
     mpl.rcParams["lines.linestyle"] = "-"
     mpl.rcParams["lines.linewidth"] = 3
     mpl.rcParams["axes.prop_cycle"] = cycler(color=color_map["line_chart"])
     mpl.rcParams["figure.facecolor"] = "w"
     mpl.rcParams["axes.facecolor"] = "w"
-    mpl.rcParams["xtick.major.size"] = 6
+    mpl.rcParams["xtick.major.size"] = 6  # length of tick marks
     mpl.rcParams["xtick.minor.size"] = 3
```

### Comparing `econoplots-0.1.1/econoplots/utils.py` & `econoplots-0.1.2/econoplots/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """Utilities."""
 # Imports
 from __future__ import annotations
 
 # Standard Library Imports
+import importlib.resources
 import json
 from itertools import cycle
 from typing import Tuple
 
 # Third Party Imports
 from matplotlib import pyplot as plt  # noqa
 from matplotlib.axes import Axes
 from matplotlib.axis import Axis
 from matplotlib.text import Text
 from matplotlib.ticker import AutoMinorLocator, FixedLocator
-from numpy import absolute
+from numpy import absolute, append, intersect1d
 
-# %% Load color map
-with open("econoplots/color_map.json") as json_file:
-    color_map = json.load(json_file)
+# %% Functions
+
+
+def loadColorMap() -> dict:
+    with importlib.resources.open_text("econoplots", "color_map.json") as file:
+        color_map = json.load(file)
+    return color_map
 
 
-# %% Functions
 def makePatchSpinesInvisible(
     ax: Axis,
     list_of_spines: list[str] = None,
 ) -> None:
     """Makes spine(s) of axis invisible.
 
     Args:
@@ -52,15 +56,17 @@
         x_labels.append(replaceMinusWithHyphen(tl))
     ax.xaxis.set_ticklabels(x_labels)
 
     y_labels = []
     tick_labels = ax.yaxis.get_ticklabels()
     for tl in tick_labels:
         y_labels.append(replaceMinusWithHyphen(tl))
-    ax.yaxis.set_ticklabels(y_labels)
+    # ax.yaxis.set_ticklabels(y_labels)
+    ytick_locs = ax.yaxis.get_ticklocs()
+    ax.set_yticks(ytick_locs[1:-2], y_labels[1:-2])
 
     return
 
 
 def setDefaultYAxisParams(
     ax: Axes,
     side: str,
@@ -68,14 +74,16 @@
 ) -> None:
     """Set y-axis side, label, tick label location and style.
 
     Args:
         ax (Axes): _description_
         side (str): "left" or "right
     """
+    color_map = loadColorMap()
+
     # Set axis parameters based on which side axis is on
     if side == "right":
         ha = "right"
         label_side = {
             "labelright": True,
             "labelleft": False,
         }
@@ -92,14 +100,16 @@
     ax.yaxis.set_tick_params(
         pad=left_right_pad,  # Pad tick labels so they don't go over y-axis
         colors=color_map["grid"]["grid_gray"],  # set tick color to same as grid
         labelcolor="black",  # set tick label color
         **label_side,
     )
 
+    # ax.ticklabel_format(ScalarFormatter)
+
     # Set tick label parameters
     # NOTE: Move labels after moving axis.
     # set vertical alignment on y-axis tick labels to be on top of of major
     # ticks. Set horizontal alignment to right (this part not necessary)
     for label in ax.yaxis.get_ticklabels():
         label.set_verticalalignment("bottom")
         label.set_horizontalalignment(ha)
@@ -123,41 +133,107 @@
         pad_side (str): Which side(s) to add padding to. Axis is always shown on
             bottom of plot.
         minor_ticks_on (bool, optional): Whether or not to plot minor tick marks.
             Defaults to True.
         n_minortick_subdivisions (int, optional): Number of minor ticks between
             major ticks. Defaults to None, which automatically determines number.
     """
+    # Add empty space to x-axis to give space between y-tick labels and plotted
+    # data. Do this BEFORE other operations, as resizing can mess up tick marks.
+    padXAxis(ax, side=pad_side)
+
+    # Set Major ticks. Make major ticks that are wider than span of the data invisible.
+    makeOutOfRangeXTicksInvisible(ax)
 
     if minor_ticks_on is True:
         # Turn on minor ticks and set frequency between major ticks
-        ax.xaxis.set_minor_locator(AutoMinorLocator(n_minortick_subdivisions))
+        addInnerMinorTicks(ax, n_minortick_subdivisions)
 
-        # Remove minor ticks that are beyond outermost VISIBLE major ticks (the
-        # outermost major ticks are not visible).
-        min_major_tick_loc = ax.xaxis.get_majorticklocs()[0]
-        max_major_tick_loc = ax.xaxis.get_majorticklocs()[-1]
-        minor_tick_locs = ax.xaxis.get_minorticklocs()
-        minor_tick_locs = minor_tick_locs[minor_tick_locs > min_major_tick_loc]
-        minor_tick_locs = minor_tick_locs[minor_tick_locs < max_major_tick_loc]
-        ax.xaxis.set_minor_locator(FixedLocator(minor_tick_locs))
+    # Add minor tick(s) if outer limits of data are NOT on major ticks. Unlike
+    # minor ticks that are in-between major ticks, the outer minor ticks are not
+    # optional.
+    addOuterMinorTicks(ax)
+
+    return
 
-    # Set Major ticks (do this AFTER setting minor ticks). Make major ticks that
-    # are wider than span of the data invisible.
+
+def addInnerMinorTicks(ax: Axes, n_minortick_subdivisions: int | None):
+    """Add minor ticks to x axis within data limits."""
+    ax.xaxis.set_minor_locator(AutoMinorLocator(n_minortick_subdivisions))
+
+    # Remove minor ticks that are beyond data range.
+    x_lims, _ = getDataLimits(ax)
+    # min_major_tick_loc = ax.xaxis.get_majorticklocs()[1]
+    # max_major_tick_loc = ax.xaxis.get_majorticklocs()[-2]
+    minor_tick_locs = ax.xaxis.get_minorticklocs()
+    minor_tick_locs = minor_tick_locs[minor_tick_locs > x_lims[0]]
+    minor_tick_locs = minor_tick_locs[minor_tick_locs < x_lims[1]]
+    ax.xaxis.set_minor_locator(FixedLocator(minor_tick_locs))
+    return
+
+
+def makeOutOfRangeXTicksInvisible(ax: Axes):
+    """Make major ticks that are < or > data range invisible."""
     major_tick_locs = ax.xaxis.get_majorticklocs()
     xticks = ax.xaxis.get_major_ticks()
     xlims, _ = getDataLimits(ax)
-    if major_tick_locs[0] < xlims[0]:
-        xticks[0].set_visible(False)
-    if major_tick_locs[-1] > xlims[1]:
-        xticks[-1].set_visible(False)
+    visibility = list(major_tick_locs > xlims[0])
 
-    # Add empty space to x-axis to give space between y-tick labels and plotted
-    # data.
-    padXAxis(ax, side=pad_side)
+    for tick, vis in zip(xticks, visibility):
+        tick.set_visible(vis)
+    visibility = list(major_tick_locs < xlims[1])
+    for tick, vis in zip(xticks, visibility):
+        tick.set_visible(vis)
+
+    return
+
+
+def addOuterMinorTicks(ax: Axes):
+    """Add minor ticks to data limits if major ticks don't already cover limits."""
+    major_locs = [b.get_loc() for b in ax.xaxis.get_major_ticks()]
+    minor_tick_locs = ax.xaxis.get_minorticklocs()
+
+    # Get locations to add new minor ticks. Add new ticks if existing major ticks
+    # don't overlap with outer limits of data.
+    x_lim, _ = getDataLimits(ax)
+    new_locs = []
+    for x in x_lim:
+        if x not in major_locs:
+            new_locs.append(x)
+    num_new_locs = len(new_locs)
+
+    # Append new minor ticks to existing minor ticks.
+    minor_tick_locs = append(minor_tick_locs, new_locs)
+    ax.xaxis.set_minor_locator(FixedLocator(minor_tick_locs))
+
+    # Refresh minor tick locs because special case where adding minor tick close
+    # to major tick causes minor tick to not be added. This step is needed to prevent
+    # an error.
+    num_minor_ticks_attempted = len(minor_tick_locs)
+    minor_tick_locs = ax.xaxis.get_minorticklocs()
+    ax.xaxis.set_minor_locator(FixedLocator(minor_tick_locs))
+
+    if num_minor_ticks_attempted != len(minor_tick_locs):
+        # Par down the list of new minor tick locations if matplotlib rejected
+        # additions.
+        print("Different number of minor ticks added than attempted.")
+        new_locs = intersect1d(minor_tick_locs, new_locs)
+        num_new_locs = len(new_locs)
+
+    # Create labels for new minor ticks and set minor tick labels
+    minor_labels = [item.get_text() for item in ax.get_xticklabels(minor=True)]
+    num_minor_labels = len(minor_labels)
+    for i, lab in enumerate(new_locs, num_minor_labels - num_new_locs):
+        # new labels are at end of minor_labels list
+        text = "%.0f" % lab
+        minor_labels[i] = text
+
+    # TODO: Make the format of the added minor ticks match the format of the major
+    # ticks.
+    ax.set_xticks(minor_tick_locs, minor_labels, minor=True)
 
     return
 
 
 def padXAxis(
     ax: Axes,
     side: str,
@@ -182,34 +258,40 @@
     x_ax_minor_pad = 0.33 * x_ax_pad
 
     if side == "left":
         # set x-axis max limit to tighter than default and with extra room on left
         ax.set_xlim(
             [
                 x_lims[0] - x_ax_pad,
-                x_lims[1] + x_ax_minor_pad * x_ax_pad,
+                x_lims[1] + x_ax_minor_pad,
             ]
         )
 
     if side == "right":
         ax.set_xlim(
             [
-                x_lims[0] - x_ax_minor_pad * x_ax_pad,
+                x_lims[0] - x_ax_minor_pad,
                 x_lims[1] + x_ax_pad,
             ]
         )
 
     if side == "both":
         ax.set_xlim(
             [
                 x_lims[0] - x_ax_pad,
                 x_lims[1] + x_ax_pad,
             ]
         )
 
+    # NOTE: This adjustment seems to have not been necessary, but keeping here
+    # in case issue crops up again.
+    # Changing plot size changes tick labels in incorrect ways, so re-initialize
+    # tick labels
+    # ax.set_xticks(ax.xaxis.get_majorticklocs()[1:-2])
+
     return ax
 
 
 def getDataLimits(ax: Axes) -> Tuple[list, list]:
     """Get x and y limits of data in ax (different from axis limits).
 
     Args:
@@ -247,15 +329,15 @@
 
     Args:
         ax (Axes): _description_
 
     Returns:
         Axes: _description_
     """
-
+    color_map = loadColorMap()
     color_cycler = cycle(color_map["line_chart"])
     for line in ax.lines:
         line.set_color(next(color_cycler))
 
     return ax
 
 
@@ -269,21 +351,35 @@
     Returns:
         Axes: _description_
     """
     ax.yaxis.label.set(rotation="horizontal")
 
     # Set label vertical alignment
     ax.yaxis.label.set_va("bottom")
+
+    # TODO: Get max value of yticklabel, then place yaxis label above that. Will
+    # be smarter than simply placing the yaxis label at an arbitrary location.
+    ytick_labels = ax.yaxis.get_majorticklabels()
+    ytick_label_locs = [label.get_position()[1] for label in ytick_labels]
+    # get max visible ytick label location
+    top_label_loc = ytick_label_locs[-2]
+
+    # Add a bit of white space between the bottom of the label and the top of the
+    # axis.
+    # y_label_pad = 0
+    y_label_pad = 0.01
+    # y_label_pad = 0.05
+
     if side == "left":
         # move label to upper-left and set horizontal alignment
-        ax.yaxis.set_label_coords(0, 1)
+        ax.yaxis.set_label_coords(0, 1 + y_label_pad)
         ax.yaxis.label.set_ha("left")
     elif side == "right":
         # move label to upper-right and set horizontal alignment
-        ax.yaxis.set_label_coords(1, 1)
+        ax.yaxis.set_label_coords(1, 1 + y_label_pad)
         ax.yaxis.label.set_ha("right")
 
     return ax
 
 
 def replaceMinusWithHyphen(text: Text) -> Text:
     """Replace all minus signs chr(8722) with hyphens chr(45)."""
```

### Comparing `econoplots-0.1.1/econoplots.egg-info/PKG-INFO` & `econoplots-0.1.2/econoplots.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econoplots
-Version: 0.1.1
+Version: 0.1.2
 Summary: Formats Matplotlib plots into the style of The Economist
 Author-email: Dylan Penn <dylan.penn@vt.edu>
 License: Copyright (c) 2022 Dylan Penn
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

### Comparing `econoplots-0.1.1/pyproject.toml` & `econoplots-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `econoplots-0.1.1/tests/test_utils.py` & `econoplots-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

