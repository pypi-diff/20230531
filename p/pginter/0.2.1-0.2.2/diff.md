# Comparing `tmp/pginter-0.2.1.tar.gz` & `tmp/pginter-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pginter-0.2.1.tar", last modified: Wed May 31 20:32:00 2023, max compression
+gzip compressed data, was "pginter-0.2.2.tar", last modified: Wed May 31 21:10:37 2023, max compression
```

## Comparing `pginter-0.2.1.tar` & `pginter-0.2.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.423661 pginter-0.2.1/
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.1/LICENSE
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.1/MANIFEST.in
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-05-31 20:32:00.420327 pginter-0.2.1/PKG-INFO
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.1/README.md
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.1/pyproject.toml
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-05-31 20:32:00.423661 pginter-0.2.1/setup.cfg
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      936 2023-05-31 20:31:44.000000 pginter-0.2.1/setup.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.413661 pginter-0.2.1/src/
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.416994 pginter-0.2.1/src/pginter/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.1/src/pginter/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20488 2023-05-31 20:25:21.000000 pginter-0.2.1/src/pginter/_pg_root.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.1/src/pginter/icon.png
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.416994 pginter-0.2.1/src/pginter/theme/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.1/src/pginter/theme/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.1/src/pginter/theme/_manager.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.416994 pginter-0.2.1/src/pginter/theme/themes/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      663 2023-05-25 20:39:17.000000 pginter-0.2.1/src/pginter/theme/themes/default.json
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.420327 pginter-0.2.1/src/pginter/types/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.1/src/pginter/types/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.1/src/pginter/types/_better_dict.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.1/src/pginter/types/_binds.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.1/src/pginter/types/_color.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.1/src/pginter/types/_constants.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.1/src/pginter/types/_geo_types.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.1/src/pginter/types/_notifications.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.1/src/pginter/types/_scheme.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.1/src/pginter/types/_style.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.1/src/pginter/types/_tk_vars.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.420327 pginter-0.2.1/src/pginter/utils/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       49 2023-05-14 20:09:36.000000 pginter-0.2.1/src/pginter/utils/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      872 2023-05-25 23:31:06.000000 pginter-0.2.1/src/pginter/utils/_funcs.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.420327 pginter-0.2.1/src/pginter/widgets/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.1/src/pginter/widgets/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.1/src/pginter/widgets/_button.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.1/src/pginter/widgets/_entry.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    25138 2023-05-31 20:14:13.000000 pginter-0.2.1/src/pginter/widgets/_frame.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-05-31 20:24:58.000000 pginter-0.2.1/src/pginter/widgets/_geo_manager.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.1/src/pginter/widgets/_label.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.1/src/pginter/widgets/_supports_children.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.1/src/pginter/widgets/_surface_frame.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.416994 pginter-0.2.1/src/pginter.egg-info/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-05-31 20:32:00.000000 pginter-0.2.1/src/pginter.egg-info/PKG-INFO
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      994 2023-05-31 20:32:00.000000 pginter-0.2.1/src/pginter.egg-info/SOURCES.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-05-31 20:32:00.000000 pginter-0.2.1/src/pginter.egg-info/dependency_links.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-05-31 20:32:00.000000 pginter-0.2.1/src/pginter.egg-info/top_level.txt
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:10:37.553765 pginter-0.2.2/
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.2/LICENSE
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.2/MANIFEST.in
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-05-31 21:10:37.553765 pginter-0.2.2/PKG-INFO
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.2/README.md
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.2/pyproject.toml
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-05-31 21:10:37.553765 pginter-0.2.2/setup.cfg
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      936 2023-05-31 21:10:15.000000 pginter-0.2.2/setup.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:10:37.547098 pginter-0.2.2/src/
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:10:37.547098 pginter-0.2.2/src/pginter/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.2/src/pginter/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20488 2023-05-31 20:25:21.000000 pginter-0.2.2/src/pginter/_pg_root.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.2/src/pginter/icon.png
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:10:37.550432 pginter-0.2.2/src/pginter/theme/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.2/src/pginter/theme/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.2/src/pginter/theme/_manager.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:10:37.550432 pginter-0.2.2/src/pginter/theme/themes/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      663 2023-05-25 20:39:17.000000 pginter-0.2.2/src/pginter/theme/themes/default.json
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:10:37.550432 pginter-0.2.2/src/pginter/types/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.2/src/pginter/types/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.2/src/pginter/types/_better_dict.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.2/src/pginter/types/_binds.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.2/src/pginter/types/_color.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.2/src/pginter/types/_constants.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.2/src/pginter/types/_geo_types.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.2/src/pginter/types/_notifications.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.2/src/pginter/types/_scheme.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.2/src/pginter/types/_style.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.2/src/pginter/types/_tk_vars.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:10:37.550432 pginter-0.2.2/src/pginter/utils/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       49 2023-05-14 20:09:36.000000 pginter-0.2.2/src/pginter/utils/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      872 2023-05-25 23:31:06.000000 pginter-0.2.2/src/pginter/utils/_funcs.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:10:37.553765 pginter-0.2.2/src/pginter/widgets/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.2/src/pginter/widgets/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.2/src/pginter/widgets/_button.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.2/src/pginter/widgets/_entry.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26515 2023-05-31 20:53:29.000000 pginter-0.2.2/src/pginter/widgets/_frame.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-05-31 20:24:58.000000 pginter-0.2.2/src/pginter/widgets/_geo_manager.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.2/src/pginter/widgets/_label.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.2/src/pginter/widgets/_supports_children.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.2/src/pginter/widgets/_surface_frame.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:10:37.550432 pginter-0.2.2/src/pginter.egg-info/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-05-31 21:10:37.000000 pginter-0.2.2/src/pginter.egg-info/PKG-INFO
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      994 2023-05-31 21:10:37.000000 pginter-0.2.2/src/pginter.egg-info/SOURCES.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-05-31 21:10:37.000000 pginter-0.2.2/src/pginter.egg-info/dependency_links.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-05-31 21:10:37.000000 pginter-0.2.2/src/pginter.egg-info/top_level.txt
```

### Comparing `pginter-0.2.1/LICENSE` & `pginter-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/setup.py` & `pginter-0.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pginter",
-    version="0.2.1",
+    version="0.2.2",
     author="Nilusink",
     author_email="nilusink@protonmail.com",
     description="A python GUI interface, based on pygame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nilusink/PgInter",
     # project_urls={
