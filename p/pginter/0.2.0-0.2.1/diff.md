# Comparing `tmp/pginter-0.2.0.tar.gz` & `tmp/pginter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pginter-0.2.0.tar", last modified: Wed May 31 11:58:06 2023, max compression
+gzip compressed data, was "pginter-0.2.1.tar", last modified: Wed May 31 20:32:00 2023, max compression
```

## Comparing `pginter-0.2.0.tar` & `pginter-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.106671 pginter-0.2.0/
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.0/LICENSE
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       53 2023-02-10 14:14:25.000000 pginter-0.2.0/MANIFEST.in
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-05-31 11:58:06.106671 pginter-0.2.0/PKG-INFO
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.0/README.md
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.0/pyproject.toml
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-05-31 11:58:06.106671 pginter-0.2.0/setup.cfg
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      936 2023-05-24 18:38:46.000000 pginter-0.2.0/setup.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.093338 pginter-0.2.0/src/
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.096671 pginter-0.2.0/src/pginter/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.0/src/pginter/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20454 2023-05-25 15:22:29.000000 pginter-0.2.0/src/pginter/_pg_root.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.0/src/pginter/icon.png
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.100005 pginter-0.2.0/src/pginter/theme/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.0/src/pginter/theme/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.0/src/pginter/theme/_manager.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.103338 pginter-0.2.0/src/pginter/types/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.0/src/pginter/types/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.0/src/pginter/types/_better_dict.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.0/src/pginter/types/_binds.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.0/src/pginter/types/_color.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.0/src/pginter/types/_constants.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.0/src/pginter/types/_geo_types.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.0/src/pginter/types/_notifications.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.0/src/pginter/types/_scheme.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.0/src/pginter/types/_style.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.0/src/pginter/types/_tk_vars.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.103338 pginter-0.2.0/src/pginter/utils/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       49 2023-05-14 20:09:36.000000 pginter-0.2.0/src/pginter/utils/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      872 2023-05-25 23:31:06.000000 pginter-0.2.0/src/pginter/utils/_funcs.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.106671 pginter-0.2.0/src/pginter/widgets/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.0/src/pginter/widgets/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.0/src/pginter/widgets/_button.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.0/src/pginter/widgets/_entry.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    22121 2023-05-25 23:31:06.000000 pginter-0.2.0/src/pginter/widgets/_frame.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    23874 2023-05-25 23:31:06.000000 pginter-0.2.0/src/pginter/widgets/_geo_manager.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.0/src/pginter/widgets/_label.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.0/src/pginter/widgets/_supports_children.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.0/src/pginter/widgets/_surface_frame.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.100005 pginter-0.2.0/src/pginter.egg-info/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-05-31 11:58:06.000000 pginter-0.2.0/src/pginter.egg-info/PKG-INFO
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      956 2023-05-31 11:58:06.000000 pginter-0.2.0/src/pginter.egg-info/SOURCES.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-05-31 11:58:06.000000 pginter-0.2.0/src/pginter.egg-info/dependency_links.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-05-31 11:58:06.000000 pginter-0.2.0/src/pginter.egg-info/top_level.txt
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.423661 pginter-0.2.1/
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.1/LICENSE
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.1/MANIFEST.in
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-05-31 20:32:00.420327 pginter-0.2.1/PKG-INFO
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.1/README.md
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.1/pyproject.toml
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-05-31 20:32:00.423661 pginter-0.2.1/setup.cfg
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      936 2023-05-31 20:31:44.000000 pginter-0.2.1/setup.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.413661 pginter-0.2.1/src/
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.416994 pginter-0.2.1/src/pginter/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.1/src/pginter/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20488 2023-05-31 20:25:21.000000 pginter-0.2.1/src/pginter/_pg_root.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.1/src/pginter/icon.png
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.416994 pginter-0.2.1/src/pginter/theme/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.1/src/pginter/theme/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.1/src/pginter/theme/_manager.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.416994 pginter-0.2.1/src/pginter/theme/themes/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      663 2023-05-25 20:39:17.000000 pginter-0.2.1/src/pginter/theme/themes/default.json
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.420327 pginter-0.2.1/src/pginter/types/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.1/src/pginter/types/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.1/src/pginter/types/_better_dict.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.1/src/pginter/types/_binds.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.1/src/pginter/types/_color.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.1/src/pginter/types/_constants.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.1/src/pginter/types/_geo_types.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.1/src/pginter/types/_notifications.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.1/src/pginter/types/_scheme.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.1/src/pginter/types/_style.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.1/src/pginter/types/_tk_vars.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.420327 pginter-0.2.1/src/pginter/utils/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       49 2023-05-14 20:09:36.000000 pginter-0.2.1/src/pginter/utils/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      872 2023-05-25 23:31:06.000000 pginter-0.2.1/src/pginter/utils/_funcs.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.420327 pginter-0.2.1/src/pginter/widgets/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.1/src/pginter/widgets/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.1/src/pginter/widgets/_button.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.1/src/pginter/widgets/_entry.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    25138 2023-05-31 20:14:13.000000 pginter-0.2.1/src/pginter/widgets/_frame.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-05-31 20:24:58.000000 pginter-0.2.1/src/pginter/widgets/_geo_manager.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.1/src/pginter/widgets/_label.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.1/src/pginter/widgets/_supports_children.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.1/src/pginter/widgets/_surface_frame.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 20:32:00.416994 pginter-0.2.1/src/pginter.egg-info/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-05-31 20:32:00.000000 pginter-0.2.1/src/pginter.egg-info/PKG-INFO
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      994 2023-05-31 20:32:00.000000 pginter-0.2.1/src/pginter.egg-info/SOURCES.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-05-31 20:32:00.000000 pginter-0.2.1/src/pginter.egg-info/dependency_links.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-05-31 20:32:00.000000 pginter-0.2.1/src/pginter.egg-info/top_level.txt
```

### Comparing `pginter-0.2.0/LICENSE` & `pginter-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pginter-0.2.0/setup.py` & `pginter-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pginter",
-    version="0.2.0",
+    version="0.2.1",
     author="Nilusink",
     author_email="nilusink@protonmail.com",
     description="A python GUI interface, based on pygame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nilusink/PgInter",
     # project_urls={
