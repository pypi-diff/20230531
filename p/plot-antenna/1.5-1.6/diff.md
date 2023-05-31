# Comparing `tmp/plot-antenna-1.5.tar.gz` & `tmp/plot-antenna-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plot-antenna-1.5.tar", last modified: Tue May 30 20:03:16 2023, max compression
+gzip compressed data, was "plot-antenna-1.6.tar", last modified: Wed May 31 14:48:06 2023, max compression
```

## Comparing `plot-antenna-1.5.tar` & `plot-antenna-1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 20:03:16.499867 plot-antenna-1.5/
--rw-r--r--   0 ralf      (1000) priv      (1011)    10664 2023-05-30 20:03:16.499867 plot-antenna-1.5/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)     8544 2023-05-30 20:00:47.000000 plot-antenna-1.5/README.rst
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 20:03:16.467867 plot-antenna-1.5/plot_antenna/
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-05-30 20:02:20.000000 plot-antenna-1.5/plot_antenna/Version.py
--rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-09-11 10:43:22.000000 plot-antenna-1.5/plot_antenna/__init__.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    50599 2023-05-30 19:59:11.000000 plot-antenna-1.5/plot_antenna/plot_antenna.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 20:03:16.491867 plot-antenna-1.5/plot_antenna.egg-info/
--rw-r--r--   0 ralf      (1000) priv      (1011)    10664 2023-05-30 20:03:16.000000 plot-antenna-1.5/plot_antenna.egg-info/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)      333 2023-05-30 20:03:16.000000 plot-antenna-1.5/plot_antenna.egg-info/SOURCES.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-30 20:03:16.000000 plot-antenna-1.5/plot_antenna.egg-info/dependency_links.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       65 2023-05-30 20:03:16.000000 plot-antenna-1.5/plot_antenna.egg-info/entry_points.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       17 2023-05-30 20:03:16.000000 plot-antenna-1.5/plot_antenna.egg-info/requires.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       13 2023-05-30 20:03:16.000000 plot-antenna-1.5/plot_antenna.egg-info/top_level.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-30 20:03:16.499867 plot-antenna-1.5/setup.cfg
--rw-r--r--   0 ralf      (1000) priv      (1011)     2716 2022-09-13 14:27:54.000000 plot-antenna-1.5/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 20:03:16.495867 plot-antenna-1.5/test/
--rw-r--r--   0 ralf      (1000) priv      (1011)     7225 2022-09-13 13:39:50.000000 plot-antenna-1.5/test/test_plot.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-31 14:48:06.841402 plot-antenna-1.6/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    11232 2023-05-31 14:48:06.841402 plot-antenna-1.6/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)     9024 2023-05-31 14:46:42.000000 plot-antenna-1.6/README.rst
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-31 14:48:06.809402 plot-antenna-1.6/plot_antenna/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-05-31 14:47:28.000000 plot-antenna-1.6/plot_antenna/Version.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-09-11 10:43:22.000000 plot-antenna-1.6/plot_antenna/__init__.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    51994 2023-05-31 07:31:41.000000 plot-antenna-1.6/plot_antenna/plot_antenna.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-31 14:48:06.833402 plot-antenna-1.6/plot_antenna.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    11232 2023-05-31 14:48:06.000000 plot-antenna-1.6/plot_antenna.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)      333 2023-05-31 14:48:06.000000 plot-antenna-1.6/plot_antenna.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-31 14:48:06.000000 plot-antenna-1.6/plot_antenna.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       65 2023-05-31 14:48:06.000000 plot-antenna-1.6/plot_antenna.egg-info/entry_points.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       17 2023-05-31 14:48:06.000000 plot-antenna-1.6/plot_antenna.egg-info/requires.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       13 2023-05-31 14:48:06.000000 plot-antenna-1.6/plot_antenna.egg-info/top_level.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-31 14:48:06.841402 plot-antenna-1.6/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2716 2022-09-13 14:27:54.000000 plot-antenna-1.6/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-31 14:48:06.837402 plot-antenna-1.6/test/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     7225 2022-09-13 13:39:50.000000 plot-antenna-1.6/test/test_plot.py
```

### Comparing `plot-antenna-1.5/PKG-INFO` & `plot-antenna-1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-antenna
-Version: 1.5
+Version: 1.6
 Summary: Antenna plotting program for plotting antenna simulation results
 Home-page: https://github.com/schlatterbeck/plot-antenna
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: MIT License
 Description: Antenna Plotting Program
         ========================