```

### Comparing `pginter-0.2.1/src/pginter/_pg_root.py` & `pginter-0.2.2/src/pginter/_pg_root.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/icon.png` & `pginter-0.2.2/src/pginter/icon.png`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/theme/_manager.py` & `pginter-0.2.2/src/pginter/theme/_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/theme/themes/default.json` & `pginter-0.2.2/src/pginter/theme/themes/default.json`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/types/_color.py` & `pginter-0.2.2/src/pginter/types/_color.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/types/_scheme.py` & `pginter-0.2.2/src/pginter/types/_scheme.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/types/_style.py` & `pginter-0.2.2/src/pginter/types/_style.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/types/_tk_vars.py` & `pginter-0.2.2/src/pginter/types/_tk_vars.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/utils/_funcs.py` & `pginter-0.2.2/src/pginter/utils/_funcs.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/widgets/_button.py` & `pginter-0.2.2/src/pginter/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/widgets/_entry.py` & `pginter-0.2.2/src/pginter/widgets/_entry.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/widgets/_frame.py` & `pginter-0.2.2/src/pginter/widgets/_frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -474,14 +474,41 @@
         else:
             self.unset_width()
 
         width, height = self.get_size()
 
         # check if the frame even exists
         if width <= 0 or height <= 0:
+            # since the image doesn't affect the calculate_size function,
+            # try to set the frames size through this piece of sh- code
+            if self._image is not ...:
+                width, height = self.get_size()
+                image_width, image_height = self._image.size
+
+                # try to reserve aspect angle
+                if width <= 0 < height:
+                    width = int((image_width / image_height) * height)
+
+                if height <= 0 < width:
+                    height = int((image_height / image_width) * width)
+
+                # if no with or height has yet been set, clone the
+                # original image's size
+                if width <= 0:
+                    width = image_width
+
+                if height <= 0:
+                    height = image_height
+
+                if width > self._width:
+                    self.width = width
+
+                if height > self._height:
+                    self.height = height
+
             return
 
         _surface = pg.Surface((width, height), pg.SRCALPHA)
 
         # draw the frame
         r_rect = pg.Rect((0, 0, width, height))
 
@@ -496,28 +523,37 @@
         )
 
         if self._image is not ...:
             width, height = self.get_size()
             image_width, image_height = self._image.size
 
             # try to reserve aspect angle
+            if hasattr(self, "debug_this"):
+                print("size: ", width, height)
+
             if width <= 0 < height:
                 width = int((image_width / image_height) * height)
 
             if height <= 0 < width:
                 height = int((image_height / image_width) * width)
 
             # if no with or height has yet been set, clone the
             # original image's size
             if width <= 0:
                 width = image_width
 
             if height <= 0:
                 height = image_height
 
+            if width >= self._width:
+                self.width = width
+
+            if height >= self._height:
+                self.height = height
+
             # center image
             pos = (
                 self.assigned_width / 2 - width / 2,
                 self.assigned_height / 2 - height / 2
             )
 
             pos = (
@@ -547,14 +583,15 @@
             child.draw(_surface)
 
         # draw children to surface
         surface.blit(_surface, (self._x, self._y))
 
         # draw wireframe
         if self.show_wireframe:
+            # font for debugging
             font = pg.font.SysFont(None, 20)
             t = font.render(self.__class__.__name__, True, (255, 0, 0))
             surface.blit(t, (self._x, self._y - t.get_height()))
 
             if self._last_rows is not ...:
                 for row in self._last_rows:
                     pg.draw.line(
@@ -581,26 +618,28 @@
                     pg.draw.line(
                         surface,
                         (255, 0, 0, 100),
                         (self._x + column["x_start"] + column["width"], self._y),
                         (self._x + column["x_start"] + column["width"], self._y + height)
                     )
 
+            # draw a different colored rectangle around the frame
             is_debug = hasattr(self, "debug_this")
             col = (255, 255 * (not is_debug), 255 * is_debug)
             pg.draw.rect(
                 surface,
                 col,
                 pg.Rect(
                     (self._x, self._y),
                     (width, height)
                 ),
                 1
             )
 
+            # display width if debug_this is enabled
             if is_debug:
                 w_text = font.render(str(width), True, col)
                 surface.blit(
                     w_text,
                     (
                         (self._x + width / 2) - w_text.get_width() / 2,
                         self._y
```

### Comparing `pginter-0.2.1/src/pginter/widgets/_geo_manager.py` & `pginter-0.2.2/src/pginter/widgets/_geo_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/widgets/_label.py` & `pginter-0.2.2/src/pginter/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter/widgets/_surface_frame.py` & `pginter-0.2.2/src/pginter/widgets/_surface_frame.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.1/src/pginter.egg-info/SOURCES.txt` & `pginter-0.2.2/src/pginter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