```

### Comparing `pginter-0.2.0/src/pginter/_pg_root.py` & `pginter-0.2.1/src/pginter/_pg_root.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     _mouse_pos: tuple[int, int] = ...
     _max_framerate: int = ...
 
     __timeouts: list[_TimeoutCandidate]
     _last_it_call: float
     _tpool: Pool
 
+    show_wireframe: bool = False
+
     def __init__(
             self,
             title: str = ...,
             icon_path: str = ...,
             size: tuple[int, int] = ...,
             bg_color: Color = ...,
             padding: int = 0,
```

### Comparing `pginter-0.2.0/src/pginter/icon.png` & `pginter-0.2.1/src/pginter/icon.png`

 * *Files identical despite different names*

### Comparing `pginter-0.2.0/src/pginter/theme/_manager.py` & `pginter-0.2.1/src/pginter/theme/_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.0/src/pginter/types/_color.py` & `pginter-0.2.1/src/pginter/types/_color.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.0/src/pginter/types/_scheme.py` & `pginter-0.2.1/src/pginter/types/_scheme.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.0/src/pginter/types/_style.py` & `pginter-0.2.1/src/pginter/types/_style.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.0/src/pginter/types/_tk_vars.py` & `pginter-0.2.1/src/pginter/types/_tk_vars.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.0/src/pginter/utils/_funcs.py` & `pginter-0.2.1/src/pginter/utils/_funcs.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.0/src/pginter/widgets/_button.py` & `pginter-0.2.1/src/pginter/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.0/src/pginter/widgets/_entry.py` & `pginter-0.2.1/src/pginter/widgets/_entry.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.0/src/pginter/widgets/_frame.py` & `pginter-0.2.1/src/pginter/widgets/_frame.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,23 +48,23 @@
     for init, config in replaces:
         if key == init:
             return config
 
     return key
 
 
-def pi_image_to_surface(pil_image):
+def pil_image_to_surface(pil_image):
     """
     helper function for converting pillow images to pygame images
     """
     return pg.image.fromstring(
         pil_image.tobytes(),
         pil_image.size,
         pil_image.mode
-    ).convert()
+    ).convert_alpha()
 
 
 class _Bind(tp.TypedDict):
     id: int
     event: FrameBind
     function: tp.Callable[[tp.Any], tp.Any | None]
 
@@ -80,14 +80,16 @@
     hover_style: Style = ...
     active_style: Style = ...
     _x: int = -1
     _y: int = -1
 
     _image: Image.Image
 