@@ -153,14 +153,22 @@
         .. _matplotlib: https://matplotlib.org/
         .. _plotly: https://github.com/plotly/plotly.py
         .. _pandas: https://pandas.pydata.org/
         
         Release Notes
         -------------
         
+        v1.6: More SWR plot changes
+        
+        - Make SWR-plot vertical line colors configurable
+        - Rename elevation-angle and azimuth-angle options to angle-elevation
+          and angle-azimuth so that we can again request an elevation/azimuth
+          plot with shortened options like --ele or --azi
+        - Sort options lexicographically on --help
+        
         v1.5: Allow target SWR frequency in VSWR plot
         
         - Add command-line option --target-swr-frequency
         - Draw user-specifed target frequency in red, best (minimum) swr in grey
         
         v1.4: Reset button and VSWR-Plot improvements
         
@@ -181,19 +189,22 @@
           graphics may collide with the graphics itself. We can now specify the
           font size with ``--title-font-size``. This option currently works only
           with plotly graphics.
         
         v1.1: Specification of azimuth / elevation angle
         
         - Now we can specify an azimuth angle for elevation plot and an
-          elevation angle for azimuth plots
+          elevation angle for azimuth plots.
         - Bug-fix in computation of maximum gain azimuth direction: If the
           maximum gain in theta direction goes up or down, the azimuth angle
           would be computed incorrectly because all gain values at that theta
           angle are the same for all azimuth angles.
+        - Sort options: Since there are some options that only exist when some
+          packages are installed we sort options instead of trying to add them
+          in the correct order.
         
         v1.0: Initial Release
         
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `plot-antenna-1.5/README.rst` & `plot-antenna-1.6/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -145,14 +145,22 @@
 .. _matplotlib: https://matplotlib.org/
 .. _plotly: https://github.com/plotly/plotly.py
 .. _pandas: https://pandas.pydata.org/
 
 Release Notes
 -------------
 
+v1.6: More SWR plot changes
+
+- Make SWR-plot vertical line colors configurable
+- Rename elevation-angle and azimuth-angle options to angle-elevation
+  and angle-azimuth so that we can again request an elevation/azimuth
+  plot with shortened options like --ele or --azi
+- Sort options lexicographically on --help
+
 v1.5: Allow target SWR frequency in VSWR plot
 
 - Add command-line option --target-swr-frequency
 - Draw user-specifed target frequency in red, best (minimum) swr in grey
 
 v1.4: Reset button and VSWR-Plot improvements
 
@@ -173,14 +181,17 @@
   graphics may collide with the graphics itself. We can now specify the
   font size with ``--title-font-size``. This option currently works only
   with plotly graphics.
 
 v1.1: Specification of azimuth / elevation angle
 
 - Now we can specify an azimuth angle for elevation plot and an
-  elevation angle for azimuth plots
+  elevation angle for azimuth plots.
 - Bug-fix in computation of maximum gain azimuth direction: If the
   maximum gain in theta direction goes up or down, the azimuth angle
   would be computed incorrectly because all gain values at that theta
   angle are the same for all azimuth angles.
+- Sort options: Since there are some options that only exist when some
+  packages are installed we sort options instead of trying to add them
+  in the correct order.
 
 v1.0: Initial Release
```

### Comparing `plot-antenna-1.5/plot_antenna/plot_antenna.py` & `plot-antenna-1.6/plot_antenna/plot_antenna.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import os
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
 import numpy as np
 from bisect import bisect
 from mpl_toolkits.mplot3d import Axes3D
-from argparse import ArgumentParser
+from argparse import ArgumentParser, HelpFormatter
 from matplotlib import cm, __version__ as matplotlib_version, rcParams
 from matplotlib.widgets import Slider
 try:
     import plotly.express as px
     import plotly.graph_objects as go
     from plotly.subplots import make_subplots
     import pandas         as pd
@@ -326,24 +326,24 @@
             self.frequencies.append (f)
         # Compute the theta index that occurs most often over all
         # frequencies
         self.theta_maxidx = list \
             (sorted (theta_idx, key = lambda a: theta_idx [a])) [-1]
         self.phi_maxidx = list \
             (sorted (phi_idx, key = lambda a: phi_idx [a])) [-1]