+    show_wireframe: bool = False
+
     def __init__(
             self,
             parent: tp.Union["Frame", tp.Any],
             width: int = ...,
             height: int = ...,
             bg: Color = ...,
             layout: Layout = Layout.Absolute,
@@ -117,14 +119,17 @@
         :param width: width of the frame
         :param height: height of the frame
         :param bg: background color of the frame
         :param border_radius: border radius of the box (all four corners)
         :param border_width: how thick the border of the box should be
         :param border_color: the color of the border
         """
+        # inherit show_wireframe from parent
+        self.show_wireframe = parent.show_wireframe
+
         if image is not ... and not PIL_EXISTS:
             raise ImportError(
                 "PIL needs to be installed to use the Image widget.\n"
                 "\tto install PIL, use\n"
                 "\t\t\"pip install pillow\""
             )
 
@@ -212,14 +217,34 @@
         # arguments
         if width is not ... and self.style.width is ...:
             self.style.width = width
 
         if height is not ... and self.style.height is ...:
             self.style.height = height
 
+        # assign to properties (for geo-manager)
+        if self.style.width is not ...:
+            self.width = self.style.width
+
+        if self.style.height is not ...:
+            self.height = self.style.height
+
+        # link the style parameters to the geo-manager properties
+        def update_width(*_):
+            if self.style.width is not ...:
+                self.width = self.style.width
+
+        def update_height(*_):
+            if self.style.height is not ...:
+                self.height = self.style.height
+
+        self.style.notify_on("width", update_width)
+        self.style.notify_on("height", update_height)
+
+        # more arguments
         if self.style.backgroundColor is ...:
             self.style.backgroundColor = self.theme.frame.bg1 if bg is ... else bg
             if isinstance(self.__parent, Frame) and \
                     self.__parent.style.backgroundColor == self.theme.frame.bg1:
                 self.style.backgroundColor = self.theme.frame.bg2 if bg is ... else bg
 
         if border_width is not ... and self.style.borderWidth == 0:
@@ -495,15 +520,15 @@
                 self.assigned_height / 2 - height / 2
             )
 
             pos = (
                 pos[0] if pos[0] >= 0 else 0,
                 pos[1] if pos[1] >= 0 else 0
             )
-            now_image = pi_image_to_surface(
+            now_image = pil_image_to_surface(
                 self._image.resize((width, height))
             )
             _surface.blit(now_image, pos)
 
         if current_style.borderWidth > 0:
             # print(f"drawing border, {current_style.borderColor}")
             pg.draw.rect(
@@ -517,17 +542,75 @@
                 border_bottom_right_radius=current_style.borderBottomRightRadius
             )
 
         # draw children
         for child, params in self._child_params:
             child.draw(_surface)
 
-        # draw
+        # draw children to surface
         surface.blit(_surface, (self._x, self._y))
 
+        # draw wireframe
+        if self.show_wireframe:
+            font = pg.font.SysFont(None, 20)
+            t = font.render(self.__class__.__name__, True, (255, 0, 0))
+            surface.blit(t, (self._x, self._y - t.get_height()))
+
+            if self._last_rows is not ...:
+                for row in self._last_rows:
+                    pg.draw.line(
+                        surface,
+                        (255, 0, 0, 100),
+                        (self._x, self._y + row["y_start"]),
+                        (self._x + width, self._y + row["y_start"])
+                    )
+                    pg.draw.line(
+                        surface,
+                        (255, 0, 0, 100),
+                        (self._x, self._y + row["y_start"] + row["height"]),
+                        (self._x + width, self._y + row["y_start"] + row["height"])
+                    )
+
+            if self._last_columns is not ...:
+                for column in self._last_columns:
+                    pg.draw.line(
+                        surface,
+                        (255, 0, 0, 100),
+                        (self._x + column["x_start"], self._y),
+                        (self._x + column["x_start"], self._y + height)
+                    )
+                    pg.draw.line(
+                        surface,
+                        (255, 0, 0, 100),
+                        (self._x + column["x_start"] + column["width"], self._y),
+                        (self._x + column["x_start"] + column["width"], self._y + height)
+                    )
+
+            is_debug = hasattr(self, "debug_this")
+            col = (255, 255 * (not is_debug), 255 * is_debug)
+            pg.draw.rect(
+                surface,
+                col,
+                pg.Rect(
+                    (self._x, self._y),
+                    (width, height)
+                ),
+                1
+            )
+
+            if is_debug:
+                w_text = font.render(str(width), True, col)
+                surface.blit(
+                    w_text,
+                    (
+                        (self._x + width / 2) - w_text.get_width() / 2,
+                        self._y
+                    )
+                )
+
     def place(
             self,
             x: int,
             y: int,
     ) -> None:
         """
         place the frame in a parent container
```

### Comparing `pginter-0.2.0/src/pginter/widgets/_geo_manager.py` & `pginter-0.2.1/src/pginter/widgets/_geo_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,14 +35,23 @@
     layout_params: BetterDict = ...
     _grid_params: BetterDict = ...
 
     _child_override: bool = False
     _is_active: bool = False
     _is_hover: bool = False
 
+    _last_rows: list[dict[
+        str,
+        list[tuple[tp.Any, BetterDict, bool]] | float
+    ]] = ...
+    _last_columns: list[dict[
+        str,
+        list[tuple[tp.Any, BetterDict, bool]] | float
+    ]] = ...
+
     def __init__(
             self,
             layout: Layout = ...,
             margin: int = 0,
             padding: int = 0
     ):
         super().__init__()
@@ -400,18 +409,24 @@
                 # add margin
                 total_x += self.layout_params.margin * 2
                 total_y += self.layout_params.margin * 2
 
                 if not self._width_configured:
                     self._width = total_x
 
+                    if hasattr(self, "debug_this"):
+                        print("setting width: ", total_x)
+
                 else:
                     total_x = self._width
     
                 if not self._height_configured:
+                    if hasattr(self, "debug_this"):
+                        print("setting height: ", total_y)
+
                     self._height = total_y
 
                 else:
                     total_y = self.height
 
                 # tell the children where they should be
                 y_cen = total_y / 2
@@ -563,40 +578,59 @@
                         # split size between columns
                         x /= params.columnspan
 
                         if x > columns[c]["max_size"]:
                             columns[c]["max_size"] = x
 
                 # calculate the container size
-                width, height = self.assigned_width, self.assigned_height
+                columns_width, rows_height = self.assigned_width, self.assigned_height
 
                 # only subtract rows that don't have a weight
                 min_width = sum([c["max_size"] for c in columns])
                 min_height = sum([r["max_size"] for r in rows])
 
+                # if children exist, set min size
                 if len(columns) + len(rows) > 0:
-                    if width == 0 or height == 0 and not\
+                    if columns_width == 0 or rows_height == 0 and not\
                             self._width_configured:
-                        self._width = min_width
 
-                    if width == 0 or height == 0 and not\
-                            self._height_configured:
-                        self._height = min_height
+                        # only set if child requires greater width
+                        if min_width > self._width:
+                            if hasattr(self, "debug_this"):
+                                print(
+                                    "setting width (children min): ", min_width
+                                    )
+                            self._width = min_width
 
+                    if columns_width == 0\
+                            or rows_height == 0\
+                            and not self._height_configured:
+
+                        # only set if child requires greater height
+                        if min_height > self._height:
+                            if hasattr(self, "debug_this"):
+                                print(
+                                    "setting height (children min): ",
+                                    min_height
+                                    )
+                            self._height = min_height
+
+                # if a size has been set by the user, overwrite the calculated
+                # size
                 if self._width_configured:
-                    width = self._width
+                    columns_width = self._width
 
                 if self._height_configured:
-                    height = self.height
+                    rows_height = self.height
 
                 # assign extra space
-                extra_width = width - sum(
+                extra_width = columns_width - sum(
                     [c["max_size"] for c in columns if c["weight"] == 0]
                 )
-                extra_height = height - sum(
+                extra_height = rows_height - sum(
                     [r["max_size"] for r in rows if r["weight"] == 0]
                 )
 
                 total_row_weight = sum(
                     [row["weight"] for row in rows]
                 )
                 total_column_weight = sum(
@@ -608,89 +642,116 @@
                     if total_row_weight == 0:
                         rows[r]["height"] = 0
 
                     else:
                         # assign either the minimum size or the
                         # calculated dynamic one
                         w_size = (
-                                (rows[r]["weight"] / total_row_weight)
-                                * extra_height
+                            (rows[r]["weight"] / total_row_weight)
+                            * extra_height
                         ).__floor__()
                         rows[r]["height"] = w_size
 
                     rows[r]["y_start"] = self.layout_params.padding / 2 + sum(
                         [prev_row["height"] for prev_row in rows[:r]]
                     )
 
-                    for c in range(len(columns)):
-                        if total_column_weight == 0:
-                            columns[c]["width"] = 0
+                for c in range(len(columns)):
+                    if total_column_weight == 0:
+                        columns[c]["width"] = 0
 
-                        else:
-                            # assign either the minimum size or the
-                            # calculated dynamic one
-                            w_size = (
-                                    (
-                                            columns[c]["weight"]
-                                            / total_column_weight
-                                    )
-                                    * extra_width
-                            ).__floor__()
-                            columns[c]["width"] = w_size
-
-                        columns[c]["x_start"] = self.layout_params.padding / 2\
-                            + sum(
-                            [prev_col["width"] for prev_col in columns[:c]]
-                        )
+                    else:
+                        # assign either the minimum size or the
+                        # calculated dynamic one
+                        w_size = (
+                            (
+                                columns[c]["weight"]
+                                / total_column_weight
+                            )
+                            * extra_width
+                        ).__floor__()
+                        columns[c]["width"] = w_size
+
+                    columns[c]["x_start"] = self.layout_params.padding / 2\
+                        + sum(
+                        [prev_col["width"] for prev_col in columns[:c]]
+                    )
+
+                if hasattr(self, "debug_this"):
+                    print(self.width, extra_width, min_width)
+                    print([f"width: {c['width']}" for c in columns])
 
                 # place children
                 for child, params in self._child_params:
                     # place the child proportional to the table and stickiness
                     # size = list(child.calculate_size())
                     size = [child._width, child._height]
 
                     row, column = params.row, params.column
                     sticky = params.sticky
                     margin = params.margin
 
-                    width = sum([
+                    columns_width = sum([
                         columns[c]["width"] for c in
                         range(column, column + params.columnspan)
                     ])
-                    height = sum([
+                    rows_height = sum([
                         rows[r]["height"] for r in
                         range(row, row + params.rowspan)
                     ])
 
                     x = columns[column]["x_start"]
                     y = rows[row]["y_start"]
 
-                    x_diff = width - size[0]
-                    y_diff = height - size[1]
+                    x_diff = columns_width - size[0]
+                    y_diff = rows_height - size[1]
+
+                    # offsets for width / height configured
+                    x_position_offset = 0
+                    y_position_offset = 0
+
+                    if hasattr(self, "debug_this"):
+                        print("cw: ", columns_width, params.columnspan)
 
                     # assign stickiness
                     if not child._width_configured:
                         if "w" in sticky:
                             size[0] += (x_diff / 2) - params.margin
 
                         if "e" in sticky:
                             size[0] += (x_diff / 2) - params.margin
 
                         child.assigned_width = size[0]
 
+                    else:
+                        # if width is configured, center the widget based
+                        # on its configured width
+                        x_position_offset += x_diff / 2 - params.margin
+
                     if not child._height_configured:
                         if "n" in sticky:
                             size[1] += (y_diff / 2) - params.margin
 
                         if "s" in sticky:
                             size[1] += (y_diff / 2) - params.margin
 
                         child.assigned_height = size[1]
 
-                    child.set_position(x + margin, y + margin)
+                    else:
+                        # if height is configured, center the widget based
+                        # on its configured height
+                        y_position_offset += y_diff / 2 - params.margin
+
+                    child.set_position(
+                        x + margin + max([x_position_offset, 0]),
+                        y + margin + max([y_position_offset, 0])
+                    )
+
+                self._last_rows = rows
+                self._last_columns = columns
 
             case _:
                 raise ValueError(f"Invalid geometry type: {self._layout}")
 
     def calculate_size(self) -> tuple[int, int]:
         """
         calculate how big the container should be
```

### Comparing `pginter-0.2.0/src/pginter/widgets/_label.py` & `pginter-0.2.1/src/pginter/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.0/src/pginter/widgets/_surface_frame.py` & `pginter-0.2.1/src/pginter/widgets/_surface_frame.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.0/src/pginter.egg-info/SOURCES.txt` & `pginter-0.2.1/src/pginter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/pginter/icon.png
 src/pginter.egg-info/PKG-INFO
 src/pginter.egg-info/SOURCES.txt
 src/pginter.egg-info/dependency_links.txt
 src/pginter.egg-info/top_level.txt
 src/pginter/theme/__init__.py
 src/pginter/theme/_manager.py
+src/pginter/theme/themes/default.json
 src/pginter/types/__init__.py
 src/pginter/types/_better_dict.py
 src/pginter/types/_binds.py
 src/pginter/types/_color.py
 src/pginter/types/_constants.py
 src/pginter/types/_geo_types.py
 src/pginter/types/_notifications.py
```