-        if self.args.azimuth_angle is not None:
+        if self.args.angle_azimuth is not None:
             phis = next (iter (self.gdata.values ())).phis_d
             self.phi_angle_idx = nearest_angle_idx \
-                (phis, self.args.azimuth_angle)
+                (phis, self.args.angle_azimuth)
         else:
             self.phi_angle_idx = self.phi_maxidx
-        if self.args.elevation_angle is not None:
+        if self.args.angle_elevation is not None:
             thetas = next (iter (self.gdata.values ())).thetas_d
             self.theta_angle_idx = nearest_angle_idx \
-                (thetas, 90 - self.args.elevation_angle)
+                (thetas, 90 - self.args.angle_elevation)
         else:
             self.theta_angle_idx = self.theta_maxidx
         if self.outfile or len (self.gdata) == 1 or not self.with_slider:
             self.with_slider = False
         # Borrow colormap from matplotlib to use in plotly
         self.colormap = []
         for cn in mcolors.TABLEAU_COLORS:
@@ -1037,29 +1037,35 @@
         ax.set_xlabel ('Frequency')
         ax.set_ylabel ('VSWR')
         X, Y = self.prepare_vswr ()
         ax.plot (X, Y)
         ax.grid (color = '0.95')
         tg = self.args.target_swr_frequency
         if tg is not None:
-            ax.axvline (x = tg, color = 'r', linestyle = 'dashed')
-        ax.axvline (x = self.min_x, color = 'grey', linestyle = 'dashed')
+            c = self.args.swr_target_color
+            ax.axvline (x = tg, color = c, linestyle = 'dashed')
+        c = self.args.swr_min_color
+        if c and c.lower () != 'none':
+            ax.axvline (x = self.min_x, color = c, linestyle = 'dashed')
     # end def plot_vswr_matplotlib
 
     def plot_vswr_plotly (self, name):
         X, Y = self.prepare_vswr ()
         df = pd.DataFrame ()
         df ['Frequency'] = X
         df ['VSWR'] = Y
         fig = px.line (df, x="Frequency", y="VSWR")
         fig.update (self.plotly_line_default)
         tg = self.args.target_swr_frequency
         if tg is not None:
-            fig.add_vline (x = tg, line_dash = "dash", line_color = "red")
-        fig.add_vline (x = self.min_x, line_dash = "dash", line_color = "grey")
+            c = self.args.swr_target_color
+            fig.add_vline (x = tg, line_dash = "dash", line_color = c)
+        c = self.args.swr_min_color
+        if c and c.lower () != 'none':
+            fig.add_vline (x = self.min_x, line_dash = "dash", line_color = c)
         self.show_plotly (fig, name)
     # end def plot_vswr_plotly
 
     def scene_ranges (self, matrix = None):
         """ Create cubic bounding box to force equal aspect ratio
             If matrix is not given, we concatenate *all* gains.
         """
@@ -1208,28 +1214,53 @@
     def update_from_slider (self, val):
         self.frequency = self.freq_slider.val
         self.update_display ()
     # end def update_from_slider
 
 # end class Gain_Plot
 
+class SortingHelpFormatter (HelpFormatter):
+
+    def add_arguments (self, actions):
+        actions = sorted (actions, key = self.argsort)
+        super ().add_arguments (actions)
+    # end def add_arguments
+
+    @staticmethod
+    def argsort (action):
+        x = action.option_strings
+        if not x:
+            return ''
+        for opt in tuple (x):
+            if opt.startswith ('--'):
+                return opt
+    # end def argsort
+
+# end class SortingHelpFormatter
+
+class SortingArgumentParser (ArgumentParser):
+    def __init__ (self, *args, **kw):
+        super ().__init__ (*args, formatter_class = SortingHelpFormatter, **kw)
+    # end def __init__
+# end class SortingArgumentParser
+
 def main (argv = sys.argv [1:]):
-    cmd = ArgumentParser ()
+    cmd = SortingArgumentParser ()
     scaling = ['arrl', 'linear', 'linear_db', 'linear_voltage']
     cmd.add_argument \
         ( 'filename'
         , help    = 'File to parse and plot'
         )
     cmd.add_argument \
         ( '--azimuth'
         , help    = 'Do an azimuth plot'
         , action  = 'store_true'
         )
     cmd.add_argument \
-        ( '--azimuth-angle'
+        ( '--angle-azimuth'
         , help    = 'Azimuth angle to use for elevation plot, default is '
                     'maximum gain angle'
         , type    = float
         )
     cmd.add_argument \
         ( '--dpi'
         , help    = 'Resolution for matplotlib, default = %(default)s'
@@ -1238,15 +1269,15 @@
         )
     cmd.add_argument \
         ( '--elevation'
         , help    = 'Do an elevation plot'
         , action  = 'store_true'
         )
     cmd.add_argument \
-        ( '--elevation-angle'
+        ( '--angle-elevation'
         , help    = 'Elevation angle to use for azimuth plot, default is '
                     'maximum gain angle'
         , type    = float
         )
     # For versions below 3.5 slider will be always off
     if matplotlib_version_float >= 3.5:
         cmd.add_argument \
@@ -1291,19 +1322,30 @@
     cmd.add_argument \
         ( '--plot-vswr', '--swr', '--vswr', '--plot-swr'
         , help    = 'Plot voltage standing wave ratio (VSWR)'
         , action  = 'store_true'
         )
     cmd.add_argument \
         ( "--target-swr-frequency", "--target-vswr-frequency"
-        , help    = "In SWR plot, draw a red vertical line at this "
-                    "frequency"
+        , help    = "In SWR plot, draw a vertical line at this frequency"
         , type    = float
         )
     cmd.add_argument \
+        ( "--swr-min-color", "--vswr-min-color"
+        , help    = "Draw minimum SWR vertical line in this color, use "
+                    "'none' to not draw the line"
+        , default = 'green'
+        )
+    cmd.add_argument \
+        ( "--swr-target-color", "--vswr-target-color"
+        , help    = "If the --target-swr-frequency option is given, draw "
+                    "vertical line in this color"
+        , default = 'grey'
+        )
+    cmd.add_argument \
         ( '--title-font-size'
         , help    = 'Title/legend font size in pt '
                     '(currently only used in plotly)'
         , type    = int
         )
     cmd.add_argument \
         ( '--wireframe'
```

### Comparing `plot-antenna-1.5/plot_antenna.egg-info/PKG-INFO` & `plot-antenna-1.6/plot_antenna.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-antenna
-Version: 1.5
+Version: 1.6
 Summary: Antenna plotting program for plotting antenna simulation results
 Home-page: https://github.com/schlatterbeck/plot-antenna
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: MIT License
 Description: Antenna Plotting Program
         ========================
@@ -153,14 +153,22 @@
         .. _matplotlib: https://matplotlib.org/
         .. _plotly: https://github.com/plotly/plotly.py
         .. _pandas: https://pandas.pydata.org/
         
         Release Notes
         -------------
         
+        v1.6: More SWR plot changes
+        
+        - Make SWR-plot vertical line colors configurable
+        - Rename elevation-angle and azimuth-angle options to angle-elevation
+          and angle-azimuth so that we can again request an elevation/azimuth
+          plot with shortened options like --ele or --azi
+        - Sort options lexicographically on --help
+        
         v1.5: Allow target SWR frequency in VSWR plot
         
         - Add command-line option --target-swr-frequency
         - Draw user-specifed target frequency in red, best (minimum) swr in grey
         
         v1.4: Reset button and VSWR-Plot improvements
         
@@ -181,19 +189,22 @@
           graphics may collide with the graphics itself. We can now specify the
           font size with ``--title-font-size``. This option currently works only
           with plotly graphics.
         
         v1.1: Specification of azimuth / elevation angle
         
         - Now we can specify an azimuth angle for elevation plot and an
-          elevation angle for azimuth plots
+          elevation angle for azimuth plots.
         - Bug-fix in computation of maximum gain azimuth direction: If the
           maximum gain in theta direction goes up or down, the azimuth angle
           would be computed incorrectly because all gain values at that theta
           angle are the same for all azimuth angles.
+        - Sort options: Since there are some options that only exist when some
+          packages are installed we sort options instead of trying to add them
+          in the correct order.
         
         v1.0: Initial Release
         
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `plot-antenna-1.5/setup.py` & `plot-antenna-1.6/setup.py`

 * *Files identical despite different names*

### Comparing `plot-antenna-1.5/test/test_plot.py` & `plot-antenna-1.6/test/test_plot.py`

 * *Files identical despite different names*

